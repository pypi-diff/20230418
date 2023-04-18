# Comparing `tmp/aa_structuretimers-1.5.0.tar.gz` & `tmp/aa_structuretimers-1.5.1.tar.gz`

## Comparing `aa_structuretimers-1.5.0.tar` & `aa_structuretimers-1.5.1.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/__init__.py
--rw-r--r--   0        0        0    14349 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/admin.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/app_settings.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/apps.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/auth_hooks.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/constants.py
--rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/forms.py
--rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/managers.py
--rw-r--r--   0        0        0    35753 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/models.py
--rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tasks.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/urls.py
--rw-r--r--   0        0        0    17849 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/views.py
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/django.pot
--rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/ko/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/management/commands/__init__.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/management/commands/structuretimers_load_eve.py
--rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/management/commands/structuretimers_migrate_timers.py
--rw-r--r--   0        0        0    20775 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/migrations/0001_initial.py
--rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/migrations/0002_distances_from_staging.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/migrations/0003_add_preliminary_timers.py
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/migrations/0004_add_space_type_and_region_filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/migrations/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/css/global.css
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/css/timer_edit.css
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/css/timer_list.css
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/structuretimers_logo.png
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/js/timer_edit.js
--rw-r--r--   0        0        0     9993 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/js/timer_list.js
--rw-r--r--   0        0        0    15823 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.css
--rw-r--r--   0        0        0    72483 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.js
--rw-r--r--   0        0        0    16792 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-bootstrap-theme-0.1.0-beta.10/select2-bootstrap.min.css
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/base.html
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_confirm_delete.html
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_create_form.html
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_detail.html
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_edit.html
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_list.html
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_update_form.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/partials/cancel_button.html
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/partials/preliminary_list_table.html
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/partials/timer_list_table.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/__init__.py
--rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_admin.py
--rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_commands.py
--rw-r--r--   0        0        0    10580 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_forms.py
--rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_integration.py
--rw-r--r--   0        0        0    47940 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_models.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_navigation_highlight.py
--rw-r--r--   0        0        0    18750 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_tasks.py
--rw-r--r--   0        0        0    20014 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/test_views.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/utils.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/__init__.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0    10514 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/factory.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/fixtures.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/generate_timers.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0    32649 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tests/testdata/test_image.jpg
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/structuretimers/tools/drop_tables.sql
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/LICENSE
--rw-r--r--   0        0        0    10160 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/README.md
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/__init__.py
+-rw-r--r--   0        0        0    14349 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/admin.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/app_settings.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/apps.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/auth_hooks.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/constants.py
+-rw-r--r--   0        0        0    11466 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/forms.py
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/managers.py
+-rw-r--r--   0        0        0    35753 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/models.py
+-rw-r--r--   0        0        0    12124 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tasks.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/urls.py
+-rw-r--r--   0        0        0    17849 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/views.py
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/django.pot
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7556 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/management/commands/__init__.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/management/commands/structuretimers_load_eve.py
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/management/commands/structuretimers_migrate_timers.py
+-rw-r--r--   0        0        0    20775 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/migrations/0001_initial.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/migrations/0002_distances_from_staging.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/migrations/0003_add_preliminary_timers.py
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/migrations/0004_add_space_type_and_region_filters.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/migrations/0005_alter_notificationrule_exclude_space_types_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/migrations/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/css/global.css
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/css/timer_edit.css
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/css/timer_list.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/img/structuretimers_logo.png
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/js/timer_edit.js
+-rw-r--r--   0        0        0     9993 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/js/timer_list.js
+-rw-r--r--   0        0        0    15823 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.css
+-rw-r--r--   0        0        0    72483 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.js
+-rw-r--r--   0        0        0    16792 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/static/structuretimers/vendor/select2-bootstrap-theme-0.1.0-beta.10/select2-bootstrap.min.css
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/base.html
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/timer_confirm_delete.html
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/timer_create_form.html
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/timer_detail.html
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/timer_edit.html
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/timer_list.html
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/timer_update_form.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/partials/cancel_button.html
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/partials/preliminary_list_table.html
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/partials/timer_list_table.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/__init__.py
+-rw-r--r--   0        0        0     7438 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/test_admin.py
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/test_commands.py
+-rw-r--r--   0        0        0    10580 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/test_forms.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/test_integration.py
+-rw-r--r--   0        0        0    47940 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/test_models.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/test_navigation_highlight.py
+-rw-r--r--   0        0        0    18750 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/test_tasks.py
+-rw-r--r--   0        0        0    20014 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/test_views.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/utils.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/testdata/__init__.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    10514 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/testdata/factory.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/testdata/fixtures.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/testdata/generate_timers.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0    32649 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tests/testdata/test_image.jpg
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/structuretimers/tools/drop_tables.sql
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/LICENSE
+-rw-r--r--   0        0        0    10160 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/README.md
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    11619 2020-02-02 00:00:00.000000 aa_structuretimers-1.5.1/PKG-INFO
```

### Comparing `aa_structuretimers-1.5.0/structuretimers/admin.py` & `aa_structuretimers-1.5.1/structuretimers/admin.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/app_settings.py` & `aa_structuretimers-1.5.1/structuretimers/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/auth_hooks.py` & `aa_structuretimers-1.5.1/structuretimers/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/forms.py` & `aa_structuretimers-1.5.1/structuretimers/forms.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/managers.py` & `aa_structuretimers-1.5.1/structuretimers/managers.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/models.py` & `aa_structuretimers-1.5.1/structuretimers/models.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tasks.py` & `aa_structuretimers-1.5.1/structuretimers/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/urls.py` & `aa_structuretimers-1.5.1/structuretimers/urls.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/views.py` & `aa_structuretimers-1.5.1/structuretimers/views.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/django.pot` & `aa_structuretimers-1.5.1/structuretimers/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/de/LC_MESSAGES/django.po` & `aa_structuretimers-1.5.1/structuretimers/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/en/LC_MESSAGES/django.po` & `aa_structuretimers-1.5.1/structuretimers/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/es/LC_MESSAGES/django.po` & `aa_structuretimers-1.5.1/structuretimers/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/fr_FR/LC_MESSAGES/django.po` & `aa_structuretimers-1.5.1/structuretimers/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/it_IT/LC_MESSAGES/django.po` & `aa_structuretimers-1.5.1/structuretimers/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/ja/LC_MESSAGES/django.po` & `aa_structuretimers-1.5.1/structuretimers/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/ko/LC_MESSAGES/django.po` & `aa_structuretimers-1.5.1/structuretimers/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/ko_KR/LC_MESSAGES/django.po` & `aa_structuretimers-1.5.1/structuretimers/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/ru/LC_MESSAGES/django.po` & `aa_structuretimers-1.5.1/structuretimers/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_structuretimers-1.5.1/structuretimers/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/management/commands/structuretimers_load_eve.py` & `aa_structuretimers-1.5.1/structuretimers/management/commands/structuretimers_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/management/commands/structuretimers_migrate_timers.py` & `aa_structuretimers-1.5.1/structuretimers/management/commands/structuretimers_migrate_timers.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/migrations/0001_initial.py` & `aa_structuretimers-1.5.1/structuretimers/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/migrations/0002_distances_from_staging.py` & `aa_structuretimers-1.5.1/structuretimers/migrations/0002_distances_from_staging.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/migrations/0003_add_preliminary_timers.py` & `aa_structuretimers-1.5.1/structuretimers/migrations/0003_add_preliminary_timers.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/migrations/0004_add_space_type_and_region_filters.py` & `aa_structuretimers-1.5.1/structuretimers/migrations/0004_add_space_type_and_region_filters.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/css/global.css` & `aa_structuretimers-1.5.1/structuretimers/static/structuretimers/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/css/timer_list.css` & `aa_structuretimers-1.5.1/structuretimers/static/structuretimers/css/timer_list.css`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/Spinner-1s-64px-dark.gif` & `aa_structuretimers-1.5.1/structuretimers/static/structuretimers/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/Spinner-1s-64px-light.gif` & `aa_structuretimers-1.5.1/structuretimers/static/structuretimers/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/img/structuretimers_logo.png` & `aa_structuretimers-1.5.1/structuretimers/static/structuretimers/img/structuretimers_logo.png`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/js/timer_edit.js` & `aa_structuretimers-1.5.1/structuretimers/static/structuretimers/js/timer_edit.js`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/js/timer_list.js` & `aa_structuretimers-1.5.1/structuretimers/static/structuretimers/js/timer_list.js`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.css` & `aa_structuretimers-1.5.1/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.css`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.js` & `aa_structuretimers-1.5.1/structuretimers/static/structuretimers/vendor/select2-4.1.0-beta.1/select2.min.js`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/static/structuretimers/vendor/select2-bootstrap-theme-0.1.0-beta.10/select2-bootstrap.min.css` & `aa_structuretimers-1.5.1/structuretimers/static/structuretimers/vendor/select2-bootstrap-theme-0.1.0-beta.10/select2-bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_confirm_delete.html` & `aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/timer_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_detail.html` & `aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/timer_detail.html`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_edit.html` & `aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/timer_edit.html`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/timer_list.html` & `aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/timer_list.html`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/partials/preliminary_list_table.html` & `aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/partials/preliminary_list_table.html`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/templates/structuretimers/partials/timer_list_table.html` & `aa_structuretimers-1.5.1/structuretimers/templates/structuretimers/partials/timer_list_table.html`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/test_admin.py` & `aa_structuretimers-1.5.1/structuretimers/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/test_commands.py` & `aa_structuretimers-1.5.1/structuretimers/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/test_forms.py` & `aa_structuretimers-1.5.1/structuretimers/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/test_integration.py` & `aa_structuretimers-1.5.1/structuretimers/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/test_models.py` & `aa_structuretimers-1.5.1/structuretimers/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/test_navigation_highlight.py` & `aa_structuretimers-1.5.1/structuretimers/tests/test_navigation_highlight.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/test_tasks.py` & `aa_structuretimers-1.5.1/structuretimers/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/test_views.py` & `aa_structuretimers-1.5.1/structuretimers/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/testdata/eveuniverse.json` & `aa_structuretimers-1.5.1/structuretimers/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/testdata/factory.py` & `aa_structuretimers-1.5.1/structuretimers/tests/testdata/factory.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/testdata/fixtures.py` & `aa_structuretimers-1.5.1/structuretimers/tests/testdata/fixtures.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/testdata/generate_timers.py` & `aa_structuretimers-1.5.1/structuretimers/tests/testdata/generate_timers.py`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tests/testdata/test_image.jpg` & `aa_structuretimers-1.5.1/structuretimers/tests/testdata/test_image.jpg`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/structuretimers/tools/drop_tables.sql` & `aa_structuretimers-1.5.1/structuretimers/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/LICENSE` & `aa_structuretimers-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/README.md` & `aa_structuretimers-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/pyproject.toml` & `aa_structuretimers-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_structuretimers-1.5.0/PKG-INFO` & `aa_structuretimers-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-structuretimers
-Version: 1.5.0
+Version: 1.5.1
 Summary: An app for keeping track of Eve Online structure timers with Alliance Auth and Discord
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-structuretimers
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-structuretimers
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-structuretimers/-/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-structuretimers/-/issues
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 License-Expression: MIT
```

