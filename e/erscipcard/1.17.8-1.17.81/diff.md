# Comparing `tmp/erscipcard-1.17.8.tar.gz` & `tmp/erscipcard-1.17.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erscipcard-1.17.8.tar", last modified: Mon Apr 17 12:06:21 2023, max compression
+gzip compressed data, was "erscipcard-1.17.81.tar", last modified: Tue Apr 18 07:07:59 2023, max compression
```

## Comparing `erscipcard-1.17.8.tar` & `erscipcard-1.17.81.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.926026 erscipcard-1.17.8/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 12:06:04.000000 erscipcard-1.17.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-17 12:06:04.000000 erscipcard-1.17.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1461 2023-04-17 12:06:21.926026 erscipcard-1.17.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1150 2023-04-17 12:06:04.000000 erscipcard-1.17.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.916025 erscipcard-1.17.8/erscipcard/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/__init__.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/admin.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/apps.py
--rw-r--r--   0 root         (0) root         (0)      313 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.917025 erscipcard-1.17.8/erscipcard/migrations/
--rw-r--r--   0 root         (0) root         (0)     1675 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/migrations/0001_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.918025 erscipcard-1.17.8/erscipcard/static/
--rw-r--r--   0 root         (0) root         (0)    19616 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/1.docx
--rw-r--r--   0 root         (0) root         (0)    14825 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/2.docx
--rw-r--r--   0 root         (0) root         (0)    60820 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/BTITR.TTF
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.912025 erscipcard-1.17.8/erscipcard/static/bt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.920025 erscipcard-1.17.8/erscipcard/static/bt/css/
--rw-r--r--   0 root         (0) root         (0)   175814 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/css/bootstrap.min.css
--rw-r--r--   0 root         (0) root         (0)    31000 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/css/font-awesome.min.css
--rw-r--r--   0 root         (0) root         (0)     9182 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/css/loginstyle.css
--rw-r--r--   0 root         (0) root         (0)     3804 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/css/persianDatepicker-default.css
--rw-r--r--   0 root         (0) root         (0)     5557 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/css/style.css
--rw-r--r--   0 root         (0) root         (0)    83821 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/css/util.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.921026 erscipcard-1.17.8/erscipcard/static/bt/fonts/
--rw-r--r--   0 root         (0) root         (0)    60820 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/fonts/BNAZANIN.TTF
--rw-r--r--   0 root         (0) root         (0)    61268 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/fonts/BTITR.TTF
--rw-r--r--   0 root         (0) root         (0)    84624 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/fonts/Vazir.ttf
--rw-r--r--   0 root         (0) root         (0)   165548 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.921026 erscipcard-1.17.8/erscipcard/static/bt/js/
--rw-r--r--   0 root         (0) root         (0)    78694 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/js/bootstrap.bundle.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    29875 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/js/persianDatepicker.js
--rw-r--r--   0 root         (0) root         (0)     1728 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/js/scripts.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.922026 erscipcard-1.17.8/erscipcard/static/bt/pics/
--rw-r--r--   0 root         (0) root         (0)    29117 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/pics/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/bt/pics/logo.png
--rw-r--r--   0 root         (0) root         (0)     4929 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/custom_modelField_with_formField
--rw-r--r--   0 root         (0) root         (0)    29117 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    35195 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/logo.png
--rw-r--r--   0 root         (0) root         (0)     1126 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.925026 erscipcard-1.17.8/erscipcard/static/spinner/
--rw-r--r--   0 root         (0) root         (0)     7573 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/atebits.css
--rw-r--r--   0 root         (0) root         (0)    14641 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/ball.css
--rw-r--r--   0 root         (0) root         (0)     1716 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/circles.css
--rw-r--r--   0 root         (0) root         (0)    11683 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/dots.css
--rw-r--r--   0 root         (0) root         (0)     2705 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/echo.css
--rw-r--r--   0 root         (0) root         (0)     3476 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/flower.css
--rw-r--r--   0 root         (0) root         (0)     6259 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/gauge.css
--rw-r--r--   0 root         (0) root         (0)     3523 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/heartbeat.css
--rw-r--r--   0 root         (0) root         (0)    17599 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/hexdots.css
--rw-r--r--   0 root         (0) root         (0)     1421 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/hole-pulse.css
--rw-r--r--   0 root         (0) root         (0)     2713 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/inner-circles.css
--rw-r--r--   0 root         (0) root         (0)     6223 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/plus-loader.css
--rw-r--r--   0 root         (0) root         (0)    18677 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/plus.css
--rw-r--r--   0 root         (0) root         (0)    12802 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/pong.css
--rw-r--r--   0 root         (0) root         (0)     1437 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/pulse.css
--rw-r--r--   0 root         (0) root         (0)     1532 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/refreshing.css
--rw-r--r--   0 root         (0) root         (0)     2105 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/spinner.css
--rw-r--r--   0 root         (0) root         (0)     4661 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/spinning-pixels.css
--rw-r--r--   0 root         (0) root         (0)     1257 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/three-quarters.css
--rw-r--r--   0 root         (0) root         (0)     1599 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/throbber.css
--rw-r--r--   0 root         (0) root         (0)     2220 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/timer.css
--rw-r--r--   0 root         (0) root         (0)    22371 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/whirly.css
--rw-r--r--   0 root         (0) root         (0)     3093 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinner/wobblebar.css
--rw-r--r--   0 root         (0) root         (0)   143659 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/static/spinners.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.926026 erscipcard-1.17.8/erscipcard/templates/
--rw-r--r--   0 root         (0) root         (0)      326 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/templates/AvatarFileUploadInput.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.926026 erscipcard-1.17.8/erscipcard/templates/erscipcard/
--rw-r--r--   0 root         (0) root         (0)     2606 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/templates/erscipcard/login.html
--rw-r--r--   0 root         (0) root         (0)    12656 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/templates/erscipcard/ou.html
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/templates/replace_re.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.926026 erscipcard-1.17.8/erscipcard/templatetags/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/templatetags/__init__.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/templatetags/basepath.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/tests.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/urls.py
--rw-r--r--   0 root         (0) root         (0)    10832 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/views.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-04-17 12:06:04.000000 erscipcard-1.17.8/erscipcard/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 12:06:21.917025 erscipcard-1.17.8/erscipcard.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1461 2023-04-17 12:06:21.000000 erscipcard-1.17.8/erscipcard.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2529 2023-04-17 12:06:21.000000 erscipcard-1.17.8/erscipcard.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 12:06:21.000000 erscipcard-1.17.8/erscipcard.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-04-17 12:06:21.000000 erscipcard-1.17.8/erscipcard.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-17 12:06:21.000000 erscipcard-1.17.8/erscipcard.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      769 2023-04-17 12:06:21.928026 erscipcard-1.17.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-17 12:06:04.000000 erscipcard-1.17.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.850565 erscipcard-1.17.81/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-18 07:07:50.000000 erscipcard-1.17.81/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-18 07:07:50.000000 erscipcard-1.17.81/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-18 07:07:59.850565 erscipcard-1.17.81/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      965 2023-04-18 07:07:50.000000 erscipcard-1.17.81/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.839564 erscipcard-1.17.81/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/admin.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/apps.py
+-rw-r--r--   0 root         (0) root         (0)      313 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.839564 erscipcard-1.17.81/erscipcard/migrations/
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/migrations/0001_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.841564 erscipcard-1.17.81/erscipcard/static/
+-rw-r--r--   0 root         (0) root         (0)    19616 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/1.docx
+-rw-r--r--   0 root         (0) root         (0)    14825 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/2.docx
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/BTITR.TTF
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.836564 erscipcard-1.17.81/erscipcard/static/bt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.842564 erscipcard-1.17.81/erscipcard/static/bt/css/
+-rw-r--r--   0 root         (0) root         (0)   175814 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/css/bootstrap.min.css
+-rw-r--r--   0 root         (0) root         (0)    31000 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/css/font-awesome.min.css
+-rw-r--r--   0 root         (0) root         (0)     9182 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/css/loginstyle.css
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/css/persianDatepicker-default.css
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/css/style.css
+-rw-r--r--   0 root         (0) root         (0)    83821 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/css/util.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.843565 erscipcard-1.17.81/erscipcard/static/bt/fonts/
+-rw-r--r--   0 root         (0) root         (0)    60820 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/fonts/BNAZANIN.TTF
+-rw-r--r--   0 root         (0) root         (0)    61268 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/fonts/BTITR.TTF
+-rw-r--r--   0 root         (0) root         (0)    84624 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/fonts/Vazir.ttf
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/fonts/fontawesome-webfont.ttf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.844565 erscipcard-1.17.81/erscipcard/static/bt/js/
+-rw-r--r--   0 root         (0) root         (0)    78694 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/js/bootstrap.bundle.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    29875 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/js/persianDatepicker.js
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/js/scripts.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.844565 erscipcard-1.17.81/erscipcard/static/bt/pics/
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/pics/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/bt/pics/logo.png
+-rw-r--r--   0 root         (0) root         (0)     4929 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/custom_modelField_with_formField
+-rw-r--r--   0 root         (0) root         (0)    29117 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/favicon.ico
+-rw-r--r--   0 root         (0) root         (0)    35195 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/logo.png
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/main.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.849565 erscipcard-1.17.81/erscipcard/static/spinner/
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/atebits.css
+-rw-r--r--   0 root         (0) root         (0)    14641 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/ball.css
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/circles.css
+-rw-r--r--   0 root         (0) root         (0)    11683 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/dots.css
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/echo.css
+-rw-r--r--   0 root         (0) root         (0)     3476 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/flower.css
+-rw-r--r--   0 root         (0) root         (0)     6259 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/gauge.css
+-rw-r--r--   0 root         (0) root         (0)     3523 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/heartbeat.css
+-rw-r--r--   0 root         (0) root         (0)    17599 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/hexdots.css
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/hole-pulse.css
+-rw-r--r--   0 root         (0) root         (0)     2713 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/inner-circles.css
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/plus-loader.css
+-rw-r--r--   0 root         (0) root         (0)    18677 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/plus.css
+-rw-r--r--   0 root         (0) root         (0)    12802 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/pong.css
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/pulse.css
+-rw-r--r--   0 root         (0) root         (0)     1532 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/refreshing.css
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/spinner.css
+-rw-r--r--   0 root         (0) root         (0)     4661 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/spinning-pixels.css
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/three-quarters.css
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/throbber.css
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/timer.css
+-rw-r--r--   0 root         (0) root         (0)    22371 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/whirly.css
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinner/wobblebar.css
+-rw-r--r--   0 root         (0) root         (0)   143659 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/static/spinners.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.849565 erscipcard-1.17.81/erscipcard/templates/
+-rw-r--r--   0 root         (0) root         (0)      309 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/templates/AvatarFileUploadInput.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.849565 erscipcard-1.17.81/erscipcard/templates/erscipcard/
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/templates/erscipcard/login.html
+-rw-r--r--   0 root         (0) root         (0)    12656 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/templates/erscipcard/ou.html
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/templates/replace_re.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.850565 erscipcard-1.17.81/erscipcard/templatetags/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/templatetags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/templatetags/basepath.py
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/tests.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/urls.py
+-rw-r--r--   0 root         (0) root         (0)    10832 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/views.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-04-18 07:07:50.000000 erscipcard-1.17.81/erscipcard/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:07:59.839564 erscipcard-1.17.81/erscipcard.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-18 07:07:59.000000 erscipcard-1.17.81/erscipcard.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-04-18 07:07:59.000000 erscipcard-1.17.81/erscipcard.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 07:07:59.000000 erscipcard-1.17.81/erscipcard.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-04-18 07:07:59.000000 erscipcard-1.17.81/erscipcard.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-18 07:07:59.000000 erscipcard-1.17.81/erscipcard.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      770 2023-04-18 07:07:59.851565 erscipcard-1.17.81/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-18 07:07:50.000000 erscipcard-1.17.81/setup.py
```

### Comparing `erscipcard-1.17.8/LICENSE` & `erscipcard-1.17.81/LICENSE`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/PKG-INFO` & `erscipcard-1.17.81/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erscipcard
-Version: 1.17.8
+Version: 1.17.81
 Summary: Erscipcard is a Django app to create personeli card.
 Home-page: https://github.com/epg900/erscipcard.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -26,29 +26,20 @@
 ```
 INSTALLED_APPS = [
 ...,
 'erscipcard',
 ]
 ```
 
-2.(optional) (for show pic in edit personel box) Add below line to STATICFILES_DIRS in your project setting.py file:
-
-```
-STATICFILES_DIRS = [
-...,
-BASE_DIR / "images",
-]
-```
-
-3.Include the erscipcard URLconf in your project urls.py like this:
+2.Include the erscipcard URLconf in your project urls.py like this:
 
 ```
 path('erscipcard/', include('erscipcard.urls')),
 ```
 
-4.Run ``python manage.py makemigrations``(optional) and ``python manage.py migrate``  to create the erscipcard models.
+3.Run ``python manage.py makemigrations``(optional) and ``python manage.py migrate``  to create the erscipcard models.
 
 then run ``python manage.py createsuperuser`` to create personel for login erscipcard page.
 
-5.Visit http://127.0.0.1:8000/erscipcard/ to create users and its cards.
+4.Visit http://127.0.0.1:8000/erscipcard/ to create users and its cards.
 
 first download card template , edit it and uplaod your custom template , then print cards.
```

