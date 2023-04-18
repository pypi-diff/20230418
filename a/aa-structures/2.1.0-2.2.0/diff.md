# Comparing `tmp/aa-structures-2.1.0.tar.gz` & `tmp/aa_structures-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-structures-2.1.0.tar", last modified: Tue Jan 31 01:15:24 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aa-structures-2.1.0.tar` & `aa_structures-2.2.0.tar`

### file list

```diff
@@ -1,208 +1,171 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.866642 aa-structures-2.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2020-10-22 17:29:44.000000 aa-structures-2.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      290 2020-10-22 17:29:44.000000 aa-structures-2.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5323 2023-01-31 01:15:24.866642 aa-structures-2.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4406 2022-08-11 17:23:18.000000 aa-structures-2.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.810642 aa-structures-2.1.0/aa_structures.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5323 2023-01-31 01:15:24.000000 aa-structures-2.1.0/aa_structures.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7772 2023-01-31 01:15:24.000000 aa-structures-2.1.0/aa_structures.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-31 01:15:24.000000 aa-structures-2.1.0/aa_structures.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      171 2023-01-31 01:15:24.000000 aa-structures-2.1.0/aa_structures.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-01-31 01:15:24.000000 aa-structures-2.1.0/aa_structures.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-31 01:15:24.866642 aa-structures-2.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-01-31 00:37:42.000000 aa-structures-2.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.818642 aa-structures-2.1.0/structures/
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-01-31 00:37:42.000000 aa-structures-2.1.0/structures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35768 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     6228 2022-08-11 17:12:19.000000 aa-structures-2.1.0/structures/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2022-01-19 15:26:06.000000 aa-structures-2.1.0/structures/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      915 2022-03-01 14:58:19.000000 aa-structures-2.1.0/structures/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      741 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.822642 aa-structures-2.1.0/structures/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-13 00:41:45.000000 aa-structures-2.1.0/structures/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    71555 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/core/notification_embeds.py
--rw-rw-rw-   0 root         (0) root         (0)    16436 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/core/notification_timers.py
--rw-rw-rw-   0 root         (0) root         (0)    19834 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/core/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)      623 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/core/sovereignty.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/core/starbases.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2021-05-01 16:36:15.000000 aa-structures-2.1.0/structures/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.822642 aa-structures-2.1.0/structures/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2022-09-10 17:27:22.000000 aa-structures-2.1.0/structures/helpers/general.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.822642 aa-structures-2.1.0/structures/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    13634 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/locale/de/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.822642 aa-structures-2.1.0/structures/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/locale/en/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.822642 aa-structures-2.1.0/structures/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     5784 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/locale/es/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/locale/ko/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.822642 aa-structures-2.1.0/structures/locale/ko/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      391 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/locale/ko/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.822642 aa-structures-2.1.0/structures/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      538 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/locale/ru/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.826642 aa-structures-2.1.0/structures/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    11588 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.826642 aa-structures-2.1.0/structures/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-07-06 21:23:42.000000 aa-structures-2.1.0/structures/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1443 2022-09-16 18:02:58.000000 aa-structures-2.1.0/structures/management/commands/structures_load_eve.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/management/commands/structures_preload_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)    18982 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.842642 aa-structures-2.1.0/structures/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    27006 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)    61811 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/migrations/0001_initial_new.py
--rw-rw-rw-   0 root         (0) root         (0)     3435 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/migrations/0002_auto_20191121_2335.py
--rw-rw-rw-   0 root         (0) root         (0)     2275 2022-09-16 13:11:05.000000 aa-structures-2.1.0/structures/migrations/0002_remove_eveuniverse_relation_names.py
--rw-rw-rw-   0 root         (0) root         (0)     1138 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/migrations/0003_auto_20191125_2157.py
--rw-rw-rw-   0 root         (0) root         (0)     1944 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/migrations/0004_auto_20191129_0308.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/migrations/0005_notification_created.py
--rw-rw-rw-   0 root         (0) root         (0)     2479 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/migrations/0006_auto_20200120_0147.py
--rw-rw-rw-   0 root         (0) root         (0)     4997 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0007_auto_20200123_1429.py
--rw-rw-rw-   0 root         (0) root         (0)     7132 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0008_auto_20200209_1638.py
--rw-rw-rw-   0 root         (0) root         (0)    24922 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/migrations/0009_localizations.py
--rw-rw-rw-   0 root         (0) root         (0)     3661 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/migrations/0010_sovereignty_map.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0011_last_online.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/migrations/0012_disable_pings.py
--rw-rw-rw-   0 root         (0) root         (0)     1903 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/migrations/0013_group_pings.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2021-01-10 20:36:03.000000 aa-structures-2.1.0/structures/migrations/0014_addtl_perm_unanchor.py
--rw-rw-rw-   0 root         (0) root         (0)     4244 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0015_refactor_notification_types.py
--rw-rw-rw-   0 root         (0) root         (0)     4438 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0016_char_join_leave_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     5010 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0017_war_dec_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     6143 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0018_restructure_notifications_2.py
--rw-rw-rw-   0 root         (0) root         (0)     4661 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0019_more_notification_types.py
--rw-rw-rw-   0 root         (0) root         (0)     4826 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0020_more_war_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     1067 2021-03-16 19:54:31.000000 aa-structures-2.1.0/structures/migrations/0021_add_corporation_permission.py
--rw-rw-rw-   0 root         (0) root         (0)     5142 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/migrations/0022_add_corp_app_notification_types.py
--rw-rw-rw-   0 root         (0) root         (0)     8579 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/migrations/0023_structure_fittings.py
--rw-rw-rw-   0 root         (0) root         (0)    11987 2021-04-30 14:20:37.000000 aa-structures-2.1.0/structures/migrations/0024_fix_name_fields_too_small.py
--rw-rw-rw-   0 root         (0) root         (0)     2849 2021-05-22 14:22:35.000000 aa-structures-2.1.0/structures/migrations/0025_add_poco_details.py
--rw-rw-rw-   0 root         (0) root         (0)     2983 2021-07-03 19:17:09.000000 aa-structures-2.1.0/structures/migrations/0026_rework_update_status.py
--rw-rw-rw-   0 root         (0) root         (0)     2745 2021-07-07 20:27:23.000000 aa-structures-2.1.0/structures/migrations/0027_create_owner_characters.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2021-07-06 21:23:42.000000 aa-structures-2.1.0/structures/migrations/0028_migrate_owner_characters.py
--rw-rw-rw-   0 root         (0) root         (0)    10529 2021-07-23 19:13:09.000000 aa-structures-2.1.0/structures/migrations/0029_custom_fuel_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     5284 2021-08-17 14:31:25.000000 aa-structures-2.1.0/structures/migrations/0030_update_refueled_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2373 2021-10-05 17:22:22.000000 aa-structures-2.1.0/structures/migrations/0031_add_service_up.py
--rw-rw-rw-   0 root         (0) root         (0)    11841 2021-12-17 19:21:23.000000 aa-structures-2.1.0/structures/migrations/0032_add_jump_fuel_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)     5363 2022-01-27 18:04:43.000000 aa-structures-2.1.0/structures/migrations/0033_fix_notification_type_fuel_alert.py
--rw-rw-rw-   0 root         (0) root         (0)     2309 2022-01-28 18:46:14.000000 aa-structures-2.1.0/structures/migrations/0034_add_structure_webhooks.py
--rw-rw-rw-   0 root         (0) root         (0)     5519 2022-02-21 22:00:28.000000 aa-structures-2.1.0/structures/migrations/0035_add_more_notifications_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2022-03-02 19:55:27.000000 aa-structures-2.1.0/structures/migrations/0036_django4_update.py
--rw-rw-rw-   0 root         (0) root         (0)     5822 2022-04-09 19:18:47.000000 aa-structures-2.1.0/structures/migrations/0037_add_billing_notification_types.py
--rw-rw-rw-   0 root         (0) root         (0)     5848 2022-05-30 21:05:57.000000 aa-structures-2.1.0/structures/migrations/0038_add_starbase_detail.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2022-07-06 13:36:19.000000 aa-structures-2.1.0/structures/migrations/0039_ownercharacter_error_count.py
--rw-rw-rw-   0 root         (0) root         (0)     9270 2022-08-11 17:23:18.000000 aa-structures-2.1.0/structures/migrations/0040_add_generated_notifications.py
--rw-rw-rw-   0 root         (0) root         (0)      570 2022-08-17 19:08:20.000000 aa-structures-2.1.0/structures/migrations/0041_notification_sender_can_be_null.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2022-08-17 19:08:20.000000 aa-structures-2.1.0/structures/migrations/0042_migrate_sender_category_other.py
--rw-rw-rw-   0 root         (0) root         (0)      695 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/migrations/0043_remove_services_localization.py
--rw-rw-rw-   0 root         (0) root         (0)     2026 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/migrations/0044_check_eveuniverse_fully_loaded.py
--rw-rw-rw-   0 root         (0) root         (0)     3380 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/migrations/0045_migrate_all_to_django_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.842642 aa-structures-2.1.0/structures/models/
--rw-rw-rw-   0 root         (0) root         (0)      505 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/models/eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)    40068 2023-01-31 00:37:42.000000 aa-structures-2.1.0/structures/models/notifications.py
--rw-rw-rw-   0 root         (0) root         (0)    52649 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/models/owners.py
--rw-rw-rw-   0 root         (0) root         (0)    34567 2022-09-16 13:11:05.000000 aa-structures-2.1.0/structures/models/structures.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2022-06-16 12:13:53.000000 aa-structures-2.1.0/structures/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/static/structures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.842642 aa-structures-2.1.0/structures/static/structures/css/
--rw-rw-rw-   0 root         (0) root         (0)     1165 2022-05-30 21:05:57.000000 aa-structures-2.1.0/structures/static/structures/css/global.css
--rw-rw-rw-   0 root         (0) root         (0)     1186 2021-12-14 22:54:11.000000 aa-structures-2.1.0/structures/static/structures/css/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.846642 aa-structures-2.1.0/structures/static/structures/img/
--rw-rw-rw-   0 root         (0) root         (0)    43262 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/Spinner-1s-64px-dark.gif
--rw-rw-rw-   0 root         (0) root         (0)    43381 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/Spinner-1s-64px-light.gif
--rw-rw-rw-   0 root         (0) root         (0)      908 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/eve_symbol_128.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.858642 aa-structures-2.1.0/structures/static/structures/img/pannel/
--rw-rw-rw-   0 root         (0) root         (0)      805 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/0h.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/0l.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/0m.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/0r.png
--rw-rw-rw-   0 root         (0) root         (0)      805 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/0s.png
--rw-rw-rw-   0 root         (0) root         (0)     2590 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/1h.png
--rw-rw-rw-   0 root         (0) root         (0)     1976 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/1l.png
--rw-rw-rw-   0 root         (0) root         (0)     2025 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/1m.png
--rw-rw-rw-   0 root         (0) root         (0)     2512 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/1r.png
--rw-rw-rw-   0 root         (0) root         (0)     3541 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/2h.png
--rw-rw-rw-   0 root         (0) root         (0)     2570 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/2l.png
--rw-rw-rw-   0 root         (0) root         (0)     2766 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/2m.png
--rw-rw-rw-   0 root         (0) root         (0)     3497 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/2r.png
--rw-rw-rw-   0 root         (0) root         (0)     4607 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/3h.png
--rw-rw-rw-   0 root         (0) root         (0)     3523 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/3l.png
--rw-rw-rw-   0 root         (0) root         (0)     3720 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/3m.png
--rw-rw-rw-   0 root         (0) root         (0)     4886 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/3r.png
--rw-rw-rw-   0 root         (0) root         (0)     5309 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/4h.png
--rw-rw-rw-   0 root         (0) root         (0)     4628 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/4l.png
--rw-rw-rw-   0 root         (0) root         (0)     4956 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/4m.png
--rw-rw-rw-   0 root         (0) root         (0)     9490 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/4s.png
--rw-rw-rw-   0 root         (0) root         (0)     6109 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/5h.png
--rw-rw-rw-   0 root         (0) root         (0)     5888 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/5l.png
--rw-rw-rw-   0 root         (0) root         (0)     6270 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/5m.png
--rw-rw-rw-   0 root         (0) root         (0)     7399 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/5s.png
--rw-rw-rw-   0 root         (0) root         (0)     7203 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/6h.png
--rw-rw-rw-   0 root         (0) root         (0)     7014 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/6l.png
--rw-rw-rw-   0 root         (0) root         (0)     7439 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/6m.png
--rw-rw-rw-   0 root         (0) root         (0)     8288 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/7h.png
--rw-rw-rw-   0 root         (0) root         (0)     8067 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/7l.png
--rw-rw-rw-   0 root         (0) root         (0)     8580 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/7m.png
--rw-rw-rw-   0 root         (0) root         (0)     9276 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/8h.png
--rw-rw-rw-   0 root         (0) root         (0)     8972 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/8l.png
--rw-rw-rw-   0 root         (0) root         (0)     9541 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/8m.png
--rw-rw-rw-   0 root         (0) root         (0)      195 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/blank.png
--rw-rw-rw-   0 root         (0) root         (0)    16840 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/circle.png
--rw-rw-rw-   0 root         (0) root         (0)    33523 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/dustwheel.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/h.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/l.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/m.png
--rw-rw-rw-   0 root         (0) root         (0)     8879 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/noship.png
--rw-rw-rw-   0 root         (0) root         (0)     1480 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/r.png
--rw-rw-rw-   0 root         (0) root         (0)    43642 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/tyrannis.png
--rw-rw-rw-   0 root         (0) root         (0)    43560 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/tyrannis_blue.png
--rw-rw-rw-   0 root         (0) root         (0)    42833 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/tyrannis_darkred.png
--rw-rw-rw-   0 root         (0) root         (0)    38343 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/tyrannis_default.png
--rw-rw-rw-   0 root         (0) root         (0)    42868 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/pannel/tyrannis_revelations.png
--rw-rw-rw-   0 root         (0) root         (0)      496 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/static/structures/img/structures_logo.png
--rw-rw-rw-   0 root         (0) root         (0)   887006 2022-06-16 12:13:53.000000 aa-structures-2.1.0/structures/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)     8685 2023-01-31 00:37:42.000000 aa-structures-2.1.0/structures/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.806642 aa-structures-2.1.0/structures/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.858642 aa-structures-2.1.0/structures/templates/structures/
--rw-rw-rw-   0 root         (0) root         (0)      298 2021-04-29 22:23:58.000000 aa-structures-2.1.0/structures/templates/structures/base.html
--rw-rw-rw-   0 root         (0) root         (0)    21200 2022-07-14 15:22:09.000000 aa-structures-2.1.0/structures/templates/structures/main.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.862642 aa-structures-2.1.0/structures/templates/structures/modals/
--rw-rw-rw-   0 root         (0) root         (0)      264 2022-06-01 20:12:19.000000 aa-structures-2.1.0/structures/templates/structures/modals/fitting_assets.html
--rw-rw-rw-   0 root         (0) root         (0)     9531 2021-04-30 19:54:48.000000 aa-structures-2.1.0/structures/templates/structures/modals/fitting_gfx.html
--rw-rw-rw-   0 root         (0) root         (0)     2705 2022-06-01 20:12:19.000000 aa-structures-2.1.0/structures/templates/structures/modals/poco_details.html
--rw-rw-rw-   0 root         (0) root         (0)     4133 2022-06-01 20:12:19.000000 aa-structures-2.1.0/structures/templates/structures/modals/starbase_detail.html
--rw-rw-rw-   0 root         (0) root         (0)     4070 2022-06-01 20:12:19.000000 aa-structures-2.1.0/structures/templates/structures/modals/structure_details.html
--rw-rw-rw-   0 root         (0) root         (0)      998 2022-06-01 20:12:19.000000 aa-structures-2.1.0/structures/templates/structures/modals/tab_general_detail.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.862642 aa-structures-2.1.0/structures/templates/structures/partials/
--rw-rw-rw-   0 root         (0) root         (0)     1501 2022-05-30 21:05:57.000000 aa-structures-2.1.0/structures/templates/structures/partials/jump_gates_list.html
--rw-rw-rw-   0 root         (0) root         (0)     1034 2021-05-22 14:22:35.000000 aa-structures-2.1.0/structures/templates/structures/partials/poco_list.html
--rw-rw-rw-   0 root         (0) root         (0)     5947 2022-05-30 21:05:57.000000 aa-structures-2.1.0/structures/templates/structures/partials/structure_list.html
--rw-rw-rw-   0 root         (0) root         (0)     1568 2021-05-17 21:50:50.000000 aa-structures-2.1.0/structures/templates/structures/partials/structure_summary.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.866642 aa-structures-2.1.0/structures/templates/structures/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)      117 2022-05-31 14:09:14.000000 aa-structures-2.1.0/structures/templates/structures/templatetags/detail_title.html
--rw-rw-rw-   0 root         (0) root         (0)      375 2022-06-01 20:12:19.000000 aa-structures-2.1.0/structures/templates/structures/templatetags/list_asset.html
--rw-rw-rw-   0 root         (0) root         (0)      706 2022-06-01 15:59:29.000000 aa-structures-2.1.0/structures/templates/structures/templatetags/list_item.html
--rw-rw-rw-   0 root         (0) root         (0)      452 2022-06-01 20:12:19.000000 aa-structures-2.1.0/structures/templates/structures/templatetags/list_tax_item.html
--rw-rw-rw-   0 root         (0) root         (0)       68 2022-05-30 21:05:57.000000 aa-structures-2.1.0/structures/templates/structures/templatetags/list_title.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.866642 aa-structures-2.1.0/structures/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-30 21:05:57.000000 aa-structures-2.1.0/structures/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1601 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/templatetags/structures.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2022-05-30 21:05:57.000000 aa-structures-2.1.0/structures/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    21714 2022-09-10 17:58:40.000000 aa-structures-2.1.0/structures/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.866642 aa-structures-2.1.0/structures/webhooks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/webhooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6521 2022-08-12 12:50:01.000000 aa-structures-2.1.0/structures/webhooks/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2021-03-24 18:47:30.000000 aa-structures-2.1.0/structures/webhooks/managers.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2021-07-19 18:48:04.000000 aa-structures-2.1.0/structures/webhooks/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-31 01:15:24.866642 aa-structures-2.1.0/structures/webhooks/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-10-22 17:29:44.000000 aa-structures-2.1.0/structures/webhooks/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6395 2021-12-10 16:02:55.000000 aa-structures-2.1.0/structures/webhooks/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2021-02-14 22:48:19.000000 aa-structures-2.1.0/structures/webhooks/tests/test_utils.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/__init__.py
+-rw-r--r--   0        0        0    35982 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/admin.py
+-rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/app_settings.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/apps.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/auth_hooks.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/checks.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/constants.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/forms.py
+-rw-r--r--   0        0        0    18930 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/managers.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/providers.py
+-rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/swagger.json
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tasks.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/urls.py
+-rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/__init__.py
+-rw-r--r--   0        0        0    71555 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/notification_embeds.py
+-rw-r--r--   0        0        0    16436 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/notification_timers.py
+-rw-r--r--   0        0        0    19834 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/serializers.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/sovereignty.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/core/starbases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/helpers/__init__.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/helpers/general.py
+-rw-r--r--   0        0        0    13634 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    60908 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47014 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5784 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    55395 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47024 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    47177 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    58666 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/management/commands/__init__.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/management/commands/structures_load_eve.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/management/commands/structures_preload_eveuniverse.py
+-rw-r--r--   0        0        0    59315 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/migrations/0002_remove_eveuniverse_relation_names.py
+-rw-r--r--   0        0        0    44042 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/migrations/0003_add_localization_and_unique_key.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/migrations/__init__.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/models/__init__.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/models/eveuniverse.py
+-rw-r--r--   0        0        0    42377 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/models/notifications.py
+-rw-r--r--   0        0        0    53989 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/models/owners.py
+-rw-r--r--   0        0        0    37246 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/models/structures.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/css/global.css
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/css/main.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/eve_symbol_128.png
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/structures_logo.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/0h.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/0l.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/0m.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/0r.png
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/0s.png
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/1h.png
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/1l.png
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/1m.png
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/1r.png
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/2h.png
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/2l.png
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/2m.png
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/2r.png
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/3h.png
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/3l.png
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/3m.png
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/3r.png
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/4h.png
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/4l.png
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/4m.png
+-rw-r--r--   0        0        0     9490 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/4s.png
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/5h.png
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/5l.png
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/5m.png
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/5s.png
+-rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/6h.png
+-rw-r--r--   0        0        0     7014 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/6l.png
+-rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/6m.png
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/7h.png
+-rw-r--r--   0        0        0     8067 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/7l.png
+-rw-r--r--   0        0        0     8580 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/7m.png
+-rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/8h.png
+-rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/8l.png
+-rw-r--r--   0        0        0     9541 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/8m.png
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/blank.png
+-rw-r--r--   0        0        0    16840 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/circle.png
+-rw-r--r--   0        0        0    33523 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/dustwheel.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/h.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/l.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/m.png
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/noship.png
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/r.png
+-rw-r--r--   0        0        0    43642 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis.png
+-rw-r--r--   0        0        0    43560 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_blue.png
+-rw-r--r--   0        0        0    42833 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_darkred.png
+-rw-r--r--   0        0        0    38343 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_default.png
+-rw-r--r--   0        0        0    42868 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_revelations.png
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/base.html
+-rw-r--r--   0        0        0    21200 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/main.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/fitting_assets.html
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/fitting_gfx.html
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/poco_details.html
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/starbase_detail.html
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/structure_details.html
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/modals/tab_general_detail.html
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/partials/jump_gates_list.html
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/partials/poco_list.html
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/partials/structure_list.html
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/partials/structure_summary.html
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/templatetags/detail_title.html
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/templatetags/list_asset.html
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/templatetags/list_item.html
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/templatetags/list_tax_item.html
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templates/structures/templatetags/list_title.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templatetags/__init__.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/templatetags/structures.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/__init__.py
+-rw-r--r--   0        0        0    20318 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_admin.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_checks.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_helpers.py
+-rw-r--r--   0        0        0    20151 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_integration.py
+-rw-r--r--   0        0        0    26102 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_managers_1.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_managers_3.py
+-rw-r--r--   0        0        0    18409 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_tasks.py
+-rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/test_views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/__init__.py
+-rw-r--r--   0        0        0    10982 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_notification_embeds.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_notification_embeds_2.py
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_notification_structuretimers.py
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_notifications_timerboard.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_serializers.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_sovereignty.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/core/test_starbases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/__init__.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_eveuniverse.py
+-rw-r--r--   0        0        0    38429 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_notifications_1.py
+-rw-r--r--   0        0        0    31553 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_notifications_2.py
+-rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_notifications_3.py
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_notifications_discord.py
+-rw-r--r--   0        0        0    26807 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_owners_1.py
+-rw-r--r--   0        0        0    54158 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_owners_2.py
+-rw-r--r--   0        0        0    37407 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_owners_3.py
+-rw-r--r--   0        0        0    37744 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/models/test_structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0    33188 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/entities.json
+-rw-r--r--   0        0        0    13864 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/esi_data.json
+-rw-r--r--   0        0        0   979813 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/factories.py
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/factories_2.py
+-rw-r--r--   0        0        0     5746 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/generate_notifications.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/generate_notifications_2.py
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/generate_structures.py
+-rw-r--r--   0        0        0    26820 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/helpers.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/tasks_loadtest.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/tests/testdata/test_generate_structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/__init__.py
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/core.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/managers.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/tests/__init__.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/tests/test_core.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_structures-2.2.0/structures/webhooks/tests/test_utils.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 aa_structures-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_structures-2.2.0/LICENSE
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 aa_structures-2.2.0/README.md
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 aa_structures-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 aa_structures-2.2.0/PKG-INFO
```

