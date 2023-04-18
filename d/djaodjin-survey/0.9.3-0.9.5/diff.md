# Comparing `tmp/djaodjin-survey-0.9.3.tar.gz` & `tmp/djaodjin-survey-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-survey-0.9.3.tar", last modified: Mon Apr 10 22:55:14 2023, max compression
+gzip compressed data, was "djaodjin-survey-0.9.5.tar", last modified: Tue Apr 18 19:58:10 2023, max compression
```

## Comparing `djaodjin-survey-0.9.3.tar` & `djaodjin-survey-0.9.5.tar`

### file list

```diff
@@ -1,100 +1,101 @@
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
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.470100 djaodjin-survey-0.9.5/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     1888 2023-04-18 19:58:10.470164 djaodjin-survey-0.9.5/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1129 2023-04-18 19:35:08.000000 djaodjin-survey-0.9.5/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.461467 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1888 2023-04-18 19:58:10.000000 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2399 2023-04-18 19:58:10.000000 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-04-18 19:58:10.000000 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       73 2023-04-18 19:58:10.000000 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-04-18 19:58:10.000000 djaodjin-survey-0.9.5/djaodjin_survey.egg-info/top_level.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)     1358 2023-04-18 19:54:04.000000 djaodjin-survey-0.9.5/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-04-18 19:58:10.470345 djaodjin-survey-0.9.5/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 16:17:24.000000 djaodjin-survey-0.9.5/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.463222 djaodjin-survey-0.9.5/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-04-18 19:57:54.000000 djaodjin-survey-0.9.5/survey/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/admin.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.464384 djaodjin-survey-0.9.5/survey/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.5/survey/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    44811 2023-04-18 18:56:03.000000 djaodjin-survey-0.9.5/survey/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.5/survey/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    23591 2023-03-23 22:52:31.000000 djaodjin-survey-0.9.5/survey/api/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    56385 2023-04-07 16:36:46.000000 djaodjin-survey-0.9.5/survey/api/sample.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    23830 2023-04-14 17:05:47.000000 djaodjin-survey-0.9.5/survey/api/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.5/survey/api/serializers_overrides.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5569 2023-04-13 17:06:50.000000 djaodjin-survey-0.9.5/survey/api/units.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.5/survey/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    17450 2023-04-07 16:40:09.000000 djaodjin-survey-0.9.5/survey/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/forms.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6173 2023-04-05 16:25:51.000000 djaodjin-survey-0.9.5/survey/helpers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    14690 2023-04-18 18:56:44.000000 djaodjin-survey-0.9.5/survey/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    39683 2023-04-05 17:20:30.000000 djaodjin-survey-0.9.5/survey/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-04-05 18:59:23.000000 djaodjin-survey-0.9.5/survey/pagination.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    13064 2023-04-05 17:26:46.000000 djaodjin-survey-0.9.5/survey/queries.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.5/survey/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.5/survey/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.459556 djaodjin-survey-0.9.5/survey/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.464512 djaodjin-survey-0.9.5/survey/static/css/
+-rw-r--r--   0 smirolo    (501) staff       (20)      296 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/css/matrix-chart.css
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.465399 djaodjin-survey-0.9.5/survey/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)    12547 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-categorize.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    15443 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-matrix.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 15:55:35.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     5462 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-set.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    17193 2023-04-14 16:37:55.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-survey-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)      544 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/js/djaodjin-survey.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    12995 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/static/js/matrix-chart.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.459669 djaodjin-survey-0.9.5/survey/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.466755 djaodjin-survey-0.9.5/survey/templates/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)      667 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/answer_form.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/campaign_form.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.466869 djaodjin-survey-0.9.5/survey/templates/survey/campaigns/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1184 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/campaigns/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2529 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/categorize.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.467192 djaodjin-survey-0.9.5/survey/templates/survey/matrix/
+-rw-r--r--   0 smirolo    (501) staff       (20)       62 2023-01-19 22:34:30.000000 djaodjin-survey-0.9.5/survey/templates/survey/matrix/compare.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2087 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/matrix/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     4088 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/matrix/matrix.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     9287 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/portfolios.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/question_form.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     1572 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/question_list.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      471 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/respondent_list.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2077 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/result.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      983 2023-03-10 17:29:52.000000 djaodjin-survey-0.9.5/survey/templates/survey/result_quizz.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      562 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/sample_create.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      356 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/sample_update.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      245 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templates/survey/send.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.467409 djaodjin-survey-0.9.5/survey/templatetags/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.5/survey/templatetags/survey_tags.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.467519 djaodjin-survey-0.9.5/survey/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.5/survey/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.468301 djaodjin-survey-0.9.5/survey/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.5/survey/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.5/survey/urls/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.5/survey/urls/api/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2125 2023-04-07 17:48:09.000000 djaodjin-survey-0.9.5/survey/urls/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.5/survey/urls/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.5/survey/urls/api/noauth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.5/survey/urls/api/portfolios.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.468638 djaodjin-survey-0.9.5/survey/urls/api/sample/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.5/survey/urls/api/sample/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.5/survey/urls/api/sample/reset.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2830 2023-04-07 17:59:33.000000 djaodjin-survey-0.9.5/survey/urls/api/sample/update.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.469227 djaodjin-survey-0.9.5/survey/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.5/survey/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.5/survey/urls/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.5/survey/urls/views/matrices.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.5/survey/urls/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.5/survey/urls/views/samples.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9367 2023-04-17 20:51:27.000000 djaodjin-survey-0.9.5/survey/utils.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-04-18 19:58:10.469985 djaodjin-survey-0.9.5/survey/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.5/survey/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/views/createquestion.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.5/survey/views/edit.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6155 2023-04-07 17:48:37.000000 djaodjin-survey-0.9.5/survey/views/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.5/survey/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.5/survey/views/sample.py
```

### Comparing `djaodjin-survey-0.9.3/LICENSE.txt` & `djaodjin-survey-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/PKG-INFO` & `djaodjin-survey-0.9.5/README.md`

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

### Comparing `djaodjin-survey-0.9.3/djaodjin_survey.egg-info/SOURCES.txt` & `djaodjin-survey-0.9.5/djaodjin_survey.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
 setup.py
 djaodjin_survey.egg-info/PKG-INFO
 djaodjin_survey.egg-info/SOURCES.txt
 djaodjin_survey.egg-info/dependency_links.txt
