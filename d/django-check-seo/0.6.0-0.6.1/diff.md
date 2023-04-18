# Comparing `tmp/django-check-seo-0.6.0.tar.gz` & `tmp/django-check-seo-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-check-seo-0.6.0.tar", last modified: Fri Mar  3 15:46:54 2023, max compression
+gzip compressed data, was "django-check-seo-0.6.1.tar", last modified: Tue Apr 18 13:51:14 2023, max compression
```

## Comparing `django-check-seo-0.6.0.tar` & `django-check-seo-0.6.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.877972 django-check-seo-0.6.0/
--rw-r--r--   0 kapt      (1000) kapt      (1000)       93 2023-03-03 15:46:27.000000 django-check-seo-0.6.0/.bumpversion.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)      365 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/.coveragerc
--rw-r--r--   0 kapt      (1000) kapt      (1000)       74 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/.flake8
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.845972 django-check-seo-0.6.0/.github/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.857972 django-check-seo-0.6.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      834 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)      595 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)      130 2021-09-09 16:31:58.000000 django-check-seo-0.6.0/.gitignore
--rw-r--r--   0 kapt      (1000) kapt      (1000)      113 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/.isort.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)      797 2022-06-14 09:16:04.000000 django-check-seo-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 kapt      (1000) kapt      (1000)       78 2021-09-09 16:31:58.000000 django-check-seo-0.6.0/AUTHORS.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)    16299 2023-03-03 15:46:31.000000 django-check-seo-0.6.0/CHANGELOG.rst
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1554 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 kapt      (1000) kapt      (1000)    35149 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/LICENSE
--rw-r--r--   0 kapt      (1000) kapt      (1000)      220 2022-06-14 08:10:41.000000 django-check-seo-0.6.0/MANIFEST.in
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6719 2023-03-03 15:46:54.877972 django-check-seo-0.6.0/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5635 2022-09-21 15:59:55.000000 django-check-seo-0.6.0/README.md
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.857972 django-check-seo-0.6.0/django_check_seo/
--rw-r--r--   0 kapt      (1000) kapt      (1000)       66 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      181 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/apps.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.861972 django-check-seo-0.6.0/django_check_seo/checks/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/checks/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      320 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/checks/custom_list.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1778 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/checks/site.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.865972 django-check-seo-0.6.0/django_check_seo/checks_list/
--rw-r--r--   0 kapt      (1000) kapt      (1000)      418 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/checks_list/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     7826 2023-03-03 15:45:59.000000 django-check-seo-0.6.0/django_check_seo/checks_list/check_description.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4001 2022-06-14 09:17:55.000000 django-check-seo-0.6.0/django_check_seo/checks_list/check_h1.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3793 2022-06-14 09:17:55.000000 django-check-seo-0.6.0/django_check_seo/checks_list/check_h2.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2914 2022-06-14 09:27:26.000000 django-check-seo-0.6.0/django_check_seo/checks_list/check_images.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3931 2022-06-14 09:17:55.000000 django-check-seo-0.6.0/django_check_seo/checks_list/check_keyword_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2037 2022-06-14 09:17:55.000000 django-check-seo-0.6.0/django_check_seo/checks_list/check_keywords.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4092 2022-06-14 09:17:55.000000 django-check-seo-0.6.0/django_check_seo/checks_list/check_links.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5709 2022-06-14 09:17:55.000000 django-check-seo-0.6.0/django_check_seo/checks_list/check_title.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3367 2022-06-14 09:17:55.000000 django-check-seo-0.6.0/django_check_seo/checks_list/check_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2018 2022-06-14 09:17:55.000000 django-check-seo-0.6.0/django_check_seo/checks_list/content_words_number.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2453 2022-06-14 09:17:55.000000 django-check-seo-0.6.0/django_check_seo/checks_list/keyword_present_first_paragraph.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2052 2022-09-21 15:03:12.000000 django-check-seo-0.6.0/django_check_seo/checks_list/launch_checks.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      668 2023-03-03 15:45:59.000000 django-check-seo-0.6.0/django_check_seo/cms_toolbars.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.865972 django-check-seo-0.6.0/django_check_seo/conf/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/conf/__init__.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      815 2022-06-14 08:53:12.000000 django-check-seo-0.6.0/django_check_seo/conf/settings.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.849972 django-check-seo-0.6.0/django_check_seo/locale/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.849972 django-check-seo-0.6.0/django_check_seo/locale/fr/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.865972 django-check-seo-0.6.0/django_check_seo/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    16533 2022-06-14 09:38:51.000000 django-check-seo-0.6.0/django_check_seo/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt      (1000) kapt      (1000)    24514 2022-06-14 09:38:24.000000 django-check-seo-0.6.0/django_check_seo/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.865972 django-check-seo-0.6.0/django_check_seo/migrations/
--rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/migrations/__init__.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.849972 django-check-seo-0.6.0/django_check_seo/static/
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.865972 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4734 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/design.css
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.869972 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    11358 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/LICENCE
--rw-r--r--   0 kapt      (1000) kapt      (1000)      139 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/NOTICE
--rw-r--r--   0 kapt      (1000) kapt      (1000)   164936 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   163448 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   162636 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   158604 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)   122512 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf
--rw-r--r--   0 kapt      (1000) kapt      (1000)    15388 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/logo-small.png
--rw-r--r--   0 kapt      (1000) kapt      (1000)   137074 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/static/django-check-seo/logo.png
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.873972 django-check-seo-0.6.0/django_check_seo/templates/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3231 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/templates/default.html
--rw-r--r--   0 kapt      (1000) kapt      (1000)      665 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/django_check_seo/templates/element.html
--rw-r--r--   0 kapt      (1000) kapt      (1000)      603 2022-06-20 09:56:51.000000 django-check-seo-0.6.0/django_check_seo/urls.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2926 2022-06-14 08:53:12.000000 django-check-seo-0.6.0/django_check_seo/views.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.861972 django-check-seo-0.6.0/django_check_seo.egg-info/
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6719 2023-03-03 15:46:54.000000 django-check-seo-0.6.0/django_check_seo.egg-info/PKG-INFO
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2490 2023-03-03 15:46:54.000000 django-check-seo-0.6.0/django_check_seo.egg-info/SOURCES.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2023-03-03 15:46:54.000000 django-check-seo-0.6.0/django_check_seo.egg-info/dependency_links.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       49 2023-03-03 15:46:54.000000 django-check-seo-0.6.0/django_check_seo.egg-info/requires.txt
--rw-r--r--   0 kapt      (1000) kapt      (1000)       17 2023-03-03 15:46:54.000000 django-check-seo-0.6.0/django_check_seo.egg-info/top_level.txt
--rwxr-xr-x   0 kapt      (1000) kapt      (1000)     4701 2022-09-21 15:17:31.000000 django-check-seo-0.6.0/launch_tests.sh
--rw-r--r--   0 kapt      (1000) kapt      (1000)       94 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/pytest.ini
--rw-r--r--   0 kapt      (1000) kapt      (1000)     1088 2023-03-03 15:46:54.877972 django-check-seo-0.6.0/setup.cfg
--rw-r--r--   0 kapt      (1000) kapt      (1000)       52 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/setup.py
-drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-03-03 15:46:54.877972 django-check-seo-0.6.0/tests/
--rw-r--r--   0 kapt      (1000) kapt      (1000)    16223 2021-09-09 16:31:52.000000 django-check-seo-0.6.0/tests/test_content_words_number.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     9522 2021-09-09 16:31:52.000000 django-check-seo-0.6.0/tests/test_description.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6045 2021-09-09 16:31:52.000000 django-check-seo-0.6.0/tests/test_h1.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6469 2021-09-09 16:31:52.000000 django-check-seo-0.6.0/tests/test_h2.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     4439 2021-09-09 16:31:52.000000 django-check-seo-0.6.0/tests/test_images.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5135 2021-09-09 16:31:52.000000 django-check-seo-0.6.0/tests/test_keyword_present_first_paragraph.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     5989 2021-09-09 16:31:58.000000 django-check-seo-0.6.0/tests/test_keyword_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     2476 2021-09-09 16:31:52.000000 django-check-seo-0.6.0/tests/test_keywords.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     6480 2021-09-09 16:31:52.000000 django-check-seo-0.6.0/tests/test_links.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     7288 2021-09-09 16:31:52.000000 django-check-seo-0.6.0/tests/test_title.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)     3672 2021-09-09 16:31:52.000000 django-check-seo-0.6.0/tests/test_url.py
--rw-r--r--   0 kapt      (1000) kapt      (1000)      618 2021-09-08 08:29:05.000000 django-check-seo-0.6.0/tests_settings.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.847270 django-check-seo-0.6.1/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       93 2023-04-18 13:50:06.000000 django-check-seo-0.6.1/.bumpversion.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      365 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/.coveragerc
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       74 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/.flake8
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.819269 django-check-seo-0.6.1/.github/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.831269 django-check-seo-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      834 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      595 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      130 2021-09-09 16:31:58.000000 django-check-seo-0.6.1/.gitignore
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      113 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/.isort.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      797 2022-06-14 09:16:04.000000 django-check-seo-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       78 2021-09-09 16:31:58.000000 django-check-seo-0.6.1/AUTHORS.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    16524 2023-04-18 13:50:09.000000 django-check-seo-0.6.1/CHANGELOG.rst
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1554 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    35149 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/LICENSE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      220 2022-06-14 08:10:41.000000 django-check-seo-0.6.1/MANIFEST.in
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6745 2023-04-18 13:51:14.847270 django-check-seo-0.6.1/PKG-INFO
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5661 2023-04-18 13:48:27.000000 django-check-seo-0.6.1/README.md
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.831269 django-check-seo-0.6.1/django_check_seo/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       66 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      181 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/apps.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.835270 django-check-seo-0.6.1/django_check_seo/checks/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/checks/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      320 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/checks/custom_list.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1778 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/checks/site.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.839269 django-check-seo-0.6.1/django_check_seo/checks_list/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      418 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/checks_list/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     7826 2023-03-03 15:45:59.000000 django-check-seo-0.6.1/django_check_seo/checks_list/check_description.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4001 2022-06-14 09:17:55.000000 django-check-seo-0.6.1/django_check_seo/checks_list/check_h1.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3793 2022-06-14 09:17:55.000000 django-check-seo-0.6.1/django_check_seo/checks_list/check_h2.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2914 2022-06-14 09:27:26.000000 django-check-seo-0.6.1/django_check_seo/checks_list/check_images.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3931 2022-06-14 09:17:55.000000 django-check-seo-0.6.1/django_check_seo/checks_list/check_keyword_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2037 2022-06-14 09:17:55.000000 django-check-seo-0.6.1/django_check_seo/checks_list/check_keywords.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4092 2022-06-14 09:17:55.000000 django-check-seo-0.6.1/django_check_seo/checks_list/check_links.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5709 2022-06-14 09:17:55.000000 django-check-seo-0.6.1/django_check_seo/checks_list/check_title.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3367 2022-06-14 09:17:55.000000 django-check-seo-0.6.1/django_check_seo/checks_list/check_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2018 2022-06-14 09:17:55.000000 django-check-seo-0.6.1/django_check_seo/checks_list/content_words_number.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2453 2022-06-14 09:17:55.000000 django-check-seo-0.6.1/django_check_seo/checks_list/keyword_present_first_paragraph.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2052 2022-09-21 15:03:12.000000 django-check-seo-0.6.1/django_check_seo/checks_list/launch_checks.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      668 2023-03-03 15:45:59.000000 django-check-seo-0.6.1/django_check_seo/cms_toolbars.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.839269 django-check-seo-0.6.1/django_check_seo/conf/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/conf/__init__.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      815 2022-06-14 08:53:12.000000 django-check-seo-0.6.1/django_check_seo/conf/settings.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.823269 django-check-seo-0.6.1/django_check_seo/locale/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.823269 django-check-seo-0.6.1/django_check_seo/locale/fr/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.839269 django-check-seo-0.6.1/django_check_seo/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    16533 2022-06-14 09:38:51.000000 django-check-seo-0.6.1/django_check_seo/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    24514 2022-06-14 09:38:24.000000 django-check-seo-0.6.1/django_check_seo/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.839269 django-check-seo-0.6.1/django_check_seo/migrations/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        0 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/migrations/__init__.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.823269 django-check-seo-0.6.1/django_check_seo/static/
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.839269 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4734 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/design.css
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.843270 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    11358 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/LICENCE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      139 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/NOTICE
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   164936 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   163448 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   162636 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   158604 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   122512 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    15388 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/logo-small.png
+-rw-r--r--   0 kapt      (1000) kapt      (1000)   137074 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/static/django-check-seo/logo.png
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.843270 django-check-seo-0.6.1/django_check_seo/templates/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3231 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/templates/default.html
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      665 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/django_check_seo/templates/element.html
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      603 2022-06-20 09:56:51.000000 django-check-seo-0.6.1/django_check_seo/urls.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2939 2023-04-18 13:32:21.000000 django-check-seo-0.6.1/django_check_seo/views.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.831269 django-check-seo-0.6.1/django_check_seo.egg-info/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6745 2023-04-18 13:51:14.000000 django-check-seo-0.6.1/django_check_seo.egg-info/PKG-INFO
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2490 2023-04-18 13:51:14.000000 django-check-seo-0.6.1/django_check_seo.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)        1 2023-04-18 13:51:14.000000 django-check-seo-0.6.1/django_check_seo.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       49 2023-04-18 13:51:14.000000 django-check-seo-0.6.1/django_check_seo.egg-info/requires.txt
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       17 2023-04-18 13:51:14.000000 django-check-seo-0.6.1/django_check_seo.egg-info/top_level.txt
+-rwxr-xr-x   0 kapt      (1000) kapt      (1000)     4701 2022-09-21 15:17:31.000000 django-check-seo-0.6.1/launch_tests.sh
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       94 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/pytest.ini
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     1088 2023-04-18 13:51:14.851270 django-check-seo-0.6.1/setup.cfg
+-rw-r--r--   0 kapt      (1000) kapt      (1000)       52 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/setup.py
+drwxr-xr-x   0 kapt      (1000) kapt      (1000)        0 2023-04-18 13:51:14.847270 django-check-seo-0.6.1/tests/
+-rw-r--r--   0 kapt      (1000) kapt      (1000)    16223 2021-09-09 16:31:52.000000 django-check-seo-0.6.1/tests/test_content_words_number.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     9522 2021-09-09 16:31:52.000000 django-check-seo-0.6.1/tests/test_description.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6045 2021-09-09 16:31:52.000000 django-check-seo-0.6.1/tests/test_h1.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6469 2021-09-09 16:31:52.000000 django-check-seo-0.6.1/tests/test_h2.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     4439 2021-09-09 16:31:52.000000 django-check-seo-0.6.1/tests/test_images.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5135 2021-09-09 16:31:52.000000 django-check-seo-0.6.1/tests/test_keyword_present_first_paragraph.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     5989 2021-09-09 16:31:58.000000 django-check-seo-0.6.1/tests/test_keyword_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     2476 2021-09-09 16:31:52.000000 django-check-seo-0.6.1/tests/test_keywords.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     6480 2021-09-09 16:31:52.000000 django-check-seo-0.6.1/tests/test_links.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     7288 2021-09-09 16:31:52.000000 django-check-seo-0.6.1/tests/test_title.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)     3672 2021-09-09 16:31:52.000000 django-check-seo-0.6.1/tests/test_url.py
+-rw-r--r--   0 kapt      (1000) kapt      (1000)      618 2021-09-08 08:29:05.000000 django-check-seo-0.6.1/tests_settings.py
```

### Comparing `django-check-seo-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `django-check-seo-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `django-check-seo-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/.pre-commit-config.yaml` & `django-check-seo-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/CHANGELOG.rst` & `django-check-seo-0.6.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 Changelog
 =========
 
 
