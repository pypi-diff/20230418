# Comparing `tmp/garpix_user-3.5.0rc6.tar.gz` & `tmp/garpix_user-3.5.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_user-3.5.0rc6.tar", last modified: Fri Apr 14 08:31:48 2023, max compression
+gzip compressed data, was "garpix_user-3.5.0rc7.tar", last modified: Tue Apr 18 20:27:00 2023, max compression
```

## Comparing `garpix_user-3.5.0rc6.tar` & `garpix_user-3.5.0rc7.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.806700 garpix_user-3.5.0rc6/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-14 08:31:48.000000 garpix_user-3.5.0rc6/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9822 2023-04-14 08:31:48.806527 garpix_user-3.5.0rc6/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.798535 garpix_user-3.5.0rc6/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4658 2023-03-07 14:06:25.000000 garpix_user-3.5.0rc6/garpix_user/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc6/garpix_user/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9155 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc6/garpix_user/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc6/garpix_user/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.799691 garpix_user-3.5.0rc6/garpix_user/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/admin/referral_type.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.5.0rc6/garpix_user/admin/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/admin/user_session.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc6/garpix_user/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.5.0rc6/garpix_user/exceptions.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.799900 garpix_user-3.5.0rc6/garpix_user/forms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/forms/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      869 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/forms/login.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.795916 garpix_user-3.5.0rc6/garpix_user/locale/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.795968 garpix_user-3.5.0rc6/garpix_user/locale/ru/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.800114 garpix_user-3.5.0rc6/garpix_user/locale/ru/LC_MESSAGES/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6866 2023-04-14 08:29:08.000000 garpix_user-3.5.0rc6/garpix_user/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9277 2023-04-07 10:32:34.000000 garpix_user-3.5.0rc6/garpix_user/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.800228 garpix_user-3.5.0rc6/garpix_user/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.800418 garpix_user-3.5.0rc6/garpix_user/mixins/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/mixins/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.800886 garpix_user-3.5.0rc6/garpix_user/mixins/models/confirm/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/mixins/models/confirm/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.5.0rc6/garpix_user/mixins/models/confirm/code_length_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4888 2023-03-07 13:29:14.000000 garpix_user-3.5.0rc6/garpix_user/mixins/models/confirm/email_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3242 2023-03-07 13:31:03.000000 garpix_user-3.5.0rc6/garpix_user/mixins/models/confirm/phone_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5436 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc6/garpix_user/mixins/models/restore_password.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.801220 garpix_user-3.5.0rc6/garpix_user/mixins/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/mixins/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc6/garpix_user/mixins/serializers/password_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.5.0rc6/garpix_user/mixins/serializers/to_lower.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.801862 garpix_user-3.5.0rc6/garpix_user/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc6/garpix_user/models/access_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/models/refferal.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc6/garpix_user/models/refresh_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.5.0rc6/garpix_user/models/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4894 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc6/garpix_user/models/user_session.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.802058 garpix_user-3.5.0rc6/garpix_user/rest/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/rest/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1709 2023-03-01 07:20:35.000000 garpix_user-3.5.0rc6/garpix_user/rest/authentication.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.802922 garpix_user-3.5.0rc6/garpix_user/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      769 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.5.0rc6/garpix_user/serializers/auth_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/serializers/email_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1418 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc6/garpix_user/serializers/passwrod_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/serializers/phone_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/serializers/refresh_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.5.0rc6/garpix_user/serializers/registration_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.5.0rc6/garpix_user/serializers/user_session_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1565 2023-04-14 08:28:12.000000 garpix_user-3.5.0rc6/garpix_user/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.803125 garpix_user-3.5.0rc6/garpix_user/tasks/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc6/garpix_user/tasks/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.5.0rc6/garpix_user/tasks/delete_unconfirmed_users.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.796617 garpix_user-3.5.0rc6/garpix_user/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.803232 garpix_user-3.5.0rc6/garpix_user/templates/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/templates/garpix_user/send_confirm.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.803442 garpix_user-3.5.0rc6/garpix_user/tests/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/tests/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.803889 garpix_user-3.5.0rc6/garpix_user/tests/test_api/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/tests/test_api/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.804090 garpix_user-3.5.0rc6/garpix_user/tests/test_api/_trial_temp/
--rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/tests/test_api/_trial_temp/_trial_marker
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.5.0rc6/garpix_user/tests/test_api/_trial_temp/test.log
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/tests/test_api/api_login.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/tests/test_api/api_registration.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc6/garpix_user/tests/test_api/api_user_session_restore_password.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/tests/test_views.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.804392 garpix_user-3.5.0rc6/garpix_user/tests/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/tests/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/tests/utils/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/tests/utils/test_case_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2581 2023-03-07 13:05:56.000000 garpix_user-3.5.0rc6/garpix_user/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.805023 garpix_user-3.5.0rc6/garpix_user/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc6/garpix_user/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-03-20 15:00:08.000000 garpix_user-3.5.0rc6/garpix_user/utils/backends.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/utils/current_date.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.5.0rc6/garpix_user/utils/drf_spectacular.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      226 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/utils/get_token_from_request.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc6/garpix_user/utils/repluralize.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.806357 garpix_user-3.5.0rc6/garpix_user/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/views/change_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4040 2023-03-07 13:07:14.000000 garpix_user-3.5.0rc6/garpix_user/views/email_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1401 2023-02-27 12:35:42.000000 garpix_user-3.5.0rc6/garpix_user/views/login_views.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc6/garpix_user/views/logout_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1610 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/views/obtain_auth_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc6/garpix_user/views/phone_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/views/referral_links_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.5.0rc6/garpix_user/views/refresh_token_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/views/registration_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3210 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc6/garpix_user/views/restore_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc6/garpix_user/views/user_session_view.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-14 08:31:48.799235 garpix_user-3.5.0rc6/garpix_user.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9822 2023-04-14 08:31:48.000000 garpix_user-3.5.0rc6/garpix_user.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3140 2023-04-14 08:31:48.000000 garpix_user-3.5.0rc6/garpix_user.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-14 08:31:48.000000 garpix_user-3.5.0rc6/garpix_user.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-14 08:31:48.000000 garpix_user-3.5.0rc6/garpix_user.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      283 2023-04-14 08:31:48.000000 garpix_user-3.5.0rc6/garpix_user.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-04-14 08:31:48.000000 garpix_user-3.5.0rc6/garpix_user.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-04-14 08:31:48.806738 garpix_user-3.5.0rc6/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1565 2023-04-14 08:31:48.000000 garpix_user-3.5.0rc6/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.391217 garpix_user-3.5.0rc7/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9822 2023-04-18 20:27:00.390958 garpix_user-3.5.0rc7/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.382817 garpix_user-3.5.0rc7/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4658 2023-04-18 20:25:50.000000 garpix_user-3.5.0rc7/garpix_user/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc7/garpix_user/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9155 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc7/garpix_user/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc7/garpix_user/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.383888 garpix_user-3.5.0rc7/garpix_user/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/admin/referral_type.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.5.0rc7/garpix_user/admin/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/admin/user_session.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.5.0rc7/garpix_user/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.5.0rc7/garpix_user/exceptions.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.384102 garpix_user-3.5.0rc7/garpix_user/forms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/forms/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      869 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/forms/login.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.380079 garpix_user-3.5.0rc7/garpix_user/locale/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.380125 garpix_user-3.5.0rc7/garpix_user/locale/ru/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.384325 garpix_user-3.5.0rc7/garpix_user/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     6866 2023-04-14 08:29:08.000000 garpix_user-3.5.0rc7/garpix_user/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9277 2023-04-07 10:32:34.000000 garpix_user-3.5.0rc7/garpix_user/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.384433 garpix_user-3.5.0rc7/garpix_user/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.384624 garpix_user-3.5.0rc7/garpix_user/mixins/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.385069 garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/code_length_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4965 2023-04-18 20:24:54.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/email_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3242 2023-03-07 13:31:03.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/phone_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5436 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc7/garpix_user/mixins/models/restore_password.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.385402 garpix_user-3.5.0rc7/garpix_user/mixins/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/mixins/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc7/garpix_user/mixins/serializers/password_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.5.0rc7/garpix_user/mixins/serializers/to_lower.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.386035 garpix_user-3.5.0rc7/garpix_user/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc7/garpix_user/models/access_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/models/refferal.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.5.0rc7/garpix_user/models/refresh_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.5.0rc7/garpix_user/models/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4894 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc7/garpix_user/models/user_session.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.386227 garpix_user-3.5.0rc7/garpix_user/rest/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/rest/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1709 2023-03-01 07:20:35.000000 garpix_user-3.5.0rc7/garpix_user/rest/authentication.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.387083 garpix_user-3.5.0rc7/garpix_user/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      769 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.5.0rc7/garpix_user/serializers/auth_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/serializers/email_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1418 2023-02-06 08:33:47.000000 garpix_user-3.5.0rc7/garpix_user/serializers/passwrod_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/serializers/phone_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/serializers/refresh_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.5.0rc7/garpix_user/serializers/registration_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.5.0rc7/garpix_user/serializers/user_session_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1565 2023-04-18 20:25:50.000000 garpix_user-3.5.0rc7/garpix_user/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.387310 garpix_user-3.5.0rc7/garpix_user/tasks/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.5.0rc7/garpix_user/tasks/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.5.0rc7/garpix_user/tasks/delete_unconfirmed_users.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.380861 garpix_user-3.5.0rc7/garpix_user/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.387425 garpix_user-3.5.0rc7/garpix_user/templates/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/templates/garpix_user/send_confirm.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.387643 garpix_user-3.5.0rc7/garpix_user/tests/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.388074 garpix_user-3.5.0rc7/garpix_user/tests/test_api/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.388266 garpix_user-3.5.0rc7/garpix_user/tests/test_api/_trial_temp/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/_trial_temp/_trial_marker
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/_trial_temp/test.log
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_login.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_registration.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_user_session_restore_password.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/tests/test_views.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.388573 garpix_user-3.5.0rc7/garpix_user/tests/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/utils/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/tests/utils/test_case_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2581 2023-03-07 13:05:56.000000 garpix_user-3.5.0rc7/garpix_user/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.389256 garpix_user-3.5.0rc7/garpix_user/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.5.0rc7/garpix_user/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-03-20 15:00:08.000000 garpix_user-3.5.0rc7/garpix_user/utils/backends.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/utils/current_date.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.5.0rc7/garpix_user/utils/drf_spectacular.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      226 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/utils/get_token_from_request.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc7/garpix_user/utils/repluralize.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.390788 garpix_user-3.5.0rc7/garpix_user/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/change_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3993 2023-04-18 20:26:41.000000 garpix_user-3.5.0rc7/garpix_user/views/email_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1401 2023-02-27 12:35:42.000000 garpix_user-3.5.0rc7/garpix_user/views/login_views.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.5.0rc7/garpix_user/views/logout_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1610 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/obtain_auth_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.5.0rc7/garpix_user/views/phone_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/referral_links_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.5.0rc7/garpix_user/views/refresh_token_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/registration_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3210 2023-04-07 13:05:13.000000 garpix_user-3.5.0rc7/garpix_user/views/restore_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.5.0rc7/garpix_user/views/user_session_view.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-04-18 20:27:00.383460 garpix_user-3.5.0rc7/garpix_user.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9822 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3140 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      283 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/garpix_user.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-04-18 20:27:00.391256 garpix_user-3.5.0rc7/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1565 2023-04-18 20:27:00.000000 garpix_user-3.5.0rc7/setup.py
```

### Comparing `garpix_user-3.5.0rc6/PKG-INFO` & `garpix_user-3.5.0rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_user
-Version: 3.5.0rc6
+Version: 3.5.0rc7
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_user-3.5.0rc6/garpix_user/CHANGELOG.md` & `garpix_user-3.5.0rc7/garpix_user/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/CONTRIBUTING.md` & `garpix_user-3.5.0rc7/garpix_user/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/README.md` & `garpix_user-3.5.0rc7/garpix_user/README.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/README.rst` & `garpix_user-3.5.0rc7/garpix_user/README.rst`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/admin/user.py` & `garpix_user-3.5.0rc7/garpix_user/admin/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/exceptions.py` & `garpix_user-3.5.0rc7/garpix_user/exceptions.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/forms/login.py` & `garpix_user-3.5.0rc7/garpix_user/forms/login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/locale/ru/LC_MESSAGES/django.mo` & `garpix_user-3.5.0rc7/garpix_user/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/locale/ru/LC_MESSAGES/django.po` & `garpix_user-3.5.0rc7/garpix_user/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/mixins/models/confirm/code_length_mixin.py` & `garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/code_length_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/mixins/models/confirm/email_confirm.py` & `garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/email_confirm.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,9 +112,13 @@
                 return True
 
         return IncorrectCodeException(field='email_confirmation_code')
 
     def check_email_confirmation(self):
         return self.is_email_confirmed
 
+    @classmethod
+    def confirm_link_redirect_url(cls):
+        return '/'
+
     class Meta:
         abstract = True
```