### Comparing `aa-structures-2.1.0/LICENSE` & `aa_structures-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/PKG-INFO` & `aa_structures-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 Metadata-Version: 2.1
 Name: aa-structures
-Version: 2.1.0
+Version: 2.2.0
 Summary: App for managing Eve Online structures with Alliance Auth
-Home-page: https://gitlab.com/ErikKalkoken/aa-structures
-Author: Erik Kalkoken
-Author-email: kalkoken87@gmail.com
-License: MIT
-Platform: UNKNOWN
+Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-structures
+Project-URL: Documentation, https://aa-structures.readthedocs.io/en/latest/
+Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-structures
+Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-structures/-/blob/master/CHANGELOG.md
+Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-structures/-/issues
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
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.8
+Requires-Python: >=3.8
+Requires-Dist: allianceauth-app-utils>=1.14.2
+Requires-Dist: allianceauth>=3.0.0
+Requires-Dist: dhooks-lite>=0.6.1
+Requires-Dist: django-eveuniverse>=0.17
+Requires-Dist: django-multiselectfield
+Requires-Dist: django-navhelper
+Requires-Dist: pytz!=2022.2
+Requires-Dist: redis-simple-mq>=0.4
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Structures
 
 App for managing Eve Online structures with Alliance Auth.
 
 [![release](https://img.shields.io/pypi/v/aa-structures?label=release)](https://pypi.org/project/aa-structures/)
 [![python](https://img.shields.io/pypi/pyversions/aa-structures)](https://pypi.org/project/aa-structures/)
@@ -94,9 +104,7 @@
 
 The tax rate and access configuration of customs offices is visible too:
 ![Poco details](https://i.imgur.com/5XXDCsQ.png)
 
 This is an example for a notification posted on Discord:
 
 ![Notification example](https://i.imgur.com/oqBqeFy.png)
-
-
```

### Comparing `aa-structures-2.1.0/README.md` & `aa_structures-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/admin.py` & `aa_structures-2.2.0/structures/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from django.conf import settings
 from django.contrib import admin
 from django.db import models
 from django.db.models import Prefetch
 from django.db.models.functions import Lower
 from django.utils.html import format_html
+from django.utils.translation import gettext as _
 
 from allianceauth.eveonline.models import EveAllianceInfo, EveCorporationInfo
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.django import admin_boolean_icon_html
 from app_utils.logging import LoggerAddTag
 
 from . import __title__, app_settings, tasks
@@ -103,15 +104,15 @@
         color = Webhook.Color(obj.color)
         return format_html(
             '<span style="color: {};">&#9646;</span>{}',
             color.css_color,
             color.label,
         )
 
-    @admin.display(description="Sent fuel notifications for selected configuration")
+    @admin.display(description=_("Sent fuel notifications for selected configuration"))
     def send_fuel_notifications(self, request, queryset):
         item_count = 0
         for obj in queryset:
             obj.send_new_notifications(force=True)
             item_count += 1
         tasks.send_queued_messages_for_webhooks(Webhook.objects.filter(is_active=True))
         self.message_user(
@@ -128,15 +129,15 @@
         "end",
         "repeat",
     ) + BaseFuelAlertConfigAdmin.list_display
     fieldsets = (
         (
             "Timeing",
             {
-                "description": (
+                "description": _(
                     "Timing configuration for sending fuel notifications. "
                     "Note that the first notification will be sent at the exact "
                     "start hour, and the last notification will be sent one repeat "
                     "before the end hour."
                 ),
                 "fields": ("start", "end", "repeat"),
             },
@@ -232,77 +233,77 @@
         ).select_related("owner", "owner__corporation")
 
     def _notification_id(self, obj):
         return obj.notification_id
 
     def _webhooks(self, obj):
         if not obj.can_be_rendered:
-            return format_html("<i>N/A</i>")
+            return format_html("<i>{}</i>", _("N/A"))
         webhooks_qs = obj.owner.webhooks.all()
         if obj.structures_with_webhooks:
             webhooks_qs = Webhook.objects.none()
             for structure in obj.structures_with_webhooks:
                 webhooks_qs |= structure.webhooks.all()
         names = list(
             {
                 webhook.name
                 for webhook in webhooks_qs
                 if obj.notif_type in webhook.notification_types
             }
         )
         if not names:
             return format_html(
-                '<b><span style="color: orange">⚠ Not configured</span></b>'
+                '<b><span style="color: orange">⚠ {}</span></b>', _("Not configured")
             )
         return lines_sorted_html(names)
 
-    def _structures(self, obj) -> Optional[list]:
+    def _structures(self, obj) -> Optional[str]:
         if obj.is_structure_related:
             structures = [str(structure) for structure in obj.structures.all()]
             return lines_sorted_html(structures) if structures else "?"
         return None
 
     def _is_sent(self, obj):
         value = obj.is_sent if obj.can_be_rendered else None
         return admin_boolean_icon_html(value)
 
     def _is_timer_added(self, obj):
         value = obj.is_timer_added if obj.can_have_timer else None
         return admin_boolean_icon_html(value)
 
-    @admin.display(description="Mark selected notifications as sent")
+    @admin.display(description=_("Mark selected notifications as sent"))
     def mark_as_sent(self, request, queryset):
         queryset.update(is_sent=True)
         self.message_user(
             request, "{} notifications marked as sent".format(queryset.count())
         )
 
-    @admin.display(description="Mark selected notifications as unsent")
+    @admin.display(description=_("Mark selected notifications as unsent"))
     def mark_as_unsent(self, request, queryset):
         queryset.update(is_sent=False)
         self.message_user(
             request, "{} notifications marked as unsent".format(queryset.count())
         )
 
-    @admin.display(description="Send selected notifications to configured webhooks")
+    @admin.display(description=_("Send selected notifications to configured webhooks"))
     def send_to_configured_webhooks(self, request, queryset):
         notifs_queued = 0
         for obj in queryset:
             if obj.can_be_rendered and obj.relevant_webhooks().exists():
                 if obj.send_to_configured_webhooks():
                     notifs_queued += 1
         if notifs_queued:
             tasks.send_queued_messages_for_webhooks(
                 Webhook.objects.filter(is_active=True)
             )
         self.message_user(
             request, f"Sent {notifs_queued}/{queryset.count()} generated messages."
         )
 
-    @admin.display(description="Process selected notifications for timerboard")
+    @admin.display(description=_("Process selected notifications for timerboard"))
     def add_or_remove_timer(self, request, queryset):
         notifications_count = 0
         ignored_count = 0
         for obj in queryset:
             if obj.add_or_remove_timer():
                 notifications_count += 1
             else:
@@ -433,16 +434,19 @@
         return None
 
     def _webhooks(self, obj):
         names = [webhook.name for webhook in obj.webhooks.all()]
         if names:
             return lines_sorted_html(names)
         return format_html(
-            '<span style="color: red">⚠ Notifications can not be sent, '
-            "because there is no webhook configured for this owner.</span>"
+            '<span style="color: red">⚠ {}</span>',
+            _(
+                "Notifications can not be sent, "
+                "because there is no webhook configured for this owner."
+            ),
         )
 
     @admin.display(description="active", boolean=True)
     def _is_active(self, obj):
         return obj.is_active
 
     @admin.display(description="alliance main")
@@ -452,46 +456,48 @@
 
     @admin.display(description="services up", boolean=True)
     def _is_sync_ok(self, obj):
         if not obj.is_active:
             return None
         return obj.is_up
 
-    @admin.display(description="Activate selected owners")
+    @admin.display(description=_("Activate selected owners"))
     def activate_owners(self, request, queryset):
         queryset.update(is_active=True)
         self.message_user(request, f"Activated {queryset.count()} owners")
 
-    @admin.display(description="Deactivate selected owner")
+    @admin.display(description=_("Deactivate selected owner"))
     def deactivate_owners(self, request, queryset):
         queryset.update(is_active=False)
         self.message_user(request, f"Deactivated {queryset.count()} owners")
 
-    @admin.display(description="Update all from EVE server for selected owners")
+    @admin.display(description=_("Update all from EVE server for selected owners"))
     def update_all(self, request, queryset):
         for obj in queryset:
             tasks.update_all_for_owner.delay(obj.pk, user_pk=request.user.pk)
-            text = (
-                f"Started updating structures and notifications for {obj}. "
-                "You will receive a notification once it is completed."
+            text = _(
+                "Started updating structures and notifications for %s. "
+                "You will receive a notification once it is completed." % obj
             )
             self.message_user(request, text)
 
-    @admin.display(description="Update structures from EVE server for selected owners")
+    @admin.display(
+        description=_("Update structures from EVE server for selected owners")
+    )
     def update_structures(self, request, queryset):
         for obj in queryset:
             tasks.update_structures_for_owner.delay(obj.pk, user_pk=request.user.pk)
             text = (
                 f"Started updating structures for {obj}. "
                 "You will receive a notification once it is completed."
             )
             self.message_user(request, text)
 
     @admin.display(
-        description="Fetch notifications from EVE server for selected owners"
+        description=_("Fetch notifications from EVE server for selected owners")
     )
     def fetch_notifications(self, request, queryset):
         for obj in queryset:
             tasks.process_notifications_for_owner.delay(obj.pk, user_pk=request.user.pk)
             text = (
                 f"Started fetching notifications for {obj}. "
                 "You will receive a notification once it is completed."
@@ -622,18 +628,18 @@
     list_filter = (
         "is_default",
         "style",
         "is_user_managed",
     )
     readonly_fields = ("is_user_managed",)
 
-    def has_delete_permission(self, request, obj=None):
+    def has_delete_permission(self, request, obj: Optional[StructureTag] = None):
         return False if obj and not obj.is_user_managed else True
 
-    def has_change_permission(self, request, obj=None):
+    def has_change_permission(self, request, obj: Optional[StructureTag] = None):
         return False if obj and not obj.is_user_managed else True
 
 
 class StructureServiceAdminInline(admin.TabularInline):
     model = StructureService
 
     def has_add_permission(self, request, obj=None):
@@ -878,15 +884,15 @@
     def _type(self, structure):
         return format_html("{}<br>{}", structure.eve_type, structure.eve_type.eve_group)
 
     def _power_mode(self, structure) -> str:
         return structure.get_power_mode_display()
 
     @admin.display(description="Tags")
-    def _tags(self, structure) -> str:
+    def _tags(self, structure) -> list:
         return sorted([tag.name for tag in structure.tags.all()])
 
     def _webhooks(self, obj):
         names = [webhook.name for webhook in obj.webhooks.all()]
         return lines_sorted_html(names) if names else None
 
     @admin.display(description="Add default tags to selected structures")
@@ -900,27 +906,27 @@
         self.message_user(
             request,
             "Added {:,} default tags to {:,} structures".format(
                 tags.count(), structure_count
             ),
         )
 
-    @admin.display(description="Remove user tags for selected structures")
+    @admin.display(description=_("Remove user tags for selected structures"))
     def remove_user_tags(self, request, queryset):
         structure_count = 0
         for structure in queryset:
             for tag in structure.tags.filter(is_user_managed=True):
                 structure.tags.remove(tag)
             structure_count += 1
         self.message_user(
             request,
             "Removed all user tags from {:,} structures".format(structure_count),
         )
 
-    @admin.display(description="Update generated tags for selected structures")
+    @admin.display(description=_("Update generated tags for selected structures"))
     def update_generated_tags(self, request, queryset):
         structure_count = 0
         for structure in queryset:
             structure.update_generated_tags(recreate_tags=True)
             structure_count += 1
         self.message_user(
             request,
@@ -980,16 +986,16 @@
                     "has_default_pings_enabled",
                     "webhook_type",
                 ),
             },
         ),
     )
 
-    def get_form(self, request, obj=None, **kwargs):
-        form = super().get_form(request, obj, **kwargs)
+    def get_form(self, *args, **kwargs):
+        form = super().get_form(*args, **kwargs)
         form.base_fields[
             "notification_types"
         ].choices = NotificationType.choices_enabled
         return form
 
     def get_queryset(self, request):
         qs = super().get_queryset(request)
@@ -1021,67 +1027,66 @@
     def _owners(self, obj):
         configurations = [str(owner) for owner in obj.owners.all()]
         configurations += [
             f"{structure.owner}: {structure}" for structure in obj.structures.all()
         ]
         if not configurations:
             return format_html(
-                '<b><span style="color: orange;">'
-                "⚠ Please add this webhook to an owner or structure to enable it."
-                "</span></b>"
+                '<b><span style="color: orange;">⚠ {}</span></b>',
+                _("Please add this webhook to an owner or structure to enable it."),
             )
         return lines_sorted_html(configurations)
 
     def _is_default(self, obj):
         value = True if obj.is_default else None
         return admin_boolean_icon_html(value)
 
     def _messages_in_queue(self, obj):
         return obj.queue_size()
 
-    @admin.display(description="Send test notification to selected webhook")
+    @admin.display(description=_("Send test notification to selected webhook"))
     def test_notification(self, request, queryset):
         for obj in queryset:
             tasks.send_test_notifications_to_webhook.delay(
                 obj.pk, user_pk=request.user.pk
             )
             self.message_user(
                 request,
                 'Initiated sending test notification to webhook "{}". '
                 "You will receive a report on completion.".format(obj),
             )
 
-    @admin.display(description="Activate selected webhook")
+    @admin.display(description=_("Activate selected webhook"))
     def activate(self, request, queryset):
         for obj in queryset:
             obj.is_active = True
             obj.save()
             self.message_user(request, f'You have activated webhook "{obj}"')
 
-    @admin.display(description="Deactivate selected webhook")
+    @admin.display(description=_("Deactivate selected webhook"))
     def deactivate(self, request, queryset):
         for obj in queryset:
             obj.is_active = False
             obj.save()
             self.message_user(request, f'You have de-activated webhook "{obj}"')
 
-    @admin.display(description="Purge queued messages from selected webhooks")
+    @admin.display(description=_("Purge queued messages from selected webhooks"))
     def purge_messages(self, request, queryset):
         actions_count = 0
         killmails_deleted = 0
         for webhook in queryset:
             killmails_deleted += webhook.clear_queue()
             actions_count += 1
         self.message_user(
             request,
             f"Purged queued messages for {actions_count} webhooks, "
             f"deleting a total of {killmails_deleted} messages.",
         )
 
-    @admin.display(description="Send queued messages from selected webhooks")
+    @admin.display(description=_("Send queued messages from selected webhooks"))
     def send_messages(self, request, queryset):
         items_count = 0
         for webhook in queryset:
             tasks.send_messages_for_webhook.delay(webhook.pk)
             items_count += 1
 
         self.message_user(
```

### Comparing `aa-structures-2.1.0/structures/app_settings.py` & `aa_structures-2.2.0/structures/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/auth_hooks.py` & `aa_structures-2.2.0/structures/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/constants.py` & `aa_structures-2.2.0/structures/constants.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/core/notification_embeds.py` & `aa_structures-2.2.0/structures/core/notification_embeds.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/core/notification_timers.py` & `aa_structures-2.2.0/structures/core/notification_timers.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/core/serializers.py` & `aa_structures-2.2.0/structures/core/serializers.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/core/sovereignty.py` & `aa_structures-2.2.0/structures/core/sovereignty.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/core/starbases.py` & `aa_structures-2.2.0/structures/core/starbases.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/locale/de/LC_MESSAGES/django.mo` & `aa_structures-2.2.0/structures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/locale/es/LC_MESSAGES/django.mo` & `aa_structures-2.2.0/structures/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/locale/ru/LC_MESSAGES/django.mo` & `aa_structures-2.2.0/structures/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_structures-2.2.0/structures/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/management/commands/structures_load_eve.py` & `aa_structures-2.2.0/structures/management/commands/structures_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/management/commands/structures_preload_eveuniverse.py` & `aa_structures-2.2.0/structures/management/commands/structures_preload_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/managers.py` & `aa_structures-2.2.0/structures/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime as dt
 import itertools
-from typing import Tuple
+from typing import Optional, Set, Tuple
 
 from django.contrib.auth.models import User
 from django.db import models, transaction
 from django.db.models import Case, Count, Exists, OuterRef, Q, Value, When
 from django.utils.timezone import now
 from esi.models import Token
 from eveuniverse.models import EveMoon, EvePlanet, EveSolarSystem, EveType
@@ -55,24 +55,26 @@
     def corporation_has_sov(
         self, eve_solar_system: models.Model, corporation: EveCorporationInfo
     ) -> bool:
         """returns true if given corporation has sov in this solar system
         else False
         """
         if not eve_solar_system.is_null_sec:
-            return None
+            return False
         else:
             alliance_id = (
                 int(corporation.alliance.alliance_id) if corporation.alliance else None
             )
-            return alliance_id and (
+            return bool(alliance_id) and (
                 self.solar_system_sov_alliance_id(eve_solar_system) == alliance_id
             )
 
-    def solar_system_sov_alliance_id(self, eve_solar_system: models.Model) -> int:
+    def solar_system_sov_alliance_id(
+        self, eve_solar_system: models.Model
+    ) -> Optional[int]:
         """returns ID of sov owning alliance for this system or None"""
         if not eve_solar_system.is_null_sec:
             return None
         try:
             sov_map = self.get(solar_system_id=eve_solar_system.id)
             return sov_map.alliance_id if sov_map.alliance_id else None
         except self.model.DoesNotExist:
@@ -182,26 +184,20 @@
             x_characters_count=Count(
                 "characters",
                 filter=Q(characters__character_ownership__isnull=False),
                 distinct=True,
             )
         )
 
-    def structures_last_updated(self):
+    def structures_last_updated(self) -> Optional[dt.datetime]:
         """Date/time when structures were last updated for any of the active owners."""
-        active_owners = self.filter(is_active=True)
-        return (
-            (
-                active_owners.order_by("-structures_last_update_at")
-                .first()
-                .structures_last_update_at
-            )
-            if active_owners
-            else None
-        )
+        obj = self.filter(is_active=True).order_by("-structures_last_update_at").first()
+        if not obj:
+            return None
+        return obj.structures_last_update_at
 
 
 class OwnerManagerBase(models.Manager):
     pass
 
 
 OwnerManager = OwnerManagerBase.from_queryset(OwnerQuerySet)
@@ -213,15 +209,15 @@
 
     def filter_customs_offices(self) -> models.QuerySet:
         return self.filter(eve_type=EveTypeId.CUSTOMS_OFFICE)
 
     def filter_starbases(self) -> models.QuerySet:
         return self.filter(eve_type__eve_group__eve_category=EveCategoryId.STARBASE)
 
-    def ids(self) -> set():
+    def ids(self) -> Set[int]:
         """Return ids as set."""
         return set(self.values_list("id", flat=True))
 
     def select_related_defaults(self) -> models.QuerySet:
         """returns a QuerySet with the default select_related"""
         return self.select_related(
             "owner",
@@ -449,15 +445,15 @@
         return obj, created
 
 
 StructureManager = StructureManagerBase.from_queryset(StructureQuerySet)
 
 
 class StructureTagManager(models.Manager):
-    def get_or_create_for_space_type(self, solar_system: models.Model) -> tuple:
+    def get_or_create_for_space_type(self, solar_system) -> tuple:
         from .models import EveSpaceType
 
         space_type = EveSpaceType.from_solar_system(solar_system)
         params = self.model.SPACE_TYPE_MAP.get(space_type)
         if params:
             try:
                 obj = self.get(name=params["name"])
@@ -505,13 +501,13 @@
                 "is_user_managed": False,
                 "is_default": False,
             },
         )
 
 
 class WebhookManager(WebhookBaseManager):
-    def enabled_notification_types(self) -> set:
+    def enabled_notification_types(self) -> Set[str]:
         """Set of all currently enabled notification types."""
         notif_types_list = list(
             self.filter(is_active=True).values_list("notification_types", flat=True)
         )
         return set(itertools.chain(*notif_types_list))
```

### Comparing `aa-structures-2.1.0/structures/migrations/0001_initial_new.py` & `aa_structures-2.2.0/structures/migrations/0001_initial_new.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,63 +7,14 @@
 import django.utils.timezone
 from django.db import migrations, models
 
 import structures.webhooks.core
 
 
 class Migration(migrations.Migration):
-
-    replaces = [
-        ("structures", "0001_initial"),
-        ("structures", "0002_auto_20191121_2335"),
-        ("structures", "0003_auto_20191125_2157"),
-        ("structures", "0004_auto_20191129_0308"),
-        ("structures", "0005_notification_created"),
-        ("structures", "0006_auto_20200120_0147"),
-        ("structures", "0007_auto_20200123_1429"),
-        ("structures", "0008_auto_20200209_1638"),
-        ("structures", "0009_localizations"),
-        ("structures", "0010_sovereignty_map"),
-        ("structures", "0011_last_online"),
-        ("structures", "0012_disable_pings"),
-        ("structures", "0013_group_pings"),
-        ("structures", "0014_addtl_perm_unanchor"),
-        ("structures", "0015_refactor_notification_types"),
-        ("structures", "0016_char_join_leave_notifications"),
-        ("structures", "0017_war_dec_notifications"),
-        ("structures", "0018_restructure_notifications_2"),
-        ("structures", "0019_more_notification_types"),
-        ("structures", "0020_more_war_notifications"),
-        ("structures", "0021_add_corporation_permission"),
-        ("structures", "0022_add_corp_app_notification_types"),
-        ("structures", "0023_structure_fittings"),
-        ("structures", "0024_fix_name_fields_too_small"),
-        ("structures", "0025_add_poco_details"),
-        ("structures", "0026_rework_update_status"),
-        ("structures", "0027_create_owner_characters"),
-        ("structures", "0028_migrate_owner_characters"),
-        ("structures", "0029_custom_fuel_notifications"),
-        ("structures", "0030_update_refueled_notifications"),
-        ("structures", "0031_add_service_up"),
-        ("structures", "0032_add_jump_fuel_alerts"),
-        ("structures", "0033_fix_notification_type_fuel_alert"),
-        ("structures", "0034_add_structure_webhooks"),
-        ("structures", "0035_add_more_notifications_types"),
-        ("structures", "0036_django4_update"),
-        ("structures", "0037_add_billing_notification_types"),
-        ("structures", "0038_add_starbase_detail"),
-        ("structures", "0039_ownercharacter_error_count"),
-        ("structures", "0040_add_generated_notifications"),
-        ("structures", "0041_notification_sender_can_be_null"),
-        ("structures", "0042_migrate_sender_category_other"),
-        ("structures", "0043_remove_services_localization"),
-        ("structures", "0044_check_eveuniverse_fully_loaded"),
-        ("structures", "0045_migrate_all_to_django_eveuniverse"),
-    ]
-
     initial = True
 
     dependencies = [
         ("eveonline", "0015_factions"),
         ("authentication", "0019_merge_20211026_0919"),
         ("auth", "0012_alter_user_first_name_max_length"),
         ("eveuniverse", "0007_evetype_description"),
```

### Comparing `aa-structures-2.1.0/structures/migrations/0002_remove_eveuniverse_relation_names.py` & `aa_structures-2.2.0/structures/migrations/0002_remove_eveuniverse_relation_names.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 4.0.7 on 2022-09-16 12:31
 
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("eveuniverse", "0007_evetype_description"),
         ("structures", "0001_initial_new"),
     ]
 
     operations = [
         migrations.AlterField(
```

### Comparing `aa-structures-2.1.0/structures/models/eveuniverse.py` & `aa_structures-2.2.0/structures/models/eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/models/notifications.py` & `aa_structures-2.2.0/structures/models/notifications.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""Notification related models"""
+"""Notification related models."""
 
 import math
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 
 import dhooks_lite
 import yaml
 from multiselectfield import MultiSelectField
 from requests.exceptions import HTTPError
 
 from django.contrib.auth.models import Group
 from django.core.exceptions import ValidationError
 from django.db import models
 from django.db.models import Q
 from django.utils import translation
-from django.utils.functional import classproperty
+from django.utils.functional import classproperty  # type: ignore
 from django.utils.timezone import now
 from django.utils.translation import gettext_lazy as _
 from eveuniverse.models import EveEntity
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.django import app_labels
 from app_utils.logging import LoggerAddTag
@@ -92,25 +92,25 @@
     TOWER_ALERT_MSG = "TowerAlertMsg", _("Starbase attacked")
     TOWER_RESOURCE_ALERT_MSG = "TowerResourceAlertMsg", _("Starbase fuel alert")
     TOWER_REFUELED_EXTRA = "TowerRefueledExtra", _("Starbase refueled (BETA)")
     TOWER_REINFORCED_EXTRA = "TowerReinforcedExtra", _("Starbase reinforced (BETA)")
 
     # moon mining
     MOONMINING_EXTRACTION_STARTED = "MoonminingExtractionStarted", _(
-        "Moonmining extraction started"
+        "Moon mining extraction started"
     )
     MOONMINING_LASER_FIRED = "MoonminingLaserFired", _("Moonmining laser fired")
     MOONMINING_EXTRACTION_CANCELLED = "MoonminingExtractionCancelled", _(
-        "Moonmining extraction cancelled"
+        "Moon mining extraction cancelled"
     )
     MOONMINING_EXTRACTION_FINISHED = "MoonminingExtractionFinished", _(
-        "Moonmining extraction finished"
+        "Moon mining extraction finished"
     )
     MOONMINING_AUTOMATIC_FRACTURE = "MoonminingAutomaticFracture", _(
-        "Moonmining automatic fracture triggered"
+        "Moon mining automatic fracture triggered"
     )
 
     # sov
     SOV_STRUCTURE_REINFORCED = "SovStructureReinforced", _(
         "Sovereignty structure reinforced"
     )
     SOV_STRUCTURE_DESTROYED = "SovStructureDestroyed", _(
@@ -329,81 +329,94 @@
 
 class Webhook(WebhookBase):
     """A destination for forwarding notification alerts."""
 
     notification_types = MultiSelectField(
         choices=NotificationType.choices,
         default=NotificationType.webhook_defaults,
-        help_text=(
-            "select which type of notifications should be forwarded to this webhook"
+        verbose_name=_("notification types"),
+        help_text=_(
+            "Select which type of notifications should be forwarded to this webhook"
         ),
     )
     language_code = models.CharField(
         max_length=8,
         choices=LANGUAGES,
         default=None,
         null=True,
         blank=True,
-        verbose_name="language",
-        help_text="language of notifications send to this webhook",
+        verbose_name=_("language"),
+        help_text=_("language of notifications send to this webhook"),
     )
     is_default = models.BooleanField(
         default=False,
-        help_text=(
-            "whether owners have this webhook automatically pre-set when created"
+        verbose_name=_("is default"),
+        help_text=_(
+            "Whether owners have this webhook automatically pre-set when created"
         ),
     )
     has_default_pings_enabled = models.BooleanField(
         default=True,
+        verbose_name=_("has default pings enabled"),
         help_text=(
-            "to enable or disable pinging of notifications for this webhook "
+            "To enable or disable pinging of notifications for this webhook "
             "e.g. with @everyone and @here"
         ),
     )
     ping_groups = models.ManyToManyField(
         Group,
         default=None,
         blank=True,
         related_name="+",
-        help_text="Groups to be pinged for each notification - ",
+        verbose_name=_("ping groups"),
+        help_text=_("Groups to be pinged for each notification - "),
     )
     objects = WebhookManager()
 
+    class Meta:
+        verbose_name = _("webhook")
+        verbose_name_plural = _("webhooks")
+
     @staticmethod
     def text_bold(text) -> str:
         """Format the given text in bold."""
         return f"**{text}**" if text else ""
 
 
 class NotificationBase(models.Model):
     """Base model for a notification."""
 
     is_sent = models.BooleanField(
         default=False,
-        help_text="True when this notification has been forwarded to Discord",
+        verbose_name=_("is sent"),
+        help_text=_("True when this notification has been forwarded to Discord"),
     )
     is_timer_added = models.BooleanField(
         null=True,
         default=False,
-        help_text="True when a timer has been added for this notification",
+        verbose_name=_("is timer added"),
+        help_text=_("True when a timer has been added for this notification"),
     )
     notif_type = models.CharField(
         max_length=100,
         default="",
         db_index=True,
-        verbose_name="type",
-        help_text="type of this notification",
+        verbose_name=_("type"),
+        help_text=_("type of this notification"),
     )
     owner = models.ForeignKey(
         "Owner",
         on_delete=models.CASCADE,
-        help_text="Corporation that owns this notification",
+        verbose_name=_("owner"),
+        help_text=_("Corporation that owns this notification"),
     )
     structures = models.ManyToManyField(
-        Structure, help_text="Structures this notification is about (if any)"
+        Structure,
+        verbose_name=_("structures"),
+        help_text=_("Structures this notification is about (if any)"),
     )
 
     class Meta:
         abstract = True
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
@@ -437,19 +450,29 @@
         return self.notif_type in NotificationType.relevant_for_timerboard
 
     @property
     def is_structure_related(self) -> bool:
         """Weather this notification related to a structure."""
         return self.notif_type in NotificationType.structure_related
 
+    @property
+    def is_temporary(self) -> bool:
+        raise NotImplementedError()
+
+    def is_npc_attacking(self) -> bool:
+        raise NotImplementedError()
+
+    def parsed_text(self) -> dict:
+        raise NotImplementedError()
+
     def send_to_configured_webhooks(
         self,
-        ping_type_override: Webhook.PingType = None,
+        ping_type_override: Optional[Union[Webhook.PingType, str]] = None,
         use_color_override: bool = False,
-        color_override: int = None,
+        color_override: Optional[int] = None,
     ) -> Optional[bool]:
         """Send this notification to all active webhooks which have this
         notification type configured
         and apply filter for NPC attacks and alliance level if needed.
 
         Returns True, if notifications has been successfully send to webhooks
         Returns None, if owner has no fitting webhook
@@ -464,15 +487,15 @@
             )
             return None
         webhooks_qs = self.relevant_webhooks()
         if not webhooks_qs.exists():
             logger.debug("%s: No relevant webhook found", self)
             return None
         if ping_type_override:
-            self._ping_type_override = ping_type_override
+            self._ping_type_override = Webhook.PingType(ping_type_override)
         if use_color_override:
             self._color_override = color_override
         success = True
         for webhook in webhooks_qs:
             success &= self.send_to_webhook(webhook)
         return success
 
@@ -603,15 +626,15 @@
         success = new_queue_size > 0
         if success and not self.is_temporary:
             self.is_sent = True
             self.save()
         return success
 
     def _generate_embed(
-        self, language_code: str
+        self, language_code: Optional[str]
     ) -> Tuple[dhooks_lite.Embed, Webhook.PingType]:
         """Generates a Discord embed for this notification."""
         from ..core.notification_embeds import NotificationBaseEmbed
 
         logger.info("Creating embed with language = %s" % language_code)
         with translation.override(language_code):
             notification_embed = NotificationBaseEmbed.create(self)
@@ -620,15 +643,15 @@
 
     @staticmethod
     def _import_discord() -> object:
         from allianceauth.services.modules.discord.models import DiscordUser
 
         return DiscordUser
 
-    def _gen_avatar(self) -> Tuple[str, str]:
+    def _gen_avatar(self) -> Tuple[Optional[str], Optional[str]]:
         if STRUCTURES_NOTIFICATION_SET_AVATAR:
             username = "Notifications"
             avatar_url = static_file_absolute_url("structures/img/structures_logo.png")
         else:
             username = None
             avatar_url = None
         return username, avatar_url
@@ -644,64 +667,73 @@
         ):
             return False
 
         from ..core import notification_timers
 
         try:
             with translation.override(STRUCTURES_DEFAULT_LANGUAGE):
-                timer_processed = notification_timers.add_or_remove_timer(self)
+                return notification_timers.add_or_remove_timer(self)
         except OSError as ex:
             logger.warning(
                 "%s: Failed to add timer from notification: %s",
                 self,
                 ex,
                 exc_info=True,
             )
-        return timer_processed
+        return False
 
 
 class Notification(NotificationBase):
     """A notification in Eve Online.
 
     Notifications are usually created from Eve Online notifications received from ESI,
     but they can also be generated directly by Structures.
     """
 
     TEMPORARY_NOTIFICATION_ID = 999999999999
 
-    notification_id = models.PositiveBigIntegerField(verbose_name="id")
+    notification_id = models.PositiveBigIntegerField(verbose_name=_("id"))
     created = models.DateTimeField(
         null=True,
         default=None,
-        help_text="Date when this notification was first received from ESI",
+        verbose_name=_("created"),
+        help_text=_("Date when this notification was first received from ESI"),
     )
     is_read = models.BooleanField(
         null=True,
         default=None,
-        help_text="True when this notification has read in the eve client",
+        verbose_name=_("is read"),
+        help_text=_("True when this notification has read in the eve client"),
     )
     last_updated = models.DateTimeField(
-        help_text="Date when this notification has last been updated from ESI"
+        verbose_name=_("last updated"),
+        help_text=_("Date when this notification has last been updated from ESI"),
     )
     sender = models.ForeignKey(
         EveEntity,
         on_delete=models.SET_NULL,
         null=True,
         related_name="+",
+        verbose_name=_("sender"),
     )
 
     text = models.TextField(
-        null=True, default=None, blank=True, help_text="Notification details in YAML"
+        null=True,
+        default=None,
+        blank=True,
+        verbose_name=_("text"),
+        help_text=_("Notification details in YAML"),
     )
-    timestamp = models.DateTimeField(db_index=True)
+    timestamp = models.DateTimeField(db_index=True, verbose_name=_("timestamp"))
 
     objects = NotificationManager()
 
     class Meta:
-        verbose_name = "eve notification"
+        verbose_name = _("eve notification")
+        verbose_name_plural = _("eve notifications")
         unique_together = (("notification_id", "owner"),)
 
     def save(self, *args, **kwargs) -> None:
         if self.is_temporary:
             raise ValueError("Temporary notifications can not be saved")
         super().save(*args, **kwargs)
 
@@ -717,15 +749,15 @@
     # @classmethod
     # def get_all_types(cls) -> Set[int]:
     #     """returns a set with all supported notification types"""
     #     return {x[0] for x in NotificationType.choices}
 
     def parsed_text(self) -> dict:
         """Returns the notifications's text as dict."""
-        return yaml.safe_load(self.text)
+        return yaml.safe_load(self.text) if self.text else {}
 
     def is_npc_attacking(self) -> bool:
         """Whether this notification is about a NPC attacking."""
         if self.notif_type in [
             NotificationType.ORBITAL_ATTACKED,
             NotificationType.STRUCTURE_UNDER_ATTACK,
         ]:
@@ -802,20 +834,24 @@
         kwargs["notif_type"] = notif_type
         return cls(**kwargs)
 
 
 class GeneratedNotification(NotificationBase):
     """A notification generated by the Structures app, not by Eve Online."""
 
-    details = models.JSONField(default=dict)
-    last_updated = models.DateTimeField(auto_now=True)
-    timestamp = models.DateTimeField(auto_now_add=True)
+    details = models.JSONField(default=dict, verbose_name=_("details"))
+    last_updated = models.DateTimeField(auto_now=True, verbose_name=_("last_updated"))
+    timestamp = models.DateTimeField(auto_now_add=True, verbose_name=_("timestamp"))
 
     objects = GeneratedNotificationManager()
 
+    class Meta:
+        verbose_name = _("generated notification")
+        verbose_name_plural = _("generated  notifications")
+
     @property
     def notification_id(self) -> int:
         return self.pk
 
     @property
     def is_temporary(self) -> bool:
         return False
@@ -835,31 +871,33 @@
 class BaseFuelAlertConfig(models.Model):
     """Configuration of structure fuel notifications."""
 
     channel_ping_type = models.CharField(
         max_length=2,
         choices=Webhook.PingType.choices,
         default=Webhook.PingType.HERE,
-        verbose_name="channel pings",
-        help_text=(
+        verbose_name=_("channel pings"),
+        help_text=_(
             "Option to ping every member of the channel. "
             "This setting can be overruled by the respective owner "
             "or webhook configuration"
         ),
     )
     color = models.IntegerField(
         choices=Webhook.Color.choices,
         default=Webhook.Color.WARNING,
         blank=True,
         null=True,
-        help_text="Context color of these notification on Discord",
+        verbose_name=_("color"),
+        help_text=_("Context color of these notification on Discord"),
     )
     is_enabled = models.BooleanField(
         default=True,
-        help_text="Disabled configurations will not create any new alerts.",
+        verbose_name=_("is_enabled"),
+        help_text=_("Disabled configurations will not create any new alerts."),
     )
 
     class Meta:
         abstract = True
 
     def __str__(self) -> str:
         return f"#{self.pk}"
@@ -874,29 +912,34 @@
         raise NotImplementedError()
 
 
 class FuelAlertConfig(BaseFuelAlertConfig):
     """Configuration of structure fuel notifications."""
 
     end = models.PositiveIntegerField(
-        help_text="End of alerts in hours before fuel expires"
+        verbose_name=_("end"), help_text=_("End of alerts in hours before fuel expires")
     )
     repeat = models.PositiveIntegerField(
-        help_text=(
+        verbose_name=_("repeat"),
+        help_text=_(
             "Notifications will be repeated every x hours. Set to 0 for no repeats"
-        )
+        ),
     )
     start = models.PositiveIntegerField(
-        help_text="Start of alerts in hours before fuel expires"
+        verbose_name=_("start"),
+        help_text=_("Start of alerts in hours before fuel expires"),
     )
 
     class Meta:
-        verbose_name = "structure fuel alert config"
+        verbose_name = _("structure fuel alert config")
+        verbose_name_plural = _("structure fuel alert configs")
 
     def clean(self) -> None:
+        if self.start is None or self.end is None or self.repeat is None:  # Fixes #83
+            return  # these will be caught by the form validation later
         if self.start <= self.end:
             raise ValidationError(
                 _("Start must be before end, i.e. have a larger value.")
             )
         if self.repeat >= self.start - self.end:
             raise ValidationError(
                 {"repeat": _("Repeat can not be larger that the interval size.")}
@@ -971,19 +1014,24 @@
         )
 
 
 class JumpFuelAlertConfig(BaseFuelAlertConfig):
     """Configuration of jump fuel notifications."""
 
     threshold = models.PositiveIntegerField(
-        help_text=(
+        verbose_name=_("threshold"),
+        help_text=_(
             "Notifications will be sent once fuel level in units reaches this threshold"
-        )
+        ),
     )
 
+    class Meta:
+        verbose_name = _("jump fuel alert config")
+        verbose_name_plural = _("jump fuel alert configs")
+
     def save(self, *args, **kwargs) -> None:
         try:
             old_instance = JumpFuelAlertConfig.objects.get(pk=self.pk)
         except JumpFuelAlertConfig.DoesNotExist:
             old_instance = None
         super().save(*args, **kwargs)
         if old_instance and (old_instance.threshold != self.threshold):
@@ -1020,28 +1068,34 @@
         raise NotImplementedError()
 
 
 class FuelAlert(BaseFuelAlert):
     """A generated notification alerting about fuel getting low in structures."""
 
     structure = models.ForeignKey(
-        Structure, on_delete=models.CASCADE, related_name="structure_fuel_alerts"
+        Structure,
+        on_delete=models.CASCADE,
+        related_name="structure_fuel_alerts",
+        verbose_name=_("structure"),
     )
     config = models.ForeignKey(
         FuelAlertConfig,
         on_delete=models.CASCADE,
         related_name="structure_fuel_alerts",
+        verbose_name=_("configuration"),
     )
     hours = models.PositiveIntegerField(
         db_index=True,
-        help_text="number of hours before fuel expiration this alert was sent",
+        verbose_name=_("hours"),
+        help_text=_("number of hours before fuel expiration this alert was sent"),
     )
 
     class Meta:
-        verbose_name = "structure fuel alert"
+        verbose_name = _("structure fuel alert")
+        verbose_name_plural = _("structure fuel alerts")
         constraints = [
             models.UniqueConstraint(
                 fields=["structure", "config", "hours"],
                 name="functional_pk_fuelalert",
             )
         ]
 
@@ -1064,20 +1118,30 @@
         )
 
 
 class JumpFuelAlert(BaseFuelAlert):
     """A generated notification alerting about jump fuel getting low."""
 
     structure = models.ForeignKey(
-        Structure, on_delete=models.CASCADE, related_name="jump_fuel_alerts"
+        Structure,
+        on_delete=models.CASCADE,
+        related_name="jump_fuel_alerts",
+        verbose_name=_("structure"),
     )
     config = models.ForeignKey(
-        JumpFuelAlertConfig, on_delete=models.CASCADE, related_name="jump_fuel_alerts"
+        JumpFuelAlertConfig,
+        on_delete=models.CASCADE,
+        related_name="jump_fuel_alerts",
+        verbose_name=_("configuration"),
     )
 
+    class Meta:
+        verbose_name = _("jump fuel alert")
+        verbose_name_plural = _("jump fuel alerts")
+
     def __str__(self) -> str:
         return f"{self.structure}-{self.config}"
 
     def send_generated_notification(self) -> None:
         notif = Notification.create_from_structure(
             structure=self.structure,
             notif_type=NotificationType.STRUCTURE_JUMP_FUEL_ALERT,
```

### Comparing `aa-structures-2.1.0/structures/models/owners.py` & `aa_structures-2.2.0/structures/models/owners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-"""Owner related models"""
+"""Owner related models."""
+
 import datetime as dt
 import json
 import os
 import re
 from email.utils import format_datetime, parsedate_to_datetime
-from typing import Optional
+from typing import Any, Iterable, List, Optional
 
 from bravado.exception import HTTPForbidden, HTTPNotFound
 
 from django.contrib.auth.models import Group, User
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models, transaction
@@ -111,102 +112,119 @@
 
     # PK
     corporation = models.OneToOneField(
         EveCorporationInfo,
         primary_key=True,
         on_delete=models.CASCADE,
         related_name="structure_owner",
-        help_text="Corporation owning structures",
+        verbose_name=_("corporation"),
+        help_text=_("Corporation owning structures"),
     )
     # regular
     are_pocos_public = models.BooleanField(
         default=False,
-        help_text=("whether pocos of this owner are shown on public POCO page"),
+        verbose_name=_("are pocos public"),
+        help_text=_("whether pocos of this owner are shown on public POCO page"),
     )
     assets_last_update_at = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text="when the last successful update happened",
+        verbose_name=_("assets last update at"),
+        help_text=_("when the last successful update happened"),
     )
     character_ownership = models.ForeignKey(
         CharacterOwnership,
         on_delete=models.SET_DEFAULT,
         default=None,
         null=True,
         blank=True,
         related_name="+",
-        help_text="OUTDATED. Has been replaced by OwnerCharacter",
+        help_text="OUTDATED. Has been replaced by OwnerCharacter",  # TODO: Remove
     )
     forwarding_last_update_at = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text="when the last successful update happened",
+        verbose_name=_("forwarding last update at"),
+        help_text=_("when the last successful update happened"),
     )
     has_default_pings_enabled = models.BooleanField(
         default=True,
-        help_text=(
+        verbose_name=_("has default pings enabled"),
+        help_text=_(
             "to enable or disable pinging of notifications for this owner "
             "e.g. with @everyone and @here"
         ),
     )
     is_active = models.BooleanField(
         default=True,
-        help_text=("whether this owner is currently included in the sync process"),
+        verbose_name=_("is active"),
+        help_text=_("whether this owner is currently included in the sync process"),
     )
     is_alliance_main = models.BooleanField(
         default=False,
-        help_text=(
+        verbose_name=_("is alliance main"),
+        help_text=_(
             "whether alliance wide notifications "
             "are forwarded for this owner (e.g. sov notifications)"
         ),
     )
     is_included_in_service_status = models.BooleanField(
         default=True,
-        help_text=(
+        verbose_name=_("is included in service status"),
+        help_text=_(
             "whether the sync status of this owner is included in "
             "the overall status of this services"
         ),
     )
     is_up = models.BooleanField(
         null=True,
         default=None,
         editable=False,
-        help_text="whether all services for this owner are currently up",
+        verbose_name=_("is up"),
+        help_text=_("whether all services for this owner are currently up"),
     )
     notifications_last_update_at = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text="when the last successful update happened",
+        verbose_name=_("notifications last update at"),
+        help_text=_("when the last successful update happened"),
     )
     ping_groups = models.ManyToManyField(
         Group,
         default=None,
         blank=True,
         related_name="+",
-        help_text="Groups to be pinged for each notification. ",
+        verbose_name=_("ping groups"),
+        help_text=_("Groups to be pinged for each notification. "),
     )
     structures_last_update_at = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text="when the last successful update happened",
+        verbose_name=_("structures last update at"),
+        help_text=_("when the last successful update happened"),
     )
     webhooks = models.ManyToManyField(
         "Webhook",
         default=None,
         blank=True,
         related_name="owners",
-        help_text="Notifications are sent to these webhooks. ",
+        verbose_name=_("webhooks"),
+        help_text=_("Notifications are sent to these webhooks."),
     )
 
     objects = OwnerManager()
 
+    class Meta:
+        verbose_name = _("owner")
+        verbose_name_plural = _("owners")
+
     def __str__(self) -> str:
         return str(self.corporation.corporation_name)
 
     def __repr__(self):
         return "{}(pk={}, corporation='{}')".format(
             self.__class__.__name__, self.pk, self.corporation
         )
@@ -221,38 +239,42 @@
             if "update_fields" in kwargs:
                 kwargs["update_fields"].append("is_alliance_main")
         super().save(*args, **kwargs)
 
     @property
     def is_structure_sync_fresh(self) -> bool:
         """True if last sync happened with grace time, else False."""
-        return self.structures_last_update_at and self.structures_last_update_at > (
+        return bool(
+            self.structures_last_update_at
+        ) and self.structures_last_update_at > (
             now() - dt.timedelta(minutes=STRUCTURES_STRUCTURE_SYNC_GRACE_MINUTES)
         )
 
     @property
     def is_notification_sync_fresh(self) -> bool:
         """True if last sync happened with grace time, else False."""
-        return (
+        return bool(
             self.notifications_last_update_at
-            and self.notifications_last_update_at
-            > (now() - dt.timedelta(minutes=STRUCTURES_NOTIFICATION_SYNC_GRACE_MINUTES))
+        ) and self.notifications_last_update_at > (
+            now() - dt.timedelta(minutes=STRUCTURES_NOTIFICATION_SYNC_GRACE_MINUTES)
         )
 
     @property
     def is_forwarding_sync_fresh(self) -> bool:
         """True if last sync happened with grace time, else False."""
-        return self.forwarding_last_update_at and self.forwarding_last_update_at > (
+        return bool(
+            self.forwarding_last_update_at
+        ) and self.forwarding_last_update_at > (
             now() - dt.timedelta(minutes=STRUCTURES_NOTIFICATION_SYNC_GRACE_MINUTES)
         )
 
     @property
     def is_assets_sync_fresh(self) -> bool:
         """True if last sync happened with grace time, else False."""
-        return self.assets_last_update_at and self.assets_last_update_at > (
+        return bool(self.assets_last_update_at) and self.assets_last_update_at > (
             now() - dt.timedelta(minutes=STRUCTURES_STRUCTURE_SYNC_GRACE_MINUTES)
         )
 
     @property
     def are_all_syncs_ok(self) -> bool:
         """returns true if they have been no errors
         and last syncing occurred within alloted time for all sync categories
@@ -410,27 +432,26 @@
             or time_since_last_used >= minimum_time_between_rotations
         ):
             setattr(character, rotate_characters.last_used_at_name, now())
             character.save()
 
     def fetch_token(
         self,
-        rotate_characters: RotateCharactersType = None,
+        rotate_characters: Optional[RotateCharactersType] = None,
         ignore_schedule: bool = False,
     ) -> Token:
         """Fetch a valid token for the owner and return it.
 
         Args:
             rotate_characters: For which sync type to rotate through characters \
                 with every new call
             ignore_schedule: Ignore current schedule when rotating
 
         Raises TokenError when no valid token can be provided.
         """
-        token = None
         order_by_last_used = (
             rotate_characters.last_used_at_name
             if rotate_characters
             else "notifications_last_used_at"
         )
         for character in self.characters.order_by(order_by_last_used):
             if (
@@ -453,36 +474,35 @@
             token = character.valid_token()
             if not token:
                 self.delete_character(
                     character=character,
                     error="Character has no valid token for sync.",
                 )
                 continue
+            found_character = character
             break  # leave the for loop if we have found a valid token
-
-        if not token:
-            error = (
+        else:
+            raise TokenError(
                 f"{self}: No valid character found for sync. "
                 "Service down for this owner."
             )
-            raise TokenError(error)
         if rotate_characters:
             self._rotate_character(
-                character=character,
+                character=found_character,
                 ignore_schedule=ignore_schedule,
                 rotate_characters=rotate_characters,
             )
         return token
 
     def _report_esi_issue(self, action: str, ex: Exception, token: Token):
         """Report an ESI issue to admins."""
         message = f"{self}: Failed to {action} from ESI with token {token} due to {ex}"
         logger.warning(message, exc_info=True)
 
-    def update_structures_esi(self, user: User = None):
+    def update_structures_esi(self, user: Optional[User] = None):
         """Updates all structures from ESI."""
         token = self.fetch_token(rotate_characters=self.RotateCharactersType.STRUCTURES)
         is_ok = self._fetch_upwell_structures(token)
         if STRUCTURES_FEATURE_CUSTOMS_OFFICES:
             is_ok &= self._fetch_custom_offices(token)
         if STRUCTURES_FEATURE_STARBASES:
             is_ok &= self._fetch_starbases(token)
@@ -492,34 +512,37 @@
             self.save(update_fields=["structures_last_update_at"])
             if user:
                 self._send_report_to_user(
                     topic="structures", topic_count=self.structures.count(), user=user
                 )
 
     def _remove_structures_not_returned_from_esi(
-        self, structures_qs: models.QuerySet, new_structures: list
+        self, structures_qs: models.QuerySet, new_structures: Iterable
     ):
         """Remove structures no longer returned from ESI."""
         ids_local = {x.id for x in structures_qs}
         ids_from_esi = {x["structure_id"] for x in new_structures}
         ids_to_remove = ids_local - ids_from_esi
         if len(ids_to_remove) > 0:
             structures_qs.filter(id__in=ids_to_remove).delete()
             logger.info(
                 "Removed %d structures which apparently no longer exist.",
                 len(ids_to_remove),
             )
 
-    def _fetch_locations_for_assets(self, item_ids: list, token: Token) -> dict:
+    def _fetch_locations_for_assets(
+        self, item_ids: Iterable[int], token: Token
+    ) -> dict:
         """Fetch locations for given asset items from ESI."""
+        item_ids = list(item_ids)
         logger.info(
             "%s: Fetching locations for %d assets from ESI", self, len(item_ids)
         )
         locations_data = list()
-        for item_ids_chunk in chunks(list(item_ids), 999):
+        for item_ids_chunk in chunks(item_ids, 999):
             try:
                 locations_data_chunk = (
                     esi.client.Assets.post_corporations_corporation_id_assets_locations(
                         corporation_id=self.corporation.corporation_id,
                         item_ids=item_ids_chunk,
                         token=token.valid_access_token(),
                     )
@@ -858,18 +881,19 @@
 
         self._remove_structures_not_returned_from_esi(
             structures_qs=self.structures.filter_starbases(),
             new_structures=structures,
         )
         return True
 
-    def _fetch_starbases_names(self, item_ids: list, token: Token) -> dict:
+    def _fetch_starbases_names(self, item_ids: Iterable, token: Token) -> dict:
+        item_ids = list(item_ids)
         logger.info("%s: Fetching names for %d starbases from ESI", self, len(item_ids))
         names_data = list()
-        for item_ids_chunk in chunks(list(item_ids), 999):
+        for item_ids_chunk in chunks(item_ids, 999):
             try:
                 names_data_chunk = (
                     esi.client.Assets.post_corporations_corporation_id_assets_names(
                         corporation_id=self.corporation.corporation_id,
                         item_ids=item_ids_chunk,
                         token=token.valid_access_token(),
                     )
@@ -932,15 +956,15 @@
         return detail
 
     def add_or_remove_timers_from_notifications(self):
         """Add/remove timers from esi and generated notification of this owner."""
         self.notification_set.add_or_remove_timers()
         self.generatednotification_set.add_or_remove_timers()
 
-    def fetch_notifications_esi(self, user: User = None) -> None:
+    def fetch_notifications_esi(self, user: Optional[User] = None) -> None:
         """Fetch notifications for this owner from ESI and process them."""
         notifications_count_all = 0
         token = self.fetch_token(
             rotate_characters=self.RotateCharactersType.NOTIFICATIONS
         )
         notifications = self._fetch_notifications_from_esi(token)
         notifications_count_new = self._store_notifications(notifications)
@@ -960,15 +984,15 @@
         if user:
             self._send_report_to_user(
                 topic="notifications",
                 topic_count=notifications_count_all,
                 user=user,
             )
 
-    def _fetch_notifications_from_esi(self, token: Token) -> dict:
+    def _fetch_notifications_from_esi(self, token: Token) -> List[dict]:
         """fetching all notifications from ESI for current owner"""
         notifications = esi.client.Character.get_characters_character_id_notifications(
             character_id=token.character_id, token=token.valid_access_token()
         ).results()
         if STRUCTURES_DEVELOPER_MODE:
             self._store_raw_data("notifications", notifications)
         if STRUCTURES_NOTIFICATIONS_ARCHIVING_ENABLED:
@@ -996,15 +1020,15 @@
                     now().strftime(DATETIME_FORMAT),
                     self.corporation.corporation_ticker,
                 )
             )
             json.dump(notifications, f, cls=DjangoJSONEncoder, sort_keys=True, indent=4)
             f.write("\n")
 
-    def _store_notifications(self, notifications: list) -> int:
+    def _store_notifications(self, notifications: List[dict]) -> int:
         """Store new notifications in database.
         Returns number of newly created objects.
         """
         # identify new notifications
         existing_notification_ids = set(
             self.notification_set.values_list("notification_id", flat=True)
         )
@@ -1070,15 +1094,15 @@
                     logger.info("%s: Updating moon for structure %s", self, refinery)
                     eve_moon, _ = EveMoon.objects.get_or_create_esi(
                         id=structure_id_2_moon_id[refinery.id]
                     )
                     refinery.eve_moon = eve_moon
                     refinery.save()
 
-    def send_new_notifications(self, user: User = None):
+    def send_new_notifications(self, user: Optional[User] = None):
         """Forward all new notification of this owner to configured webhooks."""
         notifications_count = 0
         cutoff_dt_for_stale = now() - dt.timedelta(
             hours=STRUCTURES_HOURS_UNTIL_STALE_NOTIFICATION
         )
         my_filter = {
             "notif_type__in": (
@@ -1136,22 +1160,22 @@
                 "owner": self.corporation.corporation_name,
                 "result": _("OK"),
             },
             message=message,
             level="success",
         )
 
-    def _store_raw_data(self, name: str, data: list):
+    def _store_raw_data(self, name: str, data: Any):
         """store raw data for debug purposes"""
         with open(
             f"{name}_raw_{self.corporation.corporation_id}.json", "w", encoding="utf-8"
         ) as f:
             json.dump(data, f, cls=DjangoJSONEncoder, sort_keys=True, indent=4)
 
-    def update_asset_esi(self, user: User = None):
+    def update_asset_esi(self, user: Optional[User] = None):
         token = self.fetch_token()
         assets_data = self._fetch_structure_assets_from_esi(token)
         self._store_items_for_upwell_structures(assets_data)
         self._store_items_for_starbases(assets_data)
         if user:
             self._send_report_to_user(
                 topic="assets", topic_count=self.structures.count(), user=user
@@ -1221,28 +1245,29 @@
             for item_id, item in assets_raw.items():
                 if (
                     item["location_id"] == structure.eve_solar_system_id
                     and item["location_type"] == "solar_system"
                     and item["location_flag"] == "AutoFit"
                     and item_id != structure.id
                     and item["position"]
+                    and structure.has_position
                     and structure.distance_to_object(
                         item["position"]["x"],
                         item["position"]["y"],
                         item["position"]["z"],
                     )
                     < 100_000
                 ):
                     structure_items.append(
                         StructureItem.from_esi_asset(item, structure)
                     )
             structure.update_items(structure_items)
 
-    @classmethod
-    def get_esi_scopes(cls) -> list:
+    @staticmethod
+    def get_esi_scopes() -> List[str]:
         scopes = [
             "esi-corporations.read_structures.v1",
             "esi-universe.read_structures.v1",
             "esi-characters.read_notifications.v1",
             "esi-assets.read_corporation_assets.v1",
         ]
         if STRUCTURES_FEATURE_CUSTOMS_OFFICES:
@@ -1252,44 +1277,53 @@
         return scopes
 
 
 class OwnerCharacter(models.Model):
     """Character for syncing owner data with ESI."""
 
     owner = models.ForeignKey(
-        Owner, on_delete=models.CASCADE, related_name="characters"
+        Owner,
+        on_delete=models.CASCADE,
+        related_name="characters",
+        verbose_name=_("owner"),
     )
     character_ownership = models.ForeignKey(
         CharacterOwnership,
         on_delete=models.CASCADE,
         related_name="+",
+        verbose_name=_("character_ownership"),
         help_text="character used for syncing",
     )
     structures_last_used_at = models.DateTimeField(
         null=True,
         default=None,
         editable=False,
         db_index=True,
+        verbose_name=_("structures last used at"),
         help_text="when this character was last used for syncing structures",
     )
     notifications_last_used_at = models.DateTimeField(
         null=True,
         default=None,
         editable=False,
         db_index=True,
+        verbose_name=_("notifications last used at"),
         help_text="when this character was last used for syncing notifications",
     )
     error_count = models.PositiveIntegerField(
         default=0,
         editable=False,
+        verbose_name=_("error count"),
         help_text="Count of ESI errors which happened with this character.",
     )
     created_at = models.DateTimeField(auto_now_add=True)
 
     class Meta:
+        verbose_name = _("owner character")
+        verbose_name_plural = _("owner characters")
         constraints = [
             models.UniqueConstraint(
                 fields=["owner", "character_ownership"], name="functional_pk_ownertoken"
             )
         ]
 
     def __str__(self) -> str:
```

### Comparing `aa-structures-2.1.0/structures/models/structures.py` & `aa_structures-2.2.0/structures/models/structures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Structure related models"""
+"""Structure related models."""
 
 import datetime as dt
 import math
 import re
 from typing import List, Optional
 
 from django.core.validators import MaxValueValidator, MinValueValidator
@@ -38,75 +38,88 @@
     NAME_SOV_TAG = gettext_noop("sov")
     NAME_HIGHSEC_TAG = gettext_noop("highsec")
     NAME_LOWSEC_TAG = gettext_noop("lowsec")
     NAME_NULLSEC_TAG = gettext_noop("nullsec")
     NAME_W_SPACE_TAG = gettext_noop("w_space")
 
     class Style(models.TextChoices):
-        GREY = "default", "grey"
-        DARK_BLUE = "primary", "dark blue"
-        GREEN = "success", "green"
-        LIGHT_BLUE = "info", "light blue"
-        ORANGE = "warning", "orange"
-        RED = "danger", "red"
+        GREY = "default", _("grey")
+        DARK_BLUE = "primary", _("dark blue")
+        GREEN = "success", _("green")
+        LIGHT_BLUE = "info", _("light blue")
+        ORANGE = "warning", _("orange")
+        RED = "danger", _("red")
 
     SPACE_TYPE_MAP = {
         EveSpaceType.HIGHSEC: {"name": NAME_HIGHSEC_TAG, "style": Style.GREEN},
         EveSpaceType.LOWSEC: {"name": NAME_LOWSEC_TAG, "style": Style.ORANGE},
         EveSpaceType.NULLSEC: {"name": NAME_NULLSEC_TAG, "style": Style.RED},
         EveSpaceType.W_SPACE: {"name": NAME_W_SPACE_TAG, "style": Style.LIGHT_BLUE},
     }
 
     name = models.CharField(
-        max_length=255, unique=True, help_text="name of the tag - must be unique"
+        max_length=255,
+        unique=True,
+        verbose_name=_("name"),
+        help_text=_("name of the tag - must be unique"),
     )
     description = models.TextField(
-        null=True, default=None, blank=True, help_text="description for this tag"
+        null=True,
+        default=None,
+        blank=True,
+        verbose_name=_("description"),
+        help_text=_("description for this tag"),
     )
     style = models.CharField(
         max_length=16,
         choices=Style.choices,
         default="default",
         blank=True,
-        help_text="color style of tag",
+        verbose_name=_("style"),
+        help_text=_("color style of tag"),
     )
     order = models.PositiveIntegerField(
         default=100,
         blank=True,
         validators=[MinValueValidator(100)],
-        help_text=(
+        verbose_name=_("order"),
+        help_text=_(
             "number defining the order tags are shown. "
             "custom tags can not have an order below 100"
         ),
     )
     is_default = models.BooleanField(
         default=False,
-        help_text=(
-            "if true this custom tag will automatically be added " "to new structures"
+        verbose_name=_("is default"),
+        help_text=_(
+            "if true this custom tag will automatically be added to new structures"
         ),
     )
     is_user_managed = models.BooleanField(
         default=True,
-        help_text=(
+        verbose_name=_("is user managed"),
+        help_text=_(
             "if False this tag is created and managed by the system "
             "and can not be modified by users"
         ),
     )
 
     objects = StructureTagManager()
 
+    class Meta:
+        verbose_name = _("structure tag")
+        verbose_name_plural = _("structure tags")
+        ordering = ["order", "name"]
+
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self):
         return "{}(name='{}')".format(self.__class__.__name__, self.name)
 
-    class Meta:
-        ordering = ordering = ["order", "name"]
-
     @property
     def html(self) -> str:
         if self.is_user_managed:
             name = escape(self.name)
         else:
             name = _(self.name)
         return bootstrap_label_html(name, self.style)
@@ -182,177 +195,217 @@
         FULL_POWER = "FU", _("Full Power")
         LOW_POWER = "LO", _("Low Power")
         ABANDONED = "AB", _("Abandoned")
         LOW_ABANDONED = "LA", _("Abandoned?")
         UNKNOWN = "UN", _("Unknown")
 
     id = models.BigIntegerField(
-        primary_key=True, help_text="The Item ID of the structure"
+        primary_key=True,
+        verbose_name=_("id"),
+        help_text=_("The Item ID of the structure"),
     )
 
     created_at = models.DateTimeField(
         default=now,
-        help_text="date this structure was received from ESI for the first time",
+        verbose_name=_("created at"),
+        help_text=_("date this structure was received from ESI for the first time"),
     )
     eve_moon = models.ForeignKey(
         EveMoon,
         on_delete=models.SET_DEFAULT,
         null=True,
         default=None,
         blank=True,
         related_name="+",
-        help_text="Moon next to this structure - if any",
+        verbose_name=_("moon"),
+        help_text=_("Moon next to this structure - if any"),
     )
     eve_planet = models.ForeignKey(
         EvePlanet,
         on_delete=models.SET_DEFAULT,
         null=True,
         default=None,
         blank=True,
         related_name="+",
-        help_text="Planet next to this structure - if any",
+        verbose_name=_("planet"),
+        help_text=_("Planet next to this structure - if any"),
     )
     eve_solar_system = models.ForeignKey(
         EveSolarSystem,
         on_delete=models.CASCADE,
         related_name="+",
-        help_text="Solar System the structure is located",
+        verbose_name=_("solar system"),
+        help_text=_("Solar System the structure is located"),
     )
     eve_type = models.ForeignKey(
         EveType,
         on_delete=models.CASCADE,
         related_name="+",
-        help_text="Type of the structure",
+        verbose_name=_("type"),
+        help_text=_("Type of the structure"),
     )
     fuel_expires_at = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text="Date on which the structure will run out of fuel",
+        verbose_name=_("fuel expires at"),
+        help_text=_("Date on which the structure will run out of fuel"),
     )
     has_fitting = models.BooleanField(
         null=True,
         default=None,
         blank=True,
         db_index=True,
-        help_text="bool indicating if the structure has a fitting",
+        verbose_name=_("has fitting"),
+        help_text=_("bool indicating if the structure has a fitting"),
     )
     has_core = models.BooleanField(
         null=True,
         default=None,
         blank=True,
         db_index=True,
-        help_text="bool indicating if the structure has a quantum core",
+        verbose_name=_("has core"),
+        help_text=_("bool indicating if the structure has a quantum core"),
     )
     last_online_at = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text="date this structure had any of it's services online",
+        verbose_name=_("last online at"),
+        help_text=_("date this structure had any of it's services online"),
     )
     last_updated_at = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text="date this structure was last updated from the EVE server",
+        verbose_name=_("last updated at"),
+        help_text=_("date this structure was last updated from the EVE server"),
+    )
+    name = models.CharField(
+        max_length=255,
+        verbose_name=_("name"),
+        help_text=_("The full name of the structure"),
     )
-    name = models.CharField(max_length=255, help_text="The full name of the structure")
     next_reinforce_hour = models.PositiveIntegerField(
         null=True,
         default=None,
         blank=True,
         validators=[MaxValueValidator(23)],
-        help_text=(
+        verbose_name=_("next reinforce hour"),
+        help_text=_(
             "The requested change to reinforce_hour that will take "
             "effect at the time shown by next_reinforce_apply"
         ),
     )
     next_reinforce_apply = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text=(
+        verbose_name=_("next reinforce apply"),
+        help_text=_(
             "The requested change to reinforce_hour that will take "
             "effect at the time shown by next_reinforce_apply"
         ),
     )
     owner = models.ForeignKey(
         "Owner",
         on_delete=models.CASCADE,
         related_name="structures",
-        help_text="Corporation that owns the structure",
+        verbose_name=_("owner"),
+        help_text=_("Corporation that owns the structure"),
     )
     reinforce_hour = models.PositiveIntegerField(
         validators=[MaxValueValidator(23)],
         null=True,
         default=None,
         blank=True,
-        help_text=(
-            "The hour of day that determines the four hour window "
+        verbose_name=_("reinforce hour"),
+        help_text=_(
+            "The average hour of day that determines the time +/- some hours "
             "when the structure will randomly exit its reinforcement periods "
             "and become vulnerable to attack against its armor and/or hull. "
-            "The structure will become vulnerable at a random time that "
-            "is +/- 2 hours centered on the value of this property"
         ),
     )
     position_x = models.FloatField(
-        null=True, default=None, blank=True, help_text="x position in the solar system"
+        null=True,
+        default=None,
+        blank=True,
+        verbose_name=_("position x"),
+        help_text=_("x position in the solar system"),
     )
     position_y = models.FloatField(
-        null=True, default=None, blank=True, help_text="y position in the solar system"
+        null=True,
+        default=None,
+        blank=True,
+        verbose_name=_("position y"),
+        help_text=_("y position in the solar system"),
     )
     position_z = models.FloatField(
-        null=True, default=None, blank=True, help_text="z position in the solar system"
+        null=True,
+        default=None,
+        blank=True,
+        verbose_name=_("position z"),
+        help_text=_("z position in the solar system"),
     )
     state = models.IntegerField(
         choices=State.choices,
         default=State.UNKNOWN,
         blank=True,
-        help_text="Current state of the structure",
+        verbose_name=_("state"),
+        help_text=_("Current state of the structure"),
     )
     state_timer_end = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text="Date at which the structure entered it’s current state",
+        verbose_name=_("state timer end"),
+        help_text=_("Date at which the structure entered it's current state"),
     )
     state_timer_start = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text="Date at which the structure will move to it’s next state",
+        verbose_name=_("state timer start"),
+        help_text=_("Date at which the structure will move to it's next state"),
     )
     tags = models.ManyToManyField(
         StructureTag,
         default=None,
         blank=True,
         related_name="structures",
-        help_text="List of tags for this structure. ",
+        verbose_name=_("tags"),
+        help_text=_("List of tags for this structure. "),
     )
     unanchors_at = models.DateTimeField(
         null=True,
         default=None,
         blank=True,
-        help_text="Date at which the structure will unanchor",
+        verbose_name=_("unanchors at"),
+        help_text=_("Date at which the structure will unanchor"),
     )
     webhooks = models.ManyToManyField(
         "Webhook",
         default=None,
         blank=True,
         related_name="structures",
-        help_text=(
+        verbose_name=_("webhooks"),
+        help_text=_(
             "Webhooks for sending notifications to. "
             "If any webhook is enabled, these will be used instead of the webhooks "
             "defined for the respective owner. "
             "If no webhook is enabled the owner's setting will be used. "
         ),
     )
 
     objects = StructureManager()
 
+    class Meta:
+        verbose_name = _("structure")
+        verbose_name_plural = _("structures")
+
     def __str__(self) -> str:
         if self.is_upwell_structure:
             try:
                 location_name = self.eve_solar_system.name
             except AttributeError:
                 location_name = "?"
         else:
@@ -402,48 +455,48 @@
         return starbases.is_starbase(self.eve_type)
 
     @cached_property
     def is_upwell_structure(self) -> bool:
         return self.eve_type.eve_group.eve_category_id == EveCategoryId.STRUCTURE
 
     @property
-    def is_full_power(self) -> bool:
+    def is_full_power(self) -> Optional[bool]:
         """return True if structure is full power, False if not.
 
         Returns None if state can not be determined
         """
         power_mode = self.power_mode
         if not power_mode:
             return None
         return power_mode == self.PowerMode.FULL_POWER
 
     @property
-    def is_low_power(self) -> bool:
+    def is_low_power(self) -> Optional[bool]:
         """return True if structure is low power, False if not.
 
         Returns None if state can not be determined
         """
         power_mode = self.power_mode
         if not power_mode:
             return None
         return power_mode == self.PowerMode.LOW_POWER
 
     @property
-    def is_abandoned(self) -> bool:
+    def is_abandoned(self) -> Optional[bool]:
         """return True if structure is abandoned, False if not.
 
         Returns None if state can not be determined
         """
         power_mode = self.power_mode
         if not power_mode:
             return None
         return power_mode == self.PowerMode.ABANDONED
 
     @property
-    def is_maybe_abandoned(self) -> bool:
+    def is_maybe_abandoned(self) -> Optional[bool]:
         """return True if structure is maybe abandoned, False if not.
 
         Returns None if state can not be determined
         """
         power_mode = self.power_mode
         if not power_mode:
             return None
@@ -486,14 +539,23 @@
             self.State.POS_ONLINE,
             self.State.POS_REINFORCED,
             self.State.POS_UNANCHORING,
         ]:
             return True
         return False
 
+    @property
+    def has_position(self) -> bool:
+        """Evaluate if this structure has a position."""
+        return (
+            self.position_x is not None
+            and self.position_y is not None
+            and self.position_z is not None
+        )
+
     @cached_property
     def owner_has_sov(self) -> bool:
         return self.owner.has_sov(self.eve_solar_system)
 
     @cached_property
     def location_name(self) -> str:
         """Name of this structures's location."""
@@ -508,18 +570,22 @@
         try:
             return self.eve_solar_system.name
         except AttributeError:
             return "?"
 
     def distance_to_object(self, x: float, y: float, z: float) -> float:
         """Distance to object with given coordinates (within same solar system)."""
+        if not self.has_position:
+            raise ValueError(
+                f"{self}: Can not calculate distance from a structure without a position"
+            )
         return math.sqrt(
-            pow(x - self.position_x, 2)
-            + pow(y - self.position_y, 2)
-            + pow(z - self.position_z, 2)
+            pow(x - self.position_x, 2)  # type: ignore
+            + pow(y - self.position_y, 2)  # type: ignore
+            + pow(z - self.position_z, 2)  # type: ignore
         )
 
     @cached_property
     def structure_fuel_quantity(self) -> Optional[int]:
         """Current quantity of fuel blocks in units used as fuel."""
         return self.items.filter(
             location_flag=StructureItem.LocationFlag.STRUCTURE_FUEL,
@@ -558,15 +624,15 @@
     @property
     def hours_fuel_expires(self) -> Optional[float]:
         """Hours until fuel expires."""
         if self.fuel_expires_at:
             return hours_until_deadline(self.fuel_expires_at)
         return None
 
-    def is_fuel_expiry_date_different(self, other: "Structure") -> True:
+    def is_fuel_expiry_date_different(self, other: "Structure") -> bool:
         """True when fuel expiry date from other structure is different.
 
         Will compare using threshold setting.
         """
         change_threshold = (
             self.FUEL_DATES_EQUAL_THRESHOLD_UPWELL
             if self.is_upwell_structure
@@ -699,32 +765,42 @@
         CORP_DELIVERIES = "CorpDeliveries"
         FIGHTER_BAY = "FighterBay"
         OFFICE_FOLDER = "OfficeFolder"
         QUANTUM_CORE_ROOM = "QuantumCoreRoom"
         SECONDARY_STORAGE = "SecondaryStorage"
         STRUCTURE_FUEL = "StructureFuel"
 
-    id = models.BigIntegerField(primary_key=True, help_text="The Eve item ID")
+    id = models.BigIntegerField(
+        primary_key=True, verbose_name=_("id"), help_text=_("The Eve item ID")
+    )
     structure = models.ForeignKey(
         Structure,
         on_delete=models.CASCADE,
         related_name="items",
-        help_text="Structure this item is located in",
+        verbose_name=_("structure"),
+        help_text=_("Structure this item is located in"),
     )
 
     eve_type = models.ForeignKey(
         EveType,
         on_delete=models.CASCADE,
-        help_text="eve type of the item",
         related_name="+",
+        verbose_name=_("type"),
+        help_text=_("type of the item"),
     )
-    is_singleton = models.BooleanField(null=False)
-    last_updated_at = models.DateTimeField(auto_now=True)
-    location_flag = models.CharField(max_length=255)
-    quantity = models.IntegerField(null=False)
+    is_singleton = models.BooleanField(verbose_name=_("is singleton"))
+    last_updated_at = models.DateTimeField(
+        auto_now=True, verbose_name=_("last updated at")
+    )
+    location_flag = models.CharField(max_length=255, verbose_name=_("location flag"))
+    quantity = models.IntegerField(verbose_name=_("quantity"))
+
+    class Meta:
+        verbose_name = _("structure item")
+        verbose_name_plural = _("structure items")
 
     def __str__(self) -> str:
         return str(self.eve_type.name)
 
     def __repr__(self):
         return "{}(pk={}, structure=<{}>, eve_type=<{}>)".format(
             self.__class__.__name__, self.pk, self.structure, self.eve_type
@@ -761,23 +837,30 @@
                 else cls.OFFLINE
             )
 
     structure = models.ForeignKey(
         Structure,
         on_delete=models.CASCADE,
         related_name="services",
-        help_text="Structure this service is installed to",
+        verbose_name=_("structure"),
+        help_text=_("Structure this service is installed to"),
+    )
+    name = models.CharField(
+        max_length=100, verbose_name=_("name"), help_text=_("Name of the service")
     )
-    name = models.CharField(max_length=100, help_text="Name of the service")
 
     state = models.IntegerField(
-        choices=State.choices, help_text="Current state of this service"
+        choices=State.choices,
+        verbose_name=_("state"),
+        help_text=_("Current state of this service"),
     )
 
     class Meta:
+        verbose_name = _("structure service")
+        verbose_name_plural = _("structure services")
         unique_together = (("structure", "name"),)
 
     def __str__(self):
         return "{} - {}".format(str(self.structure), self.name)
 
     def __repr__(self):
         return "{}(structure_id={}, name='{}')".format(
@@ -949,11 +1032,16 @@
 
     eve_type = models.ForeignKey(EveType, on_delete=models.CASCADE, related_name="+")
     detail = models.ForeignKey(
         StarbaseDetail, on_delete=models.CASCADE, related_name="fuels"
     )
     quantity = models.IntegerField()
 
+    class Meta:
+        constraints = [
+            models.UniqueConstraint(
+                fields=["detail", "eve_type"], name="functional_pk_starbasedetailfuel"
+            )
+        ]
+
     def __str__(self) -> str:
         return f"{self.detail}-{self.eve_type}"
-
-    # TODO: Add unique constraints for detail, eve_type
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa-structures-2.1.0/structures/static/structures/css/global.css` & `aa_structures-2.2.0/structures/static/structures/css/global.css`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/css/main.css` & `aa_structures-2.2.0/structures/static/structures/css/main.css`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/Spinner-1s-64px-dark.gif` & `aa_structures-2.2.0/structures/static/structures/img/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/Spinner-1s-64px-light.gif` & `aa_structures-2.2.0/structures/static/structures/img/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/eve_symbol_128.png` & `aa_structures-2.2.0/structures/static/structures/img/eve_symbol_128.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/0h.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/0h.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/0l.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/0l.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/0m.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/0m.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/0r.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/0r.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/0s.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/0s.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/1h.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/1h.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/1l.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/1l.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/1m.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/1m.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/1r.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/1r.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/2h.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/2h.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/2l.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/2l.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/2m.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/2m.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/2r.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/2r.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/3h.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/3h.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/3l.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/3l.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/3m.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/3m.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/3r.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/3r.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/4h.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/4h.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/4l.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/4l.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/4m.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/4m.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/4s.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/4s.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/5h.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/5h.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/5l.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/5l.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/5m.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/5m.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/5s.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/5s.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/6h.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/6h.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/6l.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/6l.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/6m.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/6m.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/7h.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/7h.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/7l.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/7l.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/7m.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/7m.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/8h.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/8h.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/8l.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/8l.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/8m.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/8m.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/circle.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/circle.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/dustwheel.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/dustwheel.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/h.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/h.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/l.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/l.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/m.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/m.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/noship.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/noship.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/r.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/r.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/tyrannis.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/tyrannis_blue.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_blue.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/tyrannis_darkred.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_darkred.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/tyrannis_default.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_default.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/static/structures/img/pannel/tyrannis_revelations.png` & `aa_structures-2.2.0/structures/static/structures/img/panel/tyrannis_revelations.png`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/swagger.json` & `aa_structures-2.2.0/structures/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/tasks.py` & `aa_structures-2.2.0/structures/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,43 +59,43 @@
         logger.warning(
             "No owner configured to process alliance wide notifications. "
             "Please set 'is alliance main' to True for the designated owner."
         )
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
-def update_all_for_owner(owner_pk, user_pk=None):
+def update_all_for_owner(owner_pk, user_pk: Optional[int] = None):
     """Update structures and notifications for owner from ESI."""
     chain(
         update_structures_for_owner.si(owner_pk, user_pk),
         process_notifications_for_owner.si(owner_pk, user_pk),
     ).delay()
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
-def update_structures_for_owner(owner_pk, user_pk=None):
+def update_structures_for_owner(owner_pk, user_pk: Optional[int] = None):
     """Fetch all structures for owner and update related corp assets from ESI."""
     if not fetch_esi_status().is_ok:
         logger.warning("ESI currently not available. Aborting.")
     else:
         chain(
             update_structures_esi_for_owner.si(owner_pk, user_pk),
             update_structures_assets_for_owner.si(owner_pk, user_pk),
         ).delay()
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
-def update_structures_esi_for_owner(owner_pk, user_pk=None):
+def update_structures_esi_for_owner(owner_pk, user_pk: Optional[int] = None):
     """Update all structures for owner for ESI."""
     owner = Owner.objects.get(pk=owner_pk)
     owner.update_structures_esi(_get_user(user_pk))
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
-def update_structures_assets_for_owner(owner_pk, user_pk=None):
+def update_structures_assets_for_owner(owner_pk, user_pk: Optional[int] = None):
     """Update all related assets for owner."""
     owner = Owner.objects.get(pk=owner_pk)
     owner.update_asset_esi(_get_user(user_pk))
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
 def fetch_all_notifications():
@@ -113,15 +113,15 @@
     for config_pk in JumpFuelAlertConfig.objects.filter(is_enabled=True).values_list(
         "pk", flat=True
     ):
         send_jump_fuel_notifications_for_config.delay(config_pk)
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
-def process_notifications_for_owner(owner_pk: int, user_pk: int = None):
+def process_notifications_for_owner(owner_pk: int, user_pk: Optional[int] = None):
     """Fetch all notification for owner from ESI and processes them."""
     if not fetch_esi_status().is_ok:
         logger.warning("ESI currently not available. Aborting.")
         return
     chain(
         fetch_notification_for_owner.si(owner_pk=owner_pk, user_pk=user_pk).set(
             priority=TASK_PRIORITY_HIGH
@@ -135,15 +135,15 @@
         generate_new_timers_for_owner.si(owner_pk=owner_pk).set(
             priority=TASK_PRIORITY_HIGH
         ),
     ).delay()
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
-def fetch_notification_for_owner(owner_pk: int, user_pk: int = None):
+def fetch_notification_for_owner(owner_pk: int, user_pk: Optional[int] = None):
     """Fetch notifications from ESI."""
     owner = Owner.objects.get(pk=owner_pk)
     owner.fetch_notifications_esi(_get_user(user_pk))
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
 def update_existing_notifications(owner_pk: int) -> int:
@@ -208,15 +208,17 @@
 @shared_task(base=QueueOnce)
 def send_messages_for_webhook(webhook_pk: int) -> None:
     """Send all currently queued messages for given webhook to Discord."""
     Webhook.objects.send_queued_messages_for_webhook(webhook_pk)
 
 
 @shared_task(time_limit=STRUCTURES_TASKS_TIME_LIMIT)
-def send_test_notifications_to_webhook(webhook_pk, user_pk=None) -> None:
+def send_test_notifications_to_webhook(
+    webhook_pk, user_pk: Optional[int] = None
+) -> None:
     """Send test notification to given webhook."""
     webhook = Webhook.objects.get(pk=webhook_pk)
     user = _get_user(user_pk)
     send_report, send_success = webhook.send_test_message(user)
     if user:
         message = 'Test notification to webhook "{}" {}.\n'.format(
             webhook, "completed successfully" if send_success else "has failed"
@@ -229,15 +231,15 @@
                 __title__, webhook, "OK" if send_success else "FAILED"
             ),
             message=message,
             level="success" if send_success else "danger",
         )
 
 
-def _get_user(user_pk: int) -> Optional[User]:
+def _get_user(user_pk: Optional[int]) -> Optional[User]:
     """Fetch the user or return None."""
     if not user_pk:
         return None
     try:
         return User.objects.get(pk=user_pk)
     except User.DoesNotExist:
         logger.warning("Ignoring non-existing user with pk %s", user_pk)
```

### Comparing `aa-structures-2.1.0/structures/templates/structures/main.html` & `aa_structures-2.2.0/structures/templates/structures/main.html`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/templates/structures/modals/fitting_gfx.html` & `aa_structures-2.2.0/structures/templates/structures/modals/fitting_gfx.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load static %}
 {% load evelinks %}
 
 <div id="Fitting_Panel" style="position: relative; height:398px; width:398px; z-index: 3; margin: 0 auto;" >
     <div id="mask" style="position:absolute; left: 0px; top: 0px; width:398px; height:398px; z-index:-1;">
-        <img style="position:absolute; left: 0px; top: 0px;  height:398px; width:398px; border:0px" src="{% static 'structures/img/pannel/tyrannis.png' %}" alt="" />
+        <img style="position:absolute; left: 0px; top: 0px;  height:398px; width:398px; border:0px" src="{% static 'structures/img/panel/tyrannis.png' %}" alt="" />
     </div>
 
     <div id="highx" style="position:absolute; left: 0px; top: 0px; width: 398px; height: 398px; z-index:-1;">
         <img src="{{ slots.high }}" alt="" style="border:0px;" />
     </div>
     <div id="high1" style="position:absolute; left:73px; top:60px; width:32px; height:32px;">{% if assets_grouped.HiSlot0 %}<img src="{{ assets_grouped.HiSlot0.eve_type_id|type_icon_url:128 }}" style="height: 32px; width: 32px;" title="{{ assets_grouped.HiSlot0.eve_type.name }}">{% endif %}</div>
     <div id="high2" style="position:absolute; left:102px; top:42px; width:32px; height:32px;">{% if assets_grouped.HiSlot1 %}<img src="{{ assets_grouped.HiSlot1.eve_type_id|type_icon_url:128 }}" style="height: 32px; width: 32px;" title="{{ assets_grouped.HiSlot1.eve_type.name }}">{% endif %}</div>
```

### Comparing `aa-structures-2.1.0/structures/templates/structures/modals/poco_details.html` & `aa_structures-2.2.0/structures/templates/structures/modals/poco_details.html`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/templates/structures/modals/starbase_detail.html` & `aa_structures-2.2.0/structures/templates/structures/modals/starbase_detail.html`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/templates/structures/modals/structure_details.html` & `aa_structures-2.2.0/structures/templates/structures/modals/structure_details.html`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/templates/structures/modals/tab_general_detail.html` & `aa_structures-2.2.0/structures/templates/structures/modals/tab_general_detail.html`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/templates/structures/partials/jump_gates_list.html` & `aa_structures-2.2.0/structures/templates/structures/partials/jump_gates_list.html`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/templates/structures/partials/poco_list.html` & `aa_structures-2.2.0/structures/templates/structures/partials/poco_list.html`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/templates/structures/partials/structure_list.html` & `aa_structures-2.2.0/structures/templates/structures/partials/structure_list.html`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/templates/structures/partials/structure_summary.html` & `aa_structures-2.2.0/structures/templates/structures/partials/structure_summary.html`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                     <th class="text-right">{% translate "Starbases" %}</th>
                     <th class="text-right">{% translate "Total" %}</th>
                 </tr>
             </thead>
             <tfoot>
                 <tr class="info">
                     <th></th>
-                    <th>Total</th>
+                    <th>{% translate "Total" %}</th>
                     <th></th>
                     <th class="text-right"></th>
                     <th class="text-right"></th>
                     <th class="text-right"></th>
                     <th class="text-right"></th>
                     <th class="text-right"></th>
                     <th class="text-right"></th>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 {% load i18n %} {% load bootstrap %}
                {%         {%         {% translate              {%        {%        {%          {%
  {% translate  translate  translate  "Engineering {% translate translate translate translate   translate
  "Corporation" "Alliance" "Citadels" Complexes"   "Refineries" "Other    "Customs  "Starbases" "Total"
  %}            %}         %}         %}           %}           Upwell"   Offices"  %}          %}
                                                                %}        %}
- Total
+ {% translate
+ "Total" %}
```

### Comparing `aa-structures-2.1.0/structures/templates/structures/templatetags/list_item.html` & `aa_structures-2.2.0/structures/templates/structures/templatetags/list_item.html`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/templatetags/structures.py` & `aa_structures-2.2.0/structures/templatetags/structures.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/urls.py` & `aa_structures-2.2.0/structures/urls.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/views.py` & `aa_structures-2.2.0/structures/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
-import urllib
 from collections import defaultdict
 from enum import IntEnum
+from urllib.parse import urlencode
 
 from django.contrib.auth.decorators import login_required, permission_required
 from django.contrib.staticfiles.storage import staticfiles_storage
 from django.db.models import Count, Q
 from django.http import HttpResponse, HttpResponseServerError, JsonResponse
 from django.shortcuts import get_object_or_404, redirect, render
 from django.urls import reverse
@@ -60,15 +60,15 @@
     url = reverse("structures:main")
     if STRUCTURES_DEFAULT_TAGS_FILTER_ENABLED:
         params = {
             QUERY_PARAM_TAGS: ",".join(
                 [x.name for x in StructureTag.objects.filter(is_default=True)]
             )
         }
-        url += "?{}".format(urllib.parse.urlencode(params))
+        url += "?{}".format(urlencode(params))
     return redirect(url)
 
 
 @login_required
 @permission_required("structures.basic_access")
 def main(request):
     """Main view"""
@@ -79,27 +79,27 @@
             for name, activated in form.cleaned_data.items():
                 if activated:
                     active_tags.append(get_object_or_404(StructureTag, name=name))
 
             url = reverse("structures:main")
             if active_tags:
                 params = {QUERY_PARAM_TAGS: ",".join([x.name for x in active_tags])}
-                url += "?{}".format(urllib.parse.urlencode(params))
+                url += "?{}".format(urlencode(params))
             return redirect(url)
     else:
         tags_raw = request.GET.get(QUERY_PARAM_TAGS)
         if tags_raw:
             tags_parsed = tags_raw.split(",")
             active_tags = [
                 x for x in StructureTag.objects.all() if x.name in tags_parsed
             ]
         form = TagsFilterForm(initial={x.name: True for x in active_tags})
 
     context = {
-        "page_title": _(__title__),
+        "page_title": __title__,
         "active_tags": active_tags,
         "tags_filter_form": form,
         "tags_exist": StructureTag.objects.exists(),
         "data_tables_page_length": STRUCTURES_DEFAULT_PAGE_LENGTH,
         "data_tables_paging": STRUCTURES_PAGING_ENABLED,
         "show_jump_gates_tab": STRUCTURES_SHOW_JUMP_GATES,
         "last_updated": Owner.objects.structures_last_updated(),
@@ -137,16 +137,17 @@
                 self.MEDIUM: "m",
                 self.LOW: "l",
                 self.RIG: "r",
                 self.SERVICE: "s",
             }
             try:
                 slot_num = type_attributes[self.value]
+                my_id = id_map[Slot(self.value)]
                 return staticfiles_storage.url(
-                    f"structures/img/pannel/{slot_num}{id_map[self.value]}.png"
+                    f"structures/img/panel/{slot_num}{my_id}.png"
                 )
             except KeyError:
                 return ""
 
     class FakeEveType:
         def __init__(self, id, name):
             self.id = id
@@ -248,15 +249,15 @@
         elif asset.location_flag == StructureItem.LocationFlag.STRUCTURE_FUEL:
             assets_grouped["fuel_bay"].append(asset)
         else:
             assets_grouped[asset.location_flag] = asset
     if structure.is_upwell_structure:
         assets_grouped["fuel_usage"] = [
             FakeAsset(
-                name="Fuel blocks per day (est.)",
+                name=_("Fuel blocks per day (est.)"),
                 quantity=structure.structure_fuel_usage(),
                 eve_type_id=24756,
             )
         ]
     modules_count = len(high_slots + med_slots + low_slots + rig_slots + service_slots)
     fuel_blocks_total = (
         functools.reduce(
@@ -386,15 +387,15 @@
         "last_updated_at": structure.last_updated_at,
     }
     return render(request, "structures/modals/starbase_detail.html", context)
 
 
 @login_required
 @permission_required("structures.add_structure_owner")
-@token_required(scopes=Owner.get_esi_scopes())
+@token_required(scopes=Owner.get_esi_scopes())  # type: ignore
 def add_structure_owner(request, token):
     token_char = get_object_or_404(EveCharacter, character_id=token.character_id)
     try:
         character_ownership = CharacterOwnership.objects.get(
             user=request.user, character=token_char
         )
     except CharacterOwnership.DoesNotExist:
```

### Comparing `aa-structures-2.1.0/structures/webhooks/core.py` & `aa_structures-2.2.0/structures/webhooks/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from time import sleep
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 from urllib.parse import urlparse
 
 import dhooks_lite
 from simple_mq import SimpleMQ
 
 from django.contrib.auth.models import User
 
@@ -60,19 +60,19 @@
             else:
                 counter += 1
 
         return counter
 
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
         Raises ValueError if message is incomplete
         """
         if not content and not embeds:
@@ -144,15 +144,15 @@
 
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
@@ -161,28 +161,28 @@
             wait_for_response=True,
         )
         logger.debug("headers: %s", response.headers)
         logger.debug("status_code: %s", response.status_code)
         logger.debug("content: %s", response.content)
         if response.status_ok:
             return True
-        message = (
+        msg = (
             f"Webhook {self} failed to send message to Discord.\n"
             f"HTTP status code: {response.status_code}\n"
             f"API response: {response.content}"
         )
-        logger.warning(message, exc_info=True)
+        logger.warning(msg, exc_info=True)
         return False
 
     @classmethod
     def create_link(cls, name: str, url: str) -> str:
         """creates a link for messages of this webhook"""
         return f"[{str(name)}]({str(url)})"
 
-    def send_test_message(self, user: User = None) -> Tuple[str, bool]:
+    def send_test_message(self, user: Optional[User] = None) -> Tuple[str, bool]:
         """Sends a test notification to this webhook and returns send report"""
         user_text = f" sent by **{user}**" if user else ""
         message = {
             "content": f"Test message for webhook **{self.name}**{user_text}",
             "username": __title__,
         }
         try:
```

### Comparing `aa-structures-2.1.0/structures/webhooks/managers.py` & `aa_structures-2.2.0/structures/webhooks/managers.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/webhooks/models.py` & `aa_structures-2.2.0/structures/webhooks/models.py`

 * *Files identical despite different names*

### Comparing `aa-structures-2.1.0/structures/webhooks/tests/test_core.py` & `aa_structures-2.2.0/structures/webhooks/tests/test_core.py`

 * *Files identical despite different names*

