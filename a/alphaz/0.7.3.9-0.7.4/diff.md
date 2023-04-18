# Comparing `tmp/alphaz-0.7.3.9.tar.gz` & `tmp/alphaz-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alphaz-0.7.3.9.tar", last modified: Wed Apr 12 11:28:54 2023, max compression
+gzip compressed data, was "dist/alphaz-0.7.4.tar", last modified: Tue Apr 18 11:53:11 2023, max compression
```

## Comparing `alphaz-0.7.3.9.tar` & `alphaz-0.7.4.tar`

### file list

```diff
@@ -1,339 +1,389 @@
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8469 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/MANIFEST.in
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.3.9/README.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.729881 alphaz-0.7.3.9/alphaz/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      320 2023-03-23 07:52:23.000000 alphaz-0.7.3.9/alphaz/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/alphaz.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/alphaz.code-workspace
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/alphaz.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/api.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      662 2021-09-15 19:20:13.000000 alphaz-0.7.3.9/alphaz/api.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.3.9/alphaz/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.729881 alphaz-0.7.3.9/alphaz/apis/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/apis/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/apis/log.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.3.9/alphaz/apis/mails.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/apis/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/apis/routes/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/apis/routes/admin.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/apis/routes/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/apis/routes/basic_tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2902 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/apis/routes/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.3.9/alphaz/apis/routes/git.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.3.9/alphaz/apis/routes/logs.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.3.9/alphaz/apis/routes/mails.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6262 2023-03-17 07:21:40.000000 alphaz-0.7.3.9/alphaz/apis/routes/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1330 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/apis/routes/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/apis/routes/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.3.9/alphaz/apis/routes/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.3.9/alphaz/apis/routes/user_management/application_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.3.9/alphaz/apis/routes/user_management/permission_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.3.9/alphaz/apis/routes/user_management/role_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.3.9/alphaz/apis/routes/user_management/user_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3025 2023-03-17 18:14:36.000000 alphaz-0.7.3.9/alphaz/apis/routes/users.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/apis/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/apis/users/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/apis/users/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.3.9/alphaz/apis/users/ldap.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.3.9/alphaz/apis/users/users.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config/config.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config/config.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.3.9/alphaz/config/main_configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config/page.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config/source.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.3.9/alphaz/core.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/documentations/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/documentations/docs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_admin.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9432 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_api.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_core.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5602 2022-07-19 09:10:48.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_database.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_screens.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_setup.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.3.9/alphaz/documentations/docs/configuration.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.3.9/alphaz/documentations/docs/documentation.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/documentations/docs/index.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      440 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/documentations/mkdocs.yml
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9286 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/404.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_admin/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10320 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_admin/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    50340 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_api/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18850 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_core/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    43708 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_database/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_screens/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17967 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_screens/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_setup/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20169 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_setup/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.721881 alphaz-0.7.3.9/alphaz/documentations/site/assets/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/assets/images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/images/favicon.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/workers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24568 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/documentation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13157 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/documentation/index.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25613 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/search/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    53878 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/search/search_index.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1081 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/sitemap.xml
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      200 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/sitemap.xml.gz
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/git.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.3.9/alphaz/help.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.749881 alphaz-0.7.3.9/alphaz/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5786 2023-03-24 12:18:56.000000 alphaz-0.7.3.9/alphaz/libs/api_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/barcode_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13997 2023-03-24 12:18:56.000000 alphaz-0.7.3.9/alphaz/libs/config_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.3.9/alphaz/libs/converter_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9014 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/libs/database_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.3.9/alphaz/libs/date_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6222 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/libs/dict_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.749881 alphaz-0.7.3.9/alphaz/libs/emulation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.3.9/alphaz/libs/emulation/vt102_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/events.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/libs/files_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1096 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/libs/flask_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/ftp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/libs/img_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/libs/io_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.3.9/alphaz/libs/json_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/libs/logs_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.3.9/alphaz/libs/mail_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/nav_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.3.9/alphaz/libs/notifications_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/number_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/os_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/process_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/libs/py_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      657 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/scp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/libs/search_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6386 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/libs/secure_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.3.9/alphaz/libs/soap_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/sql_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18289 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/libs/ssh_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11021 2023-04-08 08:30:59.000000 alphaz-0.7.3.9/alphaz/libs/string_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5139 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/libs/test_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/libs/time_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.3.9/alphaz/libs/transactions_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5041 2022-12-01 15:14:08.000000 alphaz-0.7.3.9/alphaz/libs/user_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.749881 alphaz-0.7.3.9/alphaz/libs/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.3.9/alphaz/libs/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.3.9/alphaz/libs/user_management/application_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.3.9/alphaz/libs/user_management/permission_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.3.9/alphaz/libs/user_management/role_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.3.9/alphaz/libs/user_management/user_management_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.749881 alphaz-0.7.3.9/alphaz/mails/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.753881 alphaz-0.7.3.9/alphaz/mails/Images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/Images/Background.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/Images/Facebook_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/Images/Twitter_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/Images/Web_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/mails/Images/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/Mail.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.3.9/alphaz/mails/Webmail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/mails/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.3.9/alphaz/mails/debug.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.3.9/alphaz/mails/mail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/password_reset.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.3.9/alphaz/mails/stay_in_touch.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/template.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.753881 alphaz-0.7.3.9/alphaz/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.3.9/alphaz/models/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.753881 alphaz-0.7.3.9/alphaz/models/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.3.9/alphaz/models/api/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      710 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/api/_answer.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.3.9/alphaz/models/api/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.3.9/alphaz/models/api/_methods.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14253 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/api/_parameter.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.3.9/alphaz/models/api/_requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18565 2023-03-29 19:05:00.000000 alphaz-0.7.3.9/alphaz/models/api/_route.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21563 2023-03-23 07:52:23.000000 alphaz-0.7.3.9/alphaz/models/api/_structures.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.3.9/alphaz/models/api/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.3.9/alphaz/models/base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.753881 alphaz-0.7.3.9/alphaz/models/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25438 2023-01-06 09:14:28.000000 alphaz-0.7.3.9/alphaz/models/config/_config.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12129 2021-08-12 12:49:09.000000 alphaz-0.7.3.9/alphaz/models/config/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.3.9/alphaz/models/database/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.3.9/alphaz/models/database/main_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.3.9/alphaz/models/database/models.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.3.9/alphaz/models/database/operators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.3.9/alphaz/models/database/requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/database/row.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    53758 2023-03-16 19:44:05.000000 alphaz-0.7.3.9/alphaz/models/database/structure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/database/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4418 2023-03-16 19:51:01.000000 alphaz-0.7.3.9/alphaz/models/database/users_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.3.9/alphaz/models/database/utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.3.9/alphaz/models/database/views.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/excel.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5126 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/models/ftp.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.3.9/alphaz/models/img.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/json/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/json/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.3.9/alphaz/models/json/_converters.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/logger/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.3.9/alphaz/models/logger/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.3.9/alphaz/models/logger/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14091 2023-04-05 11:16:09.000000 alphaz-0.7.3.9/alphaz/models/logger/_logger.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/logger/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/logs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.3.9/alphaz/models/logs/main.log
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.3.9/alphaz/models/logs/main.log.2021-11-07
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.3.9/alphaz/models/main/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27102 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/models/main/_base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/main/_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_core/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14630 2023-04-08 19:36:08.000000 alphaz-0.7.3.9/alphaz/models/main/_core/_core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_core/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.3.9/alphaz/models/main/_enum.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1862 2023-02-17 08:49:35.000000 alphaz-0.7.3.9/alphaz/models/main/_exception.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_file.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_process.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_request.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_singleton.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/models/request.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/models/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/models/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6780 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/tests/_category.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3095 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/tests/_group.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      109 2021-09-10 07:16:32.000000 alphaz-0.7.3.9/alphaz/models/tests/_levels.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4174 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/tests/_method.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4571 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/models/tests/_save.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13445 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/models/tests/_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6927 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/models/tests/_wrappers.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.3.9/alphaz/models/user.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/watcher.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/pocs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/pocs/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/reload_gitignore.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.3.9/alphaz/req.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/requirements.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/run.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/src/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/src/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/src/alpha.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/src/configs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/src/configs/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.3.9/alphaz/src/configs/loggers.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.3.9/alphaz/src/configs/loggers_colors.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/src/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/src/database/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/stitch/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/Core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/stitch/imports/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/imports/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/stitch/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/stitch/models/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/models/element.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/run.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/stitch.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.769881 alphaz-0.7.3.9/alphaz/stitch/web-drivers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/web-drivers/chromedriver.exe
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/stitch/web-drivers/geckodriver
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.725881 alphaz-0.7.3.9/alphaz/stitch/websites/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.777881 alphaz-0.7.3.9/alphaz/stitch/websites/Test/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/websites/Test/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.777881 alphaz-0.7.3.9/alphaz/stitch/websites/stiki/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.3.9/alphaz/stitch/websites/stiki/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.781881 alphaz-0.7.3.9/alphaz/templates/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/templates/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.781881 alphaz-0.7.3.9/alphaz/templates/assets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/templates/assets/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.781881 alphaz-0.7.3.9/alphaz/templates/assets/css/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.3.9/alphaz/templates/assets/css/home.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/css/logs.css
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/templates/assets/images/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/admin.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/alpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/save.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/start-icon.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/user.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/wsalpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/loading.gif
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/templates/assets/js/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/templates/assets/js/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/js/libs/ansi_up.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/js/libs/jquery.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.3.9/alphaz/templates/assets/js/logs.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/templates/hello.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/templates/home.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/logs.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.3.9/alphaz/test.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13857 2023-03-28 08:47:21.000000 alphaz-0.7.3.9/alphaz/tests/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/tests/basic_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.3.9/alphaz/tests/configurations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22695 2023-03-16 19:44:05.000000 alphaz-0.7.3.9/alphaz/tests/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/tests/processes.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/tests/utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/utils/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/utils/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11552 2023-02-16 14:12:47.000000 alphaz-0.7.3.9/alphaz/utils/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/utils/clean.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.3.9/alphaz/utils/configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.3.9/alphaz/utils/database_to_dataclass.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/utils/decorators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/utils/ensure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.3.9/alphaz/utils/mep.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.3.9/alphaz/utils/screens.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/utils/selectionMenu.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/utils/tasks.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1535 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/utils/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/utils/time.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/utils/transactions.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.729881 alphaz-0.7.3.9/alphaz.egg-info/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/alphaz.egg-info/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9706 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/alphaz.egg-info/SOURCES.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/alphaz.egg-info/dependency_links.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      447 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/alphaz.egg-info/requires.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/alphaz.egg-info/top_level.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-12 11:28:54.789881 alphaz-0.7.3.9/setup.cfg
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3075 2023-04-12 11:28:06.000000 alphaz-0.7.3.9/setup.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.254447 alphaz-0.7.4/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11114 2023-04-18 11:53:10.000000 alphaz-0.7.4/MANIFEST.in
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      585 2023-04-18 11:53:11.254447 alphaz-0.7.4/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.4/README.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.190447 alphaz-0.7.4/alphaz/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/README.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      333 2023-04-13 12:43:58.000000 alphaz-0.7.4/alphaz/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/alphaz.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/alphaz.code-workspace
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.4/alphaz/alphaz.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/api.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/api.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.4/alphaz/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.194447 alphaz-0.7.4/alphaz/apis/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4/alphaz/apis/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.4/alphaz/apis/log.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.4/alphaz/apis/mails.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.194447 alphaz-0.7.4/alphaz/apis/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/apis/routes/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/apis/routes/admin.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/apis/routes/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/apis/routes/basic_tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/apis/routes/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.4/alphaz/apis/routes/git.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.4/alphaz/apis/routes/logs.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.4/alphaz/apis/routes/mails.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6262 2023-03-17 07:21:40.000000 alphaz-0.7.4/alphaz/apis/routes/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1330 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/apis/routes/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.194447 alphaz-0.7.4/alphaz/apis/routes/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.4/alphaz/apis/routes/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.4/alphaz/apis/routes/user_management/application_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.4/alphaz/apis/routes/user_management/permission_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.4/alphaz/apis/routes/user_management/role_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.4/alphaz/apis/routes/user_management/user_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3025 2023-03-17 18:14:36.000000 alphaz-0.7.4/alphaz/apis/routes/users.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/apis/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.194447 alphaz-0.7.4/alphaz/apis/users/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.4/alphaz/apis/users/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.4/alphaz/apis/users/ldap.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.4/alphaz/apis/users/users.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.194447 alphaz-0.7.4/alphaz/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/config/config.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/config/config.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.4/alphaz/config/main_configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/config/page.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/config/source.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.4/alphaz/core.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.194447 alphaz-0.7.4/alphaz/documentations/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.198447 alphaz-0.7.4/alphaz/documentations/docs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.4/alphaz/documentations/docs/alpha_admin.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.4/alphaz/documentations/docs/alpha_core.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.4/alphaz/documentations/docs/alpha_screens.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.4/alphaz/documentations/docs/alpha_setup.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.198447 alphaz-0.7.4/alphaz/documentations/docs/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/api/authorizations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/api/cache.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2932 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/api/configuration.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/api/issues.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/api/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/api/methods.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/api/parameters.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/api/routes.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/api/sqlalchemy.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/api_database.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.4/alphaz/documentations/docs/configuration.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.198447 alphaz-0.7.4/alphaz/documentations/docs/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/database/init.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/database/instantiate.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/database/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/database/model.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/database/relations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/database/schema.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/docs/database/update.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.4/alphaz/documentations/docs/documentation.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.4/alphaz/documentations/docs/index.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/documentations/mkdocs.yml
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.198447 alphaz-0.7.4/alphaz/documentations/site/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/404.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.198447 alphaz-0.7.4/alphaz/documentations/site/alpha_admin/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/alpha_admin/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.198447 alphaz-0.7.4/alphaz/documentations/site/alpha_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/alpha_core/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.198447 alphaz-0.7.4/alphaz/documentations/site/alpha_screens/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/alpha_screens/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.198447 alphaz-0.7.4/alphaz/documentations/site/alpha_setup/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/alpha_setup/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.182447 alphaz-0.7.4/alphaz/documentations/site/api/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/api/authorizations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/api/authorizations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/api/cache/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/api/cache/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/api/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27646 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/api/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/api/issues/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/api/issues/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/api/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/api/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/api/methods/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/api/methods/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/api/parameters/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/api/parameters/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/api/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/api/routes/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/api/sqlalchemy/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/api/sqlalchemy/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/api_database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/api_database/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.182447 alphaz-0.7.4/alphaz/documentations/site/assets/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/assets/images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/images/favicon.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.202447 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.206447 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.206447 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/workers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/assets/stylesheets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.186447 alphaz-0.7.4/alphaz/documentations/site/database/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/database/init/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23027 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/database/init/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/database/instantiate/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/database/instantiate/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/database/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/database/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/database/model/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/database/model/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/database/relations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/database/relations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/database/schema/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/database/schema/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/database/update/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/database/update/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/documentation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/documentation/index.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.210447 alphaz-0.7.4/alphaz/documentations/site/search/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    54137 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz/documentations/site/search/search_index.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/sitemap.xml
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2023-04-18 11:53:09.000000 alphaz-0.7.4/alphaz/documentations/site/sitemap.xml.gz
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.4/alphaz/git.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.4/alphaz/help.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.214447 alphaz-0.7.4/alphaz/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/libs/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5785 2023-04-13 20:34:53.000000 alphaz-0.7.4/alphaz/libs/api_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/libs/barcode_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13999 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/libs/config_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.4/alphaz/libs/converter_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9073 2023-04-18 11:53:08.000000 alphaz-0.7.4/alphaz/libs/database_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.4/alphaz/libs/date_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6324 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/libs/dict_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.214447 alphaz-0.7.4/alphaz/libs/emulation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.4/alphaz/libs/emulation/vt102_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/libs/events.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.4/alphaz/libs/files_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/libs/flask_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/libs/ftp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.4/alphaz/libs/img_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-04-11 14:13:25.000000 alphaz-0.7.4/alphaz/libs/io_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.4/alphaz/libs/json_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.4/alphaz/libs/logs_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.4/alphaz/libs/mail_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/libs/nav_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.4/alphaz/libs/notifications_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/libs/number_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/libs/os_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/libs/process_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.4/alphaz/libs/py_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      657 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/libs/scp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.4/alphaz/libs/search_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6397 2023-04-13 20:34:53.000000 alphaz-0.7.4/alphaz/libs/secure_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.4/alphaz/libs/soap_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/libs/sql_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18289 2023-03-16 15:41:50.000000 alphaz-0.7.4/alphaz/libs/ssh_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11021 2023-04-08 08:30:59.000000 alphaz-0.7.4/alphaz/libs/string_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5139 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/libs/test_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.4/alphaz/libs/time_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.4/alphaz/libs/transactions_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5041 2022-12-01 15:14:08.000000 alphaz-0.7.4/alphaz/libs/user_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.214447 alphaz-0.7.4/alphaz/libs/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.4/alphaz/libs/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.4/alphaz/libs/user_management/application_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.4/alphaz/libs/user_management/permission_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.4/alphaz/libs/user_management/role_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.4/alphaz/libs/user_management/user_management_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.214447 alphaz-0.7.4/alphaz/mails/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.218447 alphaz-0.7.4/alphaz/mails/Images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/mails/Images/Background.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/mails/Images/Facebook_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/mails/Images/Twitter_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/mails/Images/Web_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4/alphaz/mails/Images/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/mails/Mail.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.4/alphaz/mails/Webmail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4/alphaz/mails/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.4/alphaz/mails/debug.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.4/alphaz/mails/mail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/mails/password_reset.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.4/alphaz/mails/stay_in_touch.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/mails/template.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.218447 alphaz-0.7.4/alphaz/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.4/alphaz/models/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.222447 alphaz-0.7.4/alphaz/models/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.4/alphaz/models/api/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      884 2023-04-12 16:11:09.000000 alphaz-0.7.4/alphaz/models/api/_answer.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.4/alphaz/models/api/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.4/alphaz/models/api/_methods.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14253 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/models/api/_parameter.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.4/alphaz/models/api/_requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18649 2023-04-13 20:07:38.000000 alphaz-0.7.4/alphaz/models/api/_route.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21563 2023-03-23 07:52:23.000000 alphaz-0.7.4/alphaz/models/api/_structures.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.4/alphaz/models/api/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.4/alphaz/models/base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.222447 alphaz-0.7.4/alphaz/models/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25438 2023-01-06 09:14:28.000000 alphaz-0.7.4/alphaz/models/config/_config.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12129 2021-08-12 12:49:09.000000 alphaz-0.7.4/alphaz/models/config/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.222447 alphaz-0.7.4/alphaz/models/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.4/alphaz/models/database/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.4/alphaz/models/database/main_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.4/alphaz/models/database/models.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.4/alphaz/models/database/operators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.4/alphaz/models/database/requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/database/row.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    55224 2023-04-18 11:53:08.000000 alphaz-0.7.4/alphaz/models/database/structure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/models/database/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4418 2023-03-16 19:51:01.000000 alphaz-0.7.4/alphaz/models/database/users_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.4/alphaz/models/database/utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.4/alphaz/models/database/views.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/excel.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5126 2022-01-17 10:25:20.000000 alphaz-0.7.4/alphaz/models/ftp.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.4/alphaz/models/img.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.222447 alphaz-0.7.4/alphaz/models/json/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/json/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.4/alphaz/models/json/_converters.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.222447 alphaz-0.7.4/alphaz/models/logger/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.4/alphaz/models/logger/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.4/alphaz/models/logger/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14091 2023-04-05 11:16:09.000000 alphaz-0.7.4/alphaz/models/logger/_logger.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/logger/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.222447 alphaz-0.7.4/alphaz/models/logs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.4/alphaz/models/logs/main.log
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.4/alphaz/models/logs/main.log.2021-11-07
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.226446 alphaz-0.7.4/alphaz/models/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.4/alphaz/models/main/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27277 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/models/main/_base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.226446 alphaz-0.7.4/alphaz/models/main/_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/main/_core/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14630 2023-04-08 19:36:08.000000 alphaz-0.7.4/alphaz/models/main/_core/_core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/main/_core/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.4/alphaz/models/main/_enum.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1862 2023-02-17 08:49:35.000000 alphaz-0.7.4/alphaz/models/main/_exception.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/main/_file.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/main/_process.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/main/_request.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/main/_singleton.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.4/alphaz/models/request.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.226446 alphaz-0.7.4/alphaz/models/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2023-03-16 15:41:50.000000 alphaz-0.7.4/alphaz/models/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6780 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/models/tests/_category.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3095 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/models/tests/_group.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      109 2021-09-10 07:16:32.000000 alphaz-0.7.4/alphaz/models/tests/_levels.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4174 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/models/tests/_method.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4571 2023-04-11 14:13:25.000000 alphaz-0.7.4/alphaz/models/tests/_save.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13495 2023-04-18 11:53:08.000000 alphaz-0.7.4/alphaz/models/tests/_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7359 2023-04-18 09:00:04.000000 alphaz-0.7.4/alphaz/models/tests/_wrappers.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.4/alphaz/models/user.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/models/watcher.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.226446 alphaz-0.7.4/alphaz/pocs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/pocs/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/reload_gitignore.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.4/alphaz/req.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.4/alphaz/requirements.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.4/alphaz/run.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.226446 alphaz-0.7.4/alphaz/src/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4/alphaz/src/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/src/alpha.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.226446 alphaz-0.7.4/alphaz/src/configs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.4/alphaz/src/configs/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.4/alphaz/src/configs/loggers.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.4/alphaz/src/configs/loggers_colors.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.226446 alphaz-0.7.4/alphaz/src/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4/alphaz/src/database/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.230447 alphaz-0.7.4/alphaz/stitch/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/stitch/Core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/stitch/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.230447 alphaz-0.7.4/alphaz/stitch/imports/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/stitch/imports/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.230447 alphaz-0.7.4/alphaz/stitch/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4/alphaz/stitch/models/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/stitch/models/element.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/stitch/run.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/stitch/stitch.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.238447 alphaz-0.7.4/alphaz/stitch/web-drivers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/stitch/web-drivers/chromedriver.exe
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.4/alphaz/stitch/web-drivers/geckodriver
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.186447 alphaz-0.7.4/alphaz/stitch/websites/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.250446 alphaz-0.7.4/alphaz/stitch/websites/Test/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/stitch/websites/Test/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.250446 alphaz-0.7.4/alphaz/stitch/websites/stiki/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.4/alphaz/stitch/websites/stiki/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.250446 alphaz-0.7.4/alphaz/templates/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4/alphaz/templates/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.250446 alphaz-0.7.4/alphaz/templates/assets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.4/alphaz/templates/assets/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.250446 alphaz-0.7.4/alphaz/templates/assets/css/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.4/alphaz/templates/assets/css/home.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/assets/css/logs.css
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.250446 alphaz-0.7.4/alphaz/templates/assets/images/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.250446 alphaz-0.7.4/alphaz/templates/assets/images/icons/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/assets/images/icons/admin.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/assets/images/icons/alpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/assets/images/icons/save.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/assets/images/icons/start-icon.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/assets/images/icons/user.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/assets/images/icons/wsalpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/assets/images/loading.gif
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.250446 alphaz-0.7.4/alphaz/templates/assets/js/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.250446 alphaz-0.7.4/alphaz/templates/assets/js/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/assets/js/libs/ansi_up.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/assets/js/libs/jquery.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.4/alphaz/templates/assets/js/logs.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/templates/hello.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.4/alphaz/templates/home.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.4/alphaz/templates/logs.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.4/alphaz/test.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.254447 alphaz-0.7.4/alphaz/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13857 2023-03-28 08:47:21.000000 alphaz-0.7.4/alphaz/tests/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.4/alphaz/tests/basic_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.4/alphaz/tests/configurations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22695 2023-03-16 19:44:05.000000 alphaz-0.7.4/alphaz/tests/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/tests/processes.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/tests/utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.254447 alphaz-0.7.4/alphaz/utils/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/utils/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11552 2023-02-16 14:12:47.000000 alphaz-0.7.4/alphaz/utils/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.4/alphaz/utils/clean.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.4/alphaz/utils/configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.4/alphaz/utils/database_to_dataclass.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.4/alphaz/utils/decorators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.4/alphaz/utils/ensure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.4/alphaz/utils/mep.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.4/alphaz/utils/screens.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.4/alphaz/utils/selectionMenu.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.4/alphaz/utils/tasks.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1535 2023-02-23 09:08:35.000000 alphaz-0.7.4/alphaz/utils/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.4/alphaz/utils/time.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.4/alphaz/utils/transactions.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-18 11:53:11.194447 alphaz-0.7.4/alphaz.egg-info/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      585 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz.egg-info/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11189 2023-04-18 11:53:11.000000 alphaz-0.7.4/alphaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz.egg-info/requires.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-18 11:53:10.000000 alphaz-0.7.4/alphaz.egg-info/top_level.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-18 11:53:11.254447 alphaz-0.7.4/setup.cfg
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3092 2023-04-18 11:52:29.000000 alphaz-0.7.4/setup.py
```

### Comparing `alphaz-0.7.3.9/MANIFEST.in` & `alphaz-0.7.4/MANIFEST.in`

 * *Files 18% similar despite different names*

```diff
@@ -77,49 +77,91 @@
 include alphaz/models/main/__pycache__
 include alphaz/models/logger/__pycache__
 include alphaz/models/json/__pycache__
 include alphaz/models/tests/__pycache__
 include alphaz/models/database/__pycache__
 include alphaz/models/main/_core/__pycache__
 include alphaz/libs/user_management/__pycache__
-include alphaz/documentations/docs/alpha_database.md
-include alphaz/documentations/docs/alpha_api.md
+include alphaz/documentations/docs/api
+include alphaz/documentations/docs/api_database.md
 include alphaz/documentations/docs/index.md
 include alphaz/documentations/docs/alpha_setup.md
 include alphaz/documentations/docs/documentation.md
 include alphaz/documentations/docs/alpha_admin.md
 include alphaz/documentations/docs/configuration.md
 include alphaz/documentations/docs/alpha_core.md
 include alphaz/documentations/docs/alpha_screens.md
+include alphaz/documentations/docs/database
+include alphaz/documentations/site/api
 include alphaz/documentations/site/assets
 include alphaz/documentations/site/search
-include alphaz/documentations/site/alpha_api
 include alphaz/documentations/site/sitemap.xml.gz
 include alphaz/documentations/site/alpha_setup
 include alphaz/documentations/site/404.html
 include alphaz/documentations/site/configuration
 include alphaz/documentations/site/alpha_core
 include alphaz/documentations/site/alpha_screens
 include alphaz/documentations/site/alpha_admin
 include alphaz/documentations/site/documentation
 include alphaz/documentations/site/sitemap.xml
+include alphaz/documentations/site/api_database
 include alphaz/documentations/site/index.html
-include alphaz/documentations/site/alpha_database
+include alphaz/documentations/site/database
+include alphaz/documentations/docs/api/issues.md
+include alphaz/documentations/docs/api/cache.md
+include alphaz/documentations/docs/api/parameters.md
+include alphaz/documentations/docs/api/authorizations.md
+include alphaz/documentations/docs/api/main.md
+include alphaz/documentations/docs/api/sqlalchemy.md
+include alphaz/documentations/docs/api/configuration.md
+include alphaz/documentations/docs/api/methods.md
+include alphaz/documentations/docs/api/routes.md
+include alphaz/documentations/docs/database/schema.md
+include alphaz/documentations/docs/database/init.md
+include alphaz/documentations/docs/database/update.md
+include alphaz/documentations/docs/database/relations.md
+include alphaz/documentations/docs/database/main.md
+include alphaz/documentations/docs/database/model.md
+include alphaz/documentations/docs/database/instantiate.md
+include alphaz/documentations/site/api/routes
+include alphaz/documentations/site/api/authorizations
+include alphaz/documentations/site/api/configuration
+include alphaz/documentations/site/api/main
+include alphaz/documentations/site/api/methods
+include alphaz/documentations/site/api/parameters
+include alphaz/documentations/site/api/sqlalchemy
+include alphaz/documentations/site/api/issues
+include alphaz/documentations/site/api/cache
 include alphaz/documentations/site/assets/images
 include alphaz/documentations/site/assets/stylesheets
 include alphaz/documentations/site/assets/javascripts
 include alphaz/documentations/site/search/search_index.json
-include alphaz/documentations/site/alpha_api/index.html
 include alphaz/documentations/site/alpha_setup/index.html
 include alphaz/documentations/site/configuration/index.html
 include alphaz/documentations/site/alpha_core/index.html
 include alphaz/documentations/site/alpha_screens/index.html
 include alphaz/documentations/site/alpha_admin/index.html
 include alphaz/documentations/site/documentation/index.html
-include alphaz/documentations/site/alpha_database/index.html
+include alphaz/documentations/site/api_database/index.html
+include alphaz/documentations/site/database/update
+include alphaz/documentations/site/database/main
+include alphaz/documentations/site/database/model
+include alphaz/documentations/site/database/instantiate
+include alphaz/documentations/site/database/relations
+include alphaz/documentations/site/database/schema
+include alphaz/documentations/site/database/init
+include alphaz/documentations/site/api/routes/index.html
+include alphaz/documentations/site/api/authorizations/index.html
+include alphaz/documentations/site/api/configuration/index.html
+include alphaz/documentations/site/api/main/index.html
+include alphaz/documentations/site/api/methods/index.html
+include alphaz/documentations/site/api/parameters/index.html
+include alphaz/documentations/site/api/sqlalchemy/index.html
+include alphaz/documentations/site/api/issues/index.html
+include alphaz/documentations/site/api/cache/index.html
 include alphaz/documentations/site/assets/images/favicon.png
 include alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
 include alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
 include alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
 include alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
 include alphaz/documentations/site/assets/javascripts/lunr
 include alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
@@ -146,24 +188,32 @@
 include alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
 include alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
 include alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
 include alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
 include alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
 include alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
 include alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
+include alphaz/documentations/site/database/update/index.html
+include alphaz/documentations/site/database/main/index.html
+include alphaz/documentations/site/database/model/index.html
+include alphaz/documentations/site/database/instantiate/index.html
+include alphaz/documentations/site/database/relations/index.html
+include alphaz/documentations/site/database/schema/index.html
+include alphaz/documentations/site/database/init/index.html
 include alphaz/src/configs/config.json
 include alphaz/src/configs/loggers_colors.json
 include alphaz/src/configs/loggers.json
 include alphaz/mails/Images/Twitter_logo.png
 include alphaz/mails/Images/Web_logo.png
 include alphaz/mails/Images/Facebook_logo.png
 include alphaz/mails/Images/Background.png
 include alphaz/stitch
 include alphaz/api.json
 include alphaz/apis
+include alphaz/README.md
 include alphaz/templates
 include alphaz/git.sh
 include alphaz/models
 include alphaz/requirements.txt
 include alphaz/alphaz.bat
 include alphaz/config
 include alphaz/api.bat
```

### Comparing `alphaz-0.7.3.9/PKG-INFO` & `alphaz-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.3.9
+Version: 0.7.4
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.3.9.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.4.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.3.9/README.md` & `alphaz-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/api.json` & `alphaz-0.7.4/alphaz/api.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9285714285714286%*

 * *Differences: {"'admins'": "OrderedDict([('ips', ['127.0.0.1'])])"}*

```diff
@@ -1,8 +1,13 @@
 {
+    "admins": {
+        "ips": [
+            "127.0.0.1"
+        ]
+    },
     "databases": {
         "test": {
             "host": "127.0.0.1",
             "name": "alpha",
             "password": "testalpha7",
             "port": "3306",
             "type": "mysql",
```

### Comparing `alphaz-0.7.3.9/alphaz/api.py` & `alphaz-0.7.4/alphaz/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/mails.py` & `alphaz-0.7.4/alphaz/apis/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/admin.py` & `alphaz-0.7.4/alphaz/apis/routes/admin.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/api.py` & `alphaz-0.7.4/alphaz/apis/routes/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/basic_tests.py` & `alphaz-0.7.4/alphaz/apis/routes/basic_tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/database.py` & `alphaz-0.7.4/alphaz/apis/routes/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,24 @@
 
 
 @route("/schemas", parameters=[Parameter("name")])
 def get_schemas():
     return database_lib.get_schemas(**API.gets())
 
 
-@route("/database/tables", admin=True)
+@route(
+    "/database/tables",
+    parameters=[
+        Parameter("binds", ptype=List[str]),
+        Parameter("tables", ptype=List[str]),
+    ],
+    admin=True,
+)
 def liste_tables():
-    return DB.get_tables_models()
+    return DB.get_tables_models(**API.gets())
 
 
 @route("/database/tables/names", parameters=[Parameter("bind")], admin=True)
 def liste_tables_names():
     return DB.get_tables_names(**API.gets())
 
 
@@ -56,14 +63,15 @@
     parameters=[
         Parameter("binds", ptype=List[str]),
         Parameter("tables", ptype=List[str]),
         Parameter("drop", ptype=bool, default=False),
         Parameter("truncate", ptype=bool, default=False),
         Parameter("force", ptype=bool, default=False),
         Parameter("create", ptype=bool, default=False),
+        Parameter("init", ptype=bool, default=False),
     ],
 )
 def init_all_database():
     database_lib.init_databases(core, **API.gets())
 
 
 @route("database/blocking", admin=True)
```

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/logs.py` & `alphaz-0.7.4/alphaz/apis/routes/logs.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/mails.py` & `alphaz-0.7.4/alphaz/apis/routes/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/main.py` & `alphaz-0.7.4/alphaz/apis/routes/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/tests.py` & `alphaz-0.7.4/alphaz/apis/routes/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/user_management/application_management.py` & `alphaz-0.7.4/alphaz/apis/routes/user_management/application_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/user_management/permission_management.py` & `alphaz-0.7.4/alphaz/apis/routes/user_management/permission_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/user_management/role_management.py` & `alphaz-0.7.4/alphaz/apis/routes/user_management/role_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/user_management/user_management.py` & `alphaz-0.7.4/alphaz/apis/routes/user_management/user_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/routes/users.py` & `alphaz-0.7.4/alphaz/apis/routes/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/tests.py` & `alphaz-0.7.4/alphaz/apis/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/users/ldap.py` & `alphaz-0.7.4/alphaz/apis/users/ldap.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/apis/users/users.py` & `alphaz-0.7.4/alphaz/apis/users/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/config/config.css` & `alphaz-0.7.4/alphaz/config/config.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/config/config.html` & `alphaz-0.7.4/alphaz/config/config.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/config/main_configuration.py` & `alphaz-0.7.4/alphaz/config/main_configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/config/page.py` & `alphaz-0.7.4/alphaz/config/page.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/config/source.html` & `alphaz-0.7.4/alphaz/config/source.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/config.json` & `alphaz-0.7.4/alphaz/config.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/docs/alpha_core.md` & `alphaz-0.7.4/alphaz/documentations/docs/alpha_core.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/docs/alpha_screens.md` & `alphaz-0.7.4/alphaz/documentations/docs/alpha_screens.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/docs/alpha_setup.md` & `alphaz-0.7.4/alphaz/documentations/docs/alpha_setup.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/docs/configuration.md` & `alphaz-0.7.4/alphaz/documentations/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/docs/index.md` & `alphaz-0.7.4/alphaz/documentations/docs/index.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/alpha_api/index.html` & `alphaz-0.7.4/alphaz/documentations/site/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width,initial-scale=1">
       
       
       
       
-      <link rel="icon" href="../assets/images/favicon.png">
+      <link rel="icon" href="assets/images/favicon.png">
       <meta name="generator" content="mkdocs-1.1.2, mkdocs-material-7.1.1">
     
     
       
-        <title>Api - Alpha Documentation</title>
+        <title>Alpha Documentation</title>
       
     
     
-      <link rel="stylesheet" href="../assets/stylesheets/main.9299cb39.min.css">
+      <link rel="stylesheet" href="assets/stylesheets/main.9299cb39.min.css">
       
         
-        <link rel="stylesheet" href="../assets/stylesheets/palette.ef6f36e2.min.css">
+        <link rel="stylesheet" href="assets/stylesheets/palette.ef6f36e2.min.css">
         
       
     
     
     
       
         
@@ -47,34 +47,34 @@
     
     
     
     
     <body dir="ltr" data-md-color-scheme="" data-md-color-primary="none" data-md-color-accent="none">
   
     
-    <script>function __prefix(e){return new URL("..",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
+    <script>function __prefix(e){return new URL(".",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
     
     <input class="md-toggle" data-md-toggle="drawer" type="checkbox" id="__drawer" autocomplete="off">
     <input class="md-toggle" data-md-toggle="search" type="checkbox" id="__search" autocomplete="off">
     <label class="md-overlay" for="__drawer"></label>
     <div data-md-component="skip">
       
         
-        <a href="#alpha-api-system" class="md-skip">
+        <a href="#welcome-to-alpha-environment-documention" class="md-skip">
           Skip to content
         </a>
       
     </div>
     <div data-md-component="announce">
       
     </div>
     
       <header class="md-header" data-md-component="header">
   <nav class="md-header__inner md-grid" aria-label="Header">
-    <a href=".." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     <label class="md-header__button md-icon" for="__drawer">
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M3 6h18v2H3V6m0 5h18v2H3v-2m0 5h18v2H3v-2z"/></svg>
@@ -85,15 +85,15 @@
           <span class="md-ellipsis">
             Alpha Documentation
           </span>
         </div>
         <div class="md-header__topic" data-md-component="header-topic">
           <span class="md-ellipsis">
             
-              Api
+              Home
             
           </span>
         </div>
       </div>
     </div>
     
     
@@ -146,15 +146,15 @@
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 
 
 <nav class="md-nav md-nav--primary" aria-label="Navigation" data-md-level="0">
   <label class="md-nav__title" for="__drawer">
-    <a href=".." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     Alpha Documentation
   </label>
@@ -163,76 +163,31 @@
     
       
       
       
 
   
   
-  
-    <li class="md-nav__item">
-      <a href=".." class="md-nav__link">
-        Home
-      </a>
-    </li>
-  
-
-    
-      
-      
-      
-
-  
-  
-  
-    <li class="md-nav__item">
-      <a href="../alpha_setup/" class="md-nav__link">
-        Setup
-      </a>
-    </li>
-  
-
-    
-      
-      
-      
-
-  
-  
-  
-    <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
-        Core
-      </a>
-    </li>
-  
-
-    
-      
-      
-      
-
-  
-  
     
   
   
     <li class="md-nav__item md-nav__item--active">
       
       <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
       
         
       
       
         <label class="md-nav__link md-nav__link--active" for="__toc">
-          Api
+          Home
           <span class="md-nav__icon md-icon"></span>
         </label>
       
-      <a href="./" class="md-nav__link md-nav__link--active">
-        Api
+      <a href="." class="md-nav__link md-nav__link--active">
+        Home
       </a>
       
         
 <nav class="md-nav md-nav--secondary" aria-label="Table of contents">
   
   
     
@@ -241,362 +196,437 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
-  <a href="#introduction" class="md-nav__link">
-    Introduction
+  <a href="#purpose" class="md-nav__link">
+    Purpose
   </a>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#launch" class="md-nav__link">
-    Launch
+  <a href="#backend-alphaz" class="md-nav__link">
+    Backend: Alphaz
   </a>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#how-to-use" class="md-nav__link">
-    How to use
-  </a>
-  
-    <nav class="md-nav" aria-label="How to use">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#routes" class="md-nav__link">
-    Routes
+  <a href="#features" class="md-nav__link">
+    Features
   </a>
   
 </li>
-        
-      </ul>
-    </nav>
-  
-</li>
       
         <li class="md-nav__item">
-  <a href="#configuration" class="md-nav__link">
-    Configuration
-  </a>
-  
-    <nav class="md-nav" aria-label="Configuration">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#main" class="md-nav__link">
-    Main
+  <a href="#tech" class="md-nav__link">
+    Tech
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#mails" class="md-nav__link">
-    Mails
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#auth" class="md-nav__link">
-    Auth
+      
+        <li class="md-nav__item">
+  <a href="#project-layout" class="md-nav__link">
+    Project layout
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#reloader-type" class="md-nav__link">
-    Reloader type
+      
+        <li class="md-nav__item">
+  <a href="#frontend-alphaa" class="md-nav__link">
+    Frontend: Alphaa
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#admin" class="md-nav__link">
-    Admin
+      
+        <li class="md-nav__item">
+  <a href="#features_1" class="md-nav__link">
+    Features
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#dashboard" class="md-nav__link">
-    Dashboard
+      
+        <li class="md-nav__item">
+  <a href="#project-layout_1" class="md-nav__link">
+    Project layout
   </a>
   
 </li>
-        
-      </ul>
-    </nav>
+      
+    </ul>
   
-</li>
+</nav>
       
-        <li class="md-nav__item">
-  <a href="#routes_1" class="md-nav__link">
-    Routes
-  </a>
+    </li>
   
-    <nav class="md-nav" aria-label="Routes">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#basic" class="md-nav__link">
-    Basic
-  </a>
+
+    
+      
+      
+      
+
   
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#description" class="md-nav__link">
-    Description
-  </a>
   
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#category" class="md-nav__link">
-    Category
-  </a>
   
-</li>
-        
-      </ul>
-    </nav>
+    <li class="md-nav__item">
+      <a href="alpha_setup/" class="md-nav__link">
+        Setup
+      </a>
+    </li>
   
-</li>
+
+    
       
-        <li class="md-nav__item">
-  <a href="#parameters" class="md-nav__link">
-    Parameters
-  </a>
+      
+      
+
   
-    <nav class="md-nav" aria-label="Parameters">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#simple" class="md-nav__link">
-    Simple
-  </a>
   
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#object" class="md-nav__link">
-    Object
-  </a>
   
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#default-parameters" class="md-nav__link">
-    Default parameters
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
+    <li class="md-nav__item">
+      <a href="alpha_core/" class="md-nav__link">
+        Core
+      </a>
+    </li>
   
-</li>
+
+    
       
-        <li class="md-nav__item">
-  <a href="#sqlalchemy-model" class="md-nav__link">
-    SqlAlchemy model
-  </a>
-  
-</li>
       
-        <li class="md-nav__item">
-  <a href="#methods" class="md-nav__link">
-    Methods
-  </a>
-  
-</li>
       
-        <li class="md-nav__item">
-  <a href="#authorizations" class="md-nav__link">
-    Authorizations
-  </a>
+
   
-    <nav class="md-nav" aria-label="Authorizations">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#login-system" class="md-nav__link">
-    Login system
-  </a>
   
-</li>
-        
-      </ul>
-    </nav>
   
-</li>
+    
+    <li class="md-nav__item md-nav__item--nested">
       
-        <li class="md-nav__item">
-  <a href="#cache" class="md-nav__link">
-    Cache
-  </a>
-  
-</li>
       
-        <li class="md-nav__item">
-  <a href="#admin_1" class="md-nav__link">
-    Admin
-  </a>
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_4" type="checkbox" id="__nav_4" >
+      
+      <label class="md-nav__link" for="__nav_4">
+        Api
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Api" data-md-level="1">
+        <label class="md-nav__title" for="__nav_4">
+          <span class="md-nav__icon md-icon"></span>
+          Api
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
   
-    <nav class="md-nav" aria-label="Admin">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#condition" class="md-nav__link">
-    Condition
-  </a>
   
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#how-to-use_1" class="md-nav__link">
-    How to use
-  </a>
   
-    <nav class="md-nav" aria-label="How to use">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#single-route-mode" class="md-nav__link">
-    Single route mode
-  </a>
+    <li class="md-nav__item">
+      <a href="api/main/" class="md-nav__link">
+        Main
+      </a>
+    </li>
   
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#login-to-the-api" class="md-nav__link">
-    Login to the api
-  </a>
+
+          
+            
   
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#logout-from-the-api" class="md-nav__link">
-    Logout from the api
-  </a>
   
-</li>
-        
-      </ul>
-    </nav>
   
-</li>
-        
-      </ul>
-    </nav>
+    <li class="md-nav__item">
+      <a href="api/configuration/" class="md-nav__link">
+        Configuration
+      </a>
+    </li>
   
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#issues" class="md-nav__link">
-    Issues
-  </a>
+
+          
+            
   
-    <nav class="md-nav" aria-label="Issues">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#database-alias" class="md-nav__link">
-    Database alias
-  </a>
   
-</li>
-        
-      </ul>
-    </nav>
   
-</li>
-      
-    </ul>
+    <li class="md-nav__item">
+      <a href="api/routes/" class="md-nav__link">
+        Routes
+      </a>
+    </li>
   
-</nav>
-      
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="api/parameters/" class="md-nav__link">
+        Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="api/methods/" class="md-nav__link">
+        Methods
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="api/cache/" class="md-nav__link">
+        Cache
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="api/authorizations/" class="md-nav__link">
+        Authorizations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="api/sqlalchemy/" class="md-nav__link">
+        SqlAlchemy
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="api/issues/" class="md-nav__link">
+        Issues
+      </a>
+    </li>
+  
+
+          
+        </ul>
+      </nav>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_screens/" class="md-nav__link">
+      <a href="alpha_screens/" class="md-nav__link">
         Screens
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../configuration/" class="md-nav__link">
+      <a href="configuration/" class="md-nav__link">
         Configuration
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
-    <li class="md-nav__item">
-      <a href="../alpha_database/" class="md-nav__link">
+    
+    <li class="md-nav__item md-nav__item--nested">
+      
+      
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_7" type="checkbox" id="__nav_7" >
+      
+      <label class="md-nav__link" for="__nav_7">
         Database
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Database" data-md-level="1">
+        <label class="md-nav__title" for="__nav_7">
+          <span class="md-nav__icon md-icon"></span>
+          Database
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="database/main/" class="md-nav__link">
+        Main
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="database/init/" class="md-nav__link">
+        Init
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="database/model/" class="md-nav__link">
+        Model
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="database/schema/" class="md-nav__link">
+        Schema
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="database/instantiate/" class="md-nav__link">
+        Instantiate
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="database/update/" class="md-nav__link">
+        Update
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="database/relations/" class="md-nav__link">
+        Relations
       </a>
     </li>
   
 
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
+  
+
+          
+        </ul>
+      </nav>
+    </li>
+  
+
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../documentation/" class="md-nav__link">
+      <a href="documentation/" class="md-nav__link">
         Documentation
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_admin/" class="md-nav__link">
+      <a href="alpha_admin/" class="md-nav__link">
         Administration
       </a>
     </li>
   
 
     
   </ul>
@@ -620,610 +650,199 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
-  <a href="#introduction" class="md-nav__link">
-    Introduction
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#launch" class="md-nav__link">
-    Launch
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#how-to-use" class="md-nav__link">
-    How to use
-  </a>
-  
-    <nav class="md-nav" aria-label="How to use">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#routes" class="md-nav__link">
-    Routes
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#configuration" class="md-nav__link">
-    Configuration
-  </a>
-  
-    <nav class="md-nav" aria-label="Configuration">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#main" class="md-nav__link">
-    Main
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#mails" class="md-nav__link">
-    Mails
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#auth" class="md-nav__link">
-    Auth
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#reloader-type" class="md-nav__link">
-    Reloader type
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#admin" class="md-nav__link">
-    Admin
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#dashboard" class="md-nav__link">
-    Dashboard
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#routes_1" class="md-nav__link">
-    Routes
-  </a>
-  
-    <nav class="md-nav" aria-label="Routes">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#basic" class="md-nav__link">
-    Basic
+  <a href="#purpose" class="md-nav__link">
+    Purpose
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#description" class="md-nav__link">
-    Description
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#category" class="md-nav__link">
-    Category
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
       
         <li class="md-nav__item">
-  <a href="#parameters" class="md-nav__link">
-    Parameters
-  </a>
-  
-    <nav class="md-nav" aria-label="Parameters">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#simple" class="md-nav__link">
-    Simple
+  <a href="#backend-alphaz" class="md-nav__link">
+    Backend: Alphaz
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#object" class="md-nav__link">
-    Object
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#default-parameters" class="md-nav__link">
-    Default parameters
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
       
         <li class="md-nav__item">
-  <a href="#sqlalchemy-model" class="md-nav__link">
-    SqlAlchemy model
+  <a href="#features" class="md-nav__link">
+    Features
   </a>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#methods" class="md-nav__link">
-    Methods
+  <a href="#tech" class="md-nav__link">
+    Tech
   </a>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#authorizations" class="md-nav__link">
-    Authorizations
-  </a>
-  
-    <nav class="md-nav" aria-label="Authorizations">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#login-system" class="md-nav__link">
-    Login system
+  <a href="#project-layout" class="md-nav__link">
+    Project layout
   </a>
   
 </li>
-        
-      </ul>
-    </nav>
-  
-</li>
       
         <li class="md-nav__item">
-  <a href="#cache" class="md-nav__link">
-    Cache
+  <a href="#frontend-alphaa" class="md-nav__link">
+    Frontend: Alphaa
   </a>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#admin_1" class="md-nav__link">
-    Admin
-  </a>
-  
-    <nav class="md-nav" aria-label="Admin">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#condition" class="md-nav__link">
-    Condition
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#how-to-use_1" class="md-nav__link">
-    How to use
+  <a href="#features_1" class="md-nav__link">
+    Features
   </a>
   
-    <nav class="md-nav" aria-label="How to use">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#single-route-mode" class="md-nav__link">
-    Single route mode
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#login-to-the-api" class="md-nav__link">
-    Login to the api
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#logout-from-the-api" class="md-nav__link">
-    Logout from the api
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
 </li>
       
         <li class="md-nav__item">
-  <a href="#issues" class="md-nav__link">
-    Issues
-  </a>
-  
-    <nav class="md-nav" aria-label="Issues">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#database-alias" class="md-nav__link">
-    Database alias
+  <a href="#project-layout_1" class="md-nav__link">
+    Project layout
   </a>
   
 </li>
-        
-      </ul>
-    </nav>
-  
-</li>
       
     </ul>
   
 </nav>
                   </div>
                 </div>
               </div>
             
           
           <div class="md-content" data-md-component="content">
             <article class="md-content__inner md-typeset">
               
                 
                 
-                <h1 id="alpha-api-system">Alpha API system</h1>
-<h2 id="introduction">Introduction</h2>
-<p>The api system is completely based on Flask and compatible. You could use Flask inside Alpha system without any issue.</p>
-<h2 id="launch">Launch</h2>
-<p>To start the api execute the <code>api.py</code> file</p>
-<div class="highlight"><pre><span></span><code>python api.py
+                <h1 id="welcome-to-alpha-environment-documention">Welcome to Alpha environment documention</h1>
+<p>Alpha is an <strong>ecosystem</strong> based on a multiple <strong>frameworks</strong> and <strong>libraries</strong> for both <strong>frontend</strong> and <strong>backend</strong>.</p>
+<h2 id="purpose">Purpose</h2>
+<p>The purpose of the <strong>ecosystem</strong> is to simplify any dev activity. </p>
+<details class="note"><summary>Standard query approach</summary><div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
+<span class="n">DB</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span> 
+
+<span class="k">def</span> <span class="nf">get_logs</span><span class="p">(</span><span class="n">start_date</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">end_date</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">useLimit</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">pageForLimit</span><span class="o">=</span><span class="mi">1</span><span class="p">):</span>
+    <span class="n">total</span> <span class="o">=</span> <span class="mi">0</span>
+    <span class="n">logs</span> <span class="o">=</span> <span class="p">[]</span>
+    <span class="n">limit</span> <span class="o">=</span> <span class="mi">20</span>
+    <span class="n">start</span> <span class="o">=</span> <span class="p">(</span><span class="n">pageForLimit</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span> <span class="o">*</span> <span class="n">limit</span>
+
+    <span class="n">query</span> <span class="o">=</span> <span class="s2">&quot;SELECT COUNT(*) AS count FROM logs&quot;</span>
+    <span class="n">parameters</span> <span class="o">=</span> <span class="p">[]</span>
+    <span class="k">if</span> <span class="n">start_date</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="n">end_date</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot; AND CAST(date AS DATE) between </span><span class="si">%s</span><span class="s2"> and </span><span class="si">%s</span><span class="s2">&quot;</span>
+        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">start_date</span><span class="p">)</span>
+        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">end_date</span><span class="p">)</span>       
+    <span class="n">query</span><span class="o">+=</span> <span class="s2">&quot; ORDER BY date DESC&quot;</span>
+
+    <span class="n">rows</span> <span class="o">=</span> <span class="n">DB</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">query</span><span class="p">,</span> <span class="n">parameters</span><span class="p">)</span>
+    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
+        <span class="n">total</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+
+    <span class="n">query</span> <span class="o">=</span> <span class="s2">&quot;SELECT type, origin, message, stack, date FROM logs&quot;</span>
+    <span class="n">parameters</span> <span class="o">=</span> <span class="p">[]</span>
+    <span class="k">if</span> <span class="n">start_date</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="n">end_date</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot; AND CAST(date AS DATE) between </span><span class="si">%s</span><span class="s2"> and </span><span class="si">%s</span><span class="s2">&quot;</span>
+        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">start_date</span><span class="p">)</span>
+        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">end_date</span><span class="p">)</span>       
+    <span class="n">query</span><span class="o">+=</span> <span class="s2">&quot; ORDER BY date DESC&quot;</span>
+    <span class="k">if</span> <span class="n">useLimit</span><span class="p">:</span>
+        <span class="n">query</span><span class="o">+=</span> <span class="s2">&quot; LIMIT </span><span class="si">%s</span><span class="s2"> OFFSET </span><span class="si">%s</span><span class="s2">&quot;</span>
+        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">limit</span><span class="p">)</span>
+        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">start</span><span class="p">)</span>
+
+    <span class="n">rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">query</span><span class="p">,</span> <span class="n">parameters</span><span class="p">)</span>        
+    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
+        <span class="n">log</span> <span class="o">=</span> <span class="p">{}</span>
+        <span class="n">log</span><span class="p">[</span><span class="s2">&quot;type&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+        <span class="n">log</span><span class="p">[</span><span class="s2">&quot;origin&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
+        <span class="n">log</span><span class="p">[</span><span class="s2">&quot;message&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span>
+        <span class="n">log</span><span class="p">[</span><span class="s2">&quot;stack&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">3</span><span class="p">]</span>
+        <span class="n">log</span><span class="p">[</span><span class="s2">&quot;date&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">4</span><span class="p">]</span>
+        <span class="n">logs</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">log</span><span class="p">)</span>
+
+    <span class="k">return</span> <span class="p">{</span><span class="s1">&#39;total&#39;</span> <span class="p">:</span> <span class="n">total</span><span class="p">,</span> <span class="s1">&#39;logs&#39;</span> <span class="p">:</span> <span class="n">logs</span><span class="p">}</span>
+</code></pre></div>
+</details>
+<details class="note"><summary>Alpha query approach</summary><div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
+<span class="n">DB</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">DB</span>
+<span class="k">def</span> <span class="nf">get_logs</span><span class="p">(</span>
+    <span class="n">start_date</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+    <span class="n">end_date</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
+    <span class="n">limit</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
+    <span class="n">page</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">,</span>
+    <span class="n">per_page</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">100</span><span class="p">,</span>
+<span class="p">):</span>
+    <span class="k">return</span> <span class="n">DB</span><span class="o">.</span><span class="n">select</span><span class="p">(</span>
+        <span class="n">Logs</span><span class="p">,</span>
+        <span class="n">optional_filters</span><span class="o">=</span><span class="p">[</span>
+            <span class="p">{</span><span class="n">Logs</span><span class="o">.</span><span class="n">update_date</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;&gt;&quot;</span><span class="p">:</span> <span class="n">start_date</span><span class="p">}},</span>
+            <span class="p">{</span><span class="n">Logs</span><span class="o">.</span><span class="n">update_date</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;&lt;&quot;</span><span class="p">:</span> <span class="n">end_date</span><span class="p">}},</span>
+        <span class="p">],</span>
+        <span class="n">page</span><span class="o">=</span><span class="n">page</span><span class="p">,</span>
+        <span class="n">per_page</span><span class="o">=</span><span class="n">per_page</span><span class="p">,</span>
+        <span class="n">limit</span><span class="o">=</span><span class="n">limit</span><span class="p">,</span>
+        <span class="n">order_by</span><span class="o">=</span><span class="n">Logs</span><span class="o">.</span><span class="n">update_date</span><span class="o">.</span><span class="n">desc</span><span class="p">(),</span>
+    <span class="p">)</span>
 </code></pre></div>
+</details>
+<h2 id="backend-alphaz">Backend: Alphaz</h2>
+<ul>
+<li>
+<p>Alphaz is a backend toolbox/framework based on a combination between Flask, SqlAlchemy and a multitude of other libraries.</p>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
-<p>set <code>ALPHA_CONF</code> environment parameter is you want to set the environment.</p>
+<p>The overriding goal for Alphaz is to ease the backend development and easely link python backend to Angular frontend [Alphaa].</p>
 </div>
-<p>Verify the deployment by navigating to your server address in your preferred browser:</p>
-<div class="highlight"><pre><span></span><code><span class="m">127</span>.0.0.1:&lt;port&gt;
-</code></pre></div>
-<h2 id="how-to-use">How to use</h2>
-<p>Your could import it using simply from the <strong>utils</strong>:</p>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.utils.api</span> <span class="kn">import</span> <span class="n">api</span>
-</code></pre></div>
-<p>or from the <strong>core</strong> if you are using it</p>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span><span class="p">,</span> <span class="n">API</span>
-</code></pre></div>
-<blockquote>
-<p><strong>api</strong> / <strong>API</strong> is the equivalent for <strong>app</strong> in <strong>Flask</strong> framework.</p>
-</blockquote>
-<h3 id="routes">Routes</h3>
-<p>We recommend to add all the route definition in <strong>apis/routes</strong> folder and import all the route definition in <strong>apis/routes/<strong>init</strong>.py</strong>.</p>
-<p>Then you will have to import the route in thoe <strong>core.py</strong> file:</p>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.models.main</span> <span class="kn">import</span> <span class="n">AlphaCore</span><span class="p">,</span> <span class="n">singleton</span>
-
-<span class="nd">@singleton</span>
-<span class="k">class</span> <span class="nc">Core</span><span class="p">(</span><span class="n">AlphaCore</span><span class="p">):</span>
-
-    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span><span class="n">file</span><span class="p">:</span><span class="nb">str</span><span class="p">):</span>
-
-        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="fm">__init__</span><span class="p">(</span><span class="n">file</span><span class="p">)</span>
-
-<span class="n">core</span> <span class="o">=</span> <span class="n">Core</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span>
-<span class="n">DB</span><span class="p">,</span> <span class="n">API</span><span class="p">,</span> <span class="n">LOG</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">api</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">log</span> <span class="c1"># not required but recommanded</span>
-
-<span class="kn">from</span> <span class="nn">apis.routes</span> <span class="kn">import</span> <span class="o">*</span>
-</code></pre></div>
-<h2 id="configuration">Configuration</h2>
-<p>The api is automatically configured from the <code>api.jon</code> file. See <a href="../configuration/">Configuration</a> for further details on how to use it.</p>
-<h3 id="main">Main</h3>
-<ul>
-<li>workers: In order to specify the numbers of workers</li>
-</ul>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;workers&quot;</span><span class="p">:</span> <span class="mi">6</span>
-</code></pre></div>
-<ul>
-<li>routes_no_log: In order to specify the routes where log must be ignored</li>
-</ul>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;routes_no_log&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;//status&quot;</span><span class="p">,</span> <span class="s2">&quot;//static&quot;</span><span class="p">,</span> <span class="s2">&quot;//dashboard&quot;</span><span class="p">],</span>
-</code></pre></div>
-<ul>
-<li>models: In order to specify the <strong>Flask-SqlAlchemy</strong> models definitions paths</li>
-</ul>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;models&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;models.databases&quot;</span><span class="p">]</span>
-</code></pre></div>
-<ul>
-<li>routes: In order to specify the routes definitions paths</li>
-</ul>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;routes&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;apis.routes&quot;</span><span class="p">]</span>
-</code></pre></div>
-<ul>
-<li>ssl: In order to activate ssl mode</li>
-</ul>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;ssl&quot;</span><span class="p">:</span> <span class="kc">false</span>
-</code></pre></div>
-<ul>
-<li>threaded: In order to activate the threaded mode</li>
+</li>
 </ul>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;threaded&quot;</span><span class="p">:</span> <span class="kc">false</span>
-</code></pre></div>
+<h2 id="features">Features</h2>
 <ul>
-<li>config: In order to activate pass configuration to Flask <strong>api</strong> class</li>
+<li>API Routing parameters management upgrade</li>
+<li>Enhanced json files configuration</li>
 </ul>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;config&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;MYSQL_DATABASE_CHARSET&quot;</span><span class="p">:</span> <span class="s2">&quot;utf8mb4&quot;</span><span class="p">,</span>
-    <span class="nt">&quot;SQLALCHEMY_TRACK_MODIFICATIONS&quot;</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
-    <span class="nt">&quot;SQLALCHEMY_POOL_RECYCLE&quot;</span><span class="p">:</span> <span class="mi">299</span><span class="p">,</span>
-    <span class="nt">&quot;SQLALCHEMY_POOL_TIMEOUT&quot;</span><span class="p">:</span> <span class="mi">30</span><span class="p">,</span>
-    <span class="nt">&quot;SQLALCHEMY_POOL_SIZE&quot;</span><span class="p">:</span> <span class="mi">10</span><span class="p">,</span>
-    <span class="nt">&quot;JWT_SECRET_KEY&quot;</span><span class="p">:</span> <span class="s2">&quot;a_secret_key&quot;</span><span class="p">,</span>
-    <span class="nt">&quot;JSON_SORT_KEYS&quot;</span><span class="p">:</span> <span class="kc">false</span>
-<span class="p">}</span>
-</code></pre></div>
-<h3 id="mails">Mails</h3>
-<p>In order to specify the mails configurations</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;mails&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;mail_server&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;host&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;mail&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;password&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;port&quot;</span><span class="p">:</span> <span class="mi">465</span><span class="p">,</span>
-        <span class="nt">&quot;server&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;ssl&quot;</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
-        <span class="nt">&quot;tls&quot;</span><span class="p">:</span> <span class="kc">false</span>
-    <span class="p">}</span>
-<span class="p">}</span>
-</code></pre></div>
-<h3 id="auth">Auth</h3>
-<p>In order to specify the auth mode</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;auth&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;mode&quot;</span><span class="p">:</span> <span class="s2">&quot;ldap&quot;</span><span class="p">,</span>
-    <span class="nt">&quot;ldap&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;server&quot;</span><span class="p">:</span> <span class="s2">&quot;ldap://path_to_ldap&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;baseDN&quot;</span><span class="p">:</span> <span class="s2">&quot;ou=people,dc=a_name,dc=com&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;users_filters&quot;</span><span class="p">:</span> <span class="s2">&quot;(|(uid={uid})(mail={mail})(cn={cn}))&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;user_filters&quot;</span><span class="p">:</span> <span class="s2">&quot;(|(uid={username})(mail={username})(cn={username}))&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;user_data&quot;</span><span class="p">:</span> <span class="p">{</span>
-            <span class="nt">&quot;givenName&quot;</span><span class="p">:</span> <span class="s2">&quot;name&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;sn&quot;</span><span class="p">:</span> <span class="s2">&quot;lastname&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;c&quot;</span><span class="p">:</span> <span class="s2">&quot;area&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;st-locationdescription&quot;</span><span class="p">:</span> <span class="s2">&quot;location&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;st-seatnumber&quot;</span><span class="p">:</span> <span class="s2">&quot;seat&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;telephoneNumber&quot;</span><span class="p">:</span> <span class="s2">&quot;phone-number&quot;</span>
-        <span class="p">}</span>
-    <span class="p">},</span>
-    <span class="nt">&quot;users&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;a_user_name&quot;</span><span class="p">:</span> <span class="p">{</span>
-            <span class="nt">&quot;user_permissions&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;SUPER_USER&quot;</span><span class="p">]</span>
-        <span class="p">}</span>
-    <span class="p">}</span>
-<span class="p">},</span>
-</code></pre></div>
-<h3 id="reloader-type">Reloader type</h3>
-<p>In order to specify the <a href="https://werkzeug.palletsprojects.com/en/2.1.x/">Werkzeug</a> reloader type</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;reloader_type&quot;</span><span class="p">:</span> <span class="s2">&quot;stat&quot;</span>
-</code></pre></div>
-<h3 id="admin">Admin</h3>
-<p>In order to specify the admins configurations</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;admins&quot;</span><span class="p">:</span> <span class="p">{</span><span class="nt">&quot;ips&quot;</span><span class="p">:[</span><span class="s2">&quot;127.0.0.1&quot;</span><span class="p">],</span> <span class="nt">&quot;password&quot;</span><span class="p">:</span><span class="s2">&quot;a_password&quot;</span><span class="p">},</span>
-</code></pre></div>
-<h3 id="dashboard">Dashboard</h3>
-<p>In order to configure the <a href="https://flask-monitoringdashboard.readthedocs.io/">Flask-Monitoring Dashboard</a></p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;dashboard&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;dashboard&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;APP_VERSION&quot;</span><span class="p">:</span> <span class="mf">1.0</span><span class="p">,</span>
-        <span class="nt">&quot;SAMPLING_PERIOD&quot;</span><span class="p">:</span> <span class="mi">20</span><span class="p">,</span>
-        <span class="nt">&quot;ENABLE_LOGGING&quot;</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
-        <span class="nt">&quot;active&quot;</span><span class="p">:</span> <span class="kc">false</span>
-    <span class="p">},</span>
-    <span class="nt">&quot;authentication&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;USERNAME&quot;</span><span class="p">:</span> <span class="s2">&quot;username&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;PASSWORD&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;GUEST_USERNAME&quot;</span><span class="p">:</span> <span class="s2">&quot;guest&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;GUEST_PASSWORD&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;guest1&quot;</span><span class="p">,</span> <span class="s2">&quot;guest2&quot;</span><span class="p">],</span>
-        <span class="nt">&quot;SECURITY_TOKEN&quot;</span><span class="p">:</span> <span class="s2">&quot;a_security_token&quot;</span>
-    <span class="p">},</span>
-    <span class="nt">&quot;database&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;DATABASE&quot;</span><span class="p">:</span> <span class="s2">&quot;sqlite:///{{root}}/dashboard.db&quot;</span>
-    <span class="p">}</span>
-<span class="p">}</span>
-</code></pre></div>
-<h2 id="routes_1">Routes</h2>
-<h3 id="basic">Basic</h3>
-<p>To specify an api route, juste use the <code>route</code> flag:</p>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.utils.api</span> <span class="kn">import</span> <span class="n">route</span><span class="p">,</span> <span class="n">api</span><span class="p">,</span> <span class="n">Parameter</span>
-
-<span class="nd">@route</span><span class="p">(</span><span class="s2">&quot;route_name&quot;</span><span class="p">)</span>
-<span class="k">def</span> <span class="nf">method_name</span><span class="p">():</span>
-    <span class="k">return</span> <span class="s2">&quot;hello&quot;</span>
-</code></pre></div>
-<p>Method automatically convert the output to the right format. Default format is <code>json</code></p>
-<h3 id="description">Description</h3>
-<p>A description could be specified:</p>
-<div class="highlight"><pre><span></span><code><span class="nd">@route</span><span class="p">(</span><span class="s2">&quot;route_name&quot;</span><span class="p">,</span> <span class="n">description</span><span class="o">=</span><span class="s2">&quot;This route say hello&quot;</span><span class="p">)</span>
-<span class="k">def</span> <span class="nf">method_name</span><span class="p">():</span>
-    <span class="k">return</span> <span class="s2">&quot;hello&quot;</span>
-</code></pre></div>
-<h3 id="category">Category</h3>
-<p>The routes are organized by <code>category</code>, by default the route category is defined by it <strong>file name</strong>, but it could be specified using the <code>cat</code> parameter:</p>
-<div class="highlight"><pre><span></span><code><span class="nd">@route</span><span class="p">(</span><span class="s2">&quot;route_name&quot;</span><span class="p">,</span> <span class="n">category</span><span class="o">=</span><span class="s2">&quot;politeness&quot;</span><span class="p">)</span>
-<span class="k">def</span> <span class="nf">method_name</span><span class="p">():</span>
-    <span class="k">return</span> <span class="s2">&quot;hello&quot;</span>
-</code></pre></div>
-<h2 id="parameters">Parameters</h2>
-<h3 id="simple">Simple</h3>
-<p>You could simply define parameters by listing all parameters in <code>parameters</code> list:</p>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.utils.api</span> <span class="kn">import</span> <span class="n">route</span><span class="p">,</span> <span class="n">api</span><span class="p">,</span> <span class="n">Parameter</span>
-
-<span class="nd">@route</span><span class="p">(</span><span class="s2">&quot;books&quot;</span><span class="p">,</span> <span class="n">parameters</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;name&quot;</span><span class="p">])</span>
-<span class="k">def</span> <span class="nf">method_name</span><span class="p">():</span>
-    <span class="k">return</span> <span class="s2">&quot;Book name is </span><span class="si">%s</span><span class="s2"> or </span><span class="si">%s</span><span class="s2">&quot;</span><span class="o">%</span><span class="p">(</span><span class="n">api</span><span class="p">[</span><span class="s2">&quot;name&quot;</span><span class="p">],</span> <span class="n">api</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;name&quot;</span><span class="p">,</span><span class="n">default</span><span class="o">=</span><span class="s2">&quot;&quot;</span><span class="p">))</span>
-</code></pre></div>
-<p>Parameter value is accessed by <code>api</code> instance, using <code>get</code> method, they could also be accessed using <code>get_parameters</code> method from <code>api</code> instance.</p>
-<h3 id="object">Object</h3>
-<p>Or you could use the <code>Parameter</code> class to specify properties such as:</p>
+<h2 id="tech">Tech</h2>
+<p>Alphaz uses a number of open source projects to work properly:</p>
 <ul>
-<li><strong>ptype</strong>: value type int, str, bool, <code>SqlAlchemy model</code></li>
-<li>parameter is <code>automatically converted</code> to the specified type</li>
-<li>if conversion failed an <code>exception</code> is raised</li>
-<li><strong>required</strong>: the parameter is required or not</li>
-<li><strong>default</strong>: default parameter value</li>
-<li><strong>options</strong>: authorized values</li>
-<li><strong>mode</strong>: input mode</li>
-<li><strong>cacheable</strong>: parameter is taken into acount in the caching system or not</li>
-<li><strong>private</strong>: parameter is hiden from documentation or not</li>
+<li><a href="https://flask.palletsprojects.com/en/1.1.x/">Flask</a> - a micro web framework</li>
+<li><a href="https://www.sqlalchemy.org/">SqlAlchemy</a> - a database toolkit</li>
+<li><a href="https://flask-sqlalchemy.palletsprojects.com/en/2.x/">Flask-SqlAlchemy</a> - an extension for Flask that adds support for SQLAlchemy</li>
 </ul>
-<div class="highlight"><pre><span></span><code><span class="nd">@route</span><span class="p">(</span><span class="s2">&quot;/logs&quot;</span><span class="p">,</span>
-    <span class="n">parameters</span> <span class="o">=</span> <span class="p">[</span>
-        <span class="n">Parameter</span><span class="p">(</span><span class="s1">&#39;page&#39;</span><span class="p">,</span><span class="n">required</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span><span class="n">ptype</span><span class="o">=</span><span class="nb">int</span><span class="p">),</span>
-        <span class="n">Parameter</span><span class="p">(</span><span class="s1">&#39;startDate&#39;</span><span class="p">,</span><span class="n">required</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span>
-        <span class="n">Parameter</span><span class="p">(</span><span class="s1">&#39;endDate&#39;</span><span class="p">,</span><span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">),</span>
-        <span class="n">Parameter</span><span class="p">(</span><span class="s1">&#39;error&#39;</span><span class="p">,</span> <span class="n">options</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;Y&quot;</span><span class="p">,</span><span class="s2">&quot;N&quot;</span><span class="p">])</span>
-    <span class="p">])</span>
-<span class="k">def</span> <span class="nf">admin_logs</span><span class="p">():</span>
-    <span class="k">return</span> <span class="n">get_logs</span><span class="p">(</span><span class="o">**</span><span class="n">api</span><span class="o">.</span><span class="n">get_parameters</span><span class="p">())</span>
-</code></pre></div>
-<blockquote>
-<p>Promote this method as it allows a better control on parameters</p>
-</blockquote>
-<h3 id="default-parameters">Default parameters</h3>
-<p>Some parameter are always available:
-- <strong>no_log</strong> (bool): disable logs for this route
-- <strong>reset_cache</strong> (bool): reset cache before calling this route
-- <strong>requester</strong> (str): requester to this route
-- <strong>format</strong> (str): output format
-    - json: 
-    - xml:
-- <strong>admin</strong> (str): admin password
-- <strong>admin_user_id</strong> (int): id of the user to connect has an admin </p>
-<h2 id="sqlalchemy-model">SqlAlchemy model</h2>
-<p>If you specify a <code>SqlAlchemy model</code> as a type it will be automatically converted to the specified model.</p>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
-<span class="n">db</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span>
-
-<span class="k">class</span> <span class="nc">Logs</span><span class="p">(</span><span class="n">db</span><span class="o">.</span><span class="n">Model</span><span class="p">,</span> <span class="n">AlphaTable</span><span class="p">):</span>
-    <span class="n">__tablename__</span> <span class="o">=</span> <span class="s1">&#39;LOGS&#39;</span>
-
-    <span class="nb">id</span>                       <span class="o">=</span> <span class="n">AlphaColumn</span><span class="p">(</span><span class="n">Integer</span><span class="p">,</span><span class="n">nullable</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span><span class="n">primary_key</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-    <span class="n">name</span>                     <span class="o">=</span> <span class="n">AlphaColumn</span><span class="p">(</span><span class="n">String</span><span class="p">,</span><span class="n">nullable</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-
-<span class="nd">@route</span><span class="p">(</span><span class="s2">&quot;logs&quot;</span><span class="p">,</span>
-    <span class="n">parameters</span> <span class="o">=</span> <span class="p">[</span>
-        <span class="n">Parameter</span><span class="p">(</span><span class="s1">&#39;log&#39;</span><span class="p">,</span><span class="n">ptype</span><span class="o">=</span><span class="n">Logs</span><span class="p">)</span>
-    <span class="p">])</span>
-<span class="k">def</span> <span class="nf">admin_logs</span><span class="p">():</span>
-    <span class="n">db</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">api</span><span class="p">[</span><span class="s1">&#39;log&#39;</span><span class="p">])</span>
-</code></pre></div>
-<h2 id="methods">Methods</h2>
-<p>Methods are specified the same way as in <code>Flask</code>, using <code>methods</code> parameter:</p>
-<div class="highlight"><pre><span></span><code><span class="nd">@route</span><span class="p">(</span><span class="s1">&#39;logs&#39;</span><span class="p">,</span> <span class="n">methods</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;GET&quot;</span><span class="p">])</span>
-<span class="k">def</span> <span class="nf">get_logs</span><span class="p">():</span>
-    <span class="k">return</span> <span class="n">db</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="n">Logs</span><span class="p">)</span>
-
-<span class="nd">@route</span><span class="p">(</span><span class="s1">&#39;logs&#39;</span><span class="p">,</span> <span class="n">methods</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;POST&quot;</span><span class="p">])</span>
-<span class="k">def</span> <span class="nf">set_logs</span><span class="p">():</span>
-    <span class="k">return</span> <span class="n">db</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">Logs</span><span class="p">)</span>
-</code></pre></div>
-<p>Methods can be managed using <code>different routes</code> or within <code>a single route</code>:</p>
-<div class="highlight"><pre><span></span><code><span class="nd">@route</span><span class="p">(</span><span class="s1">&#39;logs&#39;</span><span class="p">,</span> <span class="n">methods</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;GET&quot;</span><span class="p">,</span> <span class="s2">&quot;POST&quot;</span><span class="p">,</span> <span class="s2">&quot;DELETE&quot;</span><span class="p">])</span>
-<span class="k">def</span> <span class="nf">get_logs</span><span class="p">():</span>
-    <span class="k">if</span> <span class="n">api</span><span class="o">.</span><span class="n">is_get</span><span class="p">():</span>
-        <span class="k">return</span> <span class="n">db</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="n">Logs</span><span class="p">)</span>
-    <span class="k">elif</span> <span class="n">api</span><span class="o">.</span><span class="n">is_post</span><span class="p">():</span>
-        <span class="k">return</span> <span class="n">db</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">Logs</span><span class="p">)</span>
-    <span class="k">elif</span> <span class="n">api</span><span class="o">.</span><span class="n">is_delete</span><span class="p">():</span>
-        <span class="k">return</span> <span class="n">db</span><span class="o">.</span><span class="n">delete</span><span class="p">(</span><span class="n">Logs</span><span class="p">)</span>
-</code></pre></div>
-<h2 id="authorizations">Authorizations</h2>
-<p>Route can be protected using the login system or admin rights.</p>
-<h3 id="login-system">Login system</h3>
-<p>To protect a route using the login system you must specify: <code>logged=True</code></p>
-<div class="highlight"><pre><span></span><code><span class="nd">@route</span><span class="p">(</span><span class="s1">&#39;protected&#39;</span><span class="p">,</span> <span class="n">logged</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-<span class="k">def</span> <span class="nf">protected_route</span><span class="p">():</span>
-    <span class="n">user</span> <span class="o">=</span> <span class="n">api</span><span class="o">.</span><span class="n">get_logged_user</span><span class="p">()</span>
-    <span class="k">return</span> <span class="n">user</span>
-</code></pre></div>
-<p>User information can be accessed using <em>get_logged_user</em> method.</p>
-<h2 id="cache">Cache</h2>
-<p>A cache system is implemented, in order to use it you must specify the</p>
-<h2 id="admin_1">Admin</h2>
-<p>Admin could auto log to any user account on local mode</p>
-<h3 id="condition">Condition</h3>
-<p>To be an admin a user must have at least one condition:</p>
+<h2 id="project-layout">Project layout</h2>
 <ul>
-<li>a <strong>role</strong> &gt; 9</li>
-<li>specify the magic password has <strong>admin</strong> API parameter</li>
-<li>connect using an admin ip. The ips admin list must be defined in the <strong>api.json</strong> configuration files under the <strong>key</strong>=<strong>admins_ips</strong></li>
+<li>How to setup <code>Alpha</code>: <a href="alpha_setup/">Alpha</a></li>
 </ul>
-<h3 id="how-to-use_1">How to use</h3>
-<p>If you met one of the admin condition you do not need any password in order to log has any of the user in the database.</p>
-<p>You could be logged for specific routes using the <strong>single route mode</strong> or to any route using the <strong>login/logout</strong> system.</p>
-<h4 id="single-route-mode">Single route mode</h4>
+<h2 id="frontend-alphaa">Frontend: Alphaa</h2>
 <ul>
-<li>You could specifiy either admin_user_id={user_id} or admin_user_name={username} directly into any request in order to login with this user for this specific route.</li>
-</ul>
+<li>
+<p>Alphaa is a frontend toolbox/framework</p>
 <div class="admonition note">
-<p class="admonition-title">Exemple</p>
-<p>/anyroute?admin_user_id=1000</p>
+<p class="admonition-title">Note</p>
+<p>The overriding goal for Alphaa is to ease the frontend development and easely link Angular frontend to python backend [Alphaz].</p>
 </div>
-<h4 id="login-to-the-api">Login to the api</h4>
-<p>Use the route <strong>/auth/su</strong> in order to set an admin session that is valid until the end of the api runtime.</p>
+<h2 id="features_1">Features</h2>
+</li>
+<li>
+<p>Enhanced services</p>
+</li>
+<li>Master class</li>
+</ul>
+<h2 id="project-layout_1">Project layout</h2>
 <ul>
-<li>You must specifiy either admin_user_id={user_id} or admin_user_name={username}</li>
+<li>How to setup <code>Alpha</code>: <a href="alpha_setup/">Alpha</a></li>
 </ul>
-<div class="admonition note">
-<p class="admonition-title">Exemple</p>
-<p>/auth/su?admin_user_id=1000</p>
-</div>
-<h4 id="logout-from-the-api">Logout from the api</h4>
-<p>Use the route <strong>/logout/su</strong> in order to logout.</p>
-<h2 id="issues">Issues</h2>
-<blockquote>
-<p>In progress</p>
-</blockquote>
-<h3 id="database-alias">Database alias</h3>
-<blockquote>
-<p>In progress</p>
-</blockquote>
                 
               
               
                 
 
 
               
@@ -1234,36 +853,22 @@
       </main>
       
         
 <footer class="md-footer">
   
     <nav class="md-footer__inner md-grid" aria-label="Footer">
       
-        <a href="../alpha_core/" class="md-footer__link md-footer__link--prev" rel="prev">
-          <div class="md-footer__button md-icon">
-            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12z"/></svg>
-          </div>
-          <div class="md-footer__title">
-            <div class="md-ellipsis">
-              <span class="md-footer__direction">
-                Previous
-              </span>
-              Core
-            </div>
-          </div>
-        </a>
-      
       
-        <a href="../alpha_screens/" class="md-footer__link md-footer__link--next" rel="next">
+        <a href="alpha_setup/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Next
               </span>
-              Screens
+              Setup
             </div>
           </div>
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4z"/></svg>
           </div>
         </a>
       
@@ -1284,15 +889,15 @@
   </div>
 </footer>
       
     </div>
     <div class="md-dialog" data-md-component="dialog">
       <div class="md-dialog__inner md-typeset"></div>
     </div>
-    <script id="__config" type="application/json">{"base": "..", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "../assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
+    <script id="__config" type="application/json">{"base": ".", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
     
     
-      <script src="../assets/javascripts/bundle.7353b375.min.js"></script>
+      <script src="assets/javascripts/bundle.7353b375.min.js"></script>
       
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -5,356 +5,159 @@
 
 
 
  ⁰ ⁰
 Skip_to_content
 
  Alpha Documentation
- Api
+ Home
 
 [query               ]
 Initializing search
 
    Alpha Documentation
-    * Home
+    * ⁰  Home   Home    Table of contents
+          o Purpose
+          o Backend:_Alphaz
+          o Features
+          o Tech
+          o Project_layout
+          o Frontend:_Alphaa
+          o Features
+          o Project_layout
     * Setup
     * Core
-    * ⁰  Api   Api    Table of contents
-          o Introduction
-          o Launch
-          o How_to_use
-                # Routes
+    * ⁰  Api      Api
+          o Main
           o Configuration
-                # Main
-                # Mails
-                # Auth
-                # Reloader_type
-                # Admin
-                # Dashboard
           o Routes
-                # Basic
-                # Description
-                # Category
           o Parameters
-                # Simple
-                # Object
-                # Default_parameters
-          o SqlAlchemy_model
+          o Model_Parameters
           o Methods
-          o Authorizations
-                # Login_system
           o Cache
-          o Admin
-                # Condition
-                # How_to_use
-                      # Single_route_mode
-                      # Login_to_the_api
-                      # Logout_from_the_api
+          o Authorizations
+          o SqlAlchemy
           o Issues
-                # Database_alias
     * Screens
     * Configuration
-    * Database
+    * ⁰  Database      Database
+          o Main
+          o Init
+          o Model
+          o Schema
+          o Instantiate
+          o Update
+          o Relations
+          o Model_Parameters
     * Documentation
     * Administration
    Table of contents
-    * Introduction
-    * Launch
-    * How_to_use
-          o Routes
-    * Configuration
-          o Main
-          o Mails
-          o Auth
-          o Reloader_type
-          o Admin
-          o Dashboard
-    * Routes
-          o Basic
-          o Description
-          o Category
-    * Parameters
-          o Simple
-          o Object
-          o Default_parameters
-    * SqlAlchemy_model
-    * Methods
-    * Authorizations
-          o Login_system
-    * Cache
-    * Admin
-          o Condition
-          o How_to_use
-                # Single_route_mode
-                # Login_to_the_api
-                # Logout_from_the_api
-    * Issues
-          o Database_alias
-****** Alpha API system ******
-***** Introduction *****
-The api system is completely based on Flask and compatible. You could use Flask
-inside Alpha system without any issue.
-***** Launch *****
-To start the api execute the api.py file
-python api.py
-Note
-set ALPHA_CONF environment parameter is you want to set the environment.
-Verify the deployment by navigating to your server address in your preferred
-browser:
-127.0.0.1:<port>
-***** How to use *****
-Your could import it using simply from the utils:
-from alphaz.utils.api import api
-or from the core if you are using it
-from core import core, API
-     api / API is the equivalent for app in Flask framework.
-**** Routes ****
-We recommend to add all the route definition in apis/routes folder and import
-all the route definition in apis/routes/init.py.
-Then you will have to import the route in thoe core.py file:
-from alphaz.models.main import AlphaCore, singleton
-
-@singleton
-class Core(AlphaCore):
-
-    def __init__(self,file:str):
-
-        super().__init__(file)
-
-core = Core(__file__)
-DB, API, LOG = core.db, core.api, core.log # not required but recommanded
-
-from apis.routes import *
-***** Configuration *****
-The api is automatically configured from the api.jon file. See Configuration
-for further details on how to use it.
-**** Main ****
-    * workers: In order to specify the numbers of workers
-"workers": 6
-    * routes_no_log: In order to specify the routes where log must be ignored
-"routes_no_log": ["//status", "//static", "//dashboard"],
-    * models: In order to specify the Flask-SqlAlchemy models definitions paths
-"models": ["models.databases"]
-    * routes: In order to specify the routes definitions paths
-"routes": ["apis.routes"]
-    * ssl: In order to activate ssl mode
-"ssl": false
-    * threaded: In order to activate the threaded mode
-"threaded": false
-    * config: In order to activate pass configuration to Flask api class
-"config": {
-    "MYSQL_DATABASE_CHARSET": "utf8mb4",
-    "SQLALCHEMY_TRACK_MODIFICATIONS": false,
-    "SQLALCHEMY_POOL_RECYCLE": 299,
-    "SQLALCHEMY_POOL_TIMEOUT": 30,
-    "SQLALCHEMY_POOL_SIZE": 10,
-    "JWT_SECRET_KEY": "a_secret_key",
-    "JSON_SORT_KEYS": false
-}
-**** Mails ****
-In order to specify the mails configurations
-"mails": {
-    "mail_server": {
-        "host": "",
-        "mail": "",
-        "password": "",
-        "port": 465,
-        "server": "",
-        "ssl": true,
-        "tls": false
-    }
-}
-**** Auth ****
-In order to specify the auth mode
-"auth": {
-    "mode": "ldap",
-    "ldap": {
-        "server": "ldap://path_to_ldap",
-        "baseDN": "ou=people,dc=a_name,dc=com",
-        "users_filters": "(|(uid={uid})(mail={mail})(cn={cn}))",
-        "user_filters": "(|(uid={username})(mail={username})(cn={username}))",
-        "user_data": {
-            "givenName": "name",
-            "sn": "lastname",
-            "c": "area",
-            "st-locationdescription": "location",
-            "st-seatnumber": "seat",
-            "telephoneNumber": "phone-number"
-        }
-    },
-    "users": {
-        "a_user_name": {
-            "user_permissions": ["SUPER_USER"]
-        }
-    }
-},
-**** Reloader type ****
-In order to specify the Werkzeug reloader type
-"reloader_type": "stat"
-**** Admin ****
-In order to specify the admins configurations
-"admins": {"ips":["127.0.0.1"], "password":"a_password"},
-**** Dashboard ****
-In order to configure the Flask-Monitoring_Dashboard
-"dashboard": {
-    "dashboard": {
-        "APP_VERSION": 1.0,
-        "SAMPLING_PERIOD": 20,
-        "ENABLE_LOGGING": true,
-        "active": false
-    },
-    "authentication": {
-        "USERNAME": "username",
-        "PASSWORD": "",
-        "GUEST_USERNAME": "guest",
-        "GUEST_PASSWORD": ["guest1", "guest2"],
-        "SECURITY_TOKEN": "a_security_token"
-    },
-    "database": {
-        "DATABASE": "sqlite:///{{root}}/dashboard.db"
-    }
-}
-***** Routes *****
-**** Basic ****
-To specify an api route, juste use the route flag:
-from alphaz.utils.api import route, api, Parameter
-
-@route("route_name")
-def method_name():
-    return "hello"
-Method automatically convert the output to the right format. Default format is
-json
-**** Description ****
-A description could be specified:
-@route("route_name", description="This route say hello")
-def method_name():
-    return "hello"
-**** Category ****
-The routes are organized by category, by default the route category is defined
-by it file name, but it could be specified using the cat parameter:
-@route("route_name", category="politeness")
-def method_name():
-    return "hello"
-***** Parameters *****
-**** Simple ****
-You could simply define parameters by listing all parameters in parameters
-list:
-from alphaz.utils.api import route, api, Parameter
-
-@route("books", parameters=["name"])
-def method_name():
-    return "Book name is %s or %s"%(api["name"], api.get("name",default=""))
-Parameter value is accessed by api instance, using get method, they could also
-be accessed using get_parameters method from api instance.
-**** Object ****
-Or you could use the Parameter class to specify properties such as:
-    * ptype: value type int, str, bool, SqlAlchemy model
-    * parameter is automatically converted to the specified type
-    * if conversion failed an exception is raised
-    * required: the parameter is required or not
-    * default: default parameter value
-    * options: authorized values
-    * mode: input mode
-    * cacheable: parameter is taken into acount in the caching system or not
-    * private: parameter is hiden from documentation or not
-@route("/logs",
-    parameters = [
-        Parameter('page',required=True,ptype=int),
-        Parameter('startDate',required=True),
-        Parameter('endDate',default=None),
-        Parameter('error', options=["Y","N"])
-    ])
-def admin_logs():
-    return get_logs(**api.get_parameters())
-     Promote this method as it allows a better control on parameters
-**** Default parameters ****
-Some parameter are always available: - no_log (bool): disable logs for this
-route - reset_cache (bool): reset cache before calling this route - requester
-(str): requester to this route - format (str): output format - json: - xml: -
-admin (str): admin password - admin_user_id (int): id of the user to connect
-has an admin
-***** SqlAlchemy model *****
-If you specify a SqlAlchemy model as a type it will be automatically converted
-to the specified model.
+    * Purpose
+    * Backend:_Alphaz
+    * Features
+    * Tech
+    * Project_layout
+    * Frontend:_Alphaa
+    * Features
+    * Project_layout
+****** Welcome to Alpha environment documention ******
+Alpha is an ecosystem based on a multiple frameworks and libraries for both
+frontend and backend.
+***** Purpose *****
+The purpose of the ecosystem is to simplify any dev activity.
+Standard query approach
 from core import core
-db = core.db
+DB = core.db
 
-class Logs(db.Model, AlphaTable):
-    __tablename__ = 'LOGS'
+def get_logs(start_date=None, end_date=None, useLimit=False, pageForLimit=1):
+    total = 0
+    logs = []
+    limit = 20
+    start = (pageForLimit - 1) * limit
+
+    query = "SELECT COUNT(*) AS count FROM logs"
+    parameters = []
+    if start_date is not None and end_date is not None:
+        query += " AND CAST(date AS DATE) between %s and %s"
+        parameters.append(start_date)
+        parameters.append(end_date)
+    query+= " ORDER BY date DESC"
+
+    rows = DB.get(query, parameters)
+    for row in rows:
+        total = row[0]
+
+    query = "SELECT type, origin, message, stack, date FROM logs"
+    parameters = []
+    if start_date is not None and end_date is not None:
+        query += " AND CAST(date AS DATE) between %s and %s"
+        parameters.append(start_date)
+        parameters.append(end_date)
+    query+= " ORDER BY date DESC"
+    if useLimit:
+        query+= " LIMIT %s OFFSET %s"
+        parameters.append(limit)
+        parameters.append(start)
+
+    rows = db.get(query, parameters)
+    for row in rows:
+        log = {}
+        log["type"] = row[0]
+        log["origin"] = row[1]
+        log["message"] = row[2]
+        log["stack"] = row[3]
+        log["date"] = row[4]
+        logs.append(log)
 
-    id                       = AlphaColumn
-(Integer,nullable=False,primary_key=True)
-    name                     = AlphaColumn(String,nullable=False)
-
-@route("logs",
-    parameters = [
-        Parameter('log',ptype=Logs)
-    ])
-def admin_logs():
-    db.add(api['log'])
-***** Methods *****
-Methods are specified the same way as in Flask, using methods parameter:
-@route('logs', methods=["GET"])
-def get_logs():
-    return db.select(Logs)
-
-@route('logs', methods=["POST"])
-def set_logs():
-    return db.add(Logs)
-Methods can be managed using different routes or within a single route:
-@route('logs', methods=["GET", "POST", "DELETE"])
-def get_logs():
-    if api.is_get():
-        return db.select(Logs)
-    elif api.is_post():
-        return db.add(Logs)
-    elif api.is_delete():
-        return db.delete(Logs)
-***** Authorizations *****
-Route can be protected using the login system or admin rights.
-**** Login system ****
-To protect a route using the login system you must specify: logged=True
-@route('protected', logged=True)
-def protected_route():
-    user = api.get_logged_user()
-    return user
-User information can be accessed using get_logged_user method.
-***** Cache *****
-A cache system is implemented, in order to use it you must specify the
-***** Admin *****
-Admin could auto log to any user account on local mode
-**** Condition ****
-To be an admin a user must have at least one condition:
-    * a role > 9
-    * specify the magic password has admin API parameter
-    * connect using an admin ip. The ips admin list must be defined in the
-      api.json configuration files under the key=admins_ips
-**** How to use ****
-If you met one of the admin condition you do not need any password in order to
-log has any of the user in the database.
-You could be logged for specific routes using the single route mode or to any
-route using the login/logout system.
-*** Single route mode ***
-    * You could specifiy either admin_user_id={user_id} or admin_user_name=
-      {username} directly into any request in order to login with this user for
-      this specific route.
-Exemple
-/anyroute?admin_user_id=1000
-*** Login to the api ***
-Use the route /auth/su in order to set an admin session that is valid until the
-end of the api runtime.
-    * You must specifiy either admin_user_id={user_id} or admin_user_name=
-      {username}
-Exemple
-/auth/su?admin_user_id=1000
-*** Logout from the api ***
-Use the route /logout/su in order to logout.
-***** Issues *****
-     In progress
-**** Database alias ****
-     In progress
-
- Previous__Core
+    return {'total' : total, 'logs' : logs}
+ Alpha query approach
+from core import core
+DB = core.DB
+def get_logs(
+    start_date: datetime = None,
+    end_date: datetime = None,
+    limit: int = False,
+    page: int = 0,
+    per_page: int = 100,
+):
+    return DB.select(
+        Logs,
+        optional_filters=[
+            {Logs.update_date: {">": start_date}},
+            {Logs.update_date: {"<": end_date}},
+        ],
+        page=page,
+        per_page=per_page,
+        limit=limit,
+        order_by=Logs.update_date.desc(),
+    )
+***** Backend: Alphaz *****
+    * Alphaz is a backend toolbox/framework based on a combination between
+      Flask, SqlAlchemy and a multitude of other libraries.
+      Note
+      The overriding goal for Alphaz is to ease the backend development and
+      easely link python backend to Angular frontend [Alphaa].
+***** Features *****
+    * API Routing parameters management upgrade
+    * Enhanced json files configuration
+***** Tech *****
+Alphaz uses a number of open source projects to work properly:
+    * Flask - a micro web framework
+    * SqlAlchemy - a database toolkit
+    * Flask-SqlAlchemy - an extension for Flask that adds support for
+      SQLAlchemy
+***** Project layout *****
+    * How to setup Alpha: Alpha
+***** Frontend: Alphaa *****
+    * Alphaa is a frontend toolbox/framework
+      Note
+      The overriding goal for Alphaa is to ease the frontend development and
+      easely link Angular frontend to python backend [Alphaz].
+      ***** Features *****
+    * Enhanced services
+    * Master class
+***** Project layout *****
+    * How to setup Alpha: Alpha
 
- Next__Screens
+ Next__Setup
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/alpha_core/index.html` & `alphaz-0.7.4/alphaz/documentations/site/database/instantiate/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width,initial-scale=1">
       
       
       
       
-      <link rel="icon" href="../assets/images/favicon.png">
+      <link rel="icon" href="../../assets/images/favicon.png">
       <meta name="generator" content="mkdocs-1.1.2, mkdocs-material-7.1.1">
     
     
       
-        <title>Core - Alpha Documentation</title>
+        <title>Instantiate - Alpha Documentation</title>
       
     
     
-      <link rel="stylesheet" href="../assets/stylesheets/main.9299cb39.min.css">
+      <link rel="stylesheet" href="../../assets/stylesheets/main.9299cb39.min.css">
       
         
-        <link rel="stylesheet" href="../assets/stylesheets/palette.ef6f36e2.min.css">
+        <link rel="stylesheet" href="../../assets/stylesheets/palette.ef6f36e2.min.css">
         
       
     
     
     
       
         
@@ -47,34 +47,29 @@
     
     
     
     
     <body dir="ltr" data-md-color-scheme="" data-md-color-primary="none" data-md-color-accent="none">
   
     
-    <script>function __prefix(e){return new URL("..",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
+    <script>function __prefix(e){return new URL("../..",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
     
     <input class="md-toggle" data-md-toggle="drawer" type="checkbox" id="__drawer" autocomplete="off">
     <input class="md-toggle" data-md-toggle="search" type="checkbox" id="__search" autocomplete="off">
     <label class="md-overlay" for="__drawer"></label>
     <div data-md-component="skip">
       
-        
-        <a href="#alpha-core-system" class="md-skip">
-          Skip to content
-        </a>
-      
     </div>
     <div data-md-component="announce">
       
     </div>
     
       <header class="md-header" data-md-component="header">
   <nav class="md-header__inner md-grid" aria-label="Header">
-    <a href=".." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="../.." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     <label class="md-header__button md-icon" for="__drawer">
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M3 6h18v2H3V6m0 5h18v2H3v-2m0 5h18v2H3v-2z"/></svg>
@@ -85,15 +80,15 @@
           <span class="md-ellipsis">
             Alpha Documentation
           </span>
         </div>
         <div class="md-header__topic" data-md-component="header-topic">
           <span class="md-ellipsis">
             
-              Core
+              Instantiate
             
           </span>
         </div>
       </div>
     </div>
     
     
@@ -146,15 +141,15 @@
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 
 
 <nav class="md-nav md-nav--primary" aria-label="Navigation" data-md-level="0">
   <label class="md-nav__title" for="__drawer">
-    <a href=".." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="../.." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     Alpha Documentation
   </label>
@@ -165,362 +160,433 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href=".." class="md-nav__link">
+      <a href="../.." class="md-nav__link">
         Home
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_setup/" class="md-nav__link">
+      <a href="../../alpha_setup/" class="md-nav__link">
         Setup
       </a>
     </li>
   
 
     
       
       
       
 
   
   
-    
   
+    <li class="md-nav__item">
+      <a href="../../alpha_core/" class="md-nav__link">
+        Core
+      </a>
+    </li>
   
-    <li class="md-nav__item md-nav__item--active">
+
+    
       
-      <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
       
-        
       
+
+  
+  
+  
+    
+    <li class="md-nav__item md-nav__item--nested">
+      
+      
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_4" type="checkbox" id="__nav_4" >
       
-        <label class="md-nav__link md-nav__link--active" for="__toc">
-          Core
+      <label class="md-nav__link" for="__nav_4">
+        Api
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Api" data-md-level="1">
+        <label class="md-nav__title" for="__nav_4">
           <span class="md-nav__icon md-icon"></span>
+          Api
         </label>
-      
-      <a href="./" class="md-nav__link md-nav__link--active">
-        Core
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/main/" class="md-nav__link">
+        Main
       </a>
-      
-        
-<nav class="md-nav md-nav--secondary" aria-label="Table of contents">
+    </li>
   
+
+          
+            
   
-    
   
   
-    <label class="md-nav__title" for="__toc">
-      <span class="md-nav__icon md-icon"></span>
-      Table of contents
-    </label>
-    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
-      
-        <li class="md-nav__item">
-  <a href="#purpose" class="md-nav__link">
-    Purpose
-  </a>
+    <li class="md-nav__item">
+      <a href="../../api/configuration/" class="md-nav__link">
+        Configuration
+      </a>
+    </li>
   
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#how-to-use" class="md-nav__link">
-    How to use
-  </a>
+
+          
+            
   
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#logging" class="md-nav__link">
-    Logging
-  </a>
   
-    <nav class="md-nav" aria-label="Logging">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#database" class="md-nav__link">
-    Database
-  </a>
   
-</li>
-        
-      </ul>
-    </nav>
+    <li class="md-nav__item">
+      <a href="../../api/routes/" class="md-nav__link">
+        Routes
+      </a>
+    </li>
   
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#api" class="md-nav__link">
-    API
-  </a>
+
+          
+            
   
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#configuration" class="md-nav__link">
-    Configuration
-  </a>
   
-</li>
-      
-    </ul>
   
-</nav>
-      
+    <li class="md-nav__item">
+      <a href="../../api/parameters/" class="md-nav__link">
+        Parameters
+      </a>
     </li>
   
 
-    
-      
-      
-      
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/methods/" class="md-nav__link">
+        Methods
+      </a>
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
-        Api
+      <a href="../../api/cache/" class="md-nav__link">
+        Cache
       </a>
     </li>
   
 
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/authorizations/" class="md-nav__link">
+        Authorizations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/sqlalchemy/" class="md-nav__link">
+        SqlAlchemy
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/issues/" class="md-nav__link">
+        Issues
+      </a>
+    </li>
+  
+
+          
+        </ul>
+      </nav>
+    </li>
+  
+
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_screens/" class="md-nav__link">
+      <a href="../../alpha_screens/" class="md-nav__link">
         Screens
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../configuration/" class="md-nav__link">
+      <a href="../../configuration/" class="md-nav__link">
         Configuration
       </a>
     </li>
   
 
     
       
       
       
 
   
   
+    
   
-    <li class="md-nav__item">
-      <a href="../alpha_database/" class="md-nav__link">
-        Database
-      </a>
-    </li>
   
-
     
+    <li class="md-nav__item md-nav__item--active md-nav__item--nested">
       
       
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_7" type="checkbox" id="__nav_7" checked>
       
+      <label class="md-nav__link" for="__nav_7">
+        Database
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Database" data-md-level="1">
+        <label class="md-nav__title" for="__nav_7">
+          <span class="md-nav__icon md-icon"></span>
+          Database
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../main/" class="md-nav__link">
+        Main
+      </a>
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="../documentation/" class="md-nav__link">
-        Documentation
+      <a href="../init/" class="md-nav__link">
+        Init
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../model/" class="md-nav__link">
+        Model
       </a>
     </li>
   
 
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../schema/" class="md-nav__link">
+        Schema
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
     
+  
+  
+    <li class="md-nav__item md-nav__item--active">
+      
+      <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
       
       
+      <a href="./" class="md-nav__link md-nav__link--active">
+        Instantiate
+      </a>
       
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_admin/" class="md-nav__link">
-        Administration
+      <a href="../update/" class="md-nav__link">
+        Update
       </a>
     </li>
   
 
-    
-  </ul>
-</nav>
-                  </div>
-                </div>
-              </div>
+          
             
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../relations/" class="md-nav__link">
+        Relations
+      </a>
+    </li>
+  
+
+          
             
-              
-              <div class="md-sidebar md-sidebar--secondary" data-md-component="sidebar" data-md-type="toc" >
-                <div class="md-sidebar__scrollwrap">
-                  <div class="md-sidebar__inner">
-                    
-<nav class="md-nav md-nav--secondary" aria-label="Table of contents">
   
   
-    
   
+    <li class="md-nav__item">
+      <a href="../../api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
   
-    <label class="md-nav__title" for="__toc">
-      <span class="md-nav__icon md-icon"></span>
-      Table of contents
-    </label>
-    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
-      
-        <li class="md-nav__item">
-  <a href="#purpose" class="md-nav__link">
-    Purpose
-  </a>
+
+          
+        </ul>
+      </nav>
+    </li>
   
-</li>
+
+    
       
-        <li class="md-nav__item">
-  <a href="#how-to-use" class="md-nav__link">
-    How to use
-  </a>
-  
-</li>
       
-        <li class="md-nav__item">
-  <a href="#logging" class="md-nav__link">
-    Logging
-  </a>
+      
+
   
-    <nav class="md-nav" aria-label="Logging">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#database" class="md-nav__link">
-    Database
-  </a>
   
-</li>
-        
-      </ul>
-    </nav>
   
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#api" class="md-nav__link">
-    API
-  </a>
+    <li class="md-nav__item">
+      <a href="../../documentation/" class="md-nav__link">
+        Documentation
+      </a>
+    </li>
   
-</li>
+
+    
       
-        <li class="md-nav__item">
-  <a href="#configuration" class="md-nav__link">
-    Configuration
-  </a>
-  
-</li>
       
-    </ul>
+      
+
+  
+  
   
+    <li class="md-nav__item">
+      <a href="../../alpha_admin/" class="md-nav__link">
+        Administration
+      </a>
+    </li>
+  
+
+    
+  </ul>
 </nav>
                   </div>
                 </div>
               </div>
             
+            
           
           <div class="md-content" data-md-component="content">
             <article class="md-content__inner md-typeset">
               
                 
                 
-                <h1 id="alpha-core-system">Alpha core system</h1>
-<h2 id="purpose">Purpose</h2>
-<p>The <strong>core</strong> is used as a central point to manage various system:</p>
-<ul>
-<li><a href="## Logging">logging system</a></li>
-<li><a href="## Database">database access</a></li>
-<li><a href="## API">api system</a></li>
-<li><a href="## Configuration">dynamic configuration</a></li>
-</ul>
-<h2 id="how-to-use">How to use</h2>
-<p>You could:</p>
-<ul>
-<li>
-<p>Use the <strong>alphaz</strong> core and initiate it at the start of you project preferably in a file named <strong>core.py</strong> to be complient with this documentation:</p>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.models.main</span> <span class="kn">import</span> <span class="n">AlphaCore</span>
-
-<span class="n">core</span> <span class="o">=</span> <span class="n">AlphaCore</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span>
-<span class="n">DB</span><span class="p">,</span> <span class="n">API</span><span class="p">,</span> <span class="n">LOG</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">api</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">log</span> <span class="c1"># not required but recommanded</span>
-</code></pre></div>
-</li>
-<li>
-<p>Or create a <strong>core.py</strong> file at the <strong>root</strong> of your project containing at least:</p>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.models.main</span> <span class="kn">import</span> <span class="n">AlphaCore</span><span class="p">,</span> <span class="n">singleton</span>
-
-<span class="nd">@singleton</span>
-<span class="k">class</span> <span class="nc">Core</span><span class="p">(</span><span class="n">AlphaCore</span><span class="p">):</span>
-
-    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span><span class="n">file</span><span class="p">:</span><span class="nb">str</span><span class="p">):</span>
-
-        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="fm">__init__</span><span class="p">(</span><span class="n">file</span><span class="p">)</span>
-
-<span class="n">core</span> <span class="o">=</span> <span class="n">Core</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span>
-<span class="n">DB</span><span class="p">,</span> <span class="n">API</span><span class="p">,</span> <span class="n">LOG</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">api</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">log</span> <span class="c1"># not required but recommanded</span>
-</code></pre></div>
-</li>
-</ul>
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>This is the recommended way, so that you could custom the Core class</p>
-</div>
-<h2 id="logging">Logging</h2>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
-<span class="n">LOG</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">get_logger</span><span class="p">(</span><span class="s1">&#39;name&#39;</span><span class="p">)</span>
-<span class="n">LOG</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="s1">&#39;message&#39;</span><span class="p">)</span>
-</code></pre></div>
-<h3 id="database">Database</h3>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
-<span class="n">DB</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span>
+                  <h1>Instantiate</h1>
+                
+                <p>This enable the use of model columns which is not possible using SqlAlchemy:</p>
+<div class="highlight"><pre><span></span><code><span class="n">attr</span> <span class="o">=</span> <span class="p">{</span>
+    <span class="n">Duck</span><span class="o">.</span><span class="n">name</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span>
+    <span class="n">Duck</span><span class="o">.</span><span class="n">duck_type_id</span><span class="p">:</span> <span class="n">duck_type_id</span><span class="p">,</span>
+<span class="p">}</span>
+<span class="n">duck</span> <span class="o">=</span> <span class="n">Duck</span><span class="p">()</span>
+<span class="n">duck</span><span class="o">.</span><span class="n">init</span><span class="p">(</span><span class="n">attr</span><span class="p">)</span>
 </code></pre></div>
-<h2 id="api">API</h2>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
-<span class="n">API</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">api</span>
+<p>or</p>
+<div class="highlight"><pre><span></span><code><span class="n">duck</span> <span class="o">=</span> <span class="n">Duck</span><span class="p">()</span>
+<span class="n">duck</span><span class="o">.</span><span class="n">init</span><span class="p">({</span>
+    <span class="n">Duck</span><span class="o">.</span><span class="n">name</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span>
+    <span class="n">Duck</span><span class="o">.</span><span class="n">duck_type_id</span><span class="p">:</span> <span class="n">duck_type_id</span><span class="p">,</span>
+<span class="p">})</span>
 </code></pre></div>
-<h2 id="configuration">Configuration</h2>
-<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
-<span class="n">CONFIG</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">config</span>
-<span class="n">tmp_directory_path</span> <span class="o">=</span> <span class="n">CONFIG</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s1">&#39;directories/tmp&#39;</span><span class="p">)</span>
+<p>Instead of:</p>
+<div class="highlight"><pre><span></span><code><span class="n">attr</span> <span class="o">=</span> <span class="p">{</span>
+    <span class="n">Duck</span><span class="o">.</span><span class="n">name</span><span class="p">:</span> <span class="n">name</span><span class="p">,</span>
+    <span class="n">Duck</span><span class="o">.</span><span class="n">duck_type_id</span><span class="p">:</span> <span class="n">duck_type_id</span><span class="p">,</span>
+<span class="p">}</span>
+<span class="n">duck</span> <span class="o">=</span> <span class="n">Duck</span><span class="p">()</span>
+<span class="n">duck</span><span class="o">.</span><span class="n">init</span><span class="p">(</span><span class="o">**</span><span class="p">{</span><span class="n">x</span><span class="o">.</span><span class="n">key</span><span class="p">:</span><span class="n">y</span> <span class="k">for</span> <span class="n">x</span><span class="p">,</span><span class="n">y</span> <span class="ow">in</span> <span class="n">attr</span><span class="o">.</span><span class="n">items</span><span class="p">()})</span>
 </code></pre></div>
                 
               
               
                 
 
 
@@ -532,36 +598,36 @@
       </main>
       
         
 <footer class="md-footer">
   
     <nav class="md-footer__inner md-grid" aria-label="Footer">
       
-        <a href="../alpha_setup/" class="md-footer__link md-footer__link--prev" rel="prev">
+        <a href="../schema/" class="md-footer__link md-footer__link--prev" rel="prev">
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12z"/></svg>
           </div>
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Previous
               </span>
-              Setup
+              Schema
             </div>
           </div>
         </a>
       
       
-        <a href="../alpha_api/" class="md-footer__link md-footer__link--next" rel="next">
+        <a href="../update/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Next
               </span>
-              Api
+              Update
             </div>
           </div>
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4z"/></svg>
           </div>
         </a>
       
@@ -582,15 +648,15 @@
   </div>
 </footer>
       
     </div>
     <div class="md-dialog" data-md-component="dialog">
       <div class="md-dialog__inner md-typeset"></div>
     </div>
-    <script id="__config" type="application/json">{"base": "..", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "../assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
+    <script id="__config" type="application/json">{"base": "../..", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "../../assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
     
     
-      <script src="../assets/javascripts/bundle.7353b375.min.js"></script>
+      <script src="../../assets/javascripts/bundle.7353b375.min.js"></script>
       
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -2,88 +2,69 @@
 
 
 
 
 
 
  ⁰ ⁰
-Skip_to_content
 
  Alpha Documentation
- Core
+ Instantiate
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
-    * ⁰  Core   Core    Table of contents
-          o Purpose
-          o How_to_use
-          o Logging
-                # Database
-          o API
+    * Core
+    * ⁰  Api      Api
+          o Main
           o Configuration
-    * Api
+          o Routes
+          o Parameters
+          o Model_Parameters
+          o Methods
+          o Cache
+          o Authorizations
+          o SqlAlchemy
+          o Issues
     * Screens
     * Configuration
-    * Database
+    * *  Database      Database
+          o Main
+          o Init
+          o Model
+          o Schema
+          o ⁰ Instantiate
+          o Update
+          o Relations
+          o Model_Parameters
     * Documentation
     * Administration
-   Table of contents
-    * Purpose
-    * How_to_use
-    * Logging
-          o Database
-    * API
-    * Configuration
-****** Alpha core system ******
-***** Purpose *****
-The core is used as a central point to manage various system:
-    * logging_system
-    * database_access
-    * api_system
-    * dynamic_configuration
-***** How to use *****
-You could:
-    * Use the alphaz core and initiate it at the start of you project
-      preferably in a file named core.py to be complient with this
-      documentation:
-      from alphaz.models.main import AlphaCore
-
-      core = AlphaCore(__file__)
-      DB, API, LOG = core.db, core.api, core.log # not required but recommanded
-    * Or create a core.py file at the root of your project containing at least:
-      from alphaz.models.main import AlphaCore, singleton
-
-      @singleton
-      class Core(AlphaCore):
-
-          def __init__(self,file:str):
-
-              super().__init__(file)
-
-      core = Core(__file__)
-      DB, API, LOG = core.db, core.api, core.log # not required but recommanded
-Note
-This is the recommended way, so that you could custom the Core class
-***** Logging *****
-from core import core
-LOG = core.get_logger('name')
-LOG.info('message')
-**** Database ****
-from core import core
-DB = core.db
-***** API *****
-from core import core
-API = core.api
-***** Configuration *****
-from core import core
-CONFIG = core.config
-tmp_directory_path = CONFIG.get('directories/tmp')
+****** Instantiate ******
+This enable the use of model columns which is not possible using SqlAlchemy:
+attr = {
+    Duck.name: name,
+    Duck.duck_type_id: duck_type_id,
+}
+duck = Duck()
+duck.init(attr)
+or
+duck = Duck()
+duck.init({
+    Duck.name: name,
+    Duck.duck_type_id: duck_type_id,
+})
+Instead of:
+attr = {
+    Duck.name: name,
+    Duck.duck_type_id: duck_type_id,
+}
+duck = Duck()
+duck.init(**{x.key:y for x,y in attr.items()})
 
- Previous__Setup
+ Previous__Schema
 
- Next__Api
+ Next__Update
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/alpha_screens/index.html` & `alphaz-0.7.4/alphaz/documentations/site/database/init/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width,initial-scale=1">
       
       
       
       
-      <link rel="icon" href="../assets/images/favicon.png">
+      <link rel="icon" href="../../assets/images/favicon.png">
       <meta name="generator" content="mkdocs-1.1.2, mkdocs-material-7.1.1">
     
     
       
-        <title>Screens - Alpha Documentation</title>
+        <title>Init - Alpha Documentation</title>
       
     
     
-      <link rel="stylesheet" href="../assets/stylesheets/main.9299cb39.min.css">
+      <link rel="stylesheet" href="../../assets/stylesheets/main.9299cb39.min.css">
       
         
-        <link rel="stylesheet" href="../assets/stylesheets/palette.ef6f36e2.min.css">
+        <link rel="stylesheet" href="../../assets/stylesheets/palette.ef6f36e2.min.css">
         
       
     
     
     
       
         
@@ -47,34 +47,34 @@
     
     
     
     
     <body dir="ltr" data-md-color-scheme="" data-md-color-primary="none" data-md-color-accent="none">
   
     
-    <script>function __prefix(e){return new URL("..",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
+    <script>function __prefix(e){return new URL("../..",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
     
     <input class="md-toggle" data-md-toggle="drawer" type="checkbox" id="__drawer" autocomplete="off">
     <input class="md-toggle" data-md-toggle="search" type="checkbox" id="__search" autocomplete="off">
     <label class="md-overlay" for="__drawer"></label>
     <div data-md-component="skip">
       
         
-        <a href="#alpha-screens-system" class="md-skip">
+        <a href="#route" class="md-skip">
           Skip to content
         </a>
       
     </div>
     <div data-md-component="announce">
       
     </div>
     
       <header class="md-header" data-md-component="header">
   <nav class="md-header__inner md-grid" aria-label="Header">
-    <a href=".." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="../.." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     <label class="md-header__button md-icon" for="__drawer">
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M3 6h18v2H3V6m0 5h18v2H3v-2m0 5h18v2H3v-2z"/></svg>
@@ -85,15 +85,15 @@
           <span class="md-ellipsis">
             Alpha Documentation
           </span>
         </div>
         <div class="md-header__topic" data-md-component="header-topic">
           <span class="md-ellipsis">
             
-              Screens
+              Init
             
           </span>
         </div>
       </div>
     </div>
     
     
@@ -146,15 +146,15 @@
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 
 
 <nav class="md-nav md-nav--primary" aria-label="Navigation" data-md-level="0">
   <label class="md-nav__title" for="__drawer">
-    <a href=".." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="../.." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     Alpha Documentation
   </label>
@@ -165,180 +165,392 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href=".." class="md-nav__link">
+      <a href="../.." class="md-nav__link">
         Home
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_setup/" class="md-nav__link">
+      <a href="../../alpha_setup/" class="md-nav__link">
         Setup
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
+      <a href="../../alpha_core/" class="md-nav__link">
         Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
-    <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
+    
+    <li class="md-nav__item md-nav__item--nested">
+      
+      
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_4" type="checkbox" id="__nav_4" >
+      
+      <label class="md-nav__link" for="__nav_4">
         Api
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Api" data-md-level="1">
+        <label class="md-nav__title" for="__nav_4">
+          <span class="md-nav__icon md-icon"></span>
+          Api
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/main/" class="md-nav__link">
+        Main
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/configuration/" class="md-nav__link">
+        Configuration
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/routes/" class="md-nav__link">
+        Routes
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/parameters/" class="md-nav__link">
+        Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/methods/" class="md-nav__link">
+        Methods
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/cache/" class="md-nav__link">
+        Cache
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/authorizations/" class="md-nav__link">
+        Authorizations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/sqlalchemy/" class="md-nav__link">
+        SqlAlchemy
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/issues/" class="md-nav__link">
+        Issues
       </a>
     </li>
   
 
+          
+        </ul>
+      </nav>
+    </li>
+  
+
     
       
       
       
 
   
   
-    
   
+    <li class="md-nav__item">
+      <a href="../../alpha_screens/" class="md-nav__link">
+        Screens
+      </a>
+    </li>
   
-    <li class="md-nav__item md-nav__item--active">
+
+    
       
-      <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
       
-        
       
+
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../configuration/" class="md-nav__link">
+        Configuration
+      </a>
+    </li>
+  
+
+    
       
-        <label class="md-nav__link md-nav__link--active" for="__toc">
-          Screens
-          <span class="md-nav__icon md-icon"></span>
-        </label>
       
-      <a href="./" class="md-nav__link md-nav__link--active">
-        Screens
-      </a>
       
-        
-<nav class="md-nav md-nav--secondary" aria-label="Table of contents">
+
   
   
     
   
   
-    <label class="md-nav__title" for="__toc">
-      <span class="md-nav__icon md-icon"></span>
-      Table of contents
-    </label>
-    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
+    
+    <li class="md-nav__item md-nav__item--active md-nav__item--nested">
       
-        <li class="md-nav__item">
-  <a href="#launch" class="md-nav__link">
-    Launch
-  </a>
-  
-</li>
       
-        <li class="md-nav__item">
-  <a href="#help" class="md-nav__link">
-    Help
-  </a>
-  
-</li>
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_7" type="checkbox" id="__nav_7" checked>
       
-    </ul>
+      <label class="md-nav__link" for="__nav_7">
+        Database
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Database" data-md-level="1">
+        <label class="md-nav__title" for="__nav_7">
+          <span class="md-nav__icon md-icon"></span>
+          Database
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
   
-</nav>
-      
+  
+  
+    <li class="md-nav__item">
+      <a href="../main/" class="md-nav__link">
+        Main
+      </a>
     </li>
   
 
+          
+            
+  
+  
     
+  
+  
+    <li class="md-nav__item md-nav__item--active">
+      
+      <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
+      
+        
       
       
+      <a href="./" class="md-nav__link md-nav__link--active">
+        Init
+      </a>
       
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="../configuration/" class="md-nav__link">
-        Configuration
+      <a href="../model/" class="md-nav__link">
+        Model
       </a>
     </li>
   
 
-    
-      
-      
-      
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../schema/" class="md-nav__link">
+        Schema
+      </a>
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_database/" class="md-nav__link">
-        Database
+      <a href="../instantiate/" class="md-nav__link">
+        Instantiate
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../update/" class="md-nav__link">
+        Update
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../relations/" class="md-nav__link">
+        Relations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api_database/" class="md-nav__link">
+        Model Parameters
       </a>
     </li>
   
 
+          
+        </ul>
+      </nav>
+    </li>
+  
+
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../documentation/" class="md-nav__link">
+      <a href="../../documentation/" class="md-nav__link">
         Documentation
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_admin/" class="md-nav__link">
+      <a href="../../alpha_admin/" class="md-nav__link">
         Administration
       </a>
     </li>
   
 
     
   </ul>
@@ -355,127 +567,88 @@
                     
 <nav class="md-nav md-nav--secondary" aria-label="Table of contents">
   
   
     
   
   
-    <label class="md-nav__title" for="__toc">
-      <span class="md-nav__icon md-icon"></span>
-      Table of contents
-    </label>
-    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
-      
-        <li class="md-nav__item">
-  <a href="#launch" class="md-nav__link">
-    Launch
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#help" class="md-nav__link">
-    Help
-  </a>
-  
-</li>
-      
-    </ul>
-  
 </nav>
                   </div>
                 </div>
               </div>
             
           
           <div class="md-content" data-md-component="content">
             <article class="md-content__inner md-typeset">
               
                 
                 
-                <h1 id="alpha-screens-system">Alpha screens system</h1>
-<p><strong>Alpha</strong> integrate a simple utility that enable to ensure that a <code>screen</code> if running or not. </p>
+                <h1 id="route">Route</h1>
+<p>The route <strong>database/init</strong> could be use to init the database or some tables.</p>
+<div class="highlight"><pre><span></span><code><span class="nd">@route</span><span class="p">(</span>
+    <span class="s2">&quot;/database/init&quot;</span><span class="p">,</span>
+    <span class="n">admin</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+    <span class="n">parameters</span><span class="o">=</span><span class="p">[</span>
+        <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;binds&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]),</span>
+        <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;tables&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">]),</span>
+        <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;drop&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="nb">bool</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="kc">False</span><span class="p">),</span>
+        <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;truncate&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="nb">bool</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="kc">False</span><span class="p">),</span>
+        <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;force&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="nb">bool</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="kc">False</span><span class="p">),</span>
+        <span class="n">Parameter</span><span class="p">(</span><span class="s2">&quot;create&quot;</span><span class="p">,</span> <span class="n">ptype</span><span class="o">=</span><span class="nb">bool</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span><span class="kc">False</span><span class="p">),</span>
+    <span class="p">],</span>
+<span class="p">)</span>
+</code></pre></div>
+<h1 id="configuration">Configuration</h1>
+<p>Content of tables could be pre-defined in various ways:</p>
 <ul>
-<li>optional arguments:</li>
-<li>-h, * --help            show this help message and exit</li>
-<li>--log LOG, -l LOG     log file path</li>
-<li>--file FILE, -f FILE  Input configuration file</li>
-<li>--name NAME, -n NAME  Screen name</li>
-<li>--cmd CMD, -c CMD     Command to run</li>
-<li>--envs ENVS [ENVS ...], -e ENVS [ENVS ...]
-                        Command to run</li>
-<li>--directory DIRECTORY, -d DIRECTORY
-                        Working directory</li>
-<li>--request REQUEST, -req REQUEST
-                        Request to check the response</li>
-<li>--retries RETRIES, -ret RETRIES
-                        Number of check before fail state</li>
-<li>--sleep SLEEP, -s SLEEP
-                        Sleep time (s)</li>
-<li>--timeout TIMEOUT, -t TIMEOUT
-                        Sleep time (s)</li>
-<li>--message MESSAGE, -m MESSAGE
-                        Check message</li>
-<li>--failed_message FAILED_MESSAGE, -fm FAILED_MESSAGE
-                        Failed message</li>
-<li>--success_message SUCCESS_MESSAGE, -sm SUCCESS_MESSAGE
-                        Success message</li>
-<li>--restart, -r         Force a restart</li>
+<li><strong>python</strong>: you have to specify the directory where the <strong>py</strong> files are defined using the <strong>init_database_dir_py</strong> parameter in your database configuration.</li>
 </ul>
-<h2 id="launch">Launch</h2>
-<p>Easy to launch, two modes are available:</p>
-<ol>
-<li>
-<p>Configuration file</p>
-<div class="highlight"><pre><span></span><code>python -m alphaz.utils.screens -f &lt;config_file_path&gt;
-</code></pre></div>
-<p>The configuration format is the following, it use the <a href="../configuration/">dynamic json alpha configuration syntax</a>:</p>
-<div class="highlight"><pre><span></span><code><span class="p">{</span>
-    <span class="nt">&quot;screens&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;api&quot;</span><span class="p">:</span> <span class="p">{</span>
-            <span class="nt">&quot;active&quot;</span><span class="p">:</span>    <span class="kc">true</span><span class="p">,</span>
-            <span class="nt">&quot;name&quot;</span><span class="p">:</span>      <span class="s2">&quot;API&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;dir&quot;</span><span class="p">:</span>       <span class="s2">&quot;{{home}}/{{name}}&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;shell_cmd&quot;</span><span class="p">:</span> <span class="s2">&quot;python api.py&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;request&quot;</span><span class="p">:</span> <span class="s2">&quot;http://0.0.0.0:{{port}}/status&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;fail_message&quot;</span><span class="p">:</span> <span class="s2">&quot;Api failed to restart&quot;</span>
-        <span class="p">},</span>
-        <span class="nt">&quot;api&quot;</span><span class="p">:</span> <span class="p">{</span>
-            <span class="nt">&quot;active&quot;</span><span class="p">:</span>    <span class="kc">false</span><span class="p">,</span>
-            <span class="nt">&quot;name&quot;</span><span class="p">:</span>      <span class="s2">&quot;API&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;dir&quot;</span><span class="p">:</span>       <span class="s2">&quot;{{home}}/{{name}}&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;shell_cmd&quot;</span><span class="p">:</span> <span class="s2">&quot;python api.py&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;request&quot;</span><span class="p">:</span> <span class="s2">&quot;http://0.0.0.0:{{port}}/status&quot;</span><span class="p">,</span>
-            <span class="nt">&quot;fail_message&quot;</span><span class="p">:</span> <span class="s2">&quot;Failed&quot;</span>
-        <span class="p">}</span>
-    <span class="p">},</span>
-    <span class="nt">&quot;configurations&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;local&quot;</span><span class="p">:</span> <span class="p">{</span>
-            <span class="nt">&quot;port&quot;</span><span class="p">:</span> <span class="s2">&quot;auto&quot;</span>
-        <span class="p">},</span>
-        <span class="nt">&quot;dev&quot;</span><span class="p">:</span> <span class="p">{</span>
-            <span class="nt">&quot;port&quot;</span><span class="p">:</span> <span class="mi">3000</span>
-        <span class="p">},</span>
-        <span class="nt">&quot;prod&quot;</span><span class="p">:</span> <span class="p">{</span>
-            <span class="nt">&quot;port&quot;</span><span class="p">:</span> <span class="mi">5000</span>
-        <span class="p">}</span>
+<p>For every table you want to fill you could specify <strong>objects</strong> which are models in this situation:</p>
+<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">models.database.olca</span> <span class="kn">import</span> <span class="n">TblGroups</span>
+
+<span class="n">ini</span> <span class="o">=</span> <span class="p">{</span>
+    <span class="n">TblGroups</span><span class="p">:</span> <span class="p">{</span>
+        <span class="s2">&quot;objects&quot;</span><span class="p">:</span> <span class="p">[</span>
+            <span class="n">TblGroups</span><span class="o">.</span><span class="n">instantiate</span><span class="p">(</span>
+                <span class="mi">2</span><span class="p">,</span> <span class="s2">&quot;hidden&quot;</span><span class="p">,</span> <span class="s2">&quot;far fa-eye-slash&quot;</span><span class="p">,</span> <span class="s2">&quot;var(--ion-color-light)&quot;</span>
+            <span class="p">),</span>
+            <span class="n">TblGroups</span><span class="o">.</span><span class="n">instantiate</span><span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="s2">&quot;steps&quot;</span><span class="p">,</span> <span class="s2">&quot;fas fa-cogs&quot;</span><span class="p">,</span> <span class="s2">&quot;var(--ion-color-danger)&quot;</span><span class="p">),</span>
+            <span class="n">TblGroups</span><span class="o">.</span><span class="n">instantiate</span><span class="p">(</span>
+                <span class="mi">4</span><span class="p">,</span> <span class="s2">&quot;materials&quot;</span><span class="p">,</span> <span class="s2">&quot;fas fa-cubes&quot;</span><span class="p">,</span> <span class="s2">&quot;var(--ion-color-primary)&quot;</span>
+            <span class="p">),</span>
+            <span class="n">TblGroups</span><span class="o">.</span><span class="n">instantiate</span><span class="p">(</span>
+                <span class="mi">5</span><span class="p">,</span> <span class="s2">&quot;transports&quot;</span><span class="p">,</span> <span class="s2">&quot;fas fa-dolly-flatbed&quot;</span><span class="p">,</span> <span class="s2">&quot;var(--ion-color-secondary)&quot;</span>
+            <span class="p">),</span>
+            <span class="n">TblGroups</span><span class="o">.</span><span class="n">instantiate</span><span class="p">(</span>
+                <span class="mi">6</span><span class="p">,</span> <span class="s2">&quot;powers&quot;</span><span class="p">,</span> <span class="s2">&quot;fas fa-lightbulb&quot;</span><span class="p">,</span> <span class="s2">&quot;var(--ion-color-warning)&quot;</span>
+            <span class="p">),</span>
+        <span class="p">]</span>
     <span class="p">},</span>
-    <span class="nt">&quot;home&quot;</span><span class="p">:</span> <span class="s2">&quot;/home/mes&quot;</span><span class="p">,</span>
-    <span class="nt">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;pyMES&quot;</span>
 <span class="p">}</span>
 </code></pre></div>
-</li>
-<li>
-<p>Parameters:</p>
-<div class="highlight"><pre><span></span><code>python -m alphaz.utils.screens * --name TEST * --cmd <span class="s2">&quot;python api.py&quot;</span>
+<ul>
+<li><strong>json</strong>: you have to specify the directory where the <strong>json</strong> files are defined using the <strong>init_database_dir_json</strong> parameter in your database configuration.</li>
+</ul>
+<div class="highlight"><pre><span></span><code><span class="p">{</span>
+    <span class="nt">&quot;sophisme&quot;</span><span class="p">:</span> <span class="p">{</span>
+        <span class="nt">&quot;headers&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;theme&quot;</span><span class="p">,</span><span class="s2">&quot;sophisme&quot;</span><span class="p">,</span><span class="s2">&quot;user&quot;</span><span class="p">,</span><span class="s2">&quot;proposition&quot;</span><span class="p">],</span>
+        <span class="nt">&quot;values&quot;</span><span class="p">:</span>
+            <span class="p">[</span>
+                <span class="p">[</span><span class="mi">5</span><span class="p">,</span><span class="mi">20</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">34</span><span class="p">],</span>
+                <span class="p">[</span><span class="mi">5</span><span class="p">,</span><span class="mi">7</span><span class="p">,</span><span class="mi">1</span><span class="p">,</span><span class="mi">35</span><span class="p">],</span>
+                <span class="p">[</span><span class="mi">5</span><span class="p">,</span><span class="mi">9</span><span class="p">,</span><span class="mi">1</span><span class="p">,</span><span class="mi">35</span><span class="p">]</span>
+            <span class="p">]</span>
+    <span class="p">}</span>
+<span class="p">}</span>
 </code></pre></div>
-</li>
-</ol>
-<h2 id="help">Help</h2>
-<div class="highlight"><pre><span></span><code>python -m alphaz.utils.screens
+<ul>
+<li><strong>sql</strong>: you have to specify the directory where the <strong>sql</strong> files are defined using the <strong>init_database_dir_sql</strong> parameter in your database configuration.</li>
+</ul>
+<p>Here the code is directly executed, so it could have any valid sql structure.</p>
+<div class="highlight"><pre><span></span><code>
 </code></pre></div>
                 
               
               
                 
 
 
@@ -487,36 +660,36 @@
       </main>
       
         
 <footer class="md-footer">
   
     <nav class="md-footer__inner md-grid" aria-label="Footer">
       
-        <a href="../alpha_api/" class="md-footer__link md-footer__link--prev" rel="prev">
+        <a href="../main/" class="md-footer__link md-footer__link--prev" rel="prev">
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12z"/></svg>
           </div>
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Previous
               </span>
-              Api
+              Main
             </div>
           </div>
         </a>
       
       
-        <a href="../configuration/" class="md-footer__link md-footer__link--next" rel="next">
+        <a href="../model/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Next
               </span>
-              Configuration
+              Model
             </div>
           </div>
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4z"/></svg>
           </div>
         </a>
       
@@ -537,15 +710,15 @@
   </div>
 </footer>
       
     </div>
     <div class="md-dialog" data-md-component="dialog">
       <div class="md-dialog__inner md-typeset"></div>
     </div>
-    <script id="__config" type="application/json">{"base": "..", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "../assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
+    <script id="__config" type="application/json">{"base": "../..", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "../../assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
     
     
-      <script src="../assets/javascripts/bundle.7353b375.min.js"></script>
+      <script src="../../assets/javascripts/bundle.7353b375.min.js"></script>
       
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -5,95 +5,108 @@
 
 
 
  ⁰ ⁰
 Skip_to_content
 
  Alpha Documentation
- Screens
+ Init
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
     * Core
-    * Api
-    * ⁰  Screens   Screens    Table of contents
-          o Launch
-          o Help
+    * ⁰  Api      Api
+          o Main
+          o Configuration
+          o Routes
+          o Parameters
+          o Model_Parameters
+          o Methods
+          o Cache
+          o Authorizations
+          o SqlAlchemy
+          o Issues
+    * Screens
     * Configuration
-    * Database
+    * *  Database      Database
+          o Main
+          o ⁰ Init
+          o Model
+          o Schema
+          o Instantiate
+          o Update
+          o Relations
+          o Model_Parameters
     * Documentation
     * Administration
-   Table of contents
-    * Launch
-    * Help
-****** Alpha screens system ******
-Alpha integrate a simple utility that enable to ensure that a screen if running
-or not.
-    * optional arguments:
-    * -h, * --help show this help message and exit
-    * --log LOG, -l LOG log file path
-    * --file FILE, -f FILE Input configuration file
-    * --name NAME, -n NAME Screen name
-    * --cmd CMD, -c CMD Command to run
-    * --envs ENVS [ENVS ...], -e ENVS [ENVS ...] Command to run
-    * --directory DIRECTORY, -d DIRECTORY Working directory
-    * --request REQUEST, -req REQUEST Request to check the response
-    * --retries RETRIES, -ret RETRIES Number of check before fail state
-    * --sleep SLEEP, -s SLEEP Sleep time (s)
-    * --timeout TIMEOUT, -t TIMEOUT Sleep time (s)
-    * --message MESSAGE, -m MESSAGE Check message
-    * --failed_message FAILED_MESSAGE, -fm FAILED_MESSAGE Failed message
-    * --success_message SUCCESS_MESSAGE, -sm SUCCESS_MESSAGE Success message
-    * --restart, -r Force a restart
-***** Launch *****
-Easy to launch, two modes are available:
-   1. Configuration file
-      python -m alphaz.utils.screens -f <config_file_path>
-      The configuration format is the following, it use the dynamic_json_alpha
-      configuration_syntax:
-      {
-          "screens": {
-              "api": {
-                  "active":    true,
-                  "name":      "API",
-                  "dir":       "{{home}}/{{name}}",
-                  "shell_cmd": "python api.py",
-                  "request": "http://0.0.0.0:{{port}}/status",
-                  "fail_message": "Api failed to restart"
-              },
-              "api": {
-                  "active":    false,
-                  "name":      "API",
-                  "dir":       "{{home}}/{{name}}",
-                  "shell_cmd": "python api.py",
-                  "request": "http://0.0.0.0:{{port}}/status",
-                  "fail_message": "Failed"
-              }
-          },
-          "configurations": {
-              "local": {
-                  "port": "auto"
-              },
-              "dev": {
-                  "port": 3000
-              },
-              "prod": {
-                  "port": 5000
-              }
-          },
-          "home": "/home/mes",
-          "name": "pyMES"
-      }
-   2. Parameters:
-      python -m alphaz.utils.screens * --name TEST * --cmd "python api.py"
-***** Help *****
-python -m alphaz.utils.screens
 
- Previous__Api
+****** Route ******
+The route database/init could be use to init the database or some tables.
+@route(
+    "/database/init",
+    admin=True,
+    parameters=[
+        Parameter("binds", ptype=List[str]),
+        Parameter("tables", ptype=List[str]),
+        Parameter("drop", ptype=bool, default=False),
+        Parameter("truncate", ptype=bool, default=False),
+        Parameter("force", ptype=bool, default=False),
+        Parameter("create", ptype=bool, default=False),
+    ],
+)
+****** Configuration ******
+Content of tables could be pre-defined in various ways:
+    * python: you have to specify the directory where the py files are defined
+      using the init_database_dir_py parameter in your database configuration.
+For every table you want to fill you could specify objects which are models in
+this situation:
+from models.database.olca import TblGroups
+
+ini = {
+    TblGroups: {
+        "objects": [
+            TblGroups.instantiate(
+                2, "hidden", "far fa-eye-slash", "var(--ion-color-light)"
+            ),
+            TblGroups.instantiate(3, "steps", "fas fa-cogs", "var(--ion-color-
+danger)"),
+            TblGroups.instantiate(
+                4, "materials", "fas fa-cubes", "var(--ion-color-primary)"
+            ),
+            TblGroups.instantiate(
+                5, "transports", "fas fa-dolly-flatbed", "var(--ion-color-
+secondary)"
+            ),
+            TblGroups.instantiate(
+                6, "powers", "fas fa-lightbulb", "var(--ion-color-warning)"
+            ),
+        ]
+    },
+}
+    * json: you have to specify the directory where the json files are defined
+      using the init_database_dir_json parameter in your database
+      configuration.
+{
+    "sophisme": {
+        "headers": ["theme","sophisme","user","proposition"],
+        "values":
+            [
+                [5,20,6,34],
+                [5,7,1,35],
+                [5,9,1,35]
+            ]
+    }
+}
+    * sql: you have to specify the directory where the sql files are defined
+      using the init_database_dir_sql parameter in your database configuration.
+Here the code is directly executed, so it could have any valid sql structure.
 
- Next__Configuration
+
+ Previous__Main
+
+ Next__Model
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/alpha_setup/index.html` & `alphaz-0.7.4/alphaz/documentations/site/alpha_screens/index.html`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
       
       
       <link rel="icon" href="../assets/images/favicon.png">
       <meta name="generator" content="mkdocs-1.1.2, mkdocs-material-7.1.1">
     
     
       
-        <title>Setup - Alpha Documentation</title>
+        <title>Screens - Alpha Documentation</title>
       
     
     
       <link rel="stylesheet" href="../assets/stylesheets/main.9299cb39.min.css">
       
         
         <link rel="stylesheet" href="../assets/stylesheets/palette.ef6f36e2.min.css">
@@ -55,15 +55,15 @@
     
     <input class="md-toggle" data-md-toggle="drawer" type="checkbox" id="__drawer" autocomplete="off">
     <input class="md-toggle" data-md-toggle="search" type="checkbox" id="__search" autocomplete="off">
     <label class="md-overlay" for="__drawer"></label>
     <div data-md-component="skip">
       
         
-        <a href="#alpha-system" class="md-skip">
+        <a href="#alpha-screens-system" class="md-skip">
           Skip to content
         </a>
       
     </div>
     <div data-md-component="announce">
       
     </div>
@@ -85,15 +85,15 @@
           <span class="md-ellipsis">
             Alpha Documentation
           </span>
         </div>
         <div class="md-header__topic" data-md-component="header-topic">
           <span class="md-ellipsis">
             
-              Setup
+              Screens
             
           </span>
         </div>
       </div>
     </div>
     
     
@@ -178,31 +178,211 @@
     
       
       
       
 
   
   
+  
+    <li class="md-nav__item">
+      <a href="../alpha_setup/" class="md-nav__link">
+        Setup
+      </a>
+    </li>
+  
+
+    
+      
+      
+      
+
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../alpha_core/" class="md-nav__link">
+        Core
+      </a>
+    </li>
+  
+
+    
+      
+      
+      
+
+  
+  
+  
+    
+    <li class="md-nav__item md-nav__item--nested">
+      
+      
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_4" type="checkbox" id="__nav_4" >
+      
+      <label class="md-nav__link" for="__nav_4">
+        Api
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Api" data-md-level="1">
+        <label class="md-nav__title" for="__nav_4">
+          <span class="md-nav__icon md-icon"></span>
+          Api
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api/main/" class="md-nav__link">
+        Main
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api/configuration/" class="md-nav__link">
+        Configuration
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api/routes/" class="md-nav__link">
+        Routes
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api/parameters/" class="md-nav__link">
+        Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api/methods/" class="md-nav__link">
+        Methods
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api/cache/" class="md-nav__link">
+        Cache
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api/authorizations/" class="md-nav__link">
+        Authorizations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api/sqlalchemy/" class="md-nav__link">
+        SqlAlchemy
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api/issues/" class="md-nav__link">
+        Issues
+      </a>
+    </li>
+  
+
+          
+        </ul>
+      </nav>
+    </li>
+  
+
+    
+      
+      
+      
+
+  
+  
     
   
   
     <li class="md-nav__item md-nav__item--active">
       
       <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
       
         
       
       
         <label class="md-nav__link md-nav__link--active" for="__toc">
-          Setup
+          Screens
           <span class="md-nav__icon md-icon"></span>
         </label>
       
       <a href="./" class="md-nav__link md-nav__link--active">
-        Setup
+        Screens
       </a>
       
         
 <nav class="md-nav md-nav--secondary" aria-label="Table of contents">
   
   
     
@@ -211,99 +391,26 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
-  <a href="#os-configuration" class="md-nav__link">
-    OS configuration
+  <a href="#launch" class="md-nav__link">
+    Launch
   </a>
   
-    <nav class="md-nav" aria-label="OS configuration">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#python" class="md-nav__link">
-    Python
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
 </li>
       
         <li class="md-nav__item">
-  <a href="#setup" class="md-nav__link">
-    Setup
-  </a>
-  
-    <nav class="md-nav" aria-label="Setup">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#classic" class="md-nav__link">
-    Classic
+  <a href="#help" class="md-nav__link">
+    Help
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#using-sources" class="md-nav__link">
-    Using sources
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#dependencies" class="md-nav__link">
-    Dependencies
-  </a>
-  
-    <nav class="md-nav" aria-label="Dependencies">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#oracle" class="md-nav__link">
-    Oracle
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#configuration" class="md-nav__link">
-    Configuration
-  </a>
-  
-    <nav class="md-nav" aria-label="Configuration">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#angular" class="md-nav__link">
-    Angular
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
       
     </ul>
   
 </nav>
       
     </li>
   
@@ -313,80 +420,146 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
-        Core
+      <a href="../configuration/" class="md-nav__link">
+        Configuration
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
+    
+    <li class="md-nav__item md-nav__item--nested">
+      
+      
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_7" type="checkbox" id="__nav_7" >
+      
+      <label class="md-nav__link" for="__nav_7">
+        Database
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Database" data-md-level="1">
+        <label class="md-nav__title" for="__nav_7">
+          <span class="md-nav__icon md-icon"></span>
+          Database
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
+  
+  
+  
     <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
-        Api
+      <a href="../database/main/" class="md-nav__link">
+        Main
       </a>
     </li>
   
 
-    
-      
-      
-      
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../database/init/" class="md-nav__link">
+        Init
+      </a>
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_screens/" class="md-nav__link">
-        Screens
+      <a href="../database/model/" class="md-nav__link">
+        Model
       </a>
     </li>
   
 
-    
-      
-      
-      
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../database/schema/" class="md-nav__link">
+        Schema
+      </a>
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="../configuration/" class="md-nav__link">
-        Configuration
+      <a href="../database/instantiate/" class="md-nav__link">
+        Instantiate
       </a>
     </li>
   
 
-    
-      
-      
-      
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../database/update/" class="md-nav__link">
+        Update
+      </a>
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_database/" class="md-nav__link">
-        Database
+      <a href="../database/relations/" class="md-nav__link">
+        Relations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../api_database/" class="md-nav__link">
+        Model Parameters
       </a>
     </li>
   
 
+          
+        </ul>
+      </nav>
+    </li>
+  
+
     
       
       
       
 
   
   
@@ -435,98 +608,25 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
-  <a href="#os-configuration" class="md-nav__link">
-    OS configuration
-  </a>
-  
-    <nav class="md-nav" aria-label="OS configuration">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#python" class="md-nav__link">
-    Python
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#setup" class="md-nav__link">
-    Setup
-  </a>
-  
-    <nav class="md-nav" aria-label="Setup">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#classic" class="md-nav__link">
-    Classic
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#using-sources" class="md-nav__link">
-    Using sources
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#dependencies" class="md-nav__link">
-    Dependencies
-  </a>
-  
-    <nav class="md-nav" aria-label="Dependencies">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#oracle" class="md-nav__link">
-    Oracle
+  <a href="#launch" class="md-nav__link">
+    Launch
   </a>
   
 </li>
-        
-      </ul>
-    </nav>
-  
-</li>
       
         <li class="md-nav__item">
-  <a href="#configuration" class="md-nav__link">
-    Configuration
+  <a href="#help" class="md-nav__link">
+    Help
   </a>
   
-    <nav class="md-nav" aria-label="Configuration">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
-  <a href="#angular" class="md-nav__link">
-    Angular
-  </a>
-  
-</li>
-        
-      </ul>
-    </nav>
-  
 </li>
       
     </ul>
   
 </nav>
                   </div>
                 </div>
@@ -534,85 +634,94 @@
             
           
           <div class="md-content" data-md-component="content">
             <article class="md-content__inner md-typeset">
               
                 
                 
-                <h1 id="alpha-system">Alpha system</h1>
-<h2 id="os-configuration">OS configuration</h2>
-<div class="admonition important">
-<p class="admonition-title">Important</p>
-<p>make sure that <strong>Git</strong> is well configured.</p>
-</div>
-<h3 id="python">Python</h3>
+                <h1 id="alpha-screens-system">Alpha screens system</h1>
+<p><strong>Alpha</strong> integrate a simple utility that enable to ensure that a <code>screen</code> if running or not. </p>
 <ul>
-<li>Python 3.10.4 is required.
-<a href="https://www.anaconda.com/">Anaconda</a> or <a href="https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html">Miniconda</a> could be used.</li>
-</ul>
-<p>There is no constraint but the usual structure is to have:</p>
-<ul>
-<li>a user per configuration (<em>mes</em>, <em>mesacc</em>, <em>mesint</em> and <em>mesdev</em> for exemple)</li>
-<li>three location per user:<ul>
-<li><em><em>/application/USER/APP_NAME</em></em> for sources</li>
-<li><em><em>/home/USER/configs</em></em> for configurations</li>
-<li><em><em>/application/USER/APP_NAME</em></em> for tmp files and logs</li>
-</ul>
-</li>
+<li>optional arguments:</li>
+<li>-h, * --help            show this help message and exit</li>
+<li>--log LOG, -l LOG     log file path</li>
+<li>--file FILE, -f FILE  Input configuration file</li>
+<li>--name NAME, -n NAME  Screen name</li>
+<li>--cmd CMD, -c CMD     Command to run</li>
+<li>--envs ENVS [ENVS ...], -e ENVS [ENVS ...]
+                        Command to run</li>
+<li>--directory DIRECTORY, -d DIRECTORY
+                        Working directory</li>
+<li>--request REQUEST, -req REQUEST
+                        Request to check the response</li>
+<li>--retries RETRIES, -ret RETRIES
+                        Number of check before fail state</li>
+<li>--sleep SLEEP, -s SLEEP
+                        Sleep time (s)</li>
+<li>--timeout TIMEOUT, -t TIMEOUT
+                        Sleep time (s)</li>
+<li>--message MESSAGE, -m MESSAGE
+                        Check message</li>
+<li>--failed_message FAILED_MESSAGE, -fm FAILED_MESSAGE
+                        Failed message</li>
+<li>--success_message SUCCESS_MESSAGE, -sm SUCCESS_MESSAGE
+                        Success message</li>
+<li>--restart, -r         Force a restart</li>
 </ul>
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>This is configured within the conf.json file and could be modified</p>
-</div>
-<h2 id="setup">Setup</h2>
-<p>If you just want to use the system go for the <strong>classic</strong> way and if you want to modify it use the <strong>sources</strong> integration.</p>
-<h3 id="classic">Classic</h3>
-<p>The default installation procedure is:</p>
-<div class="highlight"><pre><span></span><code>pip install alphaz
-</code></pre></div>
-<p>It will install all the <strong>dependencies</strong> automatically.</p>
-<h3 id="using-sources">Using sources</h3>
-<p>If you want to edit the sources you could use this procedure to clone the sources and configure it as a <strong>sub module</strong></p>
+<h2 id="launch">Launch</h2>
+<p>Easy to launch, two modes are available:</p>
 <ol>
 <li>
-<p>Clone <strong>alphaz</strong> from the repository <em>https://github.com/ZAurele/alphaz.git</em></p>
-<div class="highlight"><pre><span></span><code><span class="nb">cd</span> &lt;your_project_repository&gt;
-git clone https://github.com/ZAurele/alphaz.git
+<p>Configuration file</p>
+<div class="highlight"><pre><span></span><code>python -m alphaz.utils.screens -f &lt;config_file_path&gt;
 </code></pre></div>
-</li>
-<li>
-<p>Launch the setup, it will install all the dependencies and other magical actions.</p>
-<div class="highlight"><pre><span></span><code>python setup.py
+<p>The configuration format is the following, it use the <a href="../configuration/">dynamic json alpha configuration syntax</a>:</p>
+<div class="highlight"><pre><span></span><code><span class="p">{</span>
+    <span class="nt">&quot;screens&quot;</span><span class="p">:</span> <span class="p">{</span>
+        <span class="nt">&quot;api&quot;</span><span class="p">:</span> <span class="p">{</span>
+            <span class="nt">&quot;active&quot;</span><span class="p">:</span>    <span class="kc">true</span><span class="p">,</span>
+            <span class="nt">&quot;name&quot;</span><span class="p">:</span>      <span class="s2">&quot;API&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;dir&quot;</span><span class="p">:</span>       <span class="s2">&quot;{{home}}/{{name}}&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;shell_cmd&quot;</span><span class="p">:</span> <span class="s2">&quot;python api.py&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;request&quot;</span><span class="p">:</span> <span class="s2">&quot;http://0.0.0.0:{{port}}/status&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;fail_message&quot;</span><span class="p">:</span> <span class="s2">&quot;Api failed to restart&quot;</span>
+        <span class="p">},</span>
+        <span class="nt">&quot;api&quot;</span><span class="p">:</span> <span class="p">{</span>
+            <span class="nt">&quot;active&quot;</span><span class="p">:</span>    <span class="kc">false</span><span class="p">,</span>
+            <span class="nt">&quot;name&quot;</span><span class="p">:</span>      <span class="s2">&quot;API&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;dir&quot;</span><span class="p">:</span>       <span class="s2">&quot;{{home}}/{{name}}&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;shell_cmd&quot;</span><span class="p">:</span> <span class="s2">&quot;python api.py&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;request&quot;</span><span class="p">:</span> <span class="s2">&quot;http://0.0.0.0:{{port}}/status&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;fail_message&quot;</span><span class="p">:</span> <span class="s2">&quot;Failed&quot;</span>
+        <span class="p">}</span>
+    <span class="p">},</span>
+    <span class="nt">&quot;configurations&quot;</span><span class="p">:</span> <span class="p">{</span>
+        <span class="nt">&quot;local&quot;</span><span class="p">:</span> <span class="p">{</span>
+            <span class="nt">&quot;port&quot;</span><span class="p">:</span> <span class="s2">&quot;auto&quot;</span>
+        <span class="p">},</span>
+        <span class="nt">&quot;dev&quot;</span><span class="p">:</span> <span class="p">{</span>
+            <span class="nt">&quot;port&quot;</span><span class="p">:</span> <span class="mi">3000</span>
+        <span class="p">},</span>
+        <span class="nt">&quot;prod&quot;</span><span class="p">:</span> <span class="p">{</span>
+            <span class="nt">&quot;port&quot;</span><span class="p">:</span> <span class="mi">5000</span>
+        <span class="p">}</span>
+    <span class="p">},</span>
+    <span class="nt">&quot;home&quot;</span><span class="p">:</span> <span class="s2">&quot;/home/mes&quot;</span><span class="p">,</span>
+    <span class="nt">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;pyMES&quot;</span>
+<span class="p">}</span>
 </code></pre></div>
 </li>
 <li>
-<p>Define it as a submodule in your project</p>
+<p>Parameters:</p>
+<div class="highlight"><pre><span></span><code>python -m alphaz.utils.screens * --name TEST * --cmd <span class="s2">&quot;python api.py&quot;</span>
+</code></pre></div>
 </li>
 </ol>
-<h2 id="dependencies">Dependencies</h2>
-<p>Main dependencies are automatically installed, however if you need specific ones, you will have to install them manually</p>
-<h3 id="oracle">Oracle</h3>
-<p>Oracle client </p>
-<h2 id="configuration">Configuration</h2>
-<h3 id="angular">Angular</h3>
-<div class="highlight"><pre><span></span><code><span class="p">{</span>
-  <span class="nt">&quot;compilerOptions&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;baseUrl&quot;</span><span class="p">:</span> <span class="s2">&quot;./src&quot;</span><span class="p">,</span>
-    <span class="nt">&quot;paths&quot;</span><span class="p">:</span> <span class="p">{</span>
-      <span class="nt">&quot;@services/*&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;app/services/*&quot;</span><span class="p">,</span> <span class="s2">&quot;src/app/services/*&quot;</span><span class="p">],</span>
-      <span class="nt">&quot;@views/*&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;app/views/*&quot;</span><span class="p">,</span> <span class="s2">&quot;src/app/views/*&quot;</span><span class="p">],</span>
-      <span class="nt">&quot;@models/*&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;app/models/*&quot;</span><span class="p">,</span> <span class="s2">&quot;src/app/models/*&quot;</span><span class="p">],</span>
-      <span class="nt">&quot;@components/*&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;app/components/*&quot;</span><span class="p">,</span> <span class="s2">&quot;src/app/components/*&quot;</span><span class="p">],</span>
-      <span class="nt">&quot;@alphaa/*&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;alphaa/*&quot;</span><span class="p">,</span> <span class="s2">&quot;src/alphaa/*&quot;</span><span class="p">],</span>
-      <span class="nt">&quot;@layout/*&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;app/layout/*&quot;</span><span class="p">,</span> <span class="s2">&quot;src/app/layout/*&quot;</span><span class="p">],</span>
-      <span class="nt">&quot;@envs/*&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;environments/*&quot;</span><span class="p">,</span> <span class="s2">&quot;src/environments/*&quot;</span><span class="p">],</span>
-      <span class="nt">&quot;@constants/*&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;app/constants/*&quot;</span><span class="p">,</span> <span class="s2">&quot;src/app/constants/*&quot;</span><span class="p">]</span>
-    <span class="p">}</span>
-  <span class="p">}</span>
-<span class="p">}</span>
+<h2 id="help">Help</h2>
+<div class="highlight"><pre><span></span><code>python -m alphaz.utils.screens
 </code></pre></div>
                 
               
               
                 
 
 
@@ -624,36 +733,36 @@
       </main>
       
         
 <footer class="md-footer">
   
     <nav class="md-footer__inner md-grid" aria-label="Footer">
       
-        <a href=".." class="md-footer__link md-footer__link--prev" rel="prev">
+        <a href="../api/issues/" class="md-footer__link md-footer__link--prev" rel="prev">
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12z"/></svg>
           </div>
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Previous
               </span>
-              Home
+              Issues
             </div>
           </div>
         </a>
       
       
-        <a href="../alpha_core/" class="md-footer__link md-footer__link--next" rel="next">
+        <a href="../configuration/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Next
               </span>
-              Core
+              Configuration
             </div>
           </div>
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4z"/></svg>
           </div>
         </a>
```

#### html2text {}

```diff
@@ -5,100 +5,113 @@
 
 
 
  ⁰ ⁰
 Skip_to_content
 
  Alpha Documentation
- Setup
+ Screens
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
-    * ⁰  Setup   Setup    Table of contents
-          o OS_configuration
-                # Python
-          o Setup
-                # Classic
-                # Using_sources
-          o Dependencies
-                # Oracle
-          o Configuration
-                # Angular
+    * Setup
     * Core
-    * Api
-    * Screens
+    * ⁰  Api      Api
+          o Main
+          o Configuration
+          o Routes
+          o Parameters
+          o Model_Parameters
+          o Methods
+          o Cache
+          o Authorizations
+          o SqlAlchemy
+          o Issues
+    * ⁰  Screens   Screens    Table of contents
+          o Launch
+          o Help
     * Configuration
-    * Database
+    * ⁰  Database      Database
+          o Main
+          o Init
+          o Model
+          o Schema
+          o Instantiate
+          o Update
+          o Relations
+          o Model_Parameters
     * Documentation
     * Administration
    Table of contents
-    * OS_configuration
-          o Python
-    * Setup
-          o Classic
-          o Using_sources
-    * Dependencies
-          o Oracle
-    * Configuration
-          o Angular
-****** Alpha system ******
-***** OS configuration *****
-Important
-make sure that Git is well configured.
-**** Python ****
-    * Python 3.10.4 is required. Anaconda or Miniconda could be used.
-There is no constraint but the usual structure is to have:
-    * a user per configuration (mes, mesacc, mesint and mesdev for exemple)
-    * three location per user:
-          o /application/USER/APP_NAME for sources
-          o /home/USER/configs for configurations
-          o /application/USER/APP_NAME for tmp files and logs
-Note
-This is configured within the conf.json file and could be modified
-***** Setup *****
-If you just want to use the system go for the classic way and if you want to
-modify it use the sources integration.
-**** Classic ****
-The default installation procedure is:
-pip install alphaz
-It will install all the dependencies automatically.
-**** Using sources ****
-If you want to edit the sources you could use this procedure to clone the
-sources and configure it as a sub module
-   1. Clone alphaz from the repository https://github.com/ZAurele/alphaz.git
-      cd <your_project_repository>
-      git clone https://github.com/ZAurele/alphaz.git
-   2. Launch the setup, it will install all the dependencies and other magical
-      actions.
-      python setup.py
-   3. Define it as a submodule in your project
-***** Dependencies *****
-Main dependencies are automatically installed, however if you need specific
-ones, you will have to install them manually
-**** Oracle ****
-Oracle client
-***** Configuration *****
-**** Angular ****
-{
-  "compilerOptions": {
-    "baseUrl": "./src",
-    "paths": {
-      "@services/*": ["app/services/*", "src/app/services/*"],
-      "@views/*": ["app/views/*", "src/app/views/*"],
-      "@models/*": ["app/models/*", "src/app/models/*"],
-      "@components/*": ["app/components/*", "src/app/components/*"],
-      "@alphaa/*": ["alphaa/*", "src/alphaa/*"],
-      "@layout/*": ["app/layout/*", "src/app/layout/*"],
-      "@envs/*": ["environments/*", "src/environments/*"],
-      "@constants/*": ["app/constants/*", "src/app/constants/*"]
-    }
-  }
-}
+    * Launch
+    * Help
+****** Alpha screens system ******
+Alpha integrate a simple utility that enable to ensure that a screen if running
+or not.
+    * optional arguments:
+    * -h, * --help show this help message and exit
+    * --log LOG, -l LOG log file path
+    * --file FILE, -f FILE Input configuration file
+    * --name NAME, -n NAME Screen name
+    * --cmd CMD, -c CMD Command to run
+    * --envs ENVS [ENVS ...], -e ENVS [ENVS ...] Command to run
+    * --directory DIRECTORY, -d DIRECTORY Working directory
+    * --request REQUEST, -req REQUEST Request to check the response
+    * --retries RETRIES, -ret RETRIES Number of check before fail state
+    * --sleep SLEEP, -s SLEEP Sleep time (s)
+    * --timeout TIMEOUT, -t TIMEOUT Sleep time (s)
+    * --message MESSAGE, -m MESSAGE Check message
+    * --failed_message FAILED_MESSAGE, -fm FAILED_MESSAGE Failed message
+    * --success_message SUCCESS_MESSAGE, -sm SUCCESS_MESSAGE Success message
+    * --restart, -r Force a restart
+***** Launch *****
+Easy to launch, two modes are available:
+   1. Configuration file
+      python -m alphaz.utils.screens -f <config_file_path>
+      The configuration format is the following, it use the dynamic_json_alpha
+      configuration_syntax:
+      {
+          "screens": {
+              "api": {
+                  "active":    true,
+                  "name":      "API",
+                  "dir":       "{{home}}/{{name}}",
+                  "shell_cmd": "python api.py",
+                  "request": "http://0.0.0.0:{{port}}/status",
+                  "fail_message": "Api failed to restart"
+              },
+              "api": {
+                  "active":    false,
+                  "name":      "API",
+                  "dir":       "{{home}}/{{name}}",
+                  "shell_cmd": "python api.py",
+                  "request": "http://0.0.0.0:{{port}}/status",
+                  "fail_message": "Failed"
+              }
+          },
+          "configurations": {
+              "local": {
+                  "port": "auto"
+              },
+              "dev": {
+                  "port": 3000
+              },
+              "prod": {
+                  "port": 5000
+              }
+          },
+          "home": "/home/mes",
+          "name": "pyMES"
+      }
+   2. Parameters:
+      python -m alphaz.utils.screens * --name TEST * --cmd "python api.py"
+***** Help *****
+python -m alphaz.utils.screens
 
- Previous__Home
+ Previous__Issues
 
- Next__Core
+ Next__Configuration
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/images/favicon.png` & `alphaz-0.7.4/alphaz/documentations/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map` & `alphaz-0.7.4/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css` & `alphaz-0.7.4/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map` & `alphaz-0.7.4/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css` & `alphaz-0.7.4/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map` & `alphaz-0.7.4/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/configuration/index.html` & `alphaz-0.7.4/alphaz/documentations/site/api/configuration/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width,initial-scale=1">
       
       
       
       
-      <link rel="icon" href="../assets/images/favicon.png">
+      <link rel="icon" href="../../assets/images/favicon.png">
       <meta name="generator" content="mkdocs-1.1.2, mkdocs-material-7.1.1">
     
     
       
         <title>Configuration - Alpha Documentation</title>
       
     
     
-      <link rel="stylesheet" href="../assets/stylesheets/main.9299cb39.min.css">
+      <link rel="stylesheet" href="../../assets/stylesheets/main.9299cb39.min.css">
       
         
-        <link rel="stylesheet" href="../assets/stylesheets/palette.ef6f36e2.min.css">
+        <link rel="stylesheet" href="../../assets/stylesheets/palette.ef6f36e2.min.css">
         
       
     
     
     
       
         
@@ -47,34 +47,34 @@
     
     
     
     
     <body dir="ltr" data-md-color-scheme="" data-md-color-primary="none" data-md-color-accent="none">
   
     
-    <script>function __prefix(e){return new URL("..",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
+    <script>function __prefix(e){return new URL("../..",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
     
     <input class="md-toggle" data-md-toggle="drawer" type="checkbox" id="__drawer" autocomplete="off">
     <input class="md-toggle" data-md-toggle="search" type="checkbox" id="__search" autocomplete="off">
     <label class="md-overlay" for="__drawer"></label>
     <div data-md-component="skip">
       
         
-        <a href="#dynamic-json-alpha-configuration-syntax" class="md-skip">
+        <a href="#main" class="md-skip">
           Skip to content
         </a>
       
     </div>
     <div data-md-component="announce">
       
     </div>
     
       <header class="md-header" data-md-component="header">
   <nav class="md-header__inner md-grid" aria-label="Header">
-    <a href=".." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="../.." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     <label class="md-header__button md-icon" for="__drawer">
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M3 6h18v2H3V6m0 5h18v2H3v-2m0 5h18v2H3v-2z"/></svg>
@@ -146,15 +146,15 @@
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 
 
 <nav class="md-nav md-nav--primary" aria-label="Navigation" data-md-level="0">
   <label class="md-nav__title" for="__drawer">
-    <a href=".." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="../.." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     Alpha Documentation
   </label>
@@ -165,242 +165,452 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href=".." class="md-nav__link">
+      <a href="../.." class="md-nav__link">
         Home
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_setup/" class="md-nav__link">
+      <a href="../../alpha_setup/" class="md-nav__link">
         Setup
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
+      <a href="../../alpha_core/" class="md-nav__link">
         Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
+    
   
-    <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
-        Api
-      </a>
-    </li>
   
-
     
+    <li class="md-nav__item md-nav__item--active md-nav__item--nested">
       
       
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_4" type="checkbox" id="__nav_4" checked>
       
-
+      <label class="md-nav__link" for="__nav_4">
+        Api
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Api" data-md-level="1">
+        <label class="md-nav__title" for="__nav_4">
+          <span class="md-nav__icon md-icon"></span>
+          Api
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_screens/" class="md-nav__link">
-        Screens
+      <a href="../main/" class="md-nav__link">
+        Main
       </a>
     </li>
   
 
-    
-      
-      
-      
-
+          
+            
   
   
     
   
   
     <li class="md-nav__item md-nav__item--active">
       
       <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
       
-        
-      
       
         <label class="md-nav__link md-nav__link--active" for="__toc">
           Configuration
           <span class="md-nav__icon md-icon"></span>
         </label>
       
       <a href="./" class="md-nav__link md-nav__link--active">
         Configuration
       </a>
       
         
 <nav class="md-nav md-nav--secondary" aria-label="Table of contents">
   
   
-    
-  
   
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
-  <a href="#parameters" class="md-nav__link">
-    Parameters
-  </a>
-  
-    <nav class="md-nav" aria-label="Parameters">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
   <a href="#main" class="md-nav__link">
     Main
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#directories" class="md-nav__link">
-    Directories
+      
+        <li class="md-nav__item">
+  <a href="#mails" class="md-nav__link">
+    Mails
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#system-environments-variables" class="md-nav__link">
-    System environments variables
+      
+        <li class="md-nav__item">
+  <a href="#auth" class="md-nav__link">
+    Auth
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#environments-configurations" class="md-nav__link">
-    Environments configurations
+      
+        <li class="md-nav__item">
+  <a href="#reloader-type" class="md-nav__link">
+    Reloader type
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#users" class="md-nav__link">
-    Users
+      
+        <li class="md-nav__item">
+  <a href="#admin" class="md-nav__link">
+    Admin
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#platforms" class="md-nav__link">
-    Platforms
+      
+        <li class="md-nav__item">
+  <a href="#dashboard" class="md-nav__link">
+    Dashboard
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#loggers" class="md-nav__link">
-    Loggers
-  </a>
+      
+    </ul>
   
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#tests" class="md-nav__link">
-    Tests
-  </a>
+</nav>
+      
+    </li>
   
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#menu" class="md-nav__link">
-    Menu
-  </a>
+
+          
+            
   
-</li>
-        
-      </ul>
-    </nav>
   
-</li>
-      
-    </ul>
   
-</nav>
+    <li class="md-nav__item">
+      <a href="../routes/" class="md-nav__link">
+        Routes
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../parameters/" class="md-nav__link">
+        Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../methods/" class="md-nav__link">
+        Methods
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../cache/" class="md-nav__link">
+        Cache
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../authorizations/" class="md-nav__link">
+        Authorizations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../sqlalchemy/" class="md-nav__link">
+        SqlAlchemy
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../issues/" class="md-nav__link">
+        Issues
+      </a>
+    </li>
+  
+
+          
+        </ul>
+      </nav>
+    </li>
+  
+
+    
+      
       
+      
+
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../alpha_screens/" class="md-nav__link">
+        Screens
+      </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_database/" class="md-nav__link">
+      <a href="../../configuration/" class="md-nav__link">
+        Configuration
+      </a>
+    </li>
+  
+
+    
+      
+      
+      
+
+  
+  
+  
+    
+    <li class="md-nav__item md-nav__item--nested">
+      
+      
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_7" type="checkbox" id="__nav_7" >
+      
+      <label class="md-nav__link" for="__nav_7">
         Database
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Database" data-md-level="1">
+        <label class="md-nav__title" for="__nav_7">
+          <span class="md-nav__icon md-icon"></span>
+          Database
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../database/main/" class="md-nav__link">
+        Main
       </a>
     </li>
   
 
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../database/init/" class="md-nav__link">
+        Init
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../database/model/" class="md-nav__link">
+        Model
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../database/schema/" class="md-nav__link">
+        Schema
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../database/instantiate/" class="md-nav__link">
+        Instantiate
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../database/update/" class="md-nav__link">
+        Update
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../database/relations/" class="md-nav__link">
+        Relations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
+  
+
+          
+        </ul>
+      </nav>
+    </li>
+  
+
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../documentation/" class="md-nav__link">
+      <a href="../../documentation/" class="md-nav__link">
         Documentation
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_admin/" class="md-nav__link">
+      <a href="../../alpha_admin/" class="md-nav__link">
         Administration
       </a>
     </li>
   
 
     
   </ul>
@@ -414,222 +624,191 @@
               <div class="md-sidebar md-sidebar--secondary" data-md-component="sidebar" data-md-type="toc" >
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 <nav class="md-nav md-nav--secondary" aria-label="Table of contents">
   
   
-    
-  
   
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
-  <a href="#parameters" class="md-nav__link">
-    Parameters
-  </a>
-  
-    <nav class="md-nav" aria-label="Parameters">
-      <ul class="md-nav__list">
-        
-          <li class="md-nav__item">
   <a href="#main" class="md-nav__link">
     Main
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#directories" class="md-nav__link">
-    Directories
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#system-environments-variables" class="md-nav__link">
-    System environments variables
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#environments-configurations" class="md-nav__link">
-    Environments configurations
-  </a>
-  
-</li>
-        
-          <li class="md-nav__item">
-  <a href="#users" class="md-nav__link">
-    Users
+      
+        <li class="md-nav__item">
+  <a href="#mails" class="md-nav__link">
+    Mails
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#platforms" class="md-nav__link">
-    Platforms
+      
+        <li class="md-nav__item">
+  <a href="#auth" class="md-nav__link">
+    Auth
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#loggers" class="md-nav__link">
-    Loggers
+      
+        <li class="md-nav__item">
+  <a href="#reloader-type" class="md-nav__link">
+    Reloader type
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#tests" class="md-nav__link">
-    Tests
+      
+        <li class="md-nav__item">
+  <a href="#admin" class="md-nav__link">
+    Admin
   </a>
   
 </li>
-        
-          <li class="md-nav__item">
-  <a href="#menu" class="md-nav__link">
-    Menu
+      
+        <li class="md-nav__item">
+  <a href="#dashboard" class="md-nav__link">
+    Dashboard
   </a>
   
 </li>
-        
-      </ul>
-    </nav>
-  
-</li>
       
     </ul>
   
 </nav>
                   </div>
                 </div>
               </div>
             
           
           <div class="md-content" data-md-component="content">
             <article class="md-content__inner md-typeset">
               
                 
                 
-                <h1 id="dynamic-json-alpha-configuration-syntax">Dynamic json alpha configuration syntax</h1>
-<h2 id="parameters">Parameters</h2>
+                  <h1>Configuration</h1>
+                
+                <p>The api is automatically configured from the <code>api.jon</code> file. See <a href="./">Configuration</a> for further details on how to use it.</p>
 <h3 id="main">Main</h3>
 <ul>
-<li>project_name: in order to specify the project name</li>
+<li>workers: In order to specify the numbers of workers</li>
 </ul>
-<h3 id="directories">Directories</h3>
-<p>You must at least specify the <strong>root</strong> and <strong>home</strong> directories:</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;root&quot;</span><span class="p">:</span> <span class="s2">&quot;/application/{{user}}&quot;</span><span class="p">,</span>
-<span class="nt">&quot;home&quot;</span><span class="p">:</span> <span class="s2">&quot;/home/{{user}}&quot;</span><span class="p">,</span>
-</code></pre></div>
-<p>Other main directories could be defined in a sub <strong>directories</strong> path:</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;directories&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;data&quot;</span><span class="p">:</span> <span class="s2">&quot;{{root}}/data&quot;</span><span class="p">,</span>
-    <span class="nt">&quot;logs&quot;</span><span class="p">:</span> <span class="s2">&quot;{{root}}/logs&quot;</span><span class="p">,</span>
-    <span class="nt">&quot;cache&quot;</span><span class="p">:</span> <span class="s2">&quot;{{root}}/cache&quot;</span>
-<span class="p">}</span>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;workers&quot;</span><span class="p">:</span> <span class="mi">6</span>
 </code></pre></div>
-<h3 id="system-environments-variables">System environments variables</h3>
-<p>In order to set operating system environment variables</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;envs&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;ORACLE_HOME&quot;</span><span class="p">:</span> <span class="s2">&quot;/application/software/oracle/12.1.0.2&quot;</span>
-<span class="p">}</span>
+<ul>
+<li>routes_no_log: In order to specify the routes where log must be ignored</li>
+</ul>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;routes_no_log&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;//status&quot;</span><span class="p">,</span> <span class="s2">&quot;//static&quot;</span><span class="p">,</span> <span class="s2">&quot;//dashboard&quot;</span><span class="p">],</span>
 </code></pre></div>
-<h3 id="environments-configurations">Environments configurations</h3>
-<p>In order to specify the envs configurations:</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;configuration&quot;</span><span class="p">:</span> <span class="s2">&quot;local&quot;</span><span class="p">,</span>
-<span class="nt">&quot;configurations&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;local&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;debug&quot;</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
-        <span class="nt">&quot;host_public&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;host_web&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;port&quot;</span><span class="p">:</span> <span class="mi">5006</span><span class="p">,</span>
-        <span class="nt">&quot;ssl_cert&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;ssl_key&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;admin&quot;</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
-        <span class="nt">&quot;admin_databases&quot;</span><span class="p">:</span> <span class="kc">true</span>
-    <span class="p">},</span>
-    <span class="nt">&quot;dev&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;debug&quot;</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
-        <span class="nt">&quot;host_public&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;host_web&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;port&quot;</span><span class="p">:</span> <span class="mi">5000</span><span class="p">,</span>
-        <span class="nt">&quot;ssl_cert&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;ssl_key&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;admin&quot;</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
-        <span class="nt">&quot;admin_databases&quot;</span><span class="p">:</span> <span class="kc">true</span>
-    <span class="p">}</span>
+<ul>
+<li>models: In order to specify the <strong>Flask-SqlAlchemy</strong> models definitions paths</li>
+</ul>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;models&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;models.databases&quot;</span><span class="p">]</span>
+</code></pre></div>
+<ul>
+<li>routes: In order to specify the routes definitions paths</li>
+</ul>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;routes&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;apis.routes&quot;</span><span class="p">]</span>
+</code></pre></div>
+<ul>
+<li>ssl: In order to activate ssl mode</li>
+</ul>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;ssl&quot;</span><span class="p">:</span> <span class="kc">false</span>
+</code></pre></div>
+<ul>
+<li>threaded: In order to activate the threaded mode</li>
+</ul>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;threaded&quot;</span><span class="p">:</span> <span class="kc">false</span>
+</code></pre></div>
+<ul>
+<li>config: In order to activate pass configuration to Flask <strong>api</strong> class</li>
+</ul>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;config&quot;</span><span class="p">:</span> <span class="p">{</span>
+    <span class="nt">&quot;MYSQL_DATABASE_CHARSET&quot;</span><span class="p">:</span> <span class="s2">&quot;utf8mb4&quot;</span><span class="p">,</span>
+    <span class="nt">&quot;SQLALCHEMY_TRACK_MODIFICATIONS&quot;</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
+    <span class="nt">&quot;SQLALCHEMY_POOL_RECYCLE&quot;</span><span class="p">:</span> <span class="mi">299</span><span class="p">,</span>
+    <span class="nt">&quot;SQLALCHEMY_POOL_TIMEOUT&quot;</span><span class="p">:</span> <span class="mi">30</span><span class="p">,</span>
+    <span class="nt">&quot;SQLALCHEMY_POOL_SIZE&quot;</span><span class="p">:</span> <span class="mi">10</span><span class="p">,</span>
+    <span class="nt">&quot;JWT_SECRET_KEY&quot;</span><span class="p">:</span> <span class="s2">&quot;a_secret_key&quot;</span><span class="p">,</span>
+    <span class="nt">&quot;JSON_SORT_KEYS&quot;</span><span class="p">:</span> <span class="kc">false</span>
 <span class="p">}</span>
 </code></pre></div>
-<p><strong>configuration</strong> parameter is the default one.</p>
-<h3 id="users">Users</h3>
-<p>Configuration could be modified dynamically depending on the user</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;users&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;user_dev&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;debug&quot;</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
-        <span class="nt">&quot;mode&quot;</span><span class="p">:</span> <span class="s2">&quot;wsgi&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;configuration&quot;</span><span class="p">:</span> <span class="s2">&quot;dev&quot;</span>
-    <span class="p">},</span>
-    <span class="nt">&quot;user_int&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;debug&quot;</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
-        <span class="nt">&quot;mode&quot;</span><span class="p">:</span> <span class="s2">&quot;wsgi&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;configuration&quot;</span><span class="p">:</span> <span class="s2">&quot;int&quot;</span>
-    <span class="p">},</span>
-    <span class="nt">&quot;user_acc&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;debug&quot;</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
-        <span class="nt">&quot;mode&quot;</span><span class="p">:</span> <span class="s2">&quot;wsgi&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;configuration&quot;</span><span class="p">:</span> <span class="s2">&quot;acc&quot;</span>
-    <span class="p">},</span>
-    <span class="nt">&quot;user_prod&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;debug&quot;</span><span class="p">:</span> <span class="kc">false</span><span class="p">,</span>
-        <span class="nt">&quot;mode&quot;</span><span class="p">:</span> <span class="s2">&quot;wsgi&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;configuration&quot;</span><span class="p">:</span> <span class="s2">&quot;prod&quot;</span>
+<h3 id="mails">Mails</h3>
+<p>In order to specify the mails configurations</p>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;mails&quot;</span><span class="p">:</span> <span class="p">{</span>
+    <span class="nt">&quot;mail_server&quot;</span><span class="p">:</span> <span class="p">{</span>
+        <span class="nt">&quot;host&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;mail&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;password&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;port&quot;</span><span class="p">:</span> <span class="mi">465</span><span class="p">,</span>
+        <span class="nt">&quot;server&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;ssl&quot;</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
+        <span class="nt">&quot;tls&quot;</span><span class="p">:</span> <span class="kc">false</span>
     <span class="p">}</span>
 <span class="p">}</span>
 </code></pre></div>
-<h3 id="platforms">Platforms</h3>
-<p>Configuration could be modified dynamically depending on the operating system</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;platforms&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;windows&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;root&quot;</span><span class="p">:</span> <span class="s2">&quot;/alpha/{{user}}&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;home&quot;</span><span class="p">:</span> <span class="s2">&quot;/alpha/{{user}}&quot;</span><span class="p">,</span>
-        <span class="nt">&quot;host&quot;</span><span class="p">:</span> <span class="s2">&quot;0.0.0.0&quot;</span>
+<h3 id="auth">Auth</h3>
+<p>In order to specify the auth mode</p>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;auth&quot;</span><span class="p">:</span> <span class="p">{</span>
+    <span class="nt">&quot;mode&quot;</span><span class="p">:</span> <span class="s2">&quot;ldap&quot;</span><span class="p">,</span>
+    <span class="nt">&quot;ldap&quot;</span><span class="p">:</span> <span class="p">{</span>
+        <span class="nt">&quot;server&quot;</span><span class="p">:</span> <span class="s2">&quot;ldap://path_to_ldap&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;baseDN&quot;</span><span class="p">:</span> <span class="s2">&quot;ou=people,dc=a_name,dc=com&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;users_filters&quot;</span><span class="p">:</span> <span class="s2">&quot;(|(uid={uid})(mail={mail})(cn={cn}))&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;user_filters&quot;</span><span class="p">:</span> <span class="s2">&quot;(|(uid={username})(mail={username})(cn={username}))&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;user_data&quot;</span><span class="p">:</span> <span class="p">{</span>
+            <span class="nt">&quot;givenName&quot;</span><span class="p">:</span> <span class="s2">&quot;name&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;sn&quot;</span><span class="p">:</span> <span class="s2">&quot;lastname&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;c&quot;</span><span class="p">:</span> <span class="s2">&quot;area&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;st-locationdescription&quot;</span><span class="p">:</span> <span class="s2">&quot;location&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;st-seatnumber&quot;</span><span class="p">:</span> <span class="s2">&quot;seat&quot;</span><span class="p">,</span>
+            <span class="nt">&quot;telephoneNumber&quot;</span><span class="p">:</span> <span class="s2">&quot;phone-number&quot;</span>
+        <span class="p">}</span>
+    <span class="p">},</span>
+    <span class="nt">&quot;users&quot;</span><span class="p">:</span> <span class="p">{</span>
+        <span class="nt">&quot;a_user_name&quot;</span><span class="p">:</span> <span class="p">{</span>
+            <span class="nt">&quot;user_permissions&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;SUPER_USER&quot;</span><span class="p">]</span>
+        <span class="p">}</span>
     <span class="p">}</span>
 <span class="p">},</span>
 </code></pre></div>
-<h3 id="loggers">Loggers</h3>
-<p>In order the specify the loggers configurations:</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;loggers&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;main&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;level&quot;</span><span class="p">:</span> <span class="s2">&quot;debug&quot;</span>
+<h3 id="reloader-type">Reloader type</h3>
+<p>In order to specify the <a href="https://werkzeug.palletsprojects.com/en/2.1.x/">Werkzeug</a> reloader type</p>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;reloader_type&quot;</span><span class="p">:</span> <span class="s2">&quot;stat&quot;</span>
+</code></pre></div>
+<h3 id="admin">Admin</h3>
+<p>In order to specify the admins configurations</p>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;admins&quot;</span><span class="p">:</span> <span class="p">{</span><span class="nt">&quot;ips&quot;</span><span class="p">:[</span><span class="s2">&quot;127.0.0.1&quot;</span><span class="p">],</span> <span class="nt">&quot;password&quot;</span><span class="p">:</span><span class="s2">&quot;a_password&quot;</span><span class="p">},</span>
+</code></pre></div>
+<h3 id="dashboard">Dashboard</h3>
+<p>In order to configure the <a href="https://flask-monitoringdashboard.readthedocs.io/">Flask-Monitoring Dashboard</a></p>
+<div class="highlight"><pre><span></span><code><span class="nt">&quot;dashboard&quot;</span><span class="p">:</span> <span class="p">{</span>
+    <span class="nt">&quot;dashboard&quot;</span><span class="p">:</span> <span class="p">{</span>
+        <span class="nt">&quot;APP_VERSION&quot;</span><span class="p">:</span> <span class="mf">1.0</span><span class="p">,</span>
+        <span class="nt">&quot;SAMPLING_PERIOD&quot;</span><span class="p">:</span> <span class="mi">20</span><span class="p">,</span>
+        <span class="nt">&quot;ENABLE_LOGGING&quot;</span><span class="p">:</span> <span class="kc">true</span><span class="p">,</span>
+        <span class="nt">&quot;active&quot;</span><span class="p">:</span> <span class="kc">false</span>
+    <span class="p">},</span>
+    <span class="nt">&quot;authentication&quot;</span><span class="p">:</span> <span class="p">{</span>
+        <span class="nt">&quot;USERNAME&quot;</span><span class="p">:</span> <span class="s2">&quot;username&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;PASSWORD&quot;</span><span class="p">:</span> <span class="s2">&quot;&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;GUEST_USERNAME&quot;</span><span class="p">:</span> <span class="s2">&quot;guest&quot;</span><span class="p">,</span>
+        <span class="nt">&quot;GUEST_PASSWORD&quot;</span><span class="p">:</span> <span class="p">[</span><span class="s2">&quot;guest1&quot;</span><span class="p">,</span> <span class="s2">&quot;guest2&quot;</span><span class="p">],</span>
+        <span class="nt">&quot;SECURITY_TOKEN&quot;</span><span class="p">:</span> <span class="s2">&quot;a_security_token&quot;</span>
     <span class="p">},</span>
     <span class="nt">&quot;database&quot;</span><span class="p">:</span> <span class="p">{</span>
-        <span class="nt">&quot;level&quot;</span><span class="p">:</span> <span class="s2">&quot;debug&quot;</span>
+        <span class="nt">&quot;DATABASE&quot;</span><span class="p">:</span> <span class="s2">&quot;sqlite:///{{root}}/dashboard.db&quot;</span>
     <span class="p">}</span>
 <span class="p">}</span>
 </code></pre></div>
-<h3 id="tests">Tests</h3>
-<p>In order to specify the directories that contains tests:</p>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;tests&quot;</span> <span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;auto_directory&quot;</span><span class="p">:</span> <span class="s2">&quot;tests/auto&quot;</span><span class="p">,</span>
-    <span class="nt">&quot;auto_import&quot;</span><span class="p">:</span> <span class="s2">&quot;alphaz.tests.auto&quot;</span><span class="p">,</span>
-    <span class="nt">&quot;save_directory&quot;</span><span class="p">:</span> <span class="s2">&quot;{{save_root}}/tests&quot;</span>
-<span class="p">},</span>
-</code></pre></div>
-<h3 id="menu">Menu</h3>
-<div class="highlight"><pre><span></span><code><span class="nt">&quot;menus&quot;</span><span class="p">:</span> <span class="p">{</span>
-    <span class="nt">&quot;save_directory&quot;</span><span class="p">:</span> <span class="s2">&quot;{{save_root}}/menus&quot;</span>
-<span class="p">},</span>
-</code></pre></div>
                 
               
               
                 
 
 
               
@@ -640,36 +819,36 @@
       </main>
       
         
 <footer class="md-footer">
   
     <nav class="md-footer__inner md-grid" aria-label="Footer">
       
-        <a href="../alpha_screens/" class="md-footer__link md-footer__link--prev" rel="prev">
+        <a href="../main/" class="md-footer__link md-footer__link--prev" rel="prev">
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12z"/></svg>
           </div>
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Previous
               </span>
-              Screens
+              Main
             </div>
           </div>
         </a>
       
       
-        <a href="../alpha_database/" class="md-footer__link md-footer__link--next" rel="next">
+        <a href="../routes/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Next
               </span>
-              Database
+              Routes
             </div>
           </div>
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4z"/></svg>
           </div>
         </a>
       
@@ -690,15 +869,15 @@
   </div>
 </footer>
       
     </div>
     <div class="md-dialog" data-md-component="dialog">
       <div class="md-dialog__inner md-typeset"></div>
     </div>
-    <script id="__config" type="application/json">{"base": "..", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "../assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
+    <script id="__config" type="application/json">{"base": "../..", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "../../assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
     
     
-      <script src="../assets/javascripts/bundle.7353b375.min.js"></script>
+      <script src="../../assets/javascripts/bundle.7353b375.min.js"></script>
       
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -14,139 +14,139 @@
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
     * Core
-    * Api
-    * Screens
-    * ⁰  Configuration   Configuration    Table of contents
-          o Parameters
+    * *  Api      Api
+          o Main
+          o ⁰  Configuration   Configuration    Table of contents
                 # Main
-                # Directories
-                # System_environments_variables
-                # Environments_configurations
-                # Users
-                # Platforms
-                # Loggers
-                # Tests
-                # Menu
-    * Database
+                # Mails
+                # Auth
+                # Reloader_type
+                # Admin
+                # Dashboard
+          o Routes
+          o Parameters
+          o Model_Parameters
+          o Methods
+          o Cache
+          o Authorizations
+          o SqlAlchemy
+          o Issues
+    * Screens
+    * Configuration
+    * ⁰  Database      Database
+          o Main
+          o Init
+          o Model
+          o Schema
+          o Instantiate
+          o Update
+          o Relations
+          o Model_Parameters
     * Documentation
     * Administration
    Table of contents
-    * Parameters
-          o Main
-          o Directories
-          o System_environments_variables
-          o Environments_configurations
-          o Users
-          o Platforms
-          o Loggers
-          o Tests
-          o Menu
-****** Dynamic json alpha configuration syntax ******
-***** Parameters *****
+    * Main
+    * Mails
+    * Auth
+    * Reloader_type
+    * Admin
+    * Dashboard
+****** Configuration ******
+The api is automatically configured from the api.jon file. See Configuration
+for further details on how to use it.
 **** Main ****
-    * project_name: in order to specify the project name
-**** Directories ****
-You must at least specify the root and home directories:
-"root": "/application/{{user}}",
-"home": "/home/{{user}}",
-Other main directories could be defined in a sub directories path:
-"directories": {
-    "data": "{{root}}/data",
-    "logs": "{{root}}/logs",
-    "cache": "{{root}}/cache"
-}
-**** System environments variables ****
-In order to set operating system environment variables
-"envs": {
-    "ORACLE_HOME": "/application/software/oracle/12.1.0.2"
+    * workers: In order to specify the numbers of workers
+"workers": 6
+    * routes_no_log: In order to specify the routes where log must be ignored
+"routes_no_log": ["//status", "//static", "//dashboard"],
+    * models: In order to specify the Flask-SqlAlchemy models definitions paths
+"models": ["models.databases"]
+    * routes: In order to specify the routes definitions paths
+"routes": ["apis.routes"]
+    * ssl: In order to activate ssl mode
+"ssl": false
+    * threaded: In order to activate the threaded mode
+"threaded": false
+    * config: In order to activate pass configuration to Flask api class
+"config": {
+    "MYSQL_DATABASE_CHARSET": "utf8mb4",
+    "SQLALCHEMY_TRACK_MODIFICATIONS": false,
+    "SQLALCHEMY_POOL_RECYCLE": 299,
+    "SQLALCHEMY_POOL_TIMEOUT": 30,
+    "SQLALCHEMY_POOL_SIZE": 10,
+    "JWT_SECRET_KEY": "a_secret_key",
+    "JSON_SORT_KEYS": false
 }
-**** Environments configurations ****
-In order to specify the envs configurations:
-"configuration": "local",
-"configurations": {
-    "local": {
-        "debug": true,
-        "host_public": "",
-        "host_web": "",
-        "port": 5006,
-        "ssl_cert": "",
-        "ssl_key": "",
-        "admin": true,
-        "admin_databases": true
-    },
-    "dev": {
-        "debug": true,
-        "host_public": "",
-        "host_web": "",
-        "port": 5000,
-        "ssl_cert": "",
-        "ssl_key": "",
-        "admin": true,
-        "admin_databases": true
+**** Mails ****
+In order to specify the mails configurations
+"mails": {
+    "mail_server": {
+        "host": "",
+        "mail": "",
+        "password": "",
+        "port": 465,
+        "server": "",
+        "ssl": true,
+        "tls": false
     }
 }
-configuration parameter is the default one.
-**** Users ****
-Configuration could be modified dynamically depending on the user
-"users": {
-    "user_dev": {
-        "debug": false,
-        "mode": "wsgi",
-        "configuration": "dev"
-    },
-    "user_int": {
-        "debug": false,
-        "mode": "wsgi",
-        "configuration": "int"
+**** Auth ****
+In order to specify the auth mode
+"auth": {
+    "mode": "ldap",
+    "ldap": {
+        "server": "ldap://path_to_ldap",
+        "baseDN": "ou=people,dc=a_name,dc=com",
+        "users_filters": "(|(uid={uid})(mail={mail})(cn={cn}))",
+        "user_filters": "(|(uid={username})(mail={username})(cn={username}))",
+        "user_data": {
+            "givenName": "name",
+            "sn": "lastname",
+            "c": "area",
+            "st-locationdescription": "location",
+            "st-seatnumber": "seat",
+            "telephoneNumber": "phone-number"
+        }
     },
-    "user_acc": {
-        "debug": false,
-        "mode": "wsgi",
-        "configuration": "acc"
-    },
-    "user_prod": {
-        "debug": false,
-        "mode": "wsgi",
-        "configuration": "prod"
-    }
-}
-**** Platforms ****
-Configuration could be modified dynamically depending on the operating system
-"platforms": {
-    "windows": {
-        "root": "/alpha/{{user}}",
-        "home": "/alpha/{{user}}",
-        "host": "0.0.0.0"
+    "users": {
+        "a_user_name": {
+            "user_permissions": ["SUPER_USER"]
+        }
     }
 },
-**** Loggers ****
-In order the specify the loggers configurations:
-"loggers": {
-    "main": {
-        "level": "debug"
+**** Reloader type ****
+In order to specify the Werkzeug reloader type
+"reloader_type": "stat"
+**** Admin ****
+In order to specify the admins configurations
+"admins": {"ips":["127.0.0.1"], "password":"a_password"},
+**** Dashboard ****
+In order to configure the Flask-Monitoring_Dashboard
+"dashboard": {
+    "dashboard": {
+        "APP_VERSION": 1.0,
+        "SAMPLING_PERIOD": 20,
+        "ENABLE_LOGGING": true,
+        "active": false
+    },
+    "authentication": {
+        "USERNAME": "username",
+        "PASSWORD": "",
+        "GUEST_USERNAME": "guest",
+        "GUEST_PASSWORD": ["guest1", "guest2"],
+        "SECURITY_TOKEN": "a_security_token"
     },
     "database": {
-        "level": "debug"
+        "DATABASE": "sqlite:///{{root}}/dashboard.db"
     }
 }
-**** Tests ****
-In order to specify the directories that contains tests:
-"tests" : {
-    "auto_directory": "tests/auto",
-    "auto_import": "alphaz.tests.auto",
-    "save_directory": "{{save_root}}/tests"
-},
-**** Menu ****
-"menus": {
-    "save_directory": "{{save_root}}/menus"
-},
 
- Previous__Screens
+ Previous__Main
 
- Next__Database
+ Next__Routes
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/documentation/index.html` & `alphaz-0.7.4/alphaz/documentations/site/database/schema/index.html`

 * *Files 27% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width,initial-scale=1">
       
       
       
       
-      <link rel="icon" href="../assets/images/favicon.png">
+      <link rel="icon" href="../../assets/images/favicon.png">
       <meta name="generator" content="mkdocs-1.1.2, mkdocs-material-7.1.1">
     
     
       
-        <title>Documentation - Alpha Documentation</title>
+        <title>Schema - Alpha Documentation</title>
       
     
     
-      <link rel="stylesheet" href="../assets/stylesheets/main.9299cb39.min.css">
+      <link rel="stylesheet" href="../../assets/stylesheets/main.9299cb39.min.css">
       
         
-        <link rel="stylesheet" href="../assets/stylesheets/palette.ef6f36e2.min.css">
+        <link rel="stylesheet" href="../../assets/stylesheets/palette.ef6f36e2.min.css">
         
       
     
     
     
       
         
@@ -47,34 +47,34 @@
     
     
     
     
     <body dir="ltr" data-md-color-scheme="" data-md-color-primary="none" data-md-color-accent="none">
   
     
-    <script>function __prefix(e){return new URL("..",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
+    <script>function __prefix(e){return new URL("../..",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
     
     <input class="md-toggle" data-md-toggle="drawer" type="checkbox" id="__drawer" autocomplete="off">
     <input class="md-toggle" data-md-toggle="search" type="checkbox" id="__search" autocomplete="off">
     <label class="md-overlay" for="__drawer"></label>
     <div data-md-component="skip">
       
         
-        <a href="#documentation" class="md-skip">
+        <a href="#specific-schema" class="md-skip">
           Skip to content
         </a>
       
     </div>
     <div data-md-component="announce">
       
     </div>
     
       <header class="md-header" data-md-component="header">
   <nav class="md-header__inner md-grid" aria-label="Header">
-    <a href=".." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="../.." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     <label class="md-header__button md-icon" for="__drawer">
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M3 6h18v2H3V6m0 5h18v2H3v-2m0 5h18v2H3v-2z"/></svg>
@@ -85,15 +85,15 @@
           <span class="md-ellipsis">
             Alpha Documentation
           </span>
         </div>
         <div class="md-header__topic" data-md-component="header-topic">
           <span class="md-ellipsis">
             
-              Documentation
+              Schema
             
           </span>
         </div>
       </div>
     </div>
     
     
@@ -146,15 +146,15 @@
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 
 
 <nav class="md-nav md-nav--primary" aria-label="Navigation" data-md-level="0">
   <label class="md-nav__title" for="__drawer">
-    <a href=".." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="../.." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     Alpha Documentation
   </label>
@@ -165,180 +165,392 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href=".." class="md-nav__link">
+      <a href="../.." class="md-nav__link">
         Home
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_setup/" class="md-nav__link">
+      <a href="../../alpha_setup/" class="md-nav__link">
         Setup
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
+      <a href="../../alpha_core/" class="md-nav__link">
         Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
-    <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
+    
+    <li class="md-nav__item md-nav__item--nested">
+      
+      
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_4" type="checkbox" id="__nav_4" >
+      
+      <label class="md-nav__link" for="__nav_4">
         Api
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Api" data-md-level="1">
+        <label class="md-nav__title" for="__nav_4">
+          <span class="md-nav__icon md-icon"></span>
+          Api
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/main/" class="md-nav__link">
+        Main
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/configuration/" class="md-nav__link">
+        Configuration
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/routes/" class="md-nav__link">
+        Routes
       </a>
     </li>
   
 
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/parameters/" class="md-nav__link">
+        Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/methods/" class="md-nav__link">
+        Methods
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/cache/" class="md-nav__link">
+        Cache
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/authorizations/" class="md-nav__link">
+        Authorizations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/sqlalchemy/" class="md-nav__link">
+        SqlAlchemy
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/issues/" class="md-nav__link">
+        Issues
+      </a>
+    </li>
+  
+
+          
+        </ul>
+      </nav>
+    </li>
+  
+
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_screens/" class="md-nav__link">
+      <a href="../../alpha_screens/" class="md-nav__link">
         Screens
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../configuration/" class="md-nav__link">
+      <a href="../../configuration/" class="md-nav__link">
         Configuration
       </a>
     </li>
   
 
     
       
       
       
 
   
   
+    
   
-    <li class="md-nav__item">
-      <a href="../alpha_database/" class="md-nav__link">
-        Database
-      </a>
-    </li>
   
-
     
+    <li class="md-nav__item md-nav__item--active md-nav__item--nested">
       
       
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_7" type="checkbox" id="__nav_7" checked>
       
+      <label class="md-nav__link" for="__nav_7">
+        Database
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Database" data-md-level="1">
+        <label class="md-nav__title" for="__nav_7">
+          <span class="md-nav__icon md-icon"></span>
+          Database
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../main/" class="md-nav__link">
+        Main
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../init/" class="md-nav__link">
+        Init
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../model/" class="md-nav__link">
+        Model
+      </a>
+    </li>
+  
 
+          
+            
   
   
     
   
   
     <li class="md-nav__item md-nav__item--active">
       
       <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
       
         
       
       
-        <label class="md-nav__link md-nav__link--active" for="__toc">
-          Documentation
-          <span class="md-nav__icon md-icon"></span>
-        </label>
-      
       <a href="./" class="md-nav__link md-nav__link--active">
-        Documentation
+        Schema
       </a>
       
-        
-<nav class="md-nav md-nav--secondary" aria-label="Table of contents">
+    </li>
   
+
+          
+            
   
-    
   
   
-    <label class="md-nav__title" for="__toc">
-      <span class="md-nav__icon md-icon"></span>
-      Table of contents
-    </label>
-    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
-      
-        <li class="md-nav__item">
-  <a href="#requirements" class="md-nav__link">
-    Requirements
-  </a>
+    <li class="md-nav__item">
+      <a href="../instantiate/" class="md-nav__link">
+        Instantiate
+      </a>
+    </li>
   
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#more" class="md-nav__link">
-    More
-  </a>
+
+          
+            
   
-</li>
-      
-    </ul>
   
-</nav>
+  
+    <li class="md-nav__item">
+      <a href="../update/" class="md-nav__link">
+        Update
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../relations/" class="md-nav__link">
+        Relations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
+  
+
+          
+        </ul>
+      </nav>
+    </li>
+  
+
+    
+      
       
+      
+
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../documentation/" class="md-nav__link">
+        Documentation
+      </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_admin/" class="md-nav__link">
+      <a href="../../alpha_admin/" class="md-nav__link">
         Administration
       </a>
     </li>
   
 
     
   </ul>
@@ -355,66 +567,67 @@
                     
 <nav class="md-nav md-nav--secondary" aria-label="Table of contents">
   
   
     
   
   
-    <label class="md-nav__title" for="__toc">
-      <span class="md-nav__icon md-icon"></span>
-      Table of contents
-    </label>
-    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
-      
-        <li class="md-nav__item">
-  <a href="#requirements" class="md-nav__link">
-    Requirements
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#more" class="md-nav__link">
-    More
-  </a>
-  
-</li>
-      
-    </ul>
-  
 </nav>
                   </div>
                 </div>
               </div>
             
           
           <div class="md-content" data-md-component="content">
             <article class="md-content__inner md-typeset">
               
                 
                 
-                <h1 id="documentation">Documentation</h1>
-<h2 id="requirements">Requirements</h2>
+                <div class="admonition note">
+<p class="admonition-title">Note</p>
+</div>
+<p>The associated Schema is created automatically, with classic and nested fields.</p>
+<p>However Marshmallow schema could be defined using the classic way <a href="https://marshmallow.readthedocs.io/en/stable/index.html">Marshmallow</a>:</p>
 <ul>
-<li>install packages</li>
+<li>Set visible to <strong>False</strong> if you dont want the column to appears in the Schema.</li>
 </ul>
-<div class="highlight"><pre><span></span><code>pip install pymdown-extensions pygments mkdocs-material
+<div class="admonition important">
+<p class="admonition-title">Important</p>
+</div>
+<p>Schema must be defined after the Model</p>
+<div class="highlight"><pre><span></span><code><span class="n">DB</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span>
+
+<span class="k">class</span> <span class="nc">DuckTypeSchema</span><span class="p">(</span><span class="n">Schema</span><span class="p">):</span>
+    <span class="n">type_id</span> <span class="o">=</span> <span class="n">fields</span><span class="o">.</span><span class="n">Integer</span><span class="p">()</span>
+    <span class="n">name</span> <span class="o">=</span> <span class="n">fields</span><span class="o">.</span><span class="n">String</span><span class="p">()</span>
+
+<span class="k">class</span> <span class="nc">DuckMedalSchema</span><span class="p">(</span><span class="n">Schema</span><span class="p">):</span>
+    <span class="n">name</span> <span class="o">=</span> <span class="n">fields</span><span class="o">.</span><span class="n">String</span><span class="p">()</span>
+
+<span class="k">class</span> <span class="nc">DuckSchema</span><span class="p">(</span><span class="n">Schema</span><span class="p">):</span>
+    <span class="n">name</span> <span class="o">=</span> <span class="n">fields</span><span class="o">.</span><span class="n">String</span><span class="p">()</span>
+
+    <span class="c1"># Many to One</span>
+    <span class="n">duck_type</span> <span class="o">=</span> <span class="n">fields</span><span class="o">.</span><span class="n">Nested</span><span class="p">(</span><span class="n">DuckTypeSchema</span><span class="p">)</span>
+
+    <span class="c1"># One to many</span>
+    <span class="n">medals</span> <span class="o">=</span> <span class="n">fields</span><span class="o">.</span><span class="n">List</span><span class="p">(</span><span class="n">fields</span><span class="o">.</span><span class="n">Nested</span><span class="p">(</span><span class="n">DuckMedalSchema</span><span class="p">))</span>
 </code></pre></div>
-<ul>
-<li>Add extensions in <strong>mkdocs.yaml</strong></li>
-</ul>
-<div class="highlight"><pre><span></span><code>markdown_extensions:
-  - admonition
-  - pymdownx.arithmatex
-  - pymdownx.details
-  - codehilite
-  - pymdownx.superfences
+<div class="admonition important">
+<p class="admonition-title">Important</p>
+</div>
+<p><strong>Alpha</strong> will automatically detect the schema if the name is defined as <code>"{ModelName}Schema"</code> and is located in the same file.</p>
+<div class="admonition note">
+<p class="admonition-title">Note</p>
+</div>
+<p>In this mode, Schema could be defined automatically, excepted for nested fields.</p>
+<h1 id="specific-schema">Specific Schema</h1>
+<p>Schema could be specified for every request:</p>
+<div class="highlight"><pre><span></span><code><span class="n">DB</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="n">model</span>  <span class="o">=</span> <span class="n">Duck</span><span class="p">,</span> <span class="n">schema</span> <span class="o">=</span> <span class="n">DuckSchema</span><span class="p">)</span>
 </code></pre></div>
-<h2 id="more">More</h2>
-<p><a href="https://pjjk.net/mdmkdocs/extensions/">for more information</a></p>
                 
               
               
                 
 
 
               
@@ -425,36 +638,36 @@
       </main>
       
         
 <footer class="md-footer">
   
     <nav class="md-footer__inner md-grid" aria-label="Footer">
       
-        <a href="../alpha_database/" class="md-footer__link md-footer__link--prev" rel="prev">
+        <a href="../model/" class="md-footer__link md-footer__link--prev" rel="prev">
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12z"/></svg>
           </div>
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Previous
               </span>
-              Database
+              Model
             </div>
           </div>
         </a>
       
       
-        <a href="../alpha_admin/" class="md-footer__link md-footer__link--next" rel="next">
+        <a href="../instantiate/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Next
               </span>
-              Administration
+              Instantiate
             </div>
           </div>
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4z"/></svg>
           </div>
         </a>
       
@@ -475,15 +688,15 @@
   </div>
 </footer>
       
     </div>
     <div class="md-dialog" data-md-component="dialog">
       <div class="md-dialog__inner md-typeset"></div>
     </div>
-    <script id="__config" type="application/json">{"base": "..", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "../assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
+    <script id="__config" type="application/json">{"base": "../..", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "../../assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
     
     
-      <script src="../assets/javascripts/bundle.7353b375.min.js"></script>
+      <script src="../../assets/javascripts/bundle.7353b375.min.js"></script>
       
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -5,46 +5,80 @@
 
 
 
  ⁰ ⁰
 Skip_to_content
 
  Alpha Documentation
- Documentation
+ Schema
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
     * Core
-    * Api
+    * ⁰  Api      Api
+          o Main
+          o Configuration
+          o Routes
+          o Parameters
+          o Model_Parameters
+          o Methods
+          o Cache
+          o Authorizations
+          o SqlAlchemy
+          o Issues
     * Screens
     * Configuration
-    * Database
-    * ⁰  Documentation   Documentation    Table of contents
-          o Requirements
-          o More
+    * *  Database      Database
+          o Main
+          o Init
+          o Model
+          o ⁰ Schema
+          o Instantiate
+          o Update
+          o Relations
+          o Model_Parameters
+    * Documentation
     * Administration
-   Table of contents
-    * Requirements
-    * More
-****** Documentation ******
-***** Requirements *****
-    * install packages
-pip install pymdown-extensions pygments mkdocs-material
-    * Add extensions in mkdocs.yaml
-markdown_extensions:
-  - admonition
-  - pymdownx.arithmatex
-  - pymdownx.details
-  - codehilite
-  - pymdownx.superfences
-***** More *****
-for_more_information
 
- Previous__Database
+Note
+The associated Schema is created automatically, with classic and nested fields.
+However Marshmallow schema could be defined using the classic way Marshmallow:
+    * Set visible to False if you dont want the column to appears in the
+      Schema.
+Important
+Schema must be defined after the Model
+DB = core.db
+
+class DuckTypeSchema(Schema):
+    type_id = fields.Integer()
+    name = fields.String()
+
+class DuckMedalSchema(Schema):
+    name = fields.String()
+
+class DuckSchema(Schema):
+    name = fields.String()
+
+    # Many to One
+    duck_type = fields.Nested(DuckTypeSchema)
+
+    # One to many
+    medals = fields.List(fields.Nested(DuckMedalSchema))
+Important
+Alpha will automatically detect the schema if the name is defined as "
+{ModelName}Schema" and is located in the same file.
+Note
+In this mode, Schema could be defined automatically, excepted for nested
+fields.
+****** Specific Schema ******
+Schema could be specified for every request:
+DB.select(model  = Duck, schema = DuckSchema)
 
- Next__Administration
+ Previous__Model
+
+ Next__Instantiate
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/index.html` & `alphaz-0.7.4/alphaz/documentations/site/database/model/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     
       <meta charset="utf-8">
       <meta name="viewport" content="width=device-width,initial-scale=1">
       
       
       
       
-      <link rel="icon" href="assets/images/favicon.png">
+      <link rel="icon" href="../../assets/images/favicon.png">
       <meta name="generator" content="mkdocs-1.1.2, mkdocs-material-7.1.1">
     
     
       
-        <title>Alpha Documentation</title>
+        <title>Model - Alpha Documentation</title>
       
     
     
-      <link rel="stylesheet" href="assets/stylesheets/main.9299cb39.min.css">
+      <link rel="stylesheet" href="../../assets/stylesheets/main.9299cb39.min.css">
       
         
-        <link rel="stylesheet" href="assets/stylesheets/palette.ef6f36e2.min.css">
+        <link rel="stylesheet" href="../../assets/stylesheets/palette.ef6f36e2.min.css">
         
       
     
     
     
       
         
@@ -47,34 +47,34 @@
     
     
     
     
     <body dir="ltr" data-md-color-scheme="" data-md-color-primary="none" data-md-color-accent="none">
   
     
-    <script>function __prefix(e){return new URL(".",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
+    <script>function __prefix(e){return new URL("../..",location).pathname+"."+e}function __get(e,t=localStorage){return JSON.parse(t.getItem(__prefix(e)))}</script>
     
     <input class="md-toggle" data-md-toggle="drawer" type="checkbox" id="__drawer" autocomplete="off">
     <input class="md-toggle" data-md-toggle="search" type="checkbox" id="__search" autocomplete="off">
     <label class="md-overlay" for="__drawer"></label>
     <div data-md-component="skip">
       
         
-        <a href="#welcome-to-alpha-environment-documention" class="md-skip">
+        <a href="#automatic-structure" class="md-skip">
           Skip to content
         </a>
       
     </div>
     <div data-md-component="announce">
       
     </div>
     
       <header class="md-header" data-md-component="header">
   <nav class="md-header__inner md-grid" aria-label="Header">
-    <a href="." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="../.." title="Alpha Documentation" class="md-header__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     <label class="md-header__button md-icon" for="__drawer">
       <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M3 6h18v2H3V6m0 5h18v2H3v-2m0 5h18v2H3v-2z"/></svg>
@@ -85,15 +85,15 @@
           <span class="md-ellipsis">
             Alpha Documentation
           </span>
         </div>
         <div class="md-header__topic" data-md-component="header-topic">
           <span class="md-ellipsis">
             
-              Home
+              Model
             
           </span>
         </div>
       </div>
     </div>
     
     
@@ -146,15 +146,15 @@
                 <div class="md-sidebar__scrollwrap">
                   <div class="md-sidebar__inner">
                     
 
 
 <nav class="md-nav md-nav--primary" aria-label="Navigation" data-md-level="0">
   <label class="md-nav__title" for="__drawer">
-    <a href="." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
+    <a href="../.." title="Alpha Documentation" class="md-nav__button md-logo" aria-label="Alpha Documentation" data-md-component="logo">
       
   
   <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M12 8a3 3 0 0 0 3-3 3 3 0 0 0-3-3 3 3 0 0 0-3 3 3 3 0 0 0 3 3m0 3.54C9.64 9.35 6.5 8 3 8v11c3.5 0 6.64 1.35 9 3.54 2.36-2.19 5.5-3.54 9-3.54V8c-3.5 0-6.64 1.35-9 3.54z"/></svg>
 
     </a>
     Alpha Documentation
   </label>
@@ -163,224 +163,394 @@
     
       
       
       
 
   
   
-    
   
+    <li class="md-nav__item">
+      <a href="../.." class="md-nav__link">
+        Home
+      </a>
+    </li>
   
-    <li class="md-nav__item md-nav__item--active">
+
+    
       
-      <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
       
-        
       
+
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../alpha_setup/" class="md-nav__link">
+        Setup
+      </a>
+    </li>
+  
+
+    
       
-        <label class="md-nav__link md-nav__link--active" for="__toc">
-          Home
-          <span class="md-nav__icon md-icon"></span>
-        </label>
       
-      <a href="." class="md-nav__link md-nav__link--active">
-        Home
-      </a>
       
-        
-<nav class="md-nav md-nav--secondary" aria-label="Table of contents">
+
   
   
-    
   
+    <li class="md-nav__item">
+      <a href="../../alpha_core/" class="md-nav__link">
+        Core
+      </a>
+    </li>
   
-    <label class="md-nav__title" for="__toc">
-      <span class="md-nav__icon md-icon"></span>
-      Table of contents
-    </label>
-    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
+
+    
       
-        <li class="md-nav__item">
-  <a href="#purpose" class="md-nav__link">
-    Purpose
-  </a>
-  
-</li>
       
-        <li class="md-nav__item">
-  <a href="#backend-alphaz" class="md-nav__link">
-    Backend: Alphaz
-  </a>
-  
-</li>
       
-        <li class="md-nav__item">
-  <a href="#features" class="md-nav__link">
-    Features
-  </a>
+
   
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#tech" class="md-nav__link">
-    Tech
-  </a>
   
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#project-layout" class="md-nav__link">
-    Project layout
-  </a>
   
-</li>
+    
+    <li class="md-nav__item md-nav__item--nested">
       
-        <li class="md-nav__item">
-  <a href="#frontend-alphaa" class="md-nav__link">
-    Frontend: Alphaa
-  </a>
-  
-</li>
       
-        <li class="md-nav__item">
-  <a href="#features_1" class="md-nav__link">
-    Features
-  </a>
-  
-</li>
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_4" type="checkbox" id="__nav_4" >
       
-        <li class="md-nav__item">
-  <a href="#project-layout_1" class="md-nav__link">
-    Project layout
-  </a>
+      <label class="md-nav__link" for="__nav_4">
+        Api
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Api" data-md-level="1">
+        <label class="md-nav__title" for="__nav_4">
+          <span class="md-nav__icon md-icon"></span>
+          Api
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
   
-</li>
-      
-    </ul>
   
-</nav>
-      
+  
+    <li class="md-nav__item">
+      <a href="../../api/main/" class="md-nav__link">
+        Main
+      </a>
     </li>
   
 
-    
-      
-      
-      
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/configuration/" class="md-nav__link">
+        Configuration
+      </a>
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="alpha_setup/" class="md-nav__link">
-        Setup
+      <a href="../../api/routes/" class="md-nav__link">
+        Routes
       </a>
     </li>
   
 
-    
-      
-      
-      
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/parameters/" class="md-nav__link">
+        Parameters
+      </a>
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="alpha_core/" class="md-nav__link">
-        Core
+      <a href="../../api_database/" class="md-nav__link">
+        Model Parameters
       </a>
     </li>
   
 
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/methods/" class="md-nav__link">
+        Methods
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/cache/" class="md-nav__link">
+        Cache
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/authorizations/" class="md-nav__link">
+        Authorizations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/sqlalchemy/" class="md-nav__link">
+        SqlAlchemy
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api/issues/" class="md-nav__link">
+        Issues
+      </a>
+    </li>
+  
+
+          
+        </ul>
+      </nav>
+    </li>
+  
+
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="alpha_api/" class="md-nav__link">
-        Api
+      <a href="../../alpha_screens/" class="md-nav__link">
+        Screens
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="alpha_screens/" class="md-nav__link">
-        Screens
+      <a href="../../configuration/" class="md-nav__link">
+        Configuration
       </a>
     </li>
   
 
     
       
       
       
 
   
   
+    
+  
+  
+    
+    <li class="md-nav__item md-nav__item--active md-nav__item--nested">
+      
+      
+        <input class="md-nav__toggle md-toggle" data-md-toggle="__nav_7" type="checkbox" id="__nav_7" checked>
+      
+      <label class="md-nav__link" for="__nav_7">
+        Database
+        <span class="md-nav__icon md-icon"></span>
+      </label>
+      <nav class="md-nav" aria-label="Database" data-md-level="1">
+        <label class="md-nav__title" for="__nav_7">
+          <span class="md-nav__icon md-icon"></span>
+          Database
+        </label>
+        <ul class="md-nav__list" data-md-scrollfix>
+          
+            
+  
+  
   
     <li class="md-nav__item">
-      <a href="configuration/" class="md-nav__link">
-        Configuration
+      <a href="../main/" class="md-nav__link">
+        Main
       </a>
     </li>
   
 
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../init/" class="md-nav__link">
+        Init
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
     
+  
+  
+    <li class="md-nav__item md-nav__item--active">
+      
+      <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
+      
+        
       
       
+      <a href="./" class="md-nav__link md-nav__link--active">
+        Model
+      </a>
       
+    </li>
+  
 
+          
+            
   
   
   
     <li class="md-nav__item">
-      <a href="alpha_database/" class="md-nav__link">
-        Database
+      <a href="../schema/" class="md-nav__link">
+        Schema
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../instantiate/" class="md-nav__link">
+        Instantiate
       </a>
     </li>
   
 
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../update/" class="md-nav__link">
+        Update
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../relations/" class="md-nav__link">
+        Relations
+      </a>
+    </li>
+  
+
+          
+            
+  
+  
+  
+    <li class="md-nav__item">
+      <a href="../../api_database/" class="md-nav__link">
+        Model Parameters
+      </a>
+    </li>
+  
+
+          
+        </ul>
+      </nav>
+    </li>
+  
+
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="documentation/" class="md-nav__link">
+      <a href="../../documentation/" class="md-nav__link">
         Documentation
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="alpha_admin/" class="md-nav__link">
+      <a href="../../alpha_admin/" class="md-nav__link">
         Administration
       </a>
     </li>
   
 
     
   </ul>
@@ -397,206 +567,82 @@
                     
 <nav class="md-nav md-nav--secondary" aria-label="Table of contents">
   
   
     
   
   
-    <label class="md-nav__title" for="__toc">
-      <span class="md-nav__icon md-icon"></span>
-      Table of contents
-    </label>
-    <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
-      
-        <li class="md-nav__item">
-  <a href="#purpose" class="md-nav__link">
-    Purpose
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#backend-alphaz" class="md-nav__link">
-    Backend: Alphaz
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#features" class="md-nav__link">
-    Features
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#tech" class="md-nav__link">
-    Tech
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#project-layout" class="md-nav__link">
-    Project layout
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#frontend-alphaa" class="md-nav__link">
-    Frontend: Alphaa
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#features_1" class="md-nav__link">
-    Features
-  </a>
-  
-</li>
-      
-        <li class="md-nav__item">
-  <a href="#project-layout_1" class="md-nav__link">
-    Project layout
-  </a>
-  
-</li>
-      
-    </ul>
-  
 </nav>
                   </div>
                 </div>
               </div>
             
           
           <div class="md-content" data-md-component="content">
             <article class="md-content__inner md-typeset">
               
                 
                 
-                <h1 id="welcome-to-alpha-environment-documention">Welcome to Alpha environment documention</h1>
-<p>Alpha is an <strong>ecosystem</strong> based on a multiple <strong>frameworks</strong> and <strong>libraries</strong> for both <strong>frontend</strong> and <strong>backend</strong>.</p>
-<h2 id="purpose">Purpose</h2>
-<p>The purpose of the <strong>ecosystem</strong> is to simplify any dev activity. </p>
-<details class="note"><summary>Standard query approach</summary><div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
-<span class="n">DB</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span> 
-
-<span class="k">def</span> <span class="nf">get_logs</span><span class="p">(</span><span class="n">start_date</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">end_date</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">useLimit</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">pageForLimit</span><span class="o">=</span><span class="mi">1</span><span class="p">):</span>
-    <span class="n">total</span> <span class="o">=</span> <span class="mi">0</span>
-    <span class="n">logs</span> <span class="o">=</span> <span class="p">[]</span>
-    <span class="n">limit</span> <span class="o">=</span> <span class="mi">20</span>
-    <span class="n">start</span> <span class="o">=</span> <span class="p">(</span><span class="n">pageForLimit</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span> <span class="o">*</span> <span class="n">limit</span>
-
-    <span class="n">query</span> <span class="o">=</span> <span class="s2">&quot;SELECT COUNT(*) AS count FROM logs&quot;</span>
-    <span class="n">parameters</span> <span class="o">=</span> <span class="p">[]</span>
-    <span class="k">if</span> <span class="n">start_date</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="n">end_date</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot; AND CAST(date AS DATE) between </span><span class="si">%s</span><span class="s2"> and </span><span class="si">%s</span><span class="s2">&quot;</span>
-        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">start_date</span><span class="p">)</span>
-        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">end_date</span><span class="p">)</span>       
-    <span class="n">query</span><span class="o">+=</span> <span class="s2">&quot; ORDER BY date DESC&quot;</span>
-
-    <span class="n">rows</span> <span class="o">=</span> <span class="n">DB</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">query</span><span class="p">,</span> <span class="n">parameters</span><span class="p">)</span>
-    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
-        <span class="n">total</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-
-    <span class="n">query</span> <span class="o">=</span> <span class="s2">&quot;SELECT type, origin, message, stack, date FROM logs&quot;</span>
-    <span class="n">parameters</span> <span class="o">=</span> <span class="p">[]</span>
-    <span class="k">if</span> <span class="n">start_date</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span> <span class="ow">and</span> <span class="n">end_date</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
-        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot; AND CAST(date AS DATE) between </span><span class="si">%s</span><span class="s2"> and </span><span class="si">%s</span><span class="s2">&quot;</span>
-        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">start_date</span><span class="p">)</span>
-        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">end_date</span><span class="p">)</span>       
-    <span class="n">query</span><span class="o">+=</span> <span class="s2">&quot; ORDER BY date DESC&quot;</span>
-    <span class="k">if</span> <span class="n">useLimit</span><span class="p">:</span>
-        <span class="n">query</span><span class="o">+=</span> <span class="s2">&quot; LIMIT </span><span class="si">%s</span><span class="s2"> OFFSET </span><span class="si">%s</span><span class="s2">&quot;</span>
-        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">limit</span><span class="p">)</span>
-        <span class="n">parameters</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">start</span><span class="p">)</span>
-
-    <span class="n">rows</span> <span class="o">=</span> <span class="n">db</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">query</span><span class="p">,</span> <span class="n">parameters</span><span class="p">)</span>        
-    <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">rows</span><span class="p">:</span>
-        <span class="n">log</span> <span class="o">=</span> <span class="p">{}</span>
-        <span class="n">log</span><span class="p">[</span><span class="s2">&quot;type&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-        <span class="n">log</span><span class="p">[</span><span class="s2">&quot;origin&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span>
-        <span class="n">log</span><span class="p">[</span><span class="s2">&quot;message&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span>
-        <span class="n">log</span><span class="p">[</span><span class="s2">&quot;stack&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">3</span><span class="p">]</span>
-        <span class="n">log</span><span class="p">[</span><span class="s2">&quot;date&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">4</span><span class="p">]</span>
-        <span class="n">logs</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">log</span><span class="p">)</span>
+                <h1 id="automatic-structure">Automatic structure</h1>
+<p>Compared to native SqlAlchemy in alpha you only need to instantiate the table model:</p>
+<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.models.database.models</span> <span class="kn">import</span> <span class="n">AlphaTable</span><span class="p">,</span> <span class="n">AlphaColumn</span><span class="p">,</span> <span class="n">Text</span><span class="p">,</span> <span class="n">integer</span>
+<span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">DB</span>
+
+<span class="k">class</span> <span class="nc">DuckType</span><span class="p">(</span><span class="n">DB</span><span class="o">.</span><span class="n">Model</span><span class="p">,</span> <span class="n">AlphaTable</span><span class="p">):</span>
+    <span class="n">__bind_key__</span> <span class="o">=</span> <span class="n">DB</span>
+    <span class="n">__tablename__</span><span class="o">=</span> <span class="s2">&quot;duck_type&quot;</span>
+
+    <span class="n">type_id</span> <span class="o">=</span> <span class="n">AlphaColumn</span><span class="p">(</span><span class="n">Integer</span><span class="p">,</span> <span class="n">primary_key</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">autoincrement</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+    <span class="n">name</span> <span class="o">=</span> <span class="n">AlphaColumn</span><span class="p">(</span><span class="n">Text</span><span class="p">,</span><span class="n">nullable</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">default</span> <span class="o">=</span> <span class="s2">&quot;SuperDuck&quot;</span><span class="p">)</span>
+
+<span class="k">class</span> <span class="nc">DuckMedal</span><span class="p">(</span><span class="n">DB</span><span class="o">.</span><span class="n">Model</span><span class="p">,</span> <span class="n">AlphaTable</span><span class="p">):</span>
+    <span class="n">__bind_key__</span> <span class="o">=</span> <span class="n">DB</span>
+    <span class="n">__tablename__</span><span class="o">=</span> <span class="s2">&quot;duck_medal&quot;</span>
+
+    <span class="n">name</span> <span class="o">=</span> <span class="n">AlphaColumn</span><span class="p">(</span><span class="n">Text</span><span class="p">,</span><span class="n">nullable</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">default</span> <span class="o">=</span> <span class="s2">&quot;Lucky&quot;</span><span class="p">)</span>
+    <span class="n">duck_id</span>       <span class="o">=</span> <span class="n">AlphaColumn</span><span class="p">(</span><span class="n">Integer</span><span class="p">,</span> <span class="n">ForeignKey</span> <span class="p">(</span><span class="s1">&#39;duck.duck_id&#39;</span>      <span class="p">),</span> <span class="n">nullable</span>     <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">default</span><span class="o">=</span> <span class="o">-</span><span class="mi">1</span><span class="p">)</span>
+
+<span class="k">class</span> <span class="nc">Duck</span><span class="p">(</span><span class="n">DB</span><span class="o">.</span><span class="n">Model</span><span class="p">,</span> <span class="n">AlphaTable</span><span class="p">):</span>
+    <span class="n">__bind_key__</span> <span class="o">=</span> <span class="n">DB</span>
+    <span class="n">__tablename__</span><span class="o">=</span> <span class="s2">&quot;duck&quot;</span>
+
+    <span class="n">duck_id</span> <span class="o">=</span> <span class="n">AlphaColumn</span><span class="p">(</span><span class="n">Integer</span><span class="p">,</span> <span class="n">primary_key</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">autoincrement</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">visible</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+    <span class="n">name</span> <span class="o">=</span> <span class="n">AlphaColumn</span><span class="p">(</span><span class="n">Text</span><span class="p">,</span><span class="n">nullable</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">default</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">)</span>
+
+    <span class="c1"># Many to one</span>
+    <span class="n">duck_type_id</span> <span class="o">=</span> <span class="n">AlphaColumn</span><span class="p">(</span><span class="n">Integer</span><span class="p">,</span> <span class="n">ForeignKey</span> <span class="p">(</span><span class="s1">&#39;duck_type.type_id&#39;</span><span class="p">),</span> <span class="n">nullable</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span> <span class="n">default</span> <span class="o">=</span> <span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="n">visible</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+    <span class="n">duck_type</span> <span class="o">=</span> <span class="n">relationship</span><span class="p">(</span><span class="s2">&quot;DuckType&quot;</span><span class="p">)</span>
 
-    <span class="k">return</span> <span class="p">{</span><span class="s1">&#39;total&#39;</span> <span class="p">:</span> <span class="n">total</span><span class="p">,</span> <span class="s1">&#39;logs&#39;</span> <span class="p">:</span> <span class="n">logs</span><span class="p">}</span>
+    <span class="c1"># One to many</span>
+    <span class="n">medals</span> <span class="o">=</span> <span class="n">relationship</span><span class="p">(</span><span class="s2">&quot;DuckMedals&quot;</span><span class="p">)</span>
 </code></pre></div>
-</details>
-<details class="note"><summary>Alpha query approach</summary><div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
-<span class="n">DB</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">DB</span>
-<span class="k">def</span> <span class="nf">get_logs</span><span class="p">(</span>
-    <span class="n">start_date</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-    <span class="n">end_date</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
-    <span class="n">limit</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
-    <span class="n">page</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">,</span>
-    <span class="n">per_page</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">100</span><span class="p">,</span>
-<span class="p">):</span>
-    <span class="k">return</span> <span class="n">DB</span><span class="o">.</span><span class="n">select</span><span class="p">(</span>
-        <span class="n">Logs</span><span class="p">,</span>
-        <span class="n">optional_filters</span><span class="o">=</span><span class="p">[</span>
-            <span class="p">{</span><span class="n">Logs</span><span class="o">.</span><span class="n">update_date</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;&gt;&quot;</span><span class="p">:</span> <span class="n">start_date</span><span class="p">}},</span>
-            <span class="p">{</span><span class="n">Logs</span><span class="o">.</span><span class="n">update_date</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;&lt;&quot;</span><span class="p">:</span> <span class="n">end_date</span><span class="p">}},</span>
-        <span class="p">],</span>
-        <span class="n">page</span><span class="o">=</span><span class="n">page</span><span class="p">,</span>
-        <span class="n">per_page</span><span class="o">=</span><span class="n">per_page</span><span class="p">,</span>
-        <span class="n">limit</span><span class="o">=</span><span class="n">limit</span><span class="p">,</span>
-        <span class="n">order_by</span><span class="o">=</span><span class="n">Logs</span><span class="o">.</span><span class="n">update_date</span><span class="o">.</span><span class="n">desc</span><span class="p">(),</span>
-    <span class="p">)</span>
+<p>By default a select query on <strong>Duck</strong> class defined like this:</p>
+<div class="highlight"><pre><span></span><code><span class="n">master_duck</span> <span class="o">=</span> <span class="n">DuckType</span><span class="p">(</span><span class="n">ame</span><span class="o">=</span><span class="s2">&quot;Master Duck&quot;</span><span class="p">)</span>
+<span class="n">DB</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">master_duck</span><span class="p">)</span>
+
+<span class="n">ducky</span> <span class="o">=</span> <span class="n">Duck</span><span class="p">(</span><span class="n">name</span><span class="o">=</span><span class="s2">&quot;Ducky&quot;</span><span class="p">,</span><span class="n">duck_type</span><span class="o">=</span><span class="n">master_duck</span><span class="p">)</span>
+<span class="n">DB</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">ducky</span><span class="p">)</span>
+
+<span class="n">honnor_medal</span> <span class="o">=</span> <span class="n">DuckMedal</span><span class="p">(</span><span class="n">name</span><span class="o">=</span><span class="s2">&quot;Honnor&quot;</span><span class="p">,</span><span class="n">duck_id</span><span class="o">=</span><span class="n">ducky</span><span class="o">.</span><span class="n">duck_id</span><span class="p">)</span>
+<span class="n">lucky_medal</span> <span class="o">=</span> <span class="n">DuckMedal</span><span class="p">(</span><span class="n">name</span><span class="o">=</span><span class="s2">&quot;Lucky&quot;</span><span class="p">,</span><span class="n">duck_id</span><span class="o">=</span><span class="n">ducky</span><span class="o">.</span><span class="n">duck_id</span><span class="p">)</span>
+<span class="n">DB</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">ducky</span><span class="p">)</span>
+
+<span class="n">ducks</span> <span class="o">=</span> <span class="n">DB</span><span class="o">.</span><span class="n">select</span><span class="p">(</span><span class="n">Duck</span><span class="p">,</span> <span class="n">filters</span><span class="o">=</span><span class="p">[</span><span class="n">Duck</span><span class="o">.</span><span class="n">name</span><span class="o">==</span><span class="s2">&quot;Ducky&quot;</span><span class="p">],</span> <span class="n">first</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+</code></pre></div>
+<p>Will result in this:</p>
+<div class="highlight"><pre><span></span><code><span class="p">{</span>
+  <span class="nt">&quot;duck_id&quot;</span><span class="p">:</span> <span class="mi">1</span><span class="p">,</span>
+  <span class="nt">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;Ducky&quot;</span><span class="p">,</span>
+  <span class="nt">&quot;duck_type&quot;</span><span class="p">:</span> <span class="p">{</span>
+    <span class="nt">&quot;type_id&quot;</span><span class="p">:</span> <span class="mi">1</span><span class="p">,</span>
+    <span class="nt">&quot;duck_type&quot;</span><span class="p">:</span> <span class="s2">&quot;Master Duck&quot;</span>
+  <span class="p">},</span>
+  <span class="nt">&quot;medals&quot;</span><span class="p">:</span> <span class="p">[{</span> <span class="nt">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;Honnor&quot;</span> <span class="p">},</span> <span class="p">{</span> <span class="nt">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;Lucky&quot;</span> <span class="p">}]</span>
+<span class="p">}</span>
 </code></pre></div>
-</details>
-<h2 id="backend-alphaz">Backend: Alphaz</h2>
-<ul>
-<li>
-<p>Alphaz is a backend toolbox/framework based on a combination between Flask, SqlAlchemy and a multitude of other libraries.</p>
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>The overriding goal for Alphaz is to ease the backend development and easely link python backend to Angular frontend [Alphaa].</p>
-</div>
-</li>
-</ul>
-<h2 id="features">Features</h2>
-<ul>
-<li>API Routing parameters management upgrade</li>
-<li>Enhanced json files configuration</li>
-</ul>
-<h2 id="tech">Tech</h2>
-<p>Alphaz uses a number of open source projects to work properly:</p>
-<ul>
-<li><a href="https://flask.palletsprojects.com/en/1.1.x/">Flask</a> - a micro web framework</li>
-<li><a href="https://www.sqlalchemy.org/">SqlAlchemy</a> - a database toolkit</li>
-<li><a href="https://flask-sqlalchemy.palletsprojects.com/en/2.x/">Flask-SqlAlchemy</a> - an extension for Flask that adds support for SQLAlchemy</li>
-</ul>
-<h2 id="project-layout">Project layout</h2>
-<ul>
-<li>How to setup <code>Alpha</code>: <a href="alpha_setup/">Alpha</a></li>
-</ul>
-<h2 id="frontend-alphaa">Frontend: Alphaa</h2>
-<ul>
-<li>
-<p>Alphaa is a frontend toolbox/framework</p>
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>The overriding goal for Alphaa is to ease the frontend development and easely link Angular frontend to python backend [Alphaz].</p>
-</div>
-<h2 id="features_1">Features</h2>
-</li>
-<li>
-<p>Enhanced services</p>
-</li>
-<li>Master class</li>
-</ul>
-<h2 id="project-layout_1">Project layout</h2>
-<ul>
-<li>How to setup <code>Alpha</code>: <a href="alpha_setup/">Alpha</a></li>
-</ul>
                 
               
               
                 
 
 
               
@@ -607,22 +653,36 @@
       </main>
       
         
 <footer class="md-footer">
   
     <nav class="md-footer__inner md-grid" aria-label="Footer">
       
+        <a href="../init/" class="md-footer__link md-footer__link--prev" rel="prev">
+          <div class="md-footer__button md-icon">
+            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12z"/></svg>
+          </div>
+          <div class="md-footer__title">
+            <div class="md-ellipsis">
+              <span class="md-footer__direction">
+                Previous
+              </span>
+              Init
+            </div>
+          </div>
+        </a>
+      
       
-        <a href="alpha_setup/" class="md-footer__link md-footer__link--next" rel="next">
+        <a href="../schema/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Next
               </span>
-              Setup
+              Schema
             </div>
           </div>
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4z"/></svg>
           </div>
         </a>
       
@@ -643,15 +703,15 @@
   </div>
 </footer>
       
     </div>
     <div class="md-dialog" data-md-component="dialog">
       <div class="md-dialog__inner md-typeset"></div>
     </div>
-    <script id="__config" type="application/json">{"base": ".", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
+    <script id="__config" type="application/json">{"base": "../..", "features": [], "translations": {"clipboard.copy": "Copy to clipboard", "clipboard.copied": "Copied to clipboard", "search.config.lang": "en", "search.config.pipeline": "trimmer, stopWordFilter", "search.config.separator": "[\\s\\-]+", "search.placeholder": "Search", "search.result.placeholder": "Type to start searching", "search.result.none": "No matching documents", "search.result.one": "1 matching document", "search.result.other": "# matching documents", "search.result.more.one": "1 more on this page", "search.result.more.other": "# more on this page", "search.result.term.missing": "Missing"}, "search": "../../assets/javascripts/workers/search.fe42c31b.min.js", "version": null}</script>
     
     
-      <script src="assets/javascripts/bundle.7353b375.min.js"></script>
+      <script src="../../assets/javascripts/bundle.7353b375.min.js"></script>
       
     
   </body>
 </html>
```

#### html2text {}

```diff
@@ -5,141 +5,106 @@
 
 
 
  ⁰ ⁰
 Skip_to_content
 
  Alpha Documentation
- Home
+ Model
 
 [query               ]
 Initializing search
 
    Alpha Documentation
-    * ⁰  Home   Home    Table of contents
-          o Purpose
-          o Backend:_Alphaz
-          o Features
-          o Tech
-          o Project_layout
-          o Frontend:_Alphaa
-          o Features
-          o Project_layout
+    * Home
     * Setup
     * Core
-    * Api
+    * ⁰  Api      Api
+          o Main
+          o Configuration
+          o Routes
+          o Parameters
+          o Model_Parameters
+          o Methods
+          o Cache
+          o Authorizations
+          o SqlAlchemy
+          o Issues
     * Screens
     * Configuration
-    * Database
+    * *  Database      Database
+          o Main
+          o Init
+          o ⁰ Model
+          o Schema
+          o Instantiate
+          o Update
+          o Relations
+          o Model_Parameters
     * Documentation
     * Administration
-   Table of contents
-    * Purpose
-    * Backend:_Alphaz
-    * Features
-    * Tech
-    * Project_layout
-    * Frontend:_Alphaa
-    * Features
-    * Project_layout
-****** Welcome to Alpha environment documention ******
-Alpha is an ecosystem based on a multiple frameworks and libraries for both
-frontend and backend.
-***** Purpose *****
-The purpose of the ecosystem is to simplify any dev activity.
-Standard query approach
-from core import core
-DB = core.db
-
-def get_logs(start_date=None, end_date=None, useLimit=False, pageForLimit=1):
-    total = 0
-    logs = []
-    limit = 20
-    start = (pageForLimit - 1) * limit
-
-    query = "SELECT COUNT(*) AS count FROM logs"
-    parameters = []
-    if start_date is not None and end_date is not None:
-        query += " AND CAST(date AS DATE) between %s and %s"
-        parameters.append(start_date)
-        parameters.append(end_date)
-    query+= " ORDER BY date DESC"
-
-    rows = DB.get(query, parameters)
-    for row in rows:
-        total = row[0]
-
-    query = "SELECT type, origin, message, stack, date FROM logs"
-    parameters = []
-    if start_date is not None and end_date is not None:
-        query += " AND CAST(date AS DATE) between %s and %s"
-        parameters.append(start_date)
-        parameters.append(end_date)
-    query+= " ORDER BY date DESC"
-    if useLimit:
-        query+= " LIMIT %s OFFSET %s"
-        parameters.append(limit)
-        parameters.append(start)
-
-    rows = db.get(query, parameters)
-    for row in rows:
-        log = {}
-        log["type"] = row[0]
-        log["origin"] = row[1]
-        log["message"] = row[2]
-        log["stack"] = row[3]
-        log["date"] = row[4]
-        logs.append(log)
-
-    return {'total' : total, 'logs' : logs}
- Alpha query approach
-from core import core
-DB = core.DB
-def get_logs(
-    start_date: datetime = None,
-    end_date: datetime = None,
-    limit: int = False,
-    page: int = 0,
-    per_page: int = 100,
-):
-    return DB.select(
-        Logs,
-        optional_filters=[
-            {Logs.update_date: {">": start_date}},
-            {Logs.update_date: {"<": end_date}},
-        ],
-        page=page,
-        per_page=per_page,
-        limit=limit,
-        order_by=Logs.update_date.desc(),
-    )
-***** Backend: Alphaz *****
-    * Alphaz is a backend toolbox/framework based on a combination between
-      Flask, SqlAlchemy and a multitude of other libraries.
-      Note
-      The overriding goal for Alphaz is to ease the backend development and
-      easely link python backend to Angular frontend [Alphaa].
-***** Features *****
-    * API Routing parameters management upgrade
-    * Enhanced json files configuration
-***** Tech *****
-Alphaz uses a number of open source projects to work properly:
-    * Flask - a micro web framework
-    * SqlAlchemy - a database toolkit
-    * Flask-SqlAlchemy - an extension for Flask that adds support for
-      SQLAlchemy
-***** Project layout *****
-    * How to setup Alpha: Alpha
-***** Frontend: Alphaa *****
-    * Alphaa is a frontend toolbox/framework
-      Note
-      The overriding goal for Alphaa is to ease the frontend development and
-      easely link Angular frontend to python backend [Alphaz].
-      ***** Features *****
-    * Enhanced services
-    * Master class
-***** Project layout *****
-    * How to setup Alpha: Alpha
 
- Next__Setup
+****** Automatic structure ******
+Compared to native SqlAlchemy in alpha you only need to instantiate the table
+model:
+from alphaz.models.database.models import AlphaTable, AlphaColumn, Text,
+integer
+from core import DB
+
+class DuckType(DB.Model, AlphaTable):
+    __bind_key__ = DB
+    __tablename__= "duck_type"
+
+    type_id = AlphaColumn(Integer, primary_key=True, autoincrement=True)
+    name = AlphaColumn(Text,nullable = False, default = "SuperDuck")
+
+class DuckMedal(DB.Model, AlphaTable):
+    __bind_key__ = DB
+    __tablename__= "duck_medal"
+
+    name = AlphaColumn(Text,nullable = False, default = "Lucky")
+    duck_id       = AlphaColumn(Integer, ForeignKey ('duck.duck_id'      ),
+nullable     = False, default= -1)
+
+class Duck(DB.Model, AlphaTable):
+    __bind_key__ = DB
+    __tablename__= "duck"
+
+    duck_id = AlphaColumn(Integer, primary_key=True, autoincrement=True,
+visible=False)
+    name = AlphaColumn(Text,nullable = False, default = "")
+
+    # Many to one
+    duck_type_id = AlphaColumn(Integer, ForeignKey ('duck_type.type_id'),
+nullable = False, default = -1, visible=False)
+    duck_type = relationship("DuckType")
+
+    # One to many
+    medals = relationship("DuckMedals")
+By default a select query on Duck class defined like this:
+master_duck = DuckType(ame="Master Duck")
+DB.add(master_duck)
+
+ducky = Duck(name="Ducky",duck_type=master_duck)
+DB.add(ducky)
+
+honnor_medal = DuckMedal(name="Honnor",duck_id=ducky.duck_id)
+lucky_medal = DuckMedal(name="Lucky",duck_id=ducky.duck_id)
+DB.add(ducky)
+
+ducks = DB.select(Duck, filters=[Duck.name=="Ducky"], first=True)
+Will result in this:
+{
+  "duck_id": 1,
+  "name": "Ducky",
+  "duck_type": {
+    "type_id": 1,
+    "duck_type": "Master Duck"
+  },
+  "medals": [{ "name": "Honnor" }, { "name": "Lucky" }]
+}
+
+ Previous__Init
+
+ Next__Schema
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.9/alphaz/documentations/site/search/search_index.json` & `alphaz-0.7.4/alphaz/documentations/site/search/search_index.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8882013201320131%*

 * *Differences: {"'docs'": '{11: {\'location\': \'alpha_core/\', \'text\': "Alpha core system Purpose The core is '*

 * *           'used as a central point to manage various system: logging system database access api '*

 * *           'system dynamic configuration How to use You could: Use the alphaz core and initiate it '*

 * *           'at the start of you project preferably in a file named core.py to be complient with '*

 * *           'this documentation: from alphaz.models.main import AlphaCore core = AlphaCore ( '*

 * *           '__file__ […]*

```diff
@@ -60,184 +60,14 @@
         },
         {
             "location": "alpha_admin/",
             "text": "",
             "title": "Administration"
         },
         {
-            "location": "alpha_api/",
-            "text": "Alpha API system Introduction The api system is completely based on Flask and compatible. You could use Flask inside Alpha system without any issue. Launch To start the api execute the api.py file python api.py Note set ALPHA_CONF environment parameter is you want to set the environment. Verify the deployment by navigating to your server address in your preferred browser: 127 .0.0.1:<port> How to use Your could import it using simply from the utils : from alphaz.utils.api import api or from the core if you are using it from core import core , API api / API is the equivalent for app in Flask framework. Routes We recommend to add all the route definition in apis/routes folder and import all the route definition in apis/routes/ init .py . Then you will have to import the route in thoe core.py file: from alphaz.models.main import AlphaCore , singleton @singleton class Core ( AlphaCore ): def __init__ ( self , file : str ): super () . __init__ ( file ) core = Core ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded from apis.routes import * Configuration The api is automatically configured from the api.jon file. See Configuration for further details on how to use it. Main workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.databases\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false } Mails In order to specify the mails configurations \"mails\" : { \"mail_server\" : { \"host\" : \"\" , \"mail\" : \"\" , \"password\" : \"\" , \"port\" : 465 , \"server\" : \"\" , \"ssl\" : true , \"tls\" : false } } Auth In order to specify the auth mode \"auth\" : { \"mode\" : \"ldap\" , \"ldap\" : { \"server\" : \"ldap://path_to_ldap\" , \"baseDN\" : \"ou=people,dc=a_name,dc=com\" , \"users_filters\" : \"(|(uid={uid})(mail={mail})(cn={cn}))\" , \"user_filters\" : \"(|(uid={username})(mail={username})(cn={username}))\" , \"user_data\" : { \"givenName\" : \"name\" , \"sn\" : \"lastname\" , \"c\" : \"area\" , \"st-locationdescription\" : \"location\" , \"st-seatnumber\" : \"seat\" , \"telephoneNumber\" : \"phone-number\" } }, \"users\" : { \"a_user_name\" : { \"user_permissions\" : [ \"SUPER_USER\" ] } } }, Reloader type In order to specify the Werkzeug reloader type \"reloader_type\" : \"stat\" Admin In order to specify the admins configurations \"admins\" : { \"ips\" :[ \"127.0.0.1\" ], \"password\" : \"a_password\" }, Dashboard In order to configure the Flask-Monitoring Dashboard \"dashboard\" : { \"dashboard\" : { \"APP_VERSION\" : 1.0 , \"SAMPLING_PERIOD\" : 20 , \"ENABLE_LOGGING\" : true , \"active\" : false }, \"authentication\" : { \"USERNAME\" : \"username\" , \"PASSWORD\" : \"\" , \"GUEST_USERNAME\" : \"guest\" , \"GUEST_PASSWORD\" : [ \"guest1\" , \"guest2\" ], \"SECURITY_TOKEN\" : \"a_security_token\" }, \"database\" : { \"DATABASE\" : \"sqlite:///{{root}}/dashboard.db\" } } Routes Basic To specify an api route, juste use the route flag: from alphaz.utils.api import route , api , Parameter @route ( \"route_name\" ) def method_name (): return \"hello\" Method automatically convert the output to the right format. Default format is json Description A description could be specified: @route ( \"route_name\" , description = \"This route say hello\" ) def method_name (): return \"hello\" Category The routes are organized by category , by default the route category is defined by it file name , but it could be specified using the cat parameter: @route ( \"route_name\" , category = \"politeness\" ) def method_name (): return \"hello\" Parameters Simple You could simply define parameters by listing all parameters in parameters list: from alphaz.utils.api import route , api , Parameter @route ( \"books\" , parameters = [ \"name\" ]) def method_name (): return \"Book name is %s or %s \" % ( api [ \"name\" ], api . get ( \"name\" , default = \"\" )) Parameter value is accessed by api instance, using get method, they could also be accessed using get_parameters method from api instance. Object Or you could use the Parameter class to specify properties such as: ptype : value type int, str, bool, SqlAlchemy model parameter is automatically converted to the specified type if conversion failed an exception is raised required : the parameter is required or not default : default parameter value options : authorized values mode : input mode cacheable : parameter is taken into acount in the caching system or not private : parameter is hiden from documentation or not @route ( \"/logs\" , parameters = [ Parameter ( 'page' , required = True , ptype = int ), Parameter ( 'startDate' , required = True ), Parameter ( 'endDate' , default = None ), Parameter ( 'error' , options = [ \"Y\" , \"N\" ]) ]) def admin_logs (): return get_logs ( ** api . get_parameters ()) Promote this method as it allows a better control on parameters Default parameters Some parameter are always available: - no_log (bool): disable logs for this route - reset_cache (bool): reset cache before calling this route - requester (str): requester to this route - format (str): output format - json: - xml: - admin (str): admin password - admin_user_id (int): id of the user to connect has an admin SqlAlchemy model If you specify a SqlAlchemy model as a type it will be automatically converted to the specified model. from core import core db = core . db class Logs ( db . Model , AlphaTable ): __tablename__ = 'LOGS' id = AlphaColumn ( Integer , nullable = False , primary_key = True ) name = AlphaColumn ( String , nullable = False ) @route ( \"logs\" , parameters = [ Parameter ( 'log' , ptype = Logs ) ]) def admin_logs (): db . add ( api [ 'log' ]) Methods Methods are specified the same way as in Flask , using methods parameter: @route ( 'logs' , methods = [ \"GET\" ]) def get_logs (): return db . select ( Logs ) @route ( 'logs' , methods = [ \"POST\" ]) def set_logs (): return db . add ( Logs ) Methods can be managed using different routes or within a single route : @route ( 'logs' , methods = [ \"GET\" , \"POST\" , \"DELETE\" ]) def get_logs (): if api . is_get (): return db . select ( Logs ) elif api . is_post (): return db . add ( Logs ) elif api . is_delete (): return db . delete ( Logs ) Authorizations Route can be protected using the login system or admin rights. Login system To protect a route using the login system you must specify: logged=True @route ( 'protected' , logged = True ) def protected_route (): user = api . get_logged_user () return user User information can be accessed using get_logged_user method. Cache A cache system is implemented, in order to use it you must specify the Admin Admin could auto log to any user account on local mode Condition To be an admin a user must have at least one condition: a role > 9 specify the magic password has admin API parameter connect using an admin ip. The ips admin list must be defined in the api.json configuration files under the key = admins_ips How to use If you met one of the admin condition you do not need any password in order to log has any of the user in the database. You could be logged for specific routes using the single route mode or to any route using the login/logout system. Single route mode You could specifiy either admin_user_id={user_id} or admin_user_name={username} directly into any request in order to login with this user for this specific route. Exemple /anyroute?admin_user_id=1000 Login to the api Use the route /auth/su in order to set an admin session that is valid until the end of the api runtime. You must specifiy either admin_user_id={user_id} or admin_user_name={username} Exemple /auth/su?admin_user_id=1000 Logout from the api Use the route /logout/su in order to logout. Issues In progress Database alias In progress",
-            "title": "Api"
-        },
-        {
-            "location": "alpha_api/#alpha-api-system",
-            "text": "",
-            "title": "Alpha API system"
-        },
-        {
-            "location": "alpha_api/#introduction",
-            "text": "The api system is completely based on Flask and compatible. You could use Flask inside Alpha system without any issue.",
-            "title": "Introduction"
-        },
-        {
-            "location": "alpha_api/#launch",
-            "text": "To start the api execute the api.py file python api.py Note set ALPHA_CONF environment parameter is you want to set the environment. Verify the deployment by navigating to your server address in your preferred browser: 127 .0.0.1:<port>",
-            "title": "Launch"
-        },
-        {
-            "location": "alpha_api/#how-to-use",
-            "text": "Your could import it using simply from the utils : from alphaz.utils.api import api or from the core if you are using it from core import core , API api / API is the equivalent for app in Flask framework.",
-            "title": "How to use"
-        },
-        {
-            "location": "alpha_api/#routes",
-            "text": "We recommend to add all the route definition in apis/routes folder and import all the route definition in apis/routes/ init .py . Then you will have to import the route in thoe core.py file: from alphaz.models.main import AlphaCore , singleton @singleton class Core ( AlphaCore ): def __init__ ( self , file : str ): super () . __init__ ( file ) core = Core ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded from apis.routes import *",
-            "title": "Routes"
-        },
-        {
-            "location": "alpha_api/#configuration",
-            "text": "The api is automatically configured from the api.jon file. See Configuration for further details on how to use it.",
-            "title": "Configuration"
-        },
-        {
-            "location": "alpha_api/#main",
-            "text": "workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.databases\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false }",
-            "title": "Main"
-        },
-        {
-            "location": "alpha_api/#mails",
-            "text": "In order to specify the mails configurations \"mails\" : { \"mail_server\" : { \"host\" : \"\" , \"mail\" : \"\" , \"password\" : \"\" , \"port\" : 465 , \"server\" : \"\" , \"ssl\" : true , \"tls\" : false } }",
-            "title": "Mails"
-        },
-        {
-            "location": "alpha_api/#auth",
-            "text": "In order to specify the auth mode \"auth\" : { \"mode\" : \"ldap\" , \"ldap\" : { \"server\" : \"ldap://path_to_ldap\" , \"baseDN\" : \"ou=people,dc=a_name,dc=com\" , \"users_filters\" : \"(|(uid={uid})(mail={mail})(cn={cn}))\" , \"user_filters\" : \"(|(uid={username})(mail={username})(cn={username}))\" , \"user_data\" : { \"givenName\" : \"name\" , \"sn\" : \"lastname\" , \"c\" : \"area\" , \"st-locationdescription\" : \"location\" , \"st-seatnumber\" : \"seat\" , \"telephoneNumber\" : \"phone-number\" } }, \"users\" : { \"a_user_name\" : { \"user_permissions\" : [ \"SUPER_USER\" ] } } },",
-            "title": "Auth"
-        },
-        {
-            "location": "alpha_api/#reloader-type",
-            "text": "In order to specify the Werkzeug reloader type \"reloader_type\" : \"stat\"",
-            "title": "Reloader type"
-        },
-        {
-            "location": "alpha_api/#admin",
-            "text": "In order to specify the admins configurations \"admins\" : { \"ips\" :[ \"127.0.0.1\" ], \"password\" : \"a_password\" },",
-            "title": "Admin"
-        },
-        {
-            "location": "alpha_api/#dashboard",
-            "text": "In order to configure the Flask-Monitoring Dashboard \"dashboard\" : { \"dashboard\" : { \"APP_VERSION\" : 1.0 , \"SAMPLING_PERIOD\" : 20 , \"ENABLE_LOGGING\" : true , \"active\" : false }, \"authentication\" : { \"USERNAME\" : \"username\" , \"PASSWORD\" : \"\" , \"GUEST_USERNAME\" : \"guest\" , \"GUEST_PASSWORD\" : [ \"guest1\" , \"guest2\" ], \"SECURITY_TOKEN\" : \"a_security_token\" }, \"database\" : { \"DATABASE\" : \"sqlite:///{{root}}/dashboard.db\" } }",
-            "title": "Dashboard"
-        },
-        {
-            "location": "alpha_api/#routes_1",
-            "text": "",
-            "title": "Routes"
-        },
-        {
-            "location": "alpha_api/#basic",
-            "text": "To specify an api route, juste use the route flag: from alphaz.utils.api import route , api , Parameter @route ( \"route_name\" ) def method_name (): return \"hello\" Method automatically convert the output to the right format. Default format is json",
-            "title": "Basic"
-        },
-        {
-            "location": "alpha_api/#description",
-            "text": "A description could be specified: @route ( \"route_name\" , description = \"This route say hello\" ) def method_name (): return \"hello\"",
-            "title": "Description"
-        },
-        {
-            "location": "alpha_api/#category",
-            "text": "The routes are organized by category , by default the route category is defined by it file name , but it could be specified using the cat parameter: @route ( \"route_name\" , category = \"politeness\" ) def method_name (): return \"hello\"",
-            "title": "Category"
-        },
-        {
-            "location": "alpha_api/#parameters",
-            "text": "",
-            "title": "Parameters"
-        },
-        {
-            "location": "alpha_api/#simple",
-            "text": "You could simply define parameters by listing all parameters in parameters list: from alphaz.utils.api import route , api , Parameter @route ( \"books\" , parameters = [ \"name\" ]) def method_name (): return \"Book name is %s or %s \" % ( api [ \"name\" ], api . get ( \"name\" , default = \"\" )) Parameter value is accessed by api instance, using get method, they could also be accessed using get_parameters method from api instance.",
-            "title": "Simple"
-        },
-        {
-            "location": "alpha_api/#object",
-            "text": "Or you could use the Parameter class to specify properties such as: ptype : value type int, str, bool, SqlAlchemy model parameter is automatically converted to the specified type if conversion failed an exception is raised required : the parameter is required or not default : default parameter value options : authorized values mode : input mode cacheable : parameter is taken into acount in the caching system or not private : parameter is hiden from documentation or not @route ( \"/logs\" , parameters = [ Parameter ( 'page' , required = True , ptype = int ), Parameter ( 'startDate' , required = True ), Parameter ( 'endDate' , default = None ), Parameter ( 'error' , options = [ \"Y\" , \"N\" ]) ]) def admin_logs (): return get_logs ( ** api . get_parameters ()) Promote this method as it allows a better control on parameters",
-            "title": "Object"
-        },
-        {
-            "location": "alpha_api/#default-parameters",
-            "text": "Some parameter are always available: - no_log (bool): disable logs for this route - reset_cache (bool): reset cache before calling this route - requester (str): requester to this route - format (str): output format - json: - xml: - admin (str): admin password - admin_user_id (int): id of the user to connect has an admin",
-            "title": "Default parameters"
-        },
-        {
-            "location": "alpha_api/#sqlalchemy-model",
-            "text": "If you specify a SqlAlchemy model as a type it will be automatically converted to the specified model. from core import core db = core . db class Logs ( db . Model , AlphaTable ): __tablename__ = 'LOGS' id = AlphaColumn ( Integer , nullable = False , primary_key = True ) name = AlphaColumn ( String , nullable = False ) @route ( \"logs\" , parameters = [ Parameter ( 'log' , ptype = Logs ) ]) def admin_logs (): db . add ( api [ 'log' ])",
-            "title": "SqlAlchemy model"
-        },
-        {
-            "location": "alpha_api/#methods",
-            "text": "Methods are specified the same way as in Flask , using methods parameter: @route ( 'logs' , methods = [ \"GET\" ]) def get_logs (): return db . select ( Logs ) @route ( 'logs' , methods = [ \"POST\" ]) def set_logs (): return db . add ( Logs ) Methods can be managed using different routes or within a single route : @route ( 'logs' , methods = [ \"GET\" , \"POST\" , \"DELETE\" ]) def get_logs (): if api . is_get (): return db . select ( Logs ) elif api . is_post (): return db . add ( Logs ) elif api . is_delete (): return db . delete ( Logs )",
-            "title": "Methods"
-        },
-        {
-            "location": "alpha_api/#authorizations",
-            "text": "Route can be protected using the login system or admin rights.",
-            "title": "Authorizations"
-        },
-        {
-            "location": "alpha_api/#login-system",
-            "text": "To protect a route using the login system you must specify: logged=True @route ( 'protected' , logged = True ) def protected_route (): user = api . get_logged_user () return user User information can be accessed using get_logged_user method.",
-            "title": "Login system"
-        },
-        {
-            "location": "alpha_api/#cache",
-            "text": "A cache system is implemented, in order to use it you must specify the",
-            "title": "Cache"
-        },
-        {
-            "location": "alpha_api/#admin_1",
-            "text": "Admin could auto log to any user account on local mode",
-            "title": "Admin"
-        },
-        {
-            "location": "alpha_api/#condition",
-            "text": "To be an admin a user must have at least one condition: a role > 9 specify the magic password has admin API parameter connect using an admin ip. The ips admin list must be defined in the api.json configuration files under the key = admins_ips",
-            "title": "Condition"
-        },
-        {
-            "location": "alpha_api/#how-to-use_1",
-            "text": "If you met one of the admin condition you do not need any password in order to log has any of the user in the database. You could be logged for specific routes using the single route mode or to any route using the login/logout system.",
-            "title": "How to use"
-        },
-        {
-            "location": "alpha_api/#single-route-mode",
-            "text": "You could specifiy either admin_user_id={user_id} or admin_user_name={username} directly into any request in order to login with this user for this specific route. Exemple /anyroute?admin_user_id=1000",
-            "title": "Single route mode"
-        },
-        {
-            "location": "alpha_api/#login-to-the-api",
-            "text": "Use the route /auth/su in order to set an admin session that is valid until the end of the api runtime. You must specifiy either admin_user_id={user_id} or admin_user_name={username} Exemple /auth/su?admin_user_id=1000",
-            "title": "Login to the api"
-        },
-        {
-            "location": "alpha_api/#logout-from-the-api",
-            "text": "Use the route /logout/su in order to logout.",
-            "title": "Logout from the api"
-        },
-        {
-            "location": "alpha_api/#issues",
-            "text": "In progress",
-            "title": "Issues"
-        },
-        {
-            "location": "alpha_api/#database-alias",
-            "text": "In progress",
-            "title": "Database alias"
-        },
-        {
             "location": "alpha_core/",
             "text": "Alpha core system Purpose The core is used as a central point to manage various system: logging system database access api system dynamic configuration How to use You could: Use the alphaz core and initiate it at the start of you project preferably in a file named core.py to be complient with this documentation: from alphaz.models.main import AlphaCore core = AlphaCore ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded Or create a core.py file at the root of your project containing at least: from alphaz.models.main import AlphaCore , singleton @singleton class Core ( AlphaCore ): def __init__ ( self , file : str ): super () . __init__ ( file ) core = Core ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded Note This is the recommended way, so that you could custom the Core class Logging from core import core LOG = core . get_logger ( 'name' ) LOG . info ( 'message' ) Database from core import core DB = core . db API from core import core API = core . api Configuration from core import core CONFIG = core . config tmp_directory_path = CONFIG . get ( 'directories/tmp' )",
             "title": "Core"
         },
         {
             "location": "alpha_core/#alpha-core-system",
             "text": "",
@@ -270,99 +100,14 @@
         },
         {
             "location": "alpha_core/#configuration",
             "text": "from core import core CONFIG = core . config tmp_directory_path = CONFIG . get ( 'directories/tmp' )",
             "title": "Configuration"
         },
         {
-            "location": "alpha_database/",
-            "text": "Alpha database system Automatic structure Compared to native SqlAlchemy in alpha you only need to instantiate the table model: from alphaz.models.database.models import AlphaTable , AlphaColumn , Text , integer from core import DB class DuckType ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck_type\" type_id = AlphaColumn ( Integer , primary_key = True , autoincrement = True ) name = AlphaColumn ( Text , nullable = False , default = \"SuperDuck\" ) class DuckMedal ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck_medal\" name = AlphaColumn ( Text , nullable = False , default = \"Lucky\" ) duck_id = AlphaColumn ( Integer , ForeignKey ( 'duck.duck_id' ), nullable = False , default = - 1 ) class Duck ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck\" duck_id = AlphaColumn ( Integer , primary_key = True , autoincrement = True , visible = False ) name = AlphaColumn ( Text , nullable = False , default = \"\" ) # Many to one duck_type_id = AlphaColumn ( Integer , ForeignKey ( 'duck_type.type_id' ), nullable = False , default = - 1 , visible = False ) duck_type = relationship ( \"DuckType\" ) # One to many medals = relationship ( \"DuckMedals\" ) By default a select query on Duck class defined like this: master_duck = DuckType ( ame = \"Master Duck\" ) DB . add ( master_duck ) ducky = Duck ( name = \"Ducky\" , duck_type = master_duck ) DB . add ( ducky ) honnor_medal = DuckMedal ( name = \"Honnor\" , duck_id = ducky . duck_id ) lucky_medal = DuckMedal ( name = \"Lucky\" , duck_id = ducky . duck_id ) DB . add ( ducky ) ducks = DB . select ( Duck , filters = [ Duck . name == \"Ducky\" ], first = True ) Will result in this: { \"duck_id\" : 1 , \"name\" : \"Ducky\" , \"duck_type\" : { \"type_id\" : 1 , \"duck_type\" : \"Master Duck\" }, \"medals\" : [{ \"name\" : \"Honnor\" }, { \"name\" : \"Lucky\" }] } Schema Note The associated Schema is created automatically, with classic and nested fields. However Marshmallow schema could be defined using the classic way Marshmallow : Set visible to False if you dont want the column to appears in the Schema. Important Schema must be defined after the Model DB = core . db class DuckTypeSchema ( Schema ): type_id = fields . Integer () name = fields . String () class DuckMedalSchema ( Schema ): name = fields . String () class DuckSchema ( Schema ): name = fields . String () # Many to One duck_type = fields . Nested ( DuckTypeSchema ) # One to many medals = fields . List ( fields . Nested ( DuckMedalSchema )) Important Alpha will automatically detect the schema if the name is defined as \"{ModelName}Schema\" and is located in the same file. Note In this mode, Schema could be defined automatically, excepted for nested fields. Specific Schema Schema could be specified for every request: DB . select ( model = Duck , schema = DuckSchema ) Alpha notation init This enable the use of model columns which is not possible using SqlAlchemy: attr = { Duck . name : name , Duck . duck_type_id : duck_type_id , } duck = Duck () duck . init ( attr ) or duck = Duck () duck . init ({ Duck . name : name , Duck . duck_type_id : duck_type_id , }) Instead of: attr = { Duck . name : name , Duck . duck_type_id : duck_type_id , } duck = Duck () duck . init ( ** { x . key : y for x , y in attr . items ()}) Update Classic SQLAlchemy Select query duck = Duck . query . filter_by ( name = name ) . first () duck . duck_type_id = duck_type_id db . session . commit () Init new_duck = Duck ( \"name\" : name , \"duck_type_id\" : duck_type_id ) db . session . merge ( new_duck ) db . session . commit () or attr = { \"name\" : name , \"duck_type_id\" : duck_type_id , } duck = Duck ( ** attr ) db . session . merge ( new_duck ) db . session . commit () Init and update new_duck = Duck () new_duck . name = name new_duck . duck_type_id = duck_type_id db . session . merge ( new_duck ) db . session . commit () Update Alphaz include a special update method that simplifies updates via api routes Model as a parameter Warning This is not recommanded because you could not specified if a field of Duck is required or not @route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"duck\" , ptype = Duck , required = True ) ], ) def update_duck (): return DB . update ( api [ \"duck\" ]) Route parameters to model @route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"name\" , ptype = str , required = True ), Parameter ( \"duck_type_id\" , ptype = int ) ], ) def update_duck (): return DB . update ( Duck ( ** api . get_parameters ()), not_none = True ) # not_none is to set if you dont want None values to update fields or using a function: def update_duck ( name : str , duck_type_id : str ): return DB . update ( Duck ( ** locals ())) @route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"name\" , ptype = str , required = True ), Parameter ( \"duck_type_id\" , ptype = int ) ], ) def update_duck (): return update_duck ( ** api . get_parameters ()) Relations Relation filter return DB . select ( Duck , filters = [ Duck . duck_type . has ( DuckType . name . like ( name ))] ) Will produce a query like: SELECT * FROM DUCK WHERE EXISTS ( SELECT 1 FROM DUCKTYPE where DUCKTYPE . id == DUCK . ducktype_id and DUCKTYPE . name = name ) Doc",
-            "title": "Database"
-        },
-        {
-            "location": "alpha_database/#alpha-database-system",
-            "text": "",
-            "title": "Alpha database system"
-        },
-        {
-            "location": "alpha_database/#automatic-structure",
-            "text": "Compared to native SqlAlchemy in alpha you only need to instantiate the table model: from alphaz.models.database.models import AlphaTable , AlphaColumn , Text , integer from core import DB class DuckType ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck_type\" type_id = AlphaColumn ( Integer , primary_key = True , autoincrement = True ) name = AlphaColumn ( Text , nullable = False , default = \"SuperDuck\" ) class DuckMedal ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck_medal\" name = AlphaColumn ( Text , nullable = False , default = \"Lucky\" ) duck_id = AlphaColumn ( Integer , ForeignKey ( 'duck.duck_id' ), nullable = False , default = - 1 ) class Duck ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck\" duck_id = AlphaColumn ( Integer , primary_key = True , autoincrement = True , visible = False ) name = AlphaColumn ( Text , nullable = False , default = \"\" ) # Many to one duck_type_id = AlphaColumn ( Integer , ForeignKey ( 'duck_type.type_id' ), nullable = False , default = - 1 , visible = False ) duck_type = relationship ( \"DuckType\" ) # One to many medals = relationship ( \"DuckMedals\" ) By default a select query on Duck class defined like this: master_duck = DuckType ( ame = \"Master Duck\" ) DB . add ( master_duck ) ducky = Duck ( name = \"Ducky\" , duck_type = master_duck ) DB . add ( ducky ) honnor_medal = DuckMedal ( name = \"Honnor\" , duck_id = ducky . duck_id ) lucky_medal = DuckMedal ( name = \"Lucky\" , duck_id = ducky . duck_id ) DB . add ( ducky ) ducks = DB . select ( Duck , filters = [ Duck . name == \"Ducky\" ], first = True ) Will result in this: { \"duck_id\" : 1 , \"name\" : \"Ducky\" , \"duck_type\" : { \"type_id\" : 1 , \"duck_type\" : \"Master Duck\" }, \"medals\" : [{ \"name\" : \"Honnor\" }, { \"name\" : \"Lucky\" }] }",
-            "title": "Automatic structure"
-        },
-        {
-            "location": "alpha_database/#schema",
-            "text": "Note The associated Schema is created automatically, with classic and nested fields. However Marshmallow schema could be defined using the classic way Marshmallow : Set visible to False if you dont want the column to appears in the Schema. Important Schema must be defined after the Model DB = core . db class DuckTypeSchema ( Schema ): type_id = fields . Integer () name = fields . String () class DuckMedalSchema ( Schema ): name = fields . String () class DuckSchema ( Schema ): name = fields . String () # Many to One duck_type = fields . Nested ( DuckTypeSchema ) # One to many medals = fields . List ( fields . Nested ( DuckMedalSchema )) Important Alpha will automatically detect the schema if the name is defined as \"{ModelName}Schema\" and is located in the same file. Note In this mode, Schema could be defined automatically, excepted for nested fields.",
-            "title": "Schema"
-        },
-        {
-            "location": "alpha_database/#specific-schema",
-            "text": "Schema could be specified for every request: DB . select ( model = Duck , schema = DuckSchema )",
-            "title": "Specific Schema"
-        },
-        {
-            "location": "alpha_database/#alpha-notation",
-            "text": "",
-            "title": "Alpha notation"
-        },
-        {
-            "location": "alpha_database/#init",
-            "text": "This enable the use of model columns which is not possible using SqlAlchemy: attr = { Duck . name : name , Duck . duck_type_id : duck_type_id , } duck = Duck () duck . init ( attr ) or duck = Duck () duck . init ({ Duck . name : name , Duck . duck_type_id : duck_type_id , }) Instead of: attr = { Duck . name : name , Duck . duck_type_id : duck_type_id , } duck = Duck () duck . init ( ** { x . key : y for x , y in attr . items ()})",
-            "title": "init"
-        },
-        {
-            "location": "alpha_database/#update",
-            "text": "",
-            "title": "Update"
-        },
-        {
-            "location": "alpha_database/#classic-sqlalchemy",
-            "text": "",
-            "title": "Classic SQLAlchemy"
-        },
-        {
-            "location": "alpha_database/#select-query",
-            "text": "duck = Duck . query . filter_by ( name = name ) . first () duck . duck_type_id = duck_type_id db . session . commit ()",
-            "title": "Select query"
-        },
-        {
-            "location": "alpha_database/#init_1",
-            "text": "new_duck = Duck ( \"name\" : name , \"duck_type_id\" : duck_type_id ) db . session . merge ( new_duck ) db . session . commit () or attr = { \"name\" : name , \"duck_type_id\" : duck_type_id , } duck = Duck ( ** attr ) db . session . merge ( new_duck ) db . session . commit ()",
-            "title": "Init"
-        },
-        {
-            "location": "alpha_database/#init-and-update",
-            "text": "new_duck = Duck () new_duck . name = name new_duck . duck_type_id = duck_type_id db . session . merge ( new_duck ) db . session . commit ()",
-            "title": "Init and update"
-        },
-        {
-            "location": "alpha_database/#update_1",
-            "text": "Alphaz include a special update method that simplifies updates via api routes",
-            "title": "Update"
-        },
-        {
-            "location": "alpha_database/#model-as-a-parameter",
-            "text": "Warning This is not recommanded because you could not specified if a field of Duck is required or not @route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"duck\" , ptype = Duck , required = True ) ], ) def update_duck (): return DB . update ( api [ \"duck\" ])",
-            "title": "Model as a parameter"
-        },
-        {
-            "location": "alpha_database/#route-parameters-to-model",
-            "text": "@route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"name\" , ptype = str , required = True ), Parameter ( \"duck_type_id\" , ptype = int ) ], ) def update_duck (): return DB . update ( Duck ( ** api . get_parameters ()), not_none = True ) # not_none is to set if you dont want None values to update fields or using a function: def update_duck ( name : str , duck_type_id : str ): return DB . update ( Duck ( ** locals ())) @route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"name\" , ptype = str , required = True ), Parameter ( \"duck_type_id\" , ptype = int ) ], ) def update_duck (): return update_duck ( ** api . get_parameters ())",
-            "title": "Route parameters to model"
-        },
-        {
-            "location": "alpha_database/#relations",
-            "text": "",
-            "title": "Relations"
-        },
-        {
-            "location": "alpha_database/#relation-filter",
-            "text": "return DB . select ( Duck , filters = [ Duck . duck_type . has ( DuckType . name . like ( name ))] ) Will produce a query like: SELECT * FROM DUCK WHERE EXISTS ( SELECT 1 FROM DUCKTYPE where DUCKTYPE . id == DUCK . ducktype_id and DUCKTYPE . name = name ) Doc",
-            "title": "Relation filter"
-        },
-        {
             "location": "alpha_screens/",
             "text": "Alpha screens system Alpha integrate a simple utility that enable to ensure that a screen if running or not. optional arguments: -h, * --help show this help message and exit --log LOG, -l LOG log file path --file FILE, -f FILE Input configuration file --name NAME, -n NAME Screen name --cmd CMD, -c CMD Command to run --envs ENVS [ENVS ...], -e ENVS [ENVS ...] Command to run --directory DIRECTORY, -d DIRECTORY Working directory --request REQUEST, -req REQUEST Request to check the response --retries RETRIES, -ret RETRIES Number of check before fail state --sleep SLEEP, -s SLEEP Sleep time (s) --timeout TIMEOUT, -t TIMEOUT Sleep time (s) --message MESSAGE, -m MESSAGE Check message --failed_message FAILED_MESSAGE, -fm FAILED_MESSAGE Failed message --success_message SUCCESS_MESSAGE, -sm SUCCESS_MESSAGE Success message --restart, -r Force a restart Launch Easy to launch, two modes are available: Configuration file python -m alphaz.utils.screens -f <config_file_path> The configuration format is the following, it use the dynamic json alpha configuration syntax : { \"screens\" : { \"api\" : { \"active\" : true , \"name\" : \"API\" , \"dir\" : \"{{home}}/{{name}}\" , \"shell_cmd\" : \"python api.py\" , \"request\" : \"http://0.0.0.0:{{port}}/status\" , \"fail_message\" : \"Api failed to restart\" }, \"api\" : { \"active\" : false , \"name\" : \"API\" , \"dir\" : \"{{home}}/{{name}}\" , \"shell_cmd\" : \"python api.py\" , \"request\" : \"http://0.0.0.0:{{port}}/status\" , \"fail_message\" : \"Failed\" } }, \"configurations\" : { \"local\" : { \"port\" : \"auto\" }, \"dev\" : { \"port\" : 3000 }, \"prod\" : { \"port\" : 5000 } }, \"home\" : \"/home/mes\" , \"name\" : \"pyMES\" } Parameters: python -m alphaz.utils.screens * --name TEST * --cmd \"python api.py\" Help python -m alphaz.utils.screens",
             "title": "Screens"
         },
         {
             "location": "alpha_screens/#alpha-screens-system",
             "text": "Alpha integrate a simple utility that enable to ensure that a screen if running or not. optional arguments: -h, * --help show this help message and exit --log LOG, -l LOG log file path --file FILE, -f FILE Input configuration file --name NAME, -n NAME Screen name --cmd CMD, -c CMD Command to run --envs ENVS [ENVS ...], -e ENVS [ENVS ...] Command to run --directory DIRECTORY, -d DIRECTORY Working directory --request REQUEST, -req REQUEST Request to check the response --retries RETRIES, -ret RETRIES Number of check before fail state --sleep SLEEP, -s SLEEP Sleep time (s) --timeout TIMEOUT, -t TIMEOUT Sleep time (s) --message MESSAGE, -m MESSAGE Check message --failed_message FAILED_MESSAGE, -fm FAILED_MESSAGE Failed message --success_message SUCCESS_MESSAGE, -sm SUCCESS_MESSAGE Success message --restart, -r Force a restart",
@@ -430,14 +175,34 @@
         },
         {
             "location": "alpha_setup/#angular",
             "text": "{ \"compilerOptions\" : { \"baseUrl\" : \"./src\" , \"paths\" : { \"@services/*\" : [ \"app/services/*\" , \"src/app/services/*\" ], \"@views/*\" : [ \"app/views/*\" , \"src/app/views/*\" ], \"@models/*\" : [ \"app/models/*\" , \"src/app/models/*\" ], \"@components/*\" : [ \"app/components/*\" , \"src/app/components/*\" ], \"@alphaa/*\" : [ \"alphaa/*\" , \"src/alphaa/*\" ], \"@layout/*\" : [ \"app/layout/*\" , \"src/app/layout/*\" ], \"@envs/*\" : [ \"environments/*\" , \"src/environments/*\" ], \"@constants/*\" : [ \"app/constants/*\" , \"src/app/constants/*\" ] } } }",
             "title": "Angular"
         },
         {
+            "location": "api_database/",
+            "text": "Update Alphaz include a special update method that simplifies updates via api routes Model as a parameter Warning This is not recommanded because you could not specified if a field of Duck is required or not @route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"duck\" , ptype = Duck , required = True ) ], ) def update_duck (): return DB . update ( api [ \"duck\" ]) Route parameters to model @route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"name\" , ptype = str , required = True ), Parameter ( \"duck_type_id\" , ptype = int ) ], ) def update_duck (): return DB . update ( Duck ( ** api . get_parameters ()), not_none = True ) # not_none is to set if you dont want None values to update fields or using a function: def update_duck ( name : str , duck_type_id : str ): return DB . update ( Duck ( ** locals ())) @route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"name\" , ptype = str , required = True ), Parameter ( \"duck_type_id\" , ptype = int ) ], ) def update_duck (): return update_duck ( ** api . get_parameters ())",
+            "title": "Model Parameters"
+        },
+        {
+            "location": "api_database/#update",
+            "text": "Alphaz include a special update method that simplifies updates via api routes",
+            "title": "Update"
+        },
+        {
+            "location": "api_database/#model-as-a-parameter",
+            "text": "Warning This is not recommanded because you could not specified if a field of Duck is required or not @route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"duck\" , ptype = Duck , required = True ) ], ) def update_duck (): return DB . update ( api [ \"duck\" ])",
+            "title": "Model as a parameter"
+        },
+        {
+            "location": "api_database/#route-parameters-to-model",
+            "text": "@route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"name\" , ptype = str , required = True ), Parameter ( \"duck_type_id\" , ptype = int ) ], ) def update_duck (): return DB . update ( Duck ( ** api . get_parameters ()), not_none = True ) # not_none is to set if you dont want None values to update fields or using a function: def update_duck ( name : str , duck_type_id : str ): return DB . update ( Duck ( ** locals ())) @route ( path = 'duck' , methods = [ \"PUT\" ], parameters = [ Parameter ( \"name\" , ptype = str , required = True ), Parameter ( \"duck_type_id\" , ptype = int ) ], ) def update_duck (): return update_duck ( ** api . get_parameters ())",
+            "title": "Route parameters to model"
+        },
+        {
             "location": "configuration/",
             "text": "Dynamic json alpha configuration syntax Parameters Main project_name: in order to specify the project name Directories You must at least specify the root and home directories: \"root\" : \"/application/{{user}}\" , \"home\" : \"/home/{{user}}\" , Other main directories could be defined in a sub directories path: \"directories\" : { \"data\" : \"{{root}}/data\" , \"logs\" : \"{{root}}/logs\" , \"cache\" : \"{{root}}/cache\" } System environments variables In order to set operating system environment variables \"envs\" : { \"ORACLE_HOME\" : \"/application/software/oracle/12.1.0.2\" } Environments configurations In order to specify the envs configurations: \"configuration\" : \"local\" , \"configurations\" : { \"local\" : { \"debug\" : true , \"host_public\" : \"\" , \"host_web\" : \"\" , \"port\" : 5006 , \"ssl_cert\" : \"\" , \"ssl_key\" : \"\" , \"admin\" : true , \"admin_databases\" : true }, \"dev\" : { \"debug\" : true , \"host_public\" : \"\" , \"host_web\" : \"\" , \"port\" : 5000 , \"ssl_cert\" : \"\" , \"ssl_key\" : \"\" , \"admin\" : true , \"admin_databases\" : true } } configuration parameter is the default one. Users Configuration could be modified dynamically depending on the user \"users\" : { \"user_dev\" : { \"debug\" : false , \"mode\" : \"wsgi\" , \"configuration\" : \"dev\" }, \"user_int\" : { \"debug\" : false , \"mode\" : \"wsgi\" , \"configuration\" : \"int\" }, \"user_acc\" : { \"debug\" : false , \"mode\" : \"wsgi\" , \"configuration\" : \"acc\" }, \"user_prod\" : { \"debug\" : false , \"mode\" : \"wsgi\" , \"configuration\" : \"prod\" } } Platforms Configuration could be modified dynamically depending on the operating system \"platforms\" : { \"windows\" : { \"root\" : \"/alpha/{{user}}\" , \"home\" : \"/alpha/{{user}}\" , \"host\" : \"0.0.0.0\" } }, Loggers In order the specify the loggers configurations: \"loggers\" : { \"main\" : { \"level\" : \"debug\" }, \"database\" : { \"level\" : \"debug\" } } Tests In order to specify the directories that contains tests: \"tests\" : { \"auto_directory\" : \"tests/auto\" , \"auto_import\" : \"alphaz.tests.auto\" , \"save_directory\" : \"{{save_root}}/tests\" }, Menu \"menus\" : { \"save_directory\" : \"{{save_root}}/menus\" },",
             "title": "Configuration"
         },
         {
             "location": "configuration/#dynamic-json-alpha-configuration-syntax",
             "text": "",
@@ -508,10 +273,240 @@
             "text": "install packages pip install pymdown-extensions pygments mkdocs-material Add extensions in mkdocs.yaml markdown_extensions: - admonition - pymdownx.arithmatex - pymdownx.details - codehilite - pymdownx.superfences",
             "title": "Requirements"
         },
         {
             "location": "documentation/#more",
             "text": "for more information",
             "title": "More"
+        },
+        {
+            "location": "api/authorizations/",
+            "text": "Route can be protected using the login system or admin rights. Login system To protect a route using the login system you must specify: logged=True @route ( 'protected' , logged = True ) def protected_route (): user = api . get_logged_user () return user User information can be accessed using get_logged_user method. Admin Admin could auto log to any user account on local mode Condition To be an admin a user must have at least one condition: a role > 9 specify the magic password has admin API parameter connect using an admin ip. The ips admin list must be defined in the api.json configuration files under the key = admins_ips How to use If you met one of the admin condition you do not need any password in order to log has any of the user in the database. You could be logged for specific routes using the single route mode or to any route using the login/logout system. Single route mode You could specifiy either admin_user_id={user_id} or admin_user_name={username} directly into any request in order to login with this user for this specific route. Exemple /anyroute?admin_user_id=1000 Login to the api Use the route /auth/su in order to set an admin session that is valid until the end of the api runtime. You must specifiy either admin_user_id={user_id} or admin_user_name={username} Exemple /auth/su?admin_user_id=1000 Logout from the api Use the route /logout/su in order to logout.",
+            "title": "Authorizations"
+        },
+        {
+            "location": "api/authorizations/#login-system",
+            "text": "To protect a route using the login system you must specify: logged=True @route ( 'protected' , logged = True ) def protected_route (): user = api . get_logged_user () return user User information can be accessed using get_logged_user method.",
+            "title": "Login system"
+        },
+        {
+            "location": "api/authorizations/#admin",
+            "text": "Admin could auto log to any user account on local mode",
+            "title": "Admin"
+        },
+        {
+            "location": "api/authorizations/#condition",
+            "text": "To be an admin a user must have at least one condition: a role > 9 specify the magic password has admin API parameter connect using an admin ip. The ips admin list must be defined in the api.json configuration files under the key = admins_ips",
+            "title": "Condition"
+        },
+        {
+            "location": "api/authorizations/#how-to-use",
+            "text": "If you met one of the admin condition you do not need any password in order to log has any of the user in the database. You could be logged for specific routes using the single route mode or to any route using the login/logout system.",
+            "title": "How to use"
+        },
+        {
+            "location": "api/authorizations/#single-route-mode",
+            "text": "You could specifiy either admin_user_id={user_id} or admin_user_name={username} directly into any request in order to login with this user for this specific route. Exemple /anyroute?admin_user_id=1000",
+            "title": "Single route mode"
+        },
+        {
+            "location": "api/authorizations/#login-to-the-api",
+            "text": "Use the route /auth/su in order to set an admin session that is valid until the end of the api runtime. You must specifiy either admin_user_id={user_id} or admin_user_name={username} Exemple /auth/su?admin_user_id=1000",
+            "title": "Login to the api"
+        },
+        {
+            "location": "api/authorizations/#logout-from-the-api",
+            "text": "Use the route /logout/su in order to logout.",
+            "title": "Logout from the api"
+        },
+        {
+            "location": "api/cache/",
+            "text": "A cache system is implemented, in order to use it you must specify the",
+            "title": "Cache"
+        },
+        {
+            "location": "api/configuration/",
+            "text": "The api is automatically configured from the api.jon file. See Configuration for further details on how to use it. Main workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.databases\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false } Mails In order to specify the mails configurations \"mails\" : { \"mail_server\" : { \"host\" : \"\" , \"mail\" : \"\" , \"password\" : \"\" , \"port\" : 465 , \"server\" : \"\" , \"ssl\" : true , \"tls\" : false } } Auth In order to specify the auth mode \"auth\" : { \"mode\" : \"ldap\" , \"ldap\" : { \"server\" : \"ldap://path_to_ldap\" , \"baseDN\" : \"ou=people,dc=a_name,dc=com\" , \"users_filters\" : \"(|(uid={uid})(mail={mail})(cn={cn}))\" , \"user_filters\" : \"(|(uid={username})(mail={username})(cn={username}))\" , \"user_data\" : { \"givenName\" : \"name\" , \"sn\" : \"lastname\" , \"c\" : \"area\" , \"st-locationdescription\" : \"location\" , \"st-seatnumber\" : \"seat\" , \"telephoneNumber\" : \"phone-number\" } }, \"users\" : { \"a_user_name\" : { \"user_permissions\" : [ \"SUPER_USER\" ] } } }, Reloader type In order to specify the Werkzeug reloader type \"reloader_type\" : \"stat\" Admin In order to specify the admins configurations \"admins\" : { \"ips\" :[ \"127.0.0.1\" ], \"password\" : \"a_password\" }, Dashboard In order to configure the Flask-Monitoring Dashboard \"dashboard\" : { \"dashboard\" : { \"APP_VERSION\" : 1.0 , \"SAMPLING_PERIOD\" : 20 , \"ENABLE_LOGGING\" : true , \"active\" : false }, \"authentication\" : { \"USERNAME\" : \"username\" , \"PASSWORD\" : \"\" , \"GUEST_USERNAME\" : \"guest\" , \"GUEST_PASSWORD\" : [ \"guest1\" , \"guest2\" ], \"SECURITY_TOKEN\" : \"a_security_token\" }, \"database\" : { \"DATABASE\" : \"sqlite:///{{root}}/dashboard.db\" } }",
+            "title": "Configuration"
+        },
+        {
+            "location": "api/configuration/#main",
+            "text": "workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.databases\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false }",
+            "title": "Main"
+        },
+        {
+            "location": "api/configuration/#mails",
+            "text": "In order to specify the mails configurations \"mails\" : { \"mail_server\" : { \"host\" : \"\" , \"mail\" : \"\" , \"password\" : \"\" , \"port\" : 465 , \"server\" : \"\" , \"ssl\" : true , \"tls\" : false } }",
+            "title": "Mails"
+        },
+        {
+            "location": "api/configuration/#auth",
+            "text": "In order to specify the auth mode \"auth\" : { \"mode\" : \"ldap\" , \"ldap\" : { \"server\" : \"ldap://path_to_ldap\" , \"baseDN\" : \"ou=people,dc=a_name,dc=com\" , \"users_filters\" : \"(|(uid={uid})(mail={mail})(cn={cn}))\" , \"user_filters\" : \"(|(uid={username})(mail={username})(cn={username}))\" , \"user_data\" : { \"givenName\" : \"name\" , \"sn\" : \"lastname\" , \"c\" : \"area\" , \"st-locationdescription\" : \"location\" , \"st-seatnumber\" : \"seat\" , \"telephoneNumber\" : \"phone-number\" } }, \"users\" : { \"a_user_name\" : { \"user_permissions\" : [ \"SUPER_USER\" ] } } },",
+            "title": "Auth"
+        },
+        {
+            "location": "api/configuration/#reloader-type",
+            "text": "In order to specify the Werkzeug reloader type \"reloader_type\" : \"stat\"",
+            "title": "Reloader type"
+        },
+        {
+            "location": "api/configuration/#admin",
+            "text": "In order to specify the admins configurations \"admins\" : { \"ips\" :[ \"127.0.0.1\" ], \"password\" : \"a_password\" },",
+            "title": "Admin"
+        },
+        {
+            "location": "api/configuration/#dashboard",
+            "text": "In order to configure the Flask-Monitoring Dashboard \"dashboard\" : { \"dashboard\" : { \"APP_VERSION\" : 1.0 , \"SAMPLING_PERIOD\" : 20 , \"ENABLE_LOGGING\" : true , \"active\" : false }, \"authentication\" : { \"USERNAME\" : \"username\" , \"PASSWORD\" : \"\" , \"GUEST_USERNAME\" : \"guest\" , \"GUEST_PASSWORD\" : [ \"guest1\" , \"guest2\" ], \"SECURITY_TOKEN\" : \"a_security_token\" }, \"database\" : { \"DATABASE\" : \"sqlite:///{{root}}/dashboard.db\" } }",
+            "title": "Dashboard"
+        },
+        {
+            "location": "api/issues/",
+            "text": "Issues In progress",
+            "title": "Issues"
+        },
+        {
+            "location": "api/issues/#issues",
+            "text": "In progress",
+            "title": "Issues"
+        },
+        {
+            "location": "api/main/",
+            "text": "Introduction The api system is completely based on Flask and compatible with it. You could use Flask inside Alpha system without any issue. Launch To start the api execute the api.py file python api.py Note set ALPHA_CONF environment parameter is you want to set the environment. Verify the deployment by navigating to your server address in your preferred browser: 127 .0.0.1:<port> How to use Your could import it using simply from the utils : from alphaz.utils.api import api or from the core if you are using it from core import core , API api / API is the equivalent for app in Flask framework.",
+            "title": "Main"
+        },
+        {
+            "location": "api/main/#introduction",
+            "text": "The api system is completely based on Flask and compatible with it. You could use Flask inside Alpha system without any issue.",
+            "title": "Introduction"
+        },
+        {
+            "location": "api/main/#launch",
+            "text": "To start the api execute the api.py file python api.py Note set ALPHA_CONF environment parameter is you want to set the environment. Verify the deployment by navigating to your server address in your preferred browser: 127 .0.0.1:<port>",
+            "title": "Launch"
+        },
+        {
+            "location": "api/main/#how-to-use",
+            "text": "Your could import it using simply from the utils : from alphaz.utils.api import api or from the core if you are using it from core import core , API api / API is the equivalent for app in Flask framework.",
+            "title": "How to use"
+        },
+        {
+            "location": "api/methods/",
+            "text": "Methods are specified the same way as in Flask , using methods parameter: @route ( 'logs' , methods = [ \"GET\" ]) def get_logs (): return db . select ( Logs ) @route ( 'logs' , methods = [ \"POST\" ]) def set_logs (): return db . add ( Logs ) Methods can be managed using different routes or within a single route : @route ( 'logs' , methods = [ \"GET\" , \"POST\" , \"DELETE\" ]) def get_logs (): if api . is_get (): return db . select ( Logs ) elif api . is_post (): return db . add ( Logs ) elif api . is_delete (): return db . delete ( Logs )",
+            "title": "Methods"
+        },
+        {
+            "location": "api/parameters/",
+            "text": "Simple You could simply define parameters by listing all parameters in parameters list: from alphaz.utils.api import route , api , Parameter @route ( \"books\" , parameters = [ \"name\" ]) def method_name (): return \"Book name is %s or %s \" % ( api [ \"name\" ], api . get ( \"name\" , default = \"\" )) Parameter value is accessed by api instance, using get method, they could also be accessed using get_parameters method from api instance. Object Or you could use the Parameter class to specify properties such as: ptype : value type int, str, bool, SqlAlchemy model parameter is automatically converted to the specified type if conversion failed an exception is raised required : the parameter is required or not default : default parameter value options : authorized values mode : input mode cacheable : parameter is taken into acount in the caching system or not private : parameter is hiden from documentation or not @route ( \"/logs\" , parameters = [ Parameter ( 'page' , required = True , ptype = int ), Parameter ( 'startDate' , required = True ), Parameter ( 'endDate' , default = None ), Parameter ( 'error' , options = [ \"Y\" , \"N\" ]) ]) def admin_logs (): return get_logs ( ** api . get_parameters ()) Promote this method as it allows a better control on parameters Default parameters Some parameter are always available: - no_log (bool): disable logs for this route - reset_cache (bool): reset cache before calling this route - requester (str): requester to this route - format (str): output format - json: - xml: - admin (str): admin password - admin_user_id (int): id of the user to connect has an admin",
+            "title": "Parameters"
+        },
+        {
+            "location": "api/parameters/#simple",
+            "text": "You could simply define parameters by listing all parameters in parameters list: from alphaz.utils.api import route , api , Parameter @route ( \"books\" , parameters = [ \"name\" ]) def method_name (): return \"Book name is %s or %s \" % ( api [ \"name\" ], api . get ( \"name\" , default = \"\" )) Parameter value is accessed by api instance, using get method, they could also be accessed using get_parameters method from api instance.",
+            "title": "Simple"
+        },
+        {
+            "location": "api/parameters/#object",
+            "text": "Or you could use the Parameter class to specify properties such as: ptype : value type int, str, bool, SqlAlchemy model parameter is automatically converted to the specified type if conversion failed an exception is raised required : the parameter is required or not default : default parameter value options : authorized values mode : input mode cacheable : parameter is taken into acount in the caching system or not private : parameter is hiden from documentation or not @route ( \"/logs\" , parameters = [ Parameter ( 'page' , required = True , ptype = int ), Parameter ( 'startDate' , required = True ), Parameter ( 'endDate' , default = None ), Parameter ( 'error' , options = [ \"Y\" , \"N\" ]) ]) def admin_logs (): return get_logs ( ** api . get_parameters ()) Promote this method as it allows a better control on parameters",
+            "title": "Object"
+        },
+        {
+            "location": "api/parameters/#default-parameters",
+            "text": "Some parameter are always available: - no_log (bool): disable logs for this route - reset_cache (bool): reset cache before calling this route - requester (str): requester to this route - format (str): output format - json: - xml: - admin (str): admin password - admin_user_id (int): id of the user to connect has an admin",
+            "title": "Default parameters"
+        },
+        {
+            "location": "api/routes/",
+            "text": "We recommend to add all the route definition in apis/routes folder and import all the route definition in apis/routes/ init .py . Then you will have to import the route in thoe core.py file: from alphaz.models.main import AlphaCore , singleton @singleton class Core ( AlphaCore ): def __init__ ( self , file : str ): super () . __init__ ( file ) core = Core ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded from apis.routes import * Basic To specify an api route, juste use the route flag: from alphaz.utils.api import route , api , Parameter @route ( \"route_name\" ) def method_name (): return \"hello\" Method automatically convert the output to the right format. Default format is json Description A description could be specified: @route ( \"route_name\" , description = \"This route say hello\" ) def method_name (): return \"hello\" Category The routes are organized by category , by default the route category is defined by it file name , but it could be specified using the cat parameter: @route ( \"route_name\" , category = \"politeness\" ) def method_name (): return \"hello\"",
+            "title": "Routes"
+        },
+        {
+            "location": "api/routes/#basic",
+            "text": "To specify an api route, juste use the route flag: from alphaz.utils.api import route , api , Parameter @route ( \"route_name\" ) def method_name (): return \"hello\" Method automatically convert the output to the right format. Default format is json",
+            "title": "Basic"
+        },
+        {
+            "location": "api/routes/#description",
+            "text": "A description could be specified: @route ( \"route_name\" , description = \"This route say hello\" ) def method_name (): return \"hello\"",
+            "title": "Description"
+        },
+        {
+            "location": "api/routes/#category",
+            "text": "The routes are organized by category , by default the route category is defined by it file name , but it could be specified using the cat parameter: @route ( \"route_name\" , category = \"politeness\" ) def method_name (): return \"hello\"",
+            "title": "Category"
+        },
+        {
+            "location": "api/sqlalchemy/",
+            "text": "If you specify a SqlAlchemy model as a type it will be automatically converted to the specified model. from core import core db = core . db class Logs ( db . Model , AlphaTable ): __tablename__ = 'LOGS' id = AlphaColumn ( Integer , nullable = False , primary_key = True ) name = AlphaColumn ( String , nullable = False ) @route ( \"logs\" , parameters = [ Parameter ( 'log' , ptype = Logs ) ]) def admin_logs (): db . add ( api [ 'log' ])",
+            "title": "SqlAlchemy"
+        },
+        {
+            "location": "database/init/",
+            "text": "Route The route database/init could be use to init the database or some tables. @route ( \"/database/init\" , admin = True , parameters = [ Parameter ( \"binds\" , ptype = List [ str ]), Parameter ( \"tables\" , ptype = List [ str ]), Parameter ( \"drop\" , ptype = bool , default = False ), Parameter ( \"truncate\" , ptype = bool , default = False ), Parameter ( \"force\" , ptype = bool , default = False ), Parameter ( \"create\" , ptype = bool , default = False ), ], ) Configuration Content of tables could be pre-defined in various ways: python : you have to specify the directory where the py files are defined using the init_database_dir_py parameter in your database configuration. For every table you want to fill you could specify objects which are models in this situation: from models.database.olca import TblGroups ini = { TblGroups : { \"objects\" : [ TblGroups . instantiate ( 2 , \"hidden\" , \"far fa-eye-slash\" , \"var(--ion-color-light)\" ), TblGroups . instantiate ( 3 , \"steps\" , \"fas fa-cogs\" , \"var(--ion-color-danger)\" ), TblGroups . instantiate ( 4 , \"materials\" , \"fas fa-cubes\" , \"var(--ion-color-primary)\" ), TblGroups . instantiate ( 5 , \"transports\" , \"fas fa-dolly-flatbed\" , \"var(--ion-color-secondary)\" ), TblGroups . instantiate ( 6 , \"powers\" , \"fas fa-lightbulb\" , \"var(--ion-color-warning)\" ), ] }, } json : you have to specify the directory where the json files are defined using the init_database_dir_json parameter in your database configuration. { \"sophisme\" : { \"headers\" : [ \"theme\" , \"sophisme\" , \"user\" , \"proposition\" ], \"values\" : [ [ 5 , 20 , 6 , 34 ], [ 5 , 7 , 1 , 35 ], [ 5 , 9 , 1 , 35 ] ] } } sql : you have to specify the directory where the sql files are defined using the init_database_dir_sql parameter in your database configuration. Here the code is directly executed, so it could have any valid sql structure.",
+            "title": "Init"
+        },
+        {
+            "location": "database/init/#route",
+            "text": "The route database/init could be use to init the database or some tables. @route ( \"/database/init\" , admin = True , parameters = [ Parameter ( \"binds\" , ptype = List [ str ]), Parameter ( \"tables\" , ptype = List [ str ]), Parameter ( \"drop\" , ptype = bool , default = False ), Parameter ( \"truncate\" , ptype = bool , default = False ), Parameter ( \"force\" , ptype = bool , default = False ), Parameter ( \"create\" , ptype = bool , default = False ), ], )",
+            "title": "Route"
+        },
+        {
+            "location": "database/init/#configuration",
+            "text": "Content of tables could be pre-defined in various ways: python : you have to specify the directory where the py files are defined using the init_database_dir_py parameter in your database configuration. For every table you want to fill you could specify objects which are models in this situation: from models.database.olca import TblGroups ini = { TblGroups : { \"objects\" : [ TblGroups . instantiate ( 2 , \"hidden\" , \"far fa-eye-slash\" , \"var(--ion-color-light)\" ), TblGroups . instantiate ( 3 , \"steps\" , \"fas fa-cogs\" , \"var(--ion-color-danger)\" ), TblGroups . instantiate ( 4 , \"materials\" , \"fas fa-cubes\" , \"var(--ion-color-primary)\" ), TblGroups . instantiate ( 5 , \"transports\" , \"fas fa-dolly-flatbed\" , \"var(--ion-color-secondary)\" ), TblGroups . instantiate ( 6 , \"powers\" , \"fas fa-lightbulb\" , \"var(--ion-color-warning)\" ), ] }, } json : you have to specify the directory where the json files are defined using the init_database_dir_json parameter in your database configuration. { \"sophisme\" : { \"headers\" : [ \"theme\" , \"sophisme\" , \"user\" , \"proposition\" ], \"values\" : [ [ 5 , 20 , 6 , 34 ], [ 5 , 7 , 1 , 35 ], [ 5 , 9 , 1 , 35 ] ] } } sql : you have to specify the directory where the sql files are defined using the init_database_dir_sql parameter in your database configuration. Here the code is directly executed, so it could have any valid sql structure.",
+            "title": "Configuration"
+        },
+        {
+            "location": "database/instantiate/",
+            "text": "This enable the use of model columns which is not possible using SqlAlchemy: attr = { Duck . name : name , Duck . duck_type_id : duck_type_id , } duck = Duck () duck . init ( attr ) or duck = Duck () duck . init ({ Duck . name : name , Duck . duck_type_id : duck_type_id , }) Instead of: attr = { Duck . name : name , Duck . duck_type_id : duck_type_id , } duck = Duck () duck . init ( ** { x . key : y for x , y in attr . items ()})",
+            "title": "Instantiate"
+        },
+        {
+            "location": "database/main/",
+            "text": "Alpha integrate some update to SqlAlchemy. This does not prevent from using standard FlaskSqlAlchemy notations.",
+            "title": "Main"
+        },
+        {
+            "location": "database/model/",
+            "text": "Automatic structure Compared to native SqlAlchemy in alpha you only need to instantiate the table model: from alphaz.models.database.models import AlphaTable , AlphaColumn , Text , integer from core import DB class DuckType ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck_type\" type_id = AlphaColumn ( Integer , primary_key = True , autoincrement = True ) name = AlphaColumn ( Text , nullable = False , default = \"SuperDuck\" ) class DuckMedal ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck_medal\" name = AlphaColumn ( Text , nullable = False , default = \"Lucky\" ) duck_id = AlphaColumn ( Integer , ForeignKey ( 'duck.duck_id' ), nullable = False , default = - 1 ) class Duck ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck\" duck_id = AlphaColumn ( Integer , primary_key = True , autoincrement = True , visible = False ) name = AlphaColumn ( Text , nullable = False , default = \"\" ) # Many to one duck_type_id = AlphaColumn ( Integer , ForeignKey ( 'duck_type.type_id' ), nullable = False , default = - 1 , visible = False ) duck_type = relationship ( \"DuckType\" ) # One to many medals = relationship ( \"DuckMedals\" ) By default a select query on Duck class defined like this: master_duck = DuckType ( ame = \"Master Duck\" ) DB . add ( master_duck ) ducky = Duck ( name = \"Ducky\" , duck_type = master_duck ) DB . add ( ducky ) honnor_medal = DuckMedal ( name = \"Honnor\" , duck_id = ducky . duck_id ) lucky_medal = DuckMedal ( name = \"Lucky\" , duck_id = ducky . duck_id ) DB . add ( ducky ) ducks = DB . select ( Duck , filters = [ Duck . name == \"Ducky\" ], first = True ) Will result in this: { \"duck_id\" : 1 , \"name\" : \"Ducky\" , \"duck_type\" : { \"type_id\" : 1 , \"duck_type\" : \"Master Duck\" }, \"medals\" : [{ \"name\" : \"Honnor\" }, { \"name\" : \"Lucky\" }] }",
+            "title": "Model"
+        },
+        {
+            "location": "database/model/#automatic-structure",
+            "text": "Compared to native SqlAlchemy in alpha you only need to instantiate the table model: from alphaz.models.database.models import AlphaTable , AlphaColumn , Text , integer from core import DB class DuckType ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck_type\" type_id = AlphaColumn ( Integer , primary_key = True , autoincrement = True ) name = AlphaColumn ( Text , nullable = False , default = \"SuperDuck\" ) class DuckMedal ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck_medal\" name = AlphaColumn ( Text , nullable = False , default = \"Lucky\" ) duck_id = AlphaColumn ( Integer , ForeignKey ( 'duck.duck_id' ), nullable = False , default = - 1 ) class Duck ( DB . Model , AlphaTable ): __bind_key__ = DB __tablename__ = \"duck\" duck_id = AlphaColumn ( Integer , primary_key = True , autoincrement = True , visible = False ) name = AlphaColumn ( Text , nullable = False , default = \"\" ) # Many to one duck_type_id = AlphaColumn ( Integer , ForeignKey ( 'duck_type.type_id' ), nullable = False , default = - 1 , visible = False ) duck_type = relationship ( \"DuckType\" ) # One to many medals = relationship ( \"DuckMedals\" ) By default a select query on Duck class defined like this: master_duck = DuckType ( ame = \"Master Duck\" ) DB . add ( master_duck ) ducky = Duck ( name = \"Ducky\" , duck_type = master_duck ) DB . add ( ducky ) honnor_medal = DuckMedal ( name = \"Honnor\" , duck_id = ducky . duck_id ) lucky_medal = DuckMedal ( name = \"Lucky\" , duck_id = ducky . duck_id ) DB . add ( ducky ) ducks = DB . select ( Duck , filters = [ Duck . name == \"Ducky\" ], first = True ) Will result in this: { \"duck_id\" : 1 , \"name\" : \"Ducky\" , \"duck_type\" : { \"type_id\" : 1 , \"duck_type\" : \"Master Duck\" }, \"medals\" : [{ \"name\" : \"Honnor\" }, { \"name\" : \"Lucky\" }] }",
+            "title": "Automatic structure"
+        },
+        {
+            "location": "database/relations/",
+            "text": "return DB . select ( Duck , filters = [ Duck . duck_type . has ( DuckType . name . like ( name ))] ) Will produce a query like: SELECT * FROM DUCK WHERE EXISTS ( SELECT 1 FROM DUCKTYPE where DUCKTYPE . id == DUCK . ducktype_id and DUCKTYPE . name = name ) Doc",
+            "title": "Relations"
+        },
+        {
+            "location": "database/schema/",
+            "text": "Note The associated Schema is created automatically, with classic and nested fields. However Marshmallow schema could be defined using the classic way Marshmallow : Set visible to False if you dont want the column to appears in the Schema. Important Schema must be defined after the Model DB = core . db class DuckTypeSchema ( Schema ): type_id = fields . Integer () name = fields . String () class DuckMedalSchema ( Schema ): name = fields . String () class DuckSchema ( Schema ): name = fields . String () # Many to One duck_type = fields . Nested ( DuckTypeSchema ) # One to many medals = fields . List ( fields . Nested ( DuckMedalSchema )) Important Alpha will automatically detect the schema if the name is defined as \"{ModelName}Schema\" and is located in the same file. Note In this mode, Schema could be defined automatically, excepted for nested fields. Specific Schema Schema could be specified for every request: DB . select ( model = Duck , schema = DuckSchema )",
+            "title": "Schema"
+        },
+        {
+            "location": "database/schema/#specific-schema",
+            "text": "Schema could be specified for every request: DB . select ( model = Duck , schema = DuckSchema )",
+            "title": "Specific Schema"
+        },
+        {
+            "location": "database/update/",
+            "text": "Select query duck = Duck . query . filter_by ( name = name ) . first () duck . duck_type_id = duck_type_id db . session . commit () Init new_duck = Duck ( \"name\" : name , \"duck_type_id\" : duck_type_id ) db . session . merge ( new_duck ) db . session . commit () or attr = { \"name\" : name , \"duck_type_id\" : duck_type_id , } duck = Duck ( ** attr ) db . session . merge ( new_duck ) db . session . commit () Init and update new_duck = Duck () new_duck . name = name new_duck . duck_type_id = duck_type_id db . session . merge ( new_duck ) db . session . commit ()",
+            "title": "Update"
+        },
+        {
+            "location": "database/update/#select-query",
+            "text": "duck = Duck . query . filter_by ( name = name ) . first () duck . duck_type_id = duck_type_id db . session . commit ()",
+            "title": "Select query"
+        },
+        {
+            "location": "database/update/#init",
+            "text": "new_duck = Duck ( \"name\" : name , \"duck_type_id\" : duck_type_id ) db . session . merge ( new_duck ) db . session . commit () or attr = { \"name\" : name , \"duck_type_id\" : duck_type_id , } duck = Duck ( ** attr ) db . session . merge ( new_duck ) db . session . commit ()",
+            "title": "Init"
+        },
+        {
+            "location": "database/update/#init-and-update",
+            "text": "new_duck = Duck () new_duck . name = name new_duck . duck_type_id = duck_type_id db . session . merge ( new_duck ) db . session . commit ()",
+            "title": "Init and update"
         }
     ]
 }
```

### Comparing `alphaz-0.7.3.9/alphaz/index.html` & `alphaz-0.7.4/alphaz/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/api_lib.py` & `alphaz-0.7.4/alphaz/libs/api_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
 def get_api_data(
     url: str,
     params: dict = {},
     log: AlphaLogger = None,
     method: ApiMethods = ApiMethods.GET,
     data_only: bool = True,
-    requester="EXT",
+    requester=None,
 ) -> dict:
     """Get data from api
 
     Args:
         url (str): [description]
         params (dict, optional): [description]. Defaults to {}.
         log (AlphaLogger, optional): [description]. Defaults to None.
```

### Comparing `alphaz-0.7.3.9/alphaz/libs/barcode_lib.py` & `alphaz-0.7.4/alphaz/libs/barcode_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/config_lib.py` & `alphaz-0.7.4/alphaz/libs/config_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,15 +361,15 @@
     elif "," in valueStr:
         listValues = valueStr.split(",")
         value = [convert_config_value(x.lstrip()) for x in listValues]
     elif stringMatch:
         # match = stringMatch.groups()[0]
         # value = match.replace('\'','')
         value = value[1:-1]
-    elif valueStr == "NONE" or valueStr is None:
+    elif str(value) == "None" or valueStr is None:
         value = None
     elif valueStr == "FALSE":
         value = False
     elif valueStr == "TRUE":
         value = True
     elif valueStr == "FLOAT":
         value = float
```

### Comparing `alphaz-0.7.3.9/alphaz/libs/converter_lib.py` & `alphaz-0.7.4/alphaz/libs/converter_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/database_lib.py` & `alphaz-0.7.4/alphaz/libs/database_lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,25 +47,29 @@
     init_databases_config = core.config.get("databases")
     if init_databases_config is None:
         raise AlphaException(
             "No initialisation configuration has been set in <databases> entry"
         )
     init_databases_config = {x.upper(): y for x, y in init_databases_config.items()}
 
-    core.db.init_all(tables=tables_models, create=create, drop=drop, sqlite=sqlite)
+    core.db.init_all(
+        tables=tables_models, create=create, drop=drop, sqlite=sqlite, log=core.log
+    )
 
     if tables is not None and truncate:
         for table_model in tables_models:
             core.db.truncate(table_model)
 
     ini_types = {
         "json": {"key": "init_database_dir_json", "pattern": "*.json"},
         "py": {"key": "init_database_dir_py", "pattern": "*.py"},
         "sql": {"key": "init_database_dir_sql", "pattern": "*.sql"},
     }
+    if not init:
+        return
 
     for bind in binds:
         if not bind in init_databases_config:
             core.log.warning(
                 f"No initialisation configuration has been set in <databases> entry for {bind=}"
             )
             continue
@@ -77,24 +81,20 @@
             if not cf_ini["key"] in bind_cf:
                 continue
 
             ini_dir = bind_cf[cf_ini["key"]]
             files = glob.glob(ini_dir + os.sep + cf_ini["pattern"])
 
             for file_path in files:
-                l_table_name = file_path.split(os.sep)[-1].split(".")[0].upper()
-                if tables is not None and len(tables) != 0:
-                    if not l_table_name in tables:
-                        continue
                 __process_databases_init(
-                    core, core.db, bind, l_table_name, file_path, file_type=ini_type
+                    core, bind, file_path, tables, file_type=ini_type
                 )
 
 
-def __process_databases_init(core, db, bind, table_name, file_path, file_type="py"):
+def __process_databases_init(core, bind, file_path, tables=None, file_type="py"):
     if file_type == "py":
         current_path = os.getcwd()
         module_path = (
             file_path.replace(current_path, "")
             .replace("/", ".")
             .replace("\\", ".")
             .replace(".py", "")
@@ -109,85 +109,64 @@
             ini = module.__dict__["ini"]
             if type(ini) != dict:
                 raise AlphaException(
                     "In file {file_path} <ini> configuration must be of type <dict>"
                     % (file_path)
                 )
             for real_table_name, conf in ini.items():
+                if tables is not None and not real_table_name.upper() in [
+                    x.upper() for x in tables
+                ]:
+                    continue
                 if type(real_table_name) != str and hasattr(
                     real_table_name, "__tablename__"
                 ):
                     real_table_name = getattr(real_table_name, "__tablename__")
-                if real_table_name.upper() == table_name.upper():
-                    __get_entries(core, db, bind, table_name, file_path, conf)
+                __get_entries(core, bind, real_table_name, file_path, conf)
     elif file_type == "json":
         try:
             ini = io_lib.read_json(file_path)
         except Exception as ex:
             raise AlphaException("Cannot read file %s: %s" % (file_path, ex))
-
-        __get_entries(core, db, bind, table_name, file_path, ini)
+        for table_name, conf in ini.items():
+            if tables is not None and not table_name.upper() in [
+                x.upper() for x in tables
+            ]:
+                continue
+            __get_entries(core, bind, table_name, file_path, conf)
     elif file_type == "sql":
         with open(file_path, "r") as f:
             sql = f.read()
             matchs = re.findall(r"to_date\('[^']+','[^']+'\)", sql)
             for match in matchs:
                 date = match.replace("to_date(", "").split(",")[0]
                 format = match.split(",")[1].replace(")", "")
                 sql = sql.replace(match, f"strftime({format}, {date})")
             statements = sql.split(";")
             for statement in statements:
                 try:
-                    db.execute(statement, bind=bind.upper())
+                    core.db.execute(statement, bind=bind.upper())
                 except Exception as ex:
-                    db.log.error(ex=ex)
-
-
-def __get_entries(core, db, bind, table_name, file_path, configuration):
-    # TODO: fix
-
-    if type(configuration) != dict:
-        core.log.error(
-            f"In file {file_path} configuration of {bind=} must be of type <dict>"
-        )
-        return
+                    core.db.log.error(f"Error with init of {file_path=}", ex=ex)
 
-    table = core.db.get_table_model(table_name)
-
-    object_initiated = "objects" in configuration
-    if object_initiated:
-        entries = configuration["objects"]
-        db.process_entries(bind, table, values=entries)
-        core.log.info(f"{table_name=} and {bind=} initiated with file {file_path}")
-
-    data_type = "alpha"
-    if "headers" in configuration and "values" in configuration:
-        values = configuration["values"]
-        headers = configuration["headers"]
-    elif (
-        "results" in configuration
-        and "columns" in configuration["results"][0]
-        and "items" in configuration["results"][0]
-    ):
-        values = configuration["results"][0]["items"]
-        headers = list(configuration["results"][0]["items"][0].keys())
-        data_type = "sql"
-    else:
-        if not object_initiated:
-            core.log.error(
-                f"Ini configuration in file {file_path} does not have a valid structure"
-            )
-        return
 
+def __process_headers_values(
+    file_path: str,
+    bind: str,
+    table_name: str,
+    table,
+    headers,
+    values,
+    data_type="alpha",
+):
     if type(values) != list:
         core.log.error(
             f'In file {file_path} "values" key from {table_name=} and {bind=} must be of type <list>'
         )
         return
-
     if type(headers) != list:
         core.log.error(
             f'In file {file_path} "headers" key from {table_name=} and {bind=} must be of type <list>'
         )
         return
 
     entries = []
@@ -198,22 +177,51 @@
             )
             continue
         elif type(entry) != dict and data_type == "sql":
             core.log.error(
                 f"In file {file_path} from {table_name=} and {bind=} entries must be of type <dict>"
             )
             continue
-        entries.append(entry if data_type == "alpha" else list(entry.values()))
+        if data_type == "sql":
+            entry = list(entry.values())
+            if len(entry) == 0:
+                continue
+        entries.append(entry)
 
         """if LOG:
             LOG.info(
                 "Adding %s entries from <list> for {table_name=} in {bind=} from file %s"
                 % (len(entries), table_name, database, file_path)
             )"""
-    db.process_entries(bind, table, headers=headers, values=entries)
+    if len(entries) != 0:
+        core.db.process_entries(bind, table, headers=headers, values=entries)
+
+
+def __get_entries(core, bind, table_name, file_path, configuration):
+    if type(configuration) != dict:
+        core.log.error(
+            f"In file {file_path} configuration of {bind=} must be of type <dict>"
+        )
+        return
+
+    table = core.db.get_table_model(table_name)
+
+    entries = configuration.get("objects", [])
+    if len(entries) != 0:
+        core.db.process_entries(bind, table, values=entries)
+        core.log.info(f"{table_name=} and {bind=} initiated with file {file_path}")
+
+    headers, values = configuration.get("headers", []), configuration.get("values", [])
+
+    __process_headers_values(file_path, bind, table_name, table, headers, values)
+
+    values = configuration.get("results", [{"items": [{}]}])[0]["items"]
+    headers = list(values[0].keys())
+    __process_headers_values(file_path, bind, table_name, table, headers, values, "sql")
+
     core.log.info(f"{table_name=} and {bind=} initiated with file {file_path}")
 
 
 def get_table_content(
     bind: str,
     tablename: str,
     order_by: str,
```

### Comparing `alphaz-0.7.3.9/alphaz/libs/date_lib.py` & `alphaz-0.7.4/alphaz/libs/date_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/dict_lib.py` & `alphaz-0.7.4/alphaz/libs/dict_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,19 +60,22 @@
     for k, v in d1.items():
         if k in d2 and type(d2) == dict:
             d2[k] = merge_dict(v, d2[k])
     d1.update(d2)
     return d1
 
 
-def show_dict(diff: dict, level: int = 0, outputs=None, show_none: bool = True):
+def show_dict(diff: dict | tuple, level: int = 0, outputs=None, show_none: bool = True):
     if diff is None:
         return
 
-    diff = dict(sorted(diff.items()))
+    if isinstance(diff, tuple):
+        diff = {"old": diff[0], "new": diff[1]}
+    else:
+        diff = dict(sorted(diff.items()))
 
     root = False
     if outputs is None:
         outputs, root = [], True
 
     for key, value in diff.items():
```

### Comparing `alphaz-0.7.3.9/alphaz/libs/emulation/vt102_lib.py` & `alphaz-0.7.4/alphaz/libs/emulation/vt102_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/events.py` & `alphaz-0.7.4/alphaz/libs/events.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/files_lib.py` & `alphaz-0.7.4/alphaz/libs/files_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/flask_lib.py` & `alphaz-0.7.4/alphaz/libs/flask_lib.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 DB = core.db
 
 
 class AlphaModelView(ModelView):
     column_display_pk = True
 
 
-def load_views(log) -> List[ModelView]:
+def load_views(binds: List[str], tables: List[str], log=None) -> List[ModelView]:
     """[Load view from tables definitions module]
 
     Args:
         module (ModuleType): [description]
 
     Returns:
         List[ModelView]: [description]
     """
     views = []
 
-    for model in DB.get_tables_models():
+    for model in DB.get_tables_models(binds=binds, tables=tables):
         table_name = model.__tablename__
         bind = model.__bind_key__
 
         attributes = [
             x for x, y in model.__dict__.items() if isinstance(y, InstrumentedAttribute)
         ]
 
@@ -41,10 +41,10 @@
             name=table_name,
             category=bind,
             endpoint=name,
         )
 
         view.column_list = attributes
         views.append(view)
-    if len(views) != 0:
+    if len(views) != 0 and log is not None:
         log.info(f"Loaded {len(views)} views models")
     return views
```

### Comparing `alphaz-0.7.3.9/alphaz/libs/img_lib.py` & `alphaz-0.7.4/alphaz/libs/img_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/io_lib.py` & `alphaz-0.7.4/alphaz/libs/io_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/json_lib.py` & `alphaz-0.7.4/alphaz/libs/json_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/logs_lib.py` & `alphaz-0.7.4/alphaz/libs/logs_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/mail_lib.py` & `alphaz-0.7.4/alphaz/libs/mail_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/notifications_lib.py` & `alphaz-0.7.4/alphaz/libs/notifications_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/number_lib.py` & `alphaz-0.7.4/alphaz/libs/number_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/process_lib.py` & `alphaz-0.7.4/alphaz/libs/process_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/py_lib.py` & `alphaz-0.7.4/alphaz/libs/py_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/scp_lib.py` & `alphaz-0.7.4/alphaz/libs/scp_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/search_lib.py` & `alphaz-0.7.4/alphaz/libs/search_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/secure_lib.py` & `alphaz-0.7.4/alphaz/libs/secure_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
     Returns:
         A string representing the encrypted message.
     """
     if isinstance(message, str):
         message = message.encode("utf-8")
     salt = secrets.token_bytes(16)
     key = _derive_key(password.encode(), salt, iterations)
-    f = Fernet(key)
+    f = Fernet(b64encode(key))
     token = f.encrypt(message)
     encoded_token = b64encode(token).decode("utf-8")
     return f"{salt.hex()}:{iterations}:{encoded_token}"
 
 
 """def password_decrypt(token: str | bytes, password: str) -> bytes:
     if type(token) == bytes:
```

### Comparing `alphaz-0.7.3.9/alphaz/libs/soap_lib.py` & `alphaz-0.7.4/alphaz/libs/soap_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/ssh_lib.py` & `alphaz-0.7.4/alphaz/libs/ssh_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/string_lib.py` & `alphaz-0.7.4/alphaz/libs/string_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/test_lib.py` & `alphaz-0.7.4/alphaz/libs/test_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/time_lib.py` & `alphaz-0.7.4/alphaz/libs/time_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/transactions_lib.py` & `alphaz-0.7.4/alphaz/libs/transactions_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/user_lib.py` & `alphaz-0.7.4/alphaz/libs/user_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/user_management/application_management_lib.py` & `alphaz-0.7.4/alphaz/libs/user_management/application_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/user_management/permission_management_lib.py` & `alphaz-0.7.4/alphaz/libs/user_management/permission_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/user_management/role_management_lib.py` & `alphaz-0.7.4/alphaz/libs/user_management/role_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/libs/user_management/user_management_lib.py` & `alphaz-0.7.4/alphaz/libs/user_management/user_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/mails/Images/Background.png` & `alphaz-0.7.4/alphaz/mails/Images/Background.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/mails/Images/Facebook_logo.png` & `alphaz-0.7.4/alphaz/mails/Images/Facebook_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/mails/Images/Twitter_logo.png` & `alphaz-0.7.4/alphaz/mails/Images/Twitter_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/mails/Images/Web_logo.png` & `alphaz-0.7.4/alphaz/mails/Images/Web_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/mails/Mail.png` & `alphaz-0.7.4/alphaz/mails/Mail.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/mails/Webmail.html` & `alphaz-0.7.4/alphaz/mails/Webmail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/mails/debug.html` & `alphaz-0.7.4/alphaz/mails/debug.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/mails/mail.html` & `alphaz-0.7.4/alphaz/mails/mail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/mails/password_reset.html` & `alphaz-0.7.4/alphaz/mails/password_reset.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/mails/stay_in_touch.html` & `alphaz-0.7.4/alphaz/mails/stay_in_touch.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/api/_answer.py` & `alphaz-0.7.4/alphaz/models/api/_answer.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,7 +25,13 @@
     status_description: str = ""
     requester: str = "unknow"
     data: dict = field(default_factory=lambda: {})
     pagination: ApiPagination = field(default_factory=lambda: {})
 
     def to_json(self):
         return self.get_fields_dict()
+
+    def set_error(self, description: str):
+        self.error = 1
+        self.status = "error"
+        self.status_code = 520
+        self.status_description = description
```

### Comparing `alphaz-0.7.3.9/alphaz/models/api/_colorations.py` & `alphaz-0.7.4/alphaz/models/api/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/api/_parameter.py` & `alphaz-0.7.4/alphaz/models/api/_parameter.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/api/_requests.py` & `alphaz-0.7.4/alphaz/models/api/_requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/api/_route.py` & `alphaz-0.7.4/alphaz/models/api/_route.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from ...models.main import AlphaException
 from ...models.api import ApiAnswer, AlphaRequest
 
 from ._parameter import Parameter
 from ..main._exception import get_message_from_name
 
 SEPARATOR = "__"
+DEBUG = False
 
 
 def get_columns_values_output(
     objects: list, columns: list = None, header: bool = False
 ) -> dict:
     """Generate columns names output columns names + list of list (only the values) + nb of values if not header
     ex : { "columns":["col1","col2",...], "values": ["value1","value2",..], "values_nb":12}
@@ -447,15 +448,16 @@
                 data = data[0]
 
         if not check_format(data):
             tic = time.perf_counter()
             data = json_lib.jsonify_data(data)
             toc = time.perf_counter()
             elapsed_time = toc - tic
-            print(f"Elapsed time: {elapsed_time:0.4f} seconds for jsonify_data")
+            if DEBUG:
+                print(f"Elapsed time: {elapsed_time:0.4f} seconds for jsonify_data")
 
         if "table" in format_:
             data = get_columns_values_output(
                 data, self.get("columns"), header="header" in format_
             )
 
         self.returned.data = data
@@ -485,15 +487,16 @@
             route_output = jsonify(data)
         else:
             # returned = jsonify(self.returned)
             route_output = self.returned.to_json()
 
         toc = time.perf_counter()
         elapsed_time = toc - tic
-        print(f"Elapsed time: {elapsed_time:0.4f} seconds for conversion")
+        if DEBUG:
+            print(f"Elapsed time: {elapsed_time:0.4f} seconds for conversion")
 
         if "txt" in format_:
             headers["Content-Type"] = "text/txt; charset=utf-8"
         elif "xml" in format_:
             headers["Content-Type"] = "text/xml; charset=utf-8"
 
         headers_content = {
@@ -512,15 +515,16 @@
         # headers["Access-Control-Allow-Headers"] = "*" # ",".join(headers_content.keys())
 
         # returned = Response(returned, status=returned["status_code"])
         tic = time.perf_counter()
         returned = make_response(route_output, status_code)
         toc = time.perf_counter()
         elapsed_time = toc - tic
-        print(f"Elapsed time: {elapsed_time:0.4f} seconds for returned")
+        if DEBUG:
+            print(f"Elapsed time: {elapsed_time:0.4f} seconds for returned")
 
         if "pagination" in format_ and is_pagination:
             headers["X-pagination"] = {
                 "total": total,
                 "total_pages": total_pages,
                 "page": page,
                 "previous_page": page - 1 if page > 0 else 0,
```

### Comparing `alphaz-0.7.3.9/alphaz/models/api/_structures.py` & `alphaz-0.7.4/alphaz/models/api/_structures.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/api/_utils.py` & `alphaz-0.7.4/alphaz/models/api/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/config/_config.py` & `alphaz-0.7.4/alphaz/models/config/_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/config/_utils.py` & `alphaz-0.7.4/alphaz/models/config/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/database/main_definitions.py` & `alphaz-0.7.4/alphaz/models/database/main_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/database/models.py` & `alphaz-0.7.4/alphaz/models/database/models.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/database/operators.py` & `alphaz-0.7.4/alphaz/models/database/operators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/database/requests.py` & `alphaz-0.7.4/alphaz/models/database/requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/database/row.py` & `alphaz-0.7.4/alphaz/models/database/row.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/database/structure.py` & `alphaz-0.7.4/alphaz/models/database/structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -259,15 +259,14 @@
                     pass  # TODO: do something ?
                 elif type(to_join) == RelationshipProperty:
                     pass  # TODO: do something ?
     return query
 
 
 class RetryingQuery(BaseQuery):
-
     __retry_count__ = 3
     __retry_sleep_interval_sec__ = 0.5
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def __iter__(self):
@@ -466,15 +465,14 @@
         query=None,
         filters=None,
         optional_filters=None,
         columns=None,
         likes=None,
         sup=None,
     ):
-
         if query is None:
             query = model.query
 
         if columns is not None:
             if type(columns) != list and type(columns) != List:
                 columns = [columns]
             ccs = []
@@ -584,14 +582,17 @@
         query,
         values=None,
         unique=False,
         log=None,
         bind=None,
         close=False,
         dataclass=None,
+        page:int=None,
+        per_page:int=None,
+        full_count_query:str=None
     ):
         session = self.get_engine(self.app, bind)
 
         if self.db_type == "sqlite":
             query = query.replace("%s", "?")
 
         if log is None:
@@ -605,14 +606,23 @@
                         query = query.replace(":%s" % list(val.keys())[0], f":p{i}", 1)
                         dict_values[f"p{i}"] = list(val.values())[0]
                     else:
                         query = query.replace("?", f":p{i}", 1)
                         dict_values[f"p{i}"] = val
                 values = dict_values
 
+        if per_page is not None:
+            page = 0 if page is None else page
+            query += f"LIMIT {per_page} OFFSET {page*per_page}"
+        if query.strip()[-1] != ";":
+            query += ";"
+        if full_count_query is not None:
+            total = self.get_query_results(full_count_query)
+            self.full_count = list(total[0].values())[0]
+
         try:
             resultproxy = (
                 session.execute(query, values)
                 if values is not None
                 else session.execute(query)
             )
         except Exception as ex:
@@ -883,31 +893,33 @@
                 self.get_tables_models(
                     tables=[table], binds=[bind] if bind is not None else None
                 )
             ),
             None,
         )
         if table is None:
-            raise AlphaException("cannot_find_table", parameters={"table": table})
+            raise AlphaException(f"Cannot find table {table} in databases models")
         return table
 
     def get_table_columns(self, table: str):
         model = self.get_table_model(table)
         return model._sa_class_manager.local_attrs
 
     def get_tables_models(
         self, tables: List[str] = None, binds: List[str] = None
     ) -> list:
         if tables is not None:
             tables = [x.upper() for x in tables]
+        if binds is not None:
+            binds = [x.upper() for x in binds]
         models = self.__get_tables_models()
         registered_models = [
             x
             for x in models
-            if (binds is None or getattr(x, "__bind_key__", None) in binds)
+            if (binds is None or getattr(x, "__bind_key__", "MAIN").upper() in binds)
             and (tables is None or x.__tablename__.upper() in tables)
         ]
         return registered_models
 
     def __get_tables_models(self, force: bool = False):
         if len(self.models) == 0 or force:
             if hasattr(self.Model, "_decl_class_registry"):
@@ -1021,17 +1033,17 @@
             #! TOTO: modify
             """if disabled_relationships:
                 if (column_property or isinstance(col.prop, RelationshipProperty)) and not binary_expression and key not in disabled_relationships:
                     attributes[key] = col"""
 
         if len(attributes) != 0:
             columns = (
-                attributes.values()
+                list(attributes.values())
                 if columns is None
-                else columns.extend(attributes.values())
+                else columns.extend(list(attributes.values()))
             )
 
         if unique and (
             type(unique) == InstrumentedAttribute or type(unique) == str
         ):  # TODO: upgrade
             columns = [unique]
             distinct = True
@@ -1460,47 +1472,57 @@
             headers = [
                 x.lower().replace(" ", "_")
                 if hasattr(x, "lower")
                 else str(x).split(".")[1]
                 for x in headers
             ]
 
-            columns_names = {}
-            for name, col in table.__dict__.items():
-                if hasattr(col, "expression") and hasattr(col.expression, "name"):
-                    columns_names[col.expression.name] = name
+            columns_names, model_names = {}, []
 
+            for key, el in table.__dict__.items():
+                if hasattr(el,"key") and hasattr(el, "expression") and hasattr(el.expression,"key"):
+                    columns_names[el.expression.key] = key
+                    
+            for header in headers:
+                if header in columns_names:
+                    model_names.append(columns_names[header])
+                elif header in list(columns_names.values()):
+                    model_names.append(header)
+                else:
+                    print(f"Failed to identified {header=}")
+                    return
             entries = [
                 table(
                     **{
-                        columns_names[headers[i]]: convert_value(value)
+                        model_names[i]: convert_value(value)
                         for i, value in enumerate(values_list)
-                        if headers[i] in columns_names
                     }
                 )
                 for values_list in values
             ]
         else:
             entries = values
 
+        self.add_or_update(entries)
         # db.session.query(class_instance).delete()
         # db.session.add_all(entries)
-        session = self.create_scoped_session(options={"bind": bind})
+        """session = self.create_scoped_session(options={"bind": bind})
 
         for entry in entries:
             session.merge(entry)
-        session.commit()
+        session.commit()"""
 
     def init_all(
         self,
         binds: List[str] = None,
         tables: List[AlphaTable] = None,
         drop: bool = False,
         create: bool = False,
         sqlite: bool = True,
+        log=None,
     ):
         """if sqlite:
         binds = [
             x.upper()
             for x, y in self.db_cnx.items()
             if y["type"] == "sqlite" and (binds is None or x in binds)
         ]"""
@@ -1519,25 +1541,35 @@
         tables_by_bind = {}
         for table_model in tables:
             bind = (
                 "MAIN"
                 if not hasattr(table_model, "__bind_key__")
                 else table_model.__bind_key__
             )
+            if binds is not None:
+                if not bind.lower() in [x.lower() for x in binds]:
+                    continue
             if not bind in tables_by_bind:
                 tables_by_bind[bind] = [table_model]
             else:
                 tables_by_bind[bind].append(table_model)
 
         for bind, tables_models in tables_by_bind.items():
             tables = [x.__table__ for x in tables_models]
             meta = MetaData(self.get_engine(bind=bind))
+            table_names = [x.__tablename__ for x in tables_models]
+            tables_names_str = ";".join(table_names)
             if drop:
+                if log is not None:
+                    log.info(f"Drop tables from bind {bind}: {tables_names_str}")
                 meta.drop_all(tables=tables)
-            meta.create_all(tables=tables)
+            if create:
+                if log is not None:
+                    log.info(f"Create tables from bind {bind}: {tables_names_str}")
+                meta.create_all(tables=tables)
 
     def create_table(self, table: str, bind: str = None, drop: bool = False):
         table_object = self.get_table_model(table, bind)
         if drop:
             try:
                 table_object.__table__.drop(self.engine)
             except:
```

### Comparing `alphaz-0.7.3.9/alphaz/models/database/tests.py` & `alphaz-0.7.4/alphaz/models/database/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/database/users_definitions.py` & `alphaz-0.7.4/alphaz/models/database/users_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/database/utils.py` & `alphaz-0.7.4/alphaz/models/database/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/database/views.py` & `alphaz-0.7.4/alphaz/models/database/views.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/excel.py` & `alphaz-0.7.4/alphaz/models/excel.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/ftp.py` & `alphaz-0.7.4/alphaz/models/ftp.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/json/_converters.py` & `alphaz-0.7.4/alphaz/models/json/_converters.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/logger/_colorations.py` & `alphaz-0.7.4/alphaz/models/logger/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/logger/_logger.py` & `alphaz-0.7.4/alphaz/models/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/logger/_utils.py` & `alphaz-0.7.4/alphaz/models/logger/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/logs/main.log` & `alphaz-0.7.4/alphaz/models/logs/main.log`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/main/_base.py` & `alphaz-0.7.4/alphaz/models/main/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,15 +511,17 @@
             dct[f.name] = value
 
         return dct
 
     def compare(
         self, other, attrs_list: List[str], attrs_eq: Dict[str, str] = None
     ) -> bool:
-        if not isinstance(other, self.__class__):
+        if not isinstance(other, self.__class__) and not issubclass(
+            self.__class__, other.__class__
+        ):
             raise AlphaException(
                 description=f"Cannot compare {self.__class__} object with {other.__class__} object"
             )
 
         [attrs_list.append(attr) for attr in (attrs_eq if attrs_eq is not None else [])]
 
         compared = []
@@ -634,15 +636,18 @@
         for key, fd in instance.__dict__.items():
             if fd is not None:
                 setattr(self, key, fd)
 
     def flatten(self, parent: str = None):
         output = {}
         for key, field in self.__dataclass_fields__.items():
-            value = self.__dict__[key]
+            if not key in self.__dict__:
+                value = field.default
+            else:
+                value = self.__dict__[key]
             value_key = f"{parent}.{key}" if parent is not None else key
 
             if value is None:
                 output[value_key] = None
             elif isinstance(value, AlphaDataclass):
                 for k, v in value.flatten(parent=key).items():
                     output[k] = v
```

### Comparing `alphaz-0.7.3.9/alphaz/models/main/_core/_core.py` & `alphaz-0.7.4/alphaz/models/main/_core/_core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/main/_exception.py` & `alphaz-0.7.4/alphaz/models/main/_exception.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/main/_request.py` & `alphaz-0.7.4/alphaz/models/main/_request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/main/_singleton.py` & `alphaz-0.7.4/alphaz/models/main/_singleton.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/request.py` & `alphaz-0.7.4/alphaz/models/request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/tests/_category.py` & `alphaz-0.7.4/alphaz/models/tests/_category.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/tests/_group.py` & `alphaz-0.7.4/alphaz/models/tests/_group.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/tests/_method.py` & `alphaz-0.7.4/alphaz/models/tests/_method.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/tests/_save.py` & `alphaz-0.7.4/alphaz/models/tests/_save.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/tests/_test.py` & `alphaz-0.7.4/alphaz/models/tests/_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,22 +41,24 @@
     def init_tables(
         self,
         tables: List[str],
         binds: List[str] = None,
         truncate: bool = False,
         drop: bool = False,
         create: bool = False,
+        init: bool = True,
     ):
         database_lib.init_databases(
             core=core,
             binds=binds,
             tables=tables,
             truncate=truncate,
             drop=drop,
             create=create,
+            init=init,
         )
 
     def test(self, name, coverage: bool = False):
         self.output = None
         self.partial_output = None
 
         status = False
```

### Comparing `alphaz-0.7.3.9/alphaz/models/tests/_wrappers.py` & `alphaz-0.7.4/alphaz/models/tests/_wrappers.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from ..main import AlphaException
 from ...models.tests import AlphaTest
 from ...libs import dict_lib
 
 from ._levels import Levels
 from ._save import AlphaSave
 
+from core import core
+
+LOG = core.get_logger("tests")
+
 TEST_METHOD_NAME = "test_alpha_in"
 
 
 def call_function(
     fct: Callable, obj: object, args: List = None, kwargs: Dict[str, object] = None
 ) -> Any:
     """
@@ -99,41 +103,48 @@
                 )
                 if logged_output is None:
                     raise AlphaException("Unable to auth as an admin")
 
             if begin:
                 call_function(begin, TestClass, begin_args, begin_kwargs)
 
-            output = func(*args, **kwargs)
+            try:
+                output = func(*args, **kwargs)
 
-            if save:
-                alpha_save = AlphaSave(root=save_path, ext=save_ext)
-                return_save = alpha_save.load(
-                    filename=func.__name__,
-                    class_name=TestClass.__class__.__name__,
-                )
-
-                alpha_save.save(
-                    object_to_save=output,
-                    filename=func.__name__,
-                    class_name=TestClass.__class__.__name__,
-                )
+                if save:
+                    alpha_save = AlphaSave(root=save_path, ext=save_ext)
+                    return_save = alpha_save.load(
+                        filename=func.__name__,
+                        class_name=TestClass.__class__.__name__,
+                    )
 
-                return_save = (
-                    save_post_process(output, return_save)
-                    if save_post_process is not None
-                    else return_save
-                )
+                    alpha_save.save(
+                        object_to_save=output,
+                        filename=func.__name__,
+                        class_name=TestClass.__class__.__name__,
+                    )
 
-                if return_diff:
-                    TestClass.outputs["dicts_diff"] = dict_lib.get_dicts_diff(
-                        dict_1=output, dict_2=return_save
+                    return_save = (
+                        save_post_process(output, return_save)
+                        if save_post_process is not None
+                        else return_save
                     )
-                    
-                TestClass.assert_equal(return_save, output)
+
+                    if return_diff:
+                        TestClass.outputs["dicts_diff"] = dict_lib.get_dicts_diff(
+                            dict_1=output, dict_2=return_save
+                        )
+
+                    TestClass.assert_equal(return_save, output)
+            except Exception as ex:
+                TestClass.output = False
+                LOG.error(
+                    message=f"An exception occurred with {TestClass.__class__.__name__}.{func.__name__}. The test has been marked as failed.",
+                    ex=ex,
+                )
 
             if end:
                 call_function(end, TestClass, end_args, end_kwargs)
 
             if logged_output is not None:
                 logout_su()
```

### Comparing `alphaz-0.7.3.9/alphaz/models/user.py` & `alphaz-0.7.4/alphaz/models/user.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/models/watcher.py` & `alphaz-0.7.4/alphaz/models/watcher.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/pocs/main.py` & `alphaz-0.7.4/alphaz/pocs/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/run.py` & `alphaz-0.7.4/alphaz/run.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/src/alpha.png` & `alphaz-0.7.4/alphaz/src/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/src/configs/loggers.json` & `alphaz-0.7.4/alphaz/src/configs/loggers.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/stitch/Core.py` & `alphaz-0.7.4/alphaz/stitch/Core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/stitch/stitch.py` & `alphaz-0.7.4/alphaz/stitch/stitch.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/stitch/web-drivers/chromedriver.exe` & `alphaz-0.7.4/alphaz/stitch/web-drivers/chromedriver.exe`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/stitch/web-drivers/geckodriver` & `alphaz-0.7.4/alphaz/stitch/web-drivers/geckodriver`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/assets/css/home.css` & `alphaz-0.7.4/alphaz/templates/assets/css/home.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/assets/css/logs.css` & `alphaz-0.7.4/alphaz/templates/assets/css/logs.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/assets/images/icons/alpha.png` & `alphaz-0.7.4/alphaz/templates/assets/images/icons/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/assets/images/icons/start-icon.png` & `alphaz-0.7.4/alphaz/templates/assets/images/icons/start-icon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/assets/images/icons/wsalpha.png` & `alphaz-0.7.4/alphaz/templates/assets/images/icons/wsalpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/assets/images/loading.gif` & `alphaz-0.7.4/alphaz/templates/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/assets/js/libs/ansi_up.js` & `alphaz-0.7.4/alphaz/templates/assets/js/libs/ansi_up.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/assets/js/libs/jquery.min.js` & `alphaz-0.7.4/alphaz/templates/assets/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/assets/js/logs.js` & `alphaz-0.7.4/alphaz/templates/assets/js/logs.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/home.html` & `alphaz-0.7.4/alphaz/templates/home.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/templates/logs.html` & `alphaz-0.7.4/alphaz/templates/logs.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/test.py` & `alphaz-0.7.4/alphaz/test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/tests/api.py` & `alphaz-0.7.4/alphaz/tests/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/tests/basic_test.py` & `alphaz-0.7.4/alphaz/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/tests/configurations.py` & `alphaz-0.7.4/alphaz/tests/configurations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/tests/database.py` & `alphaz-0.7.4/alphaz/tests/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/tests/utils.py` & `alphaz-0.7.4/alphaz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/api.py` & `alphaz-0.7.4/alphaz/utils/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/configuration.py` & `alphaz-0.7.4/alphaz/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/database_to_dataclass.py` & `alphaz-0.7.4/alphaz/utils/database_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/decorators.py` & `alphaz-0.7.4/alphaz/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/ensure.py` & `alphaz-0.7.4/alphaz/utils/ensure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/mep.py` & `alphaz-0.7.4/alphaz/utils/mep.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/screens.py` & `alphaz-0.7.4/alphaz/utils/screens.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/selectionMenu.py` & `alphaz-0.7.4/alphaz/utils/selectionMenu.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/tasks.py` & `alphaz-0.7.4/alphaz/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/tests.py` & `alphaz-0.7.4/alphaz/utils/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/time.py` & `alphaz-0.7.4/alphaz/utils/time.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz/utils/transactions.py` & `alphaz-0.7.4/alphaz/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.9/alphaz.egg-info/PKG-INFO` & `alphaz-0.7.4/alphaz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.3.9
+Version: 0.7.4
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.3.9.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.4.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.3.9/alphaz.egg-info/SOURCES.txt` & `alphaz-0.7.4/alphaz.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+alphaz/README.md
 alphaz/__init__.py
 alphaz/alphaz.bat
 alphaz/alphaz.code-workspace
 alphaz/alphaz.sh
 alphaz/api.bat
 alphaz/api.json
 alphaz/api.py
@@ -51,32 +52,55 @@
 alphaz/config/config.css
 alphaz/config/config.html
 alphaz/config/main_configuration.py
 alphaz/config/page.py
 alphaz/config/source.html
 alphaz/documentations/mkdocs.yml
 alphaz/documentations/docs/alpha_admin.md
-alphaz/documentations/docs/alpha_api.md
 alphaz/documentations/docs/alpha_core.md
-alphaz/documentations/docs/alpha_database.md
 alphaz/documentations/docs/alpha_screens.md
 alphaz/documentations/docs/alpha_setup.md
+alphaz/documentations/docs/api_database.md
 alphaz/documentations/docs/configuration.md
 alphaz/documentations/docs/documentation.md
 alphaz/documentations/docs/index.md
+alphaz/documentations/docs/api/authorizations.md
+alphaz/documentations/docs/api/cache.md
+alphaz/documentations/docs/api/configuration.md
+alphaz/documentations/docs/api/issues.md
+alphaz/documentations/docs/api/main.md
+alphaz/documentations/docs/api/methods.md
+alphaz/documentations/docs/api/parameters.md
+alphaz/documentations/docs/api/routes.md
+alphaz/documentations/docs/api/sqlalchemy.md
+alphaz/documentations/docs/database/init.md
+alphaz/documentations/docs/database/instantiate.md
+alphaz/documentations/docs/database/main.md
+alphaz/documentations/docs/database/model.md
+alphaz/documentations/docs/database/relations.md
+alphaz/documentations/docs/database/schema.md
+alphaz/documentations/docs/database/update.md
 alphaz/documentations/site/404.html
 alphaz/documentations/site/index.html
 alphaz/documentations/site/sitemap.xml
 alphaz/documentations/site/sitemap.xml.gz
 alphaz/documentations/site/alpha_admin/index.html
-alphaz/documentations/site/alpha_api/index.html
 alphaz/documentations/site/alpha_core/index.html
-alphaz/documentations/site/alpha_database/index.html
 alphaz/documentations/site/alpha_screens/index.html
 alphaz/documentations/site/alpha_setup/index.html
+alphaz/documentations/site/api/authorizations/index.html
+alphaz/documentations/site/api/cache/index.html
+alphaz/documentations/site/api/configuration/index.html
+alphaz/documentations/site/api/issues/index.html
+alphaz/documentations/site/api/main/index.html
+alphaz/documentations/site/api/methods/index.html
+alphaz/documentations/site/api/parameters/index.html
+alphaz/documentations/site/api/routes/index.html
+alphaz/documentations/site/api/sqlalchemy/index.html
+alphaz/documentations/site/api_database/index.html
 alphaz/documentations/site/assets/images/favicon.png
 alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
 alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
 alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
 alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
 alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
 alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
@@ -101,14 +125,21 @@
 alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
 alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
 alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
 alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
 alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
 alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
 alphaz/documentations/site/configuration/index.html
+alphaz/documentations/site/database/init/index.html
+alphaz/documentations/site/database/instantiate/index.html
+alphaz/documentations/site/database/main/index.html
+alphaz/documentations/site/database/model/index.html
+alphaz/documentations/site/database/relations/index.html
+alphaz/documentations/site/database/schema/index.html
+alphaz/documentations/site/database/update/index.html
 alphaz/documentations/site/documentation/index.html
 alphaz/documentations/site/search/search_index.json
 alphaz/libs/__init__.py
 alphaz/libs/api_lib.py
 alphaz/libs/barcode_lib.py
 alphaz/libs/config_lib.py
 alphaz/libs/converter_lib.py
```

### Comparing `alphaz-0.7.3.9/setup.py` & `alphaz-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, glob, re
 from datetime import date
 
 today = date.today()
 
 from setuptools import setup, find_packages
 
-version = "0.7.3.9"
+version = "0.7.4"
 
 excludes = [".git", ".vscode"]
 
 archives = glob.glob("dist/*")
 for archive in archives:
     os.remove(archive)
 
@@ -93,14 +93,15 @@
     "concurrent_log_handler",
     "flask_cors",
     "bandit",
     "black",
     "unidecode",
     "importlib_metadata",
     "vt102",
+    "dictdiffer",
 ]
 
 setup(
     name="alphaz",
     packages=[x.replace(os.sep, ".") for x in subfolders],
     include_package_data=True,
     version=version,
```

