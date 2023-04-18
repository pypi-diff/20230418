# Comparing `tmp/edc-0.4.8.tar.gz` & `tmp/edc-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.4.8.tar", last modified: Mon Aug 15 01:30:10 2022, max compression
+gzip compressed data, was "edc-0.4.9.tar", last modified: Mon Aug 15 01:45:03 2022, max compression
```

## Comparing `edc-0.4.8.tar` & `edc-0.4.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:30:10.920499 edc-0.4.8/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-12 15:19:56.000000 edc-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    24286 2022-08-15 01:30:02.000000 edc-0.4.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    36927 2022-08-15 01:30:10.920649 edc-0.4.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    35978 2022-08-15 01:30:02.000000 edc-0.4.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        5 2022-08-15 01:30:02.000000 edc-0.4.8/VERSION
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:30:10.909431 edc-0.4.8/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:30:10.912135 edc-0.4.8/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.8/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.8/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.8/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:30:10.912736 edc-0.4.8/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2778 2022-08-10 01:27:44.000000 edc-0.4.8/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.8/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.8/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.8/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:30:10.913876 edc-0.4.8/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.8/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.8/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.8/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.8/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.8/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.8/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.8/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.8/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:30:10.916624 edc-0.4.8/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)    11863 2022-07-30 01:15:42.000000 edc-0.4.8/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.8/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.8/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.8/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.8/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3625 2022-07-30 01:15:42.000000 edc-0.4.8/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.8/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.8/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.8/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.8/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.8/docs/multisite_deployment.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3267 2022-07-30 01:15:42.000000 edc-0.4.8/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.8/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.8/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.8/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:30:10.917481 edc-0.4.8/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    36927 2022-08-15 01:30:10.000000 edc-0.4.8/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1460 2022-08-15 01:30:10.000000 edc-0.4.8/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-15 01:30:10.000000 edc-0.4.8/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.8/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1810 2022-08-15 01:30:10.000000 edc-0.4.8/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-15 01:30:10.000000 edc-0.4.8/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:30:10.917583 edc-0.4.8/image/
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.8/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.8/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:30:10.919982 edc-0.4.8/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.8/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.8/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1009 2022-08-15 01:30:02.000000 edc-0.4.8/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4101 2022-08-15 01:30:02.000000 edc-0.4.8/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.8/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.8/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.8/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.8/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.8/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-08-10 01:27:44.000000 edc-0.4.8/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.8/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2941 2022-08-15 01:30:10.921079 edc-0.4.8/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:30:10.920266 edc-0.4.8/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.8/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.8/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.020420 edc-0.4.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-12 15:19:56.000000 edc-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    24315 2022-08-15 01:44:54.000000 edc-0.4.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    36927 2022-08-15 01:45:03.020572 edc-0.4.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    35978 2022-08-15 01:30:02.000000 edc-0.4.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        5 2022-08-15 01:44:54.000000 edc-0.4.9/VERSION
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.006464 edc-0.4.9/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.009745 edc-0.4.9/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.9/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.9/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.9/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.010386 edc-0.4.9/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2778 2022-08-10 01:27:44.000000 edc-0.4.9/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.9/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.9/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.9/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.011571 edc-0.4.9/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.9/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.014346 edc-0.4.9/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)    11863 2022-07-30 01:15:42.000000 edc-0.4.9/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.9/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.9/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.9/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.9/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3625 2022-07-30 01:15:42.000000 edc-0.4.9/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.9/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.9/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.9/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.9/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.9/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3267 2022-07-30 01:15:42.000000 edc-0.4.9/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.9/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.9/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.9/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.015210 edc-0.4.9/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    36927 2022-08-15 01:45:02.000000 edc-0.4.9/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1460 2022-08-15 01:45:03.000000 edc-0.4.9/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-15 01:45:02.000000 edc-0.4.9/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.9/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1810 2022-08-15 01:45:02.000000 edc-0.4.9/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-15 01:45:02.000000 edc-0.4.9/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.015311 edc-0.4.9/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.9/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.9/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.019973 edc-0.4.9/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.9/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.9/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1009 2022-08-15 01:30:02.000000 edc-0.4.9/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4101 2022-08-15 01:30:02.000000 edc-0.4.9/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.9/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.9/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.9/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.9/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.9/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      222 2022-08-10 01:27:44.000000 edc-0.4.9/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.9/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2941 2022-08-15 01:45:03.020986 edc-0.4.9/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-15 01:45:03.020261 edc-0.4.9/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.9/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.9/utils/get_edc_requirements.py
```

### Comparing `edc-0.4.8/.gitignore` & `edc-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/.pre-commit-config.yaml` & `edc-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/CHANGES` & `edc-0.4.9/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changes
 =======
 