### Comparing `erscipcard-1.17.8/README.md` & `erscipcard-1.17.81/erscipcard.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-Erscipcard
-=========
-Erscipcard is a Django app to create personeli card. 
-For each user,create a card and export it as pdf and docx documents.
-
-Tip
------------
-You can edit model.py file to create your own database table , also edit template MSWord file to customize your card.
-
-Quick start
------------
-1.Add "erscipcard" to your INSTALLED_APPS in your project setting.py file:
-```
-INSTALLED_APPS = [
-...,
-'erscipcard',
-]
-```
-
-2.(optional) (for show pic in edit personel box) Add below line to STATICFILES_DIRS in your project setting.py file:
-
-```
-STATICFILES_DIRS = [
-...,
-BASE_DIR / "images",
-]
-```
-
-3.Include the erscipcard URLconf in your project urls.py like this:
-
-```
-path('erscipcard/', include('erscipcard.urls')),
-```
-
-4.Run ``python manage.py makemigrations``(optional) and ``python manage.py migrate``  to create the erscipcard models.
-
-then run ``python manage.py createsuperuser`` to create personel for login erscipcard page.
-
-5.Visit http://127.0.0.1:8000/erscipcard/ to create users and its cards.
-
-first download card template , edit it and uplaod your custom template , then print cards.
+Metadata-Version: 2.1
+Name: erscipcard
+Version: 1.17.81
+Summary: Erscipcard is a Django app to create personeli card.
+Home-page: https://github.com/epg900/erscipcard.git
+Author: epg
+Author-email: epg900@gmail.com
+License: GNU GENERAL PUBLIC LICENSE
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+Erscipcard
+=========
+Erscipcard is a Django app to create personeli card. 
+For each user,create a card and export it as pdf and docx documents.
+
+Tip
+-----------
+You can edit model.py file to create your own database table , also edit template MSWord file to customize your card.
+
+Quick start
+-----------
+1.Add "erscipcard" to your INSTALLED_APPS in your project setting.py file:
+```
+INSTALLED_APPS = [
+...,
+'erscipcard',
+]
+```
+
+2.Include the erscipcard URLconf in your project urls.py like this:
+
+```
+path('erscipcard/', include('erscipcard.urls')),
+```
+
+3.Run ``python manage.py makemigrations``(optional) and ``python manage.py migrate``  to create the erscipcard models.
+
+then run ``python manage.py createsuperuser`` to create personel for login erscipcard page.
+
+4.Visit http://127.0.0.1:8000/erscipcard/ to create users and its cards.
+
+first download card template , edit it and uplaod your custom template , then print cards.
```

### Comparing `erscipcard-1.17.8/erscipcard/migrations/0001_initial.py` & `erscipcard-1.17.81/erscipcard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/models.py` & `erscipcard-1.17.81/erscipcard/models.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/1.docx` & `erscipcard-1.17.81/erscipcard/static/1.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/2.docx` & `erscipcard-1.17.81/erscipcard/static/2.docx`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/BNAZANIN.TTF` & `erscipcard-1.17.81/erscipcard/static/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/BTITR.TTF` & `erscipcard-1.17.81/erscipcard/static/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/css/bootstrap.min.css` & `erscipcard-1.17.81/erscipcard/static/bt/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/css/font-awesome.min.css` & `erscipcard-1.17.81/erscipcard/static/bt/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/css/loginstyle.css` & `erscipcard-1.17.81/erscipcard/static/bt/css/loginstyle.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/css/persianDatepicker-default.css` & `erscipcard-1.17.81/erscipcard/static/bt/css/persianDatepicker-default.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/css/style.css` & `erscipcard-1.17.81/erscipcard/static/bt/css/style.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/css/util.css` & `erscipcard-1.17.81/erscipcard/static/bt/css/util.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/fonts/BNAZANIN.TTF` & `erscipcard-1.17.81/erscipcard/static/bt/fonts/BNAZANIN.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/fonts/BTITR.TTF` & `erscipcard-1.17.81/erscipcard/static/bt/fonts/BTITR.TTF`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/fonts/Vazir.ttf` & `erscipcard-1.17.81/erscipcard/static/bt/fonts/Vazir.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/fonts/fontawesome-webfont.ttf` & `erscipcard-1.17.81/erscipcard/static/bt/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/js/bootstrap.bundle.min.js` & `erscipcard-1.17.81/erscipcard/static/bt/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/js/jquery.min.js` & `erscipcard-1.17.81/erscipcard/static/bt/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/js/persianDatepicker.js` & `erscipcard-1.17.81/erscipcard/static/bt/js/persianDatepicker.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/js/scripts.js` & `erscipcard-1.17.81/erscipcard/static/bt/js/scripts.js`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/pics/favicon.ico` & `erscipcard-1.17.81/erscipcard/static/bt/pics/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/bt/pics/logo.png` & `erscipcard-1.17.81/erscipcard/static/bt/pics/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/custom_modelField_with_formField` & `erscipcard-1.17.81/erscipcard/static/custom_modelField_with_formField`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/favicon.ico` & `erscipcard-1.17.81/erscipcard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/logo.png` & `erscipcard-1.17.81/erscipcard/static/logo.png`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/main.css` & `erscipcard-1.17.81/erscipcard/static/main.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/atebits.css` & `erscipcard-1.17.81/erscipcard/static/spinner/atebits.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/ball.css` & `erscipcard-1.17.81/erscipcard/static/spinner/ball.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/circles.css` & `erscipcard-1.17.81/erscipcard/static/spinner/circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/dots.css` & `erscipcard-1.17.81/erscipcard/static/spinner/dots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/echo.css` & `erscipcard-1.17.81/erscipcard/static/spinner/echo.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/flower.css` & `erscipcard-1.17.81/erscipcard/static/spinner/flower.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/gauge.css` & `erscipcard-1.17.81/erscipcard/static/spinner/gauge.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/heartbeat.css` & `erscipcard-1.17.81/erscipcard/static/spinner/heartbeat.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/hexdots.css` & `erscipcard-1.17.81/erscipcard/static/spinner/hexdots.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/hole-pulse.css` & `erscipcard-1.17.81/erscipcard/static/spinner/hole-pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/inner-circles.css` & `erscipcard-1.17.81/erscipcard/static/spinner/inner-circles.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/plus-loader.css` & `erscipcard-1.17.81/erscipcard/static/spinner/plus-loader.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/plus.css` & `erscipcard-1.17.81/erscipcard/static/spinner/plus.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/pong.css` & `erscipcard-1.17.81/erscipcard/static/spinner/pong.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/pulse.css` & `erscipcard-1.17.81/erscipcard/static/spinner/pulse.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/refreshing.css` & `erscipcard-1.17.81/erscipcard/static/spinner/refreshing.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/spinner.css` & `erscipcard-1.17.81/erscipcard/static/spinner/spinner.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/spinning-pixels.css` & `erscipcard-1.17.81/erscipcard/static/spinner/spinning-pixels.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/three-quarters.css` & `erscipcard-1.17.81/erscipcard/static/spinner/three-quarters.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/throbber.css` & `erscipcard-1.17.81/erscipcard/static/spinner/throbber.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/timer.css` & `erscipcard-1.17.81/erscipcard/static/spinner/timer.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/whirly.css` & `erscipcard-1.17.81/erscipcard/static/spinner/whirly.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinner/wobblebar.css` & `erscipcard-1.17.81/erscipcard/static/spinner/wobblebar.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/static/spinners.css` & `erscipcard-1.17.81/erscipcard/static/spinners.css`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/templates/erscipcard/login.html` & `erscipcard-1.17.81/erscipcard/templates/erscipcard/login.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/templates/erscipcard/ou.html` & `erscipcard-1.17.81/erscipcard/templates/erscipcard/ou.html`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/urls.py` & `erscipcard-1.17.81/erscipcard/urls.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard/views.py` & `erscipcard-1.17.81/erscipcard/views.py`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/erscipcard.egg-info/SOURCES.txt` & `erscipcard-1.17.81/erscipcard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erscipcard-1.17.8/setup.cfg` & `erscipcard-1.17.81/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erscipcard
-version = 1.17.8
+version = 1.17.81
 description = Erscipcard is a Django app to create personeli card.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/erscipcard.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

