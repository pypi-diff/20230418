# Comparing `tmp/djaodjin-survey-0.9.3.tar.gz` & `tmp/djaodjin-survey-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-survey-0.9.3.tar", last modified: Mon Apr 10 22:55:14 2023, max compression
+gzip compressed data, was "djaodjin-survey-0.9.4.tar", last modified: Tue Apr 18 19:36:28 2023, max compression
```

## Comparing `djaodjin-survey-0.9.3.tar` & `djaodjin-survey-0.9.4.tar`

### file list

```diff
@@ -1,100 +1,70 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.038765 djaodjin-survey-0.9.3/
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     1615 2023-04-10 22:55:14.038828 djaodjin-survey-0.9.3/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1300 2023-04-10 22:53:07.000000 djaodjin-survey-0.9.3/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.020823 djaodjin-survey-0.9.3/djaodjin_survey.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     1615 2023-04-10 22:55:14.000000 djaodjin-survey-0.9.3/djaodjin_survey.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2363 2023-04-10 22:55:14.000000 djaodjin-survey-0.9.3/djaodjin_survey.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-04-10 22:55:14.000000 djaodjin-survey-0.9.3/djaodjin_survey.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-04-10 22:55:14.000000 djaodjin-survey-0.9.3/djaodjin_survey.egg-info/top_level.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       73 2022-10-01 18:58:35.000000 djaodjin-survey-0.9.3/requirements.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-04-10 22:55:14.039015 djaodjin-survey-0.9.3/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     2242 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/setup.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.024642 djaodjin-survey-0.9.3/survey/
--rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-04-10 22:49:34.000000 djaodjin-survey-0.9.3/survey/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/admin.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.028705 djaodjin-survey-0.9.3/survey/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.3/survey/api/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)    44934 2023-04-10 22:13:16.000000 djaodjin-survey-0.9.3/survey/api/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.3/survey/api/metrics.py
--rw-r--r--   0 smirolo    (501) staff       (20)    23591 2023-03-23 22:52:31.000000 djaodjin-survey-0.9.3/survey/api/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)    56385 2023-04-07 16:36:46.000000 djaodjin-survey-0.9.3/survey/api/sample.py
--rw-r--r--   0 smirolo    (501) staff       (20)    23664 2023-04-07 16:55:31.000000 djaodjin-survey-0.9.3/survey/api/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.3/survey/api/serializers_overrides.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5408 2022-11-14 00:13:32.000000 djaodjin-survey-0.9.3/survey/api/units.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.3/survey/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)    17450 2023-04-07 16:40:09.000000 djaodjin-survey-0.9.3/survey/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/forms.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6173 2023-04-05 16:25:51.000000 djaodjin-survey-0.9.3/survey/helpers.py
--rw-r--r--   0 smirolo    (501) staff       (20)    14652 2023-04-10 22:07:21.000000 djaodjin-survey-0.9.3/survey/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)    39683 2023-04-05 17:20:30.000000 djaodjin-survey-0.9.3/survey/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-04-05 18:59:23.000000 djaodjin-survey-0.9.3/survey/pagination.py
--rw-r--r--   0 smirolo    (501) staff       (20)    13064 2023-04-05 17:26:46.000000 djaodjin-survey-0.9.3/survey/queries.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.3/survey/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.3/survey/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.018942 djaodjin-survey-0.9.3/survey/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.028946 djaodjin-survey-0.9.3/survey/static/css/
--rw-r--r--   0 smirolo    (501) staff       (20)      296 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/css/matrix-chart.css
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.030625 djaodjin-survey-0.9.3/survey/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)    12547 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-categorize.js
--rw-r--r--   0 smirolo    (501) staff       (20)    15443 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-matrix.js
--rw-r--r--   0 smirolo    (501) staff       (20)    51291 2023-04-10 22:08:00.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     5462 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-set.js
--rw-r--r--   0 smirolo    (501) staff       (20)    16018 2023-03-20 16:58:45.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-survey-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)      544 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/js/djaodjin-survey.js
--rw-r--r--   0 smirolo    (501) staff       (20)    12995 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/static/js/matrix-chart.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.019037 djaodjin-survey-0.9.3/survey/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.032446 djaodjin-survey-0.9.3/survey/templates/survey/
--rw-r--r--   0 smirolo    (501) staff       (20)      667 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/answer_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/campaign_form.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.032585 djaodjin-survey-0.9.3/survey/templates/survey/campaigns/
--rw-r--r--   0 smirolo    (501) staff       (20)     1184 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/campaigns/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2529 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/categorize.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.033106 djaodjin-survey-0.9.3/survey/templates/survey/matrix/
--rw-r--r--   0 smirolo    (501) staff       (20)       62 2023-01-19 22:34:30.000000 djaodjin-survey-0.9.3/survey/templates/survey/matrix/compare.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2087 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/matrix/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)     4088 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/matrix/matrix.html
--rw-r--r--   0 smirolo    (501) staff       (20)     9287 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/portfolios.html
--rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/question_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)     1572 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/question_list.html
--rw-r--r--   0 smirolo    (501) staff       (20)      471 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/respondent_list.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2077 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/result.html
--rw-r--r--   0 smirolo    (501) staff       (20)      983 2023-03-10 17:29:52.000000 djaodjin-survey-0.9.3/survey/templates/survey/result_quizz.html
--rw-r--r--   0 smirolo    (501) staff       (20)      562 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/sample_create.html
--rw-r--r--   0 smirolo    (501) staff       (20)      356 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/sample_update.html
--rw-r--r--   0 smirolo    (501) staff       (20)      245 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templates/survey/send.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.033338 djaodjin-survey-0.9.3/survey/templatetags/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/templatetags/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.3/survey/templatetags/survey_tags.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.033559 djaodjin-survey-0.9.3/survey/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.3/survey/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.035160 djaodjin-survey-0.9.3/survey/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.3/survey/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.3/survey/urls/api/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.3/survey/urls/api/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2125 2023-04-07 17:48:09.000000 djaodjin-survey-0.9.3/survey/urls/api/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.3/survey/urls/api/metrics.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.3/survey/urls/api/noauth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.3/survey/urls/api/portfolios.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.035795 djaodjin-survey-0.9.3/survey/urls/api/sample/
--rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.3/survey/urls/api/sample/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.3/survey/urls/api/sample/reset.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2830 2023-04-07 17:59:33.000000 djaodjin-survey-0.9.3/survey/urls/api/sample/update.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.036976 djaodjin-survey-0.9.3/survey/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.3/survey/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.3/survey/urls/views/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.3/survey/urls/views/matrices.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.3/survey/urls/views/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.3/survey/urls/views/samples.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9305 2023-04-05 18:38:45.000000 djaodjin-survey-0.9.3/survey/utils.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-10 22:55:14.038499 djaodjin-survey-0.9.3/survey/views/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.3/survey/views/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/views/createquestion.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.3/survey/views/edit.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6155 2023-04-07 17:48:37.000000 djaodjin-survey-0.9.3/survey/views/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.3/survey/views/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.3/survey/views/sample.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:36:28.511524 djaodjin-survey-0.9.4/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.4/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.4/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     1888 2023-04-18 19:36:28.511586 djaodjin-survey-0.9.4/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1129 2023-04-18 19:35:08.000000 djaodjin-survey-0.9.4/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:36:28.498634 djaodjin-survey-0.9.4/djaodjin_survey.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1888 2023-04-18 19:36:28.000000 djaodjin-survey-0.9.4/djaodjin_survey.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1436 2023-04-18 19:36:28.000000 djaodjin-survey-0.9.4/djaodjin_survey.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-04-18 19:36:28.000000 djaodjin-survey-0.9.4/djaodjin_survey.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       73 2023-04-18 19:36:28.000000 djaodjin-survey-0.9.4/djaodjin_survey.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-04-18 19:36:28.000000 djaodjin-survey-0.9.4/djaodjin_survey.egg-info/top_level.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)     1180 2023-04-18 17:14:12.000000 djaodjin-survey-0.9.4/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-04-18 19:36:28.511785 djaodjin-survey-0.9.4/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 16:17:24.000000 djaodjin-survey-0.9.4/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:36:28.502551 djaodjin-survey-0.9.4/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-04-18 19:32:23.000000 djaodjin-survey-0.9.4/survey/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.4/survey/admin.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:36:28.505977 djaodjin-survey-0.9.4/survey/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.4/survey/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.4/survey/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    44811 2023-04-18 18:56:03.000000 djaodjin-survey-0.9.4/survey/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.4/survey/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    23591 2023-03-23 22:52:31.000000 djaodjin-survey-0.9.4/survey/api/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    56385 2023-04-07 16:36:46.000000 djaodjin-survey-0.9.4/survey/api/sample.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    23830 2023-04-14 17:05:47.000000 djaodjin-survey-0.9.4/survey/api/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.4/survey/api/serializers_overrides.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5569 2023-04-13 17:06:50.000000 djaodjin-survey-0.9.4/survey/api/units.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.4/survey/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.4/survey/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    17450 2023-04-07 16:40:09.000000 djaodjin-survey-0.9.4/survey/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.4/survey/forms.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6173 2023-04-05 16:25:51.000000 djaodjin-survey-0.9.4/survey/helpers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    14690 2023-04-18 18:56:44.000000 djaodjin-survey-0.9.4/survey/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    39683 2023-04-05 17:20:30.000000 djaodjin-survey-0.9.4/survey/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-04-05 18:59:23.000000 djaodjin-survey-0.9.4/survey/pagination.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    13064 2023-04-05 17:26:46.000000 djaodjin-survey-0.9.4/survey/queries.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.4/survey/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.4/survey/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:36:28.506309 djaodjin-survey-0.9.4/survey/templatetags/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.4/survey/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.4/survey/templatetags/survey_tags.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:36:28.506534 djaodjin-survey-0.9.4/survey/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.4/survey/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:36:28.508051 djaodjin-survey-0.9.4/survey/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.4/survey/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.4/survey/urls/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.4/survey/urls/api/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2125 2023-04-07 17:48:09.000000 djaodjin-survey-0.9.4/survey/urls/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.4/survey/urls/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.4/survey/urls/api/noauth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.4/survey/urls/api/portfolios.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:36:28.508633 djaodjin-survey-0.9.4/survey/urls/api/sample/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.4/survey/urls/api/sample/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.4/survey/urls/api/sample/reset.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2830 2023-04-07 17:59:33.000000 djaodjin-survey-0.9.4/survey/urls/api/sample/update.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:36:28.509788 djaodjin-survey-0.9.4/survey/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.4/survey/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.4/survey/urls/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.4/survey/urls/views/matrices.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.4/survey/urls/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.4/survey/urls/views/samples.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9367 2023-04-17 20:51:27.000000 djaodjin-survey-0.9.4/survey/utils.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:36:28.511290 djaodjin-survey-0.9.4/survey/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.4/survey/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.4/survey/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.4/survey/views/createquestion.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.4/survey/views/edit.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6155 2023-04-07 17:48:37.000000 djaodjin-survey-0.9.4/survey/views/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.4/survey/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.4/survey/views/sample.py
```

### Comparing `djaodjin-survey-0.9.3/LICENSE.txt` & `djaodjin-survey-0.9.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/PKG-INFO` & `djaodjin-survey-0.9.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,43 @@
-Metadata-Version: 2.1
-Name: djaodjin-survey
-Version: 0.9.3
-Summary: Survey Django app
-Home-page: https://github.com/djaodjin/djaodjin-survey/
-Download-URL: https://github.com/djaodjin/djaodjin-survey/tarball/0.9.3
-Author: The DjaoDjin Team
-Author-email: support@djaodjin.com
-License: BSD
-License-File: LICENSE.txt
-
 DjaoDjin survey
 ================
 
 The Django app implements a simple survey app.
 
 Full documentation for the project is available at
 [Read-the-Docs](http://djaodjin-survey.readthedocs.org/)
 
 
 Five minutes evaluation
 =======================
 
 The source code is bundled with a sample django project.
 
-    $ virtualenv *virtual_env_dir*
-    $ cd *virtual_env_dir*
-    $ source bin/activate
+    $ python3 -m venv .venv
+    $ source .venv/bin/activate
     $ pip install -r testsite/requirements.txt
     $ python manage.py migrate --run-syncdb --noinput
     $ python manage.py loaddata testsite/fixtures/default-db.json
 
     $ python manage.py runserver
 
     # Visit url at http://localhost:8000/
     # You can use username: donny, password: yoyo to test the manager options.
 
 Releases
 ========
 
 Tested with
 
-- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/)), **Django Rest Framework:** 3.12
-- **Python:** 3.10, **Django:** 4.1 (latest), **Django Rest Framework:** 3.12
-- **Python:** 2.7, **Django:** 1.11 (legacy), **Django Rest Framework:** 3.9.4
-
-0.9.3
-
-  * adds benchmarks APIs
-  * lists all samples for an account, filtered by active or is_frozen
-  * prevents import loops between queries.py, models.py and utils.py
+- **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
+- **Python:** 3.10, **Django:** 4.2 (latest)
+- **Python:** 2.7, **Django:** 1.11 (legacy) (see testsite/requirements-legacy.txt)
+
+0.9.4
+
+  * publishes distribution using pyproject.toml
+  * edits a question default unit
 
 [previous release notes](changelog)
 
 
 Models have been completely re-designed between version 0.1.7 and 0.2.0