### Comparing `garpix_user-3.5.0rc6/garpix_user/mixins/models/confirm/phone_confirm.py` & `garpix_user-3.5.0rc7/garpix_user/mixins/models/confirm/phone_confirm.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/mixins/models/restore_password.py` & `garpix_user-3.5.0rc7/garpix_user/mixins/models/restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/mixins/serializers/password_mixin.py` & `garpix_user-3.5.0rc7/garpix_user/mixins/serializers/password_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/models/access_token.py` & `garpix_user-3.5.0rc7/garpix_user/models/access_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/models/refferal.py` & `garpix_user-3.5.0rc7/garpix_user/models/refferal.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/models/refresh_token.py` & `garpix_user-3.5.0rc7/garpix_user/models/refresh_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/models/user.py` & `garpix_user-3.5.0rc7/garpix_user/models/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/models/user_session.py` & `garpix_user-3.5.0rc7/garpix_user/models/user_session.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/rest/authentication.py` & `garpix_user-3.5.0rc7/garpix_user/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/serializers/__init__.py` & `garpix_user-3.5.0rc7/garpix_user/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/serializers/auth_token_serializer.py` & `garpix_user-3.5.0rc7/garpix_user/serializers/auth_token_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/serializers/passwrod_serializer.py` & `garpix_user-3.5.0rc7/garpix_user/serializers/passwrod_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/serializers/registration_serializer.py` & `garpix_user-3.5.0rc7/garpix_user/serializers/registration_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/settings.py` & `garpix_user-3.5.0rc7/garpix_user/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/setup.py` & `garpix_user-3.5.0rc7/garpix_user/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.5.0-rc6',
+    version='3.5.0-rc7',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_user-3.5.0rc6/garpix_user/tasks/delete_unconfirmed_users.py` & `garpix_user-3.5.0rc7/garpix_user/tasks/delete_unconfirmed_users.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/tests/test_api/api_login.py` & `garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/tests/test_api/api_registration.py` & `garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_registration.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/tests/test_api/api_user_session_restore_password.py` & `garpix_user-3.5.0rc7/garpix_user/tests/test_api/api_user_session_restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/tests/test_views.py` & `garpix_user-3.5.0rc7/garpix_user/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/tests/utils/settings.py` & `garpix_user-3.5.0rc7/garpix_user/tests/utils/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/tests/utils/test_case_mixin.py` & `garpix_user-3.5.0rc7/garpix_user/tests/utils/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/urls.py` & `garpix_user-3.5.0rc7/garpix_user/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/utils/backends.py` & `garpix_user-3.5.0rc7/garpix_user/utils/backends.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/utils/repluralize.py` & `garpix_user-3.5.0rc7/garpix_user/utils/repluralize.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/__init__.py` & `garpix_user-3.5.0rc7/garpix_user/views/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/change_password_view.py` & `garpix_user-3.5.0rc7/garpix_user/views/change_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/email_confirmation_view.py` & `garpix_user-3.5.0rc7/garpix_user/views/email_confirmation_view.py`

 * *Files 11% similar despite different names*

```diff
@@ -81,10 +81,11 @@
     def get_redirect_url(self, *args, **kwargs):
         User = get_user_model()
         hash = self.kwargs.get('hash', None)
         model_type = self.kwargs.get('model_type', None)
 
         model = UserSession if model_type == 'user_session' else User
         result = model.confirm_email_by_link(hash)
