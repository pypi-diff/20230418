# Comparing `tmp/lemoncheesecake-1.9.0.tar.gz` & `tmp/lemoncheesecake-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lemoncheesecake-1.9.0.tar", last modified: Sun Sep  5 20:19:19 2021, max compression
+gzip compressed data, was "dist/lemoncheesecake-1.9.1.tar", last modified: Mon Sep  6 20:34:56 2021, max compression
```

## Comparing `lemoncheesecake-1.9.0.tar` & `lemoncheesecake-1.9.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     3626 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/README.rst
--rwxrwxr-x   0 nicolas   (1001) nicolas   (1001)     2005 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/setup.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake.egg-info/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)        1 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      144 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake.egg-info/requires.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       16 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake.egg-info/top_level.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5909 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4433 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       50 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake.egg-info/entry_points.txt
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      510 2020-02-08 18:38:07.000000 lemoncheesecake-1.9.0/MANIFEST.in
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       38 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/setup.cfg
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     9588 2021-09-05 19:37:45.000000 lemoncheesecake-1.9.0/lemoncheesecake/project.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    14346 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/filter.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     9456 2021-09-03 22:36:36.000000 lemoncheesecake-1.9.0/lemoncheesecake/events.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/suite/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     8132 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/suite/builder.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5128 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/suite/core.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    10696 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/suite/loader.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       65 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/suite/__init__.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2135 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/utils.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       57 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/__init__.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2060 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/fixtures.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      399 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/version.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      971 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/bootstrap.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     7427 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/top.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4118 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/stats.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     6948 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/run.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2856 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/report.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      566 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/__init__.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2650 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/show.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4166 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/diff.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1584 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/main.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      265 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/cli/command.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4637 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/backend.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1763 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/loader.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    24346 2021-09-04 15:53:28.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/report.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      164 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/__init__.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2832 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/savingstrategy.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4989 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/replay.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     3250 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/reportdir.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5705 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/writer.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     8241 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/console.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2475 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/slack.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1596 2020-12-20 22:09:27.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/html.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    11004 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/reportportal.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    13286 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/xml.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      384 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/__init__.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     3768 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/junit.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    10410 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/json_.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     9760 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/console.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/bdd/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5149 2021-09-04 12:20:20.000000 lemoncheesecake-1.9.0/lemoncheesecake/bdd/behave.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)        0 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/bdd/__init__.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2189 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/exceptions.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1621 2021-09-05 19:37:45.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/threading.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      214 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/resources.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      588 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/time.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1923 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/orderedset.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1654 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/introspection.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      703 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/text.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2390 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/moduleimport.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      913 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/typecheck.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)        0 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/__init__.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2890 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/terminalsize.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      354 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/helpers/console.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       73 2021-09-05 19:55:58.000000 lemoncheesecake-1.9.0/lemoncheesecake/__init__.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4344 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/matcher.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     3174 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/dict_.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     3751 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/value.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5543 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/string.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2099 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/types_.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      560 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/__init__.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     6145 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/composites.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5344 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/list_.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5403 2021-07-30 22:33:42.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/operations.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      441 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/matching/__init__.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    21373 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/runner.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    16660 2021-09-05 19:37:45.000000 lemoncheesecake-1.9.0/lemoncheesecake/fixture.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    15454 2021-09-04 15:53:28.000000 lemoncheesecake-1.9.0/lemoncheesecake/session.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      940 2021-09-04 15:53:28.000000 lemoncheesecake-1.9.0/lemoncheesecake/api.py
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      592 2020-12-20 22:29:43.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/report_static.html
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   108738 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.svg
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    18028 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.woff2
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    23424 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.woff
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    20127 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.eot
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    45404 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.ttf
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    47706 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.css.map
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    23409 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.min.css
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   146082 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.css
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   121260 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.min.css
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    26132 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.css
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   389227 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.css.map
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    54416 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.min.css.map
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5532 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.min.css.map
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    36868 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/bootstrap.min.js
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      484 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/npm.js
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    68954 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/bootstrap.js
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2464 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/report.css
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      866 2020-02-08 18:38:07.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/report_external.html
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   246806 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/report.js
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    97180 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/jquery-1.12.3.min.js
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   142382 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-slate.min.css
-drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/project/
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      133 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/resources/project/template.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     7475 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.0/lemoncheesecake/metadatapolicy.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5799 2021-09-04 12:20:20.000000 lemoncheesecake-1.9.0/lemoncheesecake/task.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     6094 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.0/lemoncheesecake/testtree.py
--rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5909 2021-09-05 20:19:19.000000 lemoncheesecake-1.9.0/PKG-INFO
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     3626 2021-09-06 20:33:08.000000 lemoncheesecake-1.9.1/README.rst
+-rwxrwxr-x   0 nicolas   (1001) nicolas   (1001)     2005 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/setup.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake.egg-info/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)        1 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake.egg-info/dependency_links.txt
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      144 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake.egg-info/requires.txt
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       16 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake.egg-info/top_level.txt
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5909 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake.egg-info/PKG-INFO
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4433 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake.egg-info/SOURCES.txt
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       50 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake.egg-info/entry_points.txt
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      510 2020-02-08 18:38:07.000000 lemoncheesecake-1.9.1/MANIFEST.in
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       38 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/setup.cfg
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     9588 2021-09-05 19:37:45.000000 lemoncheesecake-1.9.1/lemoncheesecake/project.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    14346 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/filter.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     9456 2021-09-03 22:36:36.000000 lemoncheesecake-1.9.1/lemoncheesecake/events.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/suite/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     8132 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/suite/builder.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5128 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/suite/core.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    10696 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/suite/loader.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       65 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/suite/__init__.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2135 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/utils.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       57 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/__init__.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2060 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/fixtures.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      399 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/version.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      971 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/bootstrap.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     7427 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/top.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4118 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/stats.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     6948 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/run.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2856 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/report.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      566 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/__init__.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2650 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/show.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4166 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/diff.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1584 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/main.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      265 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/cli/command.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4637 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/backend.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1763 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/loader.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    24366 2021-09-06 20:11:09.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/report.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      164 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/__init__.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2832 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/savingstrategy.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4989 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/replay.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     3250 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/reportdir.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5782 2021-09-06 20:17:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/writer.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     8241 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/console.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2475 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/slack.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1596 2020-12-20 22:09:27.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/html.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    11004 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/reportportal.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    13286 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/xml.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      384 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/__init__.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     3768 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/junit.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    10410 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/json_.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     9760 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/console.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/bdd/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5149 2021-09-04 12:20:20.000000 lemoncheesecake-1.9.1/lemoncheesecake/bdd/behave.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)        0 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/bdd/__init__.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2189 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/exceptions.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1621 2021-09-05 19:37:45.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/threading.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      214 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/resources.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      588 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/time.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1923 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/orderedset.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     1654 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/introspection.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      703 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/text.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2390 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/moduleimport.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      913 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/typecheck.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)        0 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/__init__.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2890 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/terminalsize.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      354 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/helpers/console.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)       73 2021-09-06 20:33:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/__init__.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     4344 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/matcher.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     3174 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/dict_.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     3751 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/value.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5543 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/string.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2099 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/types_.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      560 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/__init__.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     6145 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/composites.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5344 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/list_.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5403 2021-07-30 22:33:42.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/operations.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      441 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/matching/__init__.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    21370 2021-09-06 20:14:02.000000 lemoncheesecake-1.9.1/lemoncheesecake/runner.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    16660 2021-09-05 19:37:45.000000 lemoncheesecake-1.9.1/lemoncheesecake/fixture.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    15454 2021-09-04 15:53:28.000000 lemoncheesecake-1.9.1/lemoncheesecake/session.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      940 2021-09-04 15:53:28.000000 lemoncheesecake-1.9.1/lemoncheesecake/api.py
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      592 2020-12-20 22:29:43.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/report_static.html
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   108738 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    18028 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.woff2
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    23424 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    20127 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    45404 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.ttf
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    47706 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.css.map
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    23409 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.min.css
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   146082 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.css
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   121260 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.min.css
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    26132 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.css
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   389227 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.css.map
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    54416 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.min.css.map
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5532 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.min.css.map
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    36868 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/bootstrap.min.js
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      484 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/npm.js
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    68954 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/bootstrap.js
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     2464 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/report.css
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      866 2020-02-08 18:38:07.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/report_external.html
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   246806 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/report.js
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)    97180 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/jquery-1.12.3.min.js
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)   142382 2019-05-05 22:06:18.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-slate.min.css
+drwxrwxr-x   0 nicolas   (1001) nicolas   (1001)        0 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/project/
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)      133 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/resources/project/template.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     7475 2020-11-08 15:56:23.000000 lemoncheesecake-1.9.1/lemoncheesecake/metadatapolicy.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5799 2021-09-04 12:20:20.000000 lemoncheesecake-1.9.1/lemoncheesecake/task.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     6094 2021-09-04 12:21:08.000000 lemoncheesecake-1.9.1/lemoncheesecake/testtree.py
+-rw-rw-r--   0 nicolas   (1001) nicolas   (1001)     5909 2021-09-06 20:34:56.000000 lemoncheesecake-1.9.1/PKG-INFO
```

### Comparing `lemoncheesecake-1.9.0/README.rst` & `lemoncheesecake-1.9.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 lemoncheesecake: Test Storytelling
 ==================================
 