```

### Comparing `djaodjin-survey-0.9.3/setup.py` & `djaodjin-survey-0.9.4/survey/urls/api/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,36 +18,18 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from distutils.core import setup
-import survey
+from ...compat import include, path
 
-setup(
-    name='djaodjin-survey',
-    version=survey.__version__,
-    author='The DjaoDjin Team',
-    author_email='support@djaodjin.com',
-    packages=['survey',
-              'survey.api',
-              'survey.templatetags',
-              'survey.urls',
-              'survey.urls.api',
-              'survey.urls.api.sample',
-              'survey.urls.views',
-              'survey.views'],
-    package_data={'survey': [
-        'static/css/*',
-        'static/js/*',
-        'templates/survey/*',
-        'templates/survey/campaigns/*',
-        'templates/survey/matrix/*']},
-    url='https://github.com/djaodjin/djaodjin-survey/',
-    download_url='https://github.com/djaodjin/djaodjin-survey/tarball/%s' \
-        % survey.__version__,
-    license='BSD',
-    description='Survey Django app',
-    long_description=open('README.md').read(),
-)
+
+urlpatterns = [
+    path('', include('survey.urls.api.noauth')),
+    path('', include('survey.urls.api.campaigns')),
+    path('', include('survey.urls.api.filters')),
+    path('', include('survey.urls.api.sample')),
+    path('', include('survey.urls.api.portfolios')),
+    path('<slug:campaign>/', include('survey.urls.api.matrix')),
+]
```

### Comparing `djaodjin-survey-0.9.3/survey/__init__.py` & `djaodjin-survey-0.9.4/survey/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the survey django app.
 """
 
-__version__ = '0.9.3'
+__version__ = '0.9.4'
```

### Comparing `djaodjin-survey-0.9.3/survey/admin.py` & `djaodjin-survey-0.9.4/survey/admin.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/campaigns.py` & `djaodjin-survey-0.9.4/survey/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/matrix.py` & `djaodjin-survey-0.9.4/survey/api/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,27 +37,26 @@
 from .. import settings
 from ..compat import reverse, six
 from ..mixins import (AccountMixin, CampaignMixin, DateRangeContextMixin,
     MatrixMixin, QuestionMixin, SampleMixin)
 from ..models import (Answer, Matrix, EditableFilter,
     EditableFilterEnumeratedAccounts, Sample, Unit, UnitEquivalences)
 from ..pagination import MetricsPagination
-from ..utils import (get_accessible_accounts, get_benchmarks_enumerated,
-    get_account_model, get_question_model,
+from ..utils import (datetime_or_now, get_accessible_accounts,
+    get_benchmarks_enumerated, get_account_model, get_question_model,
     get_account_serializer, get_question_serializer)
 from .serializers import (AccountsFilterAddSerializer,
     CompareQuestionSerializer, EditableFilterSerializer, MatrixSerializer,
     SampleBenchmarksSerializer)
 
-
 LOGGER = logging.getLogger(__name__)
 
 
-class BenchmarkAPIView(QuestionMixin, CampaignMixin, AccountMixin,
-                       DateRangeContextMixin, generics.ListAPIView):
+class BenchmarkAPIView(QuestionMixin, DateRangeContextMixin, CampaignMixin,
+                       AccountMixin, generics.ListAPIView):
     """
     Aggregated benchmark for requested accounts
 
     **Examples**:
 
     .. code-block:: http
 
