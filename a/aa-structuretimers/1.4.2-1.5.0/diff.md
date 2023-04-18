# Comparing `tmp/aa-structuretimers-1.4.2.tar.gz` & `tmp/aa_structuretimers-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-structuretimers-1.4.2.tar", last modified: Tue Jul 19 13:00:22 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aa-structuretimers-1.4.2.tar` & `aa_structuretimers-1.5.0.tar`

### file list

```diff
@@ -1,93 +1,76 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.716160 aa-structuretimers-1.4.2/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2020-10-24 20:20:52.000000 aa-structuretimers-1.4.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      162 2021-01-29 14:53:34.000000 aa-structuretimers-1.4.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11115 2022-07-19 13:00:22.716160 aa-structuretimers-1.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10160 2021-10-26 20:57:41.000000 aa-structuretimers-1.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.700160 aa-structuretimers-1.4.2/aa_structuretimers.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11115 2022-07-19 13:00:22.000000 aa-structuretimers-1.4.2/aa_structuretimers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3182 2022-07-19 13:00:22.000000 aa-structuretimers-1.4.2/aa_structuretimers.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 13:00:22.000000 aa-structuretimers-1.4.2/aa_structuretimers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      148 2022-07-19 13:00:22.000000 aa-structuretimers-1.4.2/aa_structuretimers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-07-19 13:00:22.000000 aa-structuretimers-1.4.2/aa_structuretimers.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-19 13:00:22.716160 aa-structuretimers-1.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1783 2022-07-19 12:46:02.000000 aa-structuretimers-1.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.700160 aa-structuretimers-1.4.2/structuretimers/
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-07-19 12:46:02.000000 aa-structuretimers-1.4.2/structuretimers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14352 2022-04-19 19:20:15.000000 aa-structuretimers-1.4.2/structuretimers/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2021-07-12 12:12:01.000000 aa-structuretimers-1.4.2/structuretimers/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2021-04-12 22:48:42.000000 aa-structuretimers-1.4.2/structuretimers/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      943 2022-05-09 18:14:56.000000 aa-structuretimers-1.4.2/structuretimers/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2022-01-10 21:15:26.000000 aa-structuretimers-1.4.2/structuretimers/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    11466 2022-05-07 20:17:49.000000 aa-structuretimers-1.4.2/structuretimers/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.696160 aa-structuretimers-1.4.2/structuretimers/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.704160 aa-structuretimers-1.4.2/structuretimers/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-24 20:20:52.000000 aa-structuretimers-1.4.2/structuretimers/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1009 2022-01-10 21:15:26.000000 aa-structuretimers-1.4.2/structuretimers/management/commands/structuretimers_load_eve.py
--rw-rw-rw-   0 root         (0) root         (0)     7766 2021-07-08 20:36:06.000000 aa-structuretimers-1.4.2/structuretimers/management/commands/structuretimers_migrate_timers.py
--rw-rw-rw-   0 root         (0) root         (0)     4585 2022-04-19 19:20:15.000000 aa-structuretimers-1.4.2/structuretimers/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.704160 aa-structuretimers-1.4.2/structuretimers/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    20776 2021-04-12 22:48:42.000000 aa-structuretimers-1.4.2/structuretimers/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     6043 2021-07-13 22:44:21.000000 aa-structuretimers-1.4.2/structuretimers/migrations/0002_distances_from_staging.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2022-01-12 20:30:56.000000 aa-structuretimers-1.4.2/structuretimers/migrations/0003_add_preliminary_timers.py
--rw-rw-rw-   0 root         (0) root         (0)     3411 2022-04-19 19:32:35.000000 aa-structuretimers-1.4.2/structuretimers/migrations/0004_add_space_type_and_region_filters.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-24 20:20:52.000000 aa-structuretimers-1.4.2/structuretimers/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35284 2022-04-19 19:20:15.000000 aa-structuretimers-1.4.2/structuretimers/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.696160 aa-structuretimers-1.4.2/structuretimers/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.696160 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.704160 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/css/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2021-07-12 12:12:01.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/css/global.css
--rw-rw-rw-   0 root         (0) root         (0)      138 2021-07-12 12:12:01.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/css/timer_edit.css
--rw-rw-rw-   0 root         (0) root         (0)      790 2022-01-10 23:47:47.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/css/timer_list.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.704160 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/img/
--rw-rw-rw-   0 root         (0) root         (0)    43262 2021-07-12 12:12:01.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/img/Spinner-1s-64px-dark.gif
--rw-rw-rw-   0 root         (0) root         (0)    43381 2021-07-12 12:12:01.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/img/Spinner-1s-64px-light.gif
--rw-rw-rw-   0 root         (0) root         (0)      788 2021-07-12 12:12:01.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/img/structuretimers_logo.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.708160 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/js/
--rw-rw-rw-   0 root         (0) root         (0)     1847 2022-05-07 20:17:49.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/js/timer_edit.js
--rw-rw-rw-   0 root         (0) root         (0)     9993 2022-01-13 20:42:51.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/js/timer_list.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.696160 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.708160 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/
--rw-rw-rw-   0 root         (0) root         (0)    15823 2020-10-24 20:20:52.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.css
--rw-rw-rw-   0 root         (0) root         (0)    72483 2020-10-24 20:20:52.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.708160 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/vendor/select2-bootstrap-theme-0.1.0-beta.10/
--rw-rw-rw-   0 root         (0) root         (0)    16792 2020-10-24 20:20:52.000000 aa-structuretimers-1.4.2/structuretimers/static/structuretimers/vendor/select2-bootstrap-theme-0.1.0-beta.10/select2-bootstrap.min.css
--rw-rw-rw-   0 root         (0) root         (0)    12386 2022-04-19 19:20:15.000000 aa-structuretimers-1.4.2/structuretimers/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.696160 aa-structuretimers-1.4.2/structuretimers/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.708160 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/
--rw-rw-rw-   0 root         (0) root         (0)      286 2021-05-04 22:14:49.000000 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.708160 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/partials/
--rw-rw-rw-   0 root         (0) root         (0)      170 2022-05-09 12:47:08.000000 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/partials/cancel_button.html
--rw-rw-rw-   0 root         (0) root         (0)      671 2022-01-10 23:47:47.000000 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/partials/preliminary_list_table.html
--rw-rw-rw-   0 root         (0) root         (0)      731 2022-01-10 21:15:26.000000 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/partials/timer_list_table.html
--rw-rw-rw-   0 root         (0) root         (0)      981 2022-05-09 12:47:08.000000 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/timer_confirm_delete.html
--rw-rw-rw-   0 root         (0) root         (0)      146 2021-07-13 22:44:21.000000 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/timer_create_form.html
--rw-rw-rw-   0 root         (0) root         (0)      649 2022-05-09 12:47:08.000000 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/timer_detail.html
--rw-rw-rw-   0 root         (0) root         (0)     2244 2022-05-09 12:47:08.000000 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/timer_edit.html
--rw-rw-rw-   0 root         (0) root         (0)     6914 2022-07-19 11:55:50.000000 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/timer_list.html
--rw-rw-rw-   0 root         (0) root         (0)      156 2021-07-13 22:44:21.000000 aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/timer_update_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.712160 aa-structuretimers-1.4.2/structuretimers/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-11 23:08:18.000000 aa-structuretimers-1.4.2/structuretimers/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7542 2022-01-11 23:08:18.000000 aa-structuretimers-1.4.2/structuretimers/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     5360 2022-01-11 23:08:18.000000 aa-structuretimers-1.4.2/structuretimers/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)    10551 2022-05-07 20:17:49.000000 aa-structuretimers-1.4.2/structuretimers/tests/test_forms.py
--rw-rw-rw-   0 root         (0) root         (0)    15409 2022-01-11 23:08:18.000000 aa-structuretimers-1.4.2/structuretimers/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    47190 2022-04-19 19:20:15.000000 aa-structuretimers-1.4.2/structuretimers/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2022-05-09 18:14:56.000000 aa-structuretimers-1.4.2/structuretimers/tests/test_navigation_highlight.py
--rw-rw-rw-   0 root         (0) root         (0)    12952 2022-01-11 23:08:18.000000 aa-structuretimers-1.4.2/structuretimers/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    19936 2022-03-18 18:40:16.000000 aa-structuretimers-1.4.2/structuretimers/tests/test_views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.712160 aa-structuretimers-1.4.2/structuretimers/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)      327 2020-10-24 20:20:52.000000 aa-structuretimers-1.4.2/structuretimers/tests/testdata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2021-04-12 22:48:42.000000 aa-structuretimers-1.4.2/structuretimers/tests/testdata/create_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)     4730 2022-04-19 19:20:15.000000 aa-structuretimers-1.4.2/structuretimers/tests/testdata/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     2642 2022-01-11 23:08:18.000000 aa-structuretimers-1.4.2/structuretimers/tests/testdata/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1646 2022-01-10 21:15:26.000000 aa-structuretimers-1.4.2/structuretimers/tests/testdata/generate_timers.py
--rw-rw-rw-   0 root         (0) root         (0)      388 2020-10-24 20:20:52.000000 aa-structuretimers-1.4.2/structuretimers/tests/testdata/load_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2022-01-12 20:21:29.000000 aa-structuretimers-1.4.2/structuretimers/tests/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      936 2022-01-13 20:42:51.000000 aa-structuretimers-1.4.2/structuretimers/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    17849 2022-04-19 19:20:15.000000 aa-structuretimers-1.4.2/structuretimers/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 13:00:22.716160 aa-structuretimers-1.4.2/testauth/
--rw-rw-rw-   0 root         (0) root         (0)       46 2020-10-24 20:20:52.000000 aa-structuretimers-1.4.2/testauth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2021-04-12 22:48:42.000000 aa-structuretimers-1.4.2/testauth/celery.py
--rw-rw-rw-   0 root         (0) root         (0)     9905 2021-10-26 21:23:11.000000 aa-structuretimers-1.4.2/testauth/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2021-04-12 22:48:42.000000 aa-structuretimers-1.4.2/testauth/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2020-10-24 20:20:52.000000 aa-structuretimers-1.4.2/testauth/wsgi.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/__init__.py
+-rw-r--r--   0        0        0    14349 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/admin.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/app_settings.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/apps.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/auth_hooks.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/constants.py
+-rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/forms.py
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/managers.py
+-rw-r--r--   0        0        0    35753 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/models.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tasks.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/urls.py
+-rw-r--r--   0        0        0    17849 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/views.py
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/django.pot
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/management/commands/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/management/commands/structuretimers_load_eve.py
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/management/commands/structuretimers_migrate_timers.py
+-rw-r--r--   0        0        0    20775 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/migrations/0001_initial.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/migrations/0002_distances_from_staging.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/migrations/0003_add_preliminary_timers.py
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/migrations/0004_add_space_type_and_region_filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/migrations/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/css/global.css
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/css/timer_edit.css
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/css/timer_list.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/structuretimers_logo.png
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/js/timer_edit.js
+-rw-r--r--   0        0        0     9993 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/js/timer_list.js
+-rw-r--r--   0        0        0    15823 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.css
+-rw-r--r--   0        0        0    72483 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.js
+-rw-r--r--   0        0        0    16792 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-bootstrap-theme-0.1.0-beta.10/select2-bootstrap.min.css
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/base.html
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_confirm_delete.html
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_create_form.html
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_detail.html
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_edit.html
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_list.html
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_update_form.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/partials/cancel_button.html
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/partials/preliminary_list_table.html
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/partials/timer_list_table.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/__init__.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_admin.py
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_commands.py
+-rw-r--r--   0        0        0    10580 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_forms.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_integration.py
+-rw-r--r--   0        0        0    47940 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_models.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_navigation_highlight.py
+-rw-r--r--   0        0        0    18750 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_tasks.py
+-rw-r--r--   0        0        0    20014 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_views.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/utils.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/__init__.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    10514 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/factory.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/fixtures.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/generate_timers.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0    32649 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/test_image.jpg
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tools/drop_tables.sql
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/LICENSE
+-rw-r--r--   0        0        0    10160 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/README.md
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/PKG-INFO
```