-lemoncheesecake is a functional test framework for Python that brings trust around test results.
+lemoncheesecake is a end-to-end test framework for Python that brings trust around test results.
 It allows test developers to be very explicit about what their tests really do with logging, matchers, file attachments, etc..
 
 Here is a test example:
 
 .. code-block:: python
 
     import json
```

### Comparing `lemoncheesecake-1.9.0/setup.py` & `lemoncheesecake-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake.egg-info/PKG-INFO` & `lemoncheesecake-1.9.1/lemoncheesecake.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: lemoncheesecake
-Version: 1.9.0
+Version: 1.9.1
 Summary: Test Storytelling
 Home-page: http://lemoncheesecake.io
 Author: Nicolas Delon
 Author-email: nicolas.delon@gmail.com
 License: Apache License (Version 2.0)
 Project-URL: Source, https://github.com/lemoncheesecake/lemoncheesecake
 Project-URL: Documentation, http://docs.lemoncheesecake.io/
 Project-URL: Tracker, https://github.com/lemoncheesecake/lemoncheesecake/issues
 Description: lemoncheesecake: Test Storytelling
         ==================================
         
-        lemoncheesecake is a functional test framework for Python that brings trust around test results.
+        lemoncheesecake is a end-to-end test framework for Python that brings trust around test results.
         It allows test developers to be very explicit about what their tests really do with logging, matchers, file attachments, etc..
         
         Here is a test example:
         
         .. code-block:: python
         
             import json