+0.4.9
+-----
+- bump edc-egfr
+
 0.4.8
 -----
 - move all eGFR code to edc-egfr module
   (edc-egfr, edc-lab-results, edc-reportables)
 
 0.4.7
 -----
```

### Comparing `edc-0.4.8/LICENSE` & `edc-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/PKG-INFO` & `edc-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.8
+Version: 0.4.9
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.8/README.rst` & `edc-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/bin/nginx/edc-uat.conf` & `edc-0.4.9/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/bin/nginx/edc.conf` & `edc-0.4.9/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/bin/scripts/dev_repos.sh` & `edc-0.4.9/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/bin/scripts/update_edc.sh` & `edc-0.4.9/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/bin/systemd/celery-uat.service` & `edc-0.4.9/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/bin/systemd/celery.service` & `edc-0.4.9/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/README.rst` & `edc-0.4.9/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/backup.rst` & `edc-0.4.9/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/celery.rst` & `edc-0.4.9/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/conda.rst` & `edc-0.4.9/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/configure_web_services.rst` & `edc-0.4.9/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/deploy_new_droplet.rst` & `edc-0.4.9/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/exporting_encrypted_data.rst` & `edc-0.4.9/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/forms_reference.md` & `edc-0.4.9/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/landing_page.rst` & `edc-0.4.9/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/prepare_database.rst` & `edc-0.4.9/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/printing.rst` & `edc-0.4.9/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/docs/update_deployment.rst` & `edc-0.4.9/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/edc.egg-info/PKG-INFO` & `edc-0.4.9/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.8
+Version: 0.4.9
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.8/edc.egg-info/SOURCES.txt` & `edc-0.4.9/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/edc.egg-info/requires.txt` & `edc-0.4.9/edc.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 edc-crf==0.3.26
 edc-dashboard==0.3.23
 edc-data-manager==0.3.32
 edc-device==0.3.8
 edc-document-status==0.1.2
 edc-dx==0.1.9
 edc-dx-review==0.1.16
-edc-egfr==0.1.0
+edc-egfr==0.1.1
 edc-export==0.3.14
 edc-facility==0.3.11
 edc-fieldsets==0.3.8
 edc-form-describer==0.3.9
 edc-form-label==0.3.4
 edc-form-validators==0.3.20
 edc-glucose==0.1.18
```

### Comparing `edc-0.4.8/image/icon-pycharm.png` & `edc-0.4.9/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/requirements.tests/edc.txt` & `edc-0.4.9/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/requirements.tests/edc_dev.txt` & `edc-0.4.9/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.8/setup.cfg` & `edc-0.4.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 	edc-crf==0.3.26
 	edc-dashboard==0.3.23
 	edc-data-manager==0.3.32
 	edc-device==0.3.8
 	edc-document-status==0.1.2
 	edc-dx==0.1.9
 	edc-dx-review==0.1.16
-	edc-egfr==0.1.0
+	edc-egfr==0.1.1
 	edc-export==0.3.14
 	edc-facility==0.3.11
 	edc-fieldsets==0.3.8
 	edc-form-describer==0.3.9
 	edc-form-label==0.3.4
 	edc-form-validators==0.3.20
 	edc-glucose==0.1.18
```

### Comparing `edc-0.4.8/utils/get_edc_requirements.py` & `edc-0.4.9/utils/get_edc_requirements.py`

 * *Files identical despite different names*