### Comparing `aa-structuretimers-1.4.2/LICENSE` & `aa_structuretimers-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/PKG-INFO` & `aa_structuretimers-1.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 Metadata-Version: 2.1
 Name: aa-structuretimers
-Version: 1.4.2
+Version: 1.5.0
 Summary: An app for keeping track of Eve Online structure timers with Alliance Auth and Discord
-Home-page: https://gitlab.com/ErikKalkoken/aa-structuretimers
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
-Platform: UNKNOWN
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-structuretimers
+Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-structuretimers
+Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-structuretimers/-/blob/master/CHANGELOG.md
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-structuretimers/-/issues
+Author-email: Erik Kalkoken <kalkoken87@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.7
+Requires-Python: >=3.8
+Requires-Dist: allianceauth-app-utils>=1.17.1
+Requires-Dist: allianceauth>=3
+Requires-Dist: dhooks-lite>=1.0.0
+Requires-Dist: django-eveuniverse>=0.16
+Requires-Dist: django-multiselectfield
+Requires-Dist: redis-simple-mq>=0.4
+Requires-Dist: requests
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Structure Timers II
 
 An app for keeping track of Eve Online structure timers with Alliance Auth and Discord.
 
 [![release](https://img.shields.io/pypi/v/aa-structuretimers?label=release)](https://pypi.org/project/aa-structuretimers/)
 [![python](https://img.shields.io/pypi/pyversions/aa-structuretimers)](https://pypi.org/project/aa-structuretimers/)
@@ -247,9 +255,7 @@
 
 ## Management commands
 
 The following management commands are available:
 
 - **structuretimers_load_eve**: Preload all eve objects required for this app to function
 - **structuretimers_migrate_timers**: Migrate pending timers from Auth's Structure Timers apps
-
-
```

### Comparing `aa-structuretimers-1.4.2/README.md` & `aa_structuretimers-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/admin.py` & `aa_structuretimers-1.5.0/structuretimers/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 
     @admin.display(ordering="scheduled time")
     def _time(self, obj) -> Optional[str]:
         if obj.scheduled_time is None:
             return None
         return obj.get_scheduled_time_display()
 
-    def _timer_clauses(self, obj) -> list:
+    def _timer_clauses(self, obj) -> str:
         clauses = list()
         for field, func, choices in [
             ("require_timer_types", self._add_to_clauses_1, Timer.Type.choices),
             ("exclude_timer_types", self._add_to_clauses_1, Timer.Type.choices),
             ("require_objectives", self._add_to_clauses_1, Timer.Objective.choices),
             ("exclude_objectives", self._add_to_clauses_1, Timer.Objective.choices),
             ("require_visibility", self._add_to_clauses_1, Timer.Visibility.choices),
@@ -241,15 +241,15 @@
                 Timer.SpaceType.choices,
             ),
             ("is_important", self._add_to_clauses_3, None),
             ("is_opsec", self._add_to_clauses_3, None),
         ]:
             func(clauses, obj, field, choices)
 
-        return mark_safe("<br>".join(clauses)) if clauses else None
+        return mark_safe("<br>".join(clauses)) if clauses else ""
 
     def _add_to_clauses_1(self, clauses, obj, field, choices):
         if getattr(obj, field):
             text = ", ".join(
                 map(
                     str,
                     [
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/app_settings.py` & `aa_structuretimers-1.5.0/structuretimers/app_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-from app_utils.django import clean_setting
+from app_utils.app_settings import clean_setting
 
-# Will not schedule notifications for timers
-# which have elapsed more than x minutes ago
 STRUCTURETIMERS_MAX_AGE_FOR_NOTIFICATIONS = clean_setting(
     "STRUCTURETIMERS_MAX_AGE_FOR_NOTIFICATIONS", 60
 )
+"""Will not schedule notifications for timers,
+which have elapsed more than x minutes ago.
+"""
 
-# Wether notifications for timers are scheduled at all
 STRUCTURETIMERS_NOTIFICATIONS_ENABLED = clean_setting(
     "STRUCTURETIMERS_NOTIFICATIONS_ENABLED", True
 )
+"""Whether notifications for timers are scheduled at all."""
 
-# Minimum age in days for a timer to be considered obsolete
-# Obsolete timers will automatically be deleted
 STRUCTURETIMERS_TIMERS_OBSOLETE_AFTER_DAYS = clean_setting(
     "STRUCTURETIMERS_TIMERS_OBSOLETE_AFTER_DAYS", default_value=30, min_value=1
 )
+"""Minimum age in days for a timer to be considered obsolete.
+Obsolete timers will automatically be deleted.
+"""
 
-# Default page size for timerboard.
-# Must be an integer value from the current options as seen in the app.
 STRUCTURETIMERS_DEFAULT_PAGE_LENGTH = clean_setting(
     "STRUCTURETIMERS_DEFAULT_PAGE_LENGTH", 10
 )
+"""Default page size for timerboard.
+Must be an integer value from the current options as seen in the app.
+"""
 
-# Wether paging is enabled on the timerboard
 STRUCTURETIMERS_PAGING_ENABLED = clean_setting("STRUCTURETIMERS_PAGING_ENABLED", True)
+"""Whether paging is enabled on the timerboard."""
 
-# Wether structures sets the name and avatar icon of a webhook.
 STRUCTURETIMER_NOTIFICATION_SET_AVATAR = clean_setting(
     "STRUCTURETIMER_NOTIFICATION_SET_AVATAR", True
 )
+"""Whether structures sets the name and avatar icon of a webhook."""
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/auth_hooks.py` & `aa_structuretimers-1.5.0/structuretimers/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/forms.py` & `aa_structuretimers-1.5.0/structuretimers/forms.py`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/management/commands/structuretimers_load_eve.py` & `aa_structuretimers-1.5.0/structuretimers/management/commands/structuretimers_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/management/commands/structuretimers_migrate_timers.py` & `aa_structuretimers-1.5.0/structuretimers/management/commands/structuretimers_migrate_timers.py`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/managers.py` & `aa_structuretimers-1.5.0/structuretimers/managers.py`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/migrations/0001_initial.py` & `aa_structuretimers-1.5.0/structuretimers/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("eveonline", "0012_index_additions"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("eveuniverse", "0002_load_eveunit"),
     ]
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/migrations/0002_distances_from_staging.py` & `aa_structuretimers-1.5.0/structuretimers/migrations/0002_distances_from_staging.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("eveonline", "0014_auto_20210105_1413"),
         ("eveuniverse", "0005_type_materials_and_sections"),
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("structuretimers", "0001_initial"),
     ]
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/migrations/0003_add_preliminary_timers.py` & `aa_structuretimers-1.5.0/structuretimers/migrations/0003_add_preliminary_timers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.10 on 2022-01-12 20:20
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("structuretimers", "0002_distances_from_staging"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="timer",
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/migrations/0004_add_space_type_and_region_filters.py` & `aa_structuretimers-1.5.0/structuretimers/migrations/0004_add_space_type_and_region_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import multiselectfield.db.fields
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("eveuniverse", "0007_evetype_description"),
         ("eveonline", "0015_factions"),
         ("structuretimers", "0003_add_preliminary_timers"),
     ]
 
     operations = [
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/models.py` & `aa_structuretimers-1.5.0/structuretimers/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from time import sleep
-from typing import Any, List, Tuple
+from typing import Any, List, Optional, Tuple
 
 import dhooks_lite
 from multiselectfield import MultiSelectField
 from simple_mq import SimpleMQ
 
 from django.contrib.auth.models import User
 from django.db import models
@@ -119,24 +119,24 @@
         return self.name
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(id={self.id}, name='{self.name}')"
 
     def send_message(
         self,
-        content: str = None,
-        embeds: List[dhooks_lite.Embed] = None,
-        tts: bool = None,
-        username: str = None,
-        avatar_url: str = None,
+        content: Optional[str] = None,
+        embeds: Optional[List[dhooks_lite.Embed]] = None,
+        tts: Optional[bool] = None,
+        username: Optional[str] = None,
+        avatar_url: Optional[str] = None,
     ) -> int:
         """Adds Discord message to queue for later sending
 
         Returns updated size of queue
-        Raises ValueError if mesage is incomplete
+        Raises ValueError if message is incomplete
         """
         if not content and not embeds:
             raise ValueError("Message must have content or embeds to be valid")
 
         if embeds:
             embeds_list = [obj.asdict() for obj in embeds]
         else:
@@ -153,17 +153,17 @@
             message["username"] = username
         if avatar_url:
             message["avatar_url"] = avatar_url
 
         return self._main_queue.enqueue(json.dumps(message, cls=JSONDateTimeEncoder))
 
     def send_queued_messages(self) -> int:
-        """sends all messages in the queue to this webhook
+        """Send all messages in the queue to this webhook
 
-        returns number of successfull sent messages
+        Return number of successful sent messages
 
         Messages that could not be sent are put back into the queue for later retry
         """
         message_count = 0
         while True:
             message_json = self._main_queue.dequeue()
             if message_json:
@@ -209,15 +209,15 @@
 
         returns True if successful, else False
         """
         hook = dhooks_lite.Webhook(url=self.url)
         if message.get("embeds"):
             embeds = [
                 dhooks_lite.Embed.from_dict(embed_dict)
-                for embed_dict in message.get("embeds")
+                for embed_dict in message.get("embeds", [])
             ]
         else:
             embeds = None
 
         response = hook.execute(
             content=message.get("content"),
             embeds=embeds,
@@ -315,32 +315,35 @@
 
     class Visibility(models.TextChoices):
         UNRESTRICTED = "UN", _("unrestricted")
         ALLIANCE = "AL", _("Alliance only")
         CORPORATION = "CO", _("Corporation only")
 
     class SpaceType(models.TextChoices):
+        UNDEFINED = "UN", _("undefined")
         HIGH_SEC = "HS", _("highsec")
         LOW_SEC = "LS", _("lowsec")
         NULL_SEC = "NS", _("nullsec")
         WH_SPACE = "WS", _("wh space")
 
         @classmethod
-        def from_eve_solar_system(cls, eve_solar_sytem: EveSolarSystem):
-            """Determin the space type of a solar system and return it."""
-            if eve_solar_sytem.is_high_sec:
+        def from_eve_solar_system(cls, eve_solar_system: Optional[EveSolarSystem]):
+            """Determine the space type of a solar system and return it."""
+            if not eve_solar_system:
+                return cls.UNDEFINED
+            if eve_solar_system.is_high_sec:
                 return cls.HIGH_SEC
-            if eve_solar_sytem.is_low_sec:
+            if eve_solar_system.is_low_sec:
                 return cls.LOW_SEC
-            if eve_solar_sytem.is_null_sec:
+            if eve_solar_system.is_null_sec:
                 return cls.NULL_SEC
-            if eve_solar_sytem.is_w_space:
+            if eve_solar_system.is_w_space:
                 return cls.WH_SPACE
             raise NotImplementedError(
-                f"System with unknown space type: {eve_solar_sytem}"
+                f"System with unknown space type: {eve_solar_system}"
             )
 
     date = models.DateTimeField(
         db_index=True,
         null=True,
         help_text="Date when this timer happens",
     )
@@ -514,23 +517,23 @@
             )
 
     @property
     def structure_display_name(self):
         return "{}{} in {}{}".format(
             self.structure_type.name,
             f' "{self.structure_name}"' if self.structure_name else "",
-            self.eve_solar_system.name,
+            self.eve_solar_system.name if self.eve_solar_system else "",
             f" near {self.location_details}" if self.location_details else "",
         )
 
     @property
     def space_type(self) -> "SpaceType":
         return self.SpaceType.from_eve_solar_system(self.eve_solar_system)
 
-    def user_can_edit(self, user: user) -> bool:
+    def user_can_edit(self, user: User) -> bool:
         """Checks if the given user can edit this timer. Returns True or False"""
         return user.has_perm("structuretimers.manage_timer") or (
             self.user == user and user.has_perm("structuretimers.create_timer")
         )
 
     """
     def user_can_view(self, user: user) -> bool:
@@ -597,36 +600,43 @@
         }
         if self.objective in label_types_map:
             label_type = label_types_map[self.objective]
         else:
             label_type = "default"
         return label_type
 
-    def send_notification(self, webhook: DiscordWebhook, content: str = None) -> None:
+    def send_notification(
+        self, webhook: DiscordWebhook, content: Optional[str] = None
+    ) -> None:
         """Sends notification related to this timer to given webhook."""
         structure_type_name = self.structure_type.name
-        solar_system_name = self.eve_solar_system.name
+        solar_system_name = self.eve_solar_system.name if self.eve_solar_system else ""
         title = f"{structure_type_name} in {solar_system_name}"
         if self.structure_name:
             structure_name_text = f'**{structure_type_name}** "{self.structure_name}"'
         else:
             article = "an" if structure_type_name[0:1].lower() in "aeiou" else "a"
             structure_name_text = f"{article} **{structure_type_name}**"
 
-        region_name = self.eve_solar_system.eve_constellation.eve_region.name
+        region_name = (
+            self.eve_solar_system.eve_constellation.eve_region.name
+            if self.eve_solar_system
+            else ""
+        )
         solar_system_link = webhook.create_discord_link(
             name=solar_system_name, url=dotlan.solar_system_url(solar_system_name)
         )
         solar_system_text = f"{solar_system_link} ({region_name})"
         near_text = f" near {self.location_details}" if self.location_details else ""
         owned_text = f" owned by **{self.owner_name}**" if self.owner_name else ""
+        elapse_at = self.date.strftime(DATETIME_FORMAT) if self.date else "?"
         description = (
             f"The **{self.get_timer_type_display()}** timer for "
             f"{structure_name_text} in {solar_system_text}{near_text}{owned_text} "
-            f"will elapse at **{self.date.strftime(DATETIME_FORMAT)}**. "
+            f"will elapse at **{elapse_at}**. "
             f"Our stance is: **{self.get_objective_display()}**."
         )
         structure_icon_url = self.structure_type.icon_url(size=128)
         if self.objective == self.Objective.FRIENDLY:
             color = int("0x375a7f", 16)
         elif self.objective == self.Objective.HOSTILE:
             color = int("0xd9534f", 16)
@@ -651,15 +661,14 @@
             embeds=[embed],
             username=username,
             avatar_url=avatar_url,
         )
 
 
 class NotificationRule(models.Model):
-
     # Trigger choices
     class Trigger(models.TextChoices):
         NEW_TIMER_CREATED = "TC", _("New timer created")
         SCHEDULED_TIME_REACHED = "TR", _("Scheduled time reached")
 
     # Minutes choices
     MINUTES_0 = 0
@@ -917,21 +926,21 @@
 
         if is_matching and self.require_alliances.exists():
             is_matching = timer.eve_alliance in self.require_alliances.all()
 
         if is_matching and self.exclude_alliances.exists():
             is_matching = timer.eve_alliance not in self.exclude_alliances.all()
 
-        if is_matching and self.require_regions.exists():
+        if is_matching and timer.eve_solar_system and self.require_regions.exists():
             is_matching = (
                 timer.eve_solar_system.eve_constellation.eve_region
                 in self.require_regions.all()
             )
 
-        if is_matching and self.exclude_regions.exists():
+        if is_matching and timer.eve_solar_system and self.exclude_regions.exists():
             is_matching = (
                 timer.eve_solar_system.eve_constellation.eve_region
                 not in self.exclude_regions.all()
             )
         if is_matching and self.require_space_types:
             is_matching = timer.space_type in self.require_space_types
 
@@ -989,15 +998,15 @@
     eve_solar_system = models.OneToOneField(
         EveSolarSystem,
         on_delete=models.SET_DEFAULT,
         default=None,
         null=True,
         blank=True,
         related_name="+",
-    )  # TODO: Remove Nullable if possible, because it is causeing issues
+    )  # TODO: Remove Nullable if possible, because it is causing issues
     is_main = models.BooleanField(default=False)
 
     def __str__(self) -> str:
         return str(self.eve_solar_system)
 
     def save(self, *args, **kwargs) -> None:
         try:
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/static/structuretimers/css/global.css` & `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/css/global.css`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/static/structuretimers/css/timer_list.css` & `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/css/timer_list.css`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/static/structuretimers/img/Spinner-1s-64px-dark.gif` & `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/static/structuretimers/img/Spinner-1s-64px-light.gif` & `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/static/structuretimers/img/structuretimers_logo.png` & `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/structuretimers_logo.png`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/static/structuretimers/js/timer_edit.js` & `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/js/timer_edit.js`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/static/structuretimers/js/timer_list.js` & `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/js/timer_list.js`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.css` & `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.css`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.js` & `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.js`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/static/structuretimers/vendor/select2-bootstrap-theme-0.1.0-beta.10/select2-bootstrap.min.css` & `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-bootstrap-theme-0.1.0-beta.10/select2-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/tasks.py` & `aa_structuretimers-1.5.0/structuretimers/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import timedelta
+from typing import Optional
 
 from celery import shared_task
 
 from django.contrib.auth.models import User
 from django.db import DatabaseError, transaction
 from django.utils.timezone import now
 
@@ -19,270 +20,283 @@
     NotificationRule,
     ScheduledNotification,
     StagingSystem,
     Timer,
 )
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
-TASK_PRIO_HIGH = 4
+TASK_PRIORITY_HIGH = 4
 
 
 @shared_task(base=QueueOnce, acks_late=True)
 def send_messages_for_webhook(webhook_pk: int) -> None:
-    """sends all currently queued messages for given webhook to Discord"""
+    """Send all currently queued messages for given webhook to Discord."""
     webhook = DiscordWebhook.objects.get(pk=webhook_pk)
     if not webhook.is_enabled:
         logger.info("Tracker %s: DiscordWebhook disabled - skipping sending", webhook)
         return
     logger.info("Started sending messages to webhook %s", webhook)
     webhook.send_queued_messages()
     logger.info("Completed sending messages to webhook %s", webhook)
 
 
 @shared_task(base=QueueOnce, bind=True, acks_late=True)
 def send_scheduled_notification(self, scheduled_notification_pk: int) -> None:
-    """Sends a scheduled notification for a timer based on a notification rule"""
+    """Send a scheduled notification for a timer based on a notification rule."""
     with transaction.atomic():
         try:
             scheduled_notification = (
                 ScheduledNotification.objects.select_for_update().get(
                     pk=scheduled_notification_pk
                 )
             )
         except (ScheduledNotification.DoesNotExist, DatabaseError):
             logger.info(
                 "ScheduledNotification with pk = %s does not / no longer exist "
                 "or is being processed by another task. Discarding.",
                 scheduled_notification_pk,
+            )
+            logger.debug(
+                "ScheduledNotification pk = %s. Debug info",
+                scheduled_notification_pk,
                 exc_info=True,
             )
             return
+
         logger.debug(
             "Delete scheduled_notification in task_id = %s: %r",
             self.request.id,
             scheduled_notification,
         )
         scheduled_notification.delete()
 
-    timer = scheduled_notification.timer
-    notification_rule = scheduled_notification.notification_rule
     if scheduled_notification.celery_task_id != self.request.id:
         logger.info(
-            "Discarded outdated scheduled notification: %r",
-            scheduled_notification,
+            "Discarded outdated scheduled notification: %r", scheduled_notification
         )
-    elif not notification_rule.is_enabled:
+        return
+
+    notification_rule = scheduled_notification.notification_rule
+    if not notification_rule.is_enabled:
         logger.info(
             "Discarded scheduled notification based on disabled rule: %r",
             scheduled_notification,
         )
-    else:
-        logger.info(
-            "Sending notifications for timer '%s' and rule '%s'",
-            timer,
-            notification_rule,
+        return
+
+    webhook = notification_rule.webhook
+    if not webhook.is_enabled:
+        logger.warning(
+            "Webhook not enabled for %r. Discarding.", scheduled_notification
         )
-        webhook = notification_rule.webhook
-        if webhook.is_enabled:
-            minutes = round((timer.date - now()).total_seconds() / 60)
-            mod_text = "**important** " if timer.is_important else ""
-            content = (
-                f"The following {mod_text}structure timer will elapse "
-                f"in less than **{minutes:,}** minutes:"
-            )
-            timer.send_notification(
-                webhook=webhook,
-                content=notification_rule.prepend_ping_text(content),
-            )
-            send_messages_for_webhook.apply_async(
-                args=[webhook.pk], priority=TASK_PRIO_HIGH
-            )
-        else:
-            logger.warning(
-                "Webhook not enabled for %r. Discarding.", scheduled_notification
-            )
+        return
+
+    timer = scheduled_notification.timer
+    if (
+        not timer.date
+        or timer.date < now()
+        or scheduled_notification.timer_date < now()
+    ):  # fix issue #28
+        logger.warning(
+            "Discarding scheduled notification %r for outdated timer.",
+            scheduled_notification,
+        )
+        return
+
+    logger.info(
+        "Sending notifications for timer '%s' and rule '%s'",
+        timer,
+        notification_rule,
+    )
+    minutes = round((timer.date - now()).total_seconds() / 60)
+    mod_text = "**important** " if timer.is_important else ""
+    content = (
+        f"The following {mod_text}structure timer will elapse "
+        f"in less than **{minutes:,}** minutes:"
+    )
+    timer.send_notification(
+        webhook=webhook,
+        content=notification_rule.prepend_ping_text(content),
+    )
+    send_messages_for_webhook.apply_async(
+        args=[webhook.pk], priority=TASK_PRIORITY_HIGH
+    )
 
 
 @shared_task
 def notify_about_new_timer(timer_pk: int, notification_rule_pk: int) -> None:
+    """Send notification about new timer."""
     timer = Timer.objects.get(pk=timer_pk)
     notification_rule = NotificationRule.objects.select_related("webhook").get(
         pk=notification_rule_pk
     )
+    if not notification_rule.is_enabled or not notification_rule.webhook.is_enabled:
+        return
 
-    if notification_rule.is_enabled and notification_rule.webhook.is_enabled:
-        author_text = f" by **{timer.eve_character}**" if timer.eve_character else ""
-        content = f"New timer added{author_text}:"
-        timer.send_notification(
-            webhook=notification_rule.webhook,
-            content=notification_rule.prepend_ping_text(content),
-        )
-        send_messages_for_webhook.apply_async(
-            args=[notification_rule.webhook.pk], priority=TASK_PRIO_HIGH
-        )
+    author_text = f" by **{timer.eve_character}**" if timer.eve_character else ""
+    content = f"New timer added{author_text}:"
+    timer.send_notification(
+        webhook=notification_rule.webhook,
+        content=notification_rule.prepend_ping_text(content),
+    )
+    send_messages_for_webhook.apply_async(
+        args=[notification_rule.webhook.pk], priority=TASK_PRIORITY_HIGH
+    )
 
 
 @shared_task(acks_late=True)
 def schedule_notifications_for_timer(timer_pk: int, is_new: bool = False) -> None:
-    """Schedules notifications for this timer based on notification rules"""
+    """Schedule notifications for this timer based on notification rules."""
     timer = Timer.objects.select_related_for_matching().get(pk=timer_pk)
     if not timer.date:
-        raise ValueError(f"Not supported for prelimiary timers: {timer}")
-    if timer.date > now():
-        # trigger: newly created
-        if is_new:
-            rules = (
-                NotificationRule.objects.select_related("webhook")
-                .filter(
-                    is_enabled=True,
-                    trigger=NotificationRule.Trigger.NEW_TIMER_CREATED,
-                    webhook__is_enabled=True,
-                )
-                .conforms_with_timer(timer)
-            )
-            if rules:
-                for rule in rules:
-                    notify_about_new_timer.apply_async(
-                        kwargs={
-                            "timer_pk": timer.pk,
-                            "notification_rule_pk": rule.pk,
-                        },
-                        priority=TASK_PRIO_HIGH,
-                    )
-
-        # trigger: timer elapses soon
-        with transaction.atomic():
-            # remove existing scheduled notifications if date has changed
-            for obj in timer.scheduled_notifications.exclude(timer_date=timer.date):
-                _revoke_notification_for_timer(scheduled_notification=obj)
+        raise ValueError(f"Not supported for preliminary timers: {timer}")
 
-            # schedule new notifications
-            for notification_rule in NotificationRule.objects.filter(
+    if timer.date < now():
+        logger.warning("Can not schedule notification for past timer: %s", timer)
+        return
+
+    # trigger: newly created
+    if is_new:
+        rules = (
+            NotificationRule.objects.select_related("webhook")
+            .filter(
                 is_enabled=True,
-                trigger=NotificationRule.Trigger.SCHEDULED_TIME_REACHED,
-            ).conforms_with_timer(timer):
-                _schedule_notification_for_timer(
-                    timer=timer, notification_rule=notification_rule
+                trigger=NotificationRule.Trigger.NEW_TIMER_CREATED,
+                webhook__is_enabled=True,
+            )
+            .conforms_with_timer(timer)
+        )
+        if rules:
+            for rule in rules:
+                notify_about_new_timer.apply_async(
+                    kwargs={"timer_pk": timer.pk, "notification_rule_pk": rule.pk},
+                    priority=TASK_PRIORITY_HIGH,
                 )
-    else:
-        logger.warning("Can not schedule notification for past timer: %s", timer)
+
+    # trigger: timer elapses soon
+    with transaction.atomic():
+        # remove existing scheduled notifications if date has changed
+        for obj in timer.scheduled_notifications.exclude(timer_date=timer.date):
+            _revoke_notification_for_timer(scheduled_notification=obj)
+
+        # schedule new notifications
+        for notification_rule in NotificationRule.objects.filter(
+            is_enabled=True,
+            trigger=NotificationRule.Trigger.SCHEDULED_TIME_REACHED,
+        ).conforms_with_timer(timer):
+            _schedule_notification_for_timer(
+                timer=timer, notification_rule=notification_rule
+            )
 
 
 @shared_task(acks_late=True)
 def schedule_notifications_for_rule(notification_rule_pk: int) -> None:
-    """Schedules notifications for all timers confirming with this rule.
+    """Schedule notifications for all timers confirming with this rule.
+
     Will recreate all existing and still pending notifications
     """
-    try:
-        notification_rule = NotificationRule.objects.get(pk=notification_rule_pk)
-    except NotificationRule.DoesNotExist:
+    notification_rule = NotificationRule.objects.get(pk=notification_rule_pk)
+    if notification_rule.trigger == NotificationRule.Trigger.NEW_TIMER_CREATED:
         logger.error(
-            "NotificationRule with pk = %s does not exist. Aborting.",
+            "NotificationRule with pk = %s has the wrong trigger. Aborting.",
             notification_rule_pk,
         )
-    else:
-        if notification_rule.trigger == NotificationRule.Trigger.NEW_TIMER_CREATED:
-            logger.error(
-                "NotificationRule with pk = %s has the wrong trigger. Aborting.",
-                notification_rule_pk,
-            )
-        else:
-            logger.debug(
-                "Checking scheduled notifications for: %s",
-                notification_rule,
+        return
+
+    logger.debug("Checking scheduled notifications for: %s", notification_rule)
+    with transaction.atomic():
+        for obj in notification_rule.scheduled_notifications.filter(
+            timer_date__gt=now()
+        ):
+            _revoke_notification_for_timer(scheduled_notification=obj)
+
+        for timer in Timer.objects.filter(
+            date__gt=now()
+        ).conforms_with_notification_rule(notification_rule):
+            _schedule_notification_for_timer(
+                timer=timer, notification_rule=notification_rule
             )
-            with transaction.atomic():
-                for obj in notification_rule.scheduled_notifications.filter(
-                    timer_date__gt=now()
-                ):
-                    _revoke_notification_for_timer(scheduled_notification=obj)
-
-                for timer in Timer.objects.filter(
-                    date__gt=now()
-                ).conforms_with_notification_rule(notification_rule):
-                    _schedule_notification_for_timer(
-                        timer=timer, notification_rule=notification_rule
-                    )
 
 
 def _schedule_notification_for_timer(
     timer: Timer, notification_rule: NotificationRule
 ) -> ScheduledNotification:
+    """Schedule notification for a timer."""
     if timer.timer_type == Timer.Type.PRELIMINARY:
-        raise ValueError(f"Can not schedule prelimiary timers: {timer}")
+        raise ValueError(f"Can not schedule preliminary timers: {timer}")
+    if not timer.date:
+        raise ValueError(f"Timer has no date: {timer}")
+    if not notification_rule.scheduled_time:
+        raise ValueError(
+            f"Notification rule has no scheduled date: {notification_rule}"
+        )
     logger.info(
         "Scheduling fresh notification for timer #%d, rule #%d",
         timer.pk,
         notification_rule.pk,
     )
     notification_date = timer.date - timedelta(minutes=notification_rule.scheduled_time)
     scheduled_notification, _ = ScheduledNotification.objects.update_or_create(
         timer=timer,
         notification_rule=notification_rule,
         defaults={"timer_date": timer.date, "notification_date": notification_date},
     )
     result = send_scheduled_notification.apply_async(
         kwargs={"scheduled_notification_pk": scheduled_notification.pk},
         eta=timer.date - timedelta(minutes=notification_rule.scheduled_time),
-        priority=TASK_PRIO_HIGH,
+        priority=TASK_PRIORITY_HIGH,
     )
     scheduled_notification.celery_task_id = result.task_id
     scheduled_notification.save()
 
     return scheduled_notification
 
 
 def _revoke_notification_for_timer(
     scheduled_notification: ScheduledNotification,
 ) -> None:
+    """Revoke notification for a timer."""
     logger.info(
         "Removing stale notification for timer #%d, rule #%d",
         scheduled_notification.timer.pk,
         scheduled_notification.notification_rule.pk,
     )
     scheduled_notification.delete()
 
 
 @shared_task
-def send_test_message_to_webhook(webhook_pk: int, user_pk: int = None) -> None:
-    """send a test message to given webhook.
-    Optional inform user about result if user ok is given
+def send_test_message_to_webhook(
+    webhook_pk: int, user_pk: Optional[int] = None
+) -> None:
+    """Send a test message to given webhook.
+    Optionally inform user about result if user ok is given
     """
-    try:
-        webhook = DiscordWebhook.objects.get(pk=webhook_pk)
-        if user_pk:
-            user = User.objects.get(pk=user_pk)
-        else:
-            user = None
-    except DiscordWebhook.DoesNotExist:
-        logger.error(
-            "DiscordWebhook with pk = %s does not exist. Aborting.", webhook_pk
-        )
-    except User.DoesNotExist:
-        logger.warning("User with pk = %s does not exist. Aborting.", user_pk)
-    else:
-        logger.info("Sending test message to webhook %s", webhook)
-        error_text, success = webhook.send_test_message(user)
-
-        if user:
-            message = (
-                f"Error text: {error_text}\nCheck log files for details."
-                if not success
-                else "No errors"
-            )
-            level = "success" if success else "error"
-            notify(
-                user=user,
-                title=(
-                    f"{__title__}: Result of test message to webhook {webhook}: "
-                    f"{level.upper()}"
-                ),
-                message=message,
-                level=level,
-            )
+    webhook = DiscordWebhook.objects.get(pk=webhook_pk)
+    user = User.objects.get(pk=user_pk) if user_pk else None
+    logger.info("Sending test message to webhook %s", webhook)
+    error_text, success = webhook.send_test_message(user)
+
+    if not user:
+        return
+
+    message = (
+        f"Error text: {error_text}\nCheck log files for details."
+        if not success
+        else "No errors"
+    )
+    level = "success" if success else "error"
+    notify(
+        user=user,
+        title=(
+            f"{__title__}: Result of test message to webhook {webhook}: "
+            f"{level.upper()}"
+        ),
+        message=message,
+        level=level,
+    )
 
 
 @shared_task
 def housekeeping() -> None:
     """Perform housekeeping tasks"""
     logger.info("Performing housekeeping")
     deleted_count = Timer.objects.delete_obsolete()
@@ -307,15 +321,15 @@
     for staging_system_pk in StagingSystem.objects.values_list("pk", flat=True):
         calc_timer_distances_for_staging_system.apply_async(
             kwargs={
                 "timer_pk": timer.pk,
                 "staging_system_pk": staging_system_pk,
                 "force_update": force_update,
             },
-            priority=TASK_PRIO_HIGH,
+            priority=TASK_PRIORITY_HIGH,
         )
 
 
 @shared_task(
     bind=True,
     max_retries=3,
     autoretry_for=(OSError,),
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/partials/preliminary_list_table.html` & `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/partials/preliminary_list_table.html`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/partials/timer_list_table.html` & `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/partials/timer_list_table.html`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/timer_confirm_delete.html` & `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_confirm_delete.html`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,14 @@
                     {% csrf_token %}
                     <p>
                         {% trans "Are you sure you want to delete timer this timer?" %}
                     </p>
                     <p>
                         <strong>{{ object }}</strong>
                     </p>
-                    <input class="btn btn-danger" type="submit" value="Delete" />
+                    <input class="btn btn-danger" type="submit" value="{% translate 'Delete' %}" />
                     {% include 'structuretimers/partials/cancel_button.html' %}
                 </form>
             </div>
         </div>
     </div>
 {% endblock content %}
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/timer_detail.html` & `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_detail.html`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/timer_edit.html` & `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_edit.html`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/templates/structuretimers/timer_list.html` & `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_list.html`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/test_admin.py` & `aa_structuretimers-1.5.0/structuretimers/tests/test_admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 from unittest.mock import patch
 
 from django.contrib.auth.models import User
 from django.test import TestCase, override_settings
 from django.urls import reverse
 from django_webtest import WebTest
 
-from ..models import DiscordWebhook, NotificationRule, StagingSystem, Timer
-from .testdata.factory import create_staging_system
+from structuretimers.models import NotificationRule, StagingSystem, Timer
+
+from .testdata.factory import (
+    create_discord_webhook,
+    create_notification_rule,
+    create_staging_system,
+)
 from .testdata.fixtures import LoadTestDataMixin
 
 
 @patch("structuretimers.models.STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
 class TestNotificationRuleChangeList(LoadTestDataMixin, WebTest):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
-        cls.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        cls.webhook = create_discord_webhook()
         cls.user = User.objects.create_superuser(
             "Bruce Wayne", "bruce@example.com", "password"
         )
 
     @patch("structuretimers.models.STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
     def setUp(self) -> None:
-        NotificationRule.objects.create(
+        create_notification_rule(
             trigger=NotificationRule.Trigger.SCHEDULED_TIME_REACHED,
             scheduled_time=NotificationRule.MINUTES_10,
             webhook=self.webhook,
         )
-        NotificationRule.objects.create(
+        create_notification_rule(
             trigger=NotificationRule.Trigger.SCHEDULED_TIME_REACHED,
             scheduled_time=NotificationRule.MINUTES_10,
             require_timer_types=[Timer.Type.ARMOR],
             webhook=self.webhook,
         )
-        rule = NotificationRule.objects.create(
+        rule = create_notification_rule(
             trigger=NotificationRule.Trigger.SCHEDULED_TIME_REACHED,
             scheduled_time=NotificationRule.MINUTES_10,
             webhook=self.webhook,
         )
         rule.require_corporations.add(self.corporation_1)
-        NotificationRule.objects.create(
+        create_notification_rule(
             trigger=NotificationRule.Trigger.SCHEDULED_TIME_REACHED,
             scheduled_time=NotificationRule.MINUTES_10,
             is_important=NotificationRule.Clause.EXCLUDED,
             webhook=self.webhook,
         )
 
     def test_can_open_page_normally(self):
@@ -60,17 +63,15 @@
 
 
 @patch("structuretimers.models.STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
 class TestNotificationRuleValidations(LoadTestDataMixin, WebTest):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
-        cls.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        cls.webhook = create_discord_webhook()
         cls.user = User.objects.create_superuser(
             "Bruce Wayne", "bruce@example.com", "password"
         )
         cls.url_add = reverse("admin:structuretimers_notificationrule_add")
         cls.url_changelist = reverse(
             "admin:structuretimers_notificationrule_changelist"
         )
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/test_commands.py` & `aa_structuretimers-1.5.0/structuretimers/tests/test_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,132 +6,126 @@
 from django.utils.timezone import now
 from eveuniverse.models import EveType
 
 from allianceauth.timerboard.models import Timer as AuthTimer
 from app_utils.django import app_labels
 from app_utils.testing import NoSocketsTestCase
 
-from ..models import Timer
+from structuretimers.models import Timer
+
 from .testdata.factory import create_user
 from .testdata.fixtures import LoadTestDataMixin
 
 PACKAGE_PATH = "structuretimers.management.commands"
 MODELS_PATH = "structuretimers.models"
 
+if "timerboard" in app_labels():
 
-@patch(MODELS_PATH + "._task_calc_timer_distances_for_all_staging_systems", Mock())
-@patch(MODELS_PATH + ".STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
-@patch(PACKAGE_PATH + ".structuretimers_migrate_timers.get_input")
-class TestMigirateTimers(LoadTestDataMixin, NoSocketsTestCase):
-    @classmethod
-    def setUpClass(cls) -> None:
-        super().setUpClass()
-        if "timerboard" not in app_labels():
-            raise KeyboardInterrupt(
-                "App `timerboard` is not installed, which is required for this test"
+    @patch(MODELS_PATH + "._task_calc_timer_distances_for_all_staging_systems", Mock())
+    @patch(MODELS_PATH + ".STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
+    @patch(PACKAGE_PATH + ".structuretimers_migrate_timers.get_input")
+    class TestMigirateTimers(LoadTestDataMixin, NoSocketsTestCase):
+        def setUp(self) -> None:
+            self.out = StringIO()
+            self.user = create_user(self.character_1)
+            self.auth_timer = AuthTimer.objects.create(
+                system="Abune",
+                planet_moon="Near Heydieles gate",
+                structure="Astrahus",
+                eve_time=now() + timedelta(hours=4),
+                eve_character=self.character_1,
+                eve_corp=self.corporation_1,
+                user=self.user,
             )
+            Timer.objects.all().delete()
+
+        def test_full_armor_friendly(self, mock_get_input):
+            mock_get_input.return_value = "Y"
+            self.auth_timer.details = "Armor timer"
+            self.auth_timer.objective = "Friendly"
+            self.auth_timer.save()
+
+            call_command("structuretimers_migrate_timers", stdout=self.out)
+
+            new_timer = Timer.objects.first()
+            self.assertEqual(new_timer.eve_solar_system, self.system_abune)
+            self.assertEqual(new_timer.structure_type, self.type_astrahus)
+            self.assertEqual(new_timer.timer_type, Timer.Type.ARMOR)
+            self.assertEqual(new_timer.details_notes, "Armor timer")
+            self.assertEqual(new_timer.objective, Timer.Objective.FRIENDLY)
+            self.assertEqual(new_timer.date, self.auth_timer.eve_time)
+            self.assertEqual(new_timer.eve_character, self.character_1)
+            self.assertEqual(new_timer.eve_corporation, self.corporation_1)
+            self.assertEqual(new_timer.user, self.auth_timer.user)
+
+        def test_hull_hostile(self, mock_get_input):
+            mock_get_input.return_value = "Y"
+            self.auth_timer.details = "Hull timer"
+            self.auth_timer.objective = "Hostile"
+            self.auth_timer.save()
+
+            call_command("structuretimers_migrate_timers", stdout=self.out)
+
+            new_timer = Timer.objects.first()
+            self.assertEqual(new_timer.timer_type, Timer.Type.HULL)
+            self.assertEqual(new_timer.objective, Timer.Objective.HOSTILE)
+
+        def test_anchoring(self, mock_get_input):
+            mock_get_input.return_value = "Y"
+            self.auth_timer.details = "Anchor timer"
+            self.auth_timer.objective = "Neutral"
+            self.auth_timer.save()
+
+            call_command("structuretimers_migrate_timers", stdout=self.out)
+
+            new_timer = Timer.objects.first()
+            self.assertEqual(new_timer.timer_type, Timer.Type.ANCHORING)
+            self.assertEqual(new_timer.objective, Timer.Objective.NEUTRAL)
+
+        def test_final_corp_timer(self, mock_get_input):
+            mock_get_input.return_value = "Y"
+            self.auth_timer.details = "Final timer"
+            self.auth_timer.corp_timer = True
+            self.auth_timer.save()
+
+            call_command("structuretimers_migrate_timers", stdout=self.out)
+
+            new_timer = Timer.objects.first()
+            self.assertEqual(new_timer.timer_type, Timer.Type.FINAL)
+            self.assertEqual(new_timer.visibility, Timer.Visibility.CORPORATION)
+
+        def test_moon_mining(self, mock_get_input):
+            mock_get_input.return_value = "Y"
+            self.auth_timer.structure = "Moon Mining Cycle"
+            self.auth_timer.save()
+
+            call_command("structuretimers_migrate_timers", stdout=self.out)
+
+            new_timer = Timer.objects.first()
+            self.assertEqual(new_timer.timer_type, Timer.Type.MOONMINING)
+            self.assertEqual(new_timer.structure_type, EveType.objects.get(id=35835))
+
+        def test_abort_on_unknown_solar_system(self, mock_get_input):
+            mock_get_input.return_value = "Y"
+            self.auth_timer.system = "Unknown"
+            self.auth_timer.save()
+
+            call_command("structuretimers_migrate_timers", stdout=self.out)
+
+            self.assertFalse(Timer.objects.all().exists())
+
+        def test_abort_on_unknown_structure_type(self, mock_get_input):
+            mock_get_input.return_value = "Y"
+            self.auth_timer.structure = "Unknown"
+            self.auth_timer.save()
+
+            call_command("structuretimers_migrate_timers", stdout=self.out)
 
-    def setUp(self) -> None:
-        self.out = StringIO()
-        self.user = create_user(self.character_1)
-        self.auth_timer = AuthTimer.objects.create(
-            system="Abune",
-            planet_moon="Near Heydieles gate",
-            structure="Astrahus",
-            eve_time=now() + timedelta(hours=4),
-            eve_character=self.character_1,
-            eve_corp=self.corporation_1,
-            user=self.user,
-        )
-        Timer.objects.all().delete()
-
-    def test_full_armor_friendly(self, mock_get_input):
-        mock_get_input.return_value = "Y"
-        self.auth_timer.details = "Armor timer"
-        self.auth_timer.objective = "Friendly"
-        self.auth_timer.save()
-
-        call_command("structuretimers_migrate_timers", stdout=self.out)
-
-        new_timer = Timer.objects.first()
-        self.assertEqual(new_timer.eve_solar_system, self.system_abune)
-        self.assertEqual(new_timer.structure_type, self.type_astrahus)
-        self.assertEqual(new_timer.timer_type, Timer.Type.ARMOR)
-        self.assertEqual(new_timer.details_notes, "Armor timer")
-        self.assertEqual(new_timer.objective, Timer.Objective.FRIENDLY)
-        self.assertEqual(new_timer.date, self.auth_timer.eve_time)
-        self.assertEqual(new_timer.eve_character, self.character_1)
-        self.assertEqual(new_timer.eve_corporation, self.corporation_1)
-        self.assertEqual(new_timer.user, self.auth_timer.user)
-
-    def test_hull_hostile(self, mock_get_input):
-        mock_get_input.return_value = "Y"
-        self.auth_timer.details = "Hull timer"
-        self.auth_timer.objective = "Hostile"
-        self.auth_timer.save()
-
-        call_command("structuretimers_migrate_timers", stdout=self.out)
-
-        new_timer = Timer.objects.first()
-        self.assertEqual(new_timer.timer_type, Timer.Type.HULL)
-        self.assertEqual(new_timer.objective, Timer.Objective.HOSTILE)
-
-    def test_anchoring(self, mock_get_input):
-        mock_get_input.return_value = "Y"
-        self.auth_timer.details = "Anchor timer"
-        self.auth_timer.objective = "Neutral"
-        self.auth_timer.save()
-
-        call_command("structuretimers_migrate_timers", stdout=self.out)
-
-        new_timer = Timer.objects.first()
-        self.assertEqual(new_timer.timer_type, Timer.Type.ANCHORING)
-        self.assertEqual(new_timer.objective, Timer.Objective.NEUTRAL)
-
-    def test_final_corp_timer(self, mock_get_input):
-        mock_get_input.return_value = "Y"
-        self.auth_timer.details = "Final timer"
-        self.auth_timer.corp_timer = True
-        self.auth_timer.save()
-
-        call_command("structuretimers_migrate_timers", stdout=self.out)
-
-        new_timer = Timer.objects.first()
-        self.assertEqual(new_timer.timer_type, Timer.Type.FINAL)
-        self.assertEqual(new_timer.visibility, Timer.Visibility.CORPORATION)
-
-    def test_moon_mining(self, mock_get_input):
-        mock_get_input.return_value = "Y"
-        self.auth_timer.structure = "Moon Mining Cycle"
-        self.auth_timer.save()
-
-        call_command("structuretimers_migrate_timers", stdout=self.out)
-
-        new_timer = Timer.objects.first()
-        self.assertEqual(new_timer.timer_type, Timer.Type.MOONMINING)
-        self.assertEqual(new_timer.structure_type, EveType.objects.get(id=35835))
-
-    def test_abort_on_unknown_solar_system(self, mock_get_input):
-        mock_get_input.return_value = "Y"
-        self.auth_timer.system = "Unknown"
-        self.auth_timer.save()
-
-        call_command("structuretimers_migrate_timers", stdout=self.out)
-
-        self.assertFalse(Timer.objects.all().exists())
-
-    def test_abort_on_unknown_structure_type(self, mock_get_input):
-        mock_get_input.return_value = "Y"
-        self.auth_timer.structure = "Unknown"
-        self.auth_timer.save()
-
-        call_command("structuretimers_migrate_timers", stdout=self.out)
-
-        self.assertFalse(Timer.objects.all().exists())
+            self.assertFalse(Timer.objects.all().exists())
 
-    def test_do_not_create_duplicates(self, mock_get_input):
-        mock_get_input.return_value = "Y"
+        def test_do_not_create_duplicates(self, mock_get_input):
+            mock_get_input.return_value = "Y"
 
-        call_command("structuretimers_migrate_timers", stdout=self.out)
-        call_command("structuretimers_migrate_timers", stdout=self.out)
+            call_command("structuretimers_migrate_timers", stdout=self.out)
+            call_command("structuretimers_migrate_timers", stdout=self.out)
 
-        self.assertEqual(Timer.objects.all().count(), 1)
+            self.assertEqual(Timer.objects.all().count(), 1)
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/test_forms.py` & `aa_structuretimers-1.5.0/structuretimers/tests/test_forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from unittest.mock import Mock, patch
 
 from requests.exceptions import ConnectionError as NewConnectionError
 from requests.exceptions import HTTPError
 
 from app_utils.testing import NoSocketsTestCase
 
-from ..forms import TimerForm
-from ..models import Timer
+from structuretimers.forms import TimerForm
+from structuretimers.models import Timer
+
 from .testdata import test_image_filename
 from .testdata.factory import create_user
 from .testdata.fixtures import LoadTestDataMixin
 
 FORMS_PATH = "structuretimers.forms"
 MODELS_PATH = "structuretimers.models"
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/test_integration.py` & `aa_structuretimers-1.5.0/structuretimers/tests/test_integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 from unittest.mock import Mock, patch
 
 from django.test import TestCase, override_settings
 from django.urls import reverse
 from django.utils.timezone import now
 from django_webtest import WebTest
 
-from allianceauth.tests.auth_utils import AuthUtils
+from structuretimers.models import ScheduledNotification, Timer
+from structuretimers.tasks import send_test_message_to_webhook
 
-from ..models import DiscordWebhook, ScheduledNotification, Timer
-from ..tasks import send_test_message_to_webhook
-from .testdata.factory import create_notification_rule, create_timer, create_user
+from .testdata.factory import (
+    create_discord_webhook,
+    create_notification_rule,
+    create_timer,
+    create_user,
+)
 from .testdata.fixtures import LoadTestDataMixin
 from .utils import add_permission_to_user_by_name
 
 MODELS_PATH = "structuretimers.models"
 FORMS_PATH = "structuretimers.forms"
 TASKS_PATH = "structuretimers.tasks"
 
@@ -341,15 +345,15 @@
 
 
 """
 @patch(MODELS_PATH+ ".sleep", new=lambda x: x)
 @patch(MODELS_PATH+ ".dhooks_lite.Webhook.execute")
 class TestSendNotifications(LoadTestDataMixin, TestCase):
     def setUp(self) -> None:
-        self.webhook = DiscordWebhook.objects.create(
+        self.webhook = create_discord_webhook(
             name="Dummy", url="http://www.example.com"
         )
         self.rule = NotificationRule.objects.create(minutes=NotificationRule.MINUTES_0)
         self.rule.webhooks.add(self.webhook)
 
     def test_normal(self, mock_execute):
         create_timer(
@@ -365,18 +369,16 @@
 
 @override_settings(CELERY_ALWAYS_EAGER=True)
 @patch(MODELS_PATH + ".sleep", new=lambda x: x)
 @patch(TASKS_PATH + ".notify", spec=True)
 @patch(MODELS_PATH + ".dhooks_lite.Webhook.execute", spec=True)
 class TestTestMessageToWebhook(LoadTestDataMixin, TestCase):
     def setUp(self) -> None:
-        self.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
-        self.user = AuthUtils.create_user("John Doe")
+        self.webhook = create_discord_webhook()
+        self.user = create_user(self.character_1)
 
     def test_without_user(self, mock_execute, mock_notify):
         send_test_message_to_webhook.delay(webhook_pk=self.webhook.pk)
         self.assertEqual(mock_execute.call_count, 1)
         self.assertFalse(mock_notify.called)
 
     def test_with_user(self, mock_execute, mock_notify):
@@ -389,17 +391,15 @@
 
 @override_settings(CELERY_ALWAYS_EAGER=True, CELERY_EAGER_PROPAGATES_EXCEPTIONS=True)
 @patch(MODELS_PATH + "._task_calc_timer_distances_for_all_staging_systems", Mock())
 class TestTimerSave(LoadTestDataMixin, TestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
-        cls.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        cls.webhook = create_discord_webhook()
 
     def test_schedule_notifications_for_new_timers_2(self):
         # when
         create_notification_rule()
         timer = create_timer(
             date=now() + timedelta(hours=4),
             eve_solar_system=self.system_abune,
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/test_models.py` & `aa_structuretimers-1.5.0/structuretimers/tests/test_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,32 +11,34 @@
 from django.utils.timezone import now
 from eveuniverse.models import EveRegion, EveSolarSystem
 
 from allianceauth.eveonline.models import EveAllianceInfo, EveCorporationInfo
 from app_utils.json import JSONDateTimeDecoder
 from app_utils.testing import NoSocketsTestCase
 
-from .. import __title__
-from ..models import (
-    DiscordWebhook,
+from structuretimers import __title__
+from structuretimers.models import (
     NotificationRule,
     ScheduledNotification,
     StagingSystem,
     Timer,
     _task_calc_staging_system,
 )
+
 from .testdata.factory import (
+    create_discord_webhook,
     create_distances_from_staging,
     create_notification_rule,
     create_scheduled_notification,
     create_staging_system,
     create_timer,
     create_user,
 )
 from .testdata.fixtures import LoadTestDataMixin
+from .testdata.load_eveuniverse import load_eveuniverse
 from .utils import add_permission_to_user_by_name
 
 MODULE_PATH = "structuretimers.models"
 
 
 class TestTimer(LoadTestDataMixin, NoSocketsTestCase):
     def test_str_1(self):
@@ -114,17 +116,15 @@
 
 
 @patch(MODULE_PATH + "._task_calc_timer_distances_for_all_staging_systems", Mock())
 class TestTimerSaveXScheduleNotifications(LoadTestDataMixin, NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
-        cls.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        cls.webhook = create_discord_webhook()
 
     @patch(MODULE_PATH + "._task_schedule_notifications_for_timer")
     def test_schedule_notifications_for_new_timers(self, mock_schedule_notifications):
         timer = create_timer(
             date=now() + dt.timedelta(hours=4),
             eve_solar_system=self.system_abune,
             structure_type=self.type_astrahus,
@@ -188,15 +188,15 @@
     ):
         # when
         create_timer(timer_type=Timer.Type.PRELIMINARY)
         # then
         self.assertFalse(mock_schedule_notifications.called)
 
     @patch(MODULE_PATH + "._task_schedule_notifications_for_timer")
-    def test_remove_scheduled_notifications_when_timer_changed_to_prelimary(
+    def test_remove_scheduled_notifications_when_timer_changed_to_preliminary(
         self, mock_schedule_notifications
     ):
         # given
         rule = create_notification_rule(is_enabled=False)
         timer = create_timer(date=now() + dt.timedelta(hours=4))
         notification = create_scheduled_notification(
             notification_rule=rule, timer=timer
@@ -213,17 +213,15 @@
 
 
 @patch(MODULE_PATH + "._task_schedule_notifications_for_timer", Mock)
 class TestTimerSaveXCalcDistances(LoadTestDataMixin, NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
-        cls.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        cls.webhook = create_discord_webhook()
 
     @patch(MODULE_PATH + "._task_calc_timer_distances_for_all_staging_systems")
     def test_should_calc_distances_when_created(self, mock_calc_distances):
         # when
         timer = Timer.objects.create(
             date=now() + dt.timedelta(hours=4),
             eve_solar_system=self.system_abune,
@@ -261,14 +259,53 @@
         # when
         timer.structure_type = self.type_raitaru
         timer.save()
         # then
         self.assertFalse(mock_calc_distances.called)
 
 
+class TestTimerSpaceType(NoSocketsTestCase):
+    @classmethod
+    def setUpClass(cls) -> None:
+        super().setUpClass()
+        load_eveuniverse()
+
+    def test_can_detect_high_sec(self):
+        # when
+        result = Timer.SpaceType.from_eve_solar_system(
+            EveSolarSystem.objects.get(name="Jita")
+        )
+        # then
+        self.assertEqual(result, Timer.SpaceType.HIGH_SEC)
+
+    def test_can_detect_low_sec(self):
+        # when
+        result = Timer.SpaceType.from_eve_solar_system(
+            EveSolarSystem.objects.get(name="Abune")
+        )
+        # then
+        self.assertEqual(result, Timer.SpaceType.LOW_SEC)
+
+    def test_can_detect_null_sec(self):
+        # when
+        result = Timer.SpaceType.from_eve_solar_system(
+            EveSolarSystem.objects.get(name="HED-GP")
+        )
+        # then
+        self.assertEqual(result, Timer.SpaceType.NULL_SEC)
+
+    def test_can_detect_w_space(self):
+        # when
+        result = Timer.SpaceType.from_eve_solar_system(
+            EveSolarSystem.objects.get(name="J151645")
+        )
+        # then
+        self.assertEqual(result, Timer.SpaceType.WH_SPACE)
+
+
 @patch(MODULE_PATH + ".STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
 class TestTimerAccess(LoadTestDataMixin, NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         cls.user_1 = create_user(cls.character_1)
         cls.user_2 = create_user(cls.character_2)
@@ -405,17 +442,15 @@
 
 
 @patch(MODULE_PATH + ".DiscordWebhook.send_message", spec=True)
 class TestTimerSendNotification(LoadTestDataMixin, NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
-        cls.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        cls.webhook = create_discord_webhook()
 
     @patch(MODULE_PATH + ".STRUCTURETIMER_NOTIFICATION_SET_AVATAR", True)
     def test_should_send_minimal_notification(self, mock_send_message):
         # given
         timer = Timer(
             eve_solar_system=self.system_abune,
             structure_type=self.type_raitaru,
@@ -507,15 +542,15 @@
             eve_corporation=self.corporation_1,
             eve_solar_system=self.system_abune,
             structure_type=self.type_raitaru,
             timer_type=Timer.Type.HULL,
             objective=Timer.Objective.FRIENDLY,
         )
         self.timer_qs = Timer.objects.all()
-        self.webhook = DiscordWebhook.objects.create(name="Dummy", url="my-url")
+        self.webhook = create_discord_webhook()
 
     def test_conforms_with_notification_rule_1(self):
         """
         given two timers in qs
         when one timer conforms with notification rule
         then qs contains only conforming timer
         """
@@ -562,17 +597,15 @@
         self.assertSetEqual(
             set(new_qs.values_list("pk", flat=True)), {self.timer_1.pk, self.timer_2.pk}
         )
 
 
 class TestDiscordWebhook(LoadTestDataMixin, TestCase):
     def setUp(self) -> None:
-        self.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        self.webhook = create_discord_webhook(name="Dummy")
 
     def test_str(self):
         self.assertEqual(str(self.webhook), "Dummy")
 
     def test_repr(self):
         self.assertEqual(
             repr(self.webhook), f"DiscordWebhook(id={self.webhook.id}, name='Dummy')"
@@ -615,36 +648,34 @@
             self.webhook.send_message()
 
 
 @patch(MODULE_PATH + ".sleep", new=lambda x: x)
 @patch(MODULE_PATH + ".DiscordWebhook.send_message_to_webhook", spec=True)
 class TestDiscordWebhookSendQueuedMessages(TestCase):
     def setUp(self) -> None:
-        self.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        self.webhook = create_discord_webhook()
         self.webhook.clear_queue()
 
     def test_one_message(self, mock_send_message_to_webhook):
         """
-        when one mesage in queue
+        when one message in queue
         then send it and returns 1
         """
         mock_send_message_to_webhook.return_value = True
         self.webhook.send_message("dummy")
 
         result = self.webhook.send_queued_messages()
 
         self.assertEqual(result, 1)
         self.assertTrue(mock_send_message_to_webhook.called)
         self.assertEqual(self.webhook.queue_size(), 0)
 
     def test_three_message(self, mock_send_message_to_webhook):
         """
-        when three mesages in queue
+        when three messages in queue
         then sends them and returns 3
         """
         mock_send_message_to_webhook.return_value = True
         self.webhook.send_message("dummy-1")
         self.webhook.send_message("dummy-2")
         self.webhook.send_message("dummy-3")
 
@@ -682,17 +713,15 @@
         self.assertEqual(self.webhook.queue_size(), 1)
 
 
 @patch(MODULE_PATH + ".dhooks_lite.Webhook.execute", spec=True)
 @patch(MODULE_PATH + ".logger", spec=True)
 class TestDiscordWebhookSendMessageToWebhook(NoSocketsTestCase):
     def setUp(self) -> None:
-        self.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        self.webhook = create_discord_webhook()
 
     def test_send_normal(self, mock_logger, mock_execute):
         """
         when sending of message successful
         return True
         """
         mock_execute.return_value = dhooks_lite.WebhookResponse(
@@ -980,15 +1009,15 @@
         self.assertFalse(rule.is_matching_timer(timer))
 
 
 @patch(MODULE_PATH + ".STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
 class TestNotificationRuleQuerySet(LoadTestDataMixin, NoSocketsTestCase):
     @patch(MODULE_PATH + ".STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
     def setUp(self) -> None:
-        self.webhook = DiscordWebhook.objects.create(name="Dummy", url="my-url")
+        self.webhook = create_discord_webhook()
         self.rule_1 = create_notification_rule(
             trigger=NotificationRule.Trigger.SCHEDULED_TIME_REACHED,
             scheduled_time=10,
             require_timer_types=[Timer.Type.ARMOR],
             webhook=self.webhook,
         )
         self.rule_2 = create_notification_rule(
@@ -1063,15 +1092,15 @@
 
 
 @patch(MODULE_PATH + ".NotificationRule._import_schedule_notifications_for_rule")
 class TestNotificationRuleSave(LoadTestDataMixin, NoSocketsTestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
-        cls.webhook = DiscordWebhook.objects.create(name="dummy", url="dummy-url")
+        cls.webhook = create_discord_webhook(name="dummy", url="dummy-url")
 
     @patch(MODULE_PATH + ".STRUCTURETIMERS_NOTIFICATIONS_ENABLED", True)
     def test_scheduled_normal(self, mock_schedule_notifications):
         """
         given notifications are enabled
         when trigger is scheduled and enabled
         then schedule notifications
@@ -1127,15 +1156,15 @@
             webhook=self.webhook,
         )
         timer = create_timer(
             date=now() + dt.timedelta(hours=4),
             eve_solar_system=self.system_abune,
             structure_type=self.type_astrahus,
         )
-        obj = ScheduledNotification.objects.create(
+        obj = create_scheduled_notification(
             timer=timer,
             notification_rule=rule,
             timer_date=timer.date,
             notification_date=timer.date - dt.timedelta(minutes=10),
         )
         rule.trigger = NotificationRule.Trigger.NEW_TIMER_CREATED
         rule.scheduled_time = None
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/test_navigation_highlight.py` & `aa_structuretimers-1.5.0/structuretimers/tests/test_navigation_highlight.py`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/test_tasks.py` & `aa_structuretimers-1.5.0/structuretimers/tests/test_tasks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-from datetime import timedelta
+import datetime as dt
 from unittest.mock import Mock, patch
 
 from celery import Task
 
 from django.test import TestCase, TransactionTestCase
 from django.utils.timezone import now
 from eveuniverse.models import EveSolarSystem, EveType
 
-from ..models import DiscordWebhook, NotificationRule, ScheduledNotification, Timer
-from ..tasks import (
+from structuretimers.models import NotificationRule, ScheduledNotification, Timer
+from structuretimers.tasks import (
+    calc_timer_distances_for_all_staging_systems,
+    housekeeping,
     notify_about_new_timer,
     schedule_notifications_for_rule,
     schedule_notifications_for_timer,
     send_messages_for_webhook,
     send_scheduled_notification,
 )
-from .testdata.factory import create_timer
+
+from .testdata.factory import (
+    create_discord_webhook,
+    create_notification_rule,
+    create_scheduled_notification,
+    create_staging_system,
+    create_timer,
+)
 from .testdata.fixtures import LoadTestDataMixin
 from .testdata.load_eveuniverse import load_eveuniverse
 
 MODULE_PATH = "structuretimers.tasks"
 
 
 class TestCaseBase(LoadTestDataMixin, TestCase):
     @patch("structuretimers.models.STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
     def setUp(self) -> None:
-        self.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        self.webhook = create_discord_webhook()
         self.webhook.clear_queue()
-        self.rule = NotificationRule.objects.create(
+        self.rule = create_notification_rule(
             trigger=NotificationRule.Trigger.SCHEDULED_TIME_REACHED,
             scheduled_time=NotificationRule.MINUTES_15,
             webhook=self.webhook,
         )
         self.timer = create_timer(
             structure_name="Test_1",
             eve_solar_system=self.system_abune,
             structure_type=self.type_raitaru,
-            date=now() + timedelta(minutes=30),
+            date=now() + dt.timedelta(minutes=30),
         )
 
 
 @patch(MODULE_PATH + ".DiscordWebhook.send_queued_messages", spec=True)
 @patch(MODULE_PATH + ".logger", spec=True)
 class TestSendMessagesForWebhook(TestCaseBase):
     def test_normal(self, mock_logger, mock_send_queued_messages):
@@ -94,19 +101,19 @@
     ):
         """
         given existing notification
         when called for timer with matching notification rule and changed date
         then deletes existing notification and schedules new notification
         """
         mock_send_notification.apply_async.return_value.task_id = "my_task_id"
-        notification_old = ScheduledNotification.objects.create(
+        notification_old = create_scheduled_notification(
             timer=self.timer,
             notification_rule=self.rule,
-            timer_date=self.timer.date + timedelta(minutes=5),
-            notification_date=self.timer.date - timedelta(minutes=5),
+            timer_date=self.timer.date + dt.timedelta(minutes=5),
+            notification_date=self.timer.date - dt.timedelta(minutes=5),
             celery_task_id="99",
         )
 
         schedule_notifications_for_timer(timer_pk=self.timer.pk, is_new=True)
 
         self.assertTrue(mock_send_notification.apply_async.called)
         self.assertTrue(
@@ -124,15 +131,15 @@
         """
         given notification rule for sending new timers exists
         when called for timer
         then send new notification
         """
         self.rule.is_enabled = False
         self.rule.save()
-        rule = NotificationRule.objects.create(
+        rule = create_notification_rule(
             trigger=NotificationRule.Trigger.NEW_TIMER_CREATED, webhook=self.webhook
         )
         schedule_notifications_for_timer(timer_pk=self.timer.pk, is_new=True)
 
         self.assertTrue(mock_send_notification_for_timer.apply_async.called)
         _, kwargs = mock_send_notification_for_timer.apply_async.call_args
         self.assertEqual(kwargs["kwargs"]["timer_pk"], self.timer.pk)
@@ -148,14 +155,25 @@
         """
         self.rule.is_enabled = False
         self.rule.save()
         schedule_notifications_for_timer(timer_pk=self.timer.pk, is_new=True)
 
         self.assertFalse(mock_send_notification_for_timer.apply_async.called)
 
+    def test_should_abort_when_outdated(
+        self, mock_send_notification, mock_send_notification_for_timer
+    ):
+        # given
+        self.timer.date = now() - dt.timedelta(hours=1)
+        self.timer.save()
+        # when
+        schedule_notifications_for_timer(timer_pk=self.timer.pk, is_new=True)
+        # then
+        self.assertFalse(mock_send_notification_for_timer.apply_async.called)
+
 
 @patch(MODULE_PATH + ".send_scheduled_notification", spec=True)
 class TestScheduleNotificationForRule(TestCaseBase):
     def test_normal(self, mock_send_notification):
         """
         given no notifications scheduled
         when called for notification rule with matching timer
@@ -175,19 +193,19 @@
     def test_remove_old_notifications(self, mock_send_notification):
         """
         given existing notification
         when called for notification rule with matching timer
         then deletes existing notification and schedules new notification
         """
         mock_send_notification.apply_async.return_value.task_id = "my_task_id"
-        notification_old = ScheduledNotification.objects.create(
+        notification_old = create_scheduled_notification(
             timer=self.timer,
             notification_rule=self.rule,
-            timer_date=self.timer.date + timedelta(minutes=5),
-            notification_date=self.timer.date - timedelta(minutes=5),
+            timer_date=self.timer.date + dt.timedelta(minutes=5),
+            notification_date=self.timer.date - dt.timedelta(minutes=5),
             celery_task_id="99",
         )
 
         schedule_notifications_for_rule(self.rule.pk)
 
         self.assertTrue(mock_send_notification.apply_async.called)
         self.assertTrue(
@@ -195,51 +213,58 @@
                 notification_rule=self.rule
             ).exists()
         )
         self.assertFalse(
             ScheduledNotification.objects.filter(pk=notification_old.pk).exists()
         )
 
+    def test_abort_when_has_the_wrong_trigger(self, mock_send_notification):
+        # given
+        self.rule.trigger = NotificationRule.Trigger.NEW_TIMER_CREATED
+        self.rule.save()
+        # when
+        schedule_notifications_for_rule(self.rule.pk)
+        # then
+        self.assertFalse(mock_send_notification.apply_async.called)
+
 
 @patch("structuretimers.models.STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
 @patch(MODULE_PATH + ".send_messages_for_webhook", spec=True)
 class TestSendScheduledNotification(TransactionTestCase):
     @patch("structuretimers.models.STRUCTURETIMERS_NOTIFICATIONS_ENABLED", False)
     def setUp(self) -> None:
         load_eveuniverse()
         self.type_raitaru = EveType.objects.get(id=35825)
         self.system_abune = EveSolarSystem.objects.get(id=30004984)
-        self.webhook = DiscordWebhook.objects.create(
-            name="Dummy", url="http://www.example.com"
-        )
+        self.webhook = create_discord_webhook()
         self.webhook.clear_queue()
-        self.rule = NotificationRule.objects.create(
+        self.rule = create_notification_rule(
             trigger=NotificationRule.Trigger.SCHEDULED_TIME_REACHED,
             scheduled_time=NotificationRule.MINUTES_15,
             webhook=self.webhook,
         )
         self.timer = create_timer(
             structure_name="Test_1",
             eve_solar_system=self.system_abune,
             structure_type=self.type_raitaru,
-            date=now() + timedelta(minutes=30),
+            date=now() + dt.timedelta(minutes=30),
         )
         ScheduledNotification.objects.all().delete()
 
     def test_normal(self, mock_send_messages_for_webhook):
         """
         when this notification is correctly scheduled
         then send the notification
         """
-        scheduled_notification = ScheduledNotification.objects.create(
+        scheduled_notification = create_scheduled_notification(
             timer=self.timer,
             notification_rule=self.rule,
             celery_task_id="my-id-123",
-            timer_date=now() + timedelta(hours=1),
-            notification_date=now() + timedelta(minutes=30),
+            timer_date=now() + dt.timedelta(hours=1),
+            notification_date=now() + dt.timedelta(minutes=30),
         )
         mock_task = Mock(spec=Task)
         mock_task.request.id = "my-id-123"
         send_scheduled_notification_inner = (
             send_scheduled_notification.__wrapped__.__func__
         )
         send_scheduled_notification_inner(
@@ -248,20 +273,20 @@
         self.assertTrue(mock_send_messages_for_webhook.apply_async.called)
 
     def test_revoked_notification(self, mock_send_messages_for_webhook):
         """
         when this is not the right task instance
         then discard this notification
         """
-        scheduled_notification = ScheduledNotification.objects.create(
+        scheduled_notification = create_scheduled_notification(
             timer=self.timer,
             notification_rule=self.rule,
             celery_task_id="my-id-123",
-            timer_date=now() + timedelta(hours=1),
-            notification_date=now() + timedelta(minutes=30),
+            timer_date=now() + dt.timedelta(hours=1),
+            notification_date=now() + dt.timedelta(minutes=30),
         )
         mock_task = Mock(**{"request.id": "my-id-456"})
         send_scheduled_notification_inner = (
             send_scheduled_notification.__wrapped__.__func__
         )
         send_scheduled_notification_inner(
             mock_task, scheduled_notification_pk=scheduled_notification.pk
@@ -271,56 +296,195 @@
     def test_rule_disabled(self, mock_send_messages_for_webhook):
         """
         when the notification rule for this scheduled notification is disabled
         then discard notification
         """
         self.rule.is_enabled = False
         self.rule.save()
-        scheduled_notification = ScheduledNotification.objects.create(
+        scheduled_notification = create_scheduled_notification(
             timer=self.timer,
             notification_rule=self.rule,
             celery_task_id="my-id-123",
-            timer_date=now() + timedelta(hours=1),
-            notification_date=now() + timedelta(minutes=30),
+            timer_date=now() + dt.timedelta(hours=1),
+            notification_date=now() + dt.timedelta(minutes=30),
         )
         mock_task = Mock(spec=Task)
         mock_task.request.id = "my-id-123"
         send_scheduled_notification_inner = (
             send_scheduled_notification.__wrapped__.__func__
         )
         send_scheduled_notification_inner(
             mock_task, scheduled_notification_pk=scheduled_notification.pk
         )
         self.assertFalse(mock_send_messages_for_webhook.apply_async.called)
 
+    def test_should_ignore_when_notification_was_deleted(
+        self, mock_send_messages_for_webhook
+    ):
+        # given
+        mock_task = Mock(spec=Task)
+        mock_task.request.id = "my-id-123"
+        send_scheduled_notification_inner = (
+            send_scheduled_notification.__wrapped__.__func__
+        )
+        # when
+        send_scheduled_notification_inner(mock_task, scheduled_notification_pk=666)
+        # then
+        self.assertFalse(mock_send_messages_for_webhook.apply_async.called)
 
-@patch(MODULE_PATH + ".send_messages_for_webhook", spec=True)
-class TestSendNotificationForTimer(TestCaseBase):
-    def setUp(self) -> None:
-        super().setUp()
-        self.rule_2 = NotificationRule.objects.create(
-            trigger=NotificationRule.Trigger.NEW_TIMER_CREATED, webhook=self.webhook
+    def test_should_abort_when_webhook_disabled(self, mock_send_messages_for_webhook):
+        # given
+        scheduled_notification = create_scheduled_notification(
+            timer=self.timer,
+            notification_rule=self.rule,
+            celery_task_id="my-id-123",
+            timer_date=now() + dt.timedelta(hours=1),
+            notification_date=now() + dt.timedelta(minutes=30),
+        )
+        mock_task = Mock(spec=Task)
+        mock_task.request.id = "my-id-123"
+        send_scheduled_notification_inner = (
+            send_scheduled_notification.__wrapped__.__func__
+        )
+        self.webhook.is_enabled = False
+        self.webhook.save()
+        # when
+        send_scheduled_notification_inner(
+            mock_task, scheduled_notification_pk=scheduled_notification.pk
+        )
+        # then
+        self.assertFalse(mock_send_messages_for_webhook.apply_async.called)
+
+    def test_should_discard_when_timer_is_outdated(
+        self, mock_send_messages_for_webhook
+    ):
+        # given
+        self.timer.date = now() - dt.timedelta(hours=1)
+        self.timer.save()
+        scheduled_notification = create_scheduled_notification(
+            timer=self.timer,
+            notification_rule=self.rule,
+            celery_task_id="my-id-123",
+            timer_date=now() + dt.timedelta(hours=1),
+            notification_date=now() + dt.timedelta(minutes=30),
+        )
+        mock_task = Mock(spec=Task)
+        mock_task.request.id = "my-id-123"
+        send_scheduled_notification_inner = (
+            send_scheduled_notification.__wrapped__.__func__
+        )
+        # when
+        send_scheduled_notification_inner(
+            mock_task, scheduled_notification_pk=scheduled_notification.pk
+        )
+        # then
+        self.assertFalse(mock_send_messages_for_webhook.apply_async.called)
+
+    def test_should_discard_when_timer_date_is_outdated(
+        self, mock_send_messages_for_webhook
+    ):
+        # given
+        self.timer.save()
+        scheduled_notification = create_scheduled_notification(
+            timer=self.timer,
+            notification_rule=self.rule,
+            celery_task_id="my-id-123",
+            timer_date=now() - dt.timedelta(hours=1),
+            notification_date=now() + dt.timedelta(minutes=30),
         )
+        mock_task = Mock(spec=Task)
+        mock_task.request.id = "my-id-123"
+        send_scheduled_notification_inner = (
+            send_scheduled_notification.__wrapped__.__func__
+        )
+        # when
+        send_scheduled_notification_inner(
+            mock_task, scheduled_notification_pk=scheduled_notification.pk
+        )
+        # then
+        self.assertFalse(mock_send_messages_for_webhook.apply_async.called)
+
 
+@patch(MODULE_PATH + ".send_messages_for_webhook", spec=True)
+class TestSendNotificationForTimer(TestCaseBase):
     def test_normal(self, mock_send_messages_for_webhook):
         """
         given rule for notifying about new timers exist
         when calling task for a timer
         then send notification for that timer
         """
-        notify_about_new_timer(self.timer.pk, self.rule_2.pk)
-
+        # given
+        rule = create_notification_rule(
+            trigger=NotificationRule.Trigger.NEW_TIMER_CREATED, webhook=self.webhook
+        )
+        # when
+        notify_about_new_timer(self.timer.pk, rule.pk)
+        # then
         self.assertTrue(mock_send_messages_for_webhook.apply_async.called)
         _, kwargs = mock_send_messages_for_webhook.apply_async.call_args
         self.assertListEqual(kwargs["args"], [self.webhook.pk])
 
     def test_webhook_disabled(self, mock_send_messages_for_webhook):
         """
         given rule for notifying about new timers does NOT exist
         when calling task for a timer
         then send notification for that timer
         """
-        notify_about_new_timer(self.timer.pk, self.rule_2.pk)
-
+        # given
+        rule = create_notification_rule(
+            trigger=NotificationRule.Trigger.NEW_TIMER_CREATED, webhook=self.webhook
+        )
+        # when
+        notify_about_new_timer(self.timer.pk, rule.pk)
+        # then
         self.assertTrue(mock_send_messages_for_webhook.apply_async.called)
         _, kwargs = mock_send_messages_for_webhook.apply_async.call_args
         self.assertListEqual(kwargs["args"], [self.webhook.pk])
+
+    def test_rule_disabled(self, mock_send_messages_for_webhook):
+        """
+        when is disabled
+        then abort
+        """
+        # given
+        rule = create_notification_rule(
+            trigger=NotificationRule.Trigger.NEW_TIMER_CREATED,
+            webhook=self.webhook,
+            is_enabled=False,
+        )
+        # when
+        notify_about_new_timer(self.timer.pk, rule.pk)
+        # then
+        self.assertFalse(mock_send_messages_for_webhook.apply_async.called)
+
+
+@patch(MODULE_PATH + ".Timer.objects.delete_obsolete", spec=True)
+class TestHousekeeping(TestCase):
+    def test_should_run_housekeeping(self, mock_delete_obsolete):
+        # given
+        mock_delete_obsolete.return_value = 1
+        # when
+        housekeeping()
+        # then
+        self.assertTrue(mock_delete_obsolete.called)
+
+
+@patch(MODULE_PATH + ".calc_timer_distances_for_staging_system", spec=True)
+class TestTimerDistancesForAllStagingSystems(TestCase):
+    def test_should_run_housekeeping(
+        self, mock_calc_timer_distances_for_staging_system
+    ):
+        # given
+        load_eveuniverse()
+        timer = create_timer(
+            structure_name="Test_1",
+            eve_solar_system=EveSolarSystem.objects.get(name="Abune"),
+            structure_type=EveType.objects.get(name="Astrahus"),
+            date=now() + dt.timedelta(minutes=30),
+        )
+        create_staging_system(light_years=10)
+        # when
+        calc_timer_distances_for_all_staging_systems(timer.pk)
+        # then
+        self.assertEqual(
+            mock_calc_timer_distances_for_staging_system.apply_async.call_count, 1
+        )
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/test_views.py` & `aa_structuretimers-1.5.0/structuretimers/tests/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from datetime import timedelta
+from typing import Optional
 from unittest.mock import Mock, patch
 
 from django.contrib.auth.models import User
 from django.test import TestCase
 from django.urls import reverse
 from django.utils.timezone import now
 
 from app_utils.testing import (
     create_user_from_evecharacter,
     json_response_to_dict,
     json_response_to_python,
 )
 
-from ..models import Timer
+from structuretimers.models import Timer
+
 from .testdata.factory import create_staging_system, create_timer, create_user
 from .testdata.fixtures import LoadTestDataMixin
 from .utils import add_permission_to_user_by_name
 
 MODELS_PATH = "structuretimers.models"
 
 
@@ -145,24 +147,26 @@
         response = self.client.get("/structuretimers/")
         # then
         self.assertEqual(response.status_code, 200)
         self.assertIsNone(response.context_data["selected_staging_system"])
 
 
 class TestListData(TestViewBase):
-    def _get_timer_list_data(self, tab_name: str = "current", user: User = None):
+    def _get_timer_list_data(
+        self, tab_name: str = "current", user: Optional[User] = None
+    ):
         if not user:
             user = self.user_1
         self.client.force_login(user)
         return self.client.get(
             reverse("structuretimers:timer_list_data", args=[tab_name])
         )
 
     def _get_timer_list_data_ids(
-        self, tab_name: str = "current", user: User = None
+        self, tab_name: str = "current", user: Optional[User] = None
     ) -> set:
         response = self._get_timer_list_data(tab_name, user)
         self.assertEqual(response.status_code, 200)
         return set(json_response_to_dict(response).keys())
 
     # def test_timer_list_view_loads(self):
     #     request = self.factory.get(reverse("structuretimers:timer_list"))
@@ -515,15 +519,15 @@
             reverse("structuretimers:select2_structure_types"), data={"term": "ast"}
         )
         # then
         self.assertEqual(response.status_code, 200)
         data = json_response_to_python(response)
         self.assertEqual(data, {"results": [{"id": 35832, "text": "Astrahus"}]})
 
-    def test_should_return_empty_struture_types_list(self):
+    def test_should_return_empty_structure_types_list(self):
         # given
         self.client.force_login(self.user_1)
         # when
         response = self.client.get(reverse("structuretimers:select2_structure_types"))
         # then
         self.assertEqual(response.status_code, 200)
         data = json_response_to_python(response)
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/testdata/factory.py` & `aa_structuretimers-1.5.0/structuretimers/tests/testdata/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,41 +91,41 @@
                     staging_system=staging_system,
                     timer=timer,
                     defaults={"light_years": light_years, "jumps": jumps},
                 )
         return staging_system
 
 
-def create_discord_webhook(*args, **kwargs):
+def create_discord_webhook(**kwargs):
     if "name" not in kwargs:
         while True:
             name = f"dummy{random_string(8)}"
             if not DiscordWebhook.objects.filter(name=name).exists():
                 break
         kwargs["name"] = name
     if "url" not in kwargs:
         kwargs["url"] = f"https://www.example.com/{kwargs['name']}"
-    return DiscordWebhook.objects.create(*args, **kwargs)
+    return DiscordWebhook.objects.create(**kwargs)
 
 
-def create_notification_rule(schedule_notification=False, *args, **kwargs):
+def create_notification_rule(schedule_notification=False, **kwargs):
     if "webhook" not in kwargs:
         kwargs["webhook"] = create_discord_webhook()
     if "trigger" not in kwargs:
         kwargs["trigger"] = NotificationRule.Trigger.SCHEDULED_TIME_REACHED
     if "scheduled_time" not in kwargs:
         kwargs["scheduled_time"] = 60
     with patch(
         "structuretimers.models.STRUCTURETIMERS_NOTIFICATIONS_ENABLED",
         schedule_notification,
     ):
-        return NotificationRule.objects.create(*args, **kwargs)
+        return NotificationRule.objects.create(**kwargs)
 
 
-def create_scheduled_notification(*args, **kwargs):
+def create_scheduled_notification(**kwargs):
     if "timer_date" not in kwargs:
         kwargs["timer_date"] = now() + dt.timedelta(hours=1)
     if "notification_date" not in kwargs:
         kwargs["notification_date"] = now() + dt.timedelta(minutes=45)
     if "celery_task_id" not in kwargs:
         kwargs["celery_task_id"] = random_string(8)
-    return ScheduledNotification.objects.create(*args, **kwargs)
+    return ScheduledNotification.objects.create(**kwargs)
```

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/testdata/fixtures.py` & `aa_structuretimers-1.5.0/structuretimers/tests/testdata/fixtures.py`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/tests/testdata/generate_timers.py` & `aa_structuretimers-1.5.0/structuretimers/tests/testdata/generate_timers.py`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/urls.py` & `aa_structuretimers-1.5.0/structuretimers/urls.py`

 * *Files identical despite different names*

### Comparing `aa-structuretimers-1.4.2/structuretimers/views.py` & `aa_structuretimers-1.5.0/structuretimers/views.py`

 * *Files identical despite different names*