@@ -87,21 +86,14 @@
         if not hasattr(self, '_unit'):
             self._unit = self.default_unit
             param_unit = self.get_query_param('unit')
             if param_unit is not None and param_unit in self.valid_units:
                 self._unit = param_unit
         return self._unit
 
-    def get_query_param(self, key):
-        try:
-            return self.request.query_params.get(key, None)
-        except AttributeError:
-            pass
-        return self.request.GET.get(key, None)
-
     def get_accessible_accounts(self, grantees):
         return get_accessible_accounts(grantees, campaign=self.campaign)
 
     def get_questions(self, prefix):
         """
         Overrides CampaignContentMixin.get_questions to return a list
         of questions based on the answers available in the benchmarkd samples.
@@ -219,15 +211,16 @@
             self._campaign = self.sample.campaign
         return self._campaign
 
     @property
     def ends_at(self):
         #pylint:disable=attribute-defined-outside-init
         if not hasattr(self, '_ends_at'):
-            self._ends_at = self.sample.created_at
+            self._ends_at = (self.sample.created_at if self.sample.is_frozen
+                else datetime_or_now())
         return self._ends_at
 
     def get_accessible_accounts(self, grantees):
         return get_account_model().objects.all()
 
 
 class SampleBenchmarksIndexAPIView(SampleBenchmarksAPIView):
@@ -249,15 +242,15 @@
         {
           "count": 4,
           "results": []
         }
     """
 
 