+djaodjin_survey.egg-info/requires.txt
 djaodjin_survey.egg-info/top_level.txt
 survey/__init__.py
 survey/admin.py
 survey/compat.py
 survey/docs.py
 survey/filters.py
 survey/forms.py
```

### Comparing `djaodjin-survey-0.9.3/setup.py` & `djaodjin-survey-0.9.5/survey/urls/api/__init__.py`

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

### Comparing `djaodjin-survey-0.9.3/survey/__init__.py` & `djaodjin-survey-0.9.5/survey/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the survey django app.
 """
 
-__version__ = '0.9.3'
+__version__ = '0.9.5'
```

### Comparing `djaodjin-survey-0.9.3/survey/admin.py` & `djaodjin-survey-0.9.5/survey/admin.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/campaigns.py` & `djaodjin-survey-0.9.5/survey/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/matrix.py` & `djaodjin-survey-0.9.5/survey/api/matrix.py`

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

### Comparing `djaodjin-survey-0.9.3/survey/api/metrics.py` & `djaodjin-survey-0.9.5/survey/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/portfolios.py` & `djaodjin-survey-0.9.5/survey/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/sample.py` & `djaodjin-survey-0.9.5/survey/api/sample.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/serializers.py` & `djaodjin-survey-0.9.5/survey/api/serializers.py`

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

### Comparing `djaodjin-survey-0.9.3/survey/api/serializers_overrides.py` & `djaodjin-survey-0.9.5/survey/api/serializers_overrides.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/api/units.py` & `djaodjin-survey-0.9.5/survey/api/units.py`

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

### Comparing `djaodjin-survey-0.9.3/survey/compat.py` & `djaodjin-survey-0.9.5/survey/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/docs.py` & `djaodjin-survey-0.9.5/survey/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/filters.py` & `djaodjin-survey-0.9.5/survey/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/forms.py` & `djaodjin-survey-0.9.5/survey/forms.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/helpers.py` & `djaodjin-survey-0.9.5/survey/helpers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/mixins.py` & `djaodjin-survey-0.9.5/survey/mixins.py`

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

### Comparing `djaodjin-survey-0.9.3/survey/models.py` & `djaodjin-survey-0.9.5/survey/models.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/pagination.py` & `djaodjin-survey-0.9.5/survey/pagination.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/queries.py` & `djaodjin-survey-0.9.5/survey/queries.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/settings.py` & `djaodjin-survey-0.9.5/survey/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/signals.py` & `djaodjin-survey-0.9.5/survey/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/static/js/djaodjin-categorize.js` & `djaodjin-survey-0.9.5/survey/static/js/djaodjin-categorize.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/static/js/djaodjin-matrix.js` & `djaodjin-survey-0.9.5/survey/static/js/djaodjin-matrix.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/static/js/djaodjin-resources-vue.js` & `djaodjin-survey-0.9.5/survey/static/js/djaodjin-resources-vue.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -158,32 +158,37 @@
     };
 
 
     /** compute outdated based on `params`.
 
         `params = {start_at, ends_at}` must exist in either the `props` or `data`
         of the component.
+
+        A subclass of this mixin must define either the function `autoReload`
+        or `reload` in order to make updates as a user is typing in input fields
+        or when a button is pressed respectively.
      */
     var paramsMixin = {
         data: function() {
             var data = {
-                autoreload: true,
                 lastGetParams: {},
             }
             return data;
         },
         methods: {
             asDateInputField: function(dateISOString) {
                 const dateValue = moment(dateISOString);
                 return dateValue.isValid() ? dateValue.format("YYYY-MM-DD") : null;
             },
             asDateISOString: function(dateInputField) {
                 const dateValue = moment(dateInputField, "YYYY-MM-DD");
                 return dateValue.isValid() ? dateValue.toISOString() : null;
             },
+            autoReload: function() {},
+            reload: function() {},
             getParams: function(excludes) {
                 var vm = this;
                 var params = {};
                 for (var key in vm.params) {
                     if (vm.params.hasOwnProperty(key) && vm.params[key]) {
                         if (excludes && key in excludes) continue;
                         params[key] = vm.params[key];
@@ -216,15 +221,15 @@
                 },
                 set: function(newVal) {
                     if (newVal) {
                         // The setter might be call with `newVal === null`
                         // when the date is incorrect (ex: 09/31/2022).
                         this.$set(this.params, 'start_at',
                             this.asDateISOString(newVal));
-                        if (this.autoreload && this.outdated) this.get();
+                        if (this.outdated) this.debouncedAutoReload();
                     }
                 }
             },
             _ends_at: {
                 get: function() {
                     // form field input="date" will expect ends_at as a String
                     // but will literally cut the hour part regardless of timezone.
@@ -240,15 +245,15 @@
                 },
                 set: function(newVal) {
                     if (newVal) {
                         // The setter might be call with `newVal === null`
                         // when the date is incorrect (ex: 09/31/2022).
                         this.$set(this.params, 'ends_at',
                             this.asDateISOString(newVal));
-                        if (this.autoreload && this.outdated) this.get();
+                        if (this.outdated) this.debouncedAutoReload();
                     }
                 }
             },
             outdated: function() {
                 var vm = this;
                 const params = vm.getParams();
                 for (var key in vm.lastGetParams) {
@@ -263,14 +268,23 @@
                         if (params[key] !== vm.lastGetParams[key]) {
                             return true;
                         }
                     }
                 }
                 return false;
             }
+        },
+        created: function() {
+            // _.debounce is a function provided by lodash to limit how
+            // often a particularly expensive operation can be run.
+            if (typeof _ != 'undefined' && typeof _.debounce != 'undefined') {
+                this.debouncedAutoReload = _.debounce(this.autoReload, 500);
+            } else {
+                this.debouncedAutoReload = this.autoReload;
+            }
         }
     };
 
 
     /** A wrapper around jQuery ajax functions that adds authentication
         parameters as necessary.
 
@@ -894,83 +908,56 @@
                 }
                 return !isEmpty;
             },
         },
     }
 
 
-    var filterableMixin = {
-        data: function() {
-            return {
-                params: {
-                    q: '',
-                },
-                mixinFilterCb: 'get',
-            }
-        },
-        methods: {
-            filterList: function() {
-                if (this.params.q) {
-                    if ("page" in this.params) {
-                        this.params.page = 1;
-                    }
-                }
-                if (this[this.mixinFilterCb]) {
-                    this[this.mixinFilterCb]();
-                }
-            },
-        },
-    }
-
-
     var paginationMixin = {
         data: function() {
             return {
                 params: {
                     page: 1,
                 },
+                mergeResults: false,
                 itemsPerPage: this.$itemsPerPage,
                 ellipsisThreshold: 4,
+                preReload: ['resetPage'],
                 getCompleteCb: 'getCompleted',
                 getBeforeCb: 'resetPage',
-                qsCache: null,
-                isInfiniteScroll: false,
             }
         },
         methods: {
             resetPage: function() {
                 var vm = this;
-                if (!vm.ISState) return;
-                if (vm.qsCache && vm.qsCache !== vm.qs) {
-                    vm.params.page = 1;
-                    vm.ISState.reset();
-                }
-                vm.qsCache = vm.qs;
+                vm.params.page = 1;
             },
             getCompleted: function() {
                 var vm = this;
-                if (!vm.ISState) return;
                 vm.mergeResults = false;
-                if (vm.pageCount > 0) {
-                    vm.ISState.loaded();
-                }
-                if (vm.params.page >= vm.pageCount) {
-                    vm.ISState.complete();
+            },
+            handleScroll: function(evt) {
+                var vm = this;
+                let element = this.$el;
+                if (element.getBoundingClientRect().bottom < window.innerHeight) {
+                    let menubar = vm.$el.querySelector('[role="pagination"]');
+                    var style = window.getComputedStyle(menubar);
+                    if (style.display == 'none') {
+                        // We are not displaying the pagination menubar,
+                        // so let's scroll!
+                        vm.paginationHandler();
+                    }
                 }
             },
             paginationHandler: function($state) {
                 var vm = this;
-                if (!vm.ISState) return;
-                if (!vm.itemsLoaded) {
-                    // this handler is triggered on initial get too
+                if (!vm.itemsLoaded || vm.mergeResults) {
+                    // this handler is triggered on initial get() too.
                     return;
                 }
-                // rudimentary way to detect which type of pagination
-                // is active. ideally need to monitor resolution changes
-                vm.isInfiniteScroll = true;
                 var nxt = vm.params.page + 1;
                 if (nxt <= vm.pageCount) {
                     vm.$set(vm.params, 'page', nxt);
                     vm.mergeResults = true;
                     vm.get();
                 }
             },
@@ -1026,23 +1013,21 @@
                 var vm = this;
                 var pages = [];
                 for (var idx = vm.minDirectPageLink; idx <= vm.maxDirectPageLink; ++idx) {
                     pages.push(idx);
                 }
                 return pages;
             },
-            ISState: function() {
-                if (!this.$refs.infiniteLoading) return;
-                return this.$refs.infiniteLoading.stateChanger;
-            },
-            qs: function() {
-                return this.getQueryString({
-                    page: null
-                });
-            },
+        },
+        mounted: function() {
+            var vm = this;
+            window.addEventListener("scroll", vm.handleScroll);
+        },
+        unmounted: function() {
+            window.removeEventListener("scroll", vm.handleScroll);
         }
     }
 
 
     var sortableMixin = {
         data: function() {
             var defaultDir = this.$sortDirection || 'desc';
@@ -1137,15 +1122,14 @@
     }
 
 
     var itemListMixin = {
         mixins: [
             httpRequestMixin,
             paginationMixin,
-            filterableMixin,
             sortableMixin
         ],
         data: function() {
             return this.getInitData();
         },
         methods: {
             getInitData: function() {
@@ -1154,15 +1138,16 @@
                     params: {
                         // The following dates will be stored as `String` objects
                         // as oppossed to `moment` or `Date` objects because this
                         // is how form fields input="date" will update them.
                         start_at: null,
                         ends_at: null,
                         // The timezone for both start_at and ends_at.
-                        timezone: 'local'
+                        timezone: 'local',
+                        q: '',
                     },
                     itemsLoaded: false,
                     items: {
                         results: [],
                         count: 0
                     },
                     mergeResults: false,
@@ -1226,19 +1211,26 @@
                 vm.fetch(cb);
             },
             fetch: function(cb) {
                 let vm = this;
                 vm.lastGetParams = vm.getParams();
                 vm.reqGet(vm.url, vm.lastGetParams, cb);
             },
+            reload: function() {
+                let vm = this;
+                for (let idx = 0; idx < vm.preReload.length; ++idx) {
+                    vm[vm.preReload[idx]]();
+                }
+                vm.get();
+            },
         },
     };
 
 
-    var TypeAhead = Vue.component('typeahead', {
+    var typeAheadMixin = {
         mixins: [
             httpRequestMixin
         ],
         data: function data() {
             return {
                 url: null,
                 items: [],
@@ -1276,15 +1268,15 @@
                 var vm = this;
                 if (vm.current !== -1) {
                     vm.onHit(vm.items[vm.current]);
                 }
             },
 
             onHit: function onHit() {
-                Vue.util.warn('You need to implement the `onHit` method', this);
+                console.warn('You need to implement the `onHit` method', this);
             },
 
             reset: function() {
                 var vm = this;
                 vm.clear();
                 vm.query = '';
             },
@@ -1350,18 +1342,18 @@
             }
         },
         mounted: function() {
             if (this.$el.dataset && this.$el.dataset.url) {
                 this.url = this.$el.dataset.url;
             }
         }
-    });
+    };
 
     // attach properties to the exports object to define
     // the exported module properties.
     exports.httpRequestMixin = httpRequestMixin;
     exports.itemListMixin = itemListMixin;
     exports.itemMixin = itemMixin;
     exports.messagesMixin = messagesMixin;
     exports.paramsMixin = paramsMixin;
-    exports.TypeAhead = TypeAhead;
+    exports.typeAheadMixin = typeAheadMixin;
 }));
```

### Comparing `djaodjin-survey-0.9.3/survey/static/js/djaodjin-set.js` & `djaodjin-survey-0.9.5/survey/static/js/djaodjin-set.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/static/js/djaodjin-survey-vue.js` & `djaodjin-survey-0.9.5/survey/static/js/djaodjin-survey-vue.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -281,15 +281,139 @@
     },
     mounted: function() {
         this.get();
     }
 });
 
 
-var AccountTypeAhead = Vue.component('account-typeahead', TypeAhead.extend({
+
+
+// shows comparaison matrices
+Vue.component('compare-dashboard', {
+    mixins: [
+        itemMixin
+    ],
+    data: function() {
+        return {
+            url: this.$urls.matrix_api,
+            colors: this.$colorsTheme ? this.$colorsTheme : ['#f0ad4e'],
+            getCb: 'updateCharts',
+            charts: {}
+        }
+    },
+    methods: {
+        updateCharts: function(resp) {
+            var vm = this;
+            vm.item = resp;
+            vm.itemLoaded = true;
+            var chartsData = {};
+            for (var tdx = 0; tdx < resp.length; ++tdx) {
+                var table = resp[tdx];
+                var labels = [];
+                var datasets = [];
+                var chartKey = table.slug;
+                for (var idx = 0; idx < table.cohorts.length; ++idx) {
+                    labels.push(table.cohorts[idx].title);
+                }
+                var data = [];
+                for (var key in table.values) {
+                    if (table.values.hasOwnProperty(key)) {
+                        data.push(table.values[key]);
+                    }
+                }
+                datasets.push({
+                    label: table.title,
+                    backgroundColor: vm.colors,
+                    borderColor: vm.colors,
+                    data: data
+                });
+                const chartLookup = chartKey.startsWith('aggregates-') ? chartKey.substr(11) : chartKey;
+                if (chartsData[chartLookup]) {
+                    /*
+                    datasets['type'] = 'line'
+                    chartsData[chartLookup].datasets = [
+                        chartsData[chartLookup].datasets,
+                        datasets,
+                    ];
+                    */
+                } else {
+                    datasets['type'] = 'bar'
+                    chartsData[chartLookup] = {
+                        datasets: datasets,
+                        labels: labels,
+                    };
+                }
+            }
+            for (var chartKey in chartsData) {
+                if (!chartsData.hasOwnProperty(chartKey)) continue;
+
+                var table = chartsData[chartKey];
+                if (vm.charts[chartKey]) {
+                    vm.charts[chartKey].destroy();
+                }
+                const element = document.getElementById(chartKey);
+                if (element) {
+                    if (table.length >= 2) {
+                        vm.charts[chartKey] = new Chart(
+                            element, {
+                                data: table,
+                                options: {
+                                    responsive: true,
+                                    plugins: {
+                                        legend: {
+                                            display: false,
+                                        },
+                                        title: {
+                                            display: false,
+                                            text: table.title
+                                        }
+                                    }
+                                },
+                            },
+
+                        );
+                    } else {
+                        vm.charts[chartKey] = new Chart(
+                            element, {
+                                type: 'bar',
+                                data: table,
+                                options: {
+                                    responsive: true,
+                                    scales: {
+                                        x: {
+                                            display: (chartKey === 'totals'),
+                                        }
+                                    },
+                                    plugins: {
+                                        legend: {
+                                            display: false,
+                                        },
+                                        title: {
+                                            display: false,
+                                            text: table.title
+                                        }
+                                    }
+                                },
+                            }
+                        );
+                    }
+                }
+            }
+        },
+    },
+    mounted: function() {
+        this.get();
+    }
+});
+
+
+var AccountTypeAhead = Vue.component('account-typeahead', {
+    mixins: [
+        typeAheadMixin
+    ],
     props: ['dataset'],
     data: function data() {
         return {
             url: this.$urls.api_account_candidates,
             items: [],
             query: '',
             current: -1,
@@ -347,25 +471,24 @@
                 vm.search();
             }
         },
         onHit: function onHit(newItem) {
             var vm = this;
             vm.$emit('selectitem', vm.dataset, newItem);
             /*XXX
-                  if( typeof newItem.full_name !== 'undefined' ) {
-                      vm.query = newItem.full_name;
-                  } else {
-                      vm.query = newItem;
-                  }
+              if( typeof newItem.full_name !== 'undefined' ) {
+              vm.query = newItem.full_name;
+              } else {
+              vm.query = newItem;
+              }
             */
             vm.reset();
-            vm.clear();
         }
     }
-}));
+});
 
 
 Vue.component('grantee-typeahead', AccountTypeAhead.extend({
     props: ['dataset', 'defaultMessage', 'showAccounts'],
     data: function data() {
         return {
             url: this.$urls.api_account_candidates,
@@ -418,124 +541,35 @@
             selectFirst: false,
             queryParamName: 'q'
         };
     }
 }));
 
 
-// shows comparaison matrices
-Vue.component('compare-dashboard', {
+Vue.component('default-unit-typeahead', {
     mixins: [
-        itemMixin
+        typeAheadMixin
     ],
-    data: function() {
+    props: [
+        'question'
+    ],
+    data: function data() {
         return {
-            url: this.$urls.matrix_api,
-            colors: this.$colorsTheme ? this.$colorsTheme : ['#f0ad4e'],
-            getCb: 'updateCharts',
-            charts: {}
-        }
+            url: this.$urls.api_units,
+        };
     },
     methods: {
-        updateCharts: function(resp) {
+        onHit: function onHit(newItem) {
             var vm = this;
-            vm.item = resp;
-            vm.itemLoaded = true;
-            var chartsData = {};
-            for (var tdx = 0; tdx < resp.length; ++tdx) {
-                var table = resp[tdx];
-                var labels = [];
-                var datasets = [];
-                var chartKey = table.slug;
-                for (var idx = 0; idx < table.cohorts.length; ++idx) {
-                    labels.push(table.cohorts[idx].title);
-                }
-                var data = [];
-                for (var key in table.values) {
-                    if (table.values.hasOwnProperty(key)) {
-                        data.push(table.values[key]);
-                    }
-                }
-                datasets.push({
-                    label: table.title,
-                    backgroundColor: vm.colors,
-                    borderColor: vm.colors,
-                    data: data
-                });
-                const chartLookup = chartKey.startsWith('aggregates-') ? chartKey.substr(11) : chartKey;
-                if (chartsData[chartLookup]) {
-                    /*
-                    datasets['type'] = 'line'
-                    chartsData[chartLookup].datasets = [
-                        chartsData[chartLookup].datasets,
-                        datasets,
-                    ];
-                    */
-                } else {
-                    datasets['type'] = 'bar'
-                    chartsData[chartLookup] = {
-                        datasets: datasets,
-                        labels: labels,
-                    };
-                }
+            if (newItem.title) {
+                vm.query = newItem.title;
             }
-            for (var chartKey in chartsData) {
-                if (!chartsData.hasOwnProperty(chartKey)) continue;
-
-                var table = chartsData[chartKey];
-                if (vm.charts[chartKey]) {
-                    vm.charts[chartKey].destroy();
-                }
-                const element = document.getElementById(chartKey);
-                if (element) {
-                    if (table.length >= 2) {
-                        vm.charts[chartKey] = new Chart(
-                            element, {
-                                data: table,
-                                options: {
-                                    responsive: true,
-                                    plugins: {
-                                        legend: {
-                                            display: false,
-                                        },
-                                        title: {
-                                            display: false,
-                                            text: table.title
-                                        }
-                                    }
-                                },
-                            },
-
-                        );
-                    } else {
-                        vm.charts[chartKey] = new Chart(
-                            element, {
-                                type: 'bar',
-                                data: table,
-                                options: {
-                                    responsive: true,
-                                    scales: {
-                                        x: {
-                                            display: (chartKey === 'totals'),
-                                        }
-                                    },
-                                    plugins: {
-                                        legend: {
-                                            display: false,
-                                        },
-                                        title: {
-                                            display: false,
-                                            text: table.title
-                                        }
-                                    }
-                                },
-                            }
-                        );
-                    }
-                }
-            }
-        },
+            vm.$emit('selectitem', newItem, vm.question);
+        }
     },
     mounted: function() {
-        this.get();
+        var vm = this;
+        if (vm.question && vm.question.default_unit) {
+            vm.query = vm.question.default_unit;
+        }
     }
 });
```

### Comparing `djaodjin-survey-0.9.3/survey/static/js/djaodjin-survey.js` & `djaodjin-survey-0.9.5/survey/static/js/djaodjin-survey.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/static/js/matrix-chart.js` & `djaodjin-survey-0.9.5/survey/static/js/matrix-chart.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templates/survey/answer_form.html` & `djaodjin-survey-0.9.5/survey/templates/survey/answer_form.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templates/survey/campaigns/index.html` & `djaodjin-survey-0.9.5/survey/templates/survey/campaigns/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templates/survey/categorize.html` & `djaodjin-survey-0.9.5/survey/templates/survey/categorize.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templates/survey/matrix/index.html` & `djaodjin-survey-0.9.5/survey/templates/survey/matrix/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templates/survey/matrix/matrix.html` & `djaodjin-survey-0.9.5/survey/templates/survey/matrix/matrix.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templates/survey/portfolios.html` & `djaodjin-survey-0.9.5/survey/templates/survey/portfolios.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templates/survey/question_list.html` & `djaodjin-survey-0.9.5/survey/templates/survey/question_list.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templates/survey/result.html` & `djaodjin-survey-0.9.5/survey/templates/survey/result.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templates/survey/result_quizz.html` & `djaodjin-survey-0.9.5/survey/templates/survey/result_quizz.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templates/survey/sample_create.html` & `djaodjin-survey-0.9.5/survey/templates/survey/sample_create.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/templatetags/survey_tags.py` & `djaodjin-survey-0.9.5/survey/templatetags/survey_tags.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/__init__.py` & `djaodjin-survey-0.9.5/survey/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/__init__.py` & `djaodjin-survey-0.9.5/survey/urls/views/__init__.py`

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

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/campaigns.py` & `djaodjin-survey-0.9.5/survey/urls/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/filters.py` & `djaodjin-survey-0.9.5/survey/urls/api/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/matrix.py` & `djaodjin-survey-0.9.5/survey/urls/api/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/metrics.py` & `djaodjin-survey-0.9.5/survey/urls/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/noauth.py` & `djaodjin-survey-0.9.5/survey/urls/api/noauth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/portfolios.py` & `djaodjin-survey-0.9.5/survey/urls/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/sample/__init__.py` & `djaodjin-survey-0.9.5/survey/urls/api/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/sample/reset.py` & `djaodjin-survey-0.9.5/survey/urls/api/sample/reset.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/api/sample/update.py` & `djaodjin-survey-0.9.5/survey/urls/api/sample/update.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/views/__init__.py` & `djaodjin-survey-0.9.5/setup.py`

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

### Comparing `djaodjin-survey-0.9.3/survey/urls/views/campaigns.py` & `djaodjin-survey-0.9.5/survey/urls/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/views/matrices.py` & `djaodjin-survey-0.9.5/survey/urls/views/matrices.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/views/portfolios.py` & `djaodjin-survey-0.9.5/survey/urls/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/urls/views/samples.py` & `djaodjin-survey-0.9.5/survey/urls/views/samples.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/utils.py` & `djaodjin-survey-0.9.5/survey/utils.py`

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

### Comparing `djaodjin-survey-0.9.3/survey/views/campaigns.py` & `djaodjin-survey-0.9.5/survey/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/views/createquestion.py` & `djaodjin-survey-0.9.5/survey/views/createquestion.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/views/edit.py` & `djaodjin-survey-0.9.5/survey/views/edit.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/views/matrix.py` & `djaodjin-survey-0.9.5/survey/views/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/views/portfolios.py` & `djaodjin-survey-0.9.5/survey/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.3/survey/views/sample.py` & `djaodjin-survey-0.9.5/survey/views/sample.py`

 * *Files identical despite different names*