```

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake.egg-info/SOURCES.txt` & `lemoncheesecake-1.9.1/lemoncheesecake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/project.py` & `lemoncheesecake-1.9.1/lemoncheesecake/project.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/filter.py` & `lemoncheesecake-1.9.1/lemoncheesecake/filter.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/events.py` & `lemoncheesecake-1.9.1/lemoncheesecake/events.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/suite/builder.py` & `lemoncheesecake-1.9.1/lemoncheesecake/suite/builder.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/suite/core.py` & `lemoncheesecake-1.9.1/lemoncheesecake/suite/core.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/suite/loader.py` & `lemoncheesecake-1.9.1/lemoncheesecake/suite/loader.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/utils.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/utils.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/fixtures.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/fixtures.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/bootstrap.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/bootstrap.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/top.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/top.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/stats.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/run.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/report.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/__init__.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/show.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/commands/diff.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/commands/diff.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/cli/main.py` & `lemoncheesecake-1.9.1/lemoncheesecake/cli/main.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/backend.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/backend.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/loader.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/loader.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/report.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -425,17 +425,18 @@
 
     def __hash__(self):
         return hash((self.node_type, self.node_hierarchy))
 
     def __str__(self):
         ret = ""
         if self.node_hierarchy:
-            ret += ".".join(self.node_hierarchy) + " "
+            ret += "'%s' " % ".".join(self.node_hierarchy)
         ret += ("session setup", "session teardown", "suite setup", "suite teardown", "test")[self.node_type]
-        return "<%s>" % ret
+
+        return "<ReportLocation %s>" % ret
 
 
 def flatten_results(suites):
     # type: (Iterator[SuiteResult]) -> Iterator[Result]
     for suite in flatten_suites(suites):
         if suite.suite_setup:
             yield suite.suite_setup
```

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/savingstrategy.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/savingstrategy.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/replay.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/replay.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/reportdir.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/reportdir.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/writer.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     def _get_suite_result(self, suite):
         return self.report.get_suite(suite)
 
     def _add_step_log(self, log, event):
         result = self.report.get(event.location)
         assert result, "Cannot find location %s in the report" % event.location
         step = self._lookup_step(event)
-        assert not step.end_time, "Cannot update step '%s', it is already ended" % step.description
+        assert step, "Cannot find active step for %s" % event.location
+        assert not step.end_time, "Cannot update step '%s', it has already been ended" % step.description
         step.add_log(log)
 
     @staticmethod
     def _initialize_result(start_time):
         result = Result()
         result.start_time = start_time
         return result