+        _redirect_url = User.confirm_link_redirect_url()
         if result is not True:
-            return f"{settings.GARPIX_USER.get('EMAIL_CONFIRMATION_LINK_REDIRECT', '/')}?status=error"
-        return f"{settings.GARPIX_USER.get('EMAIL_CONFIRMATION_LINK_REDIRECT', '/')}?status=success"
+            return f"{_redirect_url}?status=error"
+        return f"{_redirect_url}?status=success"
```

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/login_views.py` & `garpix_user-3.5.0rc7/garpix_user/views/login_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/logout_view.py` & `garpix_user-3.5.0rc7/garpix_user/views/logout_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/obtain_auth_token.py` & `garpix_user-3.5.0rc7/garpix_user/views/obtain_auth_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/phone_confirmation_view.py` & `garpix_user-3.5.0rc7/garpix_user/views/phone_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/referral_links_view.py` & `garpix_user-3.5.0rc7/garpix_user/views/referral_links_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/refresh_token_view.py` & `garpix_user-3.5.0rc7/garpix_user/views/refresh_token_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/registration_view.py` & `garpix_user-3.5.0rc7/garpix_user/views/registration_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/restore_password_view.py` & `garpix_user-3.5.0rc7/garpix_user/views/restore_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user/views/user_session_view.py` & `garpix_user-3.5.0rc7/garpix_user/views/user_session_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/garpix_user.egg-info/PKG-INFO` & `garpix_user-3.5.0rc7/garpix_user.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-user
-Version: 3.5.0rc6
+Version: 3.5.0rc7
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `garpix_user-3.5.0rc6/garpix_user.egg-info/SOURCES.txt` & `garpix_user-3.5.0rc7/garpix_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_user-3.5.0rc6/setup.py` & `garpix_user-3.5.0rc7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.5.0-rc6',
+    version='3.5.0-rc7',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