+v0.6.1 (2023-04-18)
+-------------------
+
+Documentation
+~~~~~~~~~~~~~
+- Update readme [Corentin Bettiol]
+- Update changelog [Corentin Bettiol]
+
+Other
+~~~~~
+- Have the test-client follow redirects on requests [Marco Bonetti]
+
+
 v0.6.0 (2023-03-03)
 -------------------
 
 Documentation
 ~~~~~~~~~~~~~
 - Update readme [Corentin Bettiol]
 - Update changelog [Corentin Bettiol]
```

### Comparing `django-check-seo-0.6.0/CONTRIBUTING.md` & `django-check-seo-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/LICENSE` & `django-check-seo-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/PKG-INFO` & `django-check-seo-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-check-seo
-Version: 0.6.0
+Version: 0.6.1
 Summary: Django Check SEO will check the SEO aspects of your site for you, and will provide advice in case of problems.
 Home-page: https://github.com/kapt-labs/django-check-seo
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
@@ -22,47 +22,53 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 ![Django Check SEO](https://user-images.githubusercontent.com/45763865/114545606-72178380-9c5c-11eb-99dd-1088bb2a0bd9.png)
 
-*Replacing some features of Yoast or SEMrush for django CMS users.*
+*Replacing some features of Yoast or SEMrush for Django & Django-CMS users.*
 
 In other words, django-check-seo will tell you if you have problems concerning a broad range of SEO aspects of your pages.
 
 ----
 
 [![PyPI](https://img.shields.io/pypi/v/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![GitHub last commit](https://img.shields.io/github/last-commit/kapt-labs/django-check-seo)](https://github.com/kapt-labs/django-check-seo)
 
 ----
 
 # Install
 
-*(for django >= 1.8.15 & python >= 2.7)*
+*(compatible with django >= 1.8.15 & python >= 2.7)*
 
 1. Install the module from [PyPI](https://pypi.org/project/django-check-seo/):
     ```
     python3 -m pip install django-check-seo
     ```
+
 2. Add it in your `INSTALLED_APPS`:
     ```
         "django_check_seo",
     ```
+
 3. Add this in your `urls.py` *(if you're using django-cms, put it before the `cms.urls` line or it will not work)*:
     ```
         path("django-check-seo/", include("django_check_seo.urls")),
     ```
     * *Or add this if you're still using `url` (you shouldn't):*
         ```
             url(r"^django-check-seo/", include("django_check_seo.urls")),
         ```
+
 4. Update your Django [Site](https://i.imgur.com/pNRsKs7.png) object parameters with a working url (here's an [example](https://i.imgur.com/IedF3xE.png) for dev environment).
+
 5. Add `testserver` to your `ALLOWED_HOSTS` list in your settings.py (django-check-seo uses the Test Framework in order to get content, instead of doing an HTTP request).
+
 6. *(optional) Configure the settings (see [config](#config)).*
+
 7. ![that's all folks!](https://i.imgur.com/o2Tcd2E.png)
 
 ----
 
 # Misc
 
 This application needs `beautifulsoup4` (>=4.7.0) and `djangocms_page_meta` *(==0.8.5 if using django < 1.11)*. It may be used with or without `django-cms` (a django-check-seo button will appear in the topbar if you're using django-cms).
@@ -138,15 +144,15 @@
 
 ```
 DJANGO_CHECK_SEO_EXCLUDE_CONTENT = "tag, .class, #id, tag > .child_class"
 ```
 
 *You can find a reference table of css selectors explained [here](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors#Reference_table_of_selectors) (on mdn docs).*
 
-### *Example: See [this issue's comment](https://github.com/kapt-labs/django-check-seo/issues/35#issuecomment-593429870) for an example.*
+## *Example: See [this issue's comment](https://github.com/kapt-labs/django-check-seo/issues/35#issuecomment-593429870) for an example.*
 
 ----
 
 # Want a screenshot?
 
 ![screenshot](https://i.imgur.com/hJGDvtw.png)
```

### Comparing `django-check-seo-0.6.0/README.md` & `django-check-seo-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 ![Django Check SEO](https://user-images.githubusercontent.com/45763865/114545606-72178380-9c5c-11eb-99dd-1088bb2a0bd9.png)
 
-*Replacing some features of Yoast or SEMrush for django CMS users.*
+*Replacing some features of Yoast or SEMrush for Django & Django-CMS users.*
 
 In other words, django-check-seo will tell you if you have problems concerning a broad range of SEO aspects of your pages.
 
 ----
 
 [![PyPI](https://img.shields.io/pypi/v/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![GitHub last commit](https://img.shields.io/github/last-commit/kapt-labs/django-check-seo)](https://github.com/kapt-labs/django-check-seo)
 
 ----
 
 # Install
 
-*(for django >= 1.8.15 & python >= 2.7)*
+*(compatible with django >= 1.8.15 & python >= 2.7)*
 
 1. Install the module from [PyPI](https://pypi.org/project/django-check-seo/):
     ```
     python3 -m pip install django-check-seo
     ```
+
 2. Add it in your `INSTALLED_APPS`:
     ```
         "django_check_seo",
     ```
+
 3. Add this in your `urls.py` *(if you're using django-cms, put it before the `cms.urls` line or it will not work)*:
     ```
         path("django-check-seo/", include("django_check_seo.urls")),
     ```
     * *Or add this if you're still using `url` (you shouldn't):*
         ```
             url(r"^django-check-seo/", include("django_check_seo.urls")),
         ```
+
 4. Update your Django [Site](https://i.imgur.com/pNRsKs7.png) object parameters with a working url (here's an [example](https://i.imgur.com/IedF3xE.png) for dev environment).
+
 5. Add `testserver` to your `ALLOWED_HOSTS` list in your settings.py (django-check-seo uses the Test Framework in order to get content, instead of doing an HTTP request).
+
 6. *(optional) Configure the settings (see [config](#config)).*
+
 7. ![that's all folks!](https://i.imgur.com/o2Tcd2E.png)
 
 ----
 
 # Misc
 
 This application needs `beautifulsoup4` (>=4.7.0) and `djangocms_page_meta` *(==0.8.5 if using django < 1.11)*. It may be used with or without `django-cms` (a django-check-seo button will appear in the topbar if you're using django-cms).
@@ -112,15 +118,15 @@
 
 ```
 DJANGO_CHECK_SEO_EXCLUDE_CONTENT = "tag, .class, #id, tag > .child_class"
 ```
 
 *You can find a reference table of css selectors explained [here](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors#Reference_table_of_selectors) (on mdn docs).*
 
-### *Example: See [this issue's comment](https://github.com/kapt-labs/django-check-seo/issues/35#issuecomment-593429870) for an example.*
+## *Example: See [this issue's comment](https://github.com/kapt-labs/django-check-seo/issues/35#issuecomment-593429870) for an example.*
 
 ----
 
 # Want a screenshot?
 
 ![screenshot](https://i.imgur.com/hJGDvtw.png)
```

### Comparing `django-check-seo-0.6.0/django_check_seo/checks/site.py` & `django-check-seo-0.6.1/django_check_seo/checks/site.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/check_description.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/check_description.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/check_h1.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/check_h1.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/check_h2.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/check_h2.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/check_images.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/check_images.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/check_keyword_url.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/check_keyword_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/check_keywords.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/check_keywords.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/check_links.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/check_links.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/check_title.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/check_title.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/check_url.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/check_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/content_words_number.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/content_words_number.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/keyword_present_first_paragraph.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/keyword_present_first_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/checks_list/launch_checks.py` & `django-check-seo-0.6.1/django_check_seo/checks_list/launch_checks.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/cms_toolbars.py` & `django-check-seo-0.6.1/django_check_seo/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/conf/settings.py` & `django-check-seo-0.6.1/django_check_seo/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/locale/fr/LC_MESSAGES/django.mo` & `django-check-seo-0.6.1/django_check_seo/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/locale/fr/LC_MESSAGES/django.po` & `django-check-seo-0.6.1/django_check_seo/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/static/django-check-seo/design.css` & `django-check-seo-0.6.1/django_check_seo/static/django-check-seo/design.css`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/LICENCE` & `django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/LICENCE`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf` & `django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf` & `django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf` & `django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf` & `django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf` & `django-check-seo-0.6.1/django_check_seo/static/django-check-seo/fonts/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/static/django-check-seo/logo-small.png` & `django-check-seo-0.6.1/django_check_seo/static/django-check-seo/logo-small.png`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/static/django-check-seo/logo.png` & `django-check-seo-0.6.1/django_check_seo/static/django-check-seo/logo.png`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/templates/default.html` & `django-check-seo-0.6.1/django_check_seo/templates/default.html`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/templates/element.html` & `django-check-seo-0.6.1/django_check_seo/templates/element.html`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/urls.py` & `django-check-seo-0.6.1/django_check_seo/urls.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/django_check_seo/views.py` & `django-check-seo-0.6.1/django_check_seo/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def get_context_data(self, *args, **kwargs):
         context = super(generic.base.TemplateView, self).get_context_data(
             *args, **kwargs
         )
 
         client = Client()
         page = self.request.GET.get("page")
-        response = client.get(page)
+        response = client.get(page, follow=True)
 
         soup = BeautifulSoup(response.content, features="lxml")
 
         # populate class with data
         page_stats = site.Site(soup, page)
 
         # magic happens here!
```

### Comparing `django-check-seo-0.6.0/django_check_seo.egg-info/PKG-INFO` & `django-check-seo-0.6.1/django_check_seo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-check-seo
-Version: 0.6.0
+Version: 0.6.1
 Summary: Django Check SEO will check the SEO aspects of your site for you, and will provide advice in case of problems.
 Home-page: https://github.com/kapt-labs/django-check-seo
 Author: Dev Kapt
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.8
@@ -22,47 +22,53 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 ![Django Check SEO](https://user-images.githubusercontent.com/45763865/114545606-72178380-9c5c-11eb-99dd-1088bb2a0bd9.png)
 
-*Replacing some features of Yoast or SEMrush for django CMS users.*
+*Replacing some features of Yoast or SEMrush for Django & Django-CMS users.*
 
 In other words, django-check-seo will tell you if you have problems concerning a broad range of SEO aspects of your pages.
 
 ----
 
 [![PyPI](https://img.shields.io/pypi/v/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/django-check-seo?color=%232a2)](https://pypi.org/project/django-check-seo/) [![GitHub last commit](https://img.shields.io/github/last-commit/kapt-labs/django-check-seo)](https://github.com/kapt-labs/django-check-seo)
 
 ----
 
 # Install
 
-*(for django >= 1.8.15 & python >= 2.7)*
+*(compatible with django >= 1.8.15 & python >= 2.7)*
 
 1. Install the module from [PyPI](https://pypi.org/project/django-check-seo/):
     ```
     python3 -m pip install django-check-seo
     ```
+
 2. Add it in your `INSTALLED_APPS`:
     ```
         "django_check_seo",
     ```
+
 3. Add this in your `urls.py` *(if you're using django-cms, put it before the `cms.urls` line or it will not work)*:
     ```
         path("django-check-seo/", include("django_check_seo.urls")),
     ```
     * *Or add this if you're still using `url` (you shouldn't):*
         ```
             url(r"^django-check-seo/", include("django_check_seo.urls")),
         ```
+
 4. Update your Django [Site](https://i.imgur.com/pNRsKs7.png) object parameters with a working url (here's an [example](https://i.imgur.com/IedF3xE.png) for dev environment).
+
 5. Add `testserver` to your `ALLOWED_HOSTS` list in your settings.py (django-check-seo uses the Test Framework in order to get content, instead of doing an HTTP request).
+
 6. *(optional) Configure the settings (see [config](#config)).*
+
 7. ![that's all folks!](https://i.imgur.com/o2Tcd2E.png)
 
 ----
 
 # Misc
 
 This application needs `beautifulsoup4` (>=4.7.0) and `djangocms_page_meta` *(==0.8.5 if using django < 1.11)*. It may be used with or without `django-cms` (a django-check-seo button will appear in the topbar if you're using django-cms).
@@ -138,15 +144,15 @@
 
 ```
 DJANGO_CHECK_SEO_EXCLUDE_CONTENT = "tag, .class, #id, tag > .child_class"
 ```
 
 *You can find a reference table of css selectors explained [here](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Selectors#Reference_table_of_selectors) (on mdn docs).*
 
-### *Example: See [this issue's comment](https://github.com/kapt-labs/django-check-seo/issues/35#issuecomment-593429870) for an example.*
+## *Example: See [this issue's comment](https://github.com/kapt-labs/django-check-seo/issues/35#issuecomment-593429870) for an example.*
 
 ----
 
 # Want a screenshot?
 
 ![screenshot](https://i.imgur.com/hJGDvtw.png)
```

### Comparing `django-check-seo-0.6.0/django_check_seo.egg-info/SOURCES.txt` & `django-check-seo-0.6.1/django_check_seo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/launch_tests.sh` & `django-check-seo-0.6.1/launch_tests.sh`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/setup.cfg` & `django-check-seo-0.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-check-seo
-version = 0.6.0
+version = 0.6.1
 description = Django Check SEO will check the SEO aspects of your site for you, and will provide advice in case of problems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kapt-labs/django-check-seo
 author = Dev Kapt
 author_email = dev@kapt.mobi
 classifiers =
```

### Comparing `django-check-seo-0.6.0/tests/test_content_words_number.py` & `django-check-seo-0.6.1/tests/test_content_words_number.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests/test_description.py` & `django-check-seo-0.6.1/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests/test_h1.py` & `django-check-seo-0.6.1/tests/test_h1.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests/test_h2.py` & `django-check-seo-0.6.1/tests/test_h2.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests/test_images.py` & `django-check-seo-0.6.1/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests/test_keyword_present_first_paragraph.py` & `django-check-seo-0.6.1/tests/test_keyword_present_first_paragraph.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests/test_keyword_url.py` & `django-check-seo-0.6.1/tests/test_keyword_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests/test_keywords.py` & `django-check-seo-0.6.1/tests/test_keywords.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests/test_links.py` & `django-check-seo-0.6.1/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests/test_title.py` & `django-check-seo-0.6.1/tests/test_title.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests/test_url.py` & `django-check-seo-0.6.1/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `django-check-seo-0.6.0/tests_settings.py` & `django-check-seo-0.6.1/tests_settings.py`

 * *Files identical despite different names*