```

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/console.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/console.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/slack.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/slack.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/html.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/html.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/reportportal.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/reportportal.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/xml.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/xml.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/junit.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/junit.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/json_.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/json_.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/reporting/backends/console.py` & `lemoncheesecake-1.9.1/lemoncheesecake/reporting/backends/console.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/bdd/behave.py` & `lemoncheesecake-1.9.1/lemoncheesecake/bdd/behave.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/exceptions.py` & `lemoncheesecake-1.9.1/lemoncheesecake/exceptions.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/helpers/threading.py` & `lemoncheesecake-1.9.1/lemoncheesecake/helpers/threading.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/helpers/time.py` & `lemoncheesecake-1.9.1/lemoncheesecake/helpers/time.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/helpers/orderedset.py` & `lemoncheesecake-1.9.1/lemoncheesecake/helpers/orderedset.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/helpers/introspection.py` & `lemoncheesecake-1.9.1/lemoncheesecake/helpers/introspection.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/helpers/text.py` & `lemoncheesecake-1.9.1/lemoncheesecake/helpers/text.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/helpers/moduleimport.py` & `lemoncheesecake-1.9.1/lemoncheesecake/helpers/moduleimport.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/helpers/typecheck.py` & `lemoncheesecake-1.9.1/lemoncheesecake/helpers/typecheck.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/helpers/terminalsize.py` & `lemoncheesecake-1.9.1/lemoncheesecake/helpers/terminalsize.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/matching/matcher.py` & `lemoncheesecake-1.9.1/lemoncheesecake/matching/matcher.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/dict_.py` & `lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/dict_.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/value.py` & `lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/value.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/string.py` & `lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/string.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/types_.py` & `lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/types_.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/__init__.py` & `lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/composites.py` & `lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/composites.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/matching/matchers/list_.py` & `lemoncheesecake-1.9.1/lemoncheesecake/matching/matchers/list_.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/matching/operations.py` & `lemoncheesecake-1.9.1/lemoncheesecake/matching/operations.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/runner.py` & `lemoncheesecake-1.9.1/lemoncheesecake/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,16 +169,17 @@
         setup_teardown_funcs = list()
         setup_teardown_funcs.append((setup_test_wrapper, teardown_test_wrapper))
         scheduled_fixtures = context.fixture_registry.get_fixtures_scheduled_for_test(
             self.test, self.suite_scheduled_fixtures
         )
         setup_teardown_funcs.extend(scheduled_fixtures.get_setup_teardown_pairs())
 
+        context.session.set_step("Setup test")
+
         if any(setup for setup, _ in setup_teardown_funcs):
-            context.session.set_step("Setup test")
             teardown_funcs = context.run_setup_funcs(setup_teardown_funcs, ReportLocation.in_test(self.test))
         else:
             teardown_funcs = [teardown for _, teardown in setup_teardown_funcs if teardown]
 
         ###
         # Run test:
         ###
```

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/fixture.py` & `lemoncheesecake-1.9.1/lemoncheesecake/fixture.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/session.py` & `lemoncheesecake-1.9.1/lemoncheesecake/session.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/api.py` & `lemoncheesecake-1.9.1/lemoncheesecake/api.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/report_static.html` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/report_static.html`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.svg` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.woff2` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.woff` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.eot` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.ttf` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.css.map` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.min.css` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.css` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.min.css` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.css` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.css.map` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.min.css.map` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.min.css.map` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/css/bootstrap-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/bootstrap.min.js` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/bootstrap.js` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-3.3.6-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/report.css` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/report.css`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/report_external.html` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/report_external.html`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/report.js` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/report.js`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/jquery-1.12.3.min.js` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/jquery-1.12.3.min.js`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/resources/html/bootstrap-slate.min.css` & `lemoncheesecake-1.9.1/lemoncheesecake/resources/html/bootstrap-slate.min.css`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/metadatapolicy.py` & `lemoncheesecake-1.9.1/lemoncheesecake/metadatapolicy.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/task.py` & `lemoncheesecake-1.9.1/lemoncheesecake/task.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/lemoncheesecake/testtree.py` & `lemoncheesecake-1.9.1/lemoncheesecake/testtree.py`

 * *Files identical despite different names*

### Comparing `lemoncheesecake-1.9.0/PKG-INFO` & `lemoncheesecake-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: lemoncheesecake
-Version: 1.9.0
+Version: 1.9.1
 Summary: Test Storytelling
 Home-page: http://lemoncheesecake.io
 Author: Nicolas Delon
 Author-email: nicolas.delon@gmail.com
 License: Apache License (Version 2.0)
 Project-URL: Source, https://github.com/lemoncheesecake/lemoncheesecake
 Project-URL: Documentation, http://docs.lemoncheesecake.io/
 Project-URL: Tracker, https://github.com/lemoncheesecake/lemoncheesecake/issues
 Description: lemoncheesecake: Test Storytelling
         ==================================
         
-        lemoncheesecake is a functional test framework for Python that brings trust around test results.
+        lemoncheesecake is a end-to-end test framework for Python that brings trust around test results.
         It allows test developers to be very explicit about what their tests really do with logging, matchers, file attachments, etc..
         
         Here is a test example:
         
         .. code-block:: python
         
             import json
```

