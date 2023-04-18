# Comparing `tmp/alphaz-0.7.3.8.tar.gz` & `tmp/alphaz-0.7.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alphaz-0.7.3.8.tar", last modified: Tue Apr 11 14:15:59 2023, max compression
+gzip compressed data, was "dist/alphaz-0.7.3.9.tar", last modified: Wed Apr 12 11:28:54 2023, max compression
```

## Comparing `alphaz-0.7.3.8.tar` & `alphaz-0.7.3.9.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.933067 alphaz-0.7.3.8/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8469 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/MANIFEST.in
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-11 14:15:59.933067 alphaz-0.7.3.8/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.3.8/README.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.877067 alphaz-0.7.3.8/alphaz/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      320 2023-03-23 07:52:23.000000 alphaz-0.7.3.8/alphaz/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/alphaz.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/alphaz.code-workspace
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/alphaz.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/api.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      662 2021-09-15 19:20:13.000000 alphaz-0.7.3.8/alphaz/api.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.3.8/alphaz/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/apis/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/apis/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/apis/log.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.3.8/alphaz/apis/mails.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/apis/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/apis/routes/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/apis/routes/admin.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/apis/routes/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/apis/routes/basic_tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2902 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/apis/routes/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.3.8/alphaz/apis/routes/git.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.3.8/alphaz/apis/routes/logs.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.3.8/alphaz/apis/routes/mails.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6262 2023-03-17 07:21:40.000000 alphaz-0.7.3.8/alphaz/apis/routes/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1330 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/apis/routes/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/apis/routes/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.3.8/alphaz/apis/routes/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.3.8/alphaz/apis/routes/user_management/application_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.3.8/alphaz/apis/routes/user_management/permission_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.3.8/alphaz/apis/routes/user_management/role_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.3.8/alphaz/apis/routes/user_management/user_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3025 2023-03-17 18:14:36.000000 alphaz-0.7.3.8/alphaz/apis/routes/users.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/apis/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/apis/users/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/apis/users/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.3.8/alphaz/apis/users/ldap.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.3.8/alphaz/apis/users/users.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config/config.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config/config.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.3.8/alphaz/config/main_configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config/page.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config/source.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.3.8/alphaz/core.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.881067 alphaz-0.7.3.8/alphaz/documentations/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/docs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_admin.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8923 2022-08-31 08:56:44.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_api.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1284 2022-07-19 09:10:48.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_core.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5602 2022-07-19 09:10:48.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_database.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_screens.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2215 2022-05-18 14:56:19.000000 alphaz-0.7.3.8/alphaz/documentations/docs/alpha_setup.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.3.8/alphaz/documentations/docs/configuration.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.3.8/alphaz/documentations/docs/documentation.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3505 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/documentations/docs/index.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      440 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/documentations/mkdocs.yml
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9286 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/404.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_admin/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10320 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_admin/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    47925 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_api/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18127 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_core/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    43708 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_database/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_screens/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17969 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_screens/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/alpha_setup/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20160 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/alpha_setup/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.873067 alphaz-0.7.3.8/alphaz/documentations/site/assets/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/assets/images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/images/favicon.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.885067 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.889067 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.889067 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/workers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.893067 alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.893067 alphaz-0.7.3.8/alphaz/documentations/site/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24568 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.893067 alphaz-0.7.3.8/alphaz/documentations/site/documentation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13157 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/documentation/index.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25592 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.893067 alphaz-0.7.3.8/alphaz/documentations/site/search/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    52508 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz/documentations/site/search/search_index.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1081 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/sitemap.xml
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      200 2023-04-11 14:15:58.000000 alphaz-0.7.3.8/alphaz/documentations/site/sitemap.xml.gz
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/git.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.3.8/alphaz/help.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.897067 alphaz-0.7.3.8/alphaz/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5786 2023-03-24 12:18:56.000000 alphaz-0.7.3.8/alphaz/libs/api_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/barcode_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13997 2023-03-24 12:18:56.000000 alphaz-0.7.3.8/alphaz/libs/config_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.3.8/alphaz/libs/converter_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9014 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/libs/database_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.3.8/alphaz/libs/date_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6222 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/libs/dict_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.897067 alphaz-0.7.3.8/alphaz/libs/emulation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.3.8/alphaz/libs/emulation/vt102_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/events.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/libs/files_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1096 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/libs/flask_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/ftp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/libs/img_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/libs/io_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.3.8/alphaz/libs/json_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.3.8/alphaz/libs/logs_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.3.8/alphaz/libs/mail_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/nav_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.3.8/alphaz/libs/notifications_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/number_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/os_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/process_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/libs/py_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      657 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/scp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/libs/search_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6386 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/libs/secure_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.3.8/alphaz/libs/soap_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/libs/sql_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18289 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/libs/ssh_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11021 2023-04-08 08:30:59.000000 alphaz-0.7.3.8/alphaz/libs/string_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5139 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/libs/test_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/libs/time_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.3.8/alphaz/libs/transactions_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5041 2022-12-01 15:14:08.000000 alphaz-0.7.3.8/alphaz/libs/user_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.897067 alphaz-0.7.3.8/alphaz/libs/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.3.8/alphaz/libs/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.3.8/alphaz/libs/user_management/application_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.3.8/alphaz/libs/user_management/permission_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.3.8/alphaz/libs/user_management/role_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.3.8/alphaz/libs/user_management/user_management_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.901067 alphaz-0.7.3.8/alphaz/mails/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.901067 alphaz-0.7.3.8/alphaz/mails/Images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/Images/Background.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/Images/Facebook_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/Images/Twitter_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/Images/Web_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/mails/Images/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/Mail.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.3.8/alphaz/mails/Webmail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/mails/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.3.8/alphaz/mails/debug.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.3.8/alphaz/mails/mail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/password_reset.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.3.8/alphaz/mails/stay_in_touch.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/mails/template.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.901067 alphaz-0.7.3.8/alphaz/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.3.8/alphaz/models/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.3.8/alphaz/models/api/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      710 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/api/_answer.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.3.8/alphaz/models/api/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.3.8/alphaz/models/api/_methods.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14253 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/api/_parameter.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.3.8/alphaz/models/api/_requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18565 2023-03-29 19:05:00.000000 alphaz-0.7.3.8/alphaz/models/api/_route.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21563 2023-03-23 07:52:23.000000 alphaz-0.7.3.8/alphaz/models/api/_structures.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.3.8/alphaz/models/api/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.3.8/alphaz/models/base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25438 2023-01-06 09:14:28.000000 alphaz-0.7.3.8/alphaz/models/config/_config.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12129 2021-08-12 12:49:09.000000 alphaz-0.7.3.8/alphaz/models/config/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.3.8/alphaz/models/database/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.3.8/alphaz/models/database/main_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.3.8/alphaz/models/database/models.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.3.8/alphaz/models/database/operators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.3.8/alphaz/models/database/requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/database/row.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    53758 2023-03-16 19:44:05.000000 alphaz-0.7.3.8/alphaz/models/database/structure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/database/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4418 2023-03-16 19:51:01.000000 alphaz-0.7.3.8/alphaz/models/database/users_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.3.8/alphaz/models/database/utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.3.8/alphaz/models/database/views.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/excel.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5126 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/models/ftp.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.3.8/alphaz/models/img.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/json/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/json/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.3.8/alphaz/models/json/_converters.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/logger/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.3.8/alphaz/models/logger/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.3.8/alphaz/models/logger/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14091 2023-04-05 11:16:09.000000 alphaz-0.7.3.8/alphaz/models/logger/_logger.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/logger/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.905067 alphaz-0.7.3.8/alphaz/models/logs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.3.8/alphaz/models/logs/main.log
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.3.8/alphaz/models/logs/main.log.2021-11-07
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/models/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.3.8/alphaz/models/main/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    26166 2023-04-07 09:47:18.000000 alphaz-0.7.3.8/alphaz/models/main/_base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/models/main/_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_core/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14630 2023-04-08 19:36:08.000000 alphaz-0.7.3.8/alphaz/models/main/_core/_core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_core/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.3.8/alphaz/models/main/_enum.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1862 2023-02-17 08:49:35.000000 alphaz-0.7.3.8/alphaz/models/main/_exception.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_file.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_process.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_request.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/main/_singleton.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/models/request.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/models/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/models/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6780 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/tests/_category.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3095 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/tests/_group.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      109 2021-09-10 07:16:32.000000 alphaz-0.7.3.8/alphaz/models/tests/_levels.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4174 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/models/tests/_method.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4571 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/models/tests/_save.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13445 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/models/tests/_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6927 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/models/tests/_wrappers.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.3.8/alphaz/models/user.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/models/watcher.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/pocs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/pocs/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/reload_gitignore.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.3.8/alphaz/req.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.3.8/alphaz/requirements.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/run.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/src/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/src/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/src/alpha.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/src/configs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/src/configs/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.3.8/alphaz/src/configs/loggers.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.3.8/alphaz/src/configs/loggers_colors.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/src/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/src/database/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/stitch/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/Core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/stitch/imports/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/imports/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.909067 alphaz-0.7.3.8/alphaz/stitch/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/stitch/models/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/models/element.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/run.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/stitch.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.921067 alphaz-0.7.3.8/alphaz/stitch/web-drivers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/web-drivers/chromedriver.exe
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/stitch/web-drivers/geckodriver
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.873067 alphaz-0.7.3.8/alphaz/stitch/websites/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/stitch/websites/Test/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/stitch/websites/Test/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/stitch/websites/stiki/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.3.8/alphaz/stitch/websites/stiki/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/templates/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.8/alphaz/templates/assets/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/css/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.3.8/alphaz/templates/assets/css/home.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/css/logs.css
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/images/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/admin.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/alpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/save.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/start-icon.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/user.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/icons/wsalpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/images/loading.gif
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/js/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.929067 alphaz-0.7.3.8/alphaz/templates/assets/js/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/js/libs/ansi_up.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/assets/js/libs/jquery.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.3.8/alphaz/templates/assets/js/logs.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/templates/hello.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/templates/home.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.3.8/alphaz/templates/logs.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.3.8/alphaz/test.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.933067 alphaz-0.7.3.8/alphaz/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13857 2023-03-28 08:47:21.000000 alphaz-0.7.3.8/alphaz/tests/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/tests/basic_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.3.8/alphaz/tests/configurations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22695 2023-03-16 19:44:05.000000 alphaz-0.7.3.8/alphaz/tests/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/tests/processes.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/tests/utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.933067 alphaz-0.7.3.8/alphaz/utils/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/utils/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11552 2023-02-16 14:12:47.000000 alphaz-0.7.3.8/alphaz/utils/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.3.8/alphaz/utils/clean.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.3.8/alphaz/utils/configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.3.8/alphaz/utils/database_to_dataclass.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/utils/decorators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.3.8/alphaz/utils/ensure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.3.8/alphaz/utils/mep.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.3.8/alphaz/utils/screens.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/utils/selectionMenu.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/utils/tasks.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1535 2023-02-23 09:08:35.000000 alphaz-0.7.3.8/alphaz/utils/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.3.8/alphaz/utils/time.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.3.8/alphaz/utils/transactions.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-11 14:15:59.877067 alphaz-0.7.3.8/alphaz.egg-info/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz.egg-info/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9706 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz.egg-info/SOURCES.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz.egg-info/dependency_links.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      447 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz.egg-info/requires.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-11 14:15:59.000000 alphaz-0.7.3.8/alphaz.egg-info/top_level.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-11 14:15:59.933067 alphaz-0.7.3.8/setup.cfg
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3075 2023-04-11 14:15:53.000000 alphaz-0.7.3.8/setup.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8469 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/MANIFEST.in
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.3.9/README.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.729881 alphaz-0.7.3.9/alphaz/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      320 2023-03-23 07:52:23.000000 alphaz-0.7.3.9/alphaz/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/alphaz.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/alphaz.code-workspace
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/alphaz.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/api.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      662 2021-09-15 19:20:13.000000 alphaz-0.7.3.9/alphaz/api.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2022-04-13 09:59:51.000000 alphaz-0.7.3.9/alphaz/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.729881 alphaz-0.7.3.9/alphaz/apis/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/apis/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/apis/log.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-03-17 07:06:42.000000 alphaz-0.7.3.9/alphaz/apis/mails.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/apis/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/apis/routes/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1577 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/apis/routes/admin.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1137 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/apis/routes/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3062 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/apis/routes/basic_tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2902 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/apis/routes/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2022-04-12 11:53:03.000000 alphaz-0.7.3.9/alphaz/apis/routes/git.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7225 2023-02-01 13:59:24.000000 alphaz-0.7.3.9/alphaz/apis/routes/logs.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2022-04-12 11:53:03.000000 alphaz-0.7.3.9/alphaz/apis/routes/mails.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6262 2023-03-17 07:21:40.000000 alphaz-0.7.3.9/alphaz/apis/routes/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1330 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/apis/routes/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/apis/routes/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2022-04-27 13:24:50.000000 alphaz-0.7.3.9/alphaz/apis/routes/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2475 2022-05-09 13:31:06.000000 alphaz-0.7.3.9/alphaz/apis/routes/user_management/application_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2228 2022-05-09 13:31:06.000000 alphaz-0.7.3.9/alphaz/apis/routes/user_management/permission_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4058 2022-08-31 08:56:44.000000 alphaz-0.7.3.9/alphaz/apis/routes/user_management/role_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2022-08-31 08:56:44.000000 alphaz-0.7.3.9/alphaz/apis/routes/user_management/user_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3025 2023-03-17 18:14:36.000000 alphaz-0.7.3.9/alphaz/apis/routes/users.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/apis/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/apis/users/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/apis/users/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-01-25 21:39:07.000000 alphaz-0.7.3.9/alphaz/apis/users/ldap.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11543 2023-03-28 08:47:21.000000 alphaz-0.7.3.9/alphaz/apis/users/users.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config/config.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config/config.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2022-08-11 06:44:17.000000 alphaz-0.7.3.9/alphaz/config/main_configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config/page.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config/source.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-01-06 09:14:28.000000 alphaz-0.7.3.9/alphaz/core.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/documentations/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.733881 alphaz-0.7.3.9/alphaz/documentations/docs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_admin.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9432 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_api.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_core.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5602 2022-07-19 09:10:48.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_database.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_screens.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/documentations/docs/alpha_setup.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-01-06 09:14:28.000000 alphaz-0.7.3.9/alphaz/documentations/docs/configuration.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2021-04-14 08:59:25.000000 alphaz-0.7.3.9/alphaz/documentations/docs/documentation.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/documentations/docs/index.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      440 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/documentations/mkdocs.yml
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9286 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/404.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_admin/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10320 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_admin/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    50340 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_api/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18850 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_core/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    43708 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_database/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_screens/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17967 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_screens/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/alpha_setup/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20169 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/alpha_setup/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.721881 alphaz-0.7.3.9/alphaz/documentations/site/assets/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/assets/images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/images/favicon.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.737881 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/workers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24568 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/documentation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13157 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/documentation/index.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25613 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.741881 alphaz-0.7.3.9/alphaz/documentations/site/search/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    53878 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/search/search_index.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1081 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/sitemap.xml
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      200 2023-04-12 11:28:53.000000 alphaz-0.7.3.9/alphaz/documentations/site/sitemap.xml.gz
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/git.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2022-05-14 15:57:01.000000 alphaz-0.7.3.9/alphaz/help.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.749881 alphaz-0.7.3.9/alphaz/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5786 2023-03-24 12:18:56.000000 alphaz-0.7.3.9/alphaz/libs/api_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/barcode_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13997 2023-03-24 12:18:56.000000 alphaz-0.7.3.9/alphaz/libs/config_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-03-29 19:04:59.000000 alphaz-0.7.3.9/alphaz/libs/converter_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9014 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/libs/database_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-02-06 12:52:51.000000 alphaz-0.7.3.9/alphaz/libs/date_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6222 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/libs/dict_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.749881 alphaz-0.7.3.9/alphaz/libs/emulation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-02-02 21:07:35.000000 alphaz-0.7.3.9/alphaz/libs/emulation/vt102_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/events.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/libs/files_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1096 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/libs/flask_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/ftp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/libs/img_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/libs/io_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3248 2023-03-16 19:44:05.000000 alphaz-0.7.3.9/alphaz/libs/json_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2022-07-21 11:35:27.000000 alphaz-0.7.3.9/alphaz/libs/logs_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12786 2023-03-17 15:11:43.000000 alphaz-0.7.3.9/alphaz/libs/mail_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/nav_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2022-09-07 06:57:10.000000 alphaz-0.7.3.9/alphaz/libs/notifications_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/number_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/os_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/process_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11058 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/libs/py_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      657 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/scp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/libs/search_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6386 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/libs/secure_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3018 2023-04-03 15:21:20.000000 alphaz-0.7.3.9/alphaz/libs/soap_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/libs/sql_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18289 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/libs/ssh_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11021 2023-04-08 08:30:59.000000 alphaz-0.7.3.9/alphaz/libs/string_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5139 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/libs/test_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/libs/time_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4200 2022-04-12 11:53:03.000000 alphaz-0.7.3.9/alphaz/libs/transactions_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5041 2022-12-01 15:14:08.000000 alphaz-0.7.3.9/alphaz/libs/user_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.749881 alphaz-0.7.3.9/alphaz/libs/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2022-04-27 13:24:50.000000 alphaz-0.7.3.9/alphaz/libs/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1354 2022-05-09 13:31:06.000000 alphaz-0.7.3.9/alphaz/libs/user_management/application_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1621 2022-10-07 10:05:05.000000 alphaz-0.7.3.9/alphaz/libs/user_management/permission_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3367 2022-10-07 10:05:05.000000 alphaz-0.7.3.9/alphaz/libs/user_management/role_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2336 2023-01-25 21:39:07.000000 alphaz-0.7.3.9/alphaz/libs/user_management/user_management_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.749881 alphaz-0.7.3.9/alphaz/mails/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.753881 alphaz-0.7.3.9/alphaz/mails/Images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/Images/Background.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/Images/Facebook_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/Images/Twitter_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/Images/Web_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/mails/Images/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/Mail.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2022-04-13 09:59:51.000000 alphaz-0.7.3.9/alphaz/mails/Webmail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/mails/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-03-17 05:42:16.000000 alphaz-0.7.3.9/alphaz/mails/debug.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-03-16 20:48:51.000000 alphaz-0.7.3.9/alphaz/mails/mail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/password_reset.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2022-04-13 09:59:51.000000 alphaz-0.7.3.9/alphaz/mails/stay_in_touch.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/mails/template.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.753881 alphaz-0.7.3.9/alphaz/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      145 2023-02-06 09:05:20.000000 alphaz-0.7.3.9/alphaz/models/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.753881 alphaz-0.7.3.9/alphaz/models/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2022-04-12 11:53:03.000000 alphaz-0.7.3.9/alphaz/models/api/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      710 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/api/_answer.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2021-09-13 12:55:49.000000 alphaz-0.7.3.9/alphaz/models/api/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2021-09-06 13:56:36.000000 alphaz-0.7.3.9/alphaz/models/api/_methods.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14253 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/api/_parameter.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2240 2022-08-26 12:58:11.000000 alphaz-0.7.3.9/alphaz/models/api/_requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18565 2023-03-29 19:05:00.000000 alphaz-0.7.3.9/alphaz/models/api/_route.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21563 2023-03-23 07:52:23.000000 alphaz-0.7.3.9/alphaz/models/api/_structures.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2022-02-01 21:43:05.000000 alphaz-0.7.3.9/alphaz/models/api/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2022-07-22 14:00:51.000000 alphaz-0.7.3.9/alphaz/models/base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.753881 alphaz-0.7.3.9/alphaz/models/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25438 2023-01-06 09:14:28.000000 alphaz-0.7.3.9/alphaz/models/config/_config.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12129 2021-08-12 12:49:09.000000 alphaz-0.7.3.9/alphaz/models/config/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2022-01-13 15:32:15.000000 alphaz-0.7.3.9/alphaz/models/database/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-03-17 15:16:42.000000 alphaz-0.7.3.9/alphaz/models/database/main_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10028 2023-03-19 14:55:26.000000 alphaz-0.7.3.9/alphaz/models/database/models.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2022-04-28 08:55:29.000000 alphaz-0.7.3.9/alphaz/models/database/operators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-01-25 21:39:07.000000 alphaz-0.7.3.9/alphaz/models/database/requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/database/row.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    53758 2023-03-16 19:44:05.000000 alphaz-0.7.3.9/alphaz/models/database/structure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/database/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4418 2023-03-16 19:51:01.000000 alphaz-0.7.3.9/alphaz/models/database/users_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9285 2022-08-02 08:51:28.000000 alphaz-0.7.3.9/alphaz/models/database/utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2022-04-12 11:53:03.000000 alphaz-0.7.3.9/alphaz/models/database/views.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/excel.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5126 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/models/ftp.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2022-07-19 09:10:48.000000 alphaz-0.7.3.9/alphaz/models/img.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/json/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/json/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-01-06 09:14:28.000000 alphaz-0.7.3.9/alphaz/models/json/_converters.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/logger/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2022-01-19 15:41:22.000000 alphaz-0.7.3.9/alphaz/models/logger/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-01-06 09:14:28.000000 alphaz-0.7.3.9/alphaz/models/logger/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14091 2023-04-05 11:16:09.000000 alphaz-0.7.3.9/alphaz/models/logger/_logger.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/logger/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/logs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.3.9/alphaz/models/logs/main.log
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.3.9/alphaz/models/logs/main.log.2021-11-07
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      385 2023-02-06 09:05:20.000000 alphaz-0.7.3.9/alphaz/models/main/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27102 2023-04-12 11:28:51.000000 alphaz-0.7.3.9/alphaz/models/main/_base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.757881 alphaz-0.7.3.9/alphaz/models/main/_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_core/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14630 2023-04-08 19:36:08.000000 alphaz-0.7.3.9/alphaz/models/main/_core/_core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_core/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      339 2023-02-06 09:05:20.000000 alphaz-0.7.3.9/alphaz/models/main/_enum.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1862 2023-02-17 08:49:35.000000 alphaz-0.7.3.9/alphaz/models/main/_exception.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_file.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_process.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_request.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/main/_singleton.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2258 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/models/request.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/models/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/models/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6780 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/tests/_category.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3095 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/tests/_group.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      109 2021-09-10 07:16:32.000000 alphaz-0.7.3.9/alphaz/models/tests/_levels.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4174 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/models/tests/_method.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4571 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/models/tests/_save.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13445 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/models/tests/_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6927 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/models/tests/_wrappers.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2802 2022-12-01 15:14:08.000000 alphaz-0.7.3.9/alphaz/models/user.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/models/watcher.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/pocs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/pocs/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/reload_gitignore.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2022-04-12 12:30:24.000000 alphaz-0.7.3.9/alphaz/req.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-04-11 14:13:25.000000 alphaz-0.7.3.9/alphaz/requirements.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/run.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/src/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/src/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/src/alpha.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/src/configs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/src/configs/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-01-25 21:39:07.000000 alphaz-0.7.3.9/alphaz/src/configs/loggers.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2022-01-13 15:32:15.000000 alphaz-0.7.3.9/alphaz/src/configs/loggers_colors.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/src/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/src/database/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/stitch/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/Core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/stitch/imports/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/imports/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.761881 alphaz-0.7.3.9/alphaz/stitch/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/stitch/models/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/models/element.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/run.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/stitch.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.769881 alphaz-0.7.3.9/alphaz/stitch/web-drivers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/web-drivers/chromedriver.exe
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/stitch/web-drivers/geckodriver
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.725881 alphaz-0.7.3.9/alphaz/stitch/websites/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.777881 alphaz-0.7.3.9/alphaz/stitch/websites/Test/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/stitch/websites/Test/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.777881 alphaz-0.7.3.9/alphaz/stitch/websites/stiki/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2022-04-13 09:59:51.000000 alphaz-0.7.3.9/alphaz/stitch/websites/stiki/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.781881 alphaz-0.7.3.9/alphaz/templates/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/templates/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.781881 alphaz-0.7.3.9/alphaz/templates/assets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-04-25 17:43:28.000000 alphaz-0.7.3.9/alphaz/templates/assets/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.781881 alphaz-0.7.3.9/alphaz/templates/assets/css/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2021-09-10 07:16:32.000000 alphaz-0.7.3.9/alphaz/templates/assets/css/home.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/css/logs.css
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/templates/assets/images/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/admin.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/alpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/save.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/start-icon.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/user.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/icons/wsalpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/images/loading.gif
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/templates/assets/js/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/templates/assets/js/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/js/libs/ansi_up.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/assets/js/libs/jquery.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2022-10-26 14:51:00.000000 alphaz-0.7.3.9/alphaz/templates/assets/js/logs.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/templates/hello.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/templates/home.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2021-08-06 18:55:11.000000 alphaz-0.7.3.9/alphaz/templates/logs.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-01-25 21:39:07.000000 alphaz-0.7.3.9/alphaz/test.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13857 2023-03-28 08:47:21.000000 alphaz-0.7.3.9/alphaz/tests/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      541 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/tests/basic_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2021-11-30 22:30:57.000000 alphaz-0.7.3.9/alphaz/tests/configurations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22695 2023-03-16 19:44:05.000000 alphaz-0.7.3.9/alphaz/tests/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/tests/processes.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/tests/utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.785881 alphaz-0.7.3.9/alphaz/utils/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       81 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/utils/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11552 2023-02-16 14:12:47.000000 alphaz-0.7.3.9/alphaz/utils/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2022-04-19 08:43:27.000000 alphaz-0.7.3.9/alphaz/utils/clean.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2022-05-02 08:25:25.000000 alphaz-0.7.3.9/alphaz/utils/configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2022-02-24 13:20:43.000000 alphaz-0.7.3.9/alphaz/utils/database_to_dataclass.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/utils/decorators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.3.9/alphaz/utils/ensure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2022-01-13 15:32:15.000000 alphaz-0.7.3.9/alphaz/utils/mep.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2021-04-21 22:36:11.000000 alphaz-0.7.3.9/alphaz/utils/screens.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22569 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/utils/selectionMenu.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/utils/tasks.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1535 2023-02-23 09:08:35.000000 alphaz-0.7.3.9/alphaz/utils/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-03-16 15:41:50.000000 alphaz-0.7.3.9/alphaz/utils/time.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3766 2022-01-17 10:25:20.000000 alphaz-0.7.3.9/alphaz/utils/transactions.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-04-12 11:28:54.729881 alphaz-0.7.3.9/alphaz.egg-info/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      589 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/alphaz.egg-info/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9706 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/alphaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/alphaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      447 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/alphaz.egg-info/requires.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-04-12 11:28:54.000000 alphaz-0.7.3.9/alphaz.egg-info/top_level.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-04-12 11:28:54.789881 alphaz-0.7.3.9/setup.cfg
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3075 2023-04-12 11:28:06.000000 alphaz-0.7.3.9/setup.py
```

### Comparing `alphaz-0.7.3.8/MANIFEST.in` & `alphaz-0.7.3.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/PKG-INFO` & `alphaz-0.7.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.3.8
+Version: 0.7.3.9
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.3.8.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.3.9.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.3.8/README.md` & `alphaz-0.7.3.9/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/api.json` & `alphaz-0.7.3.9/alphaz/api.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/api.py` & `alphaz-0.7.3.9/alphaz/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/mails.py` & `alphaz-0.7.3.9/alphaz/apis/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/admin.py` & `alphaz-0.7.3.9/alphaz/apis/routes/admin.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/api.py` & `alphaz-0.7.3.9/alphaz/apis/routes/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/basic_tests.py` & `alphaz-0.7.3.9/alphaz/apis/routes/basic_tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/database.py` & `alphaz-0.7.3.9/alphaz/apis/routes/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/logs.py` & `alphaz-0.7.3.9/alphaz/apis/routes/logs.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/mails.py` & `alphaz-0.7.3.9/alphaz/apis/routes/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/main.py` & `alphaz-0.7.3.9/alphaz/apis/routes/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/tests.py` & `alphaz-0.7.3.9/alphaz/apis/routes/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/user_management/application_management.py` & `alphaz-0.7.3.9/alphaz/apis/routes/user_management/application_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/user_management/permission_management.py` & `alphaz-0.7.3.9/alphaz/apis/routes/user_management/permission_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/user_management/role_management.py` & `alphaz-0.7.3.9/alphaz/apis/routes/user_management/role_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/user_management/user_management.py` & `alphaz-0.7.3.9/alphaz/apis/routes/user_management/user_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/routes/users.py` & `alphaz-0.7.3.9/alphaz/apis/routes/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/tests.py` & `alphaz-0.7.3.9/alphaz/apis/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/users/ldap.py` & `alphaz-0.7.3.9/alphaz/apis/users/ldap.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/apis/users/users.py` & `alphaz-0.7.3.9/alphaz/apis/users/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/config/config.css` & `alphaz-0.7.3.9/alphaz/config/config.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/config/config.html` & `alphaz-0.7.3.9/alphaz/config/config.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/config/main_configuration.py` & `alphaz-0.7.3.9/alphaz/config/main_configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/config/page.py` & `alphaz-0.7.3.9/alphaz/config/page.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/config/source.html` & `alphaz-0.7.3.9/alphaz/config/source.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/config.json` & `alphaz-0.7.3.9/alphaz/config.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/docs/alpha_api.md` & `alphaz-0.7.3.9/alphaz/documentations/docs/alpha_api.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,35 @@
 
 ```python
 from core import core, API
 ```
 
 > **api** / **API** is the equivalent for **app** in **Flask** framework.
 