-class CompareAPIView(CampaignMixin, AccountMixin, DateRangeContextMixin,
+class CompareAPIView(DateRangeContextMixin, CampaignMixin, AccountMixin,
                      generics.ListAPIView):
     """
     Lists compared samples
 
     **Examples**:
 
     .. code-block:: http
```

### Comparing `djaodjin-survey-0.9.3/survey/api/metrics.py` & `djaodjin-survey-0.9.4/survey/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/portfolios.py` & `djaodjin-survey-0.9.4/survey/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/sample.py` & `djaodjin-survey-0.9.4/survey/api/sample.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/serializers.py` & `djaodjin-survey-0.9.4/survey/api/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,17 +205,21 @@
     class Meta:
         model = get_question_model()
         fields = ('title', 'text', 'default_unit', 'extra')
 
 
 class QuestionDetailSerializer(QuestionCreateSerializer):
 
+    title = serializers.CharField(required=False,
+        help_text=_("Title of the question as displayed in user interfaces"))
+
     class Meta:
         model = QuestionCreateSerializer.Meta.model
         fields = QuestionCreateSerializer.Meta.fields + ('path',)
+        read_only_fields = ('path',)
 
 
 class QuestionSerializer(serializers.ModelSerializer):
     """
     Serializer of ``Question`` when used in a list of answers
     """
     title = serializers.CharField(allow_blank=True,
```

### Comparing `djaodjin-survey-0.9.3/survey/api/serializers_overrides.py` & `djaodjin-survey-0.9.4/survey/api/serializers_overrides.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/units.py` & `djaodjin-survey-0.9.4/survey/api/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import logging
 
 from rest_framework import generics
 from rest_framework.filters import BaseFilterBackend
 
+from ..filters import SearchFilter
 from ..models import Unit
 from .serializers import UnitSerializer
 
 LOGGER = logging.getLogger(__name__)
 
 
 class EquivalenceFilter(BaseFilterBackend):
@@ -177,9 +178,15 @@
                     "text": "mostly-no",
                     "descr": "Mostly no"
                 }
             ]
           }]
         }
     """
+    search_fields = (
+        'slug',
+        'title',
+    )
+
     serializer_class = UnitSerializer
-    filter_backends = (EquivalenceFilter,)
+    filter_backends = (EquivalenceFilter, SearchFilter)
+    queryset = Unit.objects.all().order_by('slug')
```

### Comparing `djaodjin-survey-0.9.3/survey/compat.py` & `djaodjin-survey-0.9.4/survey/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/docs.py` & `djaodjin-survey-0.9.4/survey/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/filters.py` & `djaodjin-survey-0.9.4/survey/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/forms.py` & `djaodjin-survey-0.9.4/survey/forms.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/helpers.py` & `djaodjin-survey-0.9.4/survey/helpers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/mixins.py` & `djaodjin-survey-0.9.4/survey/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,20 +155,20 @@
 
     @property
     def timezone(self):
         if not hasattr(self, '_timezone'):
             self._timezone = self.get_query_param('timezone')
         return self._timezone
 
-    def get_query_param(self, key):
+    def get_query_param(self, key, default_value=None):
         try:
-            return self.request.query_params.get(key, None)
+            return self.request.query_params.get(key, default_value)
         except AttributeError:
             pass
-        return self.request.GET.get(key, None)
+        return self.request.GET.get(key, default_value)
 
     def get_context_data(self, **kwargs):
         context = super(DateRangeContextMixin, self).get_context_data(**kwargs)
         if self.start_at:
             context.update({'start_at': self.start_at})
         if self.ends_at:
             context.update({'ends_at': self.ends_at})
```

### Comparing `djaodjin-survey-0.9.3/survey/models.py` & `djaodjin-survey-0.9.4/survey/models.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/pagination.py` & `djaodjin-survey-0.9.4/survey/pagination.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/queries.py` & `djaodjin-survey-0.9.4/survey/queries.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/settings.py` & `djaodjin-survey-0.9.4/survey/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/signals.py` & `djaodjin-survey-0.9.4/survey/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templatetags/survey_tags.py` & `djaodjin-survey-0.9.4/survey/templatetags/survey_tags.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/__init__.py` & `djaodjin-survey-0.9.4/survey/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/__init__.py` & `djaodjin-survey-0.9.4/survey/urls/views/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, DjaoDjin inc.
+# Copyright (c) 2023, DjaoDjin inc.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice,
 #    this list of conditions and the following disclaimer.
@@ -18,18 +18,20 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+"""
+URLs for the djaodjin-survey HTML pages Django app
+"""
+
 from ...compat import include, path
 
 
 urlpatterns = [
-    path('', include('survey.urls.api.noauth')),
-    path('', include('survey.urls.api.campaigns')),
-    path('', include('survey.urls.api.filters')),
-    path('', include('survey.urls.api.sample')),
-    path('', include('survey.urls.api.portfolios')),
-    path('<slug:campaign>/', include('survey.urls.api.matrix')),
+    path('matrix/<slug:campaign>/', include('survey.urls.views.matrices')),
+    path('campaigns/', include('survey.urls.views.campaigns')),
+    path('assess/', include('survey.urls.views.samples')),
+    path('', include('survey.urls.views.portfolios')),
 ]
```

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/campaigns.py` & `djaodjin-survey-0.9.4/survey/urls/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/filters.py` & `djaodjin-survey-0.9.4/survey/urls/api/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/matrix.py` & `djaodjin-survey-0.9.4/survey/urls/api/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/metrics.py` & `djaodjin-survey-0.9.4/survey/urls/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/noauth.py` & `djaodjin-survey-0.9.4/survey/urls/api/noauth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/portfolios.py` & `djaodjin-survey-0.9.4/survey/urls/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/sample/__init__.py` & `djaodjin-survey-0.9.4/survey/urls/api/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/sample/reset.py` & `djaodjin-survey-0.9.4/survey/urls/api/sample/reset.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/sample/update.py` & `djaodjin-survey-0.9.4/survey/urls/api/sample/update.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/views/__init__.py` & `djaodjin-survey-0.9.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,21 +17,10 @@
 # CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
 # OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+from setuptools import setup
 
-"""
-URLs for the djaodjin-survey HTML pages Django app
-"""
-
-from ...compat import include, path
-
-
-urlpatterns = [
-    path('matrix/<slug:campaign>/', include('survey.urls.views.matrices')),
-    path('campaigns/', include('survey.urls.views.campaigns')),
-    path('assess/', include('survey.urls.views.samples')),
-    path('', include('survey.urls.views.portfolios')),
-]
+setup()
```

### Comparing `djaodjin-survey-0.9.3/survey/urls/views/campaigns.py` & `djaodjin-survey-0.9.4/survey/urls/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/views/matrices.py` & `djaodjin-survey-0.9.4/survey/urls/views/matrices.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/views/portfolios.py` & `djaodjin-survey-0.9.4/survey/urls/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/views/samples.py` & `djaodjin-survey-0.9.4/survey/urls/views/samples.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/utils.py` & `djaodjin-survey-0.9.4/survey/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,30 +51,31 @@
 def as_timestamp(dtime_at=None):
     if not dtime_at:
         dtime_at = datetime_or_now()
     return int((
         dtime_at - datetime.datetime(1970, 1, 1, tzinfo=utc)).total_seconds())
 
 
-def get_accessible_accounts(grantees,
-                            campaign=None, start_at=None, ends_at=None):
+def get_accessible_accounts(grantees, campaign=None, aggregate_set=False,
+                            start_at=None, ends_at=None):
     """
     All accounts which have elected to share samples with at least one
     account in grantees.
     """
     try:
         iter(grantees)
     except TypeError:
         grantees = [grantees]
 
     queryset = None
     if (hasattr(settings, 'ACCESSIBLE_ACCOUNTS_CALLABLE') and
         settings.ACCESSIBLE_ACCOUNTS_CALLABLE):
         queryset = import_string(settings.ACCESSIBLE_ACCOUNTS_CALLABLE)(
-            grantees, campaign=campaign, start_at=start_at, ends_at=ends_at)
+            grantees, campaign=campaign, aggregate_set=aggregate_set,
+            start_at=start_at, ends_at=ends_at)
 
     if queryset is None:
         filter_params = {}
         if start_at:
             filter_params.update({
                 'portfolio_double_optin_accounts__created_at__gte': start_at})
         if campaign:
```

### Comparing `djaodjin-survey-0.9.3/survey/views/campaigns.py` & `djaodjin-survey-0.9.4/survey/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/views/createquestion.py` & `djaodjin-survey-0.9.4/survey/views/createquestion.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/views/edit.py` & `djaodjin-survey-0.9.4/survey/views/edit.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/views/matrix.py` & `djaodjin-survey-0.9.4/survey/views/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/views/portfolios.py` & `djaodjin-survey-0.9.4/survey/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/views/sample.py` & `djaodjin-survey-0.9.4/survey/views/sample.py`

 * *Files identical despite different names*

