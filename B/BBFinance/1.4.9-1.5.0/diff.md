# Comparing `tmp/BBFinance-1.4.9.tar.gz` & `tmp/BBFinance-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BBFinance-1.4.9.tar", last modified: Tue Apr 18 13:17:08 2023, max compression
+gzip compressed data, was "BBFinance-1.5.0.tar", last modified: Tue Apr 18 13:25:01 2023, max compression
```

## Comparing `BBFinance-1.4.9.tar` & `BBFinance-1.5.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:46.182278 BBFinance-1.4.9/
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:37.633333 BBFinance-1.4.9/BBFdocs/
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:38.587886 BBFinance-1.4.9/BBFdocs/docs/
--rw-rw-rw-   0        0        0     4250 2023-04-11 14:25:22.000000 BBFinance-1.4.9/BBFdocs/docs/index.md
--rw-rw-rw-   0        0        0       84 2023-04-10 19:53:10.000000 BBFinance-1.4.9/BBFdocs/mkdocs.yml
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:38.759779 BBFinance-1.4.9/BBFdocs/site/
--rw-rw-rw-   0        0        0     6094 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/404.html
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:39.228566 BBFinance-1.4.9/BBFdocs/site/css/
--rw-rw-rw-   0        0        0     5635 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/css/base.css
--rw-rw-rw-   0        0        0     3487 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/css/base.min.css
--rw-rw-rw-   0        0        0   132465 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/css/bootstrap-custom.css
--rw-rw-rw-   0        0        0   109468 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/css/bootstrap-custom.min.css
--rw-rw-rw-   0        0        0     2131 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/css/cinder.css
--rw-rw-rw-   0        0        0     1637 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/css/cinder.min.css
--rw-rw-rw-   0        0        0     1148 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/css/highlight.css
--rw-rw-rw-   0        0        0      866 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/css/highlight.min.css
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:40.884956 BBFinance-1.4.9/BBFdocs/site/fonts/
--rw-rw-rw-   0        0        0    38205 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   202148 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0    80652 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    44432 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/fonts/fontawesome-webfont.woff
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:42.869496 BBFinance-1.4.9/BBFdocs/site/img/
--rw-rw-rw-   0        0        0     1150 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/img/favicon.ico
--rw-rw-rw-   0        0        0      251 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/img/grid1.png
--rw-rw-rw-   0        0        0      495 2023-04-10 19:54:23.000000 BBFinance-1.4.9/BBFdocs/site/img/grid10.png
--rw-rw-rw-   0        0        0      253 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid11.png
--rw-rw-rw-   0        0        0      260 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid12.png
--rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid13.png
--rw-rw-rw-   0        0        0      240 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid14.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid15.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid16.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid17.png
--rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid18.png
--rw-rw-rw-   0        0        0      427 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid19.png
--rw-rw-rw-   0        0        0      271 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid2.png
--rw-rw-rw-   0        0        0      493 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid20.png
--rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid3.png
--rw-rw-rw-   0        0        0      244 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid4.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid5.png
--rw-rw-rw-   0        0        0      460 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid6.png
--rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid7.png
--rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid8.png
--rw-rw-rw-   0        0        0      456 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/img/grid9.png
--rw-rw-rw-   0        0        0    11272 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/index.html
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:43.103898 BBFinance-1.4.9/BBFdocs/site/js/
--rw-rw-rw-   0        0        0     5911 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/js/base.js
--rw-rw-rw-   0        0        0    27822 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/js/bootstrap-3.0.3.min.js
--rw-rw-rw-   0        0        0    54608 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/js/highlight.pack.js
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:43.510182 BBFinance-1.4.9/BBFdocs/site/search/
--rw-rw-rw-   0        0        0    99805 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/search/lunr.js
--rw-rw-rw-   0        0        0     3206 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/search/main.js
--rw-rw-rw-   0        0        0     9063 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/search/search_index.json
--rw-rw-rw-   0        0        0     3724 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/search/worker.js
--rw-rw-rw-   0        0        0      234 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/sitemap.xml
--rw-rw-rw-   0        0        0      189 2023-04-10 19:54:24.000000 BBFinance-1.4.9/BBFdocs/site/sitemap.xml.gz
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:43.650820 BBFinance-1.4.9/BBFinance/
--rw-rw-rw-   0        0        0    43578 2023-04-18 13:18:41.000000 BBFinance-1.4.9/BBFinance/BBFinance.py
--rw-rw-rw-   0        0        0      340 2023-04-17 19:24:24.000000 BBFinance-1.4.9/BBFinance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:44.182114 BBFinance-1.4.9/BBFinance/__pycache__/
--rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.4.9/BBFinance/__pycache__/BBFinance.cpython-311.pyc
--rw-rw-rw-   0        0        0    26949 2023-04-18 13:13:11.000000 BBFinance-1.4.9/BBFinance/__pycache__/BBFinance.cpython-39.pyc
--rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.4.9/BBFinance/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      446 2023-04-18 13:13:11.000000 BBFinance-1.4.9/BBFinance/__pycache__/__init__.cpython-39.pyc
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:44.072725 BBFinance-1.4.9/BBFinance.egg-info/
--rw-rw-rw-   0        0        0     5070 2023-04-18 13:20:19.000000 BBFinance-1.4.9/BBFinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1917 2023-04-18 13:20:35.000000 BBFinance-1.4.9/BBFinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 13:20:19.000000 BBFinance-1.4.9/BBFinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      283 2023-04-18 13:20:19.000000 BBFinance-1.4.9/BBFinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-18 13:20:19.000000 BBFinance-1.4.9/BBFinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      589 2023-04-10 16:16:08.000000 BBFinance-1.4.9/LICENSE.txt
--rw-rw-rw-   0        0        0     5070 2023-04-18 13:20:46.197908 BBFinance-1.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     4445 2023-04-11 17:27:42.000000 BBFinance-1.4.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:45.229077 BBFinance-1.4.9/__pycache__/
--rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.4.9/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.4.9/__pycache__/main.cpython-39.pyc
--rw-rw-rw-   0        0        0     8192 2023-04-17 18:28:14.000000 BBFinance-1.4.9/bases.db
-drwxrwxrwx   0        0        0        0 2023-04-18 13:20:45.682236 BBFinance-1.4.9/docs/
--rw-rw-rw-   0        0        0       17 2023-04-11 17:09:57.000000 BBFinance-1.4.9/docs/CNAME
--rw-rw-rw-   0        0        0     1354 2023-04-11 15:11:55.000000 BBFinance-1.4.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 13:20:46.213536 BBFinance-1.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1364 2023-04-18 13:19:10.000000 BBFinance-1.4.9/setup.py
--rw-rw-rw-   0        0        0       30 2023-04-18 13:00:07.000000 BBFinance-1.4.9/teste.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:39.549526 BBFinance-1.5.0/
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:32.297386 BBFinance-1.5.0/BBFdocs/
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:32.391150 BBFinance-1.5.0/BBFdocs/docs/
+-rw-rw-rw-   0        0        0     4250 2023-04-11 14:25:22.000000 BBFinance-1.5.0/BBFdocs/docs/index.md
+-rw-rw-rw-   0        0        0       84 2023-04-10 19:53:10.000000 BBFinance-1.5.0/BBFdocs/mkdocs.yml
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:32.844334 BBFinance-1.5.0/BBFdocs/site/
+-rw-rw-rw-   0        0        0     6094 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/404.html
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:34.594476 BBFinance-1.5.0/BBFdocs/site/css/
+-rw-rw-rw-   0        0        0     5635 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/css/base.css
+-rw-rw-rw-   0        0        0     3487 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/css/base.min.css
+-rw-rw-rw-   0        0        0   132465 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/css/bootstrap-custom.css
+-rw-rw-rw-   0        0        0   109468 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/css/bootstrap-custom.min.css
+-rw-rw-rw-   0        0        0     2131 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/css/cinder.css
+-rw-rw-rw-   0        0        0     1637 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/css/cinder.min.css
+-rw-rw-rw-   0        0        0     1148 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/css/highlight.css
+-rw-rw-rw-   0        0        0      866 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/css/highlight.min.css
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:34.844505 BBFinance-1.5.0/BBFdocs/site/fonts/
+-rw-rw-rw-   0        0        0    38205 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   202148 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0    80652 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    44432 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/fonts/fontawesome-webfont.woff
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:37.719794 BBFinance-1.5.0/BBFdocs/site/img/
+-rw-rw-rw-   0        0        0     1150 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/img/favicon.ico
+-rw-rw-rw-   0        0        0      251 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/img/grid1.png
+-rw-rw-rw-   0        0        0      495 2023-04-10 19:54:23.000000 BBFinance-1.5.0/BBFdocs/site/img/grid10.png
+-rw-rw-rw-   0        0        0      253 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid11.png
+-rw-rw-rw-   0        0        0      260 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid12.png
+-rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid13.png
+-rw-rw-rw-   0        0        0      240 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid14.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid15.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid16.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid17.png
+-rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid18.png
+-rw-rw-rw-   0        0        0      427 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid19.png
+-rw-rw-rw-   0        0        0      271 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid2.png
+-rw-rw-rw-   0        0        0      493 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid20.png
+-rw-rw-rw-   0        0        0      266 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid3.png
+-rw-rw-rw-   0        0        0      244 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid4.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid5.png
+-rw-rw-rw-   0        0        0      460 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid6.png
+-rw-rw-rw-   0        0        0      442 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid7.png
+-rw-rw-rw-   0        0        0      457 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid8.png
+-rw-rw-rw-   0        0        0      456 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/img/grid9.png
+-rw-rw-rw-   0        0        0    11272 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/index.html
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:37.971252 BBFinance-1.5.0/BBFdocs/site/js/
+-rw-rw-rw-   0        0        0     5911 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/js/base.js
+-rw-rw-rw-   0        0        0    27822 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/js/bootstrap-3.0.3.min.js
+-rw-rw-rw-   0        0        0    54608 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/js/highlight.pack.js
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:38.315028 BBFinance-1.5.0/BBFdocs/site/search/
+-rw-rw-rw-   0        0        0    99805 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/search/lunr.js
+-rw-rw-rw-   0        0        0     3206 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/search/main.js
+-rw-rw-rw-   0        0        0     9063 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/search/search_index.json
+-rw-rw-rw-   0        0        0     3724 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/search/worker.js
+-rw-rw-rw-   0        0        0      234 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/sitemap.xml
+-rw-rw-rw-   0        0        0      189 2023-04-10 19:54:24.000000 BBFinance-1.5.0/BBFdocs/site/sitemap.xml.gz
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:38.408805 BBFinance-1.5.0/BBFinance/
+-rw-rw-rw-   0        0        0    43532 2023-04-18 13:27:40.000000 BBFinance-1.5.0/BBFinance/BBFinance.py
+-rw-rw-rw-   0        0        0      340 2023-04-17 19:24:24.000000 BBFinance-1.5.0/BBFinance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:38.986969 BBFinance-1.5.0/BBFinance/__pycache__/
+-rw-rw-rw-   0        0        0    36738 2023-04-10 11:52:03.000000 BBFinance-1.5.0/BBFinance/__pycache__/BBFinance.cpython-311.pyc
+-rw-rw-rw-   0        0        0    26960 2023-04-18 13:25:12.000000 BBFinance-1.5.0/BBFinance/__pycache__/BBFinance.cpython-39.pyc
+-rw-rw-rw-   0        0        0      436 2023-04-10 11:52:03.000000 BBFinance-1.5.0/BBFinance/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      446 2023-04-18 13:13:11.000000 BBFinance-1.5.0/BBFinance/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:38.893252 BBFinance-1.5.0/BBFinance.egg-info/
+-rw-rw-rw-   0        0        0     5070 2023-04-18 13:28:17.000000 BBFinance-1.5.0/BBFinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1917 2023-04-18 13:28:30.000000 BBFinance-1.5.0/BBFinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 13:28:17.000000 BBFinance-1.5.0/BBFinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      283 2023-04-18 13:28:17.000000 BBFinance-1.5.0/BBFinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-18 13:28:17.000000 BBFinance-1.5.0/BBFinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      589 2023-04-10 16:16:08.000000 BBFinance-1.5.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5070 2023-04-18 13:28:39.549526 BBFinance-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4445 2023-04-11 17:27:42.000000 BBFinance-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:39.393260 BBFinance-1.5.0/__pycache__/
+-rw-rw-rw-   0        0        0      301 2023-04-05 17:36:13.000000 BBFinance-1.5.0/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8340 2023-04-05 15:20:09.000000 BBFinance-1.5.0/__pycache__/main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8192 2023-04-17 18:28:14.000000 BBFinance-1.5.0/bases.db
+drwxrwxrwx   0        0        0        0 2023-04-18 13:28:39.471392 BBFinance-1.5.0/docs/
+-rw-rw-rw-   0        0        0       17 2023-04-11 17:09:57.000000 BBFinance-1.5.0/docs/CNAME
+-rw-rw-rw-   0        0        0     1354 2023-04-11 15:11:55.000000 BBFinance-1.5.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 13:28:39.565147 BBFinance-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1364 2023-04-18 13:26:52.000000 BBFinance-1.5.0/setup.py
+-rw-rw-rw-   0        0        0       30 2023-04-18 13:00:07.000000 BBFinance-1.5.0/teste.py
```

### Comparing `BBFinance-1.4.9/BBFdocs/docs/index.md` & `BBFinance-1.5.0/BBFdocs/docs/index.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/404.html` & `BBFinance-1.5.0/BBFdocs/site/404.html`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/css/base.css` & `BBFinance-1.5.0/BBFdocs/site/css/base.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/css/base.min.css` & `BBFinance-1.5.0/BBFdocs/site/css/base.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/css/bootstrap-custom.css` & `BBFinance-1.5.0/BBFdocs/site/css/bootstrap-custom.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/css/bootstrap-custom.min.css` & `BBFinance-1.5.0/BBFdocs/site/css/bootstrap-custom.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/css/cinder.css` & `BBFinance-1.5.0/BBFdocs/site/css/cinder.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/css/cinder.min.css` & `BBFinance-1.5.0/BBFdocs/site/css/cinder.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/css/highlight.css` & `BBFinance-1.5.0/BBFdocs/site/css/highlight.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/css/highlight.min.css` & `BBFinance-1.5.0/BBFdocs/site/css/highlight.min.css`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/fonts/fontawesome-webfont.eot` & `BBFinance-1.5.0/BBFdocs/site/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/fonts/fontawesome-webfont.svg` & `BBFinance-1.5.0/BBFdocs/site/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/fonts/fontawesome-webfont.ttf` & `BBFinance-1.5.0/BBFdocs/site/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/fonts/fontawesome-webfont.woff` & `BBFinance-1.5.0/BBFdocs/site/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/img/favicon.ico` & `BBFinance-1.5.0/BBFdocs/site/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/index.html` & `BBFinance-1.5.0/BBFdocs/site/index.html`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/js/base.js` & `BBFinance-1.5.0/BBFdocs/site/js/base.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/js/bootstrap-3.0.3.min.js` & `BBFinance-1.5.0/BBFdocs/site/js/bootstrap-3.0.3.min.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/js/highlight.pack.js` & `BBFinance-1.5.0/BBFdocs/site/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/search/lunr.js` & `BBFinance-1.5.0/BBFdocs/site/search/lunr.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/search/main.js` & `BBFinance-1.5.0/BBFdocs/site/search/main.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/search/search_index.json` & `BBFinance-1.5.0/BBFdocs/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFdocs/site/search/worker.js` & `BBFinance-1.5.0/BBFdocs/site/search/worker.js`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFinance/BBFinance.py` & `BBFinance-1.5.0/BBFinance/BBFinance.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,15 +971,15 @@
 responseHistory = Response(media_type="application/json")
 
 
 
 ## INFORMAÇÕES DE OPÇÕES ##
 
 @app.get("/options/{symbol}/info", response_model=None)
-def get_opc(symbol: str, call: Union[True, False], put: Union[True, False]) -> pd.DataFrame():
+def get_opc(symbol: str, call: bool, put: bool) -> pd.DataFrame():
 
     """
     ## Usabilidade
 
     - Função que apresenta as principais informações das opções do ativo selecionado, informações como: Strike, Var, Gregas, dentre outras.
 
     ## Parâmetros
@@ -1011,15 +1011,14 @@
     dfOPC = dfOPC[0]
     dfOPC = dfOPC[['Ticker', 'Tipo', 'Strike', 'A/I/OTM', 'Dist. (%) do Strike', 'Último', 'Var. (%)', 'Núm. de Neg.', 'Vol. Financeiro', 'Delta', 'Gamma', 'Theta ($)', 'Vega']]
     if call == True:
         dfCall = dfOPC.loc[dfOPC['Tipo'] == 'CALL']
         return dfCall
     elif put == True:
         dfPut = dfOPC.loc[dfOPC['Tipo'] == 'PUT']
-        lala = 1
         return dfPut
     else:
         driver.get(url)
         time.sleep(1.5)
 
         table = driver.find_element(By.CSS_SELECTOR, '#tblListaOpc')
         table_html = table.get_attribute('outerHTML')
```

### Comparing `BBFinance-1.4.9/BBFinance/__pycache__/BBFinance.cpython-311.pyc` & `BBFinance-1.5.0/BBFinance/__pycache__/BBFinance.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/BBFinance/__pycache__/BBFinance.cpython-39.pyc` & `BBFinance-1.5.0/BBFinance/__pycache__/BBFinance.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Apr 18 12:54:56 2023 UTC, .py size: 43566 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 610d 0d0a 0000 0000 2093 3e64 2eaa 0000  a....... .>d....
+00000000: 610d 0d0a 0000 0000 b198 3e64 3aaa 0000  a.........>d:...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 2c06 0000 6400  .....@...s,...d.
+00000020: 0006 0000 0040 0000 0073 3406 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6400 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6407 6c0c 6d0d 5a0d 0100 6400  ..d.d.l.m.Z...d.
 00000080: 6408 6c0e 6d0f 5a0f 0100 6400 6401 6c10  d.l.m.Z...d.d.l.
 00000090: 5a10 6400 6401 6c11 5a11 6400 6409 6c12  Z.d.d.l.Z.d.d.l.
@@ -84,1602 +84,1602 @@
 00000530: 641f 6420 6452 6422 8d04 0100 6517 6423  d.d dRd"....e.d#
 00000540: 6424 8d01 5a40 6535 6a37 6455 6401 6419  d$..Z@e5j7dUd.d.
 00000550: 8d02 6528 6546 6545 6602 1900 6601 6522  ..e(eFeEf...f.e"
 00000560: 6a3e 644f 9c01 6456 6457 8405 8301 5a4f  j>dO..dVdW....ZO
 00000570: 653b 641d 6b02 9005 725e 6520 6a3c 6535  e;d.k...r^e j<e5
 00000580: 641f 6420 6455 6422 8d04 0100 6517 6423  d.d dUd"....e.d#
 00000590: 6424 8d01 5a40 6535 6a37 6458 6401 6419  d$..Z@e5j7dXd.d.
-000005a0: 8d02 6538 6459 6459 6522 a03e a100 645a  ..e8dYdYe".>..dZ
-000005b0: 9c04 645b 645c 8404 8301 5a50 653b 641d  ..d[d\....ZPe;d.
-000005c0: 6b02 9005 72aa 6520 6a3c 6535 641f 6420  k...r.e j<e5d.d 
-000005d0: 6458 6422 8d04 0100 6517 6423 6424 8d01  dXd"....e.d#d$..
-000005e0: 5a40 6535 6a37 645d 6401 6419 8d02 6528  Z@e5j7d]d.d...e(
-000005f0: 645e 1900 6538 6545 6545 6546 6605 6538  d^..e8eEeEeFf.e8
-00000600: 644f 9c01 645f 6460 8405 8301 5a51 653b  dO..d_d`....ZQe;
-00000610: 641d 6b02 9005 72fc 6520 6a3c 6535 641f  d.k...r.e j<e5d.
-00000620: 6420 645d 6422 8d04 0100 6517 6423 6424  d d]d"....e.d#d$
-00000630: 8d01 5a40 6467 6528 6538 6548 6602 1900  ..Z@dge(e8eHf...
-00000640: 6528 6546 6545 6602 1900 6462 9c02 6463  e(eFeEf...db..dc
-00000650: 6464 8405 5a52 6401 5300 2968 e900 0000  dd..ZRd.S.)h....
-00000660: 004e 2901 da04 6e6f 726d 2901 da08 6d69  .N)...norm)...mi
-00000670: 6e69 6d69 7a65 2901 da10 4c69 6e65 6172  nimize)...Linear
-00000680: 5265 6772 6573 7369 6f6e 2901 da09 7765  Regression)...we
-00000690: 6264 7269 7665 7229 01da 044b 6579 7329  bdriver)...Keys)
-000006a0: 01da 074f 7074 696f 6e73 2901 da02 4279  ...Options)...By
-000006b0: 2901 da0d 4265 6175 7469 6675 6c53 6f75  )...BeautifulSou
-000006c0: 7029 03da 0746 6173 7441 5049 da08 5265  p)...FastAPI..Re
-000006d0: 7370 6f6e 7365 da07 5265 7175 6573 7429  sponse..Request)
-000006e0: 01da 0c48 544d 4c52 6573 706f 6e73 6529  ...HTMLResponse)
-000006f0: 01da 0b53 7461 7469 6346 696c 6573 2901  ...StaticFiles).
-00000700: da0f 4a69 6e6a 6132 5465 6d70 6c61 7465  ..Jinja2Template
-00000710: 7329 02da 0864 6174 6574 696d 65da 0974  s)...datetime..t
-00000720: 696d 6564 656c 7461 2901 da05 556e 696f  imedelta)...Unio
-00000730: 6eda 0669 676e 6f72 6569 6d01 0000 2901  n..ignoreim...).
-00000740: da04 6461 7973 e901 0000 00e9 0700 0000  ..days..........
-00000750: 7a08 2559 2d25 6d2d 2564 6302 0000 0000  z.%Y-%m-%dc.....
-00000760: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
-00000770: 0000 0073 5e00 0000 7c00 7c01 1900 6a00  ...s^...|.|...j.
-00000780: 6401 6402 6403 6404 8d03 7c00 7c01 3c00  d.d.d.d...|.|.<.
-00000790: 7c00 7c01 1900 6a00 6405 6402 6403 6404  |.|...j.d.d.d.d.
-000007a0: 8d03 7c00 7c01 3c00 7c00 7c01 1900 6a00  ..|.|.<.|.|...j.
-000007b0: 6406 6407 6403 6404 8d03 7c00 7c01 3c00  d.d.d.d...|.|.<.
-000007c0: 7c00 7c01 1900 a001 7402 a101 7c00 7c01  |.|.....t...|.|.
-000007d0: 3c00 7c00 5300 2908 4e7a 035b 2e5d da00  <.|.S.).Nz.[.]..
-000007e0: 5429 01da 0572 6567 6578 7a03 5b25 5d7a  T)...regexz.[%]z
-000007f0: 035b 2c5d da01 2e29 03da 0772 6570 6c61  .[,]...)...repla
-00000800: 6365 da06 6173 7479 7065 da05 666c 6f61  ce..astype..floa
-00000810: 7429 02da 0264 665a 0a6e 6f6d 6543 6f6c  t)...dfZ.nomeCol
-00000820: 756e 61a9 0072 1e00 0000 fa40 713a 5c52  una..r.....@q:\R
-00000830: 6973 636f 5c4e 6f76 6f20 5269 7363 6f5c  isco\Novo Risco\
-00000840: 7079 7468 6f6e 7269 7363 6f5c 4242 4669  pythonrisco\BBFi
-00000850: 6e61 6e63 655c 4242 4669 6e61 6e63 655c  nance\BBFinance\
-00000860: 4242 4669 6e61 6e63 652e 7079 da14 666f  BBFinance.py..fo
-00000870: 726d 6174 6156 616c 6f72 6573 4e75 6d65  rmataValoresNume
-00000880: 726f 3d00 0000 730a 0000 0000 0118 0118  ro=...s.........
-00000890: 0118 0112 0272 2000 0000 7a15 2f73 746f  .....r ...z./sto
-000008a0: 636b 732f 7b73 796d 626f 6c7d 2f69 6e66  cks/{symbol}/inf
-000008b0: 6f29 015a 0e72 6573 706f 6e73 655f 6d6f  o).Z.response_mo
-000008c0: 6465 6c29 02da 0673 796d 626f 6cda 0672  del)...symbol..r
-000008d0: 6574 7572 6e63 0100 0000 0000 0000 0000  eturnc..........
-000008e0: 0000 0800 0000 0500 0000 4300 0000 7368  ..........C...sh
-000008f0: 0000 0074 00a0 017c 00a1 017d 017c 016a  ...t...|...}.|.j
-00000900: 027d 0274 037c 0283 017d 037c 0374 046b  .}.t.|...}.|.t.k
-00000910: 0272 226e 0874 0564 0183 0101 007c 016a  .r"n.t.d.....|.j
-00000920: 0264 0219 007d 047c 016a 0264 0319 007d  .d...}.|.j.d...}
-00000930: 057c 016a 067d 067c 066a 0764 0464 0585  .|.j.}.|.j.d.d..
-00000940: 0219 00a0 08a1 007d 067c 007c 047c 057c  .......}.|.|.|.|
-00000950: 0664 069c 047d 077c 0753 0029 0775 bf00  .d...}.|.S.).u..
-00000960: 0000 0a20 2020 2023 2320 5573 6162 696c  ...    ## Usabil
-00000970: 6964 6164 6520 0a20 2020 202d 2042 7573  idade .    - Bus
-00000980: 6361 2061 7320 7072 696e 6369 7061 6973  ca as principais
-00000990: 2069 6e66 6f72 6d61 c3a7 6f65 7320 736f   informa..oes so
-000009a0: 6272 6520 6f20 6174 6976 6f20 7365 6c65  bre o ativo sele
-000009b0: 6369 6f6e 6164 6f20 636f 6d6f 2050 7265  cionado como Pre
-000009c0: c3a7 6f20 6520 4469 7669 6465 6e64 6f73  ..o e Dividendos
-000009d0: 200a 0a20 2020 200a 2020 2020 2323 2050   ..    .    ## P
-000009e0: 6172 c3a2 6d65 7472 6f73 0a20 2020 202d  ar..metros.    -
-000009f0: 2073 796d 626f 6c20 2d3e 204e 6f6d 6520   symbol -> Nome 
-00000a00: 646f 2041 7469 766f 2070 6172 6120 6120  do Ativo para a 
-00000a10: 6275 7363 6120 0a0a 2020 2020 0a20 2020  busca ..    .   
-00000a20: 20fa 0f54 6963 6b65 7220 496e 7661 6c69   ..Ticker Invali
-00000a30: 646f da12 7265 6775 6c61 724d 6172 6b65  do..regularMarke
-00000a40: 7450 7269 6365 5a08 6c6f 6e67 4e61 6d65  tPriceZ.longName
-00000a50: e9ff ffff ff4e 2904 7221 0000 00da 0d63  .....N).r!.....c
-00000a60: 7572 7265 6e74 5f70 7269 6365 da0c 636f  urrent_price..co
-00000a70: 6d70 616e 795f 6e61 6d65 da09 6469 7669  mpany_name..divi
-00000a80: 6465 6e64 7329 09da 0279 66da 0654 6963  dends)...yf..Tic
-00000a90: 6b65 72da 0469 6e66 6fda 0474 7970 65da  ker..info..type.
-00000aa0: 0464 6963 74da 0570 7269 6e74 7228 0000  .dict..printr(..
-00000ab0: 00da 0469 6c6f 63da 0373 756d 2908 7221  ...iloc..sum).r!
-00000ac0: 0000 00da 0573 746f 636b 722b 0000 00da  .....stockr+....
-00000ad0: 0874 6970 6f49 6e66 6f72 2600 0000 7227  .tipoInfor&...r'
-00000ae0: 0000 005a 0864 6976 6964 656e 64da 096a  ...Z.dividend..j
-00000af0: 736f 6e5f 6461 7461 721e 0000 0072 1e00  son_datar....r..
-00000b00: 0000 721f 0000 00da 0867 6574 5f69 6e66  ..r......get_inf
-00000b10: 6f46 0000 0073 2000 0000 000c 0a01 0601  oF...s .........
-00000b20: 0801 0801 0202 0802 0a03 0a03 0601 1203  ................
-00000b30: 0201 0201 0201 02fd 0607 7234 0000 00da  ..........r4....
-00000b40: 085f 5f6d 6169 6e5f 5f7a 086d 6169 6e3a  .__main__z.main:
-00000b50: 6170 707a 0931 3237 2e30 2e30 2e31 6940  appz.127.0.0.1i@
-00000b60: 1f00 007a 1473 746f 636b 732f 7b73 796d  ...z.stocks/{sym
-00000b70: 626f 6c7d 2f69 6e66 6f29 03da 0468 6f73  bol}/info)...hos
-00000b80: 74da 0470 6f72 74da 0764 6566 6175 6c74  t..port..default
-00000b90: 7a10 6170 706c 6963 6174 696f 6e2f 6a73  z.application/js
-00000ba0: 6f6e 2901 5a0a 6d65 6469 615f 7479 7065  on).Z.media_type
-00000bb0: 7a18 2f73 746f 636b 732f 7b73 796d 626f  z./stocks/{symbo
-00000bc0: 6c7d 2f68 6973 746f 7279 da02 3179 2903  l}/history..1y).
-00000bd0: 7221 0000 00da 0670 6572 696f 6472 2200  r!.....periodr".
-00000be0: 0000 6302 0000 0000 0000 0000 0000 0008  ..c.............
-00000bf0: 0000 0003 0000 0043 0000 0073 7000 0000  .......C...sp...
-00000c00: 7400 a001 7c00 a101 7d02 7c02 6a02 7d03  t...|...}.|.j.}.
-00000c10: 7403 7c03 8301 7d04 7c04 7404 6b02 7222  t.|...}.|.t.k.r"
-00000c20: 6e08 7405 6401 8301 0100 7c02 6a06 7c01  n.t.d.....|.j.|.
-00000c30: 6402 8d01 7d05 7c05 6a07 7248 6403 7405  d...}.|.j.rHd.t.
-00000c40: 6404 8301 6901 5300 7c05 6a08 6405 6406  d...i.S.|.j.d.d.
-00000c50: 8d01 7d06 7409 6a0a a00b 7c06 a101 6a0c  ..}.t.j...|...j.
-00000c60: 6407 6408 8d01 7d07 7c07 5300 6409 5300  d.d...}.|.S.d.S.
-00000c70: 290a 75ff 0000 000a 2020 2020 2323 2055  ).u.....    ## U
-00000c80: 7361 6269 6c69 6461 6465 200a 2020 2020  sabilidade .    
-00000c90: 2d20 5573 6164 6120 7061 7261 2076 6572  - Usada para ver
-00000ca0: 6966 6963 6172 206f 2068 6973 74c3 b372  ificar o hist..r
-00000cb0: 6963 6f20 6461 2061 c3a7 616f 2073 656c  ico da a..ao sel
-00000cc0: 6563 696f 6e61 6461 2065 2065 6d20 7175  ecionada e em qu
-00000cd0: 616c 2070 6572 696f 646f 200a 0a20 2020  al periodo ..   
-00000ce0: 200a 2020 2020 2323 2050 6172 c3a2 6d65   .    ## Par..me
-00000cf0: 7472 6f73 0a20 2020 200a 2020 2020 2d20  tros.    .    - 
-00000d00: 7379 6d62 6f6c 202d 3e20 4e6f 6d65 2064  symbol -> Nome d
-00000d10: 6f20 4174 6976 6f20 7061 7261 2061 2062  o Ativo para a b
-00000d20: 7573 6361 200a 0a20 2020 202d 2070 6572  usca ..    - per
-00000d30: 696f 6420 2d3e 2044 6174 6120 656d 2041  iod -> Data em A
-00000d40: 4e4f 5320 7061 7261 2061 2062 7573 6361  NOS para a busca
-00000d50: 2064 6173 2069 6e66 6f72 6d61 c3a7 6f65   das informa..oe
-00000d60: 7320 646f 2041 7469 766f 200a 0a20 2020  s do Ativo ..   
-00000d70: 200a 2020 2020 7223 0000 00a9 0172 3a00   .    r#.....r:.
-00000d80: 0000 da05 6572 726f 727a 0d4e 6f20 6461  ....errorz.No da
-00000d90: 7461 2066 6f75 6e64 da04 6c69 7374 2901  ta found..list).
-00000da0: 5a06 6f72 6965 6e74 4629 01da 0464 726f  Z.orientF)...dro
-00000db0: 704e 290d 7229 0000 0072 2a00 0000 722b  pN).r)...r*...r+
-00000dc0: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
-00000dd0: 0000 da07 6869 7374 6f72 79da 0565 6d70  ....history..emp
-00000de0: 7479 da07 746f 5f64 6963 74da 0270 64da  ty..to_dict..pd.
-00000df0: 0944 6174 6146 7261 6d65 da09 6672 6f6d  .DataFrame..from
-00000e00: 5f64 6963 74da 0b72 6573 6574 5f69 6e64  _dict..reset_ind
-00000e10: 6578 2908 7221 0000 0072 3a00 0000 7231  ex).r!...r:...r1
-00000e20: 0000 0072 2b00 0000 7232 0000 0072 3f00  ...r+...r2...r?.
-00000e30: 0000 5a0c 6869 7374 6f72 795f 6469 6374  ..Z.history_dict
-00000e40: 5a0a 6869 7374 6f72 795f 6466 721e 0000  Z.history_dfr...
-00000e50: 0072 1e00 0000 721f 0000 00da 1167 6574  .r....r......get
-00000e60: 5f73 746f 636b 5f68 6973 746f 7279 7400  _stock_historyt.
-00000e70: 0000 7318 0000 0000 0e0a 0106 0108 0108  ..s.............
-00000e80: 0102 0208 020c 0206 010c 020c 0114 0272  ...............r
-00000e90: 4600 0000 7a17 7374 6f63 6b73 2f7b 7379  F...z.stocks/{sy
-00000ea0: 6d62 6f6c 7d2f 6869 7374 6f72 797a 152f  mbol}/historyz./
-00000eb0: 7374 6f63 6b2f 7b73 796d 626f 6c7d 2f74  stock/{symbol}/t
-00000ec0: 7265 6e64 6301 0000 0000 0000 0000 0000  rendc...........
-00000ed0: 0008 0000 0003 0000 0043 0000 0073 6800  .........C...sh.
-00000ee0: 0000 7400 a001 7c00 a101 7d01 7c01 6a02  ..t...|...}.|.j.
-00000ef0: 7d02 7403 7c02 8301 7d03 7c03 7404 6b02  }.t.|...}.|.t.k.
-00000f00: 7222 6e08 7405 6401 8301 0100 7c01 6a06  r"n.t.d.....|.j.
-00000f10: 6402 6403 8d01 7d04 7c04 6404 1900 7d05  d.d...}.|.d...}.
-00000f20: 7c05 6a07 6405 1900 7c05 6a07 6406 1900  |.j.d...|.j.d...
-00000f30: 6b04 7256 6407 6e02 6408 7d06 7c00 7c06  k.rVd.n.d.}.|.|.
-00000f40: 6409 9c02 7d07 7c07 5300 290a 75b9 0000  d...}.|.S.).u...
-00000f50: 000a 2020 2020 2323 2055 7361 6269 6c69  ..    ## Usabili
-00000f60: 6461 6465 200a 2020 2020 2d20 4964 656e  dade .    - Iden
-00000f70: 7469 6669 6361 2061 2074 656e 6465 6e63  tifica a tendenc
-00000f80: 6961 2064 6520 7072 65c3 a76f 2064 6520  ia de pre..o de 
-00000f90: 756d 6120 61c3 a761 6f2c 2073 6520 6972  uma a..ao, se ir
-00000fa0: 6120 7365 7220 6465 2041 4c54 4120 6f75  a ser de ALTA ou
-00000fb0: 2042 4149 5841 0a20 2020 200a 2020 2020   BAIXA.    .    
-00000fc0: 2323 2050 6172 c3a2 6d65 7472 6f73 0a20  ## Par..metros. 
-00000fd0: 2020 200a 2020 2020 2d20 7379 6d62 6f6c     .    - symbol
-00000fe0: 202d 3e20 4e6f 6d65 2064 6f20 4174 6976   -> Nome do Ativ
-00000ff0: 6f20 7061 7261 2061 2062 7573 6361 200a  o para a busca .
-00001000: 0a20 2020 200a 2020 2020 7223 0000 005a  .    .    r#...Z
-00001010: 0231 6472 3b00 0000 da05 436c 6f73 6572  .1dr;.....Closer
-00001020: 2500 0000 7201 0000 00da 0275 70da 0464  %...r......up..d
-00001030: 6f77 6e29 0272 2100 0000 da05 7472 656e  own).r!.....tren
-00001040: 6429 0872 2900 0000 722a 0000 0072 2b00  d).r)...r*...r+.
-00001050: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
-00001060: 0072 3f00 0000 722f 0000 0029 0872 2100  .r?...r/...).r!.
-00001070: 0000 7231 0000 0072 2b00 0000 7232 0000  ..r1...r+...r2..
-00001080: 0072 3f00 0000 da0c 636c 6f73 655f 7072  .r?.....close_pr
-00001090: 6963 6573 724a 0000 0072 3300 0000 721e  icesrJ...r3...r.
-000010a0: 0000 0072 1e00 0000 721f 0000 00da 0f67  ...r....r......g
-000010b0: 6574 5f73 746f 636b 5f74 7265 6e64 a200  et_stock_trend..
-000010c0: 0000 731a 0000 0000 0d0a 0106 0108 0108  ..s.............
-000010d0: 0102 0208 020c 0108 011c 0202 0102 ff06  ................
-000010e0: 0672 4c00 0000 7a15 7374 6f63 6b73 2f7b  .rL...z.stocks/{
-000010f0: 7379 6d62 6f6c 7d2f 7472 656e 647a 192f  symbol}/trendz./
-00001100: 7374 6f63 6b2f 7b73 796d 626f 6c7d 2f74  stock/{symbol}/t
-00001110: 6563 686e 6963 616c 6301 0000 0000 0000  echnicalc.......
-00001120: 0000 0000 0011 0000 0006 0000 0043 0000  .............C..
-00001130: 0073 f800 0000 7400 a001 7c00 a101 7d01  .s....t...|...}.
-00001140: 7c01 6a02 7d02 7403 7c02 8301 7d03 7c03  |.j.}.t.|...}.|.
-00001150: 7404 6b02 7222 6e08 7405 6401 8301 0100  t.k.r"n.t.d.....
-00001160: 7c01 6a06 6402 6403 8d01 7d04 7c04 6404  |.j.d.d...}.|.d.
-00001170: 1900 7d05 7c05 6a07 6405 6406 8d01 a008  ..}.|.j.d.d.....
-00001180: a100 6a09 6407 1900 7d06 7c05 6a07 6408  ..j.d...}.|.j.d.
-00001190: 6406 8d01 a008 a100 6a09 6407 1900 7d07  d.......j.d...}.
-000011a0: 7c05 a00a a100 7d08 7c08 a00b 7c08 6409  |.....}.|...|.d.
-000011b0: 6b04 6409 a102 7d09 7c08 a00b 7c08 6409  k.d...}.|...|.d.
-000011c0: 6b00 6409 a102 0b00 7d0a 7c09 6a07 640a  k.d.....}.|.j.d.
-000011d0: 6406 8d01 a008 a100 7d0b 7c0a 6a07 640a  d.......}.|.j.d.
-000011e0: 6406 8d01 a008 a100 7d0c 7c0b 7c0c 1b00  d.......}.|.|...
-000011f0: 7d0d 640b 640b 640c 7c0d 1700 1b00 6a09  }.d.d.d.|.....j.
-00001200: 6407 1900 1800 7d0e 7c0e 640d 6b05 72e0  d.....}.|.d.k.r.
-00001210: 640e 7d0f 6e04 640f 7d0f 7c00 7c06 7c07  d.}.n.d.}.|.|.|.
-00001220: 7c0e 7c0f 6410 9c05 7d10 7c10 5300 2911  |.|.d...}.|.S.).
-00001230: 7579 0200 000a 2020 2020 2323 2055 7361  uy....    ## Usa
-00001240: 6269 6c69 6461 6465 200a 2020 2020 2d20  bilidade .    - 
-00001250: 63c3 a16c 6375 6c6f 2065 6e76 6f6c 7665  c..lculo envolve
-00001260: 2061 2063 6f6d 7061 7261 c3a7 c3a3 6f20   a compara....o 
-00001270: 6461 206d c3a9 6469 6120 6465 2067 616e  da m..dia de gan
-00001280: 686f 7320 656d 2075 6d20 7065 72c3 ad6f  hos em um per..o
-00001290: 646f 2064 6520 7465 6d70 6f20 636f 6d20  do de tempo com 
-000012a0: 6120 6dc3 a964 6961 2064 6520 7065 7264  a m..dia de perd
-000012b0: 6173 2065 6d20 756d 2070 6572 c3ad 6f64  as em um per..od
-000012c0: 6f20 6465 2074 656d 706f 2e20 0a0a 2020  o de tempo. ..  
-000012d0: 2020 0a20 2020 2023 2320 436f 6d6f 2069    .    ## Como i
-000012e0: 6e74 6572 7072 6574 6172 200a 2020 2020  nterpretar .    
-000012f0: 2d20 5175 616e 646f 206f 2052 5349 2065  - Quando o RSI e
-00001300: 7374 c3a1 2061 6369 6d61 2064 6520 3730  st.. acima de 70
-00001310: 2c20 6f20 6174 6976 6f20 c3a9 2063 6f6e  , o ativo .. con
-00001320: 7369 6465 7261 646f 2073 6f62 7265 636f  siderado sobreco
-00001330: 6d70 7261 646f 2c20 6f20 7175 6520 7369  mprado, o que si
-00001340: 676e 6966 6963 6120 7175 6520 706f 6465  gnifica que pode
-00001350: 2065 7374 6172 2070 7265 7374 6573 2061   estar prestes a
-00001360: 2073 6f66 7265 7220 756d 6120 636f 7272   sofrer uma corr
-00001370: 65c3 a7c3 a36f 2070 6172 6120 6261 6978  e....o para baix
-00001380: 6f2e 200a 2020 2020 5175 616e 646f 206f  o. .    Quando o
-00001390: 2052 5349 2065 7374 c3a1 2061 6261 6978   RSI est.. abaix
-000013a0: 6f20 6465 2033 302c 206f 2061 7469 766f  o de 30, o ativo
-000013b0: 20c3 a920 636f 6e73 6964 6572 6164 6f20   .. considerado 
-000013c0: 736f 6272 6576 656e 6469 646f 2c20 6f20  sobrevendido, o 
-000013d0: 7175 6520 7369 676e 6966 6963 6120 7175  que significa qu
-000013e0: 6520 706f 6465 2065 7374 6172 2070 7265  e pode estar pre
-000013f0: 7374 6573 2061 2073 7562 6972 206e 6f76  stes a subir nov
-00001400: 616d 656e 7465 2e20 0a20 0a20 2020 202d  amente. . .    -
-00001410: 2073 6d61 5f35 3020 2d3e 204d 6564 6961   sma_50 -> Media
-00001420: 206d 6f76 656c 2064 6f73 2035 3020 7065   movel dos 50 pe
-00001430: 7269 6f64 6f73 0a20 2020 202d 2073 6d61  riodos.    - sma
-00001440: 5f32 3030 202d 3e20 6d65 6469 6120 6d6f  _200 -> media mo
-00001450: 7665 6c20 646f 7320 3230 3020 7065 7269  vel dos 200 peri
-00001460: 646f 730a 0a20 2020 2023 2320 5061 72c3  dos..    ## Par.
-00001470: a26d 6574 726f 730a 2020 2020 2d20 7379  .metros.    - sy
-00001480: 6d62 6f6c 202d 3e20 4e6f 6d65 2064 6f20  mbol -> Nome do 
-00001490: 4174 6976 6f20 7061 7261 2061 2062 7573  Ativo para a bus
-000014a0: 6361 200a 0a20 2020 200a 2020 2020 7223  ca ..    .    r#
-000014b0: 0000 00da 036d 6178 723b 0000 0072 4700  .....maxr;...rG.
-000014c0: 0000 e932 0000 0029 01da 0677 696e 646f  ...2...)...windo
-000014d0: 7772 2500 0000 e9c8 0000 0072 0100 0000  wr%........r....
-000014e0: e90e 0000 00e9 6400 0000 7215 0000 00e9  ......d...r.....
-000014f0: 4600 0000 7a1f 4120 6368 616e 6365 2064  F...z.A chance d
-00001500: 6f20 7072 6563 6f20 646f 2061 7469 766f  o preco do ativo
-00001510: 2043 4149 527a 2041 2063 6861 6e63 6520   CAIRz A chance 
-00001520: 646f 2070 7265 636f 2064 6f20 6174 6976  do preco do ativ
-00001530: 6f20 5355 4249 5229 0572 2100 0000 da06  o SUBIR).r!.....
-00001540: 736d 615f 3530 da07 736d 615f 3230 30da  sma_50..sma_200.
-00001550: 0372 7369 5a08 7465 6e64 656e 6379 290c  .rsiZ.tendency).
-00001560: 7229 0000 0072 2a00 0000 722b 0000 0072  r)...r*...r+...r
-00001570: 2c00 0000 722d 0000 0072 2e00 0000 723f  ,...r-...r....r?
-00001580: 0000 005a 0772 6f6c 6c69 6e67 da04 6d65  ...Z.rolling..me
-00001590: 616e 722f 0000 00da 0464 6966 66da 0577  anr/.....diff..w
-000015a0: 6865 7265 2911 7221 0000 0072 3100 0000  here).r!...r1...
-000015b0: 722b 0000 0072 3200 0000 723f 0000 0072  r+...r2...r?...r
-000015c0: 4b00 0000 7254 0000 0072 5500 0000 da05  K...rT...rU.....
-000015d0: 6465 6c74 615a 0467 6169 6e5a 046c 6f73  deltaZ.gainZ.los
-000015e0: 735a 0861 7667 5f67 6169 6e5a 0861 7667  sZ.avg_gainZ.avg
-000015f0: 5f6c 6f73 73da 0272 7372 5600 0000 da06  _loss..rsrV.....
-00001600: 7374 6174 7573 7233 0000 0072 1e00 0000  statusr3...r....
-00001610: 721e 0000 0072 1f00 0000 da14 6765 745f  r....r......get_
-00001620: 7374 6f63 6b5f 7465 6368 6e69 6361 6c73  stock_technicals
-00001630: ca00 0000 7336 0000 0000 120a 0106 0108  ....s6..........
-00001640: 0108 0102 0208 020c 0108 0316 0116 0308  ................
-00001650: 0110 0112 0110 0110 0108 0116 0208 0106  ................
-00001660: 0204 0302 0102 0102 0102 0102 fb06 0a72  ...............r
-00001670: 5d00 0000 7a19 7374 6f63 6b73 2f7b 7379  ]...z.stocks/{sy
-00001680: 6d62 6f6c 7d2f 7465 6368 6e69 6361 6c7a  mbol}/technicalz
-00001690: 1a73 746f 636b 732f 7b73 796d 626f 6c7d  .stocks/{symbol}
-000016a0: 2f76 6f6c 6174 696c 6974 7929 0472 2100  /volatility).r!.
-000016b0: 0000 da0a 7374 6172 745f 6461 7465 da08  ....start_date..
-000016c0: 656e 645f 6461 7465 7222 0000 0063 0300  end_dater"...c..
-000016d0: 0000 0000 0000 0000 0000 0600 0000 0600  ................
-000016e0: 0000 4300 0000 7368 0000 007a 2874 006a  ..C...sh...z(t.j
-000016f0: 017c 007c 017c 0264 018d 037d 037c 036a  .|.|.|.d...}.|.j
-00001700: 0272 2664 0274 0364 0383 0169 0157 0053  .r&d.t.d...i.W.S
-00001710: 0057 006e 0c01 0001 0001 0059 006e 0230  .W.n.......Y.n.0
-00001720: 0074 04a0 057c 0364 0419 007c 0364 0419  .t...|.d...|.d..
-00001730: 00a0 0664 05a1 011b 00a1 017d 0474 04a0  ...d.......}.t..
-00001740: 0764 067c 04a0 08a1 0014 00a1 017d 057c  .d.|.........}.|
-00001750: 0553 0029 0775 6e01 0000 0a20 2020 2023  .S.).un....    #
-00001760: 2320 5573 6162 696c 6964 6164 6520 0a20  # Usabilidade . 
-00001770: 2020 202d 204d c3a9 746f 646f 2075 7361     - M..todo usa
-00001780: 646f 2070 6172 6120 7665 7269 6669 6361  do para verifica
-00001790: 7220 6120 766f 6c61 7469 6c69 6461 6465  r a volatilidade
-000017a0: 2064 6520 756d 2061 7469 766f 2065 6d20   de um ativo em 
-000017b0: 636f 6d70 6172 6163 616f 2061 6f20 6d65  comparacao ao me
-000017c0: 7263 6164 6f20 656d 2071 7565 2065 7374  rcado em que est
-000017d0: 6120 200a 0a20 2020 200a 2020 2020 2323  a  ..    .    ##
-000017e0: 2050 6172 c3a2 6d65 7472 6f73 0a20 2020   Par..metros.   
-000017f0: 202d 2073 796d 626f 6c20 2d3e 204e 6f6d   - symbol -> Nom
-00001800: 6520 646f 2041 7469 766f 2070 6172 6120  e do Ativo para 
-00001810: 6120 6275 7363 6120 0a0a 2020 2020 2d20  a busca ..    - 
-00001820: 7374 6172 745f 6461 7465 202d 3e20 4461  start_date -> Da
-00001830: 7461 2064 6520 496e 6963 696f 2064 6120  ta de Inicio da 
-00001840: 6275 7363 6120 6461 7320 696e 666f 7320  busca das infos 
-00001850: 2870 7265 636f 2c20 766f 6c75 6d65 2c20  (preco, volume, 
-00001860: 6574 6329 2064 6f20 6174 6976 6f20 0a0a  etc) do ativo ..
-00001870: 2020 2020 2d20 656e 645f 6461 7465 202d      - end_date -
-00001880: 3e20 4461 7461 2046 696e 616c 2070 6172  > Data Final par
-00001890: 6120 6120 6275 7363 6120 6461 7320 696e  a a busca das in
-000018a0: 666f 7320 2870 7265 636f 2c20 766f 6c75  fos (preco, volu
-000018b0: 6d65 2c20 6574 6329 2064 6f20 6174 6976  me, etc) do ativ
-000018c0: 6f20 0a0a 2020 2020 a902 da05 7374 6172  o ..    ....star
-000018d0: 74da 0365 6e64 723c 0000 007a 384e 616f  t..endr<...z8Nao
-000018e0: 2066 6f69 2065 6e63 6f6e 7472 6164 6f20   foi encontrado 
-000018f0: 6f20 6869 7374 6f72 6963 6f20 6e65 7373  o historico ness
-00001900: 6520 7065 7269 6f64 6f2c 2076 6572 6966  e periodo, verif
-00001910: 6963 6172 2e72 4700 0000 7215 0000 00e9  icar.rG...r.....
-00001920: fc00 0000 2909 7229 0000 00da 0864 6f77  ....).r).....dow
-00001930: 6e6c 6f61 6472 4000 0000 722e 0000 00da  nloadr@...r.....
-00001940: 026e 70da 036c 6f67 da05 7368 6966 74da  .np..log..shift.
-00001950: 0473 7172 74da 0376 6172 2906 7221 0000  .sqrt..var).r!..
-00001960: 0072 5e00 0000 725f 0000 005a 0a73 746f  .r^...r_...Z.sto
-00001970: 636b 5f64 6174 615a 0b6c 6f67 5f72 6574  ck_dataZ.log_ret
-00001980: 7572 6e73 5a0a 766f 6c61 7469 6c69 7479  urnsZ.volatility
-00001990: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
-000019a0: 0e67 6574 5f76 6f6c 6174 696c 6974 790c  .get_volatility.
-000019b0: 0100 0073 1200 0000 000d 0201 1001 0601  ...s............
-000019c0: 1201 0601 0602 1c01 1202 726a 0000 007a  ..........rj...z
-000019d0: 1473 746f 636b 732f 7b73 796d 626f 6c7d  .stocks/{symbol}
-000019e0: 2f62 6574 6163 0100 0000 0000 0000 0000  /betac..........
-000019f0: 0000 0f00 0000 0300 0000 4300 0000 73be  ..........C...s.
-00001a00: 0000 0074 00a0 017c 00a1 017d 0174 00a0  ...t...|...}.t..
-00001a10: 0164 01a1 017d 027c 016a 027d 037c 026a  .d...}.|.j.}.|.j
-00001a20: 027d 0474 037c 0383 017d 057c 0574 046b  .}.t.|...}.|.t.k
-00001a30: 0273 427c 0474 046b 0272 3a6e 0874 0564  .sB|.t.k.r:n.t.d
-00001a40: 0283 0101 007c 016a 0664 0364 048d 017d  .....|.j.d.d...}
-00001a50: 067c 026a 0664 0364 048d 017d 077c 0664  .|.j.d.d...}.|.d
-00001a60: 0519 00a0 07a1 007d 087c 0764 0519 00a0  .......}.|.d....
-00001a70: 07a1 007d 097c 08a0 087c 09a1 017d 0a7c  ...}.|...|...}.|
-00001a80: 09a0 09a1 007d 0b7c 0a7c 0b1b 007d 0c7c  .....}.|.|...}.|
-00001a90: 0c64 066b 0472 9864 077d 0d7c 0c64 066b  .d.k.r.d.}.|.d.k
-00001aa0: 0072 a464 087d 0d7c 0c64 066b 0272 b064  .r.d.}.|.d.k.r.d
-00001ab0: 097d 0d7c 0c7c 0d64 0a9c 027d 0e7c 0e53  .}.|.|.d...}.|.S
-00001ac0: 0029 0b75 9501 0000 0a20 2020 2023 2320  .).u.....    ## 
-00001ad0: 5573 6162 696c 6964 6164 6520 0a20 2020  Usabilidade .   
-00001ae0: 202d 204f 2062 6574 6120 c3a9 2075 6d61   - O beta .. uma
-00001af0: 206d 6564 6964 6120 6573 7461 74c3 ad73   medida estat..s
-00001b00: 7469 6361 2071 7565 2069 6e64 6963 6120  tica que indica 
-00001b10: 6120 7265 6c61 c3a7 c3a3 6f20 656e 7472  a rela....o entr
-00001b20: 6520 6120 766f 6c61 7469 6c69 6461 6465  e a volatilidade
-00001b30: 2064 6520 756d 6120 61c3 a7c3 a36f 2065   de uma a....o e
-00001b40: 2061 2076 6f6c 6174 696c 6964 6164 6520   a volatilidade 
-00001b50: 646f 206d 6572 6361 646f 2063 6f6d 6f20  do mercado como 
-00001b60: 756d 2074 6f64 6f2e 0a20 2020 204f 2076  um todo..    O v
-00001b70: 616c 6f72 2064 6f20 6265 7461 20c3 a920  alor do beta .. 
-00001b80: 7574 696c 697a 6164 6f20 7061 7261 206d  utilizado para m
-00001b90: 6564 6972 206f 2072 6973 636f 2064 6520  edir o risco de 
-00001ba0: 756d 6120 61c3 a7c3 a36f 2065 6d20 7265  uma a....o em re
-00001bb0: 6c61 c3a7 c3a3 6f20 616f 206d 6572 6361  la....o ao merca
-00001bc0: 646f 2065 6d20 7175 6520 656c 6120 c3a9  do em que ela ..
-00001bd0: 206e 6567 6f63 6961 6461 2e20 0a0a 2020   negociada. ..  
-00001be0: 2020 0a20 2020 2023 2320 5061 72c3 a26d    .    ## Par..m
-00001bf0: 6574 726f 730a 2020 2020 2d20 7379 6d62  etros.    - symb
-00001c00: 6f6c 202d 3e20 4e6f 6d65 2064 6f20 4174  ol -> Nome do At
-00001c10: 6976 6f20 7061 7261 2061 2062 7573 6361  ivo para a busca
-00001c20: 200a 0a20 2020 202d 206d 6172 6b65 7420   ..    - market 
-00001c30: 2d3e 2043 6f6d 6f20 7061 6472 616f 2c20  -> Como padrao, 
-00001c40: 4d65 7263 6164 6f3a 2049 424f 5645 5350  Mercado: IBOVESP
-00001c50: 4120 2f20 4256 5350 0a20 2020 207a 055e  A / BVSP.    z.^
-00001c60: 4256 5350 7223 0000 0072 4d00 0000 723b  BVSPr#...rM...r;
-00001c70: 0000 0072 4700 0000 7215 0000 007a 2841  ...rG...r....z(A
-00001c80: 6361 6f20 6d61 6973 2056 6f6c 6174 696c  cao mais Volatil
-00001c90: 2071 7565 206f 206d 6572 6361 646f 2065   que o mercado e
-00001ca0: 6d20 6765 7261 6c7a 2941 6361 6f20 6d65  m geralz)Acao me
-00001cb0: 6e6f 7320 566f 6c61 7469 6c20 7175 6520  nos Volatil que 
-00001cc0: 6f20 6d65 7263 6164 6f20 656d 2067 6572  o mercado em ger
-00001cd0: 616c 7a34 4163 616f 2063 6f6d 2061 206d  alz4Acao com a m
-00001ce0: 6573 6d61 2056 6f6c 6174 696c 6964 6164  esma Volatilidad
-00001cf0: 6520 7175 6520 6f20 6d65 7263 6164 6f20  e que o mercado 
-00001d00: 656d 2067 6572 616c 2902 da04 6265 7461  em geral)...beta
-00001d10: 725c 0000 0029 0a72 2900 0000 722a 0000  r\...).r)...r*..
-00001d20: 0072 2b00 0000 722c 0000 0072 2d00 0000  .r+...r,...r-...
-00001d30: 722e 0000 0072 3f00 0000 da0a 7063 745f  r....r?.....pct_
-00001d40: 6368 616e 6765 da03 636f 7672 6900 0000  change..covri...
-00001d50: 290f 7221 0000 005a 0561 7373 6574 5a06  ).r!...Z.assetZ.
-00001d60: 6d61 726b 6574 722b 0000 005a 0a69 6e66  marketr+...Z.inf
-00001d70: 6f4d 6172 6b65 7472 3200 0000 5a0d 6173  oMarketr2...Z.as
-00001d80: 7365 745f 6869 7374 6f72 795a 0e6d 6172  set_historyZ.mar
-00001d90: 6b65 745f 6869 7374 6f72 795a 0d61 7373  ket_historyZ.ass
-00001da0: 6574 5f72 6574 7572 6e73 5a0e 6d61 726b  et_returnsZ.mark
-00001db0: 6574 5f72 6574 7572 6e73 726d 0000 0072  et_returnsrm...r
-00001dc0: 6900 0000 726b 0000 0072 5c00 0000 7233  i...rk...r\...r3
-00001dd0: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
-00001de0: 0000 da08 6765 745f 6265 7461 2c01 0000  ....get_beta,...
-00001df0: 7332 0000 0000 0e0a 010a 0106 0106 0108  s2..............
-00001e00: 0110 0102 0208 020c 010c 030c 010c 030a  ................
-00001e10: 0108 0108 0208 0104 0108 0104 0108 0104  ................
-00001e20: 0302 0102 ff06 0572 6e00 0000 7a13 7374  .......rn...z.st
-00001e30: 6f63 6b73 2f7b 7379 6d62 6f6c 7d2f 5661  ocks/{symbol}/Va
-00001e40: 5229 0472 2100 0000 da10 636f 6e66 6964  R).r!.....confid
-00001e50: 656e 6365 5f6c 6576 656c da0f 6c6f 6f6b  ence_level..look
-00001e60: 6261 636b 5f70 6572 696f 6472 2200 0000  back_periodr"...
-00001e70: 6303 0000 0000 0000 0000 0000 000b 0000  c...............
-00001e80: 0006 0000 0043 0000 0073 9e00 0000 7400  .....C...s....t.
-00001e90: a001 7c00 a101 7d03 7c03 6a02 7d04 7403  ..|...}.|.j.}.t.
-00001ea0: 7c04 8301 7d05 7c05 7404 6b02 7222 6e08  |...}.|.t.k.r"n.
-00001eb0: 7405 6401 8301 0100 7c03 6a06 7c02 9b00  t.d.....|.j.|...
-00001ec0: 6402 9d02 6403 8d01 6404 1900 7d06 7407  d...d...d...}.t.
-00001ed0: a008 7c06 7c06 a009 6405 a101 1b00 a101  ..|.|...d.......
-00001ee0: 7d07 7c07 a00a a100 7d08 7c08 740b a00c  }.|.....}.|.t...
-00001ef0: 6405 7c01 1800 a101 1400 7d09 7405 6406  d.|.......}.t.d.
-00001f00: 740d 7c09 7c06 6407 1900 1400 6408 8302  t.|.|.d.....d...
-00001f10: 6901 8301 0100 740d 7c09 7c06 6407 1900  i.....t.|.|.d...
-00001f20: 1400 6408 8302 7d0a 7c0a 5300 2909 75c8  ..d...}.|.S.).u.
-00001f30: 0100 000a 2020 2020 2323 2055 7361 6269  ....    ## Usabi
-00001f40: 6c69 6461 6465 200a 2020 2020 2d20 4f20  lidade .    - O 
-00001f50: 5661 6c75 6520 6174 2052 6973 6b20 2856  Value at Risk (V
-00001f60: 6152 2920 c3a9 2075 6d61 206d 6564 6964  aR) .. uma medid
-00001f70: 6120 6465 2072 6973 636f 2071 7565 2069  a de risco que i
-00001f80: 6e64 6963 6120 6120 7065 7264 6120 6dc3  ndica a perda m.
-00001f90: a178 696d 6120 6573 7065 7261 6461 2c20  .xima esperada, 
-00001fa0: 636f 6d20 756d 2064 6574 6572 6d69 6e61  com um determina
-00001fb0: 646f 206e c3ad 7665 6c20 6465 2063 6f6e  do n..vel de con
-00001fc0: 6669 616e c3a7 612c 2065 6d20 756d 2069  fian..a, em um i
-00001fd0: 6e74 6572 7661 6c6f 2064 6520 7465 6d70  ntervalo de temp
-00001fe0: 6f20 7072 c3a9 2d64 6574 6572 6d69 6e61  o pr..-determina
-00001ff0: 646f 2e20 0a0a 2020 2020 0a20 2020 2023  do. ..    .    #
-00002000: 2320 5061 72c3 a26d 6574 726f 730a 2020  # Par..metros.  
-00002010: 2020 0a20 2020 202d 2073 796d 626f 6c20    .    - symbol 
-00002020: 2d3e 204e 6f6d 6520 646f 2041 7469 766f  -> Nome do Ativo
-00002030: 2070 6172 6120 6661 7a65 7220 6120 6275   para fazer a bu
-00002040: 7363 6120 0a0a 2020 2020 2d20 636f 6e66  sca ..    - conf
-00002050: 6964 656e 6365 5f6c 6576 656c 202d 3e20  idence_level -> 
-00002060: 4e69 7665 6c20 6465 2063 6f6e 6669 616e  Nivel de confian
-00002070: c3a7 6120 7061 7261 206f 2056 4152 2028  ..a para o VAR (
-00002080: 3020 6120 3129 2c20 6e6f 726d 616c 6d65  0 a 1), normalme
-00002090: 6e74 6520 7573 6164 6f20 656d 2030 2e39  nte usado em 0.9
-000020a0: 3520 0a0a 2020 2020 2d20 6c6f 6f6b 6261  5 ..    - lookba
-000020b0: 636b 5f70 6572 696f 6420 2d3e 2050 6572  ck_period -> Per
-000020c0: 696f 646f 2045 4d20 4449 4153 2061 2073  iodo EM DIAS a s
-000020d0: 6572 2063 6f6e 7369 6465 7261 646f 2070  er considerado p
-000020e0: 6172 6120 6f20 63c3 a16c 6375 6c6f 2064  ara o c..lculo d
-000020f0: 6f20 5661 520a 0a20 2020 2072 2300 0000  o VaR..    r#...
-00002100: da01 6472 3b00 0000 7247 0000 0072 1500  ..dr;...rG...r..
-00002110: 0000 5a03 5661 5272 2500 0000 e902 0000  ..Z.VaRr%.......
-00002120: 0029 0e72 2900 0000 722a 0000 0072 2b00  .).r)...r*...r+.
-00002130: 0000 722c 0000 0072 2d00 0000 722e 0000  ..r,...r-...r...
-00002140: 0072 3f00 0000 7265 0000 0072 6600 0000  .r?...re...rf...
-00002150: 7267 0000 00da 0373 7464 7202 0000 005a  rg.....stdr....Z
-00002160: 0370 7066 da05 726f 756e 6429 0b72 2100  .ppf..round).r!.
-00002170: 0000 726f 0000 0072 7000 0000 7231 0000  ..ro...rp...r1..
-00002180: 0072 2b00 0000 7232 0000 005a 0670 7269  .r+...r2...Z.pri
-00002190: 6365 73da 0772 6574 7572 6e73 5a07 7374  ces..returnsZ.st
-000021a0: 645f 6465 7672 6900 0000 5a03 5661 7272  d_devri...Z.Varr
-000021b0: 1e00 0000 721e 0000 0072 1f00 0000 da07  ....r....r......
-000021c0: 6765 745f 7661 7266 0100 0073 1a00 0000  get_varf...s....
-000021d0: 000f 0a01 0601 0801 0801 0202 0803 1603  ................
-000021e0: 1403 0801 1201 1a01 1201 7276 0000 007a  ..........rv...z
-000021f0: 1c73 746f 636b 732f 7b73 796d 626f 6c7d  .stocks/{symbol}
-00002200: 2f41 6e6e 7561 6c52 6574 7572 6e29 04da  /AnnualReturn)..
-00002210: 0773 796d 626f 6c73 725e 0000 0072 5f00  .symbolsr^...r_.
-00002220: 0000 7222 0000 0063 0300 0000 0000 0000  ..r"...c........
-00002230: 0000 0000 1100 0000 0700 0000 4300 0000  ............C...
-00002240: 7392 0100 0074 007c 0074 0183 0272 c874  s....t.|.t...r.t
-00002250: 0264 017c 009b 009d 0283 0101 0074 036a  .d.|.........t.j
-00002260: 047c 007c 017c 0264 0264 038d 047d 037a  .|.|.|.d.d...}.z
-00002270: 8674 03a0 057c 00a1 016a 067d 047c 0464  .t...|...j.}.|.d
-00002280: 0419 007d 057c 0364 0519 007d 067c 06a0  ...}.|.d...}.|..
-00002290: 07a1 007d 077c 07a0 08a1 0064 0614 007d  ...}.|.....d...}
-000022a0: 087c 07a0 09a1 0064 0714 007d 097c 066a  .|.....d...}.|.j
-000022b0: 0a64 0819 0064 0914 007d 0a7c 066a 0a64  .d...d...}.|.j.d
-000022c0: 0a19 0064 0914 007d 0b7c 0b7c 0a18 007c  ...d...}.|.|...|
-000022d0: 0a1b 007d 0c74 0b6a 0c7c 007c 057c 087c  ...}.t.j.|.|.|.|
-000022e0: 097c 0c64 0b9c 0564 0c67 0164 0d8d 027d  .|.d...d.g.d...}
-000022f0: 0d7c 0d57 0053 0001 0001 0001 0074 0264  .|.W.S.......t.d
-00002300: 0e83 0101 0059 006e 0230 006e c674 007c  .....Y.n.0.n.t.|
-00002310: 0074 0d83 0290 0172 8674 0ba0 0ca1 007d  .t.....r.t.....}
-00002320: 0e74 0264 0f7c 009b 009d 0283 0101 007c  .t.d.|.........|
-00002330: 0044 005d 927d 0f74 036a 047c 0f7c 017c  .D.].}.t.j.|.|.|
-00002340: 0264 0264 038d 047d 037c 0364 0519 007d  .d.d...}.|.d...}
-00002350: 067c 06a0 07a1 007d 077c 07a0 08a1 0064  .|.....}.|.....d
-00002360: 0614 007d 087c 07a0 09a1 0064 0714 007d  ...}.|.....d...}
-00002370: 097c 066a 0a64 0819 0064 0914 007d 0a7c  .|.j.d...d...}.|
-00002380: 066a 0a64 0a19 0064 0914 007d 0b7c 0b7c  .j.d...d...}.|.|
-00002390: 0a18 007c 0a1b 007d 0c74 0b6a 0c7c 0f7c  ...|...}.t.j.|.|
-000023a0: 087c 097c 0c64 109c 0474 0e7c 0083 0167  .|.|.d...t.|...g
-000023b0: 0164 0d8d 027d 1074 0ba0 0f7c 107c 0e67  .d...}.t...|.|.g
-000023c0: 02a1 017d 0e71 ee7c 0e53 0074 0264 1183  ...}.q.|.S.t.d..
-000023d0: 0101 0064 1253 0029 1375 9b01 0000 0a20  ...d.S.).u..... 
-000023e0: 2020 2023 2320 5573 6162 696c 6964 6164     ## Usabilidad
-000023f0: 650a 2020 2020 2d20 5265 6365 6265 2075  e.    - Recebe u
-00002400: 6d61 206c 6973 7461 2065 2072 6574 6f72  ma lista e retor
-00002410: 6e61 2075 6d20 4461 7461 4672 616d 6520  na um DataFrame 
-00002420: 636f 6d20 6173 2069 6e66 6f72 6d61 c3a7  com as informa..
-00002430: c3b5 6573 2064 6f73 2061 7469 766f 7320  ..es dos ativos 
-00002440: 6520 616c 6775 6d61 7320 6573 7461 74c3  e algumas estat.
-00002450: ad73 7469 6361 7320 62c3 a173 6963 6173  .sticas b..sicas
-00002460: 2e20 0a0a 2020 2020 0a20 2020 2023 2320  . ..    .    ## 
-00002470: 5061 72c3 a26d 6574 726f 730a 2020 2020  Par..metros.    
-00002480: 2d20 7379 6d62 6f6c 7320 2d3e 2052 6563  - symbols -> Rec
-00002490: 6562 6520 756d 6120 6c69 7374 6120 6f75  ebe uma lista ou
-000024a0: 2075 6d20 756e 6963 6f20 6174 6976 6f20   um unico ativo 
-000024b0: 7061 7261 2062 7573 6361 7220 6e61 2062  para buscar na b
-000024c0: 6173 6520 0a0a 2020 2020 2d20 7374 6172  ase ..    - star
-000024d0: 745f 6461 7465 202d 3e20 4461 7461 2064  t_date -> Data d
-000024e0: 6520 496e 6963 696f 2064 6120 6275 7363  e Inicio da busc
-000024f0: 6120 6461 7320 696e 666f 7320 2870 7265  a das infos (pre
-00002500: 636f 2c20 766f 6c75 6d65 2c20 6574 6329  co, volume, etc)
-00002510: 2064 6f20 6174 6976 6f20 0a0a 2020 2020   do ativo ..    
-00002520: 2d20 656e 645f 6461 7465 202d 3e20 4461  - end_date -> Da
-00002530: 7461 2046 696e 616c 2070 6172 6120 6120  ta Final para a 
-00002540: 6275 7363 6120 6461 7320 696e 666f 7320  busca das infos 
-00002550: 2870 7265 636f 2c20 766f 6c75 6d65 2c20  (preco, volume, 
-00002560: 6574 6329 2064 6f20 6174 6976 6f20 0a0a  etc) do ativo ..
-00002570: 2020 2020 0a20 2020 2075 1a00 0000 566f      .    u....Vo
-00002580: 63c3 aa20 6469 6769 746f 7520 756d 6120  c.. digitou uma 
-00002590: 7374 7269 6e67 3a20 da06 7469 636b 6572  string: ..ticker
-000025a0: 2904 5a07 7469 636b 6572 7372 6100 0000  ).Z.tickersra...
-000025b0: 7262 0000 005a 0867 726f 7570 5f62 7972  rb...Z.group_byr
-000025c0: 2400 0000 7247 0000 0072 6300 0000 675f  $...rG...rc...g_
-000025d0: 75bc 7ebf bf2f 4072 0100 0000 7252 0000  u.~../@r....rR..
-000025e0: 0072 2500 0000 2905 da05 4174 6976 6f75  .r%...)...Ativou
-000025f0: 1000 0000 5072 65c3 a76f 2061 204d 6572  ....Pre..o a Mer
-00002600: 6361 646f fa0d 5265 746f 726e 6f20 616e  cado..Retorno an
-00002610: 7561 6cf5 1400 0000 4465 7376 696f 2070  ual.....Desvio p
-00002620: 6164 72c3 a36f 2061 6e75 616c fa0d 5265  adr..o anual..Re
-00002630: 746f 726e 6f20 746f 7461 6c72 1500 0000  torno totalr....
-00002640: a901 da05 696e 6465 7875 1000 0000 5469  ....indexu....Ti
-00002650: 636b 6572 2069 6e76 c3a1 6c69 646f 7519  cker inv..lidou.
-00002660: 0000 0056 6f63 c3aa 2064 6967 6974 6f75  ...Voc.. digitou
-00002670: 2075 6d61 206c 6973 7461 3a20 2904 7279   uma lista: ).ry
-00002680: 0000 0072 7a00 0000 727b 0000 0072 7c00  ...rz...r{...r|.
-00002690: 0000 752f 0000 0054 6970 6f20 696e 76c3  ..u/...Tipo inv.
-000026a0: a16c 6964 6f2e 2044 6967 6974 6520 756d  .lido. Digite um
-000026b0: 6120 7374 7269 6e67 206f 7520 756d 6120  a string ou uma 
-000026c0: 6c69 7374 612e 4e29 10da 0a69 7369 6e73  lista.N)...isins
-000026d0: 7461 6e63 65da 0373 7472 722e 0000 0072  tance..strr....r
-000026e0: 2900 0000 7264 0000 0072 2a00 0000 722b  )...rd...r*...r+
-000026f0: 0000 0072 6c00 0000 7257 0000 0072 7300  ...rl...rW...rs.
-00002700: 0000 722f 0000 0072 4200 0000 7243 0000  ..r/...rB...rC..
-00002710: 0072 3d00 0000 da03 6c65 6eda 0663 6f6e  .r=.....len..con
-00002720: 6361 7429 1172 7700 0000 725e 0000 0072  cat).rw...r^...r
-00002730: 5f00 0000 da05 6461 646f 73da 0464 6174  _.....dados..dat
-00002740: 615a 0b76 616c 7565 4d61 726b 6574 da05  aZ.valueMarket..
-00002750: 636c 6f73 655a 0e72 6574 6f72 6e6f 5f64  closeZ.retorno_d
-00002760: 6961 7269 6f5a 0d72 6574 6f72 6e6f 5f61  iarioZ.retorno_a
-00002770: 6e75 616c 5a13 6465 7376 696f 5f70 6164  nualZ.desvio_pad
-00002780: 7261 6f5f 616e 7561 6c5a 0f76 616c 6f72  rao_anualZ.valor
-00002790: 5f69 6e76 6573 7469 646f 5a0b 7661 6c6f  _investidoZ.valo
-000027a0: 725f 6174 7561 6c5a 0d72 6574 6f72 6e6f  r_atualZ.retorno
-000027b0: 5f74 6f74 616c 5a0c 7661 6c75 6553 796d  _totalZ.valueSym
-000027c0: 626f 6c73 5a07 7661 6c75 6544 465a 0773  bolsZ.valueDFZ.s
-000027d0: 696d 626f 6c6f 5a0d 7265 7475 726e 5379  imboloZ.returnSy
-000027e0: 6d62 6f6c 7372 1e00 0000 721e 0000 0072  mbolsr....r....r
-000027f0: 1f00 0000 da0f 6173 7365 745f 706f 7274  ......asset_port
-00002800: 666f 6c69 6f91 0100 0073 6000 0000 000e  folio....s`.....
-00002810: 0a01 0e01 1202 0202 0c01 0803 0803 0803  ................
-00002820: 0c03 0c03 0e03 0e03 0c03 0401 0201 0201  ................
-00002830: 0201 0201 02fb 0406 04fa 0608 0602 0601  ................
-00002840: 1002 0c01 0801 0e01 0801 1203 0803 0803  ................
-00002850: 0c03 0c03 0e03 0e03 0c03 0401 0201 0201  ................
-00002860: 0201 02fc 0405 08fb 0607 1002 0402 7286  ..............r.
-00002870: 0000 007a 2473 746f 636b 732f 7b73 796d  ...z$stocks/{sym
-00002880: 626f 6c7d 2f4d 6172 6b6f 7769 747a 416c  bol}/MarkowitzAl
-00002890: 6c6f 6361 7469 6f6e 6e29 0472 7700 0000  locationn).rw...
-000028a0: da09 7374 6172 5f64 6174 6572 5f00 0000  ..star_dater_...
-000028b0: 7222 0000 0063 0300 0000 0000 0000 0000  r"...c..........
-000028c0: 0000 1100 0000 0900 0000 4300 0000 733a  ..........C...s:
-000028d0: 0100 0074 006a 017c 007c 017c 0264 018d  ...t.j.|.|.|.d..
-000028e0: 0364 0219 007d 037c 03a0 02a1 00a0 03a1  .d...}.|........
-000028f0: 007d 047c 04a0 04a1 007d 0574 05a0 0664  .}.|.....}.t...d
-00002900: 0374 077c 0083 011b 0067 0174 077c 0083  .t.|.....g.t.|..
-00002910: 0114 00a1 017d 0674 05a0 087c 04a0 09a1  .....}.t...|....
-00002920: 007c 0614 00a1 0164 0414 007d 0774 05a0  .|.....d...}.t..
-00002930: 0a74 05a0 0b7c 066a 0c74 05a0 0b7c 057c  .t...|.j.t...|.|
-00002940: 06a1 02a1 02a1 0174 05a0 0a64 04a1 0114  .......t...d....
-00002950: 007d 0864 0574 05a0 0d7c 05a1 0114 007d  .}.d.t...|.....}
-00002960: 0974 056a 0ea0 0f7c 057c 0974 05a0 107c  .t.j...|.|.t...|
-00002970: 056a 1164 0619 00a1 0114 0017 00a1 017d  .j.d...........}
-00002980: 0a74 05a0 1274 077c 0083 0164 0366 02a1  .t...t.|...d.f..
-00002990: 017d 0b74 05a0 0b7c 0a7c 0ba1 0274 05a0  .}.t...|.|...t..
-000029a0: 0b74 05a0 0b7c 0b6a 0c7c 0aa1 027c 0ba1  .t...|.j.|...|..
-000029b0: 021b 007d 0c7c 0ca0 13a1 007d 0c67 007d  ...}.|.....}.g.}
-000029c0: 0d74 1474 077c 0083 0183 0144 005d 2e7d  .t.t.|.....D.].}
-000029d0: 0e64 077c 007c 0e19 009b 0064 087c 0c7c  .d.|.|.....d.|.|
-000029e0: 0e19 0064 0914 0064 0a9b 0464 0b9d 057d  ...d...d...d...}
-000029f0: 0f7c 0da0 157c 0fa1 0101 0071 fa7c 077c  .|...|.....q.|.|
-00002a00: 087c 0d64 0c9c 037d 107c 1053 0029 0d75  .|.d...}.|.S.).u
-00002a10: 2403 0000 0a20 2020 2023 2320 5573 6162  $....    ## Usab
-00002a20: 696c 6964 6164 6573 200a 2020 2020 2d20  ilidades .    - 
-00002a30: 416c 6f63 61c3 a7c3 a36f 2064 6520 4d61  Aloca....o de Ma
-00002a40: 726b 6f77 6974 7a20 c3a9 2075 6d61 2074  rkowitz .. uma t
-00002a50: c3a9 636e 6963 6120 6465 206f 7469 6d69  ..cnica de otimi
-00002a60: 7a61 c3a7 c3a3 6f20 6465 2070 6f72 7466  za....o de portf
-00002a70: c3b3 6c69 6f20 7175 6520 7669 7361 2065  ..lio que visa e
-00002a80: 6e63 6f6e 7472 6172 2061 2063 6f6d 6269  ncontrar a combi
-00002a90: 6e61 c3a7 c3a3 6f20 6964 6561 6c20 6465  na....o ideal de
-00002aa0: 2061 7469 766f 7320 7061 7261 206d 6178   ativos para max
-00002ab0: 696d 697a 6172 206f 2072 6574 6f72 6e6f  imizar o retorno
-00002ac0: 2064 6f20 696e 7665 7374 696d 656e 746f   do investimento
-00002ad0: 2065 6e71 7561 6e74 6f20 6d69 6e69 6d69   enquanto minimi
-00002ae0: 7a61 206f 2072 6973 636f 2e20 0a0a 0a20  za o risco. ... 
-00002af0: 2020 2023 2320 4f20 5265 746f 726e 6f20     ## O Retorno 
-00002b00: 4573 7065 7261 646f 0a20 2020 202d 2072  Esperado.    - r
-00002b10: 6570 7265 7365 6e74 6120 6120 7461 7861  epresenta a taxa
-00002b20: 2064 6520 7265 746f 726e 6f20 6dc3 a964   de retorno m..d
-00002b30: 6961 2071 7565 2073 6520 6573 7065 7261  ia que se espera
-00002b40: 206f 6274 6572 2064 6f20 706f 7274 66c3   obter do portf.
-00002b50: b36c 696f 2064 6520 696e 7665 7374 696d  .lio de investim
-00002b60: 656e 746f 7320 0a0a 2020 2020 2323 204f  entos ..    ## O
-00002b70: 2052 6973 636f 200a 2020 2020 2d20 7265   Risco .    - re
-00002b80: 7072 6573 656e 7461 2061 206d 6564 6964  presenta a medid
-00002b90: 6120 6465 2076 6f6c 6174 696c 6964 6164  a de volatilidad
-00002ba0: 6520 646f 2070 6f72 7466 c3b3 6c69 6f2c  e do portf..lio,
-00002bb0: 206f 7520 7365 6a61 2c20 0a20 2020 2071   ou seja, .    q
-00002bc0: 7561 6e74 6f20 6d61 6973 2069 6e73 74c3  uanto mais inst.
-00002bd0: a176 656c 2066 6f72 206f 2072 6574 6f72  .vel for o retor
-00002be0: 6e6f 2064 6f73 2061 7469 766f 732c 206d  no dos ativos, m
-00002bf0: 6169 6f72 2073 6572 c3a1 206f 2072 6973  aior ser.. o ris
-00002c00: 636f 2064 6f20 706f 7274 66c3 b36c 696f  co do portf..lio
-00002c10: 2063 6f6d 6f20 756d 2074 6f64 6f20 0a0a   como um todo ..
-00002c20: 2020 2020 0a20 2020 200a 2020 2020 0a20      .    .    . 
-00002c30: 2020 2023 2320 5061 72c3 a26d 6574 726f     ## Par..metro
-00002c40: 730a 2020 2020 0a20 2020 202d 2073 796d  s.    .    - sym
-00002c50: 626f 6c73 202d 3e20 5265 6365 6265 2075  bols -> Recebe u
-00002c60: 6d61 206c 6973 7461 2064 6520 6174 6976  ma lista de ativ
-00002c70: 6f73 2070 6172 6120 6275 7363 6172 206e  os para buscar n
-00002c80: 6120 6261 7365 200a 0a20 2020 202d 2073  a base ..    - s
-00002c90: 7461 7274 5f64 6174 6520 2d3e 2044 6174  tart_date -> Dat
-00002ca0: 6120 6465 2049 6e69 6369 6f20 6461 2062  a de Inicio da b
-00002cb0: 7573 6361 2064 6173 2069 6e66 6f73 2028  usca das infos (
-00002cc0: 7072 6563 6f2c 2076 6f6c 756d 652c 2065  preco, volume, e
-00002cd0: 7463 2920 646f 2061 7469 766f 200a 0a20  tc) do ativo .. 
-00002ce0: 2020 202d 2065 6e64 5f64 6174 6520 2d3e     - end_date ->
-00002cf0: 2044 6174 6120 4669 6e61 6c20 7061 7261   Data Final para
-00002d00: 2061 2062 7573 6361 2064 6173 2069 6e66   a busca das inf
-00002d10: 6f73 2028 7072 6563 6f2c 2076 6f6c 756d  os (preco, volum
-00002d20: 652c 2065 7463 2920 646f 2061 7469 766f  e, etc) do ativo
-00002d30: 200a 0a0a 2020 2020 7260 0000 007a 0941   ...    r`...z.A
-00002d40: 646a 2043 6c6f 7365 7215 0000 0072 6300  dj Closer....rc.
-00002d50: 0000 679a 9999 9999 99b9 3f72 0100 0000  ..g.......?r....
-00002d60: 7a08 4f20 6174 6976 6f20 7a15 2064 6576  z.O ativo z. dev
-00002d70: 6520 7365 7220 616c 6f63 6164 6f20 656d  e ser alocado em
-00002d80: 2072 5200 0000 7a03 2e32 667a 0d25 2064   rR...z..2fz.% d
-00002d90: 6120 6361 7274 6569 7261 2903 fa10 5265  a carteira)...Re
-00002da0: 746f 726e 6f20 4573 7065 7261 646f fa11  torno Esperado..
-00002db0: 5269 7363 6f20 6461 2043 6172 7465 6972  Risco da Carteir
-00002dc0: 61fa 1241 6c6f 6361 6361 6f20 4d61 726b  a..Alocacao Mark
-00002dd0: 6f77 6974 7a29 1672 2900 0000 7264 0000  owitz).r)...rd..
-00002de0: 0072 6c00 0000 da06 6472 6f70 6e61 726d  .rl.....dropnarm
-00002df0: 0000 0072 6500 0000 da05 6172 7261 7972  ...re.....arrayr
-00002e00: 8100 0000 7230 0000 0072 5700 0000 7268  ....r0...rW...rh
-00002e10: 0000 00da 0364 6f74 da01 54da 0574 7261  .....dot..T..tra
-00002e20: 6365 5a06 6c69 6e61 6c67 da03 696e 76da  ceZ.linalg..inv.
-00002e30: 0365 7965 da05 7368 6170 65da 046f 6e65  .eye..shape..one
-00002e40: 73da 0766 6c61 7474 656e da05 7261 6e67  s..flatten..rang
-00002e50: 65da 0661 7070 656e 6429 1172 7700 0000  e..append).rw...
-00002e60: 7287 0000 0072 5f00 0000 7283 0000 005a  r....r_...r....Z
-00002e70: 0872 6574 6f72 6e6f 735a 126d 6174 7269  .retornosZ.matri
-00002e80: 7a5f 636f 7661 7269 616e 6369 615a 0570  z_covarianciaZ.p
-00002e90: 6573 6f73 da10 7265 746f 726e 6f5f 6573  esos..retorno_es
-00002ea0: 7065 7261 646f da05 7269 7363 6f5a 076c  perado..riscoZ.l
-00002eb0: 616d 6264 615f 5a07 636f 765f 696e 765a  ambda_Z.cov_invZ
-00002ec0: 0976 6574 6f72 5f75 6e73 5a0b 775f 6d61  .vetor_unsZ.w_ma
-00002ed0: 726b 6f77 6974 7a5a 0d6d 6172 6b6f 7769  rkowitzZ.markowi
-00002ee0: 747a 4c69 7374 da01 695a 0574 6178 6173  tzList..iZ.taxas
-00002ef0: 7233 0000 0072 1e00 0000 721e 0000 0072  r3...r....r....r
-00002f00: 1f00 0000 da14 6d61 726b 6f77 6974 7a5f  ......markowitz_
-00002f10: 616c 6c6f 6361 7469 6f6e fb01 0000 7328  allocation....s(
-00002f20: 0000 0000 1614 030c 0308 031c 0316 0326  ...............&
-00002f30: 030e 0120 0112 0122 0108 0304 0110 0120  ... ..."....... 
-00002f40: 010c 0102 0102 0102 fe06 0672 9a00 0000  ...........r....
-00002f50: 7a23 7374 6f63 6b73 2f7b 7379 6d62 6f6c  z#stocks/{symbol
-00002f60: 7d2f 4d61 726b 6f77 6974 7a41 6c6c 6f63  }/MarkowitzAlloc
-00002f70: 6174 696f 6e7a 0a2f 696e 666f 4675 6e64  ationz./infoFund
-00002f80: 7363 0100 0000 0000 0000 0000 0000 0700  sc..............
-00002f90: 0000 0400 0000 4300 0000 7372 0000 0064  ......C...sr...d
-00002fa0: 017d 0174 00a0 017c 01a1 017d 0274 027c  .}.t...|...}.t.|
-00002fb0: 026a 0364 0283 027d 037c 03a0 0464 03a1  .j.d...}.|...d..
-00002fc0: 0164 0419 007d 0474 05a0 0674 077c 0483  .d...}.t...t.|..
-00002fd0: 01a1 0164 0419 007d 057c 0564 0519 00a0  ...d...}.|.d....
-00002fe0: 0864 0664 0784 00a1 017c 0564 053c 007c  .d.d.....|.d.<.|
-00002ff0: 056a 097c 0564 0519 007c 006b 0219 007d  .j.|.d...|.k...}
-00003000: 067c 0667 0064 08a2 0119 007d 067c 0653  .|.g.d.....}.|.S
-00003010: 0029 0975 ca00 0000 0a20 2020 2023 2320  .).u.....    ## 
-00003020: 5573 6162 696c 6964 6164 650a 2020 2020  Usabilidade.    
-00003030: 2d20 4675 6ec3 a761 6f20 7574 696c 697a  - Fun..ao utiliz
-00003040: 6164 6120 7061 7261 2061 6471 7569 7269  ada para adquiri
-00003050: 7220 6173 2070 7269 6e63 6970 6169 7320  r as principais 
-00003060: 6361 7261 6374 6572 6973 7469 6361 7320  caracteristicas 
-00003070: 6520 696e 666f 726d 61c3 a7c3 b565 7320  e informa....es 
-00003080: 646f 2066 756e 646f 2073 656c 6563 696f  do fundo selecio
-00003090: 6e61 646f 0a0a 2020 2020 2323 2050 6172  nado..    ## Par
-000030a0: c3a2 6d65 7472 6f73 0a0a 2020 2020 2d20  ..metros..    - 
-000030b0: 7379 6d62 6f6c 202d 3e20 4e6f 6d65 2064  symbol -> Nome d
-000030c0: 6f20 4675 6e64 6f20 7061 7261 2066 617a  o Fundo para faz
-000030d0: 6572 2061 2062 7573 6361 200a 0a0a 2020  er a busca ...  
-000030e0: 2020 fa28 6874 7470 733a 2f2f 7777 772e    .(https://www.
-000030f0: 6675 6e64 7365 7870 6c6f 7265 722e 636f  fundsexplorer.co
-00003100: 6d2e 6272 2f72 616e 6b69 6e67 fa0b 6874  m.br/ranking..ht
-00003110: 6d6c 2e70 6172 7365 72da 0574 6162 6c65  ml.parser..table
-00003120: 7201 0000 00f5 1000 0000 43c3 b364 6967  r.........C..dig
-00003130: 6f20 646f 2066 756e 646f 6301 0000 0000  o do fundoc.....
-00003140: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
-00003150: 0000 0073 0800 0000 7c00 6401 1700 5300  ...s....|.d...S.
-00003160: a902 4efa 032e 5341 721e 0000 00a9 01da  ..N...SAr.......
-00003170: 0178 721e 0000 0072 1e00 0000 721f 0000  .xr....r....r...
-00003180: 00da 083c 6c61 6d62 6461 3e4f 0200 00f3  ...<lambda>O....
-00003190: 0000 0000 7a1b 6765 745f 6675 6e64 732e  ....z.get_funds.
-000031a0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-000031b0: 3ea9 0672 9e00 0000 da05 5365 746f 72f5  >..r......Setor.
-000031c0: 0c00 0000 5072 65c3 a76f 2041 7475 616c  ....Pre..o Atual
-000031d0: da09 4469 7669 6465 6e64 6ff5 1100 0000  ..Dividendo.....
-000031e0: 5661 7269 61c3 a7c3 a36f 2050 7265 c3a7  Varia....o Pre..
-000031f0: 6ff5 1000 0000 5265 6e74 6162 2e20 5065  o.....Rentab. Pe
-00003200: 72c3 ad6f 646f 290a da08 7265 7175 6573  r..odo)...reques
-00003210: 7473 da03 6765 7472 0900 0000 da07 636f  ts..getr......co
-00003220: 6e74 656e 74da 0866 696e 645f 616c 6c72  ntent..find_allr
-00003230: 4200 0000 da09 7265 6164 5f68 746d 6c72  B.....read_htmlr
-00003240: 8000 0000 da05 6170 706c 79da 036c 6f63  ......apply..loc
-00003250: 2907 7221 0000 00da 0375 726c da08 7265  ).r!.....url..re
-00003260: 7370 6f6e 7365 da04 736f 7570 729d 0000  sponse..soupr...
-00003270: 00da 0766 756e 6473 4446 da08 7661 6c75  ...fundsDF..valu
-00003280: 6573 4649 721e 0000 0072 1e00 0000 721f  esFIr....r....r.
-00003290: 0000 00da 0967 6574 5f66 756e 6473 3d02  .....get_funds=.
-000032a0: 0000 7312 0000 0000 0d04 010a 010c 010e  ..s.............
-000032b0: 0112 0116 0212 010c 0272 b700 0000 7a12  .........r....z.
-000032c0: 2f63 6f6d 7061 7265 5365 746f 7246 756e  /compareSetorFun
-000032d0: 6473 2902 da05 7365 746f 7272 2200 0000  ds)...setorr"...
-000032e0: 6302 0000 0000 0000 0000 0000 000c 0000  c...............
-000032f0: 0006 0000 0043 0000 0073 1e01 0000 6401  .....C...s....d.
-00003300: 7d02 7400 a001 7c02 a101 7d03 7402 7c03  }.t...|...}.t.|.
-00003310: 6a03 6402 8302 7d04 7c04 a004 6403 a101  j.d...}.|...d...
-00003320: 6404 1900 7d05 7405 a006 7407 7c05 8301  d...}.t...t.|...
-00003330: a101 6404 1900 7d06 7408 7c06 6405 8302  ..d...}.t.|.d...
-00003340: 0100 7c01 6406 1b00 7d01 7c06 6a09 7c06  ..|.d...}.|.j.|.
-00003350: 6405 1900 6406 1b00 7c01 6b04 1900 7d07  d...d...|.k...}.
-00003360: 7c07 6700 6407 a201 1900 7d07 7c07 a00a  |.g.d.....}.|...
-00003370: a100 7d07 7c07 6405 1900 a00b a100 7d08  ..}.|.d.......}.
-00003380: 7c00 6408 6b02 72aa 6409 7d00 7c07 6a09  |.d.k.r.d.}.|.j.
-00003390: 7c07 640a 1900 7c00 6b02 1900 6405 1900  |.d...|.k...d...
-000033a0: a00b a100 7d09 6e42 7c00 640b 6b02 72d2  ....}.nB|.d.k.r.
-000033b0: 640c 7d00 7c07 6a09 7c07 640a 1900 7c00  d.}.|.j.|.d...|.
-000033c0: 6b02 1900 6405 1900 a00b a100 7d09 6e1a  k...d.......}.n.
-000033d0: 7c07 6a09 7c07 640a 1900 7c00 6b02 1900  |.j.|.d...|.k...
-000033e0: 6405 1900 a00b a100 7d09 7c07 6405 1900  d.......}.|.d...
-000033f0: a00c a100 7d0a 7405 a00d 7c08 6701 7c09  ....}.t...|.g.|.
-00003400: 6701 7c0a 6701 640d 9c03 a101 7d0b 7c0b  g.|.g.d.....}.|.
-00003410: a00e 640e a101 7d0b 7c0b 5300 290f 7506  ..d...}.|.S.).u.
-00003420: 0300 000a 2020 2020 2323 2055 7361 6269  ....    ## Usabi
-00003430: 6c69 6461 6465 0a20 2020 200a 2020 2020  lidade.    .    
-00003440: 2d20 4675 6ec3 a761 6f20 7175 6520 7574  - Fun..ao que ut
-00003450: 696c 697a 6120 6173 206d 6574 7269 6361  iliza as metrica
-00003460: 7320 6520 6d65 6469 6173 2064 6f73 2066  s e medias dos f
-00003470: 756e 646f 2063 6f6d 2062 6173 6520 6e6f  undo com base no
-00003480: 2073 6575 2053 6574 6f72 2070 6172 6120   seu Setor para 
-00003490: 756d 6120 616e 616c 6973 6520 6d61 6973  uma analise mais
-000034a0: 2072 6573 7472 6974 610a 2020 2020 0a20   restrita.    . 
-000034b0: 2020 2023 2320 5061 72c3 a26d 6574 726f     ## Par..metro
-000034c0: 730a 2020 2020 0a20 2020 202d 2072 656e  s.    .    - ren
-000034d0: 7461 6269 6c69 6461 6465 5f6d 696e 202d  tabilidade_min -
-000034e0: 3e20 5661 6c6f 7220 656d 2025 2070 6172  > Valor em % par
-000034f0: 6120 6275 7363 6172 2061 2072 656e 7461  a buscar a renta
-00003500: 6269 6c69 6461 6465 206d 696e 696d 6120  bilidade minima 
-00003510: 646f 2066 756e 646f 2065 7363 6f6c 6869  do fundo escolhi
-00003520: 646f 0a20 2020 202d 2073 6574 6f72 202d  do.    - setor -
-00003530: 3e20 5365 746f 7265 7320 6465 2066 756e  > Setores de fun
-00003540: 646f 7320 7175 6520 706f 6465 7261 6d20  dos que poderam 
-00003550: 7365 7220 6573 636f 6c68 6964 6f73 2c20  ser escolhidos, 
-00003560: 7365 6775 6520 6120 6c69 7374 613a 0a20  segue a lista:. 
-00003570: 2020 200a 2020 2020 6060 600a 2020 2020     .    ```.    
-00003580: 5469 706f 7353 6574 6f72 6573 3a0a 2020  TiposSetores:.  
-00003590: 2020 2d20 436f 7270 6f72 6174 6976 6173    - Corporativas
-000035a0: 203d 2022 4c61 6a65 7320 436f 7270 6f72   = "Lajes Corpor
-000035b0: 6174 6976 6173 2220 0a20 2020 202d 204d  ativas" .    - M
-000035c0: 6f62 696c 6961 7269 6f73 203d 2022 54c3  obiliarios = "T.
-000035d0: ad74 756c 6f73 2065 2056 616c 2e20 4d6f  .tulos e Val. Mo
-000035e0: 622e 220a 2020 2020 2d20 5368 6f70 7069  b.".    - Shoppi
-000035f0: 6e67 7320 3d20 2253 686f 7070 696e 6773  ngs = "Shoppings
-00003600: 220a 2020 2020 2d20 48c3 ad62 7269 646f  ".    - H..brido
-00003610: 203d 2027 48c3 ad62 7269 646f 270a 2020   = 'H..brido'.  
-00003620: 2020 2d20 5265 6e64 6120 3d20 2752 656e    - Renda = 'Ren
-00003630: 6461 270a 2020 2020 2d20 4c6f 67c3 ad73  da'.    - Log..s
-00003640: 7469 6361 203d 2027 4c6f 67c3 ad73 7469  tica = 'Log..sti
-00003650: 6361 270a 2020 2020 2d20 486f 7370 6974  ca'.    - Hospit
-00003660: 616c 203d 2027 486f 7370 6974 616c 270a  al = 'Hospital'.
-00003670: 2020 2020 2d20 5265 7369 6465 6e63 6961      - Residencia
-00003680: 6c20 3d20 2752 6573 6964 656e 6369 616c  l = 'Residencial
-00003690: 270a 2020 2020 2d20 4f75 7472 6f73 203d  '.    - Outros =
-000036a0: 2027 4f75 7472 6f73 270a 0a20 2020 2060   'Outros'..    `
-000036b0: 6060 0a20 2020 2023 2320 4578 656d 706c  ``.    ## Exempl
-000036c0: 6f3a 0a20 2020 200a 2020 2020 6060 600a  o:.    .    ```.
-000036d0: 2020 2020 3e3e 3e20 6262 2e63 6f6d 7061      >>> bb.compa
-000036e0: 7265 5f73 6574 6f72 5f66 756e 6473 2873  re_setor_funds(s
-000036f0: 6574 6f72 3d27 436f 7270 6f72 6174 6976  etor='Corporativ
-00003700: 6173 272c 2072 656e 7461 6269 6c69 6461  as', rentabilida
-00003710: 6465 5f6d 696e 203d 2033 290a 2020 2020  de_min = 3).    
-00003720: 6060 600a 0a20 2020 2072 9b00 0000 729c  ```..    r....r.
-00003730: 0000 0072 9d00 0000 7201 0000 0072 aa00  ...r....r....r..
-00003740: 0000 7252 0000 0072 a500 0000 5a0c 436f  ..rR...r....Z.Co
-00003750: 7270 6f72 6174 6976 6173 7a12 4c61 6a65  rporativasz.Laje
-00003760: 7320 436f 7270 6f72 6174 6976 6173 72a6  s Corporativasr.
-00003770: 0000 005a 0b4d 6f62 696c 6961 7269 6f73  ...Z.Mobiliarios
-00003780: 7514 0000 0054 c3ad 7475 6c6f 7320 6520  u....T..tulos e 
-00003790: 5661 6c2e 204d 6f62 2e29 0375 2a00 0000  Val. Mob.).u*...
-000037a0: 5265 6e74 6162 696c 6964 6164 6520 4dc3  Rentabilidade M.
-000037b0: a964 6961 2064 6f73 2046 4949 7320 5365  .dia dos FIIs Se
-000037c0: 6c65 6369 6f6e 6164 6f73 751f 0000 0052  lecionadosu....R
-000037d0: 656e 7461 6269 6c69 6461 6465 204d c3a9  entabilidade M..
-000037e0: 6469 6120 646f 204d 6572 6361 646f 7537  dia do Mercadou7
-000037f0: 0000 0044 6573 7669 6f20 5061 6472 c3a3  ...Desvio Padr..
-00003800: 6f20 6461 7320 5265 6e74 6162 696c 6964  o das Rentabilid
-00003810: 6164 6573 2064 6f73 2046 4949 7320 5365  ades dos FIIs Se
-00003820: 6c65 6369 6f6e 6164 6f73 7a20 4f20 7365  lecionadosz O se
-00003830: 746f 722f 7661 6c6f 7220 6e61 6f20 666f  tor/valor nao fo
-00003840: 6920 656e 636f 6e74 7261 646f 290f 72ab  i encontrado).r.
-00003850: 0000 0072 ac00 0000 7209 0000 0072 ad00  ...r....r....r..
-00003860: 0000 72ae 0000 0072 4200 0000 72af 0000  ..r....rB...r...
-00003870: 0072 8000 0000 7220 0000 0072 b100 0000  .r....r ...r....
-00003880: 728b 0000 0072 5700 0000 7273 0000 0072  r....rW...rs...r
-00003890: 4300 0000 5a06 6669 6c6c 6e61 290c 72b8  C...Z.fillna).r.
-000038a0: 0000 005a 1172 656e 7461 6269 6c69 6461  ...Z.rentabilida
-000038b0: 6465 5f6d 696e 72b2 0000 0072 b300 0000  de_minr....r....
-000038c0: 72b4 0000 0072 9d00 0000 72b5 0000 0072  r....r....r....r
-000038d0: b600 0000 5a13 7265 6e74 6162 696c 6964  ....Z.rentabilid
-000038e0: 6164 655f 6d65 6469 615a 1572 656e 7461  ade_mediaZ.renta
-000038f0: 6269 6c69 6461 6465 5f6d 6572 6361 646f  bilidade_mercado
-00003900: da0d 6465 7376 696f 5f70 6164 7261 6f5a  ..desvio_padraoZ
-00003910: 0a72 6573 756c 7461 646f 7372 1e00 0000  .resultadosr....
-00003920: 721e 0000 0072 1f00 0000 da13 636f 6d70  r....r......comp
-00003930: 6172 655f 7365 746f 725f 6675 6e64 735d  are_setor_funds]
-00003940: 0200 0073 3400 0000 0022 0401 0a01 0c01  ...s4...."......
-00003950: 0e01 1202 0a01 0801 1601 0c01 0801 0c01  ................
-00003960: 0801 0401 1c01 0801 0401 1c02 1a02 0c02  ................
-00003970: 0401 0401 0401 04fd 0806 0a02 72ba 0000  ............r...
-00003980: 007a 0d2f 636f 6d70 6172 6546 756e 6473  .z./compareFunds
-00003990: 2901 7222 0000 0063 0300 0000 0000 0000  ).r"...c........
-000039a0: 0000 0000 1200 0000 0400 0000 4300 0000  ............C...
-000039b0: 734a 0100 007c 0172 bc7c 0264 016b 0372  sJ...|.r.|.d.k.r
-000039c0: bc64 027d 0374 00a0 017c 03a1 017d 0474  .d.}.t...|...}.t
-000039d0: 027c 046a 0364 0383 027d 057c 05a0 0464  .|.j.d...}.|...d
-000039e0: 04a1 0164 0519 007d 0674 05a0 0674 077c  ...d...}.t...t.|
-000039f0: 0683 01a1 0164 0519 007d 077c 0764 0619  .....d...}.|.d..
-00003a00: 00a0 0864 0764 0884 00a1 017c 0764 063c  ...d.d.....|.d.<
-00003a10: 007c 0767 0064 09a2 0119 007d 077c 076a  .|.g.d.....}.|.j
-00003a20: 0964 0667 0164 0a8d 017d 077c 076a 0a7c  .d.g.d...}.|.j.|
-00003a30: 0764 0619 007c 016b 0219 007d 087c 076a  .d...|.k...}.|.j
-00003a40: 0a7c 0764 0619 007c 026b 0219 007d 0974  .|.d...|.k...}.t
-00003a50: 05a0 0b7c 087c 0967 02a1 017d 0a7c 0a6a  ...|.|.g...}.|.j
-00003a60: 0c72 b874 0d64 0b83 0101 006e 047c 0a53  .r.t.d.....n.|.S
-00003a70: 007c 0064 0175 0072 ca67 007d 006e 7c64  .|.d.u.r.g.}.n|d
-00003a80: 0c7d 0b64 0d7d 0c7c 0044 005d 3a7d 0d74  .}.d.}.|.D.]:}.t
-00003a90: 0ea0 0f7c 0da1 017d 0e7c 0e6a 1064 0e64  ...|...}.|.j.d.d
-00003aa0: 0f8d 017d 0f7c 0f64 1019 00a0 11a1 00a0  ...}.|.d........
-00003ab0: 12a1 007d 107c 107c 0b6b 0472 d67c 107d  ...}.|.|.k.r.|.}
-00003ac0: 0b7c 0d7d 0c71 d674 056a 137c 0c7c 0b64  .|.}.q.t.j.|.|.d
-00003ad0: 1114 0064 129c 0274 147c 0083 0167 0164  ...d...t.|...g.d
-00003ae0: 138d 027d 117c 116a 0c90 0172 4274 0d64  ...}.|.j...rBt.d
-00003af0: 1483 0101 006e 047c 1153 0064 0153 0029  .....n.|.S.d.S.)
-00003b00: 1575 2403 0000 0a20 2020 2023 2320 5573  .u$....    ## Us
-00003b10: 6162 696c 6964 6164 650a 2020 2020 0a20  abilidade.    . 
-00003b20: 2020 202d 2046 756e c3a7 616f 2071 7565     - Fun..ao que
-00003b30: 2072 6561 6c69 7a61 2061 2063 6f6d 7061   realiza a compa
-00003b40: 7261 c3a7 616f 2065 6e74 7265 2064 6f69  ra..ao entre doi
-00003b50: 7320 6675 6e64 6f73 2c20 7365 6a61 2066  s fundos, seja f
-00003b60: 6569 7461 2061 2072 6571 7569 7369 c3a7  eita a requisi..
-00003b70: 616f 2064 6f73 2066 756e 646f 7320 7669  ao dos fundos vi
-00003b80: 6120 6c69 7374 6120 6f75 2075 6e69 636f  a lista ou unico
-00003b90: 7320 0a20 2020 202d 2052 6571 7569 7369  s .    - Requisi
-00003ba0: c3a7 616f 204c 6973 7461 733a 2052 6574  ..ao Listas: Ret
-00003bb0: 6f72 6e61 206f 2066 756e 646f 2063 6f6d  orna o fundo com
-00003bc0: 206d 6169 6f72 2070 6f72 6365 6e74 6167   maior porcentag
-00003bd0: 656d 2064 6520 7269 7363 6f20 2861 2076  em de risco (a v
-00003be0: 6172 6961 c3a7 c3a3 6f20 7065 7263 656e  aria....o percen
-00003bf0: 7475 616c 2064 6f73 2070 7265 c3a7 6f73  tual dos pre..os
-00003c00: 2064 6f73 2061 7469 766f 732c 2063 616c   dos ativos, cal
-00003c10: 6375 6c6f 2072 6561 6c69 7a61 646f 2063  culo realizado c
-00003c20: 6f6d 2062 6173 6520 6e6f 2064 6573 7669  om base no desvi
-00003c30: 6f20 7061 6472 c3a3 6f29 0a20 2020 202d  o padr..o).    -
-00003c40: 2052 6571 7569 7369 c3a7 616f 2055 6e69   Requisi..ao Uni
-00003c50: 6361 3a20 5265 746f 726e 6120 756d 2044  ca: Retorna um D
-00003c60: 6174 6166 7261 6d65 2063 6f6d 2061 7320  ataframe com as 
-00003c70: 7072 696e 6369 7061 6973 2069 6e66 6f72  principais infor
-00003c80: 6d61 c3a7 6f65 7320 646f 7320 6675 6e64  ma..oes dos fund
-00003c90: 6f73 2c20 6166 696d 2064 6520 756d 6120  os, afim de uma 
-00003ca0: 636f 6d70 6172 61c3 a761 6f20 656e 7472  compara..ao entr
-00003cb0: 6520 7365 7573 2076 616c 6f72 6573 200a  e seus valores .
-00003cc0: 0a20 2020 200a 2020 2020 2323 2050 6172  .    .    ## Par
-00003cd0: c3a2 6d65 7472 6f73 0a20 2020 200a 2020  ..metros.    .  
-00003ce0: 2020 2d20 6c69 7374 6675 6e64 202d 3e20    - listfund -> 
-00003cf0: 4c69 7374 6120 646f 7320 6675 6e64 6f73  Lista dos fundos
-00003d00: 2070 6172 6120 616e 616c 6973 6520 6465   para analise de
-00003d10: 2072 6973 636f 0a20 2020 202d 2066 756e   risco.    - fun
-00003d20: 645f 3120 2d3e 2050 7269 6d65 6972 6f20  d_1 -> Primeiro 
-00003d30: 6675 6e64 6f20 7061 7261 2061 6e61 6c69  fundo para anali
-00003d40: 7365 2075 6e69 6361 0a20 2020 202d 2066  se unica.    - f
-00003d50: 756e 645f 3220 2d3e 2053 6567 756e 646f  und_2 -> Segundo
-00003d60: 2066 756e 646f 2070 6172 6120 616e 616c   fundo para anal
-00003d70: 6973 6520 756e 6963 610a 2020 2020 0a20  ise unica.    . 
-00003d80: 2020 2023 2320 4578 656d 706c 6f73 3a0a     ## Exemplos:.
-00003d90: 2020 2020 0a20 2020 2060 6060 0a20 2020      .    ```.   
-00003da0: 203e 3e3e 2062 622e 636f 6d70 6172 655f   >>> bb.compare_
-00003db0: 6675 6e64 7328 6c69 7374 6675 6e64 3d20  funds(listfund= 
-00003dc0: 6c69 7374 2920 0a20 2020 2020 2020 2020  list) .         
-00003dd0: 2020 2020 2020 2020 2020 206f 750a 2020             ou.  
-00003de0: 2020 3e3e 3e20 6262 2e63 6f6d 7061 7265    >>> bb.compare
-00003df0: 5f66 756e 6473 2866 756e 645f 313d 2027  _funds(fund_1= '
-00003e00: 6675 6e64 3127 2c20 6675 6e64 5f32 3d20  fund1', fund_2= 
-00003e10: 2766 756e 6432 2729 0a20 2020 2060 6060  'fund2').    ```
-00003e20: 0a20 2020 200a 2020 2020 4e72 9b00 0000  .    .    Nr....
-00003e30: 729c 0000 0072 9d00 0000 7201 0000 0072  r....r....r....r
-00003e40: 9e00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00003e50: 0001 0000 0002 0000 0053 0000 0073 0800  .........S...s..
-00003e60: 0000 7c00 6401 1700 5300 729f 0000 0072  ..|.d...S.r....r
-00003e70: 1e00 0000 72a1 0000 0072 1e00 0000 721e  ....r....r....r.
-00003e80: 0000 0072 1f00 0000 72a3 0000 00c6 0200  ...r....r.......
-00003e90: 0072 a400 0000 7a1f 636f 6d70 6172 655f  .r....z.compare_
-00003ea0: 6675 6e64 732e 3c6c 6f63 616c 733e 2e3c  funds.<locals>.<
-00003eb0: 6c61 6d62 6461 3e29 0872 9e00 0000 72a6  lambda>).r....r.
-00003ec0: 0000 0072 a700 0000 72a8 0000 0072 a900  ...r....r....r..
-00003ed0: 0000 72aa 0000 007a 0e44 6976 6964 656e  ..r....z.Dividen
-00003ee0: 6420 5969 656c 647a 1144 5920 2833 4d29  d Yieldz.DY (3M)
-00003ef0: 2041 6375 6d75 6c61 646f 2901 5a06 7375   Acumulado).Z.su
-00003f00: 6273 6574 753e 0000 004e 616f 2066 6f72  bsetu>...Nao for
-00003f10: 616d 2061 7072 6573 656e 7461 646f 2064  am apresentado d
-00003f20: 6164 6f73 2064 6f73 2066 756e 646f 7320  ados dos fundos 
-00003f30: 7061 7261 2076 6572 6966 6963 61c3 a761  para verifica..a
-00003f40: 6f20 756e 6963 6172 2500 0000 7217 0000  o unicar%...r...
-00003f50: 0072 4d00 0000 723b 0000 0072 4700 0000  .rM...r;...rG...
-00003f60: 7252 0000 0029 025a 0446 756e 647a 0c4d  rR...).Z.Fundz.M
-00003f70: 6178 2072 6973 6b20 2825 2972 7d00 0000  ax risk (%)r}...
-00003f80: 7542 0000 004e 616f 2066 6f72 616d 2061  uB...Nao foram a
-00003f90: 7072 6573 656e 7461 646f 2064 6164 6f73  presentado dados
-00003fa0: 2064 6f73 2066 756e 646f 7320 7061 7261   dos fundos para
-00003fb0: 2076 6572 6966 6963 61c3 a761 6f20 6dc3   verifica..ao m.
-00003fc0: ba6c 7469 706c 6129 1572 ab00 0000 72ac  .ltipla).r....r.
-00003fd0: 0000 0072 0900 0000 72ad 0000 0072 ae00  ...r....r....r..
-00003fe0: 0000 7242 0000 0072 af00 0000 7280 0000  ..rB...r....r...
-00003ff0: 0072 b000 0000 da0f 6472 6f70 5f64 7570  .r......drop_dup
-00004000: 6c69 6361 7465 7372 b100 0000 7282 0000  licatesr....r...
-00004010: 0072 4000 0000 722e 0000 0072 2900 0000  .r@...r....r)...
-00004020: 722a 0000 0072 3f00 0000 726c 0000 0072  r*...r?...rl...r
-00004030: 7300 0000 7243 0000 0072 8100 0000 2912  s...rC...r....).
-00004040: 5a08 6c69 7374 6675 6e64 5a06 6675 6e64  Z.listfundZ.fund
-00004050: 5f31 5a06 6675 6e64 5f32 72b2 0000 0072  _1Z.fund_2r....r
-00004060: b300 0000 72b4 0000 0072 9d00 0000 72b5  ....r....r....r.
-00004070: 0000 005a 0566 756e 6431 5a05 6675 6e64  ...Z.fund1Z.fund
-00004080: 32da 0475 6e69 745a 096d 6178 5f72 6973  2..unitZ.max_ris
-00004090: 636f 5a10 7469 636b 6572 5f6d 6178 5f72  coZ.ticker_max_r
-000040a0: 6973 636f 7278 0000 005a 0566 756e 646f  iscorx...Z.fundo
-000040b0: 721d 0000 0072 b900 0000 5a09 7661 6c75  r....r....Z.valu
-000040c0: 6572 6973 6b72 1e00 0000 721e 0000 0072  eriskr....r....r
-000040d0: 1f00 0000 da0d 636f 6d70 6172 655f 6675  ......compare_fu
-000040e0: 6e64 73a7 0200 0073 4400 0000 0019 0c01  nds....sD.......
-000040f0: 0401 0a01 0c01 0e01 1201 1601 0c01 0e02  ................
-00004100: 1201 1202 0e01 0601 0a02 0402 0801 0602  ................
-00004110: 0401 0401 0801 0a01 0c01 1001 0801 0401  ................
-00004120: 0602 0601 06ff 0401 08ff 0603 0801 0a02  ................
-00004130: 72bd 0000 007a 0b2f 6265 7374 4173 7365  r....z./bestAsse
-00004140: 7473 6301 0000 0000 0000 0000 0000 0019  tsc.............
-00004150: 0000 0005 0000 0043 0000 0073 fa02 0000  .......C...s....
-00004160: 6401 7d01 7400 a001 7c01 a101 7d02 7c02  d.}.t...|...}.|.
-00004170: 6a02 6402 6b03 7224 7403 6403 8301 0100  j.d.k.r$t.d.....
-00004180: 9002 6ed2 7404 7c02 6a05 6404 8302 7d03  ..n.t.|.j.d...}.
-00004190: 7c03 a006 6405 a101 6406 1900 7d04 7407  |...d...d...}.t.
-000041a0: 6a08 7409 7c04 8301 6407 6408 6409 8d03  j.t.|...d.d.d...
-000041b0: 6406 1900 7d05 7c05 640a 1900 a00a 640b  d...}.|.d.....d.
-000041c0: 640c 8400 a101 7c05 640a 3c00 7403 640d  d.....|.d.<.t.d.
-000041d0: 8301 0100 740b 6a0c 7c05 640a 1900 a00d  ....t.j.|.d.....
-000041e0: a100 640e 640f 8d02 6410 1900 7d06 6411  ..d.d...d...}.d.
-000041f0: 6412 8400 7d07 6413 6414 8400 7d08 6900  d...}.d.d...}.i.
-00004200: 7d09 6900 7d0a 7c06 6a0e 4400 5d24 7d0b  }.i.}.|.j.D.]$}.
-00004210: 7c06 7c0b 1900 7d0c 7c07 7c0c 8301 7c09  |.|...}.|.|...|.
-00004220: 7c0b 3c00 7c08 7c0c 8301 7c0a 7c0b 3c00  |.<.|.|...|.|.<.
-00004230: 71ac 7c00 6415 6b02 9001 7288 6700 7d0d  q.|.d.k...r.g.}.
-00004240: 7c06 6a0e 4400 5d26 7d0b 7c09 7c0b 1900  |.j.D.]&}.|.|...
-00004250: 6416 6b04 72e6 7c0a 7c0b 1900 6417 6b04  d.k.r.|.|...d.k.
-00004260: 72e6 7c0d a00f 7c0b a101 0100 71e6 7407  r.|...|.....q.t.
-00004270: 6a10 7c0d 6418 6701 6419 8d02 7d0e 7403  j.|.d.g.d...}.t.
-00004280: 641a 8301 0100 7411 7c0d 7412 7413 641b  d.....t.|.t.t.d.
-00004290: 8d03 7d0f 7c0f 6701 7d0f 7407 a010 7c0f  ..}.|.g.}.t...|.
-000042a0: a101 7d10 7c10 a014 641c a101 7d10 7c10  ..}.|...d...}.|.
-000042b0: 641d 1900 a015 a100 a016 a100 7c10 641d  d...........|.d.
-000042c0: 3c00 7c10 641e 1900 a015 a100 a016 a100  <.|.d...........
-000042d0: 7c10 641e 3c00 7c10 6a17 9001 7280 6e04  |.d.<.|.j...r.n.
-000042e0: 7c10 5300 9001 6e6e 7c00 641f 6b02 9002  |.S...nn|.d.k...
-000042f0: 7242 6700 7d11 7c06 6a0e 4400 5d2c 7d0b  rBg.}.|.j.D.],}.
-00004300: 7c09 7c0b 1900 6420 6b04 9001 729c 7c0a  |.|...d k...r.|.
-00004310: 7c0b 1900 6421 6b00 9001 729c 7c11 a00f  |...d!k...r.|...
-00004320: 7c0b a101 0100 9001 719c 7407 6a10 7c11  |.......q.t.j.|.
-00004330: 6422 6701 6419 8d02 7d12 7403 641a 8301  d"g.d...}.t.d...
-00004340: 0100 7411 7c11 7412 7413 641b 8d03 7d13  ..t.|.t.t.d...}.
-00004350: 7c13 6701 7d13 7407 a010 7c13 a101 7d14  |.g.}.t...|...}.
-00004360: 7c14 a014 641c a101 7d14 7c14 641d 1900  |...d...}.|.d...
-00004370: a015 a100 a016 a100 7c14 641d 3c00 7c14  ........|.d.<.|.
-00004380: 641e 1900 a015 a100 a016 a100 7c14 641e  d...........|.d.
-00004390: 3c00 7c14 6a17 9002 723c 6e04 7c14 5300  <.|.j...r<n.|.S.
-000043a0: 6eb4 7c00 6423 6b02 9002 72ee 6700 7d15  n.|.d#k...r.g.}.
-000043b0: 7c06 6a0e 4400 5d1e 7d0b 7c0a 7c0b 1900  |.j.D.].}.|.|...
-000043c0: 6417 6b00 9002 7256 7c15 a00f 7c0b a101  d.k...rV|...|...
-000043d0: 0100 9002 7156 7407 6a10 7c15 6424 6701  ....qVt.j.|.d$g.
-000043e0: 6419 8d02 7d16 7403 641a 8301 0100 7411  d...}.t.d.....t.
-000043f0: 7c15 7412 7413 641b 8d03 7d17 7c17 6701  |.t.t.d...}.|.g.
-00004400: 7d17 7407 a010 7c17 a101 7d18 7c18 a014  }.t...|...}.|...
-00004410: 641c a101 7d18 7c18 641d 1900 a015 a100  d...}.|.d.......
-00004420: a016 a100 7c18 641d 3c00 7c18 641e 1900  ....|.d.<.|.d...
-00004430: a015 a100 a016 a100 7c18 641e 3c00 7c18  ........|.d.<.|.
-00004440: 6a17 9002 72e8 6e04 7c18 5300 6e08 7403  j...r.n.|.S.n.t.
-00004450: 6425 8301 0100 6426 5300 2927 750c 0200  d%....d&S.)'u...
-00004460: 000a 2020 2020 2323 2055 7361 6269 6c69  ..    ## Usabili
-00004470: 6461 6465 0a20 2020 202d 2046 756e c3a7  dade.    - Fun..
-00004480: c3a3 6f20 7175 6520 616e 616c 6973 6120  ..o que analisa 
-00004490: 6f73 2070 7269 6e63 6970 6169 7320 6174  os principais at
-000044a0: 6976 6f73 206c 6973 7461 646f 7320 6e6f  ivos listados no
-000044b0: 206d 6572 6361 646f 2071 7565 2063 6f6d   mercado que com
-000044c0: 2062 6173 6520 6e6f 2070 6572 6669 6c20   base no perfil 
-000044d0: 6573 636f 6c68 6964 6f20 6d6f 7374 7261  escolhido mostra
-000044e0: 2071 7561 6973 2070 6f64 656d 2073 6572   quais podem ser
-000044f0: 2073 7561 7320 6573 636f 6c68 6173 2065   suas escolhas e
-00004500: 2071 7561 6e74 6f73 2070 6f72 6365 6e74   quantos porcent
-00004510: 6f20 7365 2064 6576 6520 7465 7220 6e61  o se deve ter na
-00004520: 2063 6172 7465 6972 610a 2020 2020 0a20   carteira.    . 
-00004530: 2020 2023 2320 5061 72c3 a26d 6574 726f     ## Par..metro
-00004540: 730a 2020 2020 0a20 2020 202d 2070 6572  s.    .    - per
-00004550: 6669 6c20 2d3e 2050 6572 6669 7320 7175  fil -> Perfis qu
-00004560: 6520 706f 6465 6d20 7365 7220 6573 636f  e podem ser esco
-00004570: 6c68 6964 6f73 2070 6172 6120 7265 616c  lhidos para real
-00004580: 697a 6172 2061 2061 6ec3 a16c 6973 652c  izar a an..lise,
-00004590: 2073 6567 7565 2061 206c 6973 7461 3a20   segue a lista: 
-000045a0: 0a0a 2020 2020 0a20 2020 2060 6060 0a20  ..    .    ```. 
-000045b0: 2020 2054 6970 6f50 6572 6669 733a 0a20     TipoPerfis:. 
-000045c0: 2020 202a 2041 6772 6573 7369 766f 0a20     * Agressivo. 
-000045d0: 2020 202a 204d 6f64 6572 6164 6f0a 2020     * Moderado.  
-000045e0: 2020 2a20 436f 6e73 6572 7661 646f 720a    * Conservador.
-000045f0: 2020 2020 0a20 2020 2060 6060 0a20 2020      .    ```.   
-00004600: 200a 2020 2020 2323 2045 7865 6d70 6c6f   .    ## Exemplo
-00004610: 0a20 2020 200a 2020 2020 6060 600a 2020  .    .    ```.  
-00004620: 2020 0a20 2020 203e 3e3e 2061 6c6f 6361    .    >>> aloca
-00004630: 7469 6f6e 203d 2062 6573 745f 6173 7365  tion = best_asse
-00004640: 7473 2870 6572 6669 6c3d 2741 6772 6573  ts(perfil='Agres
-00004650: 7369 766f 2729 0a20 2020 200a 2020 2020  sivo').    .    
-00004660: 6060 600a 2020 2020 0a20 2020 207a 2d68  ```.    .    z-h
-00004670: 7474 7073 3a2f 2f77 7777 2e64 6164 6f73  ttps://www.dados
-00004680: 6465 6d65 7263 6164 6f2e 636f 6d2e 6272  demercado.com.br
-00004690: 2f62 6f6c 7361 2f61 636f 6573 7250 0000  /bolsa/acoesrP..
-000046a0: 007a 3141 6365 7373 6f20 6e65 6761 646f  .z1Acesso negado
-000046b0: 2061 2062 6173 652c 2074 656e 7465 206e   a base, tente n
-000046c0: 6f76 616d 656e 7465 206d 6169 7320 7461  ovamente mais ta
-000046d0: 7264 652e 729c 0000 0072 9d00 0000 7201  rde.r....r....r.
-000046e0: 0000 00fa 012c 7219 0000 00a9 02da 0764  .....,r........d
-000046f0: 6563 696d 616c 5a09 7468 6f75 7361 6e64  ecimalZ.thousand
-00004700: 73f5 0700 0000 43c3 b364 6967 6f63 0100  s.....C..digoc..
-00004710: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00004720: 0000 5300 0000 7308 0000 007c 0064 0117  ..S...s....|.d..
-00004730: 0053 0072 9f00 0000 721e 0000 0072 a100  .S.r....r....r..
-00004740: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00004750: 0072 a300 0000 1503 0000 72a4 0000 007a  .r........r....z
-00004760: 1d62 6573 745f 6173 7365 7473 2e3c 6c6f  .best_assets.<lo
-00004770: 6361 6c73 3e2e 3c6c 616d 6264 613e 7a13  cals>.<lambda>z.
-00004780: 4275 7363 616e 646f 2061 7469 766f 732e  Buscando ativos.
-00004790: 2e2e 2e72 3900 0000 723b 0000 0072 4700  ...r9...r;...rG.
-000047a0: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
-000047b0: 0000 0002 0000 0053 0000 0073 1400 0000  .......S...s....
-000047c0: 7c00 a000 a100 7d01 7c01 a001 a100 7d02  |.....}.|.....}.
-000047d0: 7c02 5300 a901 4e29 0272 6c00 0000 7257  |.S...N).rl...rW
-000047e0: 0000 0029 03da 0670 7265 636f 73da 0772  ...)...precos..r
-000047f0: 6574 6f72 6e6f 5a0d 7265 746f 726e 6f5f  etornoZ.retorno_
-00004800: 6d65 6469 6f72 1e00 0000 721e 0000 0072  medior....r....r
-00004810: 1f00 0000 da10 6361 6c63 756c 6172 5f72  ......calcular_r
-00004820: 6574 6f72 6e6f 1a03 0000 7306 0000 0000  etorno....s.....
-00004830: 0108 0108 017a 2562 6573 745f 6173 7365  .....z%best_asse
-00004840: 7473 2e3c 6c6f 6361 6c73 3e2e 6361 6c63  ts.<locals>.calc
-00004850: 756c 6172 5f72 6574 6f72 6e6f 6301 0000  ular_retornoc...
-00004860: 0000 0000 0000 0000 0003 0000 0002 0000  ................
-00004870: 0053 0000 0073 1400 0000 7c00 a000 a100  .S...s....|.....
-00004880: 7d01 7c01 a001 a100 7d02 7c02 5300 72c2  }.|.....}.|.S.r.
-00004890: 0000 0029 0272 6c00 0000 7273 0000 0029  ...).rl...rs...)
-000048a0: 0372 c300 0000 72c4 0000 0072 9800 0000  .r....r....r....
-000048b0: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
-000048c0: 0e63 616c 6375 6c61 725f 7269 7363 6f20  .calcular_risco 
-000048d0: 0300 0073 0600 0000 0001 0801 0801 7a23  ...s..........z#
-000048e0: 6265 7374 5f61 7373 6574 732e 3c6c 6f63  best_assets.<loc
-000048f0: 616c 733e 2e63 616c 6375 6c61 725f 7269  als>.calcular_ri
-00004900: 7363 6f5a 0941 6772 6573 7369 766f 672d  scoZ.Agressivog-
-00004910: 431c ebe2 361a 3fe7 7b14 ae47 e17a 843f  C...6.?.{..G.z.?
-00004920: 7a12 4174 6976 6f73 2050 2f41 6772 6573  z.Ativos P/Agres
-00004930: 7369 766f a901 da07 636f 6c75 6d6e 737a  sivo....columnsz
-00004940: 3f52 6561 6c69 7a61 6e64 6f20 6361 6c63  ?Realizando calc
-00004950: 756c 6f73 2070 6172 6120 6120 7375 6120  ulos para a sua 
-00004960: 6361 7274 6569 7261 2063 6f6d 2062 6173  carteira com bas
-00004970: 6520 6e6f 2073 6575 2070 6572 6669 6c2e  e no seu perfil.
-00004980: 2902 7287 0000 0072 5f00 0000 728a 0000  ).r....r_...r...
-00004990: 0072 8800 0000 7289 0000 005a 084d 6f64  .r....r....Z.Mod
-000049a0: 6572 6164 6f67 6132 5530 2aa9 333f 67b8  eradoga2U0*.3?g.
-000049b0: 1e85 eb51 b89e 3f7a 1141 7469 766f 7320  ...Q..?z.Ativos 
-000049c0: 502f 4d6f 6465 7261 646f 5a0b 436f 6e73  P/ModeradoZ.Cons
-000049d0: 6572 7661 646f 727a 1441 7469 766f 7320  ervadorz.Ativos 
-000049e0: 502f 436f 6e73 6572 7661 646f 7275 5a00  P/ConservadoruZ.
-000049f0: 0000 5065 7266 696c 206e c3a3 6f20 7265  ..Perfil n..o re
-00004a00: 636f 6e68 6563 6964 6f2c 206f 7320 7065  conhecido, os pe
-00004a10: 7266 6973 2064 6973 706f 6e69 7665 6973  rfis disponiveis
-00004a20: 2065 7374 616f 2070 7265 7365 6e74 6573   estao presentes
-00004a30: 206e 6120 6578 706c 6963 61c3 a7c3 a36f   na explica....o
-00004a40: 2064 6120 6675 6ec3 a7c3 a36f 4e29 1872   da fun....oN).r
-00004a50: ab00 0000 72ac 0000 005a 0b73 7461 7475  ....r....Z.statu
-00004a60: 735f 636f 6465 722e 0000 0072 0900 0000  s_coder....r....
-00004a70: 72ad 0000 0072 ae00 0000 7242 0000 0072  r....r....rB...r
-00004a80: af00 0000 7280 0000 0072 b000 0000 7229  ....r....r....r)
-00004a90: 0000 0072 6400 0000 da06 746f 6c69 7374  ...rd.....tolist
-00004aa0: 72c9 0000 0072 9600 0000 7243 0000 0072  r....r....rC...r
-00004ab0: 9a00 0000 da04 6f6e 6559 da09 6375 7272  ......oneY..curr
-00004ac0: 656e 746c 795a 0765 7870 6c6f 6465 72bb  entlyZ.exploder.
-00004ad0: 0000 0072 8b00 0000 7240 0000 0029 195a  ...r....r@...).Z
-00004ae0: 0670 6572 6669 6c72 b200 0000 72b3 0000  .perfilr....r...
-00004af0: 0072 b400 0000 729d 0000 0072 b500 0000  .r....r....r....
-00004b00: 72c3 0000 0072 c500 0000 72c6 0000 0072  r....r....r....r
-00004b10: c400 0000 7298 0000 00da 0561 7469 766f  ....r......ativo
-00004b20: 5a0c 7072 6563 6f73 5f61 7469 766f 5a09  Z.precos_ativoZ.
-00004b30: 6167 7265 7373 6976 6f5a 0b44 6641 6772  agressivoZ.DfAgr
-00004b40: 6573 7369 766f 5a13 616c 6f63 6174 696f  essivoZ.alocatio
-00004b50: 6e5f 4167 7265 7373 6976 655a 1764 6174  n_AgressiveZ.dat
-00004b60: 6141 6c6f 6361 7469 6f6e 5f41 6772 6573  aAlocation_Agres
-00004b70: 7369 7665 5a08 6d6f 6465 7261 646f 5a0a  siveZ.moderadoZ.
-00004b80: 4466 4d6f 6465 7261 646f 5a12 616c 6f63  DfModeradoZ.aloc
-00004b90: 6174 696f 6e5f 4d6f 6465 7261 6465 5a16  ation_ModeradeZ.
-00004ba0: 6461 7461 416c 6f63 6174 696f 6e5f 4d6f  dataAlocation_Mo
-00004bb0: 6465 7261 6465 5a0b 636f 6e73 6572 7661  deradeZ.conserva
-00004bc0: 646f 725a 0d44 6643 6f6e 7365 7276 6164  dorZ.DfConservad
-00004bd0: 6f72 5a16 616c 6f63 6174 696f 6e5f 436f  orZ.alocation_Co
-00004be0: 6e73 6572 7661 7469 7665 5a1a 6461 7461  nservativeZ.data
-00004bf0: 416c 6f63 6174 696f 6e5f 436f 6e73 6572  Alocation_Conser
-00004c00: 7661 7469 7665 721e 0000 0072 1e00 0000  vativer....r....
-00004c10: 721f 0000 00da 0b62 6573 745f 6173 7365  r......best_asse
-00004c20: 7473 ef02 0000 7386 0000 0000 1e04 010a  ts....s.........
-00004c30: 010a 010c 020c 010e 0118 0116 0108 011a  ................
-00004c40: 0308 0608 0604 0104 010a 0108 010c 010e  ................
-00004c50: 030a 0104 010a 0118 010c 0210 0108 010e  ................
-00004c60: 0106 010a 010a 0414 0114 0208 0102 0208  ................
-00004c70: 020a 0204 010a 011c 010e 0210 0108 010e  ................
-00004c80: 0106 010a 010a 0414 0114 0208 0102 0206  ................
-00004c90: 020a 0204 010a 010e 010e 0110 0208 010e  ................
-00004ca0: 0106 010a 010a 0314 0114 0208 0102 0206  ................
-00004cb0: 0272 ce00 0000 7a11 2f62 6573 7441 7373  .r....z./bestAss
-00004cc0: 6574 7356 616c 7565 7363 0100 0000 0000  etsValuesc......
-00004cd0: 0000 0000 0000 1100 0000 0600 0000 0300  ................
-00004ce0: 0000 733a 0200 0074 00a0 01a1 0001 0074  ..s:...t.......t
-00004cf0: 0283 007d 017c 01a0 0364 01a1 0101 0074  ...}.|...d.....t
-00004d00: 046a 057c 0164 028d 017d 0264 037d 037c  .j.|.d...}.d.}.|
-00004d10: 02a0 067c 03a1 0101 0074 07a0 0864 04a1  ...|.....t...d..
-00004d20: 0101 007c 02a0 0974 0a6a 0b64 05a1 02a0  ...|...t.j.d....
-00004d30: 0ca1 007d 047c 026a 0da0 0e7c 02a0 0974  ...}.|.j...|...t
-00004d40: 0a6a 0f64 06a1 02a1 0101 007c 02a0 0974  .j.d.......|...t
-00004d50: 0a6a 0f64 07a1 02a0 0ca1 007d 057c 02a0  .j.d.......}.|..
-00004d60: 0974 0a6a 1064 08a1 02a0 0ca1 007d 067c  .t.j.d.......}.|
-00004d70: 02a0 0974 0a6a 1064 09a1 027d 077c 07a0  ...t.j.d...}.|..
-00004d80: 1164 0aa1 017d 0874 126a 1374 147c 0883  .d...}.t.j.t.|..
-00004d90: 0164 0b64 0c64 0d8d 037d 097c 0964 0e19  .d.d.d...}.|.d..
-00004da0: 007d 097c 0964 0f64 1067 0219 007d 097c  .}.|.d.d.g...}.|
-00004db0: 09a0 1564 1164 1267 02a1 017d 097c 0964  ...d.d.g...}.|.d
-00004dc0: 0f19 00a0 1664 1364 1484 00a1 017c 0964  .....d.d.....|.d
-00004dd0: 0f3c 0074 176a 187c 0964 0f19 00a0 19a1  .<.t.j.|.d......
-00004de0: 0064 1564 168d 0264 1719 007d 0a7c 0a6a  .d.d...d...}.|.j
-00004df0: 1a64 1864 198d 017d 0a7c 0aa0 1ba1 00a0  .d.d...}.|......
-00004e00: 1ca1 0064 1a14 0089 007c 0aa0 1ba1 00a0  ...d.....|......
-00004e10: 1da1 0074 1ea0 1f64 1aa1 0114 007d 0b74  ...t...d.....}.t
-00004e20: 12a0 2088 007c 0b64 1b9c 02a1 017d 0c7c  .. ..|.d.....}.|
-00004e30: 0c64 1c19 007c 0c64 1d19 001b 007c 0c64  .d...|.d.....|.d
-00004e40: 1e3c 007c 0c6a 2164 1e64 1f64 208d 02a0  .<.|.j!d.d.d ...
-00004e50: 2264 21a1 017d 0c7c 0c64 1e19 007c 0c64  "d!..}.|.d...|.d
-00004e60: 1e19 00a0 23a1 001b 007c 0c64 223c 007c  ....#....|.d"<.|
-00004e70: 0c64 2219 0088 0114 007c 0c64 233c 007c  .d"......|.d#<.|
-00004e80: 0ca0 24a1 007d 0c7c 0c6a 2564 2464 2564  ..$..}.|.j%d$d%d
-00004e90: 269c 0264 278d 017d 0c7c 0c64 2419 0044  &..d'..}.|.d$..D
-00004ea0: 005d 427d 0d74 176a 187c 0d64 1564 168d  .]B}.t.j.|.d.d..
-00004eb0: 027d 0e7c 0e64 1719 006a 2664 2819 007c  .}.|.d...j&d(..|
-00004ec0: 0e64 1719 006a 2664 0e19 0018 007c 0e64  .d...j&d.....|.d
-00004ed0: 1719 006a 2664 0e19 001b 0088 007c 0d3c  ...j&d.......|.<
-00004ee0: 0090 0171 ba87 0087 0166 0264 2964 2a84  ...q.....f.d)d*.
-00004ef0: 087c 0c64 2419 0044 0083 017d 0f7c 0fa0  .|.d$..D...}.|..
-00004f00: 27a1 007d 1074 287c 1083 017d 107c 107c  '..}.t(|...}.|.|
-00004f10: 0c64 2b3c 007c 0c67 0064 2ca2 0119 0053  .d+<.|.g.d,....S
-00004f20: 0029 2d75 1a02 0000 0a20 2020 2023 2320  .)-u.....    ## 
-00004f30: 5573 6162 696c 6964 6164 650a 2020 2020  Usabilidade.    
-00004f40: 2d20 4675 6ec3 a7c3 a36f 2071 7565 2061  - Fun....o que a
-00004f50: 6e61 6c69 7361 206f 7320 6174 6976 6f73  nalisa os ativos
-00004f60: 2064 6f20 4942 4f56 4553 5041 2071 7565   do IBOVESPA que
-00004f70: 2063 6f6d 2062 6173 6520 6e6f 2076 616c   com base no val
-00004f80: 6f72 2064 6520 696e 7665 7374 696d 656e  or de investimen
-00004f90: 746f 2065 7363 6f6c 6869 646f 206d 6f73  to escolhido mos
-00004fa0: 7472 6120 7175 6169 7320 706f 6465 6d20  tra quais podem 
-00004fb0: 7365 7220 7375 6173 2065 7363 6f6c 6861  ser suas escolha
-00004fc0: 732c 206f 2071 7561 6e74 6f20 6972 6120  s, o quanto ira 
-00004fd0: 7465 7220 7175 6520 696e 7665 7374 6972  ter que investir
-00004fe0: 2070 6172 6120 6361 6461 2061 7469 766f   para cada ativo
-00004ff0: 2065 206f 2072 6574 6f72 6e6f 2061 7072   e o retorno apr
-00005000: 6f78 696d 6164 6f20 7061 7261 2063 6164  oximado para cad
-00005010: 6120 756d 2064 656c 6573 200a 0a20 2020  a um deles ..   
-00005020: 202d 2055 7361 6d6f 7320 636f 6d6f 206d   - Usamos como m
-00005030: 6574 6f64 6f20 6465 2063 c3a1 6c63 756c  etodo de c..lcul
-00005040: 6f20 6f20 6120 6d65 6469 6461 2053 6861  o o a medida Sha
-00005050: 7270 6520 7175 6520 6e61 6461 206d 6169  rpe que nada mai
-00005060: 7320 c3a9 2071 7565 2075 6d61 2020 6d65  s .. que uma  me
-00005070: 6469 6461 2064 6520 6465 7365 6d70 656e  dida de desempen
-00005080: 686f 2064 6520 696e 7665 7374 696d 656e  ho de investimen
-00005090: 746f 7320 7175 6520 6c65 7661 2065 6d20  tos que leva em 
-000050a0: 636f 6e73 6964 6572 61c3 a7c3 a36f 206f  considera....o o
-000050b0: 2072 6574 6f72 6e6f 206f 6274 6964 6f20   retorno obtido 
-000050c0: 7065 6c6f 2069 6e76 6573 7469 6d65 6e74  pelo investiment
-000050d0: 6f20 656d 2072 656c 61c3 a7c3 a36f 2061  o em rela....o a
-000050e0: 6f20 7269 7363 6f20 6173 7375 6d69 646f  o risco assumido
-000050f0: 0a20 2020 2023 2320 5061 72c3 a26d 6574  .    ## Par..met
-00005100: 726f 730a 2020 2020 0a20 2020 202d 2076  ros.    .    - v
-00005110: 616c 6f72 202d 3e20 5661 6c6f 7220 646f  alor -> Valor do
-00005120: 2069 6e76 6573 7469 6d65 6e74 6f2c 2070   investimento, p
-00005130: 6f72 2070 6164 72c3 a36f 2030 0a0a 2020  or padr..o 0..  
-00005140: 2020 fa0a 2d2d 6865 6164 6c65 7373 a901    ..--headless..
-00005150: da07 6f70 7469 6f6e 737a 7c68 7474 7073  ..optionsz|https
-00005160: 3a2f 2f77 7777 2e62 332e 636f 6d2e 6272  ://www.b3.com.br
-00005170: 2f70 745f 6272 2f6d 6172 6b65 742d 6461  /pt_br/market-da
-00005180: 7461 2d65 2d69 6e64 6963 6573 2f69 6e64  ta-e-indices/ind
-00005190: 6963 6573 2f69 6e64 6963 6573 2d61 6d70  ices/indices-amp
-000051a0: 6c6f 732f 696e 6469 6365 2d69 626f 7665  los/indice-ibove
-000051b0: 7370 612d 6962 6f76 6573 7061 2d63 6f6d  spa-ibovespa-com
-000051c0: 706f 7369 6361 6f2d 6461 2d63 6172 7465  posicao-da-carte
-000051d0: 6972 612e 6874 6d72 7200 0000 7a1b 6f6e  ira.htmrr...z.on
-000051e0: 6574 7275 7374 2d61 6363 6570 742d 6274  etrust-accept-bt
-000051f0: 6e2d 6861 6e64 6c65 727a 162f 2f2a 5b40  n-handlerz.//*[@
-00005200: 6964 3d22 6276 6d66 5f69 6672 616d 6522  id="bvmf_iframe"
-00005210: 5d7a 152f 2f2a 5b40 6964 3d22 7365 6c65  ]z.//*[@id="sele
-00005220: 6374 5061 6765 225d 7a21 2373 656c 6563  ctPage"]z!#selec
-00005230: 7450 6167 6520 3e20 6f70 7469 6f6e 3a6e  tPage > option:n
-00005240: 7468 2d63 6869 6c64 2834 297a 6c23 6469  th-child(4)zl#di
-00005250: 7643 6f6e 7461 696e 6572 4966 7261 6d65  vContainerIframe
-00005260: 4233 203e 2064 6976 203e 2064 6976 2e63  B3 > div > div.c
-00005270: 6f6c 2d6c 672d 392e 636f 6c2d 3132 2e6f  ol-lg-9.col-12.o
-00005280: 7264 6572 2d32 2e6f 7264 6572 2d6c 672d  rder-2.order-lg-
-00005290: 3120 3e20 666f 726d 203e 2064 6976 3a6e  1 > form > div:n
-000052a0: 7468 2d63 6869 6c64 2834 2920 3e20 6469  th-child(4) > di
-000052b0: 7620 3e20 7461 626c 65da 096f 7574 6572  v > table..outer
-000052c0: 4854 4d4c 72be 0000 0072 1900 0000 72bf  HTMLr....r....r.
-000052d0: 0000 0072 0100 0000 72c1 0000 0075 0600  ...r....r....u..
-000052e0: 0000 41c3 a7c3 a36f e958 0000 00e9 5900  ..A....o.X....Y.
-000052f0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00005300: 0000 0002 0000 0053 0000 0073 0800 0000  .......S...s....
-00005310: 7c00 6401 1700 5300 729f 0000 0072 1e00  |.d...S.r....r..
-00005320: 0000 72a1 0000 0072 1e00 0000 721e 0000  ..r....r....r...
-00005330: 0072 1f00 0000 72a3 0000 009d 0300 0072  .r....r........r
-00005340: a400 0000 7a23 6265 7374 5f61 7373 6574  ....z#best_asset
-00005350: 735f 7661 6c75 652e 3c6c 6f63 616c 733e  s_value.<locals>
-00005360: 2e3c 6c61 6d62 6461 3e72 3900 0000 723b  .<lambda>r9...r;
-00005370: 0000 0072 4700 0000 7215 0000 0029 015a  ...rG...r....).Z
-00005380: 0461 7869 7372 6300 0000 2902 7297 0000  .axisrc...).r...
-00005390: 0072 9800 0000 7297 0000 0072 9800 0000  .r....r....r....
-000053a0: 5a06 7368 6172 7065 4629 015a 0961 7363  Z.sharpeF).Z.asc
-000053b0: 656e 6469 6e67 e906 0000 005a 0861 6c6f  ending.....Z.alo
-000053c0: 6361 6361 6fda 0576 616c 6f72 da06 4174  cacao..valor..At
-000053d0: 6976 6f73 fa13 5174 6420 4e65 6365 7373  ivos..Qtd Necess
-000053e0: 6172 6961 2028 5224 2929 0272 7e00 0000  aria (R$)).r~...
-000053f0: 72d6 0000 0072 c800 0000 7225 0000 0063  r....r....r%...c
-00005400: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00005410: 0500 0000 1300 0000 731a 0000 0069 007c  ........s....i.|
-00005420: 005d 127d 017c 0188 007c 0119 0088 0114  .].}.|...|......
-00005430: 0093 0271 0453 0072 1e00 0000 721e 0000  ...q.S.r....r...
-00005440: 0029 02da 022e 3072 cd00 0000 a902 7297  .)....0r......r.
-00005450: 0000 0072 d600 0000 721e 0000 0072 1f00  ...r....r....r..
-00005460: 0000 da0a 3c64 6963 7463 6f6d 703e c003  ....<dictcomp>..
-00005470: 0000 72a4 0000 007a 2562 6573 745f 6173  ..r....z%best_as
-00005480: 7365 7473 5f76 616c 7565 2e3c 6c6f 6361  sets_value.<loca
-00005490: 6c73 3e2e 3c64 6963 7463 6f6d 703e fa0e  ls>.<dictcomp>..
-000054a0: 5265 746f 726e 6f20 4170 726f 782e 2903  Retorno Aprox.).
-000054b0: 72d7 0000 0072 d800 0000 72dc 0000 0029  r....r....r....)
-000054c0: 29da 1a63 6872 6f6d 6564 7269 7665 725f  )..chromedriver_
-000054d0: 6175 746f 696e 7374 616c 6c65 72da 0769  autoinstaller..i
-000054e0: 6e73 7461 6c6c 7207 0000 00da 0c61 6464  nstallr......add
-000054f0: 5f61 7267 756d 656e 7472 0500 0000 da06  _argumentr......
-00005500: 4368 726f 6d65 72ac 0000 00da 0474 696d  Chromer......tim
-00005510: 65da 0573 6c65 6570 da0c 6669 6e64 5f65  e..sleep..find_e
-00005520: 6c65 6d65 6e74 7208 0000 00da 0249 44da  lementr......ID.
-00005530: 0563 6c69 636b 5a09 7377 6974 6368 5f74  .clickZ.switch_t
-00005540: 6fda 0566 7261 6d65 5a05 5850 4154 48da  o..frameZ.XPATH.
-00005550: 0c43 5353 5f53 454c 4543 544f 52da 0d67  .CSS_SELECTOR..g
-00005560: 6574 5f61 7474 7269 6275 7465 7242 0000  et_attributerB..
-00005570: 0072 af00 0000 7280 0000 0072 3e00 0000  .r....r....r>...
-00005580: 72b0 0000 0072 2900 0000 7264 0000 0072  r....r)...rd...r
-00005590: ca00 0000 728b 0000 0072 6c00 0000 7257  ....r....rl...rW
-000055a0: 0000 0072 7300 0000 7265 0000 0072 6800  ...rs...re...rh.
-000055b0: 0000 7243 0000 005a 0b73 6f72 745f 7661  ..rC...Z.sort_va
-000055c0: 6c75 6573 da04 6865 6164 7230 0000 0072  lues..headr0...r
-000055d0: 4500 0000 da06 7265 6e61 6d65 722f 0000  E.....renamer/..
-000055e0: 00da 0676 616c 7565 7372 3d00 0000 2911  ...valuesr=...).
-000055f0: 72d6 0000 00da 0e63 6872 6f6d 655f 6f70  r......chrome_op
-00005600: 7469 6f6e 73da 0664 7269 7665 7272 b200  tions..driverr..
-00005610: 0000 5a07 636f 6f6b 6965 73da 0673 656c  ..Z.cookies..sel
-00005620: 6563 74da 0361 6c6c 729d 0000 00da 0a74  ect..allr......t
-00005630: 6162 6c65 5f68 746d 6cda 0661 7469 766f  able_html..ativo
-00005640: 7372 c300 0000 7298 0000 005a 0961 7469  sr....r....Z.ati
-00005650: 766f 735f 6466 72cd 0000 0072 8400 0000  vos_dfr....r....
-00005660: 5a11 7265 746f 726e 6f5f 706f 725f 6174  Z.retorno_por_at
-00005670: 6976 6f5a 0c4c 6973 7461 5265 746f 726e  ivoZ.ListaRetorn
-00005680: 6f72 1e00 0000 72da 0000 0072 1f00 0000  or....r....r....
-00005690: da11 6265 7374 5f61 7373 6574 735f 7661  ..best_assets_va
-000056a0: 6c75 657b 0300 0073 4a00 0000 000e 0801  lue{...sJ.......
-000056b0: 0601 0a01 0c02 0401 0a01 0a01 1201 1601  ................
-000056c0: 1201 1202 0e01 0a01 1401 0801 0c01 0e02  ................
-000056d0: 1603 1a03 0c03 1001 1603 1003 1403 1403  ................
-000056e0: 1803 1001 0802 1202 0c01 0e01 3203 1801  ............2...
-000056f0: 0801 0802 0803 72f2 0000 007a 162f 6f70  ......r....z./op
-00005700: 7469 6f6e 732f 7b73 796d 626f 6c7d 2f69  tions/{symbol}/i
-00005710: 6e66 6f54 2904 7221 0000 00da 0463 616c  nfoT).r!.....cal
-00005720: 6cda 0370 7574 7222 0000 0063 0300 0000  l..putr"...c....
-00005730: 0000 0000 0000 0000 0c00 0000 0500 0000  ................
-00005740: 4300 0000 737e 0100 007c 00a0 0064 01a1  C...s~...|...d..
-00005750: 0172 187c 00a0 0164 0164 02a1 027d 006e  .r.|...d.d...}.n
-00005760: 0874 0264 0383 0101 0074 03a0 04a1 0001  .t.d.....t......
-00005770: 0074 0583 007d 037c 03a0 0664 04a1 0101  .t...}.|...d....
-00005780: 0074 076a 087c 0364 058d 017d 0464 067c  .t.j.|.d...}.d.|
-00005790: 009b 009d 027d 057c 04a0 097c 05a1 0101  .....}.|...|....
-000057a0: 0074 0aa0 0b64 07a1 0101 007c 04a0 0c74  .t...d.....|...t
-000057b0: 0d6a 0e64 08a1 027d 067c 06a0 0f64 09a1  .j.d...}.|...d..
-000057c0: 017d 0774 106a 1174 127c 0783 0164 0a64  .}.t.j.t.|...d.d
-000057d0: 0b64 0c8d 037d 087c 0864 0d19 007d 087c  .d...}.|.d...}.|
-000057e0: 0867 0064 0ea2 0119 007d 087c 0164 0f6b  .g.d.....}.|.d.k
-000057f0: 0272 c07c 086a 137c 0864 1019 0064 116b  .r.|.j.|.d...d.k
-00005800: 0219 007d 097c 0953 007c 0264 0f6b 0272  ...}.|.S.|.d.k.r
-00005810: e27c 086a 137c 0864 1019 0064 126b 0219  .|.j.|.d...d.k..
-00005820: 007d 0a64 137d 0b7c 0a53 007c 04a0 097c  .}.d.}.|.S.|...|
-00005830: 05a1 0101 0074 0aa0 0b64 07a1 0101 007c  .....t...d.....|
-00005840: 04a0 0c74 0d6a 0e64 08a1 027d 067c 06a0  ...t.j.d...}.|..
-00005850: 0f64 09a1 017d 0774 106a 1174 127c 0783  .d...}.t.j.t.|..
-00005860: 0164 0a64 0b64 0c8d 037d 087c 0864 0d19  .d.d.d...}.|.d..
-00005870: 007d 087c 0867 0064 0ea2 0119 007d 087c  .}.|.g.d.....}.|
-00005880: 0164 0f6b 0290 0172 567c 086a 137c 0864  .d.k...rV|.j.|.d
-00005890: 1019 0064 116b 0219 007d 097c 0953 007c  ...d.k...}.|.S.|
-000058a0: 0264 0f6b 0290 0172 767c 086a 137c 0864  .d.k...rv|.j.|.d
-000058b0: 1019 0064 126b 0219 007d 0a7c 0a53 007c  ...d.k...}.|.S.|
-000058c0: 0853 0064 1453 0029 1575 c801 0000 0a20  .S.d.S.).u..... 
-000058d0: 2020 2023 2320 5573 6162 696c 6964 6164     ## Usabilidad
-000058e0: 650a 0a20 2020 202d 2046 756e c3a7 c3a3  e..    - Fun....
-000058f0: 6f20 7175 6520 6170 7265 7365 6e74 6120  o que apresenta 
-00005900: 6173 2070 7269 6e63 6970 6169 7320 696e  as principais in
-00005910: 666f 726d 61c3 a7c3 b565 7320 6461 7320  forma....es das 
-00005920: 6f70 c3a7 c3b5 6573 2064 6f20 6174 6976  op....es do ativ
-00005930: 6f20 7365 6c65 6369 6f6e 6164 6f2c 2069  o selecionado, i
-00005940: 6e66 6f72 6d61 c3a7 c3b5 6573 2063 6f6d  nforma....es com
-00005950: 6f3a 2053 7472 696b 652c 2056 6172 2c20  o: Strike, Var, 
-00005960: 4772 6567 6173 2c20 6465 6e74 7265 206f  Gregas, dentre o
-00005970: 7574 7261 732e 0a0a 2020 2020 2323 2050  utras...    ## P
-00005980: 6172 c3a2 6d65 7472 6f73 0a0a 2020 2020  ar..metros..    
-00005990: 2d20 7379 6d62 6f6c 202d 3e20 4e6f 6d65  - symbol -> Nome
-000059a0: 2064 6f20 6174 6976 6f20 7061 7261 2062   do ativo para b
-000059b0: 7573 6361 7220 6173 206f 70c3 a7c3 b565  uscar as op....e
-000059c0: 7320 7265 6665 7265 6e74 6573 2061 2065  s referentes a e
-000059d0: 6c65 2e0a 2020 2020 2d20 6361 6c6c 202d  le..    - call -
-000059e0: 3e20 5265 6365 6265 2054 7275 6520 6f75  > Recebe True ou
-000059f0: 2046 616c 7365 2c20 7365 2054 7275 6520   False, se True 
-00005a00: 666f 7220 7365 6c65 6369 6f6e 6164 6f20  for selecionado 
-00005a10: 6120 6675 6ec3 a7c3 a36f 2069 7261 2066  a fun....o ira f
-00005a20: 696c 7472 6172 2073 6f20 6173 2043 414c  iltrar so as CAL
-00005a30: 4c2e 0a20 2020 202d 2070 7574 202d 3e20  L..    - put -> 
-00005a40: 5265 6365 6265 2054 7275 6520 6f75 2046  Recebe True ou F
-00005a50: 616c 7365 2c20 7365 2054 7275 6520 666f  alse, se True fo
-00005a60: 7220 7365 6c65 6369 6f6e 6164 6f20 6120  r selecionado a 
-00005a70: 6675 6ec3 a7c3 a36f 2069 7261 2066 696c  fun....o ira fil
-00005a80: 7472 6172 2073 6f20 6173 2050 5554 2e0a  trar so as PUT..
-00005a90: 0a0a 2020 2020 72a0 0000 0072 1700 0000  ..    r....r....
-00005aa0: 7534 0000 0050 726f 6375 7261 6e64 6f20  u4...Procurando 
-00005ab0: 6461 646f 7320 6465 206f 70c3 a7c3 b565  dados de op....e
-00005ac0: 7320 646f 2061 7469 766f 2073 656c 6563  s do ativo selec
-00005ad0: 696f 6e61 646f 2e2e 2e72 cf00 0000 72d0  ionado...r....r.
-00005ae0: 0000 007a 2568 7474 7073 3a2f 2f6f 7063  ...z%https://opc
-00005af0: 6f65 732e 6e65 742e 6272 2f6f 7063 6f65  oes.net.br/opcoe
-00005b00: 732f 626f 7665 7370 612f 6700 0000 0000  s/bovespa/g.....
-00005b10: 00f8 3f7a 0c23 7462 6c4c 6973 7461 4f70  ..?z.#tblListaOp
-00005b20: 6372 d200 0000 72be 0000 0072 1900 0000  cr....r....r....
-00005b30: 72bf 0000 0072 0100 0000 290d 722a 0000  r....r....).r*..
-00005b40: 00da 0454 6970 6f5a 0653 7472 696b 657a  ...TipoZ.Strikez
-00005b50: 0741 2f49 2f4f 544d 7a13 4469 7374 2e20  .A/I/OTMz.Dist. 
-00005b60: 2825 2920 646f 2053 7472 696b 6575 0700  (%) do Strikeu..
-00005b70: 0000 c39a 6c74 696d 6f7a 0856 6172 2e20  ....ltimoz.Var. 
-00005b80: 2825 2975 0d00 0000 4ec3 ba6d 2e20 6465  (%)u....N..m. de
-00005b90: 204e 6567 2e7a 0f56 6f6c 2e20 4669 6e61   Neg.z.Vol. Fina
-00005ba0: 6e63 6569 726f da05 4465 6c74 61da 0547  nceiro..Delta..G
-00005bb0: 616d 6d61 7a09 5468 6574 6120 2824 295a  ammaz.Theta ($)Z
-00005bc0: 0456 6567 6154 72f5 0000 00da 0443 414c  .VegaTr......CAL
-00005bd0: 4cda 0350 5554 7215 0000 004e 2914 da08  L..PUTr....N)...
-00005be0: 656e 6473 7769 7468 721a 0000 0072 2e00  endswithr....r..
-00005bf0: 0000 72dd 0000 0072 de00 0000 7207 0000  ..r....r....r...
-00005c00: 0072 df00 0000 7205 0000 0072 e000 0000  .r....r....r....
-00005c10: 72ac 0000 0072 e100 0000 72e2 0000 0072  r....r....r....r
-00005c20: e300 0000 7208 0000 0072 e700 0000 72e8  ....r....r....r.
-00005c30: 0000 0072 4200 0000 72af 0000 0072 8000  ...rB...r....r..
-00005c40: 0000 72b1 0000 0029 0c72 2100 0000 72f3  ..r....).r!...r.
-00005c50: 0000 0072 f400 0000 72ec 0000 0072 ed00  ...r....r....r..
-00005c60: 0000 72b2 0000 0072 9d00 0000 72f0 0000  ..r....r....r...
-00005c70: 005a 0564 664f 5043 5a06 6466 4361 6c6c  .Z.dfOPCZ.dfCall
-00005c80: 5a05 6466 5075 745a 046c 616c 6172 1e00  Z.dfPutZ.lalar..
-00005c90: 0000 721e 0000 0072 1f00 0000 da07 6765  ..r....r......ge
-00005ca0: 745f 6f70 63d1 0300 0073 4800 0000 0012  t_opc....sH.....
-00005cb0: 0a01 0e02 0802 0801 0601 0a01 0c02 0a01  ................
-00005cc0: 0a01 0a01 0e01 0a01 1401 0801 0c01 0801  ................
-00005cd0: 1201 0401 0801 1201 0401 0402 0a01 0a02  ................
-00005ce0: 0e01 0a01 1401 0804 0c01 0a01 1201 0401  ................
-00005cf0: 0a01 1201 0402 72fb 0000 007a 152f 6f70  ......r....z./op
-00005d00: 7469 6f6e 732f 626c 6163 6b53 6368 6f6c  tions/blackSchol
-00005d10: 6573 2902 72f3 0000 0072 f400 0000 6305  es).r....r....c.
-00005d20: 0000 0000 0000 0000 0000 000c 0000 0006  ................
-00005d30: 0000 0043 0000 0073 e800 0000 7400 7c01  ...C...s....t.|.
-00005d40: 7401 7402 8303 7d05 7c05 6401 1400 7d06  t.t...}.|.d...}.
-00005d50: 6402 7d07 7403 a004 7c02 7c03 1b00 a101  d.}.t...|.|.....
-00005d60: 7c07 7c06 6403 1300 6403 1b00 7c04 1400  |.|.d...d...|...
-00005d70: 1700 7c06 7403 a005 7c04 a101 1400 1400  ..|.t...|.......
-00005d80: 1700 7d08 7c06 7403 a005 7c04 a101 1400  ..}.|.t...|.....
-00005d90: 0400 7d09 7d08 7c00 6404 6b02 729a 7406  ..}.}.|.d.k.r.t.
-00005da0: 6405 8301 0100 7c02 7407 a008 7c08 a101  d.....|.t...|...
-00005db0: 1400 7c03 7403 a009 7c07 0b00 7c04 1400  ..|.t...|...|...
-00005dc0: a101 1400 7407 a008 7c09 a101 1400 1800  ....t...|.......
-00005dd0: 7d0a 7c0a 5300 7c00 6406 6b02 72dc 7406  }.|.S.|.d.k.r.t.
-00005de0: 6407 8301 0100 7c03 7403 a009 7c07 0b00  d.....|.t...|...
-00005df0: 7c04 1400 a101 1400 7407 a008 7c09 a101  |.......t...|...
-00005e00: 1400 7c02 7407 a008 7c08 0b00 a101 1400  ..|.t...|.......
-00005e10: 1800 7d0b 7c0b 5300 7406 6408 8301 0100  ..}.|.S.t.d.....
-00005e20: 6409 5300 290a 754a 0300 000a 2020 2020  d.S.).uJ....    
-00005e30: 2323 2055 7361 6269 6c69 6461 6465 0a0a  ## Usabilidade..
-00005e40: 2020 2020 2d20 4675 6ec3 a7c3 a36f 2071      - Fun....o q
-00005e50: 7565 2073 696d 756c 6120 6f20 6361 6375  ue simula o cacu
-00005e60: 6c6f 2064 6f20 626c 6163 6b2d 7363 686f  lo do black-scho
-00005e70: 6c65 732c 206d 6f64 656c 6f20 6e6f 2071  les, modelo no q
-00005e80: 7561 6c20 c3a9 2075 7469 6c69 7a61 646f  ual .. utilizado
-00005e90: 2070 6172 6120 7072 6563 6966 6963 6172   para precificar
-00005ea0: 206f 70c3 a7c3 b565 7320 6e6f 206d 6572   op....es no mer
-00005eb0: 6361 646f 2064 6520 6465 7269 7661 7469  cado de derivati
-00005ec0: 766f 732e 0a20 2020 202d 2050 6f72 2073  vos..    - Por s
-00005ed0: 6520 7472 6174 6172 2064 6520 756d 6120  e tratar de uma 
-00005ee0: 6675 6ec3 a7c3 a36f 2065 6d20 6465 7365  fun....o em dese
-00005ef0: 6e76 6f6c 7669 6d65 6e74 6f20 6ec3 a36f  nvolvimento n..o
-00005f00: 206c 6576 6172 206f 2072 6573 756c 7461   levar o resulta
-00005f10: 646f 2063 6f6d 6f20 7665 7264 6164 6520  do como verdade 
-00005f20: 6162 736f 6c75 7461 2c20 6d61 7320 756d  absoluta, mas um
-00005f30: 2076 616c 6f72 2061 2073 6520 6261 7365   valor a se base
-00005f40: 6172 2e0a 0a20 2020 2023 2320 5061 72c3  ar...    ## Par.
-00005f50: a26d 6574 726f 730a 0a20 2020 202d 2043  .metros..    - C
-00005f60: 616c 6c5f 6f72 5f50 7574 202d 3e20 5265  all_or_Put -> Re
-00005f70: 6365 6265 206f 7320 7661 6c6f 7265 7320  cebe os valores 
-00005f80: 2263 616c 6c22 2065 2022 7075 7422 2c20  "call" e "put", 
-00005f90: 706f 7220 7365 7265 6d20 6361 6c63 756c  por serem calcul
-00005fa0: 6f73 2064 6966 6572 656e 7465 7320 7061  os diferentes pa
-00005fb0: 7261 6461 2063 6164 6120 7469 706f 2c20  rada cada tipo, 
-00005fc0: c3a9 206e 6563 6573 7361 7269 6f20 6120  .. necessario a 
-00005fd0: 7365 6c65 c3a7 c3a3 6f0a 2020 2020 2d20  sele....o.    - 
-00005fe0: 6174 6976 6f20 2d3e 2049 6e73 6572 6972  ativo -> Inserir
-00005ff0: 206f 2061 7469 766f 2063 6f72 7265 7370   o ativo corresp
-00006000: 6f6e 6465 6e74 6520 6461 2066 756e c3a7  ondente da fun..
-00006010: c3a3 6f20 2845 7865 6d70 6c6f 3a20 2750  ..o (Exemplo: 'P
-00006020: 4554 5234 2e53 4127 290a 2020 2020 2d20  ETR4.SA').    - 
-00006030: 7072 6563 6f20 2d3e 2069 6e73 6572 6972  preco -> inserir
-00006040: 206f 2070 7265 c3a7 6f20 646f 2061 7469   o pre..o do ati
-00006050: 766f 2073 656c 6563 696f 6e61 646f 0a20  vo selecionado. 
-00006060: 2020 202d 2073 7472 696b 6520 2d3e 2049     - strike -> I
-00006070: 6e73 6572 6972 206f 2073 7472 696b 6520  nserir o strike 
-00006080: 6461 206f 70c3 a7c3 a36f 0a20 2020 202d  da op....o.    -
-00006090: 2064 6961 7355 7465 6973 202d 3e20 4164   diasUteis -> Ad
-000060a0: 6963 696f 6e61 7220 6120 7175 616e 7469  icionar a quanti
-000060b0: 6461 6465 2064 6520 6469 6173 20c3 ba74  dade de dias ..t
-000060c0: 6569 7320 6174 6520 6f20 7665 6e63 696d  eis ate o vencim
-000060d0: 656e 746f 2064 6120 6f70 c3a7 c3a3 6f2e  ento da op....o.
-000060e0: 0a0a 2020 2020 2323 2045 7865 6d70 6c6f  ..    ## Exemplo
-000060f0: 0a0a 2020 2020 6060 600a 2020 2020 3e3e  ..    ```.    >>
-00006100: 3e20 6262 2e62 6c61 636b 5f73 6368 6f6c  > bb.black_schol
-00006110: 6573 2843 616c 6c5f 6f72 5f50 7574 3d20  es(Call_or_Put= 
-00006120: 2763 616c 6c27 2c20 6174 6976 6f3d 2027  'call', ativo= '
-00006130: 5045 5452 342e 5341 272c 2070 7265 636f  PETR4.SA', preco
-00006140: 3d20 3236 2e32 352c 2073 7472 696b 653d  = 26.25, strike=
-00006150: 2032 362e 3235 2c20 6469 6173 5574 6569   26.25, diasUtei
-00006160: 733d 2032 3220 290a 2020 2020 6060 600a  s= 22 ).    ```.
-00006170: 0a20 2020 2069 10f8 0000 67c1 a8a4 4e40  .    i....g...N@
-00006180: d315 4072 7200 0000 72f3 0000 007a 1053  ..@rr...r....z.S
-00006190: 656c 6563 696f 6e61 646f 2043 616c 6c72  elecionado Callr
-000061a0: f400 0000 7a0f 5365 6c65 6369 6f6e 6164  ....z.Selecionad
-000061b0: 6f20 5075 7475 3000 0000 4173 206f 70c3  o Putu0...As op.
-000061c0: a7c3 b565 7320 7661 6c69 6461 7320 7361  ...es validas sa
-000061d0: 6f20 736f 6d65 6e74 6520 6173 2064 6520  o somente as de 
-000061e0: 4341 4c4c 2065 2050 5554 4e29 0a72 6a00  CALL e PUTN).rj.
-000061f0: 0000 da06 7365 7665 6e44 72cc 0000 0072  ....sevenDr....r
-00006200: 6500 0000 7266 0000 0072 6800 0000 722e  e...rf...rh...r.
-00006210: 0000 0072 0200 0000 5a03 6364 66da 0365  ...r....Z.cdf..e
-00006220: 7870 290c 5a0b 4361 6c6c 5f6f 725f 5075  xp).Z.Call_or_Pu
-00006230: 7472 cd00 0000 da05 7072 6563 6fda 0673  tr......preco..s
-00006240: 7472 696b 655a 0964 6961 7355 7465 6973  trikeZ.diasUteis
-00006250: 5a0d 766f 6c61 7469 6c69 6461 6465 445a  Z.volatilidadeDZ
-00006260: 0c76 6f6c 6174 696c 6964 6164 655a 0674  .volatilidadeZ.t
-00006270: 6178 614c 52da 0264 31da 0264 32da 0143  axaLR..d1..d2..C
-00006280: da01 5072 1e00 0000 721e 0000 0072 1f00  ..Pr....r....r..
-00006290: 0000 da0d 626c 6163 6b5f 7363 686f 6c65  ....black_schole
-000062a0: 7316 0400 0073 1c00 0000 0019 0c01 0801  s....s..........
-000062b0: 0402 3001 1202 0801 0801 2c01 0401 0801  ..0.......,.....
-000062c0: 0801 2e01 0402 7204 0100 00e7 713d 0ad7  ......r.....q=..
-000062d0: a370 cd3f 2902 72f1 0000 00da 0c69 6e76  .p.?).r......inv
-000062e0: 6573 7469 6d65 6e74 6f63 0300 0000 0000  estimentoc......
-000062f0: 0000 0000 0000 0a00 0000 0700 0000 4300  ..............C.
-00006300: 0000 731e 0100 0074 006a 0167 0064 01a2  ..s....t.j.g.d..
-00006310: 0164 028d 017d 0374 027c 0074 0383 0272  .d...}.t.|.t...r
-00006320: 9674 04a0 057c 00a1 017d 047c 046a 0664  .t...|...}.|.j.d
-00006330: 0364 048d 0164 0519 0064 0619 007d 057c  .d...d...d...}.|
-00006340: 046a 07a0 08a1 007d 067c 057c 0617 007c  .j.....}.|.|...|
-00006350: 051b 0064 0718 007c 0114 007d 0774 09a0  ...d...|...}.t..
-00006360: 0a7c 077c 011b 0064 0717 00a1 0174 09a0  .|.|...d.....t..
-00006370: 0a64 0764 087c 0214 0017 00a1 011b 0064  .d.d.|.........d
-00006380: 091b 007d 087c 036a 0b7c 007c 077c 0864  ...}.|.j.|.|.|.d
-00006390: 019c 0364 0a64 0b8d 027d 036e 847c 0044  ...d.d...}.n.|.D
-000063a0: 005d 7e7d 0974 04a0 057c 09a1 017d 047c  .]~}.t...|...}.|
-000063b0: 046a 0664 0364 048d 0164 0519 0064 0619  .j.d.d...d...d..
-000063c0: 007d 057c 046a 07a0 08a1 007d 067c 057c  .}.|.j.....}.|.|
-000063d0: 0617 007c 051b 0064 0718 007c 0114 007d  ...|...d...|...}
-000063e0: 0774 09a0 0a7c 077c 011b 0064 0717 00a1  .t...|.|...d....
-000063f0: 0174 09a0 0a64 0764 087c 0214 0017 00a1  .t...d.d.|......
-00006400: 011b 0064 091b 007d 087c 036a 0b7c 097c  ...d...}.|.j.|.|
-00006410: 077c 0864 019c 0364 0a64 0b8d 027d 0371  .|.d...d.d...}.q
-00006420: 9a7c 0353 0029 0c4e 2903 7279 0000 007a  .|.S.).N).ry...z
-00006430: 1652 6574 6f72 6e6f 2063 6f6d 2044 6976  .Retorno com Div
-00006440: 6964 656e 646f 737a 1a54 656d 706f 2070  idendosz.Tempo p
-00006450: 6172 6120 4174 696e 6769 7220 5265 746f  ara Atingir Reto
-00006460: 726e 6f72 c800 0000 7239 0000 0072 3b00  rnor....r9...r;.
-00006470: 0000 7247 0000 0072 0100 0000 7215 0000  ..rG...r....r...
-00006480: 0072 c700 0000 e90c 0000 0054 2901 5a0c  .r.........T).Z.
-00006490: 6967 6e6f 7265 5f69 6e64 6578 290c 7242  ignore_index).rB
-000064a0: 0000 0072 4300 0000 727f 0000 0072 8000  ...rC...r....r..
-000064b0: 0000 7229 0000 0072 2a00 0000 723f 0000  ..r)...r*...r?..
-000064c0: 0072 2800 0000 7230 0000 0072 6500 0000  .r(...r0...re...
-000064d0: 7266 0000 0072 9600 0000 290a 72f1 0000  rf...r....).r...
-000064e0: 0072 0601 0000 5a0d 7461 7861 5f64 6573  .r....Z.taxa_des
-000064f0: 636f 6e74 6f72 8400 0000 7278 0000 0072  contor....rx...r
-00006500: fe00 0000 5a0a 6469 7669 6465 6e64 6f73  ....Z.dividendos
-00006510: 72c4 0000 005a 0574 656d 706f 72cd 0000  r....Z.tempor...
-00006520: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00006530: da13 7265 746f 726e 6f73 5f64 6976 6964  ..retornos_divid
-00006540: 656e 646f 734e 0400 0073 2000 0000 0001  endosN...s .....
-00006550: 1002 0a01 0a01 1401 0a01 1401 2801 1802  ............(...
-00006560: 0801 0a01 1401 0a01 1401 2801 1802 7208  ..........(...r.
-00006570: 0100 0029 0172 3900 0000 2901 7201 0000  ...).r9...).r...
-00006580: 0029 0172 0501 0000 2953 5a08 7966 696e  .).r....)SZ.yfin
-00006590: 616e 6365 7229 0000 005a 0b73 6369 7079  ancer)...Z.scipy
-000065a0: 2e73 7461 7473 7202 0000 005a 0e73 6369  .statsr....Z.sci
-000065b0: 7079 2e6f 7074 696d 697a 6572 0300 0000  py.optimizer....
-000065c0: 5a14 736b 6c65 6172 6e2e 6c69 6e65 6172  Z.sklearn.linear
-000065d0: 5f6d 6f64 656c 7204 0000 005a 0873 656c  _modelr....Z.sel
-000065e0: 656e 6975 6d72 0500 0000 5a1e 7365 6c65  eniumr....Z.sele
-000065f0: 6e69 756d 2e77 6562 6472 6976 6572 2e63  nium.webdriver.c
-00006600: 6f6d 6d6f 6e2e 6b65 7973 7206 0000 005a  ommon.keysr....Z
-00006610: 2173 656c 656e 6975 6d2e 7765 6264 7269  !selenium.webdri
-00006620: 7665 722e 6368 726f 6d65 2e6f 7074 696f  ver.chrome.optio
-00006630: 6e73 7207 0000 005a 1c73 656c 656e 6975  nsr....Z.seleniu
-00006640: 6d2e 7765 6264 7269 7665 722e 636f 6d6d  m.webdriver.comm
-00006650: 6f6e 2e62 7972 0800 0000 72dd 0000 0072  on.byr....r....r
-00006660: ab00 0000 5a03 6273 3472 0900 0000 72e1  ....Z.bs4r....r.
-00006670: 0000 005a 0766 6173 7461 7069 720a 0000  ...Z.fastapir...
-00006680: 0072 0b00 0000 720c 0000 005a 1166 6173  .r....r....Z.fas
-00006690: 7461 7069 2e72 6573 706f 6e73 6573 720d  tapi.responsesr.
-000066a0: 0000 005a 1366 6173 7461 7069 2e73 7461  ...Z.fastapi.sta
-000066b0: 7469 6366 696c 6573 720e 0000 005a 1266  ticfilesr....Z.f
-000066c0: 6173 7461 7069 2e74 656d 706c 6174 696e  astapi.templatin
-000066d0: 6772 0f00 0000 da04 6a73 6f6e 5a07 7576  gr......jsonZ.uv
-000066e0: 6963 6f72 6eda 0670 616e 6461 7372 4200  icorn..pandasrB.
-000066f0: 0000 da05 6e75 6d70 7972 6500 0000 7210  ....numpyre...r.
-00006700: 0000 0072 1100 0000 da06 7479 7069 6e67  ...r......typing
-00006710: 7212 0000 00da 0877 6172 6e69 6e67 73da  r......warnings.
-00006720: 0e66 696c 7465 7277 6172 6e69 6e67 735a  .filterwarningsZ
-00006730: 0c70 6472 5f6f 7665 7272 6964 65da 0574  .pdr_override..t
-00006740: 6f64 6179 5a0c 6f6e 655f 7965 6172 5f61  odayZ.one_year_a
-00006750: 676f 5a0c 6f6e 655f 6461 7973 5f61 676f  goZ.one_days_ago
-00006760: 5a0e 7365 7665 6e5f 6461 7973 5f61 676f  Z.seven_days_ago
-00006770: da08 7374 7266 7469 6d65 72cb 0000 005a  ..strftimer....Z
-00006780: 046f 6e65 4472 fc00 0000 72cc 0000 00da  .oneDr....r.....
-00006790: 0361 7070 7220 0000 0072 ac00 0000 7280  .appr ...r....r.
-000067a0: 0000 0072 2d00 0000 7234 0000 00da 085f  ...r-...r4....._
-000067b0: 5f6e 616d 655f 5fda 0372 756e 72b3 0000  _name__..runr...
-000067c0: 0072 4300 0000 7246 0000 005a 0f72 6573  .rC...rF...Z.res
-000067d0: 706f 6e73 6548 6973 746f 7279 724c 0000  ponseHistoryrL..
-000067e0: 0072 5d00 0000 726a 0000 0072 6e00 0000  .r]...rj...rn...
-000067f0: 721c 0000 00da 0369 6e74 7276 0000 0072  r......intrv...r
-00006800: 3d00 0000 7286 0000 0072 9a00 0000 72b7  =...r....r....r.
-00006810: 0000 0072 ba00 0000 72bd 0000 0072 ce00  ...r....r....r..
-00006820: 0000 72f2 0000 0072 fb00 0000 7204 0100  ..r....r....r...
-00006830: 0072 0801 0000 721e 0000 0072 1e00 0000  .r....r....r....
-00006840: 721e 0000 0072 1f00 0000 da08 3c6d 6f64  r....r......<mod
-00006850: 756c 653e 0200 0000 73e8 0000 0008 010c  ule>....s.......
-00006860: 010c 010c 030c 010c 010c 010c 0108 0108  ................
-00006870: 010c 0108 0314 010c 010c 010c 0108 0108  ................
-00006880: 0308 0108 0110 010c 0208 010a 0208 0208  ................
-00006890: 020e 010e 010e 030a 010a 010a 020a 0206  ................
-000068a0: 0c08 090c 0112 260a 0112 010a 050c 0118  ......&.........
-000068b0: 260a 0112 010a 050c 0112 200a 0112 010a  &......... .....
-000068c0: 050c 0112 3a0a 0112 010a 050c 0116 180a  ....:...........
-000068d0: 0112 010a 050c 0112 320a 0112 010a 050c  ........2.......
-000068e0: 0116 230a 0112 010a 050c 0120 620a 0112  ..#........ b...
-000068f0: 010a 0508 0116 3a0a 0112 010a 050c 0114  ......:.........
-00006900: 180a 0112 010a 050c 0116 420a 0112 010a  ..........B.....
-00006910: 050c 011a 400a 0112 010a 050c 0116 7f00  ....@...........
-00006920: 070a 0112 010a 030c 011e 4d0a 0112 010a  ..........M.....
-00006930: 060c 011a 3f0a 0112 010a 030c 0120 2a0a  ....?........ *.
-00006940: 0112 010a 0b                             .....
+000005a0: 8d02 6538 6528 6459 1900 6528 6459 1900  ..e8e(dY..e(dY..
+000005b0: 6522 a03e a100 645a 9c04 645b 645c 8404  e".>..dZ..d[d\..
+000005c0: 8301 5a50 653b 641d 6b02 9005 72b2 6520  ..ZPe;d.k...r.e 
+000005d0: 6a3c 6535 641f 6420 6458 6422 8d04 0100  j<e5d.d dXd"....
+000005e0: 6517 6423 6424 8d01 5a40 6535 6a37 645d  e.d#d$..Z@e5j7d]
+000005f0: 6401 6419 8d02 6528 645e 1900 6538 6545  d.d...e(d^..e8eE
+00000600: 6545 6546 6605 6538 644f 9c01 645f 6460  eEeFf.e8dO..d_d`
+00000610: 8405 8301 5a51 653b 641d 6b02 9006 7204  ....ZQe;d.k...r.
+00000620: 6520 6a3c 6535 641f 6420 645d 6422 8d04  e j<e5d.d d]d"..
+00000630: 0100 6517 6423 6424 8d01 5a40 6467 6528  ..e.d#d$..Z@dge(
+00000640: 6538 6548 6602 1900 6528 6546 6545 6602  e8eHf...e(eFeEf.
+00000650: 1900 6462 9c02 6463 6464 8405 5a52 6401  ..db..dcdd..ZRd.
+00000660: 5300 2968 e900 0000 004e 2901 da04 6e6f  S.)h.....N)...no
+00000670: 726d 2901 da08 6d69 6e69 6d69 7a65 2901  rm)...minimize).
+00000680: da10 4c69 6e65 6172 5265 6772 6573 7369  ..LinearRegressi
+00000690: 6f6e 2901 da09 7765 6264 7269 7665 7229  on)...webdriver)
+000006a0: 01da 044b 6579 7329 01da 074f 7074 696f  ...Keys)...Optio
+000006b0: 6e73 2901 da02 4279 2901 da0d 4265 6175  ns)...By)...Beau
+000006c0: 7469 6675 6c53 6f75 7029 03da 0746 6173  tifulSoup)...Fas
+000006d0: 7441 5049 da08 5265 7370 6f6e 7365 da07  tAPI..Response..
+000006e0: 5265 7175 6573 7429 01da 0c48 544d 4c52  Request)...HTMLR
+000006f0: 6573 706f 6e73 6529 01da 0b53 7461 7469  esponse)...Stati
+00000700: 6346 696c 6573 2901 da0f 4a69 6e6a 6132  cFiles)...Jinja2
+00000710: 5465 6d70 6c61 7465 7329 02da 0864 6174  Templates)...dat
+00000720: 6574 696d 65da 0974 696d 6564 656c 7461  etime..timedelta
+00000730: 2901 da05 556e 696f 6eda 0669 676e 6f72  )...Union..ignor
+00000740: 6569 6d01 0000 2901 da04 6461 7973 e901  eim...)...days..
+00000750: 0000 00e9 0700 0000 7a08 2559 2d25 6d2d  ........z.%Y-%m-
+00000760: 2564 6302 0000 0000 0000 0000 0000 0002  %dc.............
+00000770: 0000 0005 0000 0043 0000 0073 5e00 0000  .......C...s^...
+00000780: 7c00 7c01 1900 6a00 6401 6402 6403 6404  |.|...j.d.d.d.d.
+00000790: 8d03 7c00 7c01 3c00 7c00 7c01 1900 6a00  ..|.|.<.|.|...j.
+000007a0: 6405 6402 6403 6404 8d03 7c00 7c01 3c00  d.d.d.d...|.|.<.
+000007b0: 7c00 7c01 1900 6a00 6406 6407 6403 6404  |.|...j.d.d.d.d.
+000007c0: 8d03 7c00 7c01 3c00 7c00 7c01 1900 a001  ..|.|.<.|.|.....
+000007d0: 7402 a101 7c00 7c01 3c00 7c00 5300 2908  t...|.|.<.|.S.).
+000007e0: 4e7a 035b 2e5d da00 5429 01da 0572 6567  Nz.[.]..T)...reg
+000007f0: 6578 7a03 5b25 5d7a 035b 2c5d da01 2e29  exz.[%]z.[,]...)
+00000800: 03da 0772 6570 6c61 6365 da06 6173 7479  ...replace..asty
+00000810: 7065 da05 666c 6f61 7429 02da 0264 665a  pe..float)...dfZ
+00000820: 0a6e 6f6d 6543 6f6c 756e 61a9 0072 1e00  .nomeColuna..r..
+00000830: 0000 fa40 713a 5c52 6973 636f 5c4e 6f76  ...@q:\Risco\Nov
+00000840: 6f20 5269 7363 6f5c 7079 7468 6f6e 7269  o Risco\pythonri
+00000850: 7363 6f5c 4242 4669 6e61 6e63 655c 4242  sco\BBFinance\BB
+00000860: 4669 6e61 6e63 655c 4242 4669 6e61 6e63  Finance\BBFinanc
+00000870: 652e 7079 da14 666f 726d 6174 6156 616c  e.py..formataVal
+00000880: 6f72 6573 4e75 6d65 726f 3d00 0000 730a  oresNumero=...s.
+00000890: 0000 0000 0118 0118 0118 0112 0272 2000  .............r .
+000008a0: 0000 7a15 2f73 746f 636b 732f 7b73 796d  ..z./stocks/{sym
+000008b0: 626f 6c7d 2f69 6e66 6f29 015a 0e72 6573  bol}/info).Z.res
+000008c0: 706f 6e73 655f 6d6f 6465 6c29 02da 0673  ponse_model)...s
+000008d0: 796d 626f 6cda 0672 6574 7572 6e63 0100  ymbol..returnc..
+000008e0: 0000 0000 0000 0000 0000 0800 0000 0500  ................
+000008f0: 0000 4300 0000 7368 0000 0074 00a0 017c  ..C...sh...t...|
+00000900: 00a1 017d 017c 016a 027d 0274 037c 0283  ...}.|.j.}.t.|..
+00000910: 017d 037c 0374 046b 0272 226e 0874 0564  .}.|.t.k.r"n.t.d
+00000920: 0183 0101 007c 016a 0264 0219 007d 047c  .....|.j.d...}.|
+00000930: 016a 0264 0319 007d 057c 016a 067d 067c  .j.d...}.|.j.}.|
+00000940: 066a 0764 0464 0585 0219 00a0 08a1 007d  .j.d.d.........}
+00000950: 067c 007c 047c 057c 0664 069c 047d 077c  .|.|.|.|.d...}.|
+00000960: 0753 0029 0775 bf00 0000 0a20 2020 2023  .S.).u.....    #
+00000970: 2320 5573 6162 696c 6964 6164 6520 0a20  # Usabilidade . 
+00000980: 2020 202d 2042 7573 6361 2061 7320 7072     - Busca as pr
+00000990: 696e 6369 7061 6973 2069 6e66 6f72 6d61  incipais informa
+000009a0: c3a7 6f65 7320 736f 6272 6520 6f20 6174  ..oes sobre o at
+000009b0: 6976 6f20 7365 6c65 6369 6f6e 6164 6f20  ivo selecionado 
+000009c0: 636f 6d6f 2050 7265 c3a7 6f20 6520 4469  como Pre..o e Di
+000009d0: 7669 6465 6e64 6f73 200a 0a20 2020 200a  videndos ..    .
+000009e0: 2020 2020 2323 2050 6172 c3a2 6d65 7472      ## Par..metr
+000009f0: 6f73 0a20 2020 202d 2073 796d 626f 6c20  os.    - symbol 
+00000a00: 2d3e 204e 6f6d 6520 646f 2041 7469 766f  -> Nome do Ativo
+00000a10: 2070 6172 6120 6120 6275 7363 6120 0a0a   para a busca ..
+00000a20: 2020 2020 0a20 2020 20fa 0f54 6963 6b65      .    ..Ticke
+00000a30: 7220 496e 7661 6c69 646f da12 7265 6775  r Invalido..regu
+00000a40: 6c61 724d 6172 6b65 7450 7269 6365 5a08  larMarketPriceZ.
+00000a50: 6c6f 6e67 4e61 6d65 e9ff ffff ff4e 2904  longName.....N).
+00000a60: 7221 0000 00da 0d63 7572 7265 6e74 5f70  r!.....current_p
+00000a70: 7269 6365 da0c 636f 6d70 616e 795f 6e61  rice..company_na
+00000a80: 6d65 da09 6469 7669 6465 6e64 7329 09da  me..dividends)..
+00000a90: 0279 66da 0654 6963 6b65 72da 0469 6e66  .yf..Ticker..inf
+00000aa0: 6fda 0474 7970 65da 0464 6963 74da 0570  o..type..dict..p
+00000ab0: 7269 6e74 7228 0000 00da 0469 6c6f 63da  rintr(.....iloc.
+00000ac0: 0373 756d 2908 7221 0000 00da 0573 746f  .sum).r!.....sto
+00000ad0: 636b 722b 0000 00da 0874 6970 6f49 6e66  ckr+.....tipoInf
+00000ae0: 6f72 2600 0000 7227 0000 005a 0864 6976  or&...r'...Z.div
+00000af0: 6964 656e 64da 096a 736f 6e5f 6461 7461  idend..json_data
+00000b00: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
+00000b10: 0867 6574 5f69 6e66 6f46 0000 0073 2000  .get_infoF...s .
+00000b20: 0000 000c 0a01 0601 0801 0801 0202 0802  ................
+00000b30: 0a03 0a03 0601 1203 0201 0201 0201 02fd  ................
+00000b40: 0607 7234 0000 00da 085f 5f6d 6169 6e5f  ..r4.....__main_
+00000b50: 5f7a 086d 6169 6e3a 6170 707a 0931 3237  _z.main:appz.127
+00000b60: 2e30 2e30 2e31 6940 1f00 007a 1473 746f  .0.0.1i@...z.sto
+00000b70: 636b 732f 7b73 796d 626f 6c7d 2f69 6e66  cks/{symbol}/inf
+00000b80: 6f29 03da 0468 6f73 74da 0470 6f72 74da  o)...host..port.
+00000b90: 0764 6566 6175 6c74 7a10 6170 706c 6963  .defaultz.applic
+00000ba0: 6174 696f 6e2f 6a73 6f6e 2901 5a0a 6d65  ation/json).Z.me
+00000bb0: 6469 615f 7479 7065 7a18 2f73 746f 636b  dia_typez./stock
+00000bc0: 732f 7b73 796d 626f 6c7d 2f68 6973 746f  s/{symbol}/histo
+00000bd0: 7279 da02 3179 2903 7221 0000 00da 0670  ry..1y).r!.....p
+00000be0: 6572 696f 6472 2200 0000 6302 0000 0000  eriodr"...c.....
+00000bf0: 0000 0000 0000 0008 0000 0003 0000 0043  ...............C
+00000c00: 0000 0073 7000 0000 7400 a001 7c00 a101  ...sp...t...|...
+00000c10: 7d02 7c02 6a02 7d03 7403 7c03 8301 7d04  }.|.j.}.t.|...}.
+00000c20: 7c04 7404 6b02 7222 6e08 7405 6401 8301  |.t.k.r"n.t.d...
+00000c30: 0100 7c02 6a06 7c01 6402 8d01 7d05 7c05  ..|.j.|.d...}.|.
+00000c40: 6a07 7248 6403 7405 6404 8301 6901 5300  j.rHd.t.d...i.S.
+00000c50: 7c05 6a08 6405 6406 8d01 7d06 7409 6a0a  |.j.d.d...}.t.j.
+00000c60: a00b 7c06 a101 6a0c 6407 6408 8d01 7d07  ..|...j.d.d...}.
+00000c70: 7c07 5300 6409 5300 290a 75ff 0000 000a  |.S.d.S.).u.....
+00000c80: 2020 2020 2323 2055 7361 6269 6c69 6461      ## Usabilida
+00000c90: 6465 200a 2020 2020 2d20 5573 6164 6120  de .    - Usada 
+00000ca0: 7061 7261 2076 6572 6966 6963 6172 206f  para verificar o
+00000cb0: 2068 6973 74c3 b372 6963 6f20 6461 2061   hist..rico da a
+00000cc0: c3a7 616f 2073 656c 6563 696f 6e61 6461  ..ao selecionada
+00000cd0: 2065 2065 6d20 7175 616c 2070 6572 696f   e em qual perio
+00000ce0: 646f 200a 0a20 2020 200a 2020 2020 2323  do ..    .    ##
+00000cf0: 2050 6172 c3a2 6d65 7472 6f73 0a20 2020   Par..metros.   
+00000d00: 200a 2020 2020 2d20 7379 6d62 6f6c 202d   .    - symbol -
+00000d10: 3e20 4e6f 6d65 2064 6f20 4174 6976 6f20  > Nome do Ativo 
+00000d20: 7061 7261 2061 2062 7573 6361 200a 0a20  para a busca .. 
+00000d30: 2020 202d 2070 6572 696f 6420 2d3e 2044     - period -> D
+00000d40: 6174 6120 656d 2041 4e4f 5320 7061 7261  ata em ANOS para
+00000d50: 2061 2062 7573 6361 2064 6173 2069 6e66   a busca das inf
+00000d60: 6f72 6d61 c3a7 6f65 7320 646f 2041 7469  orma..oes do Ati
+00000d70: 766f 200a 0a20 2020 200a 2020 2020 7223  vo ..    .    r#
+00000d80: 0000 00a9 0172 3a00 0000 da05 6572 726f  .....r:.....erro
+00000d90: 727a 0d4e 6f20 6461 7461 2066 6f75 6e64  rz.No data found
+00000da0: da04 6c69 7374 2901 5a06 6f72 6965 6e74  ..list).Z.orient
+00000db0: 4629 01da 0464 726f 704e 290d 7229 0000  F)...dropN).r)..
+00000dc0: 0072 2a00 0000 722b 0000 0072 2c00 0000  .r*...r+...r,...
+00000dd0: 722d 0000 0072 2e00 0000 da07 6869 7374  r-...r......hist
+00000de0: 6f72 79da 0565 6d70 7479 da07 746f 5f64  ory..empty..to_d
+00000df0: 6963 74da 0270 64da 0944 6174 6146 7261  ict..pd..DataFra
+00000e00: 6d65 da09 6672 6f6d 5f64 6963 74da 0b72  me..from_dict..r
+00000e10: 6573 6574 5f69 6e64 6578 2908 7221 0000  eset_index).r!..
+00000e20: 0072 3a00 0000 7231 0000 0072 2b00 0000  .r:...r1...r+...
+00000e30: 7232 0000 0072 3f00 0000 5a0c 6869 7374  r2...r?...Z.hist
+00000e40: 6f72 795f 6469 6374 5a0a 6869 7374 6f72  ory_dictZ.histor
+00000e50: 795f 6466 721e 0000 0072 1e00 0000 721f  y_dfr....r....r.
+00000e60: 0000 00da 1167 6574 5f73 746f 636b 5f68  .....get_stock_h
+00000e70: 6973 746f 7279 7400 0000 7318 0000 0000  istoryt...s.....
+00000e80: 0e0a 0106 0108 0108 0102 0208 020c 0206  ................
+00000e90: 010c 020c 0114 0272 4600 0000 7a17 7374  .......rF...z.st
+00000ea0: 6f63 6b73 2f7b 7379 6d62 6f6c 7d2f 6869  ocks/{symbol}/hi
+00000eb0: 7374 6f72 797a 152f 7374 6f63 6b2f 7b73  storyz./stock/{s
+00000ec0: 796d 626f 6c7d 2f74 7265 6e64 6301 0000  ymbol}/trendc...
+00000ed0: 0000 0000 0000 0000 0008 0000 0003 0000  ................
+00000ee0: 0043 0000 0073 6800 0000 7400 a001 7c00  .C...sh...t...|.
+00000ef0: a101 7d01 7c01 6a02 7d02 7403 7c02 8301  ..}.|.j.}.t.|...
+00000f00: 7d03 7c03 7404 6b02 7222 6e08 7405 6401  }.|.t.k.r"n.t.d.
+00000f10: 8301 0100 7c01 6a06 6402 6403 8d01 7d04  ....|.j.d.d...}.
+00000f20: 7c04 6404 1900 7d05 7c05 6a07 6405 1900  |.d...}.|.j.d...
+00000f30: 7c05 6a07 6406 1900 6b04 7256 6407 6e02  |.j.d...k.rVd.n.
+00000f40: 6408 7d06 7c00 7c06 6409 9c02 7d07 7c07  d.}.|.|.d...}.|.
+00000f50: 5300 290a 75b9 0000 000a 2020 2020 2323  S.).u.....    ##
+00000f60: 2055 7361 6269 6c69 6461 6465 200a 2020   Usabilidade .  
+00000f70: 2020 2d20 4964 656e 7469 6669 6361 2061    - Identifica a
+00000f80: 2074 656e 6465 6e63 6961 2064 6520 7072   tendencia de pr
+00000f90: 65c3 a76f 2064 6520 756d 6120 61c3 a761  e..o de uma a..a
+00000fa0: 6f2c 2073 6520 6972 6120 7365 7220 6465  o, se ira ser de
+00000fb0: 2041 4c54 4120 6f75 2042 4149 5841 0a20   ALTA ou BAIXA. 
+00000fc0: 2020 200a 2020 2020 2323 2050 6172 c3a2     .    ## Par..
+00000fd0: 6d65 7472 6f73 0a20 2020 200a 2020 2020  metros.    .    
+00000fe0: 2d20 7379 6d62 6f6c 202d 3e20 4e6f 6d65  - symbol -> Nome
+00000ff0: 2064 6f20 4174 6976 6f20 7061 7261 2061   do Ativo para a
+00001000: 2062 7573 6361 200a 0a20 2020 200a 2020   busca ..    .  
+00001010: 2020 7223 0000 005a 0231 6472 3b00 0000    r#...Z.1dr;...
+00001020: da05 436c 6f73 6572 2500 0000 7201 0000  ..Closer%...r...
+00001030: 00da 0275 70da 0464 6f77 6e29 0272 2100  ...up..down).r!.
+00001040: 0000 da05 7472 656e 6429 0872 2900 0000  ....trend).r)...
+00001050: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
+00001060: 2d00 0000 722e 0000 0072 3f00 0000 722f  -...r....r?...r/
+00001070: 0000 0029 0872 2100 0000 7231 0000 0072  ...).r!...r1...r
+00001080: 2b00 0000 7232 0000 0072 3f00 0000 da0c  +...r2...r?.....
+00001090: 636c 6f73 655f 7072 6963 6573 724a 0000  close_pricesrJ..
+000010a0: 0072 3300 0000 721e 0000 0072 1e00 0000  .r3...r....r....
+000010b0: 721f 0000 00da 0f67 6574 5f73 746f 636b  r......get_stock
+000010c0: 5f74 7265 6e64 a200 0000 731a 0000 0000  _trend....s.....
+000010d0: 0d0a 0106 0108 0108 0102 0208 020c 0108  ................
+000010e0: 011c 0202 0102 ff06 0672 4c00 0000 7a15  .........rL...z.
+000010f0: 7374 6f63 6b73 2f7b 7379 6d62 6f6c 7d2f  stocks/{symbol}/
+00001100: 7472 656e 647a 192f 7374 6f63 6b2f 7b73  trendz./stock/{s
+00001110: 796d 626f 6c7d 2f74 6563 686e 6963 616c  ymbol}/technical
+00001120: 6301 0000 0000 0000 0000 0000 0011 0000  c...............
+00001130: 0006 0000 0043 0000 0073 f800 0000 7400  .....C...s....t.
+00001140: a001 7c00 a101 7d01 7c01 6a02 7d02 7403  ..|...}.|.j.}.t.
+00001150: 7c02 8301 7d03 7c03 7404 6b02 7222 6e08  |...}.|.t.k.r"n.
+00001160: 7405 6401 8301 0100 7c01 6a06 6402 6403  t.d.....|.j.d.d.
+00001170: 8d01 7d04 7c04 6404 1900 7d05 7c05 6a07  ..}.|.d...}.|.j.
+00001180: 6405 6406 8d01 a008 a100 6a09 6407 1900  d.d.......j.d...
+00001190: 7d06 7c05 6a07 6408 6406 8d01 a008 a100  }.|.j.d.d.......
+000011a0: 6a09 6407 1900 7d07 7c05 a00a a100 7d08  j.d...}.|.....}.
+000011b0: 7c08 a00b 7c08 6409 6b04 6409 a102 7d09  |...|.d.k.d...}.
+000011c0: 7c08 a00b 7c08 6409 6b00 6409 a102 0b00  |...|.d.k.d.....
+000011d0: 7d0a 7c09 6a07 640a 6406 8d01 a008 a100  }.|.j.d.d.......
+000011e0: 7d0b 7c0a 6a07 640a 6406 8d01 a008 a100  }.|.j.d.d.......
+000011f0: 7d0c 7c0b 7c0c 1b00 7d0d 640b 640b 640c  }.|.|...}.d.d.d.
+00001200: 7c0d 1700 1b00 6a09 6407 1900 1800 7d0e  |.....j.d.....}.
+00001210: 7c0e 640d 6b05 72e0 640e 7d0f 6e04 640f  |.d.k.r.d.}.n.d.
+00001220: 7d0f 7c00 7c06 7c07 7c0e 7c0f 6410 9c05  }.|.|.|.|.|.d...
+00001230: 7d10 7c10 5300 2911 7579 0200 000a 2020  }.|.S.).uy....  
+00001240: 2020 2323 2055 7361 6269 6c69 6461 6465    ## Usabilidade
+00001250: 200a 2020 2020 2d20 63c3 a16c 6375 6c6f   .    - c..lculo
+00001260: 2065 6e76 6f6c 7665 2061 2063 6f6d 7061   envolve a compa
+00001270: 7261 c3a7 c3a3 6f20 6461 206d c3a9 6469  ra....o da m..di
+00001280: 6120 6465 2067 616e 686f 7320 656d 2075  a de ganhos em u
+00001290: 6d20 7065 72c3 ad6f 646f 2064 6520 7465  m per..odo de te
+000012a0: 6d70 6f20 636f 6d20 6120 6dc3 a964 6961  mpo com a m..dia
+000012b0: 2064 6520 7065 7264 6173 2065 6d20 756d   de perdas em um
+000012c0: 2070 6572 c3ad 6f64 6f20 6465 2074 656d   per..odo de tem
+000012d0: 706f 2e20 0a0a 2020 2020 0a20 2020 2023  po. ..    .    #
+000012e0: 2320 436f 6d6f 2069 6e74 6572 7072 6574  # Como interpret
+000012f0: 6172 200a 2020 2020 2d20 5175 616e 646f  ar .    - Quando
+00001300: 206f 2052 5349 2065 7374 c3a1 2061 6369   o RSI est.. aci
+00001310: 6d61 2064 6520 3730 2c20 6f20 6174 6976  ma de 70, o ativ
+00001320: 6f20 c3a9 2063 6f6e 7369 6465 7261 646f  o .. considerado
+00001330: 2073 6f62 7265 636f 6d70 7261 646f 2c20   sobrecomprado, 
+00001340: 6f20 7175 6520 7369 676e 6966 6963 6120  o que significa 
+00001350: 7175 6520 706f 6465 2065 7374 6172 2070  que pode estar p
+00001360: 7265 7374 6573 2061 2073 6f66 7265 7220  restes a sofrer 
+00001370: 756d 6120 636f 7272 65c3 a7c3 a36f 2070  uma corre....o p
+00001380: 6172 6120 6261 6978 6f2e 200a 2020 2020  ara baixo. .    
+00001390: 5175 616e 646f 206f 2052 5349 2065 7374  Quando o RSI est
+000013a0: c3a1 2061 6261 6978 6f20 6465 2033 302c  .. abaixo de 30,
+000013b0: 206f 2061 7469 766f 20c3 a920 636f 6e73   o ativo .. cons
+000013c0: 6964 6572 6164 6f20 736f 6272 6576 656e  iderado sobreven
+000013d0: 6469 646f 2c20 6f20 7175 6520 7369 676e  dido, o que sign
+000013e0: 6966 6963 6120 7175 6520 706f 6465 2065  ifica que pode e
+000013f0: 7374 6172 2070 7265 7374 6573 2061 2073  star prestes a s
+00001400: 7562 6972 206e 6f76 616d 656e 7465 2e20  ubir novamente. 
+00001410: 0a20 0a20 2020 202d 2073 6d61 5f35 3020  . .    - sma_50 
+00001420: 2d3e 204d 6564 6961 206d 6f76 656c 2064  -> Media movel d
+00001430: 6f73 2035 3020 7065 7269 6f64 6f73 0a20  os 50 periodos. 
+00001440: 2020 202d 2073 6d61 5f32 3030 202d 3e20     - sma_200 -> 
+00001450: 6d65 6469 6120 6d6f 7665 6c20 646f 7320  media movel dos 
+00001460: 3230 3020 7065 7269 646f 730a 0a20 2020  200 peridos..   
+00001470: 2023 2320 5061 72c3 a26d 6574 726f 730a   ## Par..metros.
+00001480: 2020 2020 2d20 7379 6d62 6f6c 202d 3e20      - symbol -> 
+00001490: 4e6f 6d65 2064 6f20 4174 6976 6f20 7061  Nome do Ativo pa
+000014a0: 7261 2061 2062 7573 6361 200a 0a20 2020  ra a busca ..   
+000014b0: 200a 2020 2020 7223 0000 00da 036d 6178   .    r#.....max
+000014c0: 723b 0000 0072 4700 0000 e932 0000 0029  r;...rG....2...)
+000014d0: 01da 0677 696e 646f 7772 2500 0000 e9c8  ...windowr%.....
+000014e0: 0000 0072 0100 0000 e90e 0000 00e9 6400  ...r..........d.
+000014f0: 0000 7215 0000 00e9 4600 0000 7a1f 4120  ..r.....F...z.A 
+00001500: 6368 616e 6365 2064 6f20 7072 6563 6f20  chance do preco 
+00001510: 646f 2061 7469 766f 2043 4149 527a 2041  do ativo CAIRz A
+00001520: 2063 6861 6e63 6520 646f 2070 7265 636f   chance do preco
+00001530: 2064 6f20 6174 6976 6f20 5355 4249 5229   do ativo SUBIR)
+00001540: 0572 2100 0000 da06 736d 615f 3530 da07  .r!.....sma_50..
+00001550: 736d 615f 3230 30da 0372 7369 5a08 7465  sma_200..rsiZ.te
+00001560: 6e64 656e 6379 290c 7229 0000 0072 2a00  ndency).r)...r*.
+00001570: 0000 722b 0000 0072 2c00 0000 722d 0000  ..r+...r,...r-..
+00001580: 0072 2e00 0000 723f 0000 005a 0772 6f6c  .r....r?...Z.rol
+00001590: 6c69 6e67 da04 6d65 616e 722f 0000 00da  ling..meanr/....
+000015a0: 0464 6966 66da 0577 6865 7265 2911 7221  .diff..where).r!
+000015b0: 0000 0072 3100 0000 722b 0000 0072 3200  ...r1...r+...r2.
+000015c0: 0000 723f 0000 0072 4b00 0000 7254 0000  ..r?...rK...rT..
+000015d0: 0072 5500 0000 da05 6465 6c74 615a 0467  .rU.....deltaZ.g
+000015e0: 6169 6e5a 046c 6f73 735a 0861 7667 5f67  ainZ.lossZ.avg_g
+000015f0: 6169 6e5a 0861 7667 5f6c 6f73 73da 0272  ainZ.avg_loss..r
+00001600: 7372 5600 0000 da06 7374 6174 7573 7233  srV.....statusr3
+00001610: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
+00001620: 0000 da14 6765 745f 7374 6f63 6b5f 7465  ....get_stock_te
+00001630: 6368 6e69 6361 6c73 ca00 0000 7336 0000  chnicals....s6..
+00001640: 0000 120a 0106 0108 0108 0102 0208 020c  ................
+00001650: 0108 0316 0116 0308 0110 0112 0110 0110  ................
+00001660: 0108 0116 0208 0106 0204 0302 0102 0102  ................
+00001670: 0102 0102 fb06 0a72 5d00 0000 7a19 7374  .......r]...z.st
+00001680: 6f63 6b73 2f7b 7379 6d62 6f6c 7d2f 7465  ocks/{symbol}/te
+00001690: 6368 6e69 6361 6c7a 1a73 746f 636b 732f  chnicalz.stocks/
+000016a0: 7b73 796d 626f 6c7d 2f76 6f6c 6174 696c  {symbol}/volatil
+000016b0: 6974 7929 0472 2100 0000 da0a 7374 6172  ity).r!.....star
+000016c0: 745f 6461 7465 da08 656e 645f 6461 7465  t_date..end_date
+000016d0: 7222 0000 0063 0300 0000 0000 0000 0000  r"...c..........
+000016e0: 0000 0600 0000 0600 0000 4300 0000 7368  ..........C...sh
+000016f0: 0000 007a 2874 006a 017c 007c 017c 0264  ...z(t.j.|.|.|.d
+00001700: 018d 037d 037c 036a 0272 2664 0274 0364  ...}.|.j.r&d.t.d
+00001710: 0383 0169 0157 0053 0057 006e 0c01 0001  ...i.W.S.W.n....
+00001720: 0001 0059 006e 0230 0074 04a0 057c 0364  ...Y.n.0.t...|.d
+00001730: 0419 007c 0364 0419 00a0 0664 05a1 011b  ...|.d.....d....
+00001740: 00a1 017d 0474 04a0 0764 067c 04a0 08a1  ...}.t...d.|....
+00001750: 0014 00a1 017d 057c 0553 0029 0775 6e01  .....}.|.S.).un.
+00001760: 0000 0a20 2020 2023 2320 5573 6162 696c  ...    ## Usabil
+00001770: 6964 6164 6520 0a20 2020 202d 204d c3a9  idade .    - M..
+00001780: 746f 646f 2075 7361 646f 2070 6172 6120  todo usado para 
+00001790: 7665 7269 6669 6361 7220 6120 766f 6c61  verificar a vola
+000017a0: 7469 6c69 6461 6465 2064 6520 756d 2061  tilidade de um a
+000017b0: 7469 766f 2065 6d20 636f 6d70 6172 6163  tivo em comparac
+000017c0: 616f 2061 6f20 6d65 7263 6164 6f20 656d  ao ao mercado em
+000017d0: 2071 7565 2065 7374 6120 200a 0a20 2020   que esta  ..   
+000017e0: 200a 2020 2020 2323 2050 6172 c3a2 6d65   .    ## Par..me
+000017f0: 7472 6f73 0a20 2020 202d 2073 796d 626f  tros.    - symbo
+00001800: 6c20 2d3e 204e 6f6d 6520 646f 2041 7469  l -> Nome do Ati
+00001810: 766f 2070 6172 6120 6120 6275 7363 6120  vo para a busca 
+00001820: 0a0a 2020 2020 2d20 7374 6172 745f 6461  ..    - start_da
+00001830: 7465 202d 3e20 4461 7461 2064 6520 496e  te -> Data de In
+00001840: 6963 696f 2064 6120 6275 7363 6120 6461  icio da busca da
+00001850: 7320 696e 666f 7320 2870 7265 636f 2c20  s infos (preco, 
+00001860: 766f 6c75 6d65 2c20 6574 6329 2064 6f20  volume, etc) do 
+00001870: 6174 6976 6f20 0a0a 2020 2020 2d20 656e  ativo ..    - en
+00001880: 645f 6461 7465 202d 3e20 4461 7461 2046  d_date -> Data F
+00001890: 696e 616c 2070 6172 6120 6120 6275 7363  inal para a busc
+000018a0: 6120 6461 7320 696e 666f 7320 2870 7265  a das infos (pre
+000018b0: 636f 2c20 766f 6c75 6d65 2c20 6574 6329  co, volume, etc)
+000018c0: 2064 6f20 6174 6976 6f20 0a0a 2020 2020   do ativo ..    
+000018d0: a902 da05 7374 6172 74da 0365 6e64 723c  ....start..endr<
+000018e0: 0000 007a 384e 616f 2066 6f69 2065 6e63  ...z8Nao foi enc
+000018f0: 6f6e 7472 6164 6f20 6f20 6869 7374 6f72  ontrado o histor
+00001900: 6963 6f20 6e65 7373 6520 7065 7269 6f64  ico nesse period
+00001910: 6f2c 2076 6572 6966 6963 6172 2e72 4700  o, verificar.rG.
+00001920: 0000 7215 0000 00e9 fc00 0000 2909 7229  ..r.........).r)
+00001930: 0000 00da 0864 6f77 6e6c 6f61 6472 4000  .....downloadr@.
+00001940: 0000 722e 0000 00da 026e 70da 036c 6f67  ..r......np..log
+00001950: da05 7368 6966 74da 0473 7172 74da 0376  ..shift..sqrt..v
+00001960: 6172 2906 7221 0000 0072 5e00 0000 725f  ar).r!...r^...r_
+00001970: 0000 005a 0a73 746f 636b 5f64 6174 615a  ...Z.stock_dataZ
+00001980: 0b6c 6f67 5f72 6574 7572 6e73 5a0a 766f  .log_returnsZ.vo
+00001990: 6c61 7469 6c69 7479 721e 0000 0072 1e00  latilityr....r..
+000019a0: 0000 721f 0000 00da 0e67 6574 5f76 6f6c  ..r......get_vol
+000019b0: 6174 696c 6974 790c 0100 0073 1200 0000  atility....s....
+000019c0: 000d 0201 1001 0601 1201 0601 0602 1c01  ................
+000019d0: 1202 726a 0000 007a 1473 746f 636b 732f  ..rj...z.stocks/
+000019e0: 7b73 796d 626f 6c7d 2f62 6574 6163 0100  {symbol}/betac..
+000019f0: 0000 0000 0000 0000 0000 0f00 0000 0300  ................
+00001a00: 0000 4300 0000 73be 0000 0074 00a0 017c  ..C...s....t...|
+00001a10: 00a1 017d 0174 00a0 0164 01a1 017d 027c  ...}.t...d...}.|
+00001a20: 016a 027d 037c 026a 027d 0474 037c 0383  .j.}.|.j.}.t.|..
+00001a30: 017d 057c 0574 046b 0273 427c 0474 046b  .}.|.t.k.sB|.t.k
+00001a40: 0272 3a6e 0874 0564 0283 0101 007c 016a  .r:n.t.d.....|.j
+00001a50: 0664 0364 048d 017d 067c 026a 0664 0364  .d.d...}.|.j.d.d
+00001a60: 048d 017d 077c 0664 0519 00a0 07a1 007d  ...}.|.d.......}
+00001a70: 087c 0764 0519 00a0 07a1 007d 097c 08a0  .|.d.......}.|..
+00001a80: 087c 09a1 017d 0a7c 09a0 09a1 007d 0b7c  .|...}.|.....}.|
+00001a90: 0a7c 0b1b 007d 0c7c 0c64 066b 0472 9864  .|...}.|.d.k.r.d
+00001aa0: 077d 0d7c 0c64 066b 0072 a464 087d 0d7c  .}.|.d.k.r.d.}.|
+00001ab0: 0c64 066b 0272 b064 097d 0d7c 0c7c 0d64  .d.k.r.d.}.|.|.d
+00001ac0: 0a9c 027d 0e7c 0e53 0029 0b75 9501 0000  ...}.|.S.).u....
+00001ad0: 0a20 2020 2023 2320 5573 6162 696c 6964  .    ## Usabilid
+00001ae0: 6164 6520 0a20 2020 202d 204f 2062 6574  ade .    - O bet
+00001af0: 6120 c3a9 2075 6d61 206d 6564 6964 6120  a .. uma medida 
+00001b00: 6573 7461 74c3 ad73 7469 6361 2071 7565  estat..stica que
+00001b10: 2069 6e64 6963 6120 6120 7265 6c61 c3a7   indica a rela..
+00001b20: c3a3 6f20 656e 7472 6520 6120 766f 6c61  ..o entre a vola
+00001b30: 7469 6c69 6461 6465 2064 6520 756d 6120  tilidade de uma 
+00001b40: 61c3 a7c3 a36f 2065 2061 2076 6f6c 6174  a....o e a volat
+00001b50: 696c 6964 6164 6520 646f 206d 6572 6361  ilidade do merca
+00001b60: 646f 2063 6f6d 6f20 756d 2074 6f64 6f2e  do como um todo.
+00001b70: 0a20 2020 204f 2076 616c 6f72 2064 6f20  .    O valor do 
+00001b80: 6265 7461 20c3 a920 7574 696c 697a 6164  beta .. utilizad
+00001b90: 6f20 7061 7261 206d 6564 6972 206f 2072  o para medir o r
+00001ba0: 6973 636f 2064 6520 756d 6120 61c3 a7c3  isco de uma a...
+00001bb0: a36f 2065 6d20 7265 6c61 c3a7 c3a3 6f20  .o em rela....o 
+00001bc0: 616f 206d 6572 6361 646f 2065 6d20 7175  ao mercado em qu
+00001bd0: 6520 656c 6120 c3a9 206e 6567 6f63 6961  e ela .. negocia
+00001be0: 6461 2e20 0a0a 2020 2020 0a20 2020 2023  da. ..    .    #
+00001bf0: 2320 5061 72c3 a26d 6574 726f 730a 2020  # Par..metros.  
+00001c00: 2020 2d20 7379 6d62 6f6c 202d 3e20 4e6f    - symbol -> No
+00001c10: 6d65 2064 6f20 4174 6976 6f20 7061 7261  me do Ativo para
+00001c20: 2061 2062 7573 6361 200a 0a20 2020 202d   a busca ..    -
+00001c30: 206d 6172 6b65 7420 2d3e 2043 6f6d 6f20   market -> Como 
+00001c40: 7061 6472 616f 2c20 4d65 7263 6164 6f3a  padrao, Mercado:
+00001c50: 2049 424f 5645 5350 4120 2f20 4256 5350   IBOVESPA / BVSP
+00001c60: 0a20 2020 207a 055e 4256 5350 7223 0000  .    z.^BVSPr#..
+00001c70: 0072 4d00 0000 723b 0000 0072 4700 0000  .rM...r;...rG...
+00001c80: 7215 0000 007a 2841 6361 6f20 6d61 6973  r....z(Acao mais
+00001c90: 2056 6f6c 6174 696c 2071 7565 206f 206d   Volatil que o m
+00001ca0: 6572 6361 646f 2065 6d20 6765 7261 6c7a  ercado em geralz
+00001cb0: 2941 6361 6f20 6d65 6e6f 7320 566f 6c61  )Acao menos Vola
+00001cc0: 7469 6c20 7175 6520 6f20 6d65 7263 6164  til que o mercad
+00001cd0: 6f20 656d 2067 6572 616c 7a34 4163 616f  o em geralz4Acao
+00001ce0: 2063 6f6d 2061 206d 6573 6d61 2056 6f6c   com a mesma Vol
+00001cf0: 6174 696c 6964 6164 6520 7175 6520 6f20  atilidade que o 
+00001d00: 6d65 7263 6164 6f20 656d 2067 6572 616c  mercado em geral
+00001d10: 2902 da04 6265 7461 725c 0000 0029 0a72  )...betar\...).r
+00001d20: 2900 0000 722a 0000 0072 2b00 0000 722c  )...r*...r+...r,
+00001d30: 0000 0072 2d00 0000 722e 0000 0072 3f00  ...r-...r....r?.
+00001d40: 0000 da0a 7063 745f 6368 616e 6765 da03  ....pct_change..
+00001d50: 636f 7672 6900 0000 290f 7221 0000 005a  covri...).r!...Z
+00001d60: 0561 7373 6574 5a06 6d61 726b 6574 722b  .assetZ.marketr+
+00001d70: 0000 005a 0a69 6e66 6f4d 6172 6b65 7472  ...Z.infoMarketr
+00001d80: 3200 0000 5a0d 6173 7365 745f 6869 7374  2...Z.asset_hist
+00001d90: 6f72 795a 0e6d 6172 6b65 745f 6869 7374  oryZ.market_hist
+00001da0: 6f72 795a 0d61 7373 6574 5f72 6574 7572  oryZ.asset_retur
+00001db0: 6e73 5a0e 6d61 726b 6574 5f72 6574 7572  nsZ.market_retur
+00001dc0: 6e73 726d 0000 0072 6900 0000 726b 0000  nsrm...ri...rk..
+00001dd0: 0072 5c00 0000 7233 0000 0072 1e00 0000  .r\...r3...r....
+00001de0: 721e 0000 0072 1f00 0000 da08 6765 745f  r....r......get_
+00001df0: 6265 7461 2c01 0000 7332 0000 0000 0e0a  beta,...s2......
+00001e00: 010a 0106 0106 0108 0110 0102 0208 020c  ................
+00001e10: 010c 030c 010c 030a 0108 0108 0208 0104  ................
+00001e20: 0108 0104 0108 0104 0302 0102 ff06 0572  ...............r
+00001e30: 6e00 0000 7a13 7374 6f63 6b73 2f7b 7379  n...z.stocks/{sy
+00001e40: 6d62 6f6c 7d2f 5661 5229 0472 2100 0000  mbol}/VaR).r!...
+00001e50: da10 636f 6e66 6964 656e 6365 5f6c 6576  ..confidence_lev
+00001e60: 656c da0f 6c6f 6f6b 6261 636b 5f70 6572  el..lookback_per
+00001e70: 696f 6472 2200 0000 6303 0000 0000 0000  iodr"...c.......
+00001e80: 0000 0000 000b 0000 0006 0000 0043 0000  .............C..
+00001e90: 0073 9e00 0000 7400 a001 7c00 a101 7d03  .s....t...|...}.
+00001ea0: 7c03 6a02 7d04 7403 7c04 8301 7d05 7c05  |.j.}.t.|...}.|.
+00001eb0: 7404 6b02 7222 6e08 7405 6401 8301 0100  t.k.r"n.t.d.....
+00001ec0: 7c03 6a06 7c02 9b00 6402 9d02 6403 8d01  |.j.|...d...d...
+00001ed0: 6404 1900 7d06 7407 a008 7c06 7c06 a009  d...}.t...|.|...
+00001ee0: 6405 a101 1b00 a101 7d07 7c07 a00a a100  d.......}.|.....
+00001ef0: 7d08 7c08 740b a00c 6405 7c01 1800 a101  }.|.t...d.|.....
+00001f00: 1400 7d09 7405 6406 740d 7c09 7c06 6407  ..}.t.d.t.|.|.d.
+00001f10: 1900 1400 6408 8302 6901 8301 0100 740d  ....d...i.....t.
+00001f20: 7c09 7c06 6407 1900 1400 6408 8302 7d0a  |.|.d.....d...}.
+00001f30: 7c0a 5300 2909 75c8 0100 000a 2020 2020  |.S.).u.....    
+00001f40: 2323 2055 7361 6269 6c69 6461 6465 200a  ## Usabilidade .
+00001f50: 2020 2020 2d20 4f20 5661 6c75 6520 6174      - O Value at
+00001f60: 2052 6973 6b20 2856 6152 2920 c3a9 2075   Risk (VaR) .. u
+00001f70: 6d61 206d 6564 6964 6120 6465 2072 6973  ma medida de ris
+00001f80: 636f 2071 7565 2069 6e64 6963 6120 6120  co que indica a 
+00001f90: 7065 7264 6120 6dc3 a178 696d 6120 6573  perda m..xima es
+00001fa0: 7065 7261 6461 2c20 636f 6d20 756d 2064  perada, com um d
+00001fb0: 6574 6572 6d69 6e61 646f 206e c3ad 7665  eterminado n..ve
+00001fc0: 6c20 6465 2063 6f6e 6669 616e c3a7 612c  l de confian..a,
+00001fd0: 2065 6d20 756d 2069 6e74 6572 7661 6c6f   em um intervalo
+00001fe0: 2064 6520 7465 6d70 6f20 7072 c3a9 2d64   de tempo pr..-d
+00001ff0: 6574 6572 6d69 6e61 646f 2e20 0a0a 2020  eterminado. ..  
+00002000: 2020 0a20 2020 2023 2320 5061 72c3 a26d    .    ## Par..m
+00002010: 6574 726f 730a 2020 2020 0a20 2020 202d  etros.    .    -
+00002020: 2073 796d 626f 6c20 2d3e 204e 6f6d 6520   symbol -> Nome 
+00002030: 646f 2041 7469 766f 2070 6172 6120 6661  do Ativo para fa
+00002040: 7a65 7220 6120 6275 7363 6120 0a0a 2020  zer a busca ..  
+00002050: 2020 2d20 636f 6e66 6964 656e 6365 5f6c    - confidence_l
+00002060: 6576 656c 202d 3e20 4e69 7665 6c20 6465  evel -> Nivel de
+00002070: 2063 6f6e 6669 616e c3a7 6120 7061 7261   confian..a para
+00002080: 206f 2056 4152 2028 3020 6120 3129 2c20   o VAR (0 a 1), 
+00002090: 6e6f 726d 616c 6d65 6e74 6520 7573 6164  normalmente usad
+000020a0: 6f20 656d 2030 2e39 3520 0a0a 2020 2020  o em 0.95 ..    
+000020b0: 2d20 6c6f 6f6b 6261 636b 5f70 6572 696f  - lookback_perio
+000020c0: 6420 2d3e 2050 6572 696f 646f 2045 4d20  d -> Periodo EM 
+000020d0: 4449 4153 2061 2073 6572 2063 6f6e 7369  DIAS a ser consi
+000020e0: 6465 7261 646f 2070 6172 6120 6f20 63c3  derado para o c.
+000020f0: a16c 6375 6c6f 2064 6f20 5661 520a 0a20  .lculo do VaR.. 
+00002100: 2020 2072 2300 0000 da01 6472 3b00 0000     r#.....dr;...
+00002110: 7247 0000 0072 1500 0000 5a03 5661 5272  rG...r....Z.VaRr
+00002120: 2500 0000 e902 0000 0029 0e72 2900 0000  %........).r)...
+00002130: 722a 0000 0072 2b00 0000 722c 0000 0072  r*...r+...r,...r
+00002140: 2d00 0000 722e 0000 0072 3f00 0000 7265  -...r....r?...re
+00002150: 0000 0072 6600 0000 7267 0000 00da 0373  ...rf...rg.....s
+00002160: 7464 7202 0000 005a 0370 7066 da05 726f  tdr....Z.ppf..ro
+00002170: 756e 6429 0b72 2100 0000 726f 0000 0072  und).r!...ro...r
+00002180: 7000 0000 7231 0000 0072 2b00 0000 7232  p...r1...r+...r2
+00002190: 0000 005a 0670 7269 6365 73da 0772 6574  ...Z.prices..ret
+000021a0: 7572 6e73 5a07 7374 645f 6465 7672 6900  urnsZ.std_devri.
+000021b0: 0000 5a03 5661 7272 1e00 0000 721e 0000  ..Z.Varr....r...
+000021c0: 0072 1f00 0000 da07 6765 745f 7661 7266  .r......get_varf
+000021d0: 0100 0073 1a00 0000 000f 0a01 0601 0801  ...s............
+000021e0: 0801 0202 0803 1603 1403 0801 1201 1a01  ................
+000021f0: 1201 7276 0000 007a 1c73 746f 636b 732f  ..rv...z.stocks/
+00002200: 7b73 796d 626f 6c7d 2f41 6e6e 7561 6c52  {symbol}/AnnualR
+00002210: 6574 7572 6e29 04da 0773 796d 626f 6c73  eturn)...symbols
+00002220: 725e 0000 0072 5f00 0000 7222 0000 0063  r^...r_...r"...c
+00002230: 0300 0000 0000 0000 0000 0000 1100 0000  ................
+00002240: 0700 0000 4300 0000 7392 0100 0074 007c  ....C...s....t.|
+00002250: 0074 0183 0272 c874 0264 017c 009b 009d  .t...r.t.d.|....
+00002260: 0283 0101 0074 036a 047c 007c 017c 0264  .....t.j.|.|.|.d
+00002270: 0264 038d 047d 037a 8674 03a0 057c 00a1  .d...}.z.t...|..
+00002280: 016a 067d 047c 0464 0419 007d 057c 0364  .j.}.|.d...}.|.d
+00002290: 0519 007d 067c 06a0 07a1 007d 077c 07a0  ...}.|.....}.|..
+000022a0: 08a1 0064 0614 007d 087c 07a0 09a1 0064  ...d...}.|.....d
+000022b0: 0714 007d 097c 066a 0a64 0819 0064 0914  ...}.|.j.d...d..
+000022c0: 007d 0a7c 066a 0a64 0a19 0064 0914 007d  .}.|.j.d...d...}
+000022d0: 0b7c 0b7c 0a18 007c 0a1b 007d 0c74 0b6a  .|.|...|...}.t.j
+000022e0: 0c7c 007c 057c 087c 097c 0c64 0b9c 0564  .|.|.|.|.|.d...d
+000022f0: 0c67 0164 0d8d 027d 0d7c 0d57 0053 0001  .g.d...}.|.W.S..
+00002300: 0001 0001 0074 0264 0e83 0101 0059 006e  .....t.d.....Y.n
+00002310: 0230 006e c674 007c 0074 0d83 0290 0172  .0.n.t.|.t.....r
+00002320: 8674 0ba0 0ca1 007d 0e74 0264 0f7c 009b  .t.....}.t.d.|..
+00002330: 009d 0283 0101 007c 0044 005d 927d 0f74  .......|.D.].}.t
+00002340: 036a 047c 0f7c 017c 0264 0264 038d 047d  .j.|.|.|.d.d...}
+00002350: 037c 0364 0519 007d 067c 06a0 07a1 007d  .|.d...}.|.....}
+00002360: 077c 07a0 08a1 0064 0614 007d 087c 07a0  .|.....d...}.|..
+00002370: 09a1 0064 0714 007d 097c 066a 0a64 0819  ...d...}.|.j.d..
+00002380: 0064 0914 007d 0a7c 066a 0a64 0a19 0064  .d...}.|.j.d...d
+00002390: 0914 007d 0b7c 0b7c 0a18 007c 0a1b 007d  ...}.|.|...|...}
+000023a0: 0c74 0b6a 0c7c 0f7c 087c 097c 0c64 109c  .t.j.|.|.|.|.d..
+000023b0: 0474 0e7c 0083 0167 0164 0d8d 027d 1074  .t.|...g.d...}.t
+000023c0: 0ba0 0f7c 107c 0e67 02a1 017d 0e71 ee7c  ...|.|.g...}.q.|
+000023d0: 0e53 0074 0264 1183 0101 0064 1253 0029  .S.t.d.....d.S.)
+000023e0: 1375 9b01 0000 0a20 2020 2023 2320 5573  .u.....    ## Us
+000023f0: 6162 696c 6964 6164 650a 2020 2020 2d20  abilidade.    - 
+00002400: 5265 6365 6265 2075 6d61 206c 6973 7461  Recebe uma lista
+00002410: 2065 2072 6574 6f72 6e61 2075 6d20 4461   e retorna um Da
+00002420: 7461 4672 616d 6520 636f 6d20 6173 2069  taFrame com as i
+00002430: 6e66 6f72 6d61 c3a7 c3b5 6573 2064 6f73  nforma....es dos
+00002440: 2061 7469 766f 7320 6520 616c 6775 6d61   ativos e alguma
+00002450: 7320 6573 7461 74c3 ad73 7469 6361 7320  s estat..sticas 
+00002460: 62c3 a173 6963 6173 2e20 0a0a 2020 2020  b..sicas. ..    
+00002470: 0a20 2020 2023 2320 5061 72c3 a26d 6574  .    ## Par..met
+00002480: 726f 730a 2020 2020 2d20 7379 6d62 6f6c  ros.    - symbol
+00002490: 7320 2d3e 2052 6563 6562 6520 756d 6120  s -> Recebe uma 
+000024a0: 6c69 7374 6120 6f75 2075 6d20 756e 6963  lista ou um unic
+000024b0: 6f20 6174 6976 6f20 7061 7261 2062 7573  o ativo para bus
+000024c0: 6361 7220 6e61 2062 6173 6520 0a0a 2020  car na base ..  
+000024d0: 2020 2d20 7374 6172 745f 6461 7465 202d    - start_date -
+000024e0: 3e20 4461 7461 2064 6520 496e 6963 696f  > Data de Inicio
+000024f0: 2064 6120 6275 7363 6120 6461 7320 696e   da busca das in
+00002500: 666f 7320 2870 7265 636f 2c20 766f 6c75  fos (preco, volu
+00002510: 6d65 2c20 6574 6329 2064 6f20 6174 6976  me, etc) do ativ
+00002520: 6f20 0a0a 2020 2020 2d20 656e 645f 6461  o ..    - end_da
+00002530: 7465 202d 3e20 4461 7461 2046 696e 616c  te -> Data Final
+00002540: 2070 6172 6120 6120 6275 7363 6120 6461   para a busca da
+00002550: 7320 696e 666f 7320 2870 7265 636f 2c20  s infos (preco, 
+00002560: 766f 6c75 6d65 2c20 6574 6329 2064 6f20  volume, etc) do 
+00002570: 6174 6976 6f20 0a0a 2020 2020 0a20 2020  ativo ..    .   
+00002580: 2075 1a00 0000 566f 63c3 aa20 6469 6769   u....Voc.. digi
+00002590: 746f 7520 756d 6120 7374 7269 6e67 3a20  tou uma string: 
+000025a0: da06 7469 636b 6572 2904 5a07 7469 636b  ..ticker).Z.tick
+000025b0: 6572 7372 6100 0000 7262 0000 005a 0867  ersra...rb...Z.g
+000025c0: 726f 7570 5f62 7972 2400 0000 7247 0000  roup_byr$...rG..
+000025d0: 0072 6300 0000 675f 75bc 7ebf bf2f 4072  .rc...g_u.~../@r
+000025e0: 0100 0000 7252 0000 0072 2500 0000 2905  ....rR...r%...).
+000025f0: da05 4174 6976 6f75 1000 0000 5072 65c3  ..Ativou....Pre.
+00002600: a76f 2061 204d 6572 6361 646f fa0d 5265  .o a Mercado..Re
+00002610: 746f 726e 6f20 616e 7561 6cf5 1400 0000  torno anual.....
+00002620: 4465 7376 696f 2070 6164 72c3 a36f 2061  Desvio padr..o a
+00002630: 6e75 616c fa0d 5265 746f 726e 6f20 746f  nual..Retorno to
+00002640: 7461 6c72 1500 0000 a901 da05 696e 6465  talr........inde
+00002650: 7875 1000 0000 5469 636b 6572 2069 6e76  xu....Ticker inv
+00002660: c3a1 6c69 646f 7519 0000 0056 6f63 c3aa  ..lidou....Voc..
+00002670: 2064 6967 6974 6f75 2075 6d61 206c 6973   digitou uma lis
+00002680: 7461 3a20 2904 7279 0000 0072 7a00 0000  ta: ).ry...rz...
+00002690: 727b 0000 0072 7c00 0000 752f 0000 0054  r{...r|...u/...T
+000026a0: 6970 6f20 696e 76c3 a16c 6964 6f2e 2044  ipo inv..lido. D
+000026b0: 6967 6974 6520 756d 6120 7374 7269 6e67  igite uma string
+000026c0: 206f 7520 756d 6120 6c69 7374 612e 4e29   ou uma lista.N)
+000026d0: 10da 0a69 7369 6e73 7461 6e63 65da 0373  ...isinstance..s
+000026e0: 7472 722e 0000 0072 2900 0000 7264 0000  trr....r)...rd..
+000026f0: 0072 2a00 0000 722b 0000 0072 6c00 0000  .r*...r+...rl...
+00002700: 7257 0000 0072 7300 0000 722f 0000 0072  rW...rs...r/...r
+00002710: 4200 0000 7243 0000 0072 3d00 0000 da03  B...rC...r=.....
+00002720: 6c65 6eda 0663 6f6e 6361 7429 1172 7700  len..concat).rw.
+00002730: 0000 725e 0000 0072 5f00 0000 da05 6461  ..r^...r_.....da
+00002740: 646f 73da 0464 6174 615a 0b76 616c 7565  dos..dataZ.value
+00002750: 4d61 726b 6574 da05 636c 6f73 655a 0e72  Market..closeZ.r
+00002760: 6574 6f72 6e6f 5f64 6961 7269 6f5a 0d72  etorno_diarioZ.r
+00002770: 6574 6f72 6e6f 5f61 6e75 616c 5a13 6465  etorno_anualZ.de
+00002780: 7376 696f 5f70 6164 7261 6f5f 616e 7561  svio_padrao_anua
+00002790: 6c5a 0f76 616c 6f72 5f69 6e76 6573 7469  lZ.valor_investi
+000027a0: 646f 5a0b 7661 6c6f 725f 6174 7561 6c5a  doZ.valor_atualZ
+000027b0: 0d72 6574 6f72 6e6f 5f74 6f74 616c 5a0c  .retorno_totalZ.
+000027c0: 7661 6c75 6553 796d 626f 6c73 5a07 7661  valueSymbolsZ.va
+000027d0: 6c75 6544 465a 0773 696d 626f 6c6f 5a0d  lueDFZ.simboloZ.
+000027e0: 7265 7475 726e 5379 6d62 6f6c 7372 1e00  returnSymbolsr..
+000027f0: 0000 721e 0000 0072 1f00 0000 da0f 6173  ..r....r......as
+00002800: 7365 745f 706f 7274 666f 6c69 6f91 0100  set_portfolio...
+00002810: 0073 6000 0000 000e 0a01 0e01 1202 0202  .s`.............
+00002820: 0c01 0803 0803 0803 0c03 0c03 0e03 0e03  ................
+00002830: 0c03 0401 0201 0201 0201 0201 02fb 0406  ................
+00002840: 04fa 0608 0602 0601 1002 0c01 0801 0e01  ................
+00002850: 0801 1203 0803 0803 0c03 0c03 0e03 0e03  ................
+00002860: 0c03 0401 0201 0201 0201 02fc 0405 08fb  ................
+00002870: 0607 1002 0402 7286 0000 007a 2473 746f  ......r....z$sto
+00002880: 636b 732f 7b73 796d 626f 6c7d 2f4d 6172  cks/{symbol}/Mar
+00002890: 6b6f 7769 747a 416c 6c6f 6361 7469 6f6e  kowitzAllocation
+000028a0: 6e29 0472 7700 0000 da09 7374 6172 5f64  n).rw.....star_d
+000028b0: 6174 6572 5f00 0000 7222 0000 0063 0300  ater_...r"...c..
+000028c0: 0000 0000 0000 0000 0000 1100 0000 0900  ................
+000028d0: 0000 4300 0000 733a 0100 0074 006a 017c  ..C...s:...t.j.|
+000028e0: 007c 017c 0264 018d 0364 0219 007d 037c  .|.|.d...d...}.|
+000028f0: 03a0 02a1 00a0 03a1 007d 047c 04a0 04a1  .........}.|....
+00002900: 007d 0574 05a0 0664 0374 077c 0083 011b  .}.t...d.t.|....
+00002910: 0067 0174 077c 0083 0114 00a1 017d 0674  .g.t.|.......}.t
+00002920: 05a0 087c 04a0 09a1 007c 0614 00a1 0164  ...|.....|.....d
+00002930: 0414 007d 0774 05a0 0a74 05a0 0b7c 066a  ...}.t...t...|.j
+00002940: 0c74 05a0 0b7c 057c 06a1 02a1 02a1 0174  .t...|.|.......t
+00002950: 05a0 0a64 04a1 0114 007d 0864 0574 05a0  ...d.....}.d.t..
+00002960: 0d7c 05a1 0114 007d 0974 056a 0ea0 0f7c  .|.....}.t.j...|
+00002970: 057c 0974 05a0 107c 056a 1164 0619 00a1  .|.t...|.j.d....
+00002980: 0114 0017 00a1 017d 0a74 05a0 1274 077c  .......}.t...t.|
+00002990: 0083 0164 0366 02a1 017d 0b74 05a0 0b7c  ...d.f...}.t...|
+000029a0: 0a7c 0ba1 0274 05a0 0b74 05a0 0b7c 0b6a  .|...t...t...|.j
+000029b0: 0c7c 0aa1 027c 0ba1 021b 007d 0c7c 0ca0  .|...|.....}.|..
+000029c0: 13a1 007d 0c67 007d 0d74 1474 077c 0083  ...}.g.}.t.t.|..
+000029d0: 0183 0144 005d 2e7d 0e64 077c 007c 0e19  ...D.].}.d.|.|..
+000029e0: 009b 0064 087c 0c7c 0e19 0064 0914 0064  ...d.|.|...d...d
+000029f0: 0a9b 0464 0b9d 057d 0f7c 0da0 157c 0fa1  ...d...}.|...|..
+00002a00: 0101 0071 fa7c 077c 087c 0d64 0c9c 037d  ...q.|.|.|.d...}
+00002a10: 107c 1053 0029 0d75 2403 0000 0a20 2020  .|.S.).u$....   
+00002a20: 2023 2320 5573 6162 696c 6964 6164 6573   ## Usabilidades
+00002a30: 200a 2020 2020 2d20 416c 6f63 61c3 a7c3   .    - Aloca...
+00002a40: a36f 2064 6520 4d61 726b 6f77 6974 7a20  .o de Markowitz 
+00002a50: c3a9 2075 6d61 2074 c3a9 636e 6963 6120  .. uma t..cnica 
+00002a60: 6465 206f 7469 6d69 7a61 c3a7 c3a3 6f20  de otimiza....o 
+00002a70: 6465 2070 6f72 7466 c3b3 6c69 6f20 7175  de portf..lio qu
+00002a80: 6520 7669 7361 2065 6e63 6f6e 7472 6172  e visa encontrar
+00002a90: 2061 2063 6f6d 6269 6e61 c3a7 c3a3 6f20   a combina....o 
+00002aa0: 6964 6561 6c20 6465 2061 7469 766f 7320  ideal de ativos 
+00002ab0: 7061 7261 206d 6178 696d 697a 6172 206f  para maximizar o
+00002ac0: 2072 6574 6f72 6e6f 2064 6f20 696e 7665   retorno do inve
+00002ad0: 7374 696d 656e 746f 2065 6e71 7561 6e74  stimento enquant
+00002ae0: 6f20 6d69 6e69 6d69 7a61 206f 2072 6973  o minimiza o ris
+00002af0: 636f 2e20 0a0a 0a20 2020 2023 2320 4f20  co. ...    ## O 
+00002b00: 5265 746f 726e 6f20 4573 7065 7261 646f  Retorno Esperado
+00002b10: 0a20 2020 202d 2072 6570 7265 7365 6e74  .    - represent
+00002b20: 6120 6120 7461 7861 2064 6520 7265 746f  a a taxa de reto
+00002b30: 726e 6f20 6dc3 a964 6961 2071 7565 2073  rno m..dia que s
+00002b40: 6520 6573 7065 7261 206f 6274 6572 2064  e espera obter d
+00002b50: 6f20 706f 7274 66c3 b36c 696f 2064 6520  o portf..lio de 
+00002b60: 696e 7665 7374 696d 656e 746f 7320 0a0a  investimentos ..
+00002b70: 2020 2020 2323 204f 2052 6973 636f 200a      ## O Risco .
+00002b80: 2020 2020 2d20 7265 7072 6573 656e 7461      - representa
+00002b90: 2061 206d 6564 6964 6120 6465 2076 6f6c   a medida de vol
+00002ba0: 6174 696c 6964 6164 6520 646f 2070 6f72  atilidade do por
+00002bb0: 7466 c3b3 6c69 6f2c 206f 7520 7365 6a61  tf..lio, ou seja
+00002bc0: 2c20 0a20 2020 2071 7561 6e74 6f20 6d61  , .    quanto ma
+00002bd0: 6973 2069 6e73 74c3 a176 656c 2066 6f72  is inst..vel for
+00002be0: 206f 2072 6574 6f72 6e6f 2064 6f73 2061   o retorno dos a
+00002bf0: 7469 766f 732c 206d 6169 6f72 2073 6572  tivos, maior ser
+00002c00: c3a1 206f 2072 6973 636f 2064 6f20 706f  .. o risco do po
+00002c10: 7274 66c3 b36c 696f 2063 6f6d 6f20 756d  rtf..lio como um
+00002c20: 2074 6f64 6f20 0a0a 2020 2020 0a20 2020   todo ..    .   
+00002c30: 200a 2020 2020 0a20 2020 2023 2320 5061   .    .    ## Pa
+00002c40: 72c3 a26d 6574 726f 730a 2020 2020 0a20  r..metros.    . 
+00002c50: 2020 202d 2073 796d 626f 6c73 202d 3e20     - symbols -> 
+00002c60: 5265 6365 6265 2075 6d61 206c 6973 7461  Recebe uma lista
+00002c70: 2064 6520 6174 6976 6f73 2070 6172 6120   de ativos para 
+00002c80: 6275 7363 6172 206e 6120 6261 7365 200a  buscar na base .
+00002c90: 0a20 2020 202d 2073 7461 7274 5f64 6174  .    - start_dat
+00002ca0: 6520 2d3e 2044 6174 6120 6465 2049 6e69  e -> Data de Ini
+00002cb0: 6369 6f20 6461 2062 7573 6361 2064 6173  cio da busca das
+00002cc0: 2069 6e66 6f73 2028 7072 6563 6f2c 2076   infos (preco, v
+00002cd0: 6f6c 756d 652c 2065 7463 2920 646f 2061  olume, etc) do a
+00002ce0: 7469 766f 200a 0a20 2020 202d 2065 6e64  tivo ..    - end
+00002cf0: 5f64 6174 6520 2d3e 2044 6174 6120 4669  _date -> Data Fi
+00002d00: 6e61 6c20 7061 7261 2061 2062 7573 6361  nal para a busca
+00002d10: 2064 6173 2069 6e66 6f73 2028 7072 6563   das infos (prec
+00002d20: 6f2c 2076 6f6c 756d 652c 2065 7463 2920  o, volume, etc) 
+00002d30: 646f 2061 7469 766f 200a 0a0a 2020 2020  do ativo ...    
+00002d40: 7260 0000 007a 0941 646a 2043 6c6f 7365  r`...z.Adj Close
+00002d50: 7215 0000 0072 6300 0000 679a 9999 9999  r....rc...g.....
+00002d60: 99b9 3f72 0100 0000 7a08 4f20 6174 6976  ..?r....z.O ativ
+00002d70: 6f20 7a15 2064 6576 6520 7365 7220 616c  o z. deve ser al
+00002d80: 6f63 6164 6f20 656d 2072 5200 0000 7a03  ocado em rR...z.
+00002d90: 2e32 667a 0d25 2064 6120 6361 7274 6569  .2fz.% da cartei
+00002da0: 7261 2903 fa10 5265 746f 726e 6f20 4573  ra)...Retorno Es
+00002db0: 7065 7261 646f fa11 5269 7363 6f20 6461  perado..Risco da
+00002dc0: 2043 6172 7465 6972 61fa 1241 6c6f 6361   Carteira..Aloca
+00002dd0: 6361 6f20 4d61 726b 6f77 6974 7a29 1672  cao Markowitz).r
+00002de0: 2900 0000 7264 0000 0072 6c00 0000 da06  )...rd...rl.....
+00002df0: 6472 6f70 6e61 726d 0000 0072 6500 0000  dropnarm...re...
+00002e00: da05 6172 7261 7972 8100 0000 7230 0000  ..arrayr....r0..
+00002e10: 0072 5700 0000 7268 0000 00da 0364 6f74  .rW...rh.....dot
+00002e20: da01 54da 0574 7261 6365 5a06 6c69 6e61  ..T..traceZ.lina
+00002e30: 6c67 da03 696e 76da 0365 7965 da05 7368  lg..inv..eye..sh
+00002e40: 6170 65da 046f 6e65 73da 0766 6c61 7474  ape..ones..flatt
+00002e50: 656e da05 7261 6e67 65da 0661 7070 656e  en..range..appen
+00002e60: 6429 1172 7700 0000 7287 0000 0072 5f00  d).rw...r....r_.
+00002e70: 0000 7283 0000 005a 0872 6574 6f72 6e6f  ..r....Z.retorno
+00002e80: 735a 126d 6174 7269 7a5f 636f 7661 7269  sZ.matriz_covari
+00002e90: 616e 6369 615a 0570 6573 6f73 da10 7265  anciaZ.pesos..re
+00002ea0: 746f 726e 6f5f 6573 7065 7261 646f da05  torno_esperado..
+00002eb0: 7269 7363 6f5a 076c 616d 6264 615f 5a07  riscoZ.lambda_Z.
+00002ec0: 636f 765f 696e 765a 0976 6574 6f72 5f75  cov_invZ.vetor_u
+00002ed0: 6e73 5a0b 775f 6d61 726b 6f77 6974 7a5a  nsZ.w_markowitzZ
+00002ee0: 0d6d 6172 6b6f 7769 747a 4c69 7374 da01  .markowitzList..
+00002ef0: 695a 0574 6178 6173 7233 0000 0072 1e00  iZ.taxasr3...r..
+00002f00: 0000 721e 0000 0072 1f00 0000 da14 6d61  ..r....r......ma
+00002f10: 726b 6f77 6974 7a5f 616c 6c6f 6361 7469  rkowitz_allocati
+00002f20: 6f6e fb01 0000 7328 0000 0000 1614 030c  on....s(........
+00002f30: 0308 031c 0316 0326 030e 0120 0112 0122  .......&... ..."
+00002f40: 0108 0304 0110 0120 010c 0102 0102 0102  ....... ........
+00002f50: fe06 0672 9a00 0000 7a23 7374 6f63 6b73  ...r....z#stocks
+00002f60: 2f7b 7379 6d62 6f6c 7d2f 4d61 726b 6f77  /{symbol}/Markow
+00002f70: 6974 7a41 6c6c 6f63 6174 696f 6e7a 0a2f  itzAllocationz./
+00002f80: 696e 666f 4675 6e64 7363 0100 0000 0000  infoFundsc......
+00002f90: 0000 0000 0000 0700 0000 0400 0000 4300  ..............C.
+00002fa0: 0000 7372 0000 0064 017d 0174 00a0 017c  ..sr...d.}.t...|
+00002fb0: 01a1 017d 0274 027c 026a 0364 0283 027d  ...}.t.|.j.d...}
+00002fc0: 037c 03a0 0464 03a1 0164 0419 007d 0474  .|...d...d...}.t
+00002fd0: 05a0 0674 077c 0483 01a1 0164 0419 007d  ...t.|.....d...}
+00002fe0: 057c 0564 0519 00a0 0864 0664 0784 00a1  .|.d.....d.d....
+00002ff0: 017c 0564 053c 007c 056a 097c 0564 0519  .|.d.<.|.j.|.d..
+00003000: 007c 006b 0219 007d 067c 0667 0064 08a2  .|.k...}.|.g.d..
+00003010: 0119 007d 067c 0653 0029 0975 ca00 0000  ...}.|.S.).u....
+00003020: 0a20 2020 2023 2320 5573 6162 696c 6964  .    ## Usabilid
+00003030: 6164 650a 2020 2020 2d20 4675 6ec3 a761  ade.    - Fun..a
+00003040: 6f20 7574 696c 697a 6164 6120 7061 7261  o utilizada para
+00003050: 2061 6471 7569 7269 7220 6173 2070 7269   adquirir as pri
+00003060: 6e63 6970 6169 7320 6361 7261 6374 6572  ncipais caracter
+00003070: 6973 7469 6361 7320 6520 696e 666f 726d  isticas e inform
+00003080: 61c3 a7c3 b565 7320 646f 2066 756e 646f  a....es do fundo
+00003090: 2073 656c 6563 696f 6e61 646f 0a0a 2020   selecionado..  
+000030a0: 2020 2323 2050 6172 c3a2 6d65 7472 6f73    ## Par..metros
+000030b0: 0a0a 2020 2020 2d20 7379 6d62 6f6c 202d  ..    - symbol -
+000030c0: 3e20 4e6f 6d65 2064 6f20 4675 6e64 6f20  > Nome do Fundo 
+000030d0: 7061 7261 2066 617a 6572 2061 2062 7573  para fazer a bus
+000030e0: 6361 200a 0a0a 2020 2020 fa28 6874 7470  ca ...    .(http
+000030f0: 733a 2f2f 7777 772e 6675 6e64 7365 7870  s://www.fundsexp
+00003100: 6c6f 7265 722e 636f 6d2e 6272 2f72 616e  lorer.com.br/ran
+00003110: 6b69 6e67 fa0b 6874 6d6c 2e70 6172 7365  king..html.parse
+00003120: 72da 0574 6162 6c65 7201 0000 00f5 1000  r..tabler.......
+00003130: 0000 43c3 b364 6967 6f20 646f 2066 756e  ..C..digo do fun
+00003140: 646f 6301 0000 0000 0000 0000 0000 0001  doc.............
+00003150: 0000 0002 0000 0053 0000 0073 0800 0000  .......S...s....
+00003160: 7c00 6401 1700 5300 a902 4efa 032e 5341  |.d...S...N...SA
+00003170: 721e 0000 00a9 01da 0178 721e 0000 0072  r........xr....r
+00003180: 1e00 0000 721f 0000 00da 083c 6c61 6d62  ....r......<lamb
+00003190: 6461 3e4f 0200 00f3 0000 0000 7a1b 6765  da>O........z.ge
+000031a0: 745f 6675 6e64 732e 3c6c 6f63 616c 733e  t_funds.<locals>
+000031b0: 2e3c 6c61 6d62 6461 3ea9 0672 9e00 0000  .<lambda>..r....
+000031c0: da05 5365 746f 72f5 0c00 0000 5072 65c3  ..Setor.....Pre.
+000031d0: a76f 2041 7475 616c da09 4469 7669 6465  .o Atual..Divide
+000031e0: 6e64 6ff5 1100 0000 5661 7269 61c3 a7c3  ndo.....Varia...
+000031f0: a36f 2050 7265 c3a7 6ff5 1000 0000 5265  .o Pre..o.....Re
+00003200: 6e74 6162 2e20 5065 72c3 ad6f 646f 290a  ntab. Per..odo).
+00003210: da08 7265 7175 6573 7473 da03 6765 7472  ..requests..getr
+00003220: 0900 0000 da07 636f 6e74 656e 74da 0866  ......content..f
+00003230: 696e 645f 616c 6c72 4200 0000 da09 7265  ind_allrB.....re
+00003240: 6164 5f68 746d 6c72 8000 0000 da05 6170  ad_htmlr......ap
+00003250: 706c 79da 036c 6f63 2907 7221 0000 00da  ply..loc).r!....
+00003260: 0375 726c da08 7265 7370 6f6e 7365 da04  .url..response..
+00003270: 736f 7570 729d 0000 00da 0766 756e 6473  soupr......funds
+00003280: 4446 da08 7661 6c75 6573 4649 721e 0000  DF..valuesFIr...
+00003290: 0072 1e00 0000 721f 0000 00da 0967 6574  .r....r......get
+000032a0: 5f66 756e 6473 3d02 0000 7312 0000 0000  _funds=...s.....
+000032b0: 0d04 010a 010c 010e 0112 0116 0212 010c  ................
+000032c0: 0272 b700 0000 7a12 2f63 6f6d 7061 7265  .r....z./compare
+000032d0: 5365 746f 7246 756e 6473 2902 da05 7365  SetorFunds)...se
+000032e0: 746f 7272 2200 0000 6302 0000 0000 0000  torr"...c.......
+000032f0: 0000 0000 000c 0000 0006 0000 0043 0000  .............C..
+00003300: 0073 1e01 0000 6401 7d02 7400 a001 7c02  .s....d.}.t...|.
+00003310: a101 7d03 7402 7c03 6a03 6402 8302 7d04  ..}.t.|.j.d...}.
+00003320: 7c04 a004 6403 a101 6404 1900 7d05 7405  |...d...d...}.t.
+00003330: a006 7407 7c05 8301 a101 6404 1900 7d06  ..t.|.....d...}.
+00003340: 7408 7c06 6405 8302 0100 7c01 6406 1b00  t.|.d.....|.d...
+00003350: 7d01 7c06 6a09 7c06 6405 1900 6406 1b00  }.|.j.|.d...d...
+00003360: 7c01 6b04 1900 7d07 7c07 6700 6407 a201  |.k...}.|.g.d...
+00003370: 1900 7d07 7c07 a00a a100 7d07 7c07 6405  ..}.|.....}.|.d.
+00003380: 1900 a00b a100 7d08 7c00 6408 6b02 72aa  ......}.|.d.k.r.
+00003390: 6409 7d00 7c07 6a09 7c07 640a 1900 7c00  d.}.|.j.|.d...|.
+000033a0: 6b02 1900 6405 1900 a00b a100 7d09 6e42  k...d.......}.nB
+000033b0: 7c00 640b 6b02 72d2 640c 7d00 7c07 6a09  |.d.k.r.d.}.|.j.
+000033c0: 7c07 640a 1900 7c00 6b02 1900 6405 1900  |.d...|.k...d...
+000033d0: a00b a100 7d09 6e1a 7c07 6a09 7c07 640a  ....}.n.|.j.|.d.
+000033e0: 1900 7c00 6b02 1900 6405 1900 a00b a100  ..|.k...d.......
+000033f0: 7d09 7c07 6405 1900 a00c a100 7d0a 7405  }.|.d.......}.t.
+00003400: a00d 7c08 6701 7c09 6701 7c0a 6701 640d  ..|.g.|.g.|.g.d.
+00003410: 9c03 a101 7d0b 7c0b a00e 640e a101 7d0b  ....}.|...d...}.
+00003420: 7c0b 5300 290f 7506 0300 000a 2020 2020  |.S.).u.....    
+00003430: 2323 2055 7361 6269 6c69 6461 6465 0a20  ## Usabilidade. 
+00003440: 2020 200a 2020 2020 2d20 4675 6ec3 a761     .    - Fun..a
+00003450: 6f20 7175 6520 7574 696c 697a 6120 6173  o que utiliza as
+00003460: 206d 6574 7269 6361 7320 6520 6d65 6469   metricas e medi
+00003470: 6173 2064 6f73 2066 756e 646f 2063 6f6d  as dos fundo com
+00003480: 2062 6173 6520 6e6f 2073 6575 2053 6574   base no seu Set
+00003490: 6f72 2070 6172 6120 756d 6120 616e 616c  or para uma anal
+000034a0: 6973 6520 6d61 6973 2072 6573 7472 6974  ise mais restrit
+000034b0: 610a 2020 2020 0a20 2020 2023 2320 5061  a.    .    ## Pa
+000034c0: 72c3 a26d 6574 726f 730a 2020 2020 0a20  r..metros.    . 
+000034d0: 2020 202d 2072 656e 7461 6269 6c69 6461     - rentabilida
+000034e0: 6465 5f6d 696e 202d 3e20 5661 6c6f 7220  de_min -> Valor 
+000034f0: 656d 2025 2070 6172 6120 6275 7363 6172  em % para buscar
+00003500: 2061 2072 656e 7461 6269 6c69 6461 6465   a rentabilidade
+00003510: 206d 696e 696d 6120 646f 2066 756e 646f   minima do fundo
+00003520: 2065 7363 6f6c 6869 646f 0a20 2020 202d   escolhido.    -
+00003530: 2073 6574 6f72 202d 3e20 5365 746f 7265   setor -> Setore
+00003540: 7320 6465 2066 756e 646f 7320 7175 6520  s de fundos que 
+00003550: 706f 6465 7261 6d20 7365 7220 6573 636f  poderam ser esco
+00003560: 6c68 6964 6f73 2c20 7365 6775 6520 6120  lhidos, segue a 
+00003570: 6c69 7374 613a 0a20 2020 200a 2020 2020  lista:.    .    
+00003580: 6060 600a 2020 2020 5469 706f 7353 6574  ```.    TiposSet
+00003590: 6f72 6573 3a0a 2020 2020 2d20 436f 7270  ores:.    - Corp
+000035a0: 6f72 6174 6976 6173 203d 2022 4c61 6a65  orativas = "Laje
+000035b0: 7320 436f 7270 6f72 6174 6976 6173 2220  s Corporativas" 
+000035c0: 0a20 2020 202d 204d 6f62 696c 6961 7269  .    - Mobiliari
+000035d0: 6f73 203d 2022 54c3 ad74 756c 6f73 2065  os = "T..tulos e
+000035e0: 2056 616c 2e20 4d6f 622e 220a 2020 2020   Val. Mob.".    
+000035f0: 2d20 5368 6f70 7069 6e67 7320 3d20 2253  - Shoppings = "S
+00003600: 686f 7070 696e 6773 220a 2020 2020 2d20  hoppings".    - 
+00003610: 48c3 ad62 7269 646f 203d 2027 48c3 ad62  H..brido = 'H..b
+00003620: 7269 646f 270a 2020 2020 2d20 5265 6e64  rido'.    - Rend
+00003630: 6120 3d20 2752 656e 6461 270a 2020 2020  a = 'Renda'.    
+00003640: 2d20 4c6f 67c3 ad73 7469 6361 203d 2027  - Log..stica = '
+00003650: 4c6f 67c3 ad73 7469 6361 270a 2020 2020  Log..stica'.    
+00003660: 2d20 486f 7370 6974 616c 203d 2027 486f  - Hospital = 'Ho
+00003670: 7370 6974 616c 270a 2020 2020 2d20 5265  spital'.    - Re
+00003680: 7369 6465 6e63 6961 6c20 3d20 2752 6573  sidencial = 'Res
+00003690: 6964 656e 6369 616c 270a 2020 2020 2d20  idencial'.    - 
+000036a0: 4f75 7472 6f73 203d 2027 4f75 7472 6f73  Outros = 'Outros
+000036b0: 270a 0a20 2020 2060 6060 0a20 2020 2023  '..    ```.    #
+000036c0: 2320 4578 656d 706c 6f3a 0a20 2020 200a  # Exemplo:.    .
+000036d0: 2020 2020 6060 600a 2020 2020 3e3e 3e20      ```.    >>> 
+000036e0: 6262 2e63 6f6d 7061 7265 5f73 6574 6f72  bb.compare_setor
+000036f0: 5f66 756e 6473 2873 6574 6f72 3d27 436f  _funds(setor='Co
+00003700: 7270 6f72 6174 6976 6173 272c 2072 656e  rporativas', ren
+00003710: 7461 6269 6c69 6461 6465 5f6d 696e 203d  tabilidade_min =
+00003720: 2033 290a 2020 2020 6060 600a 0a20 2020   3).    ```..   
+00003730: 2072 9b00 0000 729c 0000 0072 9d00 0000   r....r....r....
+00003740: 7201 0000 0072 aa00 0000 7252 0000 0072  r....r....rR...r
+00003750: a500 0000 5a0c 436f 7270 6f72 6174 6976  ....Z.Corporativ
+00003760: 6173 7a12 4c61 6a65 7320 436f 7270 6f72  asz.Lajes Corpor
+00003770: 6174 6976 6173 72a6 0000 005a 0b4d 6f62  ativasr....Z.Mob
+00003780: 696c 6961 7269 6f73 7514 0000 0054 c3ad  iliariosu....T..
+00003790: 7475 6c6f 7320 6520 5661 6c2e 204d 6f62  tulos e Val. Mob
+000037a0: 2e29 0375 2a00 0000 5265 6e74 6162 696c  .).u*...Rentabil
+000037b0: 6964 6164 6520 4dc3 a964 6961 2064 6f73  idade M..dia dos
+000037c0: 2046 4949 7320 5365 6c65 6369 6f6e 6164   FIIs Selecionad
+000037d0: 6f73 751f 0000 0052 656e 7461 6269 6c69  osu....Rentabili
+000037e0: 6461 6465 204d c3a9 6469 6120 646f 204d  dade M..dia do M
+000037f0: 6572 6361 646f 7537 0000 0044 6573 7669  ercadou7...Desvi
+00003800: 6f20 5061 6472 c3a3 6f20 6461 7320 5265  o Padr..o das Re
+00003810: 6e74 6162 696c 6964 6164 6573 2064 6f73  ntabilidades dos
+00003820: 2046 4949 7320 5365 6c65 6369 6f6e 6164   FIIs Selecionad
+00003830: 6f73 7a20 4f20 7365 746f 722f 7661 6c6f  osz O setor/valo
+00003840: 7220 6e61 6f20 666f 6920 656e 636f 6e74  r nao foi encont
+00003850: 7261 646f 290f 72ab 0000 0072 ac00 0000  rado).r....r....
+00003860: 7209 0000 0072 ad00 0000 72ae 0000 0072  r....r....r....r
+00003870: 4200 0000 72af 0000 0072 8000 0000 7220  B...r....r....r 
+00003880: 0000 0072 b100 0000 728b 0000 0072 5700  ...r....r....rW.
+00003890: 0000 7273 0000 0072 4300 0000 5a06 6669  ..rs...rC...Z.fi
+000038a0: 6c6c 6e61 290c 72b8 0000 005a 1172 656e  llna).r....Z.ren
+000038b0: 7461 6269 6c69 6461 6465 5f6d 696e 72b2  tabilidade_minr.
+000038c0: 0000 0072 b300 0000 72b4 0000 0072 9d00  ...r....r....r..
+000038d0: 0000 72b5 0000 0072 b600 0000 5a13 7265  ..r....r....Z.re
+000038e0: 6e74 6162 696c 6964 6164 655f 6d65 6469  ntabilidade_medi
+000038f0: 615a 1572 656e 7461 6269 6c69 6461 6465  aZ.rentabilidade
+00003900: 5f6d 6572 6361 646f da0d 6465 7376 696f  _mercado..desvio
+00003910: 5f70 6164 7261 6f5a 0a72 6573 756c 7461  _padraoZ.resulta
+00003920: 646f 7372 1e00 0000 721e 0000 0072 1f00  dosr....r....r..
+00003930: 0000 da13 636f 6d70 6172 655f 7365 746f  ....compare_seto
+00003940: 725f 6675 6e64 735d 0200 0073 3400 0000  r_funds]...s4...
+00003950: 0022 0401 0a01 0c01 0e01 1202 0a01 0801  ."..............
+00003960: 1601 0c01 0801 0c01 0801 0401 1c01 0801  ................
+00003970: 0401 1c02 1a02 0c02 0401 0401 0401 04fd  ................
+00003980: 0806 0a02 72ba 0000 007a 0d2f 636f 6d70  ....r....z./comp
+00003990: 6172 6546 756e 6473 2901 7222 0000 0063  areFunds).r"...c
+000039a0: 0300 0000 0000 0000 0000 0000 1200 0000  ................
+000039b0: 0400 0000 4300 0000 734a 0100 007c 0172  ....C...sJ...|.r
+000039c0: bc7c 0264 016b 0372 bc64 027d 0374 00a0  .|.d.k.r.d.}.t..
+000039d0: 017c 03a1 017d 0474 027c 046a 0364 0383  .|...}.t.|.j.d..
+000039e0: 027d 057c 05a0 0464 04a1 0164 0519 007d  .}.|...d...d...}
+000039f0: 0674 05a0 0674 077c 0683 01a1 0164 0519  .t...t.|.....d..
+00003a00: 007d 077c 0764 0619 00a0 0864 0764 0884  .}.|.d.....d.d..
+00003a10: 00a1 017c 0764 063c 007c 0767 0064 09a2  ...|.d.<.|.g.d..
+00003a20: 0119 007d 077c 076a 0964 0667 0164 0a8d  ...}.|.j.d.g.d..
+00003a30: 017d 077c 076a 0a7c 0764 0619 007c 016b  .}.|.j.|.d...|.k
+00003a40: 0219 007d 087c 076a 0a7c 0764 0619 007c  ...}.|.j.|.d...|
+00003a50: 026b 0219 007d 0974 05a0 0b7c 087c 0967  .k...}.t...|.|.g
+00003a60: 02a1 017d 0a7c 0a6a 0c72 b874 0d64 0b83  ...}.|.j.r.t.d..
+00003a70: 0101 006e 047c 0a53 007c 0064 0175 0072  ...n.|.S.|.d.u.r
+00003a80: ca67 007d 006e 7c64 0c7d 0b64 0d7d 0c7c  .g.}.n|d.}.d.}.|
+00003a90: 0044 005d 3a7d 0d74 0ea0 0f7c 0da1 017d  .D.]:}.t...|...}
+00003aa0: 0e7c 0e6a 1064 0e64 0f8d 017d 0f7c 0f64  .|.j.d.d...}.|.d
+00003ab0: 1019 00a0 11a1 00a0 12a1 007d 107c 107c  ...........}.|.|
+00003ac0: 0b6b 0472 d67c 107d 0b7c 0d7d 0c71 d674  .k.r.|.}.|.}.q.t
+00003ad0: 056a 137c 0c7c 0b64 1114 0064 129c 0274  .j.|.|.d...d...t
+00003ae0: 147c 0083 0167 0164 138d 027d 117c 116a  .|...g.d...}.|.j
+00003af0: 0c90 0172 4274 0d64 1483 0101 006e 047c  ...rBt.d.....n.|
+00003b00: 1153 0064 0153 0029 1575 2403 0000 0a20  .S.d.S.).u$.... 
+00003b10: 2020 2023 2320 5573 6162 696c 6964 6164     ## Usabilidad
+00003b20: 650a 2020 2020 0a20 2020 202d 2046 756e  e.    .    - Fun
+00003b30: c3a7 616f 2071 7565 2072 6561 6c69 7a61  ..ao que realiza
+00003b40: 2061 2063 6f6d 7061 7261 c3a7 616f 2065   a compara..ao e
+00003b50: 6e74 7265 2064 6f69 7320 6675 6e64 6f73  ntre dois fundos
+00003b60: 2c20 7365 6a61 2066 6569 7461 2061 2072  , seja feita a r
+00003b70: 6571 7569 7369 c3a7 616f 2064 6f73 2066  equisi..ao dos f
+00003b80: 756e 646f 7320 7669 6120 6c69 7374 6120  undos via lista 
+00003b90: 6f75 2075 6e69 636f 7320 0a20 2020 202d  ou unicos .    -
+00003ba0: 2052 6571 7569 7369 c3a7 616f 204c 6973   Requisi..ao Lis
+00003bb0: 7461 733a 2052 6574 6f72 6e61 206f 2066  tas: Retorna o f
+00003bc0: 756e 646f 2063 6f6d 206d 6169 6f72 2070  undo com maior p
+00003bd0: 6f72 6365 6e74 6167 656d 2064 6520 7269  orcentagem de ri
+00003be0: 7363 6f20 2861 2076 6172 6961 c3a7 c3a3  sco (a varia....
+00003bf0: 6f20 7065 7263 656e 7475 616c 2064 6f73  o percentual dos
+00003c00: 2070 7265 c3a7 6f73 2064 6f73 2061 7469   pre..os dos ati
+00003c10: 766f 732c 2063 616c 6375 6c6f 2072 6561  vos, calculo rea
+00003c20: 6c69 7a61 646f 2063 6f6d 2062 6173 6520  lizado com base 
+00003c30: 6e6f 2064 6573 7669 6f20 7061 6472 c3a3  no desvio padr..
+00003c40: 6f29 0a20 2020 202d 2052 6571 7569 7369  o).    - Requisi
+00003c50: c3a7 616f 2055 6e69 6361 3a20 5265 746f  ..ao Unica: Reto
+00003c60: 726e 6120 756d 2044 6174 6166 7261 6d65  rna um Dataframe
+00003c70: 2063 6f6d 2061 7320 7072 696e 6369 7061   com as principa
+00003c80: 6973 2069 6e66 6f72 6d61 c3a7 6f65 7320  is informa..oes 
+00003c90: 646f 7320 6675 6e64 6f73 2c20 6166 696d  dos fundos, afim
+00003ca0: 2064 6520 756d 6120 636f 6d70 6172 61c3   de uma compara.
+00003cb0: a761 6f20 656e 7472 6520 7365 7573 2076  .ao entre seus v
+00003cc0: 616c 6f72 6573 200a 0a20 2020 200a 2020  alores ..    .  
+00003cd0: 2020 2323 2050 6172 c3a2 6d65 7472 6f73    ## Par..metros
+00003ce0: 0a20 2020 200a 2020 2020 2d20 6c69 7374  .    .    - list
+00003cf0: 6675 6e64 202d 3e20 4c69 7374 6120 646f  fund -> Lista do
+00003d00: 7320 6675 6e64 6f73 2070 6172 6120 616e  s fundos para an
+00003d10: 616c 6973 6520 6465 2072 6973 636f 0a20  alise de risco. 
+00003d20: 2020 202d 2066 756e 645f 3120 2d3e 2050     - fund_1 -> P
+00003d30: 7269 6d65 6972 6f20 6675 6e64 6f20 7061  rimeiro fundo pa
+00003d40: 7261 2061 6e61 6c69 7365 2075 6e69 6361  ra analise unica
+00003d50: 0a20 2020 202d 2066 756e 645f 3220 2d3e  .    - fund_2 ->
+00003d60: 2053 6567 756e 646f 2066 756e 646f 2070   Segundo fundo p
+00003d70: 6172 6120 616e 616c 6973 6520 756e 6963  ara analise unic
+00003d80: 610a 2020 2020 0a20 2020 2023 2320 4578  a.    .    ## Ex
+00003d90: 656d 706c 6f73 3a0a 2020 2020 0a20 2020  emplos:.    .   
+00003da0: 2060 6060 0a20 2020 203e 3e3e 2062 622e   ```.    >>> bb.
+00003db0: 636f 6d70 6172 655f 6675 6e64 7328 6c69  compare_funds(li
+00003dc0: 7374 6675 6e64 3d20 6c69 7374 2920 0a20  stfund= list) . 
+00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003de0: 2020 206f 750a 2020 2020 3e3e 3e20 6262     ou.    >>> bb
+00003df0: 2e63 6f6d 7061 7265 5f66 756e 6473 2866  .compare_funds(f
+00003e00: 756e 645f 313d 2027 6675 6e64 3127 2c20  und_1= 'fund1', 
+00003e10: 6675 6e64 5f32 3d20 2766 756e 6432 2729  fund_2= 'fund2')
+00003e20: 0a20 2020 2060 6060 0a20 2020 200a 2020  .    ```.    .  
+00003e30: 2020 4e72 9b00 0000 729c 0000 0072 9d00    Nr....r....r..
+00003e40: 0000 7201 0000 0072 9e00 0000 6301 0000  ..r....r....c...
+00003e50: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00003e60: 0053 0000 0073 0800 0000 7c00 6401 1700  .S...s....|.d...
+00003e70: 5300 729f 0000 0072 1e00 0000 72a1 0000  S.r....r....r...
+00003e80: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00003e90: 72a3 0000 00c6 0200 0072 a400 0000 7a1f  r........r....z.
+00003ea0: 636f 6d70 6172 655f 6675 6e64 732e 3c6c  compare_funds.<l
+00003eb0: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e29  ocals>.<lambda>)
+00003ec0: 0872 9e00 0000 72a6 0000 0072 a700 0000  .r....r....r....
+00003ed0: 72a8 0000 0072 a900 0000 72aa 0000 007a  r....r....r....z
+00003ee0: 0e44 6976 6964 656e 6420 5969 656c 647a  .Dividend Yieldz
+00003ef0: 1144 5920 2833 4d29 2041 6375 6d75 6c61  .DY (3M) Acumula
+00003f00: 646f 2901 5a06 7375 6273 6574 753e 0000  do).Z.subsetu>..
+00003f10: 004e 616f 2066 6f72 616d 2061 7072 6573  .Nao foram apres
+00003f20: 656e 7461 646f 2064 6164 6f73 2064 6f73  entado dados dos
+00003f30: 2066 756e 646f 7320 7061 7261 2076 6572   fundos para ver
+00003f40: 6966 6963 61c3 a761 6f20 756e 6963 6172  ifica..ao unicar
+00003f50: 2500 0000 7217 0000 0072 4d00 0000 723b  %...r....rM...r;
+00003f60: 0000 0072 4700 0000 7252 0000 0029 025a  ...rG...rR...).Z
+00003f70: 0446 756e 647a 0c4d 6178 2072 6973 6b20  .Fundz.Max risk 
+00003f80: 2825 2972 7d00 0000 7542 0000 004e 616f  (%)r}...uB...Nao
+00003f90: 2066 6f72 616d 2061 7072 6573 656e 7461   foram apresenta
+00003fa0: 646f 2064 6164 6f73 2064 6f73 2066 756e  do dados dos fun
+00003fb0: 646f 7320 7061 7261 2076 6572 6966 6963  dos para verific
+00003fc0: 61c3 a761 6f20 6dc3 ba6c 7469 706c 6129  a..ao m..ltipla)
+00003fd0: 1572 ab00 0000 72ac 0000 0072 0900 0000  .r....r....r....
+00003fe0: 72ad 0000 0072 ae00 0000 7242 0000 0072  r....r....rB...r
+00003ff0: af00 0000 7280 0000 0072 b000 0000 da0f  ....r....r......
+00004000: 6472 6f70 5f64 7570 6c69 6361 7465 7372  drop_duplicatesr
+00004010: b100 0000 7282 0000 0072 4000 0000 722e  ....r....r@...r.
+00004020: 0000 0072 2900 0000 722a 0000 0072 3f00  ...r)...r*...r?.
+00004030: 0000 726c 0000 0072 7300 0000 7243 0000  ..rl...rs...rC..
+00004040: 0072 8100 0000 2912 5a08 6c69 7374 6675  .r....).Z.listfu
+00004050: 6e64 5a06 6675 6e64 5f31 5a06 6675 6e64  ndZ.fund_1Z.fund
+00004060: 5f32 72b2 0000 0072 b300 0000 72b4 0000  _2r....r....r...
+00004070: 0072 9d00 0000 72b5 0000 005a 0566 756e  .r....r....Z.fun
+00004080: 6431 5a05 6675 6e64 32da 0475 6e69 745a  d1Z.fund2..unitZ
+00004090: 096d 6178 5f72 6973 636f 5a10 7469 636b  .max_riscoZ.tick
+000040a0: 6572 5f6d 6178 5f72 6973 636f 7278 0000  er_max_riscorx..
+000040b0: 005a 0566 756e 646f 721d 0000 0072 b900  .Z.fundor....r..
+000040c0: 0000 5a09 7661 6c75 6572 6973 6b72 1e00  ..Z.valueriskr..
+000040d0: 0000 721e 0000 0072 1f00 0000 da0d 636f  ..r....r......co
+000040e0: 6d70 6172 655f 6675 6e64 73a7 0200 0073  mpare_funds....s
+000040f0: 4400 0000 0019 0c01 0401 0a01 0c01 0e01  D...............
+00004100: 1201 1601 0c01 0e02 1201 1202 0e01 0601  ................
+00004110: 0a02 0402 0801 0602 0401 0401 0801 0a01  ................
+00004120: 0c01 1001 0801 0401 0602 0601 06ff 0401  ................
+00004130: 08ff 0603 0801 0a02 72bd 0000 007a 0b2f  ........r....z./
+00004140: 6265 7374 4173 7365 7473 6301 0000 0000  bestAssetsc.....
+00004150: 0000 0000 0000 0019 0000 0005 0000 0043  ...............C
+00004160: 0000 0073 fa02 0000 6401 7d01 7400 a001  ...s....d.}.t...
+00004170: 7c01 a101 7d02 7c02 6a02 6402 6b03 7224  |...}.|.j.d.k.r$
+00004180: 7403 6403 8301 0100 9002 6ed2 7404 7c02  t.d.......n.t.|.
+00004190: 6a05 6404 8302 7d03 7c03 a006 6405 a101  j.d...}.|...d...
+000041a0: 6406 1900 7d04 7407 6a08 7409 7c04 8301  d...}.t.j.t.|...
+000041b0: 6407 6408 6409 8d03 6406 1900 7d05 7c05  d.d.d...d...}.|.
+000041c0: 640a 1900 a00a 640b 640c 8400 a101 7c05  d.....d.d.....|.
+000041d0: 640a 3c00 7403 640d 8301 0100 740b 6a0c  d.<.t.d.....t.j.
+000041e0: 7c05 640a 1900 a00d a100 640e 640f 8d02  |.d.......d.d...
+000041f0: 6410 1900 7d06 6411 6412 8400 7d07 6413  d...}.d.d...}.d.
+00004200: 6414 8400 7d08 6900 7d09 6900 7d0a 7c06  d...}.i.}.i.}.|.
+00004210: 6a0e 4400 5d24 7d0b 7c06 7c0b 1900 7d0c  j.D.]$}.|.|...}.
+00004220: 7c07 7c0c 8301 7c09 7c0b 3c00 7c08 7c0c  |.|...|.|.<.|.|.
+00004230: 8301 7c0a 7c0b 3c00 71ac 7c00 6415 6b02  ..|.|.<.q.|.d.k.
+00004240: 9001 7288 6700 7d0d 7c06 6a0e 4400 5d26  ..r.g.}.|.j.D.]&
+00004250: 7d0b 7c09 7c0b 1900 6416 6b04 72e6 7c0a  }.|.|...d.k.r.|.
+00004260: 7c0b 1900 6417 6b04 72e6 7c0d a00f 7c0b  |...d.k.r.|...|.
+00004270: a101 0100 71e6 7407 6a10 7c0d 6418 6701  ....q.t.j.|.d.g.
+00004280: 6419 8d02 7d0e 7403 641a 8301 0100 7411  d...}.t.d.....t.
+00004290: 7c0d 7412 7413 641b 8d03 7d0f 7c0f 6701  |.t.t.d...}.|.g.
+000042a0: 7d0f 7407 a010 7c0f a101 7d10 7c10 a014  }.t...|...}.|...
+000042b0: 641c a101 7d10 7c10 641d 1900 a015 a100  d...}.|.d.......
+000042c0: a016 a100 7c10 641d 3c00 7c10 641e 1900  ....|.d.<.|.d...
+000042d0: a015 a100 a016 a100 7c10 641e 3c00 7c10  ........|.d.<.|.
+000042e0: 6a17 9001 7280 6e04 7c10 5300 9001 6e6e  j...r.n.|.S...nn
+000042f0: 7c00 641f 6b02 9002 7242 6700 7d11 7c06  |.d.k...rBg.}.|.
+00004300: 6a0e 4400 5d2c 7d0b 7c09 7c0b 1900 6420  j.D.],}.|.|...d 
+00004310: 6b04 9001 729c 7c0a 7c0b 1900 6421 6b00  k...r.|.|...d!k.
+00004320: 9001 729c 7c11 a00f 7c0b a101 0100 9001  ..r.|...|.......
+00004330: 719c 7407 6a10 7c11 6422 6701 6419 8d02  q.t.j.|.d"g.d...
+00004340: 7d12 7403 641a 8301 0100 7411 7c11 7412  }.t.d.....t.|.t.
+00004350: 7413 641b 8d03 7d13 7c13 6701 7d13 7407  t.d...}.|.g.}.t.
+00004360: a010 7c13 a101 7d14 7c14 a014 641c a101  ..|...}.|...d...
+00004370: 7d14 7c14 641d 1900 a015 a100 a016 a100  }.|.d...........
+00004380: 7c14 641d 3c00 7c14 641e 1900 a015 a100  |.d.<.|.d.......
+00004390: a016 a100 7c14 641e 3c00 7c14 6a17 9002  ....|.d.<.|.j...
+000043a0: 723c 6e04 7c14 5300 6eb4 7c00 6423 6b02  r<n.|.S.n.|.d#k.
+000043b0: 9002 72ee 6700 7d15 7c06 6a0e 4400 5d1e  ..r.g.}.|.j.D.].
+000043c0: 7d0b 7c0a 7c0b 1900 6417 6b00 9002 7256  }.|.|...d.k...rV
+000043d0: 7c15 a00f 7c0b a101 0100 9002 7156 7407  |...|.......qVt.
+000043e0: 6a10 7c15 6424 6701 6419 8d02 7d16 7403  j.|.d$g.d...}.t.
+000043f0: 641a 8301 0100 7411 7c15 7412 7413 641b  d.....t.|.t.t.d.
+00004400: 8d03 7d17 7c17 6701 7d17 7407 a010 7c17  ..}.|.g.}.t...|.
+00004410: a101 7d18 7c18 a014 641c a101 7d18 7c18  ..}.|...d...}.|.
+00004420: 641d 1900 a015 a100 a016 a100 7c18 641d  d...........|.d.
+00004430: 3c00 7c18 641e 1900 a015 a100 a016 a100  <.|.d...........
+00004440: 7c18 641e 3c00 7c18 6a17 9002 72e8 6e04  |.d.<.|.j...r.n.
+00004450: 7c18 5300 6e08 7403 6425 8301 0100 6426  |.S.n.t.d%....d&
+00004460: 5300 2927 750c 0200 000a 2020 2020 2323  S.)'u.....    ##
+00004470: 2055 7361 6269 6c69 6461 6465 0a20 2020   Usabilidade.   
+00004480: 202d 2046 756e c3a7 c3a3 6f20 7175 6520   - Fun....o que 
+00004490: 616e 616c 6973 6120 6f73 2070 7269 6e63  analisa os princ
+000044a0: 6970 6169 7320 6174 6976 6f73 206c 6973  ipais ativos lis
+000044b0: 7461 646f 7320 6e6f 206d 6572 6361 646f  tados no mercado
+000044c0: 2071 7565 2063 6f6d 2062 6173 6520 6e6f   que com base no
+000044d0: 2070 6572 6669 6c20 6573 636f 6c68 6964   perfil escolhid
+000044e0: 6f20 6d6f 7374 7261 2071 7561 6973 2070  o mostra quais p
+000044f0: 6f64 656d 2073 6572 2073 7561 7320 6573  odem ser suas es
+00004500: 636f 6c68 6173 2065 2071 7561 6e74 6f73  colhas e quantos
+00004510: 2070 6f72 6365 6e74 6f20 7365 2064 6576   porcento se dev
+00004520: 6520 7465 7220 6e61 2063 6172 7465 6972  e ter na carteir
+00004530: 610a 2020 2020 0a20 2020 2023 2320 5061  a.    .    ## Pa
+00004540: 72c3 a26d 6574 726f 730a 2020 2020 0a20  r..metros.    . 
+00004550: 2020 202d 2070 6572 6669 6c20 2d3e 2050     - perfil -> P
+00004560: 6572 6669 7320 7175 6520 706f 6465 6d20  erfis que podem 
+00004570: 7365 7220 6573 636f 6c68 6964 6f73 2070  ser escolhidos p
+00004580: 6172 6120 7265 616c 697a 6172 2061 2061  ara realizar a a
+00004590: 6ec3 a16c 6973 652c 2073 6567 7565 2061  n..lise, segue a
+000045a0: 206c 6973 7461 3a20 0a0a 2020 2020 0a20   lista: ..    . 
+000045b0: 2020 2060 6060 0a20 2020 2054 6970 6f50     ```.    TipoP
+000045c0: 6572 6669 733a 0a20 2020 202a 2041 6772  erfis:.    * Agr
+000045d0: 6573 7369 766f 0a20 2020 202a 204d 6f64  essivo.    * Mod
+000045e0: 6572 6164 6f0a 2020 2020 2a20 436f 6e73  erado.    * Cons
+000045f0: 6572 7661 646f 720a 2020 2020 0a20 2020  ervador.    .   
+00004600: 2060 6060 0a20 2020 200a 2020 2020 2323   ```.    .    ##
+00004610: 2045 7865 6d70 6c6f 0a20 2020 200a 2020   Exemplo.    .  
+00004620: 2020 6060 600a 2020 2020 0a20 2020 203e    ```.    .    >
+00004630: 3e3e 2061 6c6f 6361 7469 6f6e 203d 2062  >> alocation = b
+00004640: 6573 745f 6173 7365 7473 2870 6572 6669  est_assets(perfi
+00004650: 6c3d 2741 6772 6573 7369 766f 2729 0a20  l='Agressivo'). 
+00004660: 2020 200a 2020 2020 6060 600a 2020 2020     .    ```.    
+00004670: 0a20 2020 207a 2d68 7474 7073 3a2f 2f77  .    z-https://w
+00004680: 7777 2e64 6164 6f73 6465 6d65 7263 6164  ww.dadosdemercad
+00004690: 6f2e 636f 6d2e 6272 2f62 6f6c 7361 2f61  o.com.br/bolsa/a
+000046a0: 636f 6573 7250 0000 007a 3141 6365 7373  coesrP...z1Acess
+000046b0: 6f20 6e65 6761 646f 2061 2062 6173 652c  o negado a base,
+000046c0: 2074 656e 7465 206e 6f76 616d 656e 7465   tente novamente
+000046d0: 206d 6169 7320 7461 7264 652e 729c 0000   mais tarde.r...
+000046e0: 0072 9d00 0000 7201 0000 00fa 012c 7219  .r....r......,r.
+000046f0: 0000 00a9 02da 0764 6563 696d 616c 5a09  .......decimalZ.
+00004700: 7468 6f75 7361 6e64 73f5 0700 0000 43c3  thousands.....C.
+00004710: b364 6967 6f63 0100 0000 0000 0000 0000  .digoc..........
+00004720: 0000 0100 0000 0200 0000 5300 0000 7308  ..........S...s.
+00004730: 0000 007c 0064 0117 0053 0072 9f00 0000  ...|.d...S.r....
+00004740: 721e 0000 0072 a100 0000 721e 0000 0072  r....r....r....r
+00004750: 1e00 0000 721f 0000 0072 a300 0000 1503  ....r....r......
+00004760: 0000 72a4 0000 007a 1d62 6573 745f 6173  ..r....z.best_as
+00004770: 7365 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c  sets.<locals>.<l
+00004780: 616d 6264 613e 7a13 4275 7363 616e 646f  ambda>z.Buscando
+00004790: 2061 7469 766f 732e 2e2e 2e72 3900 0000   ativos....r9...
+000047a0: 723b 0000 0072 4700 0000 6301 0000 0000  r;...rG...c.....
+000047b0: 0000 0000 0000 0003 0000 0002 0000 0053  ...............S
+000047c0: 0000 0073 1400 0000 7c00 a000 a100 7d01  ...s....|.....}.
+000047d0: 7c01 a001 a100 7d02 7c02 5300 a901 4e29  |.....}.|.S...N)
+000047e0: 0272 6c00 0000 7257 0000 0029 03da 0670  .rl...rW...)...p
+000047f0: 7265 636f 73da 0772 6574 6f72 6e6f 5a0d  recos..retornoZ.
+00004800: 7265 746f 726e 6f5f 6d65 6469 6f72 1e00  retorno_medior..
+00004810: 0000 721e 0000 0072 1f00 0000 da10 6361  ..r....r......ca
+00004820: 6c63 756c 6172 5f72 6574 6f72 6e6f 1a03  lcular_retorno..
+00004830: 0000 7306 0000 0000 0108 0108 017a 2562  ..s..........z%b
+00004840: 6573 745f 6173 7365 7473 2e3c 6c6f 6361  est_assets.<loca
+00004850: 6c73 3e2e 6361 6c63 756c 6172 5f72 6574  ls>.calcular_ret
+00004860: 6f72 6e6f 6301 0000 0000 0000 0000 0000  ornoc...........
+00004870: 0003 0000 0002 0000 0053 0000 0073 1400  .........S...s..
+00004880: 0000 7c00 a000 a100 7d01 7c01 a001 a100  ..|.....}.|.....
+00004890: 7d02 7c02 5300 72c2 0000 0029 0272 6c00  }.|.S.r....).rl.
+000048a0: 0000 7273 0000 0029 0372 c300 0000 72c4  ..rs...).r....r.
+000048b0: 0000 0072 9800 0000 721e 0000 0072 1e00  ...r....r....r..
+000048c0: 0000 721f 0000 00da 0e63 616c 6375 6c61  ..r......calcula
+000048d0: 725f 7269 7363 6f20 0300 0073 0600 0000  r_risco ...s....
+000048e0: 0001 0801 0801 7a23 6265 7374 5f61 7373  ......z#best_ass
+000048f0: 6574 732e 3c6c 6f63 616c 733e 2e63 616c  ets.<locals>.cal
+00004900: 6375 6c61 725f 7269 7363 6f5a 0941 6772  cular_riscoZ.Agr
+00004910: 6573 7369 766f 672d 431c ebe2 361a 3fe7  essivog-C...6.?.
+00004920: 7b14 ae47 e17a 843f 7a12 4174 6976 6f73  {..G.z.?z.Ativos
+00004930: 2050 2f41 6772 6573 7369 766f a901 da07   P/Agressivo....
+00004940: 636f 6c75 6d6e 737a 3f52 6561 6c69 7a61  columnsz?Realiza
+00004950: 6e64 6f20 6361 6c63 756c 6f73 2070 6172  ndo calculos par
+00004960: 6120 6120 7375 6120 6361 7274 6569 7261  a a sua carteira
+00004970: 2063 6f6d 2062 6173 6520 6e6f 2073 6575   com base no seu
+00004980: 2070 6572 6669 6c2e 2902 7287 0000 0072   perfil.).r....r
+00004990: 5f00 0000 728a 0000 0072 8800 0000 7289  _...r....r....r.
+000049a0: 0000 005a 084d 6f64 6572 6164 6f67 6132  ...Z.Moderadoga2
+000049b0: 5530 2aa9 333f 67b8 1e85 eb51 b89e 3f7a  U0*.3?g....Q..?z
+000049c0: 1141 7469 766f 7320 502f 4d6f 6465 7261  .Ativos P/Modera
+000049d0: 646f 5a0b 436f 6e73 6572 7661 646f 727a  doZ.Conservadorz
+000049e0: 1441 7469 766f 7320 502f 436f 6e73 6572  .Ativos P/Conser
+000049f0: 7661 646f 7275 5a00 0000 5065 7266 696c  vadoruZ...Perfil
+00004a00: 206e c3a3 6f20 7265 636f 6e68 6563 6964   n..o reconhecid
+00004a10: 6f2c 206f 7320 7065 7266 6973 2064 6973  o, os perfis dis
+00004a20: 706f 6e69 7665 6973 2065 7374 616f 2070  poniveis estao p
+00004a30: 7265 7365 6e74 6573 206e 6120 6578 706c  resentes na expl
+00004a40: 6963 61c3 a7c3 a36f 2064 6120 6675 6ec3  ica....o da fun.
+00004a50: a7c3 a36f 4e29 1872 ab00 0000 72ac 0000  ...oN).r....r...
+00004a60: 005a 0b73 7461 7475 735f 636f 6465 722e  .Z.status_coder.
+00004a70: 0000 0072 0900 0000 72ad 0000 0072 ae00  ...r....r....r..
+00004a80: 0000 7242 0000 0072 af00 0000 7280 0000  ..rB...r....r...
+00004a90: 0072 b000 0000 7229 0000 0072 6400 0000  .r....r)...rd...
+00004aa0: da06 746f 6c69 7374 72c9 0000 0072 9600  ..tolistr....r..
+00004ab0: 0000 7243 0000 0072 9a00 0000 da04 6f6e  ..rC...r......on
+00004ac0: 6559 da09 6375 7272 656e 746c 795a 0765  eY..currentlyZ.e
+00004ad0: 7870 6c6f 6465 72bb 0000 0072 8b00 0000  xploder....r....
+00004ae0: 7240 0000 0029 195a 0670 6572 6669 6c72  r@...).Z.perfilr
+00004af0: b200 0000 72b3 0000 0072 b400 0000 729d  ....r....r....r.
+00004b00: 0000 0072 b500 0000 72c3 0000 0072 c500  ...r....r....r..
+00004b10: 0000 72c6 0000 0072 c400 0000 7298 0000  ..r....r....r...
+00004b20: 00da 0561 7469 766f 5a0c 7072 6563 6f73  ...ativoZ.precos
+00004b30: 5f61 7469 766f 5a09 6167 7265 7373 6976  _ativoZ.agressiv
+00004b40: 6f5a 0b44 6641 6772 6573 7369 766f 5a13  oZ.DfAgressivoZ.
+00004b50: 616c 6f63 6174 696f 6e5f 4167 7265 7373  alocation_Agress
+00004b60: 6976 655a 1764 6174 6141 6c6f 6361 7469  iveZ.dataAlocati
+00004b70: 6f6e 5f41 6772 6573 7369 7665 5a08 6d6f  on_AgressiveZ.mo
+00004b80: 6465 7261 646f 5a0a 4466 4d6f 6465 7261  deradoZ.DfModera
+00004b90: 646f 5a12 616c 6f63 6174 696f 6e5f 4d6f  doZ.alocation_Mo
+00004ba0: 6465 7261 6465 5a16 6461 7461 416c 6f63  deradeZ.dataAloc
+00004bb0: 6174 696f 6e5f 4d6f 6465 7261 6465 5a0b  ation_ModeradeZ.
+00004bc0: 636f 6e73 6572 7661 646f 725a 0d44 6643  conservadorZ.DfC
+00004bd0: 6f6e 7365 7276 6164 6f72 5a16 616c 6f63  onservadorZ.aloc
+00004be0: 6174 696f 6e5f 436f 6e73 6572 7661 7469  ation_Conservati
+00004bf0: 7665 5a1a 6461 7461 416c 6f63 6174 696f  veZ.dataAlocatio
+00004c00: 6e5f 436f 6e73 6572 7661 7469 7665 721e  n_Conservativer.
+00004c10: 0000 0072 1e00 0000 721f 0000 00da 0b62  ...r....r......b
+00004c20: 6573 745f 6173 7365 7473 ef02 0000 7386  est_assets....s.
+00004c30: 0000 0000 1e04 010a 010a 010c 020c 010e  ................
+00004c40: 0118 0116 0108 011a 0308 0608 0604 0104  ................
+00004c50: 010a 0108 010c 010e 030a 0104 010a 0118  ................
+00004c60: 010c 0210 0108 010e 0106 010a 010a 0414  ................
+00004c70: 0114 0208 0102 0208 020a 0204 010a 011c  ................
+00004c80: 010e 0210 0108 010e 0106 010a 010a 0414  ................
+00004c90: 0114 0208 0102 0206 020a 0204 010a 010e  ................
+00004ca0: 010e 0110 0208 010e 0106 010a 010a 0314  ................
+00004cb0: 0114 0208 0102 0206 0272 ce00 0000 7a11  .........r....z.
+00004cc0: 2f62 6573 7441 7373 6574 7356 616c 7565  /bestAssetsValue
+00004cd0: 7363 0100 0000 0000 0000 0000 0000 1100  sc..............
+00004ce0: 0000 0600 0000 0300 0000 733a 0200 0074  ..........s:...t
+00004cf0: 00a0 01a1 0001 0074 0283 007d 017c 01a0  .......t...}.|..
+00004d00: 0364 01a1 0101 0074 046a 057c 0164 028d  .d.....t.j.|.d..
+00004d10: 017d 0264 037d 037c 02a0 067c 03a1 0101  .}.d.}.|...|....
+00004d20: 0074 07a0 0864 04a1 0101 007c 02a0 0974  .t...d.....|...t
+00004d30: 0a6a 0b64 05a1 02a0 0ca1 007d 047c 026a  .j.d.......}.|.j
+00004d40: 0da0 0e7c 02a0 0974 0a6a 0f64 06a1 02a1  ...|...t.j.d....
+00004d50: 0101 007c 02a0 0974 0a6a 0f64 07a1 02a0  ...|...t.j.d....
+00004d60: 0ca1 007d 057c 02a0 0974 0a6a 1064 08a1  ...}.|...t.j.d..
+00004d70: 02a0 0ca1 007d 067c 02a0 0974 0a6a 1064  .....}.|...t.j.d
+00004d80: 09a1 027d 077c 07a0 1164 0aa1 017d 0874  ...}.|...d...}.t
+00004d90: 126a 1374 147c 0883 0164 0b64 0c64 0d8d  .j.t.|...d.d.d..
+00004da0: 037d 097c 0964 0e19 007d 097c 0964 0f64  .}.|.d...}.|.d.d
+00004db0: 1067 0219 007d 097c 09a0 1564 1164 1267  .g...}.|...d.d.g
+00004dc0: 02a1 017d 097c 0964 0f19 00a0 1664 1364  ...}.|.d.....d.d
+00004dd0: 1484 00a1 017c 0964 0f3c 0074 176a 187c  .....|.d.<.t.j.|
+00004de0: 0964 0f19 00a0 19a1 0064 1564 168d 0264  .d.......d.d...d
+00004df0: 1719 007d 0a7c 0a6a 1a64 1864 198d 017d  ...}.|.j.d.d...}
+00004e00: 0a7c 0aa0 1ba1 00a0 1ca1 0064 1a14 0089  .|.........d....
+00004e10: 007c 0aa0 1ba1 00a0 1da1 0074 1ea0 1f64  .|.........t...d
+00004e20: 1aa1 0114 007d 0b74 12a0 2088 007c 0b64  .....}.t.. ..|.d
+00004e30: 1b9c 02a1 017d 0c7c 0c64 1c19 007c 0c64  .....}.|.d...|.d
+00004e40: 1d19 001b 007c 0c64 1e3c 007c 0c6a 2164  .....|.d.<.|.j!d
+00004e50: 1e64 1f64 208d 02a0 2264 21a1 017d 0c7c  .d.d ..."d!..}.|
+00004e60: 0c64 1e19 007c 0c64 1e19 00a0 23a1 001b  .d...|.d....#...
+00004e70: 007c 0c64 223c 007c 0c64 2219 0088 0114  .|.d"<.|.d".....
+00004e80: 007c 0c64 233c 007c 0ca0 24a1 007d 0c7c  .|.d#<.|..$..}.|
+00004e90: 0c6a 2564 2464 2564 269c 0264 278d 017d  .j%d$d%d&..d'..}
+00004ea0: 0c7c 0c64 2419 0044 005d 427d 0d74 176a  .|.d$..D.]B}.t.j
+00004eb0: 187c 0d64 1564 168d 027d 0e7c 0e64 1719  .|.d.d...}.|.d..
+00004ec0: 006a 2664 2819 007c 0e64 1719 006a 2664  .j&d(..|.d...j&d
+00004ed0: 0e19 0018 007c 0e64 1719 006a 2664 0e19  .....|.d...j&d..
+00004ee0: 001b 0088 007c 0d3c 0090 0171 ba87 0087  .....|.<...q....
+00004ef0: 0166 0264 2964 2a84 087c 0c64 2419 0044  .f.d)d*..|.d$..D
+00004f00: 0083 017d 0f7c 0fa0 27a1 007d 1074 287c  ...}.|..'..}.t(|
+00004f10: 1083 017d 107c 107c 0c64 2b3c 007c 0c67  ...}.|.|.d+<.|.g
+00004f20: 0064 2ca2 0119 0053 0029 2d75 1a02 0000  .d,....S.)-u....
+00004f30: 0a20 2020 2023 2320 5573 6162 696c 6964  .    ## Usabilid
+00004f40: 6164 650a 2020 2020 2d20 4675 6ec3 a7c3  ade.    - Fun...
+00004f50: a36f 2071 7565 2061 6e61 6c69 7361 206f  .o que analisa o
+00004f60: 7320 6174 6976 6f73 2064 6f20 4942 4f56  s ativos do IBOV
+00004f70: 4553 5041 2071 7565 2063 6f6d 2062 6173  ESPA que com bas
+00004f80: 6520 6e6f 2076 616c 6f72 2064 6520 696e  e no valor de in
+00004f90: 7665 7374 696d 656e 746f 2065 7363 6f6c  vestimento escol
+00004fa0: 6869 646f 206d 6f73 7472 6120 7175 6169  hido mostra quai
+00004fb0: 7320 706f 6465 6d20 7365 7220 7375 6173  s podem ser suas
+00004fc0: 2065 7363 6f6c 6861 732c 206f 2071 7561   escolhas, o qua
+00004fd0: 6e74 6f20 6972 6120 7465 7220 7175 6520  nto ira ter que 
+00004fe0: 696e 7665 7374 6972 2070 6172 6120 6361  investir para ca
+00004ff0: 6461 2061 7469 766f 2065 206f 2072 6574  da ativo e o ret
+00005000: 6f72 6e6f 2061 7072 6f78 696d 6164 6f20  orno aproximado 
+00005010: 7061 7261 2063 6164 6120 756d 2064 656c  para cada um del
+00005020: 6573 200a 0a20 2020 202d 2055 7361 6d6f  es ..    - Usamo
+00005030: 7320 636f 6d6f 206d 6574 6f64 6f20 6465  s como metodo de
+00005040: 2063 c3a1 6c63 756c 6f20 6f20 6120 6d65   c..lculo o a me
+00005050: 6469 6461 2053 6861 7270 6520 7175 6520  dida Sharpe que 
+00005060: 6e61 6461 206d 6169 7320 c3a9 2071 7565  nada mais .. que
+00005070: 2075 6d61 2020 6d65 6469 6461 2064 6520   uma  medida de 
+00005080: 6465 7365 6d70 656e 686f 2064 6520 696e  desempenho de in
+00005090: 7665 7374 696d 656e 746f 7320 7175 6520  vestimentos que 
+000050a0: 6c65 7661 2065 6d20 636f 6e73 6964 6572  leva em consider
+000050b0: 61c3 a7c3 a36f 206f 2072 6574 6f72 6e6f  a....o o retorno
+000050c0: 206f 6274 6964 6f20 7065 6c6f 2069 6e76   obtido pelo inv
+000050d0: 6573 7469 6d65 6e74 6f20 656d 2072 656c  estimento em rel
+000050e0: 61c3 a7c3 a36f 2061 6f20 7269 7363 6f20  a....o ao risco 
+000050f0: 6173 7375 6d69 646f 0a20 2020 2023 2320  assumido.    ## 
+00005100: 5061 72c3 a26d 6574 726f 730a 2020 2020  Par..metros.    
+00005110: 0a20 2020 202d 2076 616c 6f72 202d 3e20  .    - valor -> 
+00005120: 5661 6c6f 7220 646f 2069 6e76 6573 7469  Valor do investi
+00005130: 6d65 6e74 6f2c 2070 6f72 2070 6164 72c3  mento, por padr.
+00005140: a36f 2030 0a0a 2020 2020 fa0a 2d2d 6865  .o 0..    ..--he
+00005150: 6164 6c65 7373 a901 da07 6f70 7469 6f6e  adless....option
+00005160: 737a 7c68 7474 7073 3a2f 2f77 7777 2e62  sz|https://www.b
+00005170: 332e 636f 6d2e 6272 2f70 745f 6272 2f6d  3.com.br/pt_br/m
+00005180: 6172 6b65 742d 6461 7461 2d65 2d69 6e64  arket-data-e-ind
+00005190: 6963 6573 2f69 6e64 6963 6573 2f69 6e64  ices/indices/ind
+000051a0: 6963 6573 2d61 6d70 6c6f 732f 696e 6469  ices-amplos/indi
+000051b0: 6365 2d69 626f 7665 7370 612d 6962 6f76  ce-ibovespa-ibov
+000051c0: 6573 7061 2d63 6f6d 706f 7369 6361 6f2d  espa-composicao-
+000051d0: 6461 2d63 6172 7465 6972 612e 6874 6d72  da-carteira.htmr
+000051e0: 7200 0000 7a1b 6f6e 6574 7275 7374 2d61  r...z.onetrust-a
+000051f0: 6363 6570 742d 6274 6e2d 6861 6e64 6c65  ccept-btn-handle
+00005200: 727a 162f 2f2a 5b40 6964 3d22 6276 6d66  rz.//*[@id="bvmf
+00005210: 5f69 6672 616d 6522 5d7a 152f 2f2a 5b40  _iframe"]z.//*[@
+00005220: 6964 3d22 7365 6c65 6374 5061 6765 225d  id="selectPage"]
+00005230: 7a21 2373 656c 6563 7450 6167 6520 3e20  z!#selectPage > 
+00005240: 6f70 7469 6f6e 3a6e 7468 2d63 6869 6c64  option:nth-child
+00005250: 2834 297a 6c23 6469 7643 6f6e 7461 696e  (4)zl#divContain
+00005260: 6572 4966 7261 6d65 4233 203e 2064 6976  erIframeB3 > div
+00005270: 203e 2064 6976 2e63 6f6c 2d6c 672d 392e   > div.col-lg-9.
+00005280: 636f 6c2d 3132 2e6f 7264 6572 2d32 2e6f  col-12.order-2.o
+00005290: 7264 6572 2d6c 672d 3120 3e20 666f 726d  rder-lg-1 > form
+000052a0: 203e 2064 6976 3a6e 7468 2d63 6869 6c64   > div:nth-child
+000052b0: 2834 2920 3e20 6469 7620 3e20 7461 626c  (4) > div > tabl
+000052c0: 65da 096f 7574 6572 4854 4d4c 72be 0000  e..outerHTMLr...
+000052d0: 0072 1900 0000 72bf 0000 0072 0100 0000  .r....r....r....
+000052e0: 72c1 0000 0075 0600 0000 41c3 a7c3 a36f  r....u....A....o
+000052f0: e958 0000 00e9 5900 0000 6301 0000 0000  .X....Y...c.....
+00005300: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
+00005310: 0000 0073 0800 0000 7c00 6401 1700 5300  ...s....|.d...S.
+00005320: 729f 0000 0072 1e00 0000 72a1 0000 0072  r....r....r....r
+00005330: 1e00 0000 721e 0000 0072 1f00 0000 72a3  ....r....r....r.
+00005340: 0000 009d 0300 0072 a400 0000 7a23 6265  .......r....z#be
+00005350: 7374 5f61 7373 6574 735f 7661 6c75 652e  st_assets_value.
+00005360: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+00005370: 3e72 3900 0000 723b 0000 0072 4700 0000  >r9...r;...rG...
+00005380: 7215 0000 0029 015a 0461 7869 7372 6300  r....).Z.axisrc.
+00005390: 0000 2902 7297 0000 0072 9800 0000 7297  ..).r....r....r.
+000053a0: 0000 0072 9800 0000 5a06 7368 6172 7065  ...r....Z.sharpe
+000053b0: 4629 015a 0961 7363 656e 6469 6e67 e906  F).Z.ascending..
+000053c0: 0000 005a 0861 6c6f 6361 6361 6fda 0576  ...Z.alocacao..v
+000053d0: 616c 6f72 da06 4174 6976 6f73 fa13 5174  alor..Ativos..Qt
+000053e0: 6420 4e65 6365 7373 6172 6961 2028 5224  d Necessaria (R$
+000053f0: 2929 0272 7e00 0000 72d6 0000 0072 c800  )).r~...r....r..
+00005400: 0000 7225 0000 0063 0100 0000 0000 0000  ..r%...c........
+00005410: 0000 0000 0200 0000 0500 0000 1300 0000  ................
+00005420: 731a 0000 0069 007c 005d 127d 017c 0188  s....i.|.].}.|..
+00005430: 007c 0119 0088 0114 0093 0271 0453 0072  .|.........q.S.r
+00005440: 1e00 0000 721e 0000 0029 02da 022e 3072  ....r....)....0r
+00005450: cd00 0000 a902 7297 0000 0072 d600 0000  ......r....r....
+00005460: 721e 0000 0072 1f00 0000 da0a 3c64 6963  r....r......<dic
+00005470: 7463 6f6d 703e c003 0000 72a4 0000 007a  tcomp>....r....z
+00005480: 2562 6573 745f 6173 7365 7473 5f76 616c  %best_assets_val
+00005490: 7565 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  ue.<locals>.<dic
+000054a0: 7463 6f6d 703e fa0e 5265 746f 726e 6f20  tcomp>..Retorno 
+000054b0: 4170 726f 782e 2903 72d7 0000 0072 d800  Aprox.).r....r..
+000054c0: 0000 72dc 0000 0029 29da 1a63 6872 6f6d  ..r....))..chrom
+000054d0: 6564 7269 7665 725f 6175 746f 696e 7374  edriver_autoinst
+000054e0: 616c 6c65 72da 0769 6e73 7461 6c6c 7207  aller..installr.
+000054f0: 0000 00da 0c61 6464 5f61 7267 756d 656e  .....add_argumen
+00005500: 7472 0500 0000 da06 4368 726f 6d65 72ac  tr......Chromer.
+00005510: 0000 00da 0474 696d 65da 0573 6c65 6570  .....time..sleep
+00005520: da0c 6669 6e64 5f65 6c65 6d65 6e74 7208  ..find_elementr.
+00005530: 0000 00da 0249 44da 0563 6c69 636b 5a09  .....ID..clickZ.
+00005540: 7377 6974 6368 5f74 6fda 0566 7261 6d65  switch_to..frame
+00005550: 5a05 5850 4154 48da 0c43 5353 5f53 454c  Z.XPATH..CSS_SEL
+00005560: 4543 544f 52da 0d67 6574 5f61 7474 7269  ECTOR..get_attri
+00005570: 6275 7465 7242 0000 0072 af00 0000 7280  buterB...r....r.
+00005580: 0000 0072 3e00 0000 72b0 0000 0072 2900  ...r>...r....r).
+00005590: 0000 7264 0000 0072 ca00 0000 728b 0000  ..rd...r....r...
+000055a0: 0072 6c00 0000 7257 0000 0072 7300 0000  .rl...rW...rs...
+000055b0: 7265 0000 0072 6800 0000 7243 0000 005a  re...rh...rC...Z
+000055c0: 0b73 6f72 745f 7661 6c75 6573 da04 6865  .sort_values..he
+000055d0: 6164 7230 0000 0072 4500 0000 da06 7265  adr0...rE.....re
+000055e0: 6e61 6d65 722f 0000 00da 0676 616c 7565  namer/.....value
+000055f0: 7372 3d00 0000 2911 72d6 0000 00da 0e63  sr=...).r......c
+00005600: 6872 6f6d 655f 6f70 7469 6f6e 73da 0664  hrome_options..d
+00005610: 7269 7665 7272 b200 0000 5a07 636f 6f6b  riverr....Z.cook
+00005620: 6965 73da 0673 656c 6563 74da 0361 6c6c  ies..select..all
+00005630: 729d 0000 00da 0a74 6162 6c65 5f68 746d  r......table_htm
+00005640: 6cda 0661 7469 766f 7372 c300 0000 7298  l..ativosr....r.
+00005650: 0000 005a 0961 7469 766f 735f 6466 72cd  ...Z.ativos_dfr.
+00005660: 0000 0072 8400 0000 5a11 7265 746f 726e  ...r....Z.retorn
+00005670: 6f5f 706f 725f 6174 6976 6f5a 0c4c 6973  o_por_ativoZ.Lis
+00005680: 7461 5265 746f 726e 6f72 1e00 0000 72da  taRetornor....r.
+00005690: 0000 0072 1f00 0000 da11 6265 7374 5f61  ...r......best_a
+000056a0: 7373 6574 735f 7661 6c75 657b 0300 0073  ssets_value{...s
+000056b0: 4a00 0000 000e 0801 0601 0a01 0c02 0401  J...............
+000056c0: 0a01 0a01 1201 1601 1201 1202 0e01 0a01  ................
+000056d0: 1401 0801 0c01 0e02 1603 1a03 0c03 1001  ................
+000056e0: 1603 1003 1403 1403 1803 1001 0802 1202  ................
+000056f0: 0c01 0e01 3203 1801 0801 0802 0803 72f2  ....2.........r.
+00005700: 0000 007a 162f 6f70 7469 6f6e 732f 7b73  ...z./options/{s
+00005710: 796d 626f 6c7d 2f69 6e66 6f29 0254 4629  ymbol}/info).TF)
+00005720: 0472 2100 0000 da04 6361 6c6c da03 7075  .r!.....call..pu
+00005730: 7472 2200 0000 6303 0000 0000 0000 0000  tr"...c.........
+00005740: 0000 000c 0000 0005 0000 0043 0000 0073  ...........C...s
+00005750: 7e01 0000 7c00 a000 6401 a101 7218 7c00  ~...|...d...r.|.
+00005760: a001 6401 6402 a102 7d00 6e08 7402 6403  ..d.d...}.n.t.d.
+00005770: 8301 0100 7403 a004 a100 0100 7405 8300  ....t.......t...
+00005780: 7d03 7c03 a006 6404 a101 0100 7407 6a08  }.|...d.....t.j.
+00005790: 7c03 6405 8d01 7d04 6406 7c00 9b00 9d02  |.d...}.d.|.....
+000057a0: 7d05 7c04 a009 7c05 a101 0100 740a a00b  }.|...|.....t...
+000057b0: 6407 a101 0100 7c04 a00c 740d 6a0e 6408  d.....|...t.j.d.
+000057c0: a102 7d06 7c06 a00f 6409 a101 7d07 7410  ..}.|...d...}.t.
+000057d0: 6a11 7412 7c07 8301 640a 640b 640c 8d03  j.t.|...d.d.d...
+000057e0: 7d08 7c08 640d 1900 7d08 7c08 6700 640e  }.|.d...}.|.g.d.
+000057f0: a201 1900 7d08 7c01 640f 6b02 72c0 7c08  ....}.|.d.k.r.|.
+00005800: 6a13 7c08 6410 1900 6411 6b02 1900 7d09  j.|.d...d.k...}.
+00005810: 7c09 5300 7c02 640f 6b02 72e2 7c08 6a13  |.S.|.d.k.r.|.j.
+00005820: 7c08 6410 1900 6412 6b02 1900 7d0a 6413  |.d...d.k...}.d.
+00005830: 7d0b 7c0a 5300 7c04 a009 7c05 a101 0100  }.|.S.|...|.....
+00005840: 740a a00b 6407 a101 0100 7c04 a00c 740d  t...d.....|...t.
+00005850: 6a0e 6408 a102 7d06 7c06 a00f 6409 a101  j.d...}.|...d...
+00005860: 7d07 7410 6a11 7412 7c07 8301 640a 640b  }.t.j.t.|...d.d.
+00005870: 640c 8d03 7d08 7c08 640d 1900 7d08 7c08  d...}.|.d...}.|.
+00005880: 6700 640e a201 1900 7d08 7c01 640f 6b02  g.d.....}.|.d.k.
+00005890: 9001 7256 7c08 6a13 7c08 6410 1900 6411  ..rV|.j.|.d...d.
+000058a0: 6b02 1900 7d09 7c09 5300 7c02 640f 6b02  k...}.|.S.|.d.k.
+000058b0: 9001 7276 7c08 6a13 7c08 6410 1900 6412  ..rv|.j.|.d...d.
+000058c0: 6b02 1900 7d0a 7c0a 5300 7c08 5300 6414  k...}.|.S.|.S.d.
+000058d0: 5300 2915 75c8 0100 000a 2020 2020 2323  S.).u.....    ##
+000058e0: 2055 7361 6269 6c69 6461 6465 0a0a 2020   Usabilidade..  
+000058f0: 2020 2d20 4675 6ec3 a7c3 a36f 2071 7565    - Fun....o que
+00005900: 2061 7072 6573 656e 7461 2061 7320 7072   apresenta as pr
+00005910: 696e 6369 7061 6973 2069 6e66 6f72 6d61  incipais informa
+00005920: c3a7 c3b5 6573 2064 6173 206f 70c3 a7c3  ....es das op...
+00005930: b565 7320 646f 2061 7469 766f 2073 656c  .es do ativo sel
+00005940: 6563 696f 6e61 646f 2c20 696e 666f 726d  ecionado, inform
+00005950: 61c3 a7c3 b565 7320 636f 6d6f 3a20 5374  a....es como: St
+00005960: 7269 6b65 2c20 5661 722c 2047 7265 6761  rike, Var, Grega
+00005970: 732c 2064 656e 7472 6520 6f75 7472 6173  s, dentre outras
+00005980: 2e0a 0a20 2020 2023 2320 5061 72c3 a26d  ...    ## Par..m
+00005990: 6574 726f 730a 0a20 2020 202d 2073 796d  etros..    - sym
+000059a0: 626f 6c20 2d3e 204e 6f6d 6520 646f 2061  bol -> Nome do a
+000059b0: 7469 766f 2070 6172 6120 6275 7363 6172  tivo para buscar
+000059c0: 2061 7320 6f70 c3a7 c3b5 6573 2072 6566   as op....es ref
+000059d0: 6572 656e 7465 7320 6120 656c 652e 0a20  erentes a ele.. 
+000059e0: 2020 202d 2063 616c 6c20 2d3e 2052 6563     - call -> Rec
+000059f0: 6562 6520 5472 7565 206f 7520 4661 6c73  ebe True ou Fals
+00005a00: 652c 2073 6520 5472 7565 2066 6f72 2073  e, se True for s
+00005a10: 656c 6563 696f 6e61 646f 2061 2066 756e  elecionado a fun
+00005a20: c3a7 c3a3 6f20 6972 6120 6669 6c74 7261  ....o ira filtra
+00005a30: 7220 736f 2061 7320 4341 4c4c 2e0a 2020  r so as CALL..  
+00005a40: 2020 2d20 7075 7420 2d3e 2052 6563 6562    - put -> Receb
+00005a50: 6520 5472 7565 206f 7520 4661 6c73 652c  e True ou False,
+00005a60: 2073 6520 5472 7565 2066 6f72 2073 656c   se True for sel
+00005a70: 6563 696f 6e61 646f 2061 2066 756e c3a7  ecionado a fun..
+00005a80: c3a3 6f20 6972 6120 6669 6c74 7261 7220  ..o ira filtrar 
+00005a90: 736f 2061 7320 5055 542e 0a0a 0a20 2020  so as PUT....   
+00005aa0: 2072 a000 0000 7217 0000 0075 3400 0000   r....r....u4...
+00005ab0: 5072 6f63 7572 616e 646f 2064 6164 6f73  Procurando dados
+00005ac0: 2064 6520 6f70 c3a7 c3b5 6573 2064 6f20   de op....es do 
+00005ad0: 6174 6976 6f20 7365 6c65 6369 6f6e 6164  ativo selecionad
+00005ae0: 6f2e 2e2e 72cf 0000 0072 d000 0000 7a25  o...r....r....z%
+00005af0: 6874 7470 733a 2f2f 6f70 636f 6573 2e6e  https://opcoes.n
+00005b00: 6574 2e62 722f 6f70 636f 6573 2f62 6f76  et.br/opcoes/bov
+00005b10: 6573 7061 2f67 0000 0000 0000 f83f 7a0c  espa/g.......?z.
+00005b20: 2374 626c 4c69 7374 614f 7063 72d2 0000  #tblListaOpcr...
+00005b30: 0072 be00 0000 7219 0000 0072 bf00 0000  .r....r....r....
+00005b40: 7201 0000 0029 0d72 2a00 0000 da04 5469  r....).r*.....Ti
+00005b50: 706f 5a06 5374 7269 6b65 7a07 412f 492f  poZ.Strikez.A/I/
+00005b60: 4f54 4d7a 1344 6973 742e 2028 2529 2064  OTMz.Dist. (%) d
+00005b70: 6f20 5374 7269 6b65 7507 0000 00c3 9a6c  o Strikeu......l
+00005b80: 7469 6d6f 7a08 5661 722e 2028 2529 750d  timoz.Var. (%)u.
+00005b90: 0000 004e c3ba 6d2e 2064 6520 4e65 672e  ...N..m. de Neg.
+00005ba0: 7a0f 566f 6c2e 2046 696e 616e 6365 6972  z.Vol. Financeir
+00005bb0: 6fda 0544 656c 7461 da05 4761 6d6d 617a  o..Delta..Gammaz
+00005bc0: 0954 6865 7461 2028 2429 5a04 5665 6761  .Theta ($)Z.Vega
+00005bd0: 5472 f500 0000 da04 4341 4c4c da03 5055  Tr......CALL..PU
+00005be0: 5472 1500 0000 4e29 14da 0865 6e64 7377  Tr....N)...endsw
+00005bf0: 6974 6872 1a00 0000 722e 0000 0072 dd00  ithr....r....r..
+00005c00: 0000 72de 0000 0072 0700 0000 72df 0000  ..r....r....r...
+00005c10: 0072 0500 0000 72e0 0000 0072 ac00 0000  .r....r....r....
+00005c20: 72e1 0000 0072 e200 0000 72e3 0000 0072  r....r....r....r
+00005c30: 0800 0000 72e7 0000 0072 e800 0000 7242  ....r....r....rB
+00005c40: 0000 0072 af00 0000 7280 0000 0072 b100  ...r....r....r..
+00005c50: 0000 290c 7221 0000 0072 f300 0000 72f4  ..).r!...r....r.
+00005c60: 0000 0072 ec00 0000 72ed 0000 0072 b200  ...r....r....r..
+00005c70: 0000 729d 0000 0072 f000 0000 5a05 6466  ..r....r....Z.df
+00005c80: 4f50 435a 0664 6643 616c 6c5a 0564 6650  OPCZ.dfCallZ.dfP
+00005c90: 7574 5a04 6c61 6c61 721e 0000 0072 1e00  utZ.lalar....r..
+00005ca0: 0000 721f 0000 00da 0767 6574 5f6f 7063  ..r......get_opc
+00005cb0: d103 0000 7348 0000 0000 120a 010e 0208  ....sH..........
+00005cc0: 0208 0106 010a 010c 020a 010a 010a 010e  ................
+00005cd0: 010a 0114 0108 010c 0108 0112 0104 0108  ................
+00005ce0: 0112 0104 0104 020a 010a 020e 010a 0114  ................
+00005cf0: 0108 040c 010a 0112 0104 010a 0112 0104  ................
+00005d00: 0272 fb00 0000 7a15 2f6f 7074 696f 6e73  .r....z./options
+00005d10: 2f62 6c61 636b 5363 686f 6c65 7329 0272  /blackScholes).r
+00005d20: f300 0000 72f4 0000 0063 0500 0000 0000  ....r....c......
+00005d30: 0000 0000 0000 0c00 0000 0600 0000 4300  ..............C.
+00005d40: 0000 73e8 0000 0074 007c 0174 0174 0283  ..s....t.|.t.t..
+00005d50: 037d 057c 0564 0114 007d 0664 027d 0774  .}.|.d...}.d.}.t
+00005d60: 03a0 047c 027c 031b 00a1 017c 077c 0664  ...|.|.....|.|.d
+00005d70: 0313 0064 031b 007c 0414 0017 007c 0674  ...d...|.....|.t
+00005d80: 03a0 057c 04a1 0114 0014 0017 007d 087c  ...|.........}.|
+00005d90: 0674 03a0 057c 04a1 0114 0004 007d 097d  .t...|.......}.}
+00005da0: 087c 0064 046b 0272 9a74 0664 0583 0101  .|.d.k.r.t.d....
+00005db0: 007c 0274 07a0 087c 08a1 0114 007c 0374  .|.t...|.....|.t
+00005dc0: 03a0 097c 070b 007c 0414 00a1 0114 0074  ...|...|.......t
+00005dd0: 07a0 087c 09a1 0114 0018 007d 0a7c 0a53  ...|.......}.|.S
+00005de0: 007c 0064 066b 0272 dc74 0664 0783 0101  .|.d.k.r.t.d....
+00005df0: 007c 0374 03a0 097c 070b 007c 0414 00a1  .|.t...|...|....
+00005e00: 0114 0074 07a0 087c 09a1 0114 007c 0274  ...t...|.....|.t
+00005e10: 07a0 087c 080b 00a1 0114 0018 007d 0b7c  ...|.........}.|
+00005e20: 0b53 0074 0664 0883 0101 0064 0953 0029  .S.t.d.....d.S.)
+00005e30: 0a75 4a03 0000 0a20 2020 2023 2320 5573  .uJ....    ## Us
+00005e40: 6162 696c 6964 6164 650a 0a20 2020 202d  abilidade..    -
+00005e50: 2046 756e c3a7 c3a3 6f20 7175 6520 7369   Fun....o que si
+00005e60: 6d75 6c61 206f 2063 6163 756c 6f20 646f  mula o caculo do
+00005e70: 2062 6c61 636b 2d73 6368 6f6c 6573 2c20   black-scholes, 
+00005e80: 6d6f 6465 6c6f 206e 6f20 7175 616c 20c3  modelo no qual .
+00005e90: a920 7574 696c 697a 6164 6f20 7061 7261  . utilizado para
+00005ea0: 2070 7265 6369 6669 6361 7220 6f70 c3a7   precificar op..
+00005eb0: c3b5 6573 206e 6f20 6d65 7263 6164 6f20  ..es no mercado 
+00005ec0: 6465 2064 6572 6976 6174 6976 6f73 2e0a  de derivativos..
+00005ed0: 2020 2020 2d20 506f 7220 7365 2074 7261      - Por se tra
+00005ee0: 7461 7220 6465 2075 6d61 2066 756e c3a7  tar de uma fun..
+00005ef0: c3a3 6f20 656d 2064 6573 656e 766f 6c76  ..o em desenvolv
+00005f00: 696d 656e 746f 206e c3a3 6f20 6c65 7661  imento n..o leva
+00005f10: 7220 6f20 7265 7375 6c74 6164 6f20 636f  r o resultado co
+00005f20: 6d6f 2076 6572 6461 6465 2061 6273 6f6c  mo verdade absol
+00005f30: 7574 612c 206d 6173 2075 6d20 7661 6c6f  uta, mas um valo
+00005f40: 7220 6120 7365 2062 6173 6561 722e 0a0a  r a se basear...
+00005f50: 2020 2020 2323 2050 6172 c3a2 6d65 7472      ## Par..metr
+00005f60: 6f73 0a0a 2020 2020 2d20 4361 6c6c 5f6f  os..    - Call_o
+00005f70: 725f 5075 7420 2d3e 2052 6563 6562 6520  r_Put -> Recebe 
+00005f80: 6f73 2076 616c 6f72 6573 2022 6361 6c6c  os valores "call
+00005f90: 2220 6520 2270 7574 222c 2070 6f72 2073  " e "put", por s
+00005fa0: 6572 656d 2063 616c 6375 6c6f 7320 6469  erem calculos di
+00005fb0: 6665 7265 6e74 6573 2070 6172 6164 6120  ferentes parada 
+00005fc0: 6361 6461 2074 6970 6f2c 20c3 a920 6e65  cada tipo, .. ne
+00005fd0: 6365 7373 6172 696f 2061 2073 656c 65c3  cessario a sele.
+00005fe0: a7c3 a36f 0a20 2020 202d 2061 7469 766f  ...o.    - ativo
+00005ff0: 202d 3e20 496e 7365 7269 7220 6f20 6174   -> Inserir o at
+00006000: 6976 6f20 636f 7272 6573 706f 6e64 656e  ivo corresponden
+00006010: 7465 2064 6120 6675 6ec3 a7c3 a36f 2028  te da fun....o (
+00006020: 4578 656d 706c 6f3a 2027 5045 5452 342e  Exemplo: 'PETR4.
+00006030: 5341 2729 0a20 2020 202d 2070 7265 636f  SA').    - preco
+00006040: 202d 3e20 696e 7365 7269 7220 6f20 7072   -> inserir o pr
+00006050: 65c3 a76f 2064 6f20 6174 6976 6f20 7365  e..o do ativo se
+00006060: 6c65 6369 6f6e 6164 6f0a 2020 2020 2d20  lecionado.    - 
+00006070: 7374 7269 6b65 202d 3e20 496e 7365 7269  strike -> Inseri
+00006080: 7220 6f20 7374 7269 6b65 2064 6120 6f70  r o strike da op
+00006090: c3a7 c3a3 6f0a 2020 2020 2d20 6469 6173  ....o.    - dias
+000060a0: 5574 6569 7320 2d3e 2041 6469 6369 6f6e  Uteis -> Adicion
+000060b0: 6172 2061 2071 7561 6e74 6964 6164 6520  ar a quantidade 
+000060c0: 6465 2064 6961 7320 c3ba 7465 6973 2061  de dias ..teis a
+000060d0: 7465 206f 2076 656e 6369 6d65 6e74 6f20  te o vencimento 
+000060e0: 6461 206f 70c3 a7c3 a36f 2e0a 0a20 2020  da op....o...   
+000060f0: 2023 2320 4578 656d 706c 6f0a 0a20 2020   ## Exemplo..   
+00006100: 2060 6060 0a20 2020 203e 3e3e 2062 622e   ```.    >>> bb.
+00006110: 626c 6163 6b5f 7363 686f 6c65 7328 4361  black_scholes(Ca
+00006120: 6c6c 5f6f 725f 5075 743d 2027 6361 6c6c  ll_or_Put= 'call
+00006130: 272c 2061 7469 766f 3d20 2750 4554 5234  ', ativo= 'PETR4
+00006140: 2e53 4127 2c20 7072 6563 6f3d 2032 362e  .SA', preco= 26.
+00006150: 3235 2c20 7374 7269 6b65 3d20 3236 2e32  25, strike= 26.2
+00006160: 352c 2064 6961 7355 7465 6973 3d20 3232  5, diasUteis= 22
+00006170: 2029 0a20 2020 2060 6060 0a0a 2020 2020   ).    ```..    
+00006180: 6910 f800 0067 c1a8 a44e 40d3 1540 7272  i....g...N@..@rr
+00006190: 0000 0072 f300 0000 7a10 5365 6c65 6369  ...r....z.Seleci
+000061a0: 6f6e 6164 6f20 4361 6c6c 72f4 0000 007a  onado Callr....z
+000061b0: 0f53 656c 6563 696f 6e61 646f 2050 7574  .Selecionado Put
+000061c0: 7530 0000 0041 7320 6f70 c3a7 c3b5 6573  u0...As op....es
+000061d0: 2076 616c 6964 6173 2073 616f 2073 6f6d   validas sao som
+000061e0: 656e 7465 2061 7320 6465 2043 414c 4c20  ente as de CALL 
+000061f0: 6520 5055 544e 290a 726a 0000 00da 0673  e PUTN).rj.....s
+00006200: 6576 656e 4472 cc00 0000 7265 0000 0072  evenDr....re...r
+00006210: 6600 0000 7268 0000 0072 2e00 0000 7202  f...rh...r....r.
+00006220: 0000 005a 0363 6466 da03 6578 7029 0c5a  ...Z.cdf..exp).Z
+00006230: 0b43 616c 6c5f 6f72 5f50 7574 72cd 0000  .Call_or_Putr...
+00006240: 00da 0570 7265 636f da06 7374 7269 6b65  ...preco..strike
+00006250: 5a09 6469 6173 5574 6569 735a 0d76 6f6c  Z.diasUteisZ.vol
+00006260: 6174 696c 6964 6164 6544 5a0c 766f 6c61  atilidadeDZ.vola
+00006270: 7469 6c69 6461 6465 5a06 7461 7861 4c52  tilidadeZ.taxaLR
+00006280: da02 6431 da02 6432 da01 43da 0150 721e  ..d1..d2..C..Pr.
+00006290: 0000 0072 1e00 0000 721f 0000 00da 0d62  ...r....r......b
+000062a0: 6c61 636b 5f73 6368 6f6c 6573 1604 0000  lack_scholes....
+000062b0: 731c 0000 0000 190c 0108 0104 0230 0112  s............0..
+000062c0: 0208 0108 012c 0104 0108 0108 012e 0104  .....,..........
+000062d0: 0272 0401 0000 e771 3d0a d7a3 70cd 3f29  .r.....q=...p.?)
+000062e0: 0272 f100 0000 da0c 696e 7665 7374 696d  .r......investim
+000062f0: 656e 746f 6303 0000 0000 0000 0000 0000  entoc...........
+00006300: 000a 0000 0007 0000 0043 0000 0073 1e01  .........C...s..
+00006310: 0000 7400 6a01 6700 6401 a201 6402 8d01  ..t.j.g.d...d...
+00006320: 7d03 7402 7c00 7403 8302 7296 7404 a005  }.t.|.t...r.t...
+00006330: 7c00 a101 7d04 7c04 6a06 6403 6404 8d01  |...}.|.j.d.d...
+00006340: 6405 1900 6406 1900 7d05 7c04 6a07 a008  d...d...}.|.j...
+00006350: a100 7d06 7c05 7c06 1700 7c05 1b00 6407  ..}.|.|...|...d.
+00006360: 1800 7c01 1400 7d07 7409 a00a 7c07 7c01  ..|...}.t...|.|.
+00006370: 1b00 6407 1700 a101 7409 a00a 6407 6408  ..d.....t...d.d.
+00006380: 7c02 1400 1700 a101 1b00 6409 1b00 7d08  |.........d...}.
+00006390: 7c03 6a0b 7c00 7c07 7c08 6401 9c03 640a  |.j.|.|.|.d...d.
+000063a0: 640b 8d02 7d03 6e84 7c00 4400 5d7e 7d09  d...}.n.|.D.]~}.
+000063b0: 7404 a005 7c09 a101 7d04 7c04 6a06 6403  t...|...}.|.j.d.
+000063c0: 6404 8d01 6405 1900 6406 1900 7d05 7c04  d...d...d...}.|.
+000063d0: 6a07 a008 a100 7d06 7c05 7c06 1700 7c05  j.....}.|.|...|.
+000063e0: 1b00 6407 1800 7c01 1400 7d07 7409 a00a  ..d...|...}.t...
+000063f0: 7c07 7c01 1b00 6407 1700 a101 7409 a00a  |.|...d.....t...
+00006400: 6407 6408 7c02 1400 1700 a101 1b00 6409  d.d.|.........d.
+00006410: 1b00 7d08 7c03 6a0b 7c09 7c07 7c08 6401  ..}.|.j.|.|.|.d.
+00006420: 9c03 640a 640b 8d02 7d03 719a 7c03 5300  ..d.d...}.q.|.S.
+00006430: 290c 4e29 0372 7900 0000 7a16 5265 746f  ).N).ry...z.Reto
+00006440: 726e 6f20 636f 6d20 4469 7669 6465 6e64  rno com Dividend
+00006450: 6f73 7a1a 5465 6d70 6f20 7061 7261 2041  osz.Tempo para A
+00006460: 7469 6e67 6972 2052 6574 6f72 6e6f 72c8  tingir Retornor.
+00006470: 0000 0072 3900 0000 723b 0000 0072 4700  ...r9...r;...rG.
+00006480: 0000 7201 0000 0072 1500 0000 72c7 0000  ..r....r....r...
+00006490: 00e9 0c00 0000 5429 015a 0c69 676e 6f72  ......T).Z.ignor
+000064a0: 655f 696e 6465 7829 0c72 4200 0000 7243  e_index).rB...rC
+000064b0: 0000 0072 7f00 0000 7280 0000 0072 2900  ...r....r....r).
+000064c0: 0000 722a 0000 0072 3f00 0000 7228 0000  ..r*...r?...r(..
+000064d0: 0072 3000 0000 7265 0000 0072 6600 0000  .r0...re...rf...
+000064e0: 7296 0000 0029 0a72 f100 0000 7206 0100  r....).r....r...
+000064f0: 005a 0d74 6178 615f 6465 7363 6f6e 746f  .Z.taxa_desconto
+00006500: 7284 0000 0072 7800 0000 72fe 0000 005a  r....rx...r....Z
+00006510: 0a64 6976 6964 656e 646f 7372 c400 0000  .dividendosr....
+00006520: 5a05 7465 6d70 6f72 cd00 0000 721e 0000  Z.tempor....r...
+00006530: 0072 1e00 0000 721f 0000 00da 1372 6574  .r....r......ret
+00006540: 6f72 6e6f 735f 6469 7669 6465 6e64 6f73  ornos_dividendos
+00006550: 4e04 0000 7320 0000 0000 0110 020a 010a  N...s ..........
+00006560: 0114 010a 0114 0128 0118 0208 010a 0114  .......(........
+00006570: 010a 0114 0128 0118 0272 0801 0000 2901  .....(...r....).
+00006580: 7239 0000 0029 0172 0100 0000 2901 7205  r9...).r....).r.
+00006590: 0100 0029 535a 0879 6669 6e61 6e63 6572  ...)SZ.yfinancer
+000065a0: 2900 0000 5a0b 7363 6970 792e 7374 6174  )...Z.scipy.stat
+000065b0: 7372 0200 0000 5a0e 7363 6970 792e 6f70  sr....Z.scipy.op
+000065c0: 7469 6d69 7a65 7203 0000 005a 1473 6b6c  timizer....Z.skl
+000065d0: 6561 726e 2e6c 696e 6561 725f 6d6f 6465  earn.linear_mode
+000065e0: 6c72 0400 0000 5a08 7365 6c65 6e69 756d  lr....Z.selenium
+000065f0: 7205 0000 005a 1e73 656c 656e 6975 6d2e  r....Z.selenium.
+00006600: 7765 6264 7269 7665 722e 636f 6d6d 6f6e  webdriver.common
+00006610: 2e6b 6579 7372 0600 0000 5a21 7365 6c65  .keysr....Z!sele
+00006620: 6e69 756d 2e77 6562 6472 6976 6572 2e63  nium.webdriver.c
+00006630: 6872 6f6d 652e 6f70 7469 6f6e 7372 0700  hrome.optionsr..
+00006640: 0000 5a1c 7365 6c65 6e69 756d 2e77 6562  ..Z.selenium.web
+00006650: 6472 6976 6572 2e63 6f6d 6d6f 6e2e 6279  driver.common.by
+00006660: 7208 0000 0072 dd00 0000 72ab 0000 005a  r....r....r....Z
+00006670: 0362 7334 7209 0000 0072 e100 0000 5a07  .bs4r....r....Z.
+00006680: 6661 7374 6170 6972 0a00 0000 720b 0000  fastapir....r...
+00006690: 0072 0c00 0000 5a11 6661 7374 6170 692e  .r....Z.fastapi.
+000066a0: 7265 7370 6f6e 7365 7372 0d00 0000 5a13  responsesr....Z.
+000066b0: 6661 7374 6170 692e 7374 6174 6963 6669  fastapi.staticfi
+000066c0: 6c65 7372 0e00 0000 5a12 6661 7374 6170  lesr....Z.fastap
+000066d0: 692e 7465 6d70 6c61 7469 6e67 720f 0000  i.templatingr...
+000066e0: 00da 046a 736f 6e5a 0775 7669 636f 726e  ...jsonZ.uvicorn
+000066f0: da06 7061 6e64 6173 7242 0000 00da 056e  ..pandasrB.....n
+00006700: 756d 7079 7265 0000 0072 1000 0000 7211  umpyre...r....r.
+00006710: 0000 00da 0674 7970 696e 6772 1200 0000  .....typingr....
+00006720: da08 7761 726e 696e 6773 da0e 6669 6c74  ..warnings..filt
+00006730: 6572 7761 726e 696e 6773 5a0c 7064 725f  erwarningsZ.pdr_
+00006740: 6f76 6572 7269 6465 da05 746f 6461 795a  override..todayZ
+00006750: 0c6f 6e65 5f79 6561 725f 6167 6f5a 0c6f  .one_year_agoZ.o
+00006760: 6e65 5f64 6179 735f 6167 6f5a 0e73 6576  ne_days_agoZ.sev
+00006770: 656e 5f64 6179 735f 6167 6fda 0873 7472  en_days_ago..str
+00006780: 6674 696d 6572 cb00 0000 5a04 6f6e 6544  ftimer....Z.oneD
+00006790: 72fc 0000 0072 cc00 0000 da03 6170 7072  r....r......appr
+000067a0: 2000 0000 72ac 0000 0072 8000 0000 722d   ...r....r....r-
+000067b0: 0000 0072 3400 0000 da08 5f5f 6e61 6d65  ...r4.....__name
+000067c0: 5f5f da03 7275 6e72 b300 0000 7243 0000  __..runr....rC..
+000067d0: 0072 4600 0000 5a0f 7265 7370 6f6e 7365  .rF...Z.response
+000067e0: 4869 7374 6f72 7972 4c00 0000 725d 0000  HistoryrL...r]..
+000067f0: 0072 6a00 0000 726e 0000 0072 1c00 0000  .rj...rn...r....
+00006800: da03 696e 7472 7600 0000 723d 0000 0072  ..intrv...r=...r
+00006810: 8600 0000 729a 0000 0072 b700 0000 72ba  ....r....r....r.
+00006820: 0000 0072 bd00 0000 72ce 0000 0072 f200  ...r....r....r..
+00006830: 0000 72fb 0000 0072 0401 0000 7208 0100  ..r....r....r...
+00006840: 0072 1e00 0000 721e 0000 0072 1e00 0000  .r....r....r....
+00006850: 721f 0000 00da 083c 6d6f 6475 6c65 3e02  r......<module>.
+00006860: 0000 0073 e800 0000 0801 0c01 0c01 0c03  ...s............
+00006870: 0c01 0c01 0c01 0c01 0801 0801 0c01 0803  ................
+00006880: 1401 0c01 0c01 0c01 0801 0803 0801 0801  ................
+00006890: 1001 0c02 0801 0a02 0802 0802 0e01 0e01  ................
+000068a0: 0e03 0a01 0a01 0a02 0a02 060c 0809 0c01  ................
+000068b0: 1226 0a01 1201 0a05 0c01 1826 0a01 1201  .&.........&....
+000068c0: 0a05 0c01 1220 0a01 1201 0a05 0c01 123a  ..... .........:
+000068d0: 0a01 1201 0a05 0c01 1618 0a01 1201 0a05  ................
+000068e0: 0c01 1232 0a01 1201 0a05 0c01 1623 0a01  ...2.........#..
+000068f0: 1201 0a05 0c01 2062 0a01 1201 0a05 0801  ...... b........
+00006900: 163a 0a01 1201 0a05 0c01 1418 0a01 1201  .:..............
+00006910: 0a05 0c01 1642 0a01 1201 0a05 0c01 1a40  .....B.........@
+00006920: 0a01 1201 0a05 0c01 167f 0007 0a01 1201  ................
+00006930: 0a03 0c01 1e4d 0a01 1201 0a06 0c01 223f  .....M........"?
+00006940: 0a01 1201 0a03 0c01 202a 0a01 1201 0a0b  ........ *......
```

### Comparing `BBFinance-1.4.9/BBFinance.egg-info/PKG-INFO` & `BBFinance-1.5.0/BBFinance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.4.9
+Version: 1.5.0
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.4.9/BBFinance.egg-info/SOURCES.txt` & `BBFinance-1.5.0/BBFinance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/LICENSE.txt` & `BBFinance-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/PKG-INFO` & `BBFinance-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BBFinance
-Version: 1.4.9
+Version: 1.5.0
 Summary: Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado
 Home-page: https://github.com/beb0pp/BBFinance
 Author: Luis Abreu
 Author-email: luss.fel@gmail.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BBFinance-1.4.9/README.md` & `BBFinance-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/__pycache__/main.cpython-39.pyc` & `BBFinance-1.5.0/__pycache__/main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/bases.db` & `BBFinance-1.5.0/bases.db`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/requirements.txt` & `BBFinance-1.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `BBFinance-1.4.9/setup.py` & `BBFinance-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='BBFinance',
-    version='1.4.9',
+    version='1.5.0',
     description='Uma biblioteca com o objetivo de adquirir informações de ações do mercado financeiro de maneira rapida e prática, afim de incluir todos no mercado',
     url='https://github.com/beb0pp/BBFinance',
     author='Luis Abreu',
     author_email='luss.fel@gmail.com',
     license='GPLv3',
     packages=['BBFinance'],
     long_description= long_description,
```