+### Routes
+
+We recommend to add all the route definition in **apis/routes** folder and import all the route definition in **apis/routes/__init__.py**.
+
+Then you will have to import the route in thoe **core.py** file:
+
+```python
+from alphaz.models.main import AlphaCore, singleton
+
+@singleton
+class Core(AlphaCore):
+
+    def __init__(self,file:str):
+
+        super().__init__(file)
+
+core = Core(__file__)
+DB, API, LOG = core.db, core.api, core.log # not required but recommanded
+
+from apis.routes import *
+```
 
 ## Configuration
 
 The api is automatically configured from the `api.jon` file. See [Configuration](configuration.md) for further details on how to use it.
 
 ### Main
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/docs/alpha_core.md` & `alphaz-0.7.3.9/alphaz/documentations/docs/alpha_core.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Alpha core system 
 
 ## Purpose
 
 The **core** is used as a central point to manage various system:
-    - [logging system](## Logging)
-    - [database access](## Database)
-    - [api system](## API)
-    - [dynamic configuration](## Configuration)
+
+- [logging system](## Logging)
+- [database access](## Database)
+- [api system](## API)
+- [dynamic configuration](## Configuration)
 
 ## How to use
 
 You could:
 
-- Use the **alphaz** core and initiate it at the start of you project:
+- Use the **alphaz** core and initiate it at the start of you project preferably in a file named **core.py** to be complient with this documentation:
 
     ```python
     from alphaz.models.main import AlphaCore
 
     core = AlphaCore(__file__)
-    DB = core.db # not required but recommanded
+    DB, API, LOG = core.db, core.api, core.log # not required but recommanded
     ```
 
 - Or create a **core.py** file at the **root** of your project containing at least:
 
     ```python
     from alphaz.models.main import AlphaCore, singleton
 
@@ -30,15 +31,15 @@
     class Core(AlphaCore):
 
         def __init__(self,file:str):
 
             super().__init__(file)
 
     core = Core(__file__)
-    DB = core.db # not required but recommanded
+    DB, API, LOG = core.db, core.api, core.log # not required but recommanded
     ```
 
 !!! note
     This is the recommended way, so that you could custom the Core class
 
 ## Logging
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/docs/alpha_database.md` & `alphaz-0.7.3.9/alphaz/documentations/docs/alpha_database.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/docs/alpha_screens.md` & `alphaz-0.7.3.9/alphaz/documentations/docs/alpha_screens.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/docs/alpha_setup.md` & `alphaz-0.7.3.9/alphaz/documentations/docs/alpha_setup.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - Python 3.10.4 is required.
 [Anaconda](https://www.anaconda.com/) or [Miniconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html) could be used.
 
 There is no constraint but the usual structure is to have:
 
 - a user per configuration (_mes_, _mesacc_, _mesint_ and _mesdev_ for exemple)
 - three location per user:
-    - *_/home/USER/APP_NAME_* for sources
+    - *_/application/USER/APP_NAME_* for sources
     - *_/home/USER/configs_* for configurations
     - *_/application/USER/APP_NAME_* for tmp files and logs
 
 !!! note
     This is configured within the conf.json file and could be modified
 
 ## Setup
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/docs/configuration.md` & `alphaz-0.7.3.9/alphaz/documentations/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/docs/index.md` & `alphaz-0.7.3.9/alphaz/documentations/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Welcome to Alpha environment documention
 
-Alpha is an **ecosystem** based on multiple **frameworks** and **libraries** for both **frontend** and **backend**.
+Alpha is an **ecosystem** based on a multiple **frameworks** and **libraries** for both **frontend** and **backend**.
 
 ## Purpose
 
 The purpose of the **ecosystem** is to simplify any dev activity. 
 
-??? note "Standard query"
+??? note "Standard query approach"
 
     ```py
     from core import core
     DB = core.db 
+
     def get_logs(start_date=None, end_date=None, useLimit=False, pageForLimit=1):
         total = 0
         logs = []
         limit = 20
         start = (pageForLimit - 1) * limit
 
         query = "SELECT COUNT(*) AS count FROM logs"
@@ -50,15 +51,15 @@
             log["stack"] = row[3]
             log["date"] = row[4]
             logs.append(log)
 
         return {'total' : total, 'logs' : logs}
     ```
 
-??? note "Alpha Query"
+??? note "Alpha query approach"
 
     ```py
     from core import core
     DB = core.DB
     def get_logs(
         start_date: datetime = None,
         end_date: datetime = None,
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/404.html` & `alphaz-0.7.3.9/alphaz/documentations/site/404.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -190,31 +190,31 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="/alpha_api/" class="md-nav__link">
-        Api
+      <a href="/alpha_core/" class="md-nav__link">
+        Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="/alpha_core/" class="md-nav__link">
-        Core
+      <a href="/alpha_api/" class="md-nav__link">
+        Api
       </a>
     </li>
```

#### html2text {}

```diff
@@ -12,16 +12,16 @@
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
-    * Api
     * Core
+    * Api
     * Screens
     * Configuration
     * Database
     * Documentation
     * Administration
 ****** 404 - Not found ******
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/alpha_admin/index.html` & `alphaz-0.7.3.9/alphaz/documentations/site/alpha_admin/index.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -190,31 +190,31 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
-        Api
+      <a href="../alpha_core/" class="md-nav__link">
+        Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
-        Core
+      <a href="../alpha_api/" class="md-nav__link">
+        Api
       </a>
     </li>
```

#### html2text {}

```diff
@@ -12,16 +12,16 @@
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
-    * Api
     * Core
+    * Api
     * Screens
     * Configuration
     * Database
     * Documentation
     * ⁰ Administration
 ****** Administration ******
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/alpha_api/index.html` & `alphaz-0.7.3.9/alphaz/documentations/site/alpha_api/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -193,14 +193,29 @@
     
       
       
       
 
   
   
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
     
   
   
     <li class="md-nav__item md-nav__item--active">
       
       <input class="md-nav__toggle md-toggle" data-md-toggle="toc" type="checkbox" id="__toc">
       
@@ -244,14 +259,27 @@
 </li>
       
         <li class="md-nav__item">
   <a href="#how-to-use" class="md-nav__link">
     How to use
   </a>
   
+    <nav class="md-nav" aria-label="How to use">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#routes" class="md-nav__link">
+    Routes
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
 </li>
       
         <li class="md-nav__item">
   <a href="#configuration" class="md-nav__link">
     Configuration
   </a>
   
@@ -302,15 +330,15 @@
         
       </ul>
     </nav>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#routes" class="md-nav__link">
+  <a href="#routes_1" class="md-nav__link">
     Routes
   </a>
   
     <nav class="md-nav" aria-label="Routes">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
@@ -500,29 +528,14 @@
       
       
 
   
   
   
     <li class="md-nav__item">
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
-  
-    <li class="md-nav__item">
       <a href="../alpha_screens/" class="md-nav__link">
         Screens
       </a>
     </li>
   
 
     
@@ -625,14 +638,27 @@
 </li>
       
         <li class="md-nav__item">
   <a href="#how-to-use" class="md-nav__link">
     How to use
   </a>
   
+    <nav class="md-nav" aria-label="How to use">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#routes" class="md-nav__link">
+    Routes
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
 </li>
       
         <li class="md-nav__item">
   <a href="#configuration" class="md-nav__link">
     Configuration
   </a>
   
@@ -683,15 +709,15 @@
         
       </ul>
     </nav>
   
 </li>
       
         <li class="md-nav__item">
-  <a href="#routes" class="md-nav__link">
+  <a href="#routes_1" class="md-nav__link">
     Routes
   </a>
   
     <nav class="md-nav" aria-label="Routes">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
@@ -902,14 +928,31 @@
 </code></pre></div>
 <p>or from the <strong>core</strong> if you are using it</p>
 <div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span><span class="p">,</span> <span class="n">API</span>
 </code></pre></div>
 <blockquote>
 <p><strong>api</strong> / <strong>API</strong> is the equivalent for <strong>app</strong> in <strong>Flask</strong> framework.</p>
 </blockquote>
+<h3 id="routes">Routes</h3>
+<p>We recommend to add all the route definition in <strong>apis/routes</strong> folder and import all the route definition in <strong>apis/routes/<strong>init</strong>.py</strong>.</p>
+<p>Then you will have to import the route in thoe <strong>core.py</strong> file:</p>
+<div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.models.main</span> <span class="kn">import</span> <span class="n">AlphaCore</span><span class="p">,</span> <span class="n">singleton</span>
+
+<span class="nd">@singleton</span>
+<span class="k">class</span> <span class="nc">Core</span><span class="p">(</span><span class="n">AlphaCore</span><span class="p">):</span>
+
+    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span><span class="n">file</span><span class="p">:</span><span class="nb">str</span><span class="p">):</span>
+
+        <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="fm">__init__</span><span class="p">(</span><span class="n">file</span><span class="p">)</span>
+
+<span class="n">core</span> <span class="o">=</span> <span class="n">Core</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span>
+<span class="n">DB</span><span class="p">,</span> <span class="n">API</span><span class="p">,</span> <span class="n">LOG</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">api</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">log</span> <span class="c1"># not required but recommanded</span>
+
+<span class="kn">from</span> <span class="nn">apis.routes</span> <span class="kn">import</span> <span class="o">*</span>
+</code></pre></div>
 <h2 id="configuration">Configuration</h2>
 <p>The api is automatically configured from the <code>api.jon</code> file. See <a href="../configuration/">Configuration</a> for further details on how to use it.</p>
 <h3 id="main">Main</h3>
 <ul>
 <li>workers: In order to specify the numbers of workers</li>
 </ul>
 <div class="highlight"><pre><span></span><code><span class="nt">&quot;workers&quot;</span><span class="p">:</span> <span class="mi">6</span>
@@ -1016,15 +1059,15 @@
         <span class="nt">&quot;SECURITY_TOKEN&quot;</span><span class="p">:</span> <span class="s2">&quot;a_security_token&quot;</span>
     <span class="p">},</span>
     <span class="nt">&quot;database&quot;</span><span class="p">:</span> <span class="p">{</span>
         <span class="nt">&quot;DATABASE&quot;</span><span class="p">:</span> <span class="s2">&quot;sqlite:///{{root}}/dashboard.db&quot;</span>
     <span class="p">}</span>
 <span class="p">}</span>
 </code></pre></div>
-<h2 id="routes">Routes</h2>
+<h2 id="routes_1">Routes</h2>
 <h3 id="basic">Basic</h3>
 <p>To specify an api route, juste use the <code>route</code> flag:</p>
 <div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.utils.api</span> <span class="kn">import</span> <span class="n">route</span><span class="p">,</span> <span class="n">api</span><span class="p">,</span> <span class="n">Parameter</span>
 
 <span class="nd">@route</span><span class="p">(</span><span class="s2">&quot;route_name&quot;</span><span class="p">)</span>
 <span class="k">def</span> <span class="nf">method_name</span><span class="p">():</span>
     <span class="k">return</span> <span class="s2">&quot;hello&quot;</span>
@@ -1191,36 +1234,36 @@
       </main>
       
         
 <footer class="md-footer">
   
     <nav class="md-footer__inner md-grid" aria-label="Footer">
       
-        <a href="../alpha_setup/" class="md-footer__link md-footer__link--prev" rel="prev">
+        <a href="../alpha_core/" class="md-footer__link md-footer__link--prev" rel="prev">
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12z"/></svg>
           </div>
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Previous
               </span>
-              Setup
+              Core
             </div>
           </div>
         </a>
       
       
-        <a href="../alpha_core/" class="md-footer__link md-footer__link--next" rel="next">
+        <a href="../alpha_screens/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Next
               </span>
-              Core
+              Screens
             </div>
           </div>
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4z"/></svg>
           </div>
         </a>
```

#### html2text {}

```diff
@@ -13,18 +13,20 @@
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
+    * Core
     * ⁰  Api   Api    Table of contents
           o Introduction
           o Launch
           o How_to_use
+                # Routes
           o Configuration
                 # Main
                 # Mails
                 # Auth
                 # Reloader_type
                 # Admin
                 # Dashboard
@@ -45,24 +47,24 @@
                 # Condition
                 # How_to_use
                       # Single_route_mode
                       # Login_to_the_api
                       # Logout_from_the_api
           o Issues
                 # Database_alias
-    * Core
     * Screens
     * Configuration
     * Database
     * Documentation
     * Administration
    Table of contents
     * Introduction
     * Launch
     * How_to_use
+          o Routes
     * Configuration
           o Main
           o Mails
           o Auth
           o Reloader_type
           o Admin
           o Dashboard
@@ -101,14 +103,31 @@
 127.0.0.1:<port>
 ***** How to use *****
 Your could import it using simply from the utils:
 from alphaz.utils.api import api
 or from the core if you are using it
 from core import core, API
      api / API is the equivalent for app in Flask framework.
+**** Routes ****
+We recommend to add all the route definition in apis/routes folder and import
+all the route definition in apis/routes/init.py.
+Then you will have to import the route in thoe core.py file:
+from alphaz.models.main import AlphaCore, singleton
+
+@singleton
+class Core(AlphaCore):
+
+    def __init__(self,file:str):
+
+        super().__init__(file)
+
+core = Core(__file__)
+DB, API, LOG = core.db, core.api, core.log # not required but recommanded
+
+from apis.routes import *
 ***** Configuration *****
 The api is automatically configured from the api.jon file. See Configuration
 for further details on how to use it.
 **** Main ****
     * workers: In order to specify the numbers of workers
 "workers": 6
     * routes_no_log: In order to specify the routes where log must be ignored
@@ -330,12 +349,12 @@
 *** Logout from the api ***
 Use the route /logout/su in order to logout.
 ***** Issues *****
      In progress
 **** Database alias ****
      In progress
 
- Previous__Setup
+ Previous__Core
 
- Next__Core
+ Next__Screens
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/alpha_core/index.html` & `alphaz-0.7.3.9/alphaz/documentations/site/alpha_core/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -193,29 +193,14 @@
     
       
       
       
 
   
   
-  
-    <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
-        Api
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
       
@@ -304,14 +289,29 @@
       
       
 
   
   
   
     <li class="md-nav__item">
+      <a href="../alpha_api/" class="md-nav__link">
+        Api
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
       <a href="../alpha_screens/" class="md-nav__link">
         Screens
       </a>
     </li>
   
 
     
@@ -458,43 +458,45 @@
           <div class="md-content" data-md-component="content">
             <article class="md-content__inner md-typeset">
               
                 
                 
                 <h1 id="alpha-core-system">Alpha core system</h1>
 <h2 id="purpose">Purpose</h2>
-<p>The <strong>core</strong> is used as a central point to manage various system:
-    - <a href="## Logging">logging system</a>
-    - <a href="## Database">database access</a>
-    - <a href="## API">api system</a>
-    - <a href="## Configuration">dynamic configuration</a></p>
+<p>The <strong>core</strong> is used as a central point to manage various system:</p>
+<ul>
+<li><a href="## Logging">logging system</a></li>
+<li><a href="## Database">database access</a></li>
+<li><a href="## API">api system</a></li>
+<li><a href="## Configuration">dynamic configuration</a></li>
+</ul>
 <h2 id="how-to-use">How to use</h2>
 <p>You could:</p>
 <ul>
 <li>
-<p>Use the <strong>alphaz</strong> core and initiate it at the start of you project:</p>
+<p>Use the <strong>alphaz</strong> core and initiate it at the start of you project preferably in a file named <strong>core.py</strong> to be complient with this documentation:</p>
 <div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.models.main</span> <span class="kn">import</span> <span class="n">AlphaCore</span>
 
 <span class="n">core</span> <span class="o">=</span> <span class="n">AlphaCore</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span>
-<span class="n">DB</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span> <span class="c1"># not required but recommanded</span>
+<span class="n">DB</span><span class="p">,</span> <span class="n">API</span><span class="p">,</span> <span class="n">LOG</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">api</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">log</span> <span class="c1"># not required but recommanded</span>
 </code></pre></div>
 </li>
 <li>
 <p>Or create a <strong>core.py</strong> file at the <strong>root</strong> of your project containing at least:</p>
 <div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">alphaz.models.main</span> <span class="kn">import</span> <span class="n">AlphaCore</span><span class="p">,</span> <span class="n">singleton</span>
 
 <span class="nd">@singleton</span>
 <span class="k">class</span> <span class="nc">Core</span><span class="p">(</span><span class="n">AlphaCore</span><span class="p">):</span>
 
     <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span><span class="n">file</span><span class="p">:</span><span class="nb">str</span><span class="p">):</span>
 
         <span class="nb">super</span><span class="p">()</span><span class="o">.</span><span class="fm">__init__</span><span class="p">(</span><span class="n">file</span><span class="p">)</span>
 
 <span class="n">core</span> <span class="o">=</span> <span class="n">Core</span><span class="p">(</span><span class="vm">__file__</span><span class="p">)</span>
-<span class="n">DB</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span> <span class="c1"># not required but recommanded</span>
+<span class="n">DB</span><span class="p">,</span> <span class="n">API</span><span class="p">,</span> <span class="n">LOG</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">api</span><span class="p">,</span> <span class="n">core</span><span class="o">.</span><span class="n">log</span> <span class="c1"># not required but recommanded</span>
 </code></pre></div>
 </li>
 </ul>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
 <p>This is the recommended way, so that you could custom the Core class</p>
 </div>
@@ -530,36 +532,36 @@
       </main>
       
         
 <footer class="md-footer">
   
     <nav class="md-footer__inner md-grid" aria-label="Footer">
       
-        <a href="../alpha_api/" class="md-footer__link md-footer__link--prev" rel="prev">
+        <a href="../alpha_setup/" class="md-footer__link md-footer__link--prev" rel="prev">
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12z"/></svg>
           </div>
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Previous
               </span>
-              Api
+              Setup
             </div>
           </div>
         </a>
       
       
-        <a href="../alpha_screens/" class="md-footer__link md-footer__link--next" rel="next">
+        <a href="../alpha_api/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Next
               </span>
-              Screens
+              Api
             </div>
           </div>
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4z"/></svg>
           </div>
         </a>
```

#### html2text {}

```diff
@@ -13,57 +13,62 @@
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
-    * Api
     * ⁰  Core   Core    Table of contents
           o Purpose
           o How_to_use
           o Logging
                 # Database
           o API
           o Configuration
+    * Api
     * Screens
     * Configuration
     * Database
     * Documentation
     * Administration
    Table of contents
     * Purpose
     * How_to_use
     * Logging
           o Database
     * API
     * Configuration
 ****** Alpha core system ******
 ***** Purpose *****
-The core is used as a central point to manage various system: - logging_system
-- database_access - api_system - dynamic_configuration
+The core is used as a central point to manage various system:
+    * logging_system
+    * database_access
+    * api_system
+    * dynamic_configuration
 ***** How to use *****
 You could:
-    * Use the alphaz core and initiate it at the start of you project:
+    * Use the alphaz core and initiate it at the start of you project
+      preferably in a file named core.py to be complient with this
+      documentation:
       from alphaz.models.main import AlphaCore
 
       core = AlphaCore(__file__)
-      DB = core.db # not required but recommanded
+      DB, API, LOG = core.db, core.api, core.log # not required but recommanded
     * Or create a core.py file at the root of your project containing at least:
       from alphaz.models.main import AlphaCore, singleton
 
       @singleton
       class Core(AlphaCore):
 
           def __init__(self,file:str):
 
               super().__init__(file)
 
       core = Core(__file__)
-      DB = core.db # not required but recommanded
+      DB, API, LOG = core.db, core.api, core.log # not required but recommanded
 Note
 This is the recommended way, so that you could custom the Core class
 ***** Logging *****
 from core import core
 LOG = core.get_logger('name')
 LOG.info('message')
 **** Database ****
@@ -73,12 +78,12 @@
 from core import core
 API = core.api
 ***** Configuration *****
 from core import core
 CONFIG = core.config
 tmp_directory_path = CONFIG.get('directories/tmp')
 
- Previous__Api
+ Previous__Setup
 
- Next__Screens
+ Next__Api
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/alpha_database/index.html` & `alphaz-0.7.3.9/alphaz/documentations/site/alpha_database/index.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,31 +195,31 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
-        Api
+      <a href="../alpha_core/" class="md-nav__link">
+        Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
-        Core
+      <a href="../alpha_api/" class="md-nav__link">
+        Api
       </a>
     </li>
```

#### html2text {}

```diff
@@ -13,16 +13,16 @@
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
-    * Api
     * Core
+    * Api
     * Screens
     * Configuration
     * ⁰  Database   Database    Table of contents
           o Automatic_structure
           o Schema
                 # Specific_Schema
           o Alpha_notation
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/alpha_screens/index.html` & `alphaz-0.7.3.9/alphaz/documentations/site/alpha_screens/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -195,31 +195,31 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
-        Api
+      <a href="../alpha_core/" class="md-nav__link">
+        Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
-        Core
+      <a href="../alpha_api/" class="md-nav__link">
+        Api
       </a>
     </li>
   
 
     
       
       
@@ -487,24 +487,24 @@
       </main>
       
         
 <footer class="md-footer">
   
     <nav class="md-footer__inner md-grid" aria-label="Footer">
       
-        <a href="../alpha_core/" class="md-footer__link md-footer__link--prev" rel="prev">
+        <a href="../alpha_api/" class="md-footer__link md-footer__link--prev" rel="prev">
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M20 11v2H8l5.5 5.5-1.42 1.42L4.16 12l7.92-7.92L13.5 5.5 8 11h12z"/></svg>
           </div>
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Previous
               </span>
-              Core
+              Api
             </div>
           </div>
         </a>
       
       
         <a href="../configuration/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
```

#### html2text {}

```diff
@@ -13,16 +13,16 @@
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
-    * Api
     * Core
+    * Api
     * ⁰  Screens   Screens    Table of contents
           o Launch
           o Help
     * Configuration
     * Database
     * Documentation
     * Administration
@@ -88,12 +88,12 @@
           "name": "pyMES"
       }
    2. Parameters:
       python -m alphaz.utils.screens * --name TEST * --cmd "python api.py"
 ***** Help *****
 python -m alphaz.utils.screens
 
- Previous__Core
+ Previous__Api
 
  Next__Configuration
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/alpha_setup/index.html` & `alphaz-0.7.3.9/alphaz/documentations/site/alpha_setup/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -313,31 +313,31 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
-        Api
+      <a href="../alpha_core/" class="md-nav__link">
+        Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
-        Core
+      <a href="../alpha_api/" class="md-nav__link">
+        Api
       </a>
     </li>
   
 
     
       
       
@@ -549,15 +549,15 @@
 <li>Python 3.10.4 is required.
 <a href="https://www.anaconda.com/">Anaconda</a> or <a href="https://docs.conda.io/projects/conda/en/latest/user-guide/install/linux.html">Miniconda</a> could be used.</li>
 </ul>
 <p>There is no constraint but the usual structure is to have:</p>
 <ul>
 <li>a user per configuration (<em>mes</em>, <em>mesacc</em>, <em>mesint</em> and <em>mesdev</em> for exemple)</li>
 <li>three location per user:<ul>
-<li><em><em>/home/USER/APP_NAME</em></em> for sources</li>
+<li><em><em>/application/USER/APP_NAME</em></em> for sources</li>
 <li><em><em>/home/USER/configs</em></em> for configurations</li>
 <li><em><em>/application/USER/APP_NAME</em></em> for tmp files and logs</li>
 </ul>
 </li>
 </ul>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
@@ -639,21 +639,21 @@
               </span>
               Home
             </div>
           </div>
         </a>
       
       
-        <a href="../alpha_api/" class="md-footer__link md-footer__link--next" rel="next">
+        <a href="../alpha_core/" class="md-footer__link md-footer__link--next" rel="next">
           <div class="md-footer__title">
             <div class="md-ellipsis">
               <span class="md-footer__direction">
                 Next
               </span>
-              Api
+              Core
             </div>
           </div>
           <div class="md-footer__button md-icon">
             <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M4 11v2h12l-5.5 5.5 1.42 1.42L19.84 12l-7.92-7.92L10.5 5.5 16 11H4z"/></svg>
           </div>
         </a>
```

#### html2text {}

```diff
@@ -22,16 +22,16 @@
           o Setup
                 # Classic
                 # Using_sources
           o Dependencies
                 # Oracle
           o Configuration
                 # Angular
-    * Api
     * Core
+    * Api
     * Screens
     * Configuration
     * Database
     * Documentation
     * Administration
    Table of contents
     * OS_configuration
@@ -48,15 +48,15 @@
 Important
 make sure that Git is well configured.
 **** Python ****
     * Python 3.10.4 is required. Anaconda or Miniconda could be used.
 There is no constraint but the usual structure is to have:
     * a user per configuration (mes, mesacc, mesint and mesdev for exemple)
     * three location per user:
-          o /home/USER/APP_NAME for sources
+          o /application/USER/APP_NAME for sources
           o /home/USER/configs for configurations
           o /application/USER/APP_NAME for tmp files and logs
 Note
 This is configured within the conf.json file and could be modified
 ***** Setup *****
 If you just want to use the system go for the classic way and if you want to
 modify it use the sources integration.
@@ -95,10 +95,10 @@
       "@constants/*": ["app/constants/*", "src/app/constants/*"]
     }
   }
 }
 
  Previous__Home
 
- Next__Api
+ Next__Core
 
 Made with Material_for_MkDocs
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/images/favicon.png` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map` & `alphaz-0.7.3.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/configuration/index.html` & `alphaz-0.7.3.9/alphaz/documentations/site/configuration/index.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,31 +195,31 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
-        Api
+      <a href="../alpha_core/" class="md-nav__link">
+        Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
-        Core
+      <a href="../alpha_api/" class="md-nav__link">
+        Api
       </a>
     </li>
```

#### html2text {}

```diff
@@ -13,16 +13,16 @@
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
-    * Api
     * Core
+    * Api
     * Screens
     * ⁰  Configuration   Configuration    Table of contents
           o Parameters
                 # Main
                 # Directories
                 # System_environments_variables
                 # Environments_configurations
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/documentation/index.html` & `alphaz-0.7.3.9/alphaz/documentations/site/documentation/index.html`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -195,31 +195,31 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_api/" class="md-nav__link">
-        Api
+      <a href="../alpha_core/" class="md-nav__link">
+        Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="../alpha_core/" class="md-nav__link">
-        Core
+      <a href="../alpha_api/" class="md-nav__link">
+        Api
       </a>
     </li>
```

#### html2text {}

```diff
@@ -13,16 +13,16 @@
 
 [query               ]
 Initializing search
 
    Alpha Documentation
     * Home
     * Setup
-    * Api
     * Core
+    * Api
     * Screens
     * Configuration
     * Database
     * ⁰  Documentation   Documentation    Table of contents
           o Requirements
           o More
     * Administration
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/index.html` & `alphaz-0.7.3.9/alphaz/documentations/site/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -282,31 +282,31 @@
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="alpha_api/" class="md-nav__link">
-        Api
+      <a href="alpha_core/" class="md-nav__link">
+        Core
       </a>
     </li>
   
 
     
       
       
       
 
   
   
   
     <li class="md-nav__item">
-      <a href="alpha_core/" class="md-nav__link">
-        Core
+      <a href="alpha_api/" class="md-nav__link">
+        Api
       </a>
     </li>
   
 
     
       
       
@@ -473,19 +473,20 @@
           
           <div class="md-content" data-md-component="content">
             <article class="md-content__inner md-typeset">
               
                 
                 
                 <h1 id="welcome-to-alpha-environment-documention">Welcome to Alpha environment documention</h1>
-<p>Alpha is an <strong>ecosystem</strong> based on multiple <strong>frameworks</strong> and <strong>libraries</strong> for both <strong>frontend</strong> and <strong>backend</strong>.</p>
+<p>Alpha is an <strong>ecosystem</strong> based on a multiple <strong>frameworks</strong> and <strong>libraries</strong> for both <strong>frontend</strong> and <strong>backend</strong>.</p>
 <h2 id="purpose">Purpose</h2>
 <p>The purpose of the <strong>ecosystem</strong> is to simplify any dev activity. </p>
-<details class="note"><summary>Standard query</summary><div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
+<details class="note"><summary>Standard query approach</summary><div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
 <span class="n">DB</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">db</span> 
+
 <span class="k">def</span> <span class="nf">get_logs</span><span class="p">(</span><span class="n">start_date</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">end_date</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span> <span class="n">useLimit</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">pageForLimit</span><span class="o">=</span><span class="mi">1</span><span class="p">):</span>
     <span class="n">total</span> <span class="o">=</span> <span class="mi">0</span>
     <span class="n">logs</span> <span class="o">=</span> <span class="p">[]</span>
     <span class="n">limit</span> <span class="o">=</span> <span class="mi">20</span>
     <span class="n">start</span> <span class="o">=</span> <span class="p">(</span><span class="n">pageForLimit</span> <span class="o">-</span> <span class="mi">1</span><span class="p">)</span> <span class="o">*</span> <span class="n">limit</span>
 
     <span class="n">query</span> <span class="o">=</span> <span class="s2">&quot;SELECT COUNT(*) AS count FROM logs&quot;</span>
@@ -521,15 +522,15 @@
         <span class="n">log</span><span class="p">[</span><span class="s2">&quot;stack&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">3</span><span class="p">]</span>
         <span class="n">log</span><span class="p">[</span><span class="s2">&quot;date&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">4</span><span class="p">]</span>
         <span class="n">logs</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">log</span><span class="p">)</span>
 
     <span class="k">return</span> <span class="p">{</span><span class="s1">&#39;total&#39;</span> <span class="p">:</span> <span class="n">total</span><span class="p">,</span> <span class="s1">&#39;logs&#39;</span> <span class="p">:</span> <span class="n">logs</span><span class="p">}</span>
 </code></pre></div>
 </details>
-<details class="note"><summary>Alpha Query</summary><div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
+<details class="note"><summary>Alpha query approach</summary><div class="highlight"><pre><span></span><code><span class="kn">from</span> <span class="nn">core</span> <span class="kn">import</span> <span class="n">core</span>
 <span class="n">DB</span> <span class="o">=</span> <span class="n">core</span><span class="o">.</span><span class="n">DB</span>
 <span class="k">def</span> <span class="nf">get_logs</span><span class="p">(</span>
     <span class="n">start_date</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
     <span class="n">end_date</span><span class="p">:</span> <span class="n">datetime</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
     <span class="n">limit</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="kc">False</span><span class="p">,</span>
     <span class="n">page</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">0</span><span class="p">,</span>
     <span class="n">per_page</span><span class="p">:</span> <span class="nb">int</span> <span class="o">=</span> <span class="mi">100</span><span class="p">,</span>
```

#### html2text {}

```diff
@@ -21,16 +21,16 @@
           o Features
           o Tech
           o Project_layout
           o Frontend:_Alphaa
           o Features
           o Project_layout
     * Setup
-    * Api
     * Core
+    * Api
     * Screens
     * Configuration
     * Database
     * Documentation
     * Administration
    Table of contents
     * Purpose
@@ -38,21 +38,22 @@
     * Features
     * Tech
     * Project_layout
     * Frontend:_Alphaa
     * Features
     * Project_layout
 ****** Welcome to Alpha environment documention ******
-Alpha is an ecosystem based on multiple frameworks and libraries for both
+Alpha is an ecosystem based on a multiple frameworks and libraries for both
 frontend and backend.
 ***** Purpose *****
 The purpose of the ecosystem is to simplify any dev activity.
-Standard query
+Standard query approach
 from core import core
 DB = core.db
+
 def get_logs(start_date=None, end_date=None, useLimit=False, pageForLimit=1):
     total = 0
     logs = []
     limit = 20
     start = (pageForLimit - 1) * limit
 
     query = "SELECT COUNT(*) AS count FROM logs"
@@ -86,15 +87,15 @@
         log["origin"] = row[1]
         log["message"] = row[2]
         log["stack"] = row[3]
         log["date"] = row[4]
         logs.append(log)
 
     return {'total' : total, 'logs' : logs}
- Alpha Query
+ Alpha query approach
 from core import core
 DB = core.DB
 def get_logs(
     start_date: datetime = None,
     end_date: datetime = None,
     limit: int = False,
     page: int = 0,
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/search/search_index.json` & `alphaz-0.7.3.9/alphaz/documentations/site/search/search_index.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933993399339934%*

 * *Differences: {"'docs'": "{0: {'text': 'Welcome to Alpha environment documention Alpha is an ecosystem based on "*

 * *           'a multiple frameworks and libraries for both frontend and backend . Purpose The '*

 * *           'purpose of the ecosystem is to simplify any dev activity. Standard query approach from '*

 * *           'core import core DB = core . db def get_logs ( start_date = None , end_date = None , '*

 * *           'useLimit = False , pageForLimit = 1 ): total = 0 logs = [] limit = 20 start = ( '*

 * *           'pageForLimit […]*

```diff
@@ -6,25 +6,25 @@
         "min_search_length": 3,
         "prebuild_index": false,
         "separator": "[\\s\\-]+"
     },
     "docs": [
         {
             "location": "",
-            "text": "Welcome to Alpha environment documention Alpha is an ecosystem based on multiple frameworks and libraries for both frontend and backend . Purpose The purpose of the ecosystem is to simplify any dev activity. Standard query from core import core DB = core . db def get_logs ( start_date = None , end_date = None , useLimit = False , pageForLimit = 1 ): total = 0 logs = [] limit = 20 start = ( pageForLimit - 1 ) * limit query = \"SELECT COUNT(*) AS count FROM logs\" parameters = [] if start_date is not None and end_date is not None : query += \" AND CAST(date AS DATE) between %s and %s \" parameters . append ( start_date ) parameters . append ( end_date ) query += \" ORDER BY date DESC\" rows = DB . get ( query , parameters ) for row in rows : total = row [ 0 ] query = \"SELECT type, origin, message, stack, date FROM logs\" parameters = [] if start_date is not None and end_date is not None : query += \" AND CAST(date AS DATE) between %s and %s \" parameters . append ( start_date ) parameters . append ( end_date ) query += \" ORDER BY date DESC\" if useLimit : query += \" LIMIT %s OFFSET %s \" parameters . append ( limit ) parameters . append ( start ) rows = db . get ( query , parameters ) for row in rows : log = {} log [ \"type\" ] = row [ 0 ] log [ \"origin\" ] = row [ 1 ] log [ \"message\" ] = row [ 2 ] log [ \"stack\" ] = row [ 3 ] log [ \"date\" ] = row [ 4 ] logs . append ( log ) return { 'total' : total , 'logs' : logs } Alpha Query from core import core DB = core . DB def get_logs ( start_date : datetime = None , end_date : datetime = None , limit : int = False , page : int = 0 , per_page : int = 100 , ): return DB . select ( Logs , optional_filters = [ { Logs . update_date : { \">\" : start_date }}, { Logs . update_date : { \"<\" : end_date }}, ], page = page , per_page = per_page , limit = limit , order_by = Logs . update_date . desc (), ) Backend: Alphaz Alphaz is a backend toolbox/framework based on a combination between Flask, SqlAlchemy and a multitude of other libraries. Note The overriding goal for Alphaz is to ease the backend development and easely link python backend to Angular frontend [Alphaa]. Features API Routing parameters management upgrade Enhanced json files configuration Tech Alphaz uses a number of open source projects to work properly: Flask - a micro web framework SqlAlchemy - a database toolkit Flask-SqlAlchemy - an extension for Flask that adds support for SQLAlchemy Project layout How to setup Alpha : Alpha Frontend: Alphaa Alphaa is a frontend toolbox/framework Note The overriding goal for Alphaa is to ease the frontend development and easely link Angular frontend to python backend [Alphaz]. Features Enhanced services Master class Project layout How to setup Alpha : Alpha",
+            "text": "Welcome to Alpha environment documention Alpha is an ecosystem based on a multiple frameworks and libraries for both frontend and backend . Purpose The purpose of the ecosystem is to simplify any dev activity. Standard query approach from core import core DB = core . db def get_logs ( start_date = None , end_date = None , useLimit = False , pageForLimit = 1 ): total = 0 logs = [] limit = 20 start = ( pageForLimit - 1 ) * limit query = \"SELECT COUNT(*) AS count FROM logs\" parameters = [] if start_date is not None and end_date is not None : query += \" AND CAST(date AS DATE) between %s and %s \" parameters . append ( start_date ) parameters . append ( end_date ) query += \" ORDER BY date DESC\" rows = DB . get ( query , parameters ) for row in rows : total = row [ 0 ] query = \"SELECT type, origin, message, stack, date FROM logs\" parameters = [] if start_date is not None and end_date is not None : query += \" AND CAST(date AS DATE) between %s and %s \" parameters . append ( start_date ) parameters . append ( end_date ) query += \" ORDER BY date DESC\" if useLimit : query += \" LIMIT %s OFFSET %s \" parameters . append ( limit ) parameters . append ( start ) rows = db . get ( query , parameters ) for row in rows : log = {} log [ \"type\" ] = row [ 0 ] log [ \"origin\" ] = row [ 1 ] log [ \"message\" ] = row [ 2 ] log [ \"stack\" ] = row [ 3 ] log [ \"date\" ] = row [ 4 ] logs . append ( log ) return { 'total' : total , 'logs' : logs } Alpha query approach from core import core DB = core . DB def get_logs ( start_date : datetime = None , end_date : datetime = None , limit : int = False , page : int = 0 , per_page : int = 100 , ): return DB . select ( Logs , optional_filters = [ { Logs . update_date : { \">\" : start_date }}, { Logs . update_date : { \"<\" : end_date }}, ], page = page , per_page = per_page , limit = limit , order_by = Logs . update_date . desc (), ) Backend: Alphaz Alphaz is a backend toolbox/framework based on a combination between Flask, SqlAlchemy and a multitude of other libraries. Note The overriding goal for Alphaz is to ease the backend development and easely link python backend to Angular frontend [Alphaa]. Features API Routing parameters management upgrade Enhanced json files configuration Tech Alphaz uses a number of open source projects to work properly: Flask - a micro web framework SqlAlchemy - a database toolkit Flask-SqlAlchemy - an extension for Flask that adds support for SQLAlchemy Project layout How to setup Alpha : Alpha Frontend: Alphaa Alphaa is a frontend toolbox/framework Note The overriding goal for Alphaa is to ease the frontend development and easely link Angular frontend to python backend [Alphaz]. Features Enhanced services Master class Project layout How to setup Alpha : Alpha",
             "title": "Home"
         },
         {
             "location": "#welcome-to-alpha-environment-documention",
-            "text": "Alpha is an ecosystem based on multiple frameworks and libraries for both frontend and backend .",
+            "text": "Alpha is an ecosystem based on a multiple frameworks and libraries for both frontend and backend .",
             "title": "Welcome to Alpha environment documention"
         },
         {
             "location": "#purpose",
-            "text": "The purpose of the ecosystem is to simplify any dev activity. Standard query from core import core DB = core . db def get_logs ( start_date = None , end_date = None , useLimit = False , pageForLimit = 1 ): total = 0 logs = [] limit = 20 start = ( pageForLimit - 1 ) * limit query = \"SELECT COUNT(*) AS count FROM logs\" parameters = [] if start_date is not None and end_date is not None : query += \" AND CAST(date AS DATE) between %s and %s \" parameters . append ( start_date ) parameters . append ( end_date ) query += \" ORDER BY date DESC\" rows = DB . get ( query , parameters ) for row in rows : total = row [ 0 ] query = \"SELECT type, origin, message, stack, date FROM logs\" parameters = [] if start_date is not None and end_date is not None : query += \" AND CAST(date AS DATE) between %s and %s \" parameters . append ( start_date ) parameters . append ( end_date ) query += \" ORDER BY date DESC\" if useLimit : query += \" LIMIT %s OFFSET %s \" parameters . append ( limit ) parameters . append ( start ) rows = db . get ( query , parameters ) for row in rows : log = {} log [ \"type\" ] = row [ 0 ] log [ \"origin\" ] = row [ 1 ] log [ \"message\" ] = row [ 2 ] log [ \"stack\" ] = row [ 3 ] log [ \"date\" ] = row [ 4 ] logs . append ( log ) return { 'total' : total , 'logs' : logs } Alpha Query from core import core DB = core . DB def get_logs ( start_date : datetime = None , end_date : datetime = None , limit : int = False , page : int = 0 , per_page : int = 100 , ): return DB . select ( Logs , optional_filters = [ { Logs . update_date : { \">\" : start_date }}, { Logs . update_date : { \"<\" : end_date }}, ], page = page , per_page = per_page , limit = limit , order_by = Logs . update_date . desc (), )",
+            "text": "The purpose of the ecosystem is to simplify any dev activity. Standard query approach from core import core DB = core . db def get_logs ( start_date = None , end_date = None , useLimit = False , pageForLimit = 1 ): total = 0 logs = [] limit = 20 start = ( pageForLimit - 1 ) * limit query = \"SELECT COUNT(*) AS count FROM logs\" parameters = [] if start_date is not None and end_date is not None : query += \" AND CAST(date AS DATE) between %s and %s \" parameters . append ( start_date ) parameters . append ( end_date ) query += \" ORDER BY date DESC\" rows = DB . get ( query , parameters ) for row in rows : total = row [ 0 ] query = \"SELECT type, origin, message, stack, date FROM logs\" parameters = [] if start_date is not None and end_date is not None : query += \" AND CAST(date AS DATE) between %s and %s \" parameters . append ( start_date ) parameters . append ( end_date ) query += \" ORDER BY date DESC\" if useLimit : query += \" LIMIT %s OFFSET %s \" parameters . append ( limit ) parameters . append ( start ) rows = db . get ( query , parameters ) for row in rows : log = {} log [ \"type\" ] = row [ 0 ] log [ \"origin\" ] = row [ 1 ] log [ \"message\" ] = row [ 2 ] log [ \"stack\" ] = row [ 3 ] log [ \"date\" ] = row [ 4 ] logs . append ( log ) return { 'total' : total , 'logs' : logs } Alpha query approach from core import core DB = core . DB def get_logs ( start_date : datetime = None , end_date : datetime = None , limit : int = False , page : int = 0 , per_page : int = 100 , ): return DB . select ( Logs , optional_filters = [ { Logs . update_date : { \">\" : start_date }}, { Logs . update_date : { \"<\" : end_date }}, ], page = page , per_page = per_page , limit = limit , order_by = Logs . update_date . desc (), )",
             "title": "Purpose"
         },
         {
             "location": "#backend-alphaz",
             "text": "Alphaz is a backend toolbox/framework based on a combination between Flask, SqlAlchemy and a multitude of other libraries. Note The overriding goal for Alphaz is to ease the backend development and easely link python backend to Angular frontend [Alphaa].",
             "title": "Backend: Alphaz"
         },
@@ -61,15 +61,15 @@
         {
             "location": "alpha_admin/",
             "text": "",
             "title": "Administration"
         },
         {
             "location": "alpha_api/",
-            "text": "Alpha API system Introduction The api system is completely based on Flask and compatible. You could use Flask inside Alpha system without any issue. Launch To start the api execute the api.py file python api.py Note set ALPHA_CONF environment parameter is you want to set the environment. Verify the deployment by navigating to your server address in your preferred browser: 127 .0.0.1:<port> How to use Your could import it using simply from the utils : from alphaz.utils.api import api or from the core if you are using it from core import core , API api / API is the equivalent for app in Flask framework. Configuration The api is automatically configured from the api.jon file. See Configuration for further details on how to use it. Main workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.databases\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false } Mails In order to specify the mails configurations \"mails\" : { \"mail_server\" : { \"host\" : \"\" , \"mail\" : \"\" , \"password\" : \"\" , \"port\" : 465 , \"server\" : \"\" , \"ssl\" : true , \"tls\" : false } } Auth In order to specify the auth mode \"auth\" : { \"mode\" : \"ldap\" , \"ldap\" : { \"server\" : \"ldap://path_to_ldap\" , \"baseDN\" : \"ou=people,dc=a_name,dc=com\" , \"users_filters\" : \"(|(uid={uid})(mail={mail})(cn={cn}))\" , \"user_filters\" : \"(|(uid={username})(mail={username})(cn={username}))\" , \"user_data\" : { \"givenName\" : \"name\" , \"sn\" : \"lastname\" , \"c\" : \"area\" , \"st-locationdescription\" : \"location\" , \"st-seatnumber\" : \"seat\" , \"telephoneNumber\" : \"phone-number\" } }, \"users\" : { \"a_user_name\" : { \"user_permissions\" : [ \"SUPER_USER\" ] } } }, Reloader type In order to specify the Werkzeug reloader type \"reloader_type\" : \"stat\" Admin In order to specify the admins configurations \"admins\" : { \"ips\" :[ \"127.0.0.1\" ], \"password\" : \"a_password\" }, Dashboard In order to configure the Flask-Monitoring Dashboard \"dashboard\" : { \"dashboard\" : { \"APP_VERSION\" : 1.0 , \"SAMPLING_PERIOD\" : 20 , \"ENABLE_LOGGING\" : true , \"active\" : false }, \"authentication\" : { \"USERNAME\" : \"username\" , \"PASSWORD\" : \"\" , \"GUEST_USERNAME\" : \"guest\" , \"GUEST_PASSWORD\" : [ \"guest1\" , \"guest2\" ], \"SECURITY_TOKEN\" : \"a_security_token\" }, \"database\" : { \"DATABASE\" : \"sqlite:///{{root}}/dashboard.db\" } } Routes Basic To specify an api route, juste use the route flag: from alphaz.utils.api import route , api , Parameter @route ( \"route_name\" ) def method_name (): return \"hello\" Method automatically convert the output to the right format. Default format is json Description A description could be specified: @route ( \"route_name\" , description = \"This route say hello\" ) def method_name (): return \"hello\" Category The routes are organized by category , by default the route category is defined by it file name , but it could be specified using the cat parameter: @route ( \"route_name\" , category = \"politeness\" ) def method_name (): return \"hello\" Parameters Simple You could simply define parameters by listing all parameters in parameters list: from alphaz.utils.api import route , api , Parameter @route ( \"books\" , parameters = [ \"name\" ]) def method_name (): return \"Book name is %s or %s \" % ( api [ \"name\" ], api . get ( \"name\" , default = \"\" )) Parameter value is accessed by api instance, using get method, they could also be accessed using get_parameters method from api instance. Object Or you could use the Parameter class to specify properties such as: ptype : value type int, str, bool, SqlAlchemy model parameter is automatically converted to the specified type if conversion failed an exception is raised required : the parameter is required or not default : default parameter value options : authorized values mode : input mode cacheable : parameter is taken into acount in the caching system or not private : parameter is hiden from documentation or not @route ( \"/logs\" , parameters = [ Parameter ( 'page' , required = True , ptype = int ), Parameter ( 'startDate' , required = True ), Parameter ( 'endDate' , default = None ), Parameter ( 'error' , options = [ \"Y\" , \"N\" ]) ]) def admin_logs (): return get_logs ( ** api . get_parameters ()) Promote this method as it allows a better control on parameters Default parameters Some parameter are always available: - no_log (bool): disable logs for this route - reset_cache (bool): reset cache before calling this route - requester (str): requester to this route - format (str): output format - json: - xml: - admin (str): admin password - admin_user_id (int): id of the user to connect has an admin SqlAlchemy model If you specify a SqlAlchemy model as a type it will be automatically converted to the specified model. from core import core db = core . db class Logs ( db . Model , AlphaTable ): __tablename__ = 'LOGS' id = AlphaColumn ( Integer , nullable = False , primary_key = True ) name = AlphaColumn ( String , nullable = False ) @route ( \"logs\" , parameters = [ Parameter ( 'log' , ptype = Logs ) ]) def admin_logs (): db . add ( api [ 'log' ]) Methods Methods are specified the same way as in Flask , using methods parameter: @route ( 'logs' , methods = [ \"GET\" ]) def get_logs (): return db . select ( Logs ) @route ( 'logs' , methods = [ \"POST\" ]) def set_logs (): return db . add ( Logs ) Methods can be managed using different routes or within a single route : @route ( 'logs' , methods = [ \"GET\" , \"POST\" , \"DELETE\" ]) def get_logs (): if api . is_get (): return db . select ( Logs ) elif api . is_post (): return db . add ( Logs ) elif api . is_delete (): return db . delete ( Logs ) Authorizations Route can be protected using the login system or admin rights. Login system To protect a route using the login system you must specify: logged=True @route ( 'protected' , logged = True ) def protected_route (): user = api . get_logged_user () return user User information can be accessed using get_logged_user method. Cache A cache system is implemented, in order to use it you must specify the Admin Admin could auto log to any user account on local mode Condition To be an admin a user must have at least one condition: a role > 9 specify the magic password has admin API parameter connect using an admin ip. The ips admin list must be defined in the api.json configuration files under the key = admins_ips How to use If you met one of the admin condition you do not need any password in order to log has any of the user in the database. You could be logged for specific routes using the single route mode or to any route using the login/logout system. Single route mode You could specifiy either admin_user_id={user_id} or admin_user_name={username} directly into any request in order to login with this user for this specific route. Exemple /anyroute?admin_user_id=1000 Login to the api Use the route /auth/su in order to set an admin session that is valid until the end of the api runtime. You must specifiy either admin_user_id={user_id} or admin_user_name={username} Exemple /auth/su?admin_user_id=1000 Logout from the api Use the route /logout/su in order to logout. Issues In progress Database alias In progress",
+            "text": "Alpha API system Introduction The api system is completely based on Flask and compatible. You could use Flask inside Alpha system without any issue. Launch To start the api execute the api.py file python api.py Note set ALPHA_CONF environment parameter is you want to set the environment. Verify the deployment by navigating to your server address in your preferred browser: 127 .0.0.1:<port> How to use Your could import it using simply from the utils : from alphaz.utils.api import api or from the core if you are using it from core import core , API api / API is the equivalent for app in Flask framework. Routes We recommend to add all the route definition in apis/routes folder and import all the route definition in apis/routes/ init .py . Then you will have to import the route in thoe core.py file: from alphaz.models.main import AlphaCore , singleton @singleton class Core ( AlphaCore ): def __init__ ( self , file : str ): super () . __init__ ( file ) core = Core ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded from apis.routes import * Configuration The api is automatically configured from the api.jon file. See Configuration for further details on how to use it. Main workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.databases\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false } Mails In order to specify the mails configurations \"mails\" : { \"mail_server\" : { \"host\" : \"\" , \"mail\" : \"\" , \"password\" : \"\" , \"port\" : 465 , \"server\" : \"\" , \"ssl\" : true , \"tls\" : false } } Auth In order to specify the auth mode \"auth\" : { \"mode\" : \"ldap\" , \"ldap\" : { \"server\" : \"ldap://path_to_ldap\" , \"baseDN\" : \"ou=people,dc=a_name,dc=com\" , \"users_filters\" : \"(|(uid={uid})(mail={mail})(cn={cn}))\" , \"user_filters\" : \"(|(uid={username})(mail={username})(cn={username}))\" , \"user_data\" : { \"givenName\" : \"name\" , \"sn\" : \"lastname\" , \"c\" : \"area\" , \"st-locationdescription\" : \"location\" , \"st-seatnumber\" : \"seat\" , \"telephoneNumber\" : \"phone-number\" } }, \"users\" : { \"a_user_name\" : { \"user_permissions\" : [ \"SUPER_USER\" ] } } }, Reloader type In order to specify the Werkzeug reloader type \"reloader_type\" : \"stat\" Admin In order to specify the admins configurations \"admins\" : { \"ips\" :[ \"127.0.0.1\" ], \"password\" : \"a_password\" }, Dashboard In order to configure the Flask-Monitoring Dashboard \"dashboard\" : { \"dashboard\" : { \"APP_VERSION\" : 1.0 , \"SAMPLING_PERIOD\" : 20 , \"ENABLE_LOGGING\" : true , \"active\" : false }, \"authentication\" : { \"USERNAME\" : \"username\" , \"PASSWORD\" : \"\" , \"GUEST_USERNAME\" : \"guest\" , \"GUEST_PASSWORD\" : [ \"guest1\" , \"guest2\" ], \"SECURITY_TOKEN\" : \"a_security_token\" }, \"database\" : { \"DATABASE\" : \"sqlite:///{{root}}/dashboard.db\" } } Routes Basic To specify an api route, juste use the route flag: from alphaz.utils.api import route , api , Parameter @route ( \"route_name\" ) def method_name (): return \"hello\" Method automatically convert the output to the right format. Default format is json Description A description could be specified: @route ( \"route_name\" , description = \"This route say hello\" ) def method_name (): return \"hello\" Category The routes are organized by category , by default the route category is defined by it file name , but it could be specified using the cat parameter: @route ( \"route_name\" , category = \"politeness\" ) def method_name (): return \"hello\" Parameters Simple You could simply define parameters by listing all parameters in parameters list: from alphaz.utils.api import route , api , Parameter @route ( \"books\" , parameters = [ \"name\" ]) def method_name (): return \"Book name is %s or %s \" % ( api [ \"name\" ], api . get ( \"name\" , default = \"\" )) Parameter value is accessed by api instance, using get method, they could also be accessed using get_parameters method from api instance. Object Or you could use the Parameter class to specify properties such as: ptype : value type int, str, bool, SqlAlchemy model parameter is automatically converted to the specified type if conversion failed an exception is raised required : the parameter is required or not default : default parameter value options : authorized values mode : input mode cacheable : parameter is taken into acount in the caching system or not private : parameter is hiden from documentation or not @route ( \"/logs\" , parameters = [ Parameter ( 'page' , required = True , ptype = int ), Parameter ( 'startDate' , required = True ), Parameter ( 'endDate' , default = None ), Parameter ( 'error' , options = [ \"Y\" , \"N\" ]) ]) def admin_logs (): return get_logs ( ** api . get_parameters ()) Promote this method as it allows a better control on parameters Default parameters Some parameter are always available: - no_log (bool): disable logs for this route - reset_cache (bool): reset cache before calling this route - requester (str): requester to this route - format (str): output format - json: - xml: - admin (str): admin password - admin_user_id (int): id of the user to connect has an admin SqlAlchemy model If you specify a SqlAlchemy model as a type it will be automatically converted to the specified model. from core import core db = core . db class Logs ( db . Model , AlphaTable ): __tablename__ = 'LOGS' id = AlphaColumn ( Integer , nullable = False , primary_key = True ) name = AlphaColumn ( String , nullable = False ) @route ( \"logs\" , parameters = [ Parameter ( 'log' , ptype = Logs ) ]) def admin_logs (): db . add ( api [ 'log' ]) Methods Methods are specified the same way as in Flask , using methods parameter: @route ( 'logs' , methods = [ \"GET\" ]) def get_logs (): return db . select ( Logs ) @route ( 'logs' , methods = [ \"POST\" ]) def set_logs (): return db . add ( Logs ) Methods can be managed using different routes or within a single route : @route ( 'logs' , methods = [ \"GET\" , \"POST\" , \"DELETE\" ]) def get_logs (): if api . is_get (): return db . select ( Logs ) elif api . is_post (): return db . add ( Logs ) elif api . is_delete (): return db . delete ( Logs ) Authorizations Route can be protected using the login system or admin rights. Login system To protect a route using the login system you must specify: logged=True @route ( 'protected' , logged = True ) def protected_route (): user = api . get_logged_user () return user User information can be accessed using get_logged_user method. Cache A cache system is implemented, in order to use it you must specify the Admin Admin could auto log to any user account on local mode Condition To be an admin a user must have at least one condition: a role > 9 specify the magic password has admin API parameter connect using an admin ip. The ips admin list must be defined in the api.json configuration files under the key = admins_ips How to use If you met one of the admin condition you do not need any password in order to log has any of the user in the database. You could be logged for specific routes using the single route mode or to any route using the login/logout system. Single route mode You could specifiy either admin_user_id={user_id} or admin_user_name={username} directly into any request in order to login with this user for this specific route. Exemple /anyroute?admin_user_id=1000 Login to the api Use the route /auth/su in order to set an admin session that is valid until the end of the api runtime. You must specifiy either admin_user_id={user_id} or admin_user_name={username} Exemple /auth/su?admin_user_id=1000 Logout from the api Use the route /logout/su in order to logout. Issues In progress Database alias In progress",
             "title": "Api"
         },
         {
             "location": "alpha_api/#alpha-api-system",
             "text": "",
             "title": "Alpha API system"
         },
@@ -85,14 +85,19 @@
         },
         {
             "location": "alpha_api/#how-to-use",
             "text": "Your could import it using simply from the utils : from alphaz.utils.api import api or from the core if you are using it from core import core , API api / API is the equivalent for app in Flask framework.",
             "title": "How to use"
         },
         {
+            "location": "alpha_api/#routes",
+            "text": "We recommend to add all the route definition in apis/routes folder and import all the route definition in apis/routes/ init .py . Then you will have to import the route in thoe core.py file: from alphaz.models.main import AlphaCore , singleton @singleton class Core ( AlphaCore ): def __init__ ( self , file : str ): super () . __init__ ( file ) core = Core ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded from apis.routes import *",
+            "title": "Routes"
+        },
+        {
             "location": "alpha_api/#configuration",
             "text": "The api is automatically configured from the api.jon file. See Configuration for further details on how to use it.",
             "title": "Configuration"
         },
         {
             "location": "alpha_api/#main",
             "text": "workers: In order to specify the numbers of workers \"workers\" : 6 routes_no_log: In order to specify the routes where log must be ignored \"routes_no_log\" : [ \"//status\" , \"//static\" , \"//dashboard\" ], models: In order to specify the Flask-SqlAlchemy models definitions paths \"models\" : [ \"models.databases\" ] routes: In order to specify the routes definitions paths \"routes\" : [ \"apis.routes\" ] ssl: In order to activate ssl mode \"ssl\" : false threaded: In order to activate the threaded mode \"threaded\" : false config: In order to activate pass configuration to Flask api class \"config\" : { \"MYSQL_DATABASE_CHARSET\" : \"utf8mb4\" , \"SQLALCHEMY_TRACK_MODIFICATIONS\" : false , \"SQLALCHEMY_POOL_RECYCLE\" : 299 , \"SQLALCHEMY_POOL_TIMEOUT\" : 30 , \"SQLALCHEMY_POOL_SIZE\" : 10 , \"JWT_SECRET_KEY\" : \"a_secret_key\" , \"JSON_SORT_KEYS\" : false }",
@@ -120,15 +125,15 @@
         },
         {
             "location": "alpha_api/#dashboard",
             "text": "In order to configure the Flask-Monitoring Dashboard \"dashboard\" : { \"dashboard\" : { \"APP_VERSION\" : 1.0 , \"SAMPLING_PERIOD\" : 20 , \"ENABLE_LOGGING\" : true , \"active\" : false }, \"authentication\" : { \"USERNAME\" : \"username\" , \"PASSWORD\" : \"\" , \"GUEST_USERNAME\" : \"guest\" , \"GUEST_PASSWORD\" : [ \"guest1\" , \"guest2\" ], \"SECURITY_TOKEN\" : \"a_security_token\" }, \"database\" : { \"DATABASE\" : \"sqlite:///{{root}}/dashboard.db\" } }",
             "title": "Dashboard"
         },
         {
-            "location": "alpha_api/#routes",
+            "location": "alpha_api/#routes_1",
             "text": "",
             "title": "Routes"
         },
         {
             "location": "alpha_api/#basic",
             "text": "To specify an api route, juste use the route flag: from alphaz.utils.api import route , api , Parameter @route ( \"route_name\" ) def method_name (): return \"hello\" Method automatically convert the output to the right format. Default format is json",
             "title": "Basic"
@@ -226,30 +231,30 @@
         {
             "location": "alpha_api/#database-alias",
             "text": "In progress",
             "title": "Database alias"
         },
         {
             "location": "alpha_core/",
-            "text": "Alpha core system Purpose The core is used as a central point to manage various system: - logging system - database access - api system - dynamic configuration How to use You could: Use the alphaz core and initiate it at the start of you project: from alphaz.models.main import AlphaCore core = AlphaCore ( __file__ ) DB = core . db # not required but recommanded Or create a core.py file at the root of your project containing at least: from alphaz.models.main import AlphaCore , singleton @singleton class Core ( AlphaCore ): def __init__ ( self , file : str ): super () . __init__ ( file ) core = Core ( __file__ ) DB = core . db # not required but recommanded Note This is the recommended way, so that you could custom the Core class Logging from core import core LOG = core . get_logger ( 'name' ) LOG . info ( 'message' ) Database from core import core DB = core . db API from core import core API = core . api Configuration from core import core CONFIG = core . config tmp_directory_path = CONFIG . get ( 'directories/tmp' )",
+            "text": "Alpha core system Purpose The core is used as a central point to manage various system: logging system database access api system dynamic configuration How to use You could: Use the alphaz core and initiate it at the start of you project preferably in a file named core.py to be complient with this documentation: from alphaz.models.main import AlphaCore core = AlphaCore ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded Or create a core.py file at the root of your project containing at least: from alphaz.models.main import AlphaCore , singleton @singleton class Core ( AlphaCore ): def __init__ ( self , file : str ): super () . __init__ ( file ) core = Core ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded Note This is the recommended way, so that you could custom the Core class Logging from core import core LOG = core . get_logger ( 'name' ) LOG . info ( 'message' ) Database from core import core DB = core . db API from core import core API = core . api Configuration from core import core CONFIG = core . config tmp_directory_path = CONFIG . get ( 'directories/tmp' )",
             "title": "Core"
         },
         {
             "location": "alpha_core/#alpha-core-system",
             "text": "",
             "title": "Alpha core system"
         },
         {
             "location": "alpha_core/#purpose",
-            "text": "The core is used as a central point to manage various system: - logging system - database access - api system - dynamic configuration",
+            "text": "The core is used as a central point to manage various system: logging system database access api system dynamic configuration",
             "title": "Purpose"
         },
         {
             "location": "alpha_core/#how-to-use",
-            "text": "You could: Use the alphaz core and initiate it at the start of you project: from alphaz.models.main import AlphaCore core = AlphaCore ( __file__ ) DB = core . db # not required but recommanded Or create a core.py file at the root of your project containing at least: from alphaz.models.main import AlphaCore , singleton @singleton class Core ( AlphaCore ): def __init__ ( self , file : str ): super () . __init__ ( file ) core = Core ( __file__ ) DB = core . db # not required but recommanded Note This is the recommended way, so that you could custom the Core class",
+            "text": "You could: Use the alphaz core and initiate it at the start of you project preferably in a file named core.py to be complient with this documentation: from alphaz.models.main import AlphaCore core = AlphaCore ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded Or create a core.py file at the root of your project containing at least: from alphaz.models.main import AlphaCore , singleton @singleton class Core ( AlphaCore ): def __init__ ( self , file : str ): super () . __init__ ( file ) core = Core ( __file__ ) DB , API , LOG = core . db , core . api , core . log # not required but recommanded Note This is the recommended way, so that you could custom the Core class",
             "title": "How to use"
         },
         {
             "location": "alpha_core/#logging",
             "text": "from core import core LOG = core . get_logger ( 'name' ) LOG . info ( 'message' )",
             "title": "Logging"
         },
@@ -371,30 +376,30 @@
         {
             "location": "alpha_screens/#help",
             "text": "python -m alphaz.utils.screens",
             "title": "Help"
         },
         {
             "location": "alpha_setup/",
-            "text": "Alpha system OS configuration Important make sure that Git is well configured. Python Python 3.10.4 is required. Anaconda or Miniconda could be used. There is no constraint but the usual structure is to have: a user per configuration ( mes , mesacc , mesint and mesdev for exemple) three location per user: /home/USER/APP_NAME for sources /home/USER/configs for configurations /application/USER/APP_NAME for tmp files and logs Note This is configured within the conf.json file and could be modified Setup If you just want to use the system go for the classic way and if you want to modify it use the sources integration. Classic The default installation procedure is: pip install alphaz It will install all the dependencies automatically. Using sources If you want to edit the sources you could use this procedure to clone the sources and configure it as a sub module Clone alphaz from the repository https://github.com/ZAurele/alphaz.git cd <your_project_repository> git clone https://github.com/ZAurele/alphaz.git Launch the setup, it will install all the dependencies and other magical actions. python setup.py Define it as a submodule in your project Dependencies Main dependencies are automatically installed, however if you need specific ones, you will have to install them manually Oracle Oracle client Configuration Angular { \"compilerOptions\" : { \"baseUrl\" : \"./src\" , \"paths\" : { \"@services/*\" : [ \"app/services/*\" , \"src/app/services/*\" ], \"@views/*\" : [ \"app/views/*\" , \"src/app/views/*\" ], \"@models/*\" : [ \"app/models/*\" , \"src/app/models/*\" ], \"@components/*\" : [ \"app/components/*\" , \"src/app/components/*\" ], \"@alphaa/*\" : [ \"alphaa/*\" , \"src/alphaa/*\" ], \"@layout/*\" : [ \"app/layout/*\" , \"src/app/layout/*\" ], \"@envs/*\" : [ \"environments/*\" , \"src/environments/*\" ], \"@constants/*\" : [ \"app/constants/*\" , \"src/app/constants/*\" ] } } }",
+            "text": "Alpha system OS configuration Important make sure that Git is well configured. Python Python 3.10.4 is required. Anaconda or Miniconda could be used. There is no constraint but the usual structure is to have: a user per configuration ( mes , mesacc , mesint and mesdev for exemple) three location per user: /application/USER/APP_NAME for sources /home/USER/configs for configurations /application/USER/APP_NAME for tmp files and logs Note This is configured within the conf.json file and could be modified Setup If you just want to use the system go for the classic way and if you want to modify it use the sources integration. Classic The default installation procedure is: pip install alphaz It will install all the dependencies automatically. Using sources If you want to edit the sources you could use this procedure to clone the sources and configure it as a sub module Clone alphaz from the repository https://github.com/ZAurele/alphaz.git cd <your_project_repository> git clone https://github.com/ZAurele/alphaz.git Launch the setup, it will install all the dependencies and other magical actions. python setup.py Define it as a submodule in your project Dependencies Main dependencies are automatically installed, however if you need specific ones, you will have to install them manually Oracle Oracle client Configuration Angular { \"compilerOptions\" : { \"baseUrl\" : \"./src\" , \"paths\" : { \"@services/*\" : [ \"app/services/*\" , \"src/app/services/*\" ], \"@views/*\" : [ \"app/views/*\" , \"src/app/views/*\" ], \"@models/*\" : [ \"app/models/*\" , \"src/app/models/*\" ], \"@components/*\" : [ \"app/components/*\" , \"src/app/components/*\" ], \"@alphaa/*\" : [ \"alphaa/*\" , \"src/alphaa/*\" ], \"@layout/*\" : [ \"app/layout/*\" , \"src/app/layout/*\" ], \"@envs/*\" : [ \"environments/*\" , \"src/environments/*\" ], \"@constants/*\" : [ \"app/constants/*\" , \"src/app/constants/*\" ] } } }",
             "title": "Setup"
         },
         {
             "location": "alpha_setup/#alpha-system",
             "text": "",
             "title": "Alpha system"
         },
         {
             "location": "alpha_setup/#os-configuration",
             "text": "Important make sure that Git is well configured.",
             "title": "OS configuration"
         },
         {
             "location": "alpha_setup/#python",
-            "text": "Python 3.10.4 is required. Anaconda or Miniconda could be used. There is no constraint but the usual structure is to have: a user per configuration ( mes , mesacc , mesint and mesdev for exemple) three location per user: /home/USER/APP_NAME for sources /home/USER/configs for configurations /application/USER/APP_NAME for tmp files and logs Note This is configured within the conf.json file and could be modified",
+            "text": "Python 3.10.4 is required. Anaconda or Miniconda could be used. There is no constraint but the usual structure is to have: a user per configuration ( mes , mesacc , mesint and mesdev for exemple) three location per user: /application/USER/APP_NAME for sources /home/USER/configs for configurations /application/USER/APP_NAME for tmp files and logs Note This is configured within the conf.json file and could be modified",
             "title": "Python"
         },
         {
             "location": "alpha_setup/#setup",
             "text": "If you just want to use the system go for the classic way and if you want to modify it use the sources integration.",
             "title": "Setup"
         },
```

### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.3.9/alphaz/documentations/site/sitemap.xml`

 * *Files 3% similar despite different names*

#### Comparing `alphaz-0.7.3.8/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.3.9/alphaz/documentations/site/sitemap.xml`

```diff
@@ -1,48 +1,48 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-11</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-11</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-11</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-11</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-11</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-11</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-11</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-11</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>None</loc>
-    <lastmod>2023-04-11</lastmod>
+    <lastmod>2023-04-12</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `alphaz-0.7.3.8/alphaz/index.html` & `alphaz-0.7.3.9/alphaz/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/api_lib.py` & `alphaz-0.7.3.9/alphaz/libs/api_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/barcode_lib.py` & `alphaz-0.7.3.9/alphaz/libs/barcode_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/config_lib.py` & `alphaz-0.7.3.9/alphaz/libs/config_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/converter_lib.py` & `alphaz-0.7.3.9/alphaz/libs/converter_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/database_lib.py` & `alphaz-0.7.3.9/alphaz/libs/database_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/date_lib.py` & `alphaz-0.7.3.9/alphaz/libs/date_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/dict_lib.py` & `alphaz-0.7.3.9/alphaz/libs/dict_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/emulation/vt102_lib.py` & `alphaz-0.7.3.9/alphaz/libs/emulation/vt102_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/events.py` & `alphaz-0.7.3.9/alphaz/libs/events.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/files_lib.py` & `alphaz-0.7.3.9/alphaz/libs/files_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/flask_lib.py` & `alphaz-0.7.3.9/alphaz/libs/flask_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/img_lib.py` & `alphaz-0.7.3.9/alphaz/libs/img_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/io_lib.py` & `alphaz-0.7.3.9/alphaz/libs/io_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/json_lib.py` & `alphaz-0.7.3.9/alphaz/libs/json_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/logs_lib.py` & `alphaz-0.7.3.9/alphaz/libs/logs_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/mail_lib.py` & `alphaz-0.7.3.9/alphaz/libs/mail_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/notifications_lib.py` & `alphaz-0.7.3.9/alphaz/libs/notifications_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/number_lib.py` & `alphaz-0.7.3.9/alphaz/libs/number_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/process_lib.py` & `alphaz-0.7.3.9/alphaz/libs/process_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/py_lib.py` & `alphaz-0.7.3.9/alphaz/libs/py_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/scp_lib.py` & `alphaz-0.7.3.9/alphaz/libs/scp_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/search_lib.py` & `alphaz-0.7.3.9/alphaz/libs/search_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/secure_lib.py` & `alphaz-0.7.3.9/alphaz/libs/secure_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/soap_lib.py` & `alphaz-0.7.3.9/alphaz/libs/soap_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/ssh_lib.py` & `alphaz-0.7.3.9/alphaz/libs/ssh_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/string_lib.py` & `alphaz-0.7.3.9/alphaz/libs/string_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/test_lib.py` & `alphaz-0.7.3.9/alphaz/libs/test_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/time_lib.py` & `alphaz-0.7.3.9/alphaz/libs/time_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/transactions_lib.py` & `alphaz-0.7.3.9/alphaz/libs/transactions_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/user_lib.py` & `alphaz-0.7.3.9/alphaz/libs/user_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/user_management/application_management_lib.py` & `alphaz-0.7.3.9/alphaz/libs/user_management/application_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/user_management/permission_management_lib.py` & `alphaz-0.7.3.9/alphaz/libs/user_management/permission_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/user_management/role_management_lib.py` & `alphaz-0.7.3.9/alphaz/libs/user_management/role_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/libs/user_management/user_management_lib.py` & `alphaz-0.7.3.9/alphaz/libs/user_management/user_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/mails/Images/Background.png` & `alphaz-0.7.3.9/alphaz/mails/Images/Background.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/mails/Images/Facebook_logo.png` & `alphaz-0.7.3.9/alphaz/mails/Images/Facebook_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/mails/Images/Twitter_logo.png` & `alphaz-0.7.3.9/alphaz/mails/Images/Twitter_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/mails/Images/Web_logo.png` & `alphaz-0.7.3.9/alphaz/mails/Images/Web_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/mails/Mail.png` & `alphaz-0.7.3.9/alphaz/mails/Mail.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/mails/Webmail.html` & `alphaz-0.7.3.9/alphaz/mails/Webmail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/mails/debug.html` & `alphaz-0.7.3.9/alphaz/mails/debug.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/mails/mail.html` & `alphaz-0.7.3.9/alphaz/mails/mail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/mails/password_reset.html` & `alphaz-0.7.3.9/alphaz/mails/password_reset.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/mails/stay_in_touch.html` & `alphaz-0.7.3.9/alphaz/mails/stay_in_touch.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/api/_answer.py` & `alphaz-0.7.3.9/alphaz/models/api/_answer.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/api/_colorations.py` & `alphaz-0.7.3.9/alphaz/models/api/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/api/_parameter.py` & `alphaz-0.7.3.9/alphaz/models/api/_parameter.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/api/_requests.py` & `alphaz-0.7.3.9/alphaz/models/api/_requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/api/_route.py` & `alphaz-0.7.3.9/alphaz/models/api/_route.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/api/_structures.py` & `alphaz-0.7.3.9/alphaz/models/api/_structures.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/api/_utils.py` & `alphaz-0.7.3.9/alphaz/models/api/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/config/_config.py` & `alphaz-0.7.3.9/alphaz/models/config/_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/config/_utils.py` & `alphaz-0.7.3.9/alphaz/models/config/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/database/main_definitions.py` & `alphaz-0.7.3.9/alphaz/models/database/main_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/database/models.py` & `alphaz-0.7.3.9/alphaz/models/database/models.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/database/operators.py` & `alphaz-0.7.3.9/alphaz/models/database/operators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/database/requests.py` & `alphaz-0.7.3.9/alphaz/models/database/requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/database/row.py` & `alphaz-0.7.3.9/alphaz/models/database/row.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/database/structure.py` & `alphaz-0.7.3.9/alphaz/models/database/structure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/database/tests.py` & `alphaz-0.7.3.9/alphaz/models/database/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/database/users_definitions.py` & `alphaz-0.7.3.9/alphaz/models/database/users_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/database/utils.py` & `alphaz-0.7.3.9/alphaz/models/database/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/database/views.py` & `alphaz-0.7.3.9/alphaz/models/database/views.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/excel.py` & `alphaz-0.7.3.9/alphaz/models/excel.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/ftp.py` & `alphaz-0.7.3.9/alphaz/models/ftp.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/json/_converters.py` & `alphaz-0.7.3.9/alphaz/models/json/_converters.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/logger/_colorations.py` & `alphaz-0.7.3.9/alphaz/models/logger/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/logger/_logger.py` & `alphaz-0.7.3.9/alphaz/models/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/logger/_utils.py` & `alphaz-0.7.3.9/alphaz/models/logger/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/logs/main.log` & `alphaz-0.7.3.9/alphaz/models/logs/main.log`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/main/_base.py` & `alphaz-0.7.3.9/alphaz/models/main/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses, traceback
 import enum, inspect, operator, re, copy
-from dataclasses import dataclass, field, is_dataclass, _MISSING_TYPE
+from dataclasses import dataclass, field, is_dataclass, _MISSING_TYPE, asdict
 from collections import OrderedDict
 
 from typing import Dict, Iterable, List, Optional, Tuple
 from typing_extensions import Annotated
 
 from ..logger import AlphaLogger
 from ...libs import py_lib, json_lib, string_lib
@@ -478,15 +478,19 @@
         return field_values
 
 
 def convert_value_from_field(field_type, value, automap: bool = False):
     if value is None:
         return None
     if is_dataclass(field_type):
-        return field_type.map_from_dict(value, automap=automap)
+        return field_type.map_from_dict(
+            asdict(value) if is_dataclass(value) else value, automap=automap
+        )
+    elif isinstance(value, list) and all(isinstance(item, dict) for item in value):
+        return [convert_value_from_field(field_type, item) for item in value]
     else:
         try:
             return field_type(value)
         except:
             return value
 
 
@@ -653,16 +657,28 @@
                     else:
                         output[value_key].append(el)
             else:
                 output[value_key] = value
         return output
 
     @classmethod
-    def get_fields_names(dataclass_type):
-        return [f.name for f in dataclasses.fields(dataclass_type)]
+    def get_fields_names(dataclass_type, init_only: bool = False):
+        return [
+            f.name
+            for f in dataclasses.fields(dataclass_type)
+            if (init_only and f.init) or not init_only
+        ]
+
+    @classmethod
+    def get_fields(dataclass_type, init_only: bool = False):
+        return [
+            f
+            for f in dataclasses.fields(dataclass_type)
+            if (init_only and f.init) or not init_only
+        ]
 
     @classmethod
     def auto_map_from_dict(
         dataclass_type,
         dict_values: Dict[str, object],
         associations: Dict[str, str] = {},
         no_match: List[str] = [],
@@ -692,15 +708,23 @@
         ]
         is_required_fields = set(required_fields).intersection(
             fields_values.keys()
         ) == set(required_fields)
         if not is_required_fields:
             return None
         try:
-            instance = dataclass_type(**fields_values)
+            if False and hasattr(dataclass_type, "map_from_dict"):
+                instance = dataclass_type.map_from_dict(fields_values)
+            else:
+                fields_values = {
+                    x: y
+                    for x, y in fields_values.items()
+                    if x in dataclass_type.get_fields_names(True)
+                }
+                instance = dataclass_type(**fields_values)
         except Exception as ex:
             print(f"Error mapping {dataclass_type}")
             tb = traceback.format_exc()
             raise ex
         return instance
 
     @classmethod
```

### Comparing `alphaz-0.7.3.8/alphaz/models/main/_core/_core.py` & `alphaz-0.7.3.9/alphaz/models/main/_core/_core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/main/_exception.py` & `alphaz-0.7.3.9/alphaz/models/main/_exception.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/main/_request.py` & `alphaz-0.7.3.9/alphaz/models/main/_request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/main/_singleton.py` & `alphaz-0.7.3.9/alphaz/models/main/_singleton.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/request.py` & `alphaz-0.7.3.9/alphaz/models/request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/tests/_category.py` & `alphaz-0.7.3.9/alphaz/models/tests/_category.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/tests/_group.py` & `alphaz-0.7.3.9/alphaz/models/tests/_group.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/tests/_method.py` & `alphaz-0.7.3.9/alphaz/models/tests/_method.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/tests/_save.py` & `alphaz-0.7.3.9/alphaz/models/tests/_save.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/tests/_test.py` & `alphaz-0.7.3.9/alphaz/models/tests/_test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/tests/_wrappers.py` & `alphaz-0.7.3.9/alphaz/models/tests/_wrappers.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/user.py` & `alphaz-0.7.3.9/alphaz/models/user.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/models/watcher.py` & `alphaz-0.7.3.9/alphaz/models/watcher.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/pocs/main.py` & `alphaz-0.7.3.9/alphaz/pocs/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/run.py` & `alphaz-0.7.3.9/alphaz/run.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/src/alpha.png` & `alphaz-0.7.3.9/alphaz/src/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/src/configs/loggers.json` & `alphaz-0.7.3.9/alphaz/src/configs/loggers.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/stitch/Core.py` & `alphaz-0.7.3.9/alphaz/stitch/Core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/stitch/stitch.py` & `alphaz-0.7.3.9/alphaz/stitch/stitch.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/stitch/web-drivers/chromedriver.exe` & `alphaz-0.7.3.9/alphaz/stitch/web-drivers/chromedriver.exe`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/stitch/web-drivers/geckodriver` & `alphaz-0.7.3.9/alphaz/stitch/web-drivers/geckodriver`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/assets/css/home.css` & `alphaz-0.7.3.9/alphaz/templates/assets/css/home.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/assets/css/logs.css` & `alphaz-0.7.3.9/alphaz/templates/assets/css/logs.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/assets/images/icons/alpha.png` & `alphaz-0.7.3.9/alphaz/templates/assets/images/icons/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/assets/images/icons/start-icon.png` & `alphaz-0.7.3.9/alphaz/templates/assets/images/icons/start-icon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/assets/images/icons/wsalpha.png` & `alphaz-0.7.3.9/alphaz/templates/assets/images/icons/wsalpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/assets/images/loading.gif` & `alphaz-0.7.3.9/alphaz/templates/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/assets/js/libs/ansi_up.js` & `alphaz-0.7.3.9/alphaz/templates/assets/js/libs/ansi_up.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/assets/js/libs/jquery.min.js` & `alphaz-0.7.3.9/alphaz/templates/assets/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/assets/js/logs.js` & `alphaz-0.7.3.9/alphaz/templates/assets/js/logs.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/home.html` & `alphaz-0.7.3.9/alphaz/templates/home.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/templates/logs.html` & `alphaz-0.7.3.9/alphaz/templates/logs.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/test.py` & `alphaz-0.7.3.9/alphaz/test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/tests/api.py` & `alphaz-0.7.3.9/alphaz/tests/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/tests/basic_test.py` & `alphaz-0.7.3.9/alphaz/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/tests/configurations.py` & `alphaz-0.7.3.9/alphaz/tests/configurations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/tests/database.py` & `alphaz-0.7.3.9/alphaz/tests/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/tests/utils.py` & `alphaz-0.7.3.9/alphaz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/api.py` & `alphaz-0.7.3.9/alphaz/utils/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/configuration.py` & `alphaz-0.7.3.9/alphaz/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/database_to_dataclass.py` & `alphaz-0.7.3.9/alphaz/utils/database_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/decorators.py` & `alphaz-0.7.3.9/alphaz/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/ensure.py` & `alphaz-0.7.3.9/alphaz/utils/ensure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/mep.py` & `alphaz-0.7.3.9/alphaz/utils/mep.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/screens.py` & `alphaz-0.7.3.9/alphaz/utils/screens.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/selectionMenu.py` & `alphaz-0.7.3.9/alphaz/utils/selectionMenu.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/tasks.py` & `alphaz-0.7.3.9/alphaz/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/tests.py` & `alphaz-0.7.3.9/alphaz/utils/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/time.py` & `alphaz-0.7.3.9/alphaz/utils/time.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz/utils/transactions.py` & `alphaz-0.7.3.9/alphaz/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/alphaz.egg-info/PKG-INFO` & `alphaz-0.7.3.9/alphaz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: alphaz
-Version: 0.7.3.8
+Version: 0.7.3.9
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.3.8.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.3.9.tar.gz
 Description: UNKNOWN
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `alphaz-0.7.3.8/alphaz.egg-info/SOURCES.txt` & `alphaz-0.7.3.9/alphaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.3.8/setup.py` & `alphaz-0.7.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, glob, re
 from datetime import date
 
 today = date.today()
 
 from setuptools import setup, find_packages
 
-version = "0.7.3.8"
+version = "0.7.3.9"
 
 excludes = [".git", ".vscode"]
 
 archives = glob.glob("dist/*")
 for archive in archives:
     os.remove(archive)
```

