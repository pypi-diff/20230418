# Comparing `tmp/starlette_web-0.1.3.tar.gz` & `tmp/starlette_web-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_web-0.1.3.tar", last modified: Sat Apr 15 08:29:36 2023, max compression
+gzip compressed data, was "starlette_web-0.1.4.tar", last modified: Tue Apr 18 20:55:02 2023, max compression
```

## Comparing `starlette_web-0.1.3.tar` & `starlette_web-0.1.4.tar`

### file list

```diff
@@ -1,260 +1,259 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.318779 starlette_web-0.1.3/
--rw-rw-rw-   0        0        0     1108 2023-04-15 07:48:43.000000 starlette_web-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       75 2023-04-13 19:30:53.000000 starlette_web-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3430 2023-04-15 08:29:36.318779 starlette_web-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2329 2023-03-26 13:41:03.000000 starlette_web-0.1.3/README.md
--rw-rw-rw-   0        0        0     2382 2023-04-15 08:29:19.000000 starlette_web-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 08:29:36.318779 starlette_web-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.177866 starlette_web-0.1.3/starlette_web/
--rw-rw-rw-   0        0        0       23 2022-12-29 14:13:54.000000 starlette_web-0.1.3/starlette_web/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.187874 starlette_web-0.1.3/starlette_web/common/
--rw-rw-rw-   0        0        0       52 2022-04-25 19:06:18.000000 starlette_web-0.1.3/starlette_web/common/__init__.py
--rw-rw-rw-   0        0        0     5348 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/app.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.190724 starlette_web-0.1.3/starlette_web/common/authorization/
--rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.3/starlette_web/common/authorization/__init__.py
--rw-rw-rw-   0        0        0      856 2023-03-25 08:05:20.000000 starlette_web-0.1.3/starlette_web/common/authorization/backends.py
--rw-rw-rw-   0        0        0      329 2023-03-25 08:05:20.000000 starlette_web-0.1.3/starlette_web/common/authorization/base_user.py
--rw-rw-rw-   0        0        0     3025 2023-03-25 08:05:20.000000 starlette_web-0.1.3/starlette_web/common/authorization/permissions.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.193718 starlette_web-0.1.3/starlette_web/common/caches/
--rw-rw-rw-   0        0        0       80 2023-03-16 18:44:56.000000 starlette_web-0.1.3/starlette_web/common/caches/__init__.py
--rw-rw-rw-   0        0        0     2162 2023-03-25 08:05:20.000000 starlette_web-0.1.3/starlette_web/common/caches/base.py
--rw-rw-rw-   0        0        0     3342 2023-04-01 08:01:57.000000 starlette_web-0.1.3/starlette_web/common/caches/base_lock.py
--rw-rw-rw-   0        0        0     1112 2023-03-16 18:44:56.000000 starlette_web-0.1.3/starlette_web/common/caches/cache_handler.py
--rw-rw-rw-   0        0        0     5241 2023-03-24 16:47:56.000000 starlette_web-0.1.3/starlette_web/common/caches/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.195712 starlette_web-0.1.3/starlette_web/common/channels/
--rw-rw-rw-   0        0        0       54 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/common/channels/__init__.py
--rw-rw-rw-   0        0        0     4253 2023-04-01 19:06:23.000000 starlette_web-0.1.3/starlette_web/common/channels/base.py
--rw-rw-rw-   0        0        0      447 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/common/channels/event.py
--rw-rw-rw-   0        0        0      181 2023-03-22 16:38:31.000000 starlette_web-0.1.3/starlette_web/common/channels/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.199702 starlette_web-0.1.3/starlette_web/common/channels/layers/
--rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/common/channels/layers/__init__.py
--rw-rw-rw-   0        0        0      753 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/common/channels/layers/base.py
--rw-rw-rw-   0        0        0     1694 2023-03-12 19:30:41.000000 starlette_web-0.1.3/starlette_web/common/channels/layers/local_memory.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.203153 starlette_web-0.1.3/starlette_web/common/conf/
--rw-rw-rw-   0        0        0     2285 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/conf/__init__.py
--rw-rw-rw-   0        0        0     3314 2023-04-13 17:27:54.000000 starlette_web-0.1.3/starlette_web/common/conf/app_manager.py
--rw-rw-rw-   0        0        0      198 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/common/conf/base_app_config.py
--rw-rw-rw-   0        0        0     1994 2023-04-15 07:17:45.000000 starlette_web-0.1.3/starlette_web/common/conf/global_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.206147 starlette_web-0.1.3/starlette_web/common/database/
--rw-rw-rw-   0        0        0      359 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/common/database/__init__.py
--rw-rw-rw-   0        0        0     1362 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/common/database/columns.py
--rw-rw-rw-   0        0        0       81 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/common/database/model_base.py
--rw-rw-rw-   0        0        0     9279 2023-04-09 22:15:24.000000 starlette_web-0.1.3/starlette_web/common/database/model_mixin.py
--rw-rw-rw-   0        0        0     1550 2023-02-17 20:43:07.000000 starlette_web-0.1.3/starlette_web/common/database/session_maker.py
--rw-rw-rw-   0        0        0     2059 2023-02-18 12:47:03.000000 starlette_web-0.1.3/starlette_web/common/database/types.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.209138 starlette_web-0.1.3/starlette_web/common/email/
--rw-rw-rw-   0        0        0      169 2022-05-22 18:14:32.000000 starlette_web-0.1.3/starlette_web/common/email/__init__.py
--rw-rw-rw-   0        0        0     1604 2023-03-28 17:00:26.000000 starlette_web-0.1.3/starlette_web/common/email/base_sender.py
--rw-rw-rw-   0        0        0     1770 2023-03-27 20:27:55.000000 starlette_web-0.1.3/starlette_web/common/email/email_manager.py
--rw-rw-rw-   0        0        0     1728 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/email/smtp.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.210800 starlette_web-0.1.3/starlette_web/common/files/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.3/starlette_web/common/files/__init__.py
--rw-rw-rw-   0        0        0     7085 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/files/cache.py
--rw-rw-rw-   0        0        0     3837 2023-04-01 08:06:20.000000 starlette_web-0.1.3/starlette_web/common/files/filelock.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.212416 starlette_web-0.1.3/starlette_web/common/files/storages/
--rw-rw-rw-   0        0        0      136 2023-03-30 20:24:14.000000 starlette_web-0.1.3/starlette_web/common/files/storages/__init__.py
--rw-rw-rw-   0        0        0     6332 2023-03-31 18:48:34.000000 starlette_web-0.1.3/starlette_web/common/files/storages/base.py
--rw-rw-rw-   0        0        0     4532 2023-04-01 16:31:26.000000 starlette_web-0.1.3/starlette_web/common/files/storages/filesystem.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.219803 starlette_web-0.1.3/starlette_web/common/http/
--rw-rw-rw-   0        0        0        0 2022-05-03 08:01:50.000000 starlette_web-0.1.3/starlette_web/common/http/__init__.py
--rw-rw-rw-   0        0        0     6650 2023-04-15 07:20:59.000000 starlette_web-0.1.3/starlette_web/common/http/base_endpoint.py
--rw-rw-rw-   0        0        0     4338 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/common/http/exception_handlers.py
--rw-rw-rw-   0        0        0     4287 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/http/exceptions.py
--rw-rw-rw-   0        0        0     1075 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/common/http/renderers.py
--rw-rw-rw-   0        0        0      336 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/common/http/responses.py
--rw-rw-rw-   0        0        0     1174 2023-04-14 17:38:43.000000 starlette_web-0.1.3/starlette_web/common/http/schemas.py
--rw-rw-rw-   0        0        0      942 2023-03-14 17:15:47.000000 starlette_web-0.1.3/starlette_web/common/http/statuses.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.220388 starlette_web-0.1.3/starlette_web/common/i18n/
--rw-rw-rw-   0        0        0      163 2022-09-03 15:11:31.000000 starlette_web-0.1.3/starlette_web/common/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.223045 starlette_web-0.1.3/starlette_web/common/management/
--rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.3/starlette_web/common/management/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-04-15 07:46:58.000000 starlette_web-0.1.3/starlette_web/common/management/admin_util.py
--rw-rw-rw-   0        0        0     1080 2023-04-06 12:18:07.000000 starlette_web-0.1.3/starlette_web/common/management/alembic_mixin.py
--rw-rw-rw-   0        0        0     6023 2023-04-13 17:02:30.000000 starlette_web-0.1.3/starlette_web/common/management/base.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.226010 starlette_web-0.1.3/starlette_web/common/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-21 19:56:59.000000 starlette_web-0.1.3/starlette_web/common/management/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.233019 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/
--rw-rw-rw-   0        0        0        0 2023-03-26 18:53:46.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/__init__.py
--rw-rw-rw-   0        0        0      376 2023-03-26 18:59:14.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/admin.py
--rw-rw-rw-   0        0        0      224 2023-03-26 18:55:02.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/apps.py
--rw-rw-rw-   0        0        0      297 2023-03-26 18:59:20.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/models.py
--rw-rw-rw-   0        0        0       95 2023-03-26 19:00:40.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/routes.py
--rw-rw-rw-   0        0        0      154 2023-03-26 19:00:00.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_app_defaults/views.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.235016 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/
--rw-rw-rw-   0        0        0        0 2023-03-26 17:54:43.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/__init__.py
--rw-rw-rw-   0        0        0      466 2023-04-03 20:19:20.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/asgi.py
--rw-rw-rw-   0        0        0      896 2023-03-26 17:36:41.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/command.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.237035 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/__init__.py
--rw-rw-rw-   0        0        0      885 2023-04-13 18:30:43.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/routes.py
--rw-rw-rw-   0        0        0     3354 2023-04-14 17:40:54.000000 starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/settings.py
--rw-rw-rw-   0        0        0     1552 2023-04-06 16:46:50.000000 starlette_web-0.1.3/starlette_web/common/management/commands/makemigrations.py
--rw-rw-rw-   0        0        0     1294 2023-04-06 16:46:56.000000 starlette_web-0.1.3/starlette_web/common/management/commands/migrate.py
--rw-rw-rw-   0        0        0     2171 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/management/commands/startapp.py
--rw-rw-rw-   0        0        0     3800 2023-04-06 16:47:27.000000 starlette_web-0.1.3/starlette_web/common/management/commands/startproject.py
--rw-rw-rw-   0        0        0     2019 2023-04-08 06:35:50.000000 starlette_web-0.1.3/starlette_web/common/management/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.242995 starlette_web-0.1.3/starlette_web/common/utils/
--rw-rw-rw-   0        0        0      506 2023-04-01 19:36:50.000000 starlette_web-0.1.3/starlette_web/common/utils/__init__.py
--rw-rw-rw-   0        0        0     2578 2022-09-03 15:11:31.000000 starlette_web-0.1.3/starlette_web/common/utils/choices.py
--rw-rw-rw-   0        0        0     1265 2023-03-18 14:43:23.000000 starlette_web-0.1.3/starlette_web/common/utils/crypto.py
--rw-rw-rw-   0        0        0      187 2023-04-01 19:33:59.000000 starlette_web-0.1.3/starlette_web/common/utils/encoding.py
--rw-rw-rw-   0        0        0      633 2023-02-17 20:46:29.000000 starlette_web-0.1.3/starlette_web/common/utils/importing.py
--rw-rw-rw-   0        0        0      546 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/utils/inspect.py
--rw-rw-rw-   0        0        0     2324 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/common/utils/json.py
--rw-rw-rw-   0        0        0     2273 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/common/utils/regex.py
--rw-rw-rw-   0        0        0     1828 2023-03-25 08:05:10.000000 starlette_web-0.1.3/starlette_web/common/utils/serializers.py
--rw-rw-rw-   0        0        0      246 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/common/utils/singleton.py
--rw-rw-rw-   0        0        0      217 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/common/utils/urls.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.243992 starlette_web-0.1.3/starlette_web/common/ws/
--rw-rw-rw-   0        0        0        0 2022-12-29 14:13:54.000000 starlette_web-0.1.3/starlette_web/common/ws/__init__.py
--rw-rw-rw-   0        0        0     6919 2023-03-14 17:15:47.000000 starlette_web-0.1.3/starlette_web/common/ws/base_endpoint.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.247013 starlette_web-0.1.3/starlette_web/contrib/
--rw-rw-rw-   0        0        0        0 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.249976 starlette_web-0.1.3/starlette_web/contrib/admin/
--rw-rw-rw-   0        0        0      185 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/contrib/admin/__init__.py
--rw-rw-rw-   0        0        0     3705 2023-03-24 18:55:03.000000 starlette_web-0.1.3/starlette_web/contrib/admin/admin.py
--rw-rw-rw-   0        0        0      564 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/admin/apps.py
--rw-rw-rw-   0        0        0     2780 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/contrib/admin/auth_provider.py
--rw-rw-rw-   0        0        0     5122 2023-03-18 20:17:51.000000 starlette_web-0.1.3/starlette_web/contrib/admin/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.252973 starlette_web-0.1.3/starlette_web/contrib/apispec/
--rw-rw-rw-   0        0        0        0 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/__init__.py
--rw-rw-rw-   0        0        0     2017 2023-04-03 20:01:29.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/apps.py
--rw-rw-rw-   0        0        0     5451 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/introspection.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.254001 starlette_web-0.1.3/starlette_web/contrib/apispec/marshmallow/
--rw-rw-rw-   0        0        0      352 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/marshmallow/__init__.py
--rw-rw-rw-   0        0        0     1545 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/marshmallow/converters.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.169232 starlette_web-0.1.3/starlette_web/contrib/apispec/static/
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.254001 starlette_web-0.1.3/starlette_web/contrib/apispec/static/apispec/
--rw-rw-rw-   0        0        0   879592 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/static/apispec/redoc.js
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.169232 starlette_web-0.1.3/starlette_web/contrib/apispec/templates/
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.255891 starlette_web-0.1.3/starlette_web/contrib/apispec/templates/apispec/
--rw-rw-rw-   0        0        0      539 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/templates/apispec/redoc.html
--rw-rw-rw-   0        0        0     1889 2023-04-13 18:25:49.000000 starlette_web-0.1.3/starlette_web/contrib/apispec/views.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.264264 starlette_web-0.1.3/starlette_web/contrib/auth/
--rw-rw-rw-   0        0        0        0 2023-04-13 17:15:05.000000 starlette_web-0.1.3/starlette_web/contrib/auth/__init__.py
--rw-rw-rw-   0        0        0     3484 2023-02-26 16:10:52.000000 starlette_web-0.1.3/starlette_web/contrib/auth/admin.py
--rw-rw-rw-   0        0        0      261 2023-03-17 18:16:19.000000 starlette_web-0.1.3/starlette_web/contrib/auth/apps.py
--rw-rw-rw-   0        0        0     4299 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/contrib/auth/backend.py
--rw-rw-rw-   0        0        0     3981 2023-03-25 08:05:10.000000 starlette_web-0.1.3/starlette_web/contrib/auth/hashers.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.266226 starlette_web-0.1.3/starlette_web/contrib/auth/management/
--rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/contrib/auth/management/__init__.py
--rw-rw-rw-   0        0        0     1308 2023-04-01 16:41:19.000000 starlette_web-0.1.3/starlette_web/contrib/auth/management/auth_command_mixin.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.267291 starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/
--rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-04-01 16:41:42.000000 starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/changepassword.py
--rw-rw-rw-   0        0        0     1459 2023-04-01 16:41:42.000000 starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/createsuperuser.py
--rw-rw-rw-   0        0        0     3192 2023-02-26 15:17:30.000000 starlette_web-0.1.3/starlette_web/contrib/auth/models.py
--rw-rw-rw-   0        0        0     3057 2023-03-18 20:17:51.000000 starlette_web-0.1.3/starlette_web/contrib/auth/password_validation.py
--rw-rw-rw-   0        0        0      624 2023-02-26 15:17:30.000000 starlette_web-0.1.3/starlette_web/contrib/auth/permissions.py
--rw-rw-rw-   0        0        0      654 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/contrib/auth/routes.py
--rw-rw-rw-   0        0        0     2724 2022-10-01 11:03:47.000000 starlette_web-0.1.3/starlette_web/contrib/auth/schemas.py
--rw-rw-rw-   0        0        0     1414 2023-03-18 20:17:51.000000 starlette_web-0.1.3/starlette_web/contrib/auth/utils.py
--rw-rw-rw-   0        0        0    18290 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/contrib/auth/views.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.267291 starlette_web-0.1.3/starlette_web/contrib/camel_case/
--rw-rw-rw-   0        0        0      249 2022-05-03 14:50:29.000000 starlette_web-0.1.3/starlette_web/contrib/camel_case/__init__.py
--rw-rw-rw-   0        0        0      389 2023-04-09 20:47:08.000000 starlette_web-0.1.3/starlette_web/contrib/camel_case/parser.py
--rw-rw-rw-   0        0        0      262 2022-05-03 14:50:29.000000 starlette_web-0.1.3/starlette_web/contrib/camel_case/renderer.py
--rw-rw-rw-   0        0        0     4103 2022-10-03 19:19:24.000000 starlette_web-0.1.3/starlette_web/contrib/camel_case/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.271291 starlette_web-0.1.3/starlette_web/contrib/constance/
--rw-rw-rw-   0        0        0     3754 2023-04-06 19:52:27.000000 starlette_web-0.1.3/starlette_web/contrib/constance/__init__.py
--rw-rw-rw-   0        0        0     1144 2023-04-06 20:13:04.000000 starlette_web-0.1.3/starlette_web/contrib/constance/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.271291 starlette_web-0.1.3/starlette_web/contrib/constance/backends/
--rw-rw-rw-   0        0        0        0 2023-02-20 07:01:30.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/__init__.py
--rw-rw-rw-   0        0        0     1410 2023-04-06 19:49:34.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/base.py
--rw-rw-rw-   0        0        0     1656 2023-04-06 20:18:43.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/caching_mixin.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.271291 starlette_web-0.1.3/starlette_web/contrib/constance/backends/database/
--rw-rw-rw-   0        0        0     1717 2023-03-12 16:44:01.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/database/__init__.py
--rw-rw-rw-   0        0        0      152 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/database/apps.py
--rw-rw-rw-   0        0        0      368 2023-03-12 16:44:01.000000 starlette_web-0.1.3/starlette_web/contrib/constance/backends/database/models.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.275292 starlette_web-0.1.3/starlette_web/contrib/postgres/
--rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/contrib/postgres/__init__.py
--rw-rw-rw-   0        0        0     3535 2023-04-02 10:14:34.000000 starlette_web-0.1.3/starlette_web/contrib/postgres/channel_layers.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.275292 starlette_web-0.1.3/starlette_web/contrib/redis/
--rw-rw-rw-   0        0        0      137 2022-05-14 13:30:44.000000 starlette_web-0.1.3/starlette_web/contrib/redis/__init__.py
--rw-rw-rw-   0        0        0     4616 2023-04-01 19:37:06.000000 starlette_web-0.1.3/starlette_web/contrib/redis/cache.py
--rw-rw-rw-   0        0        0     2261 2023-04-01 19:42:16.000000 starlette_web-0.1.3/starlette_web/contrib/redis/channel_layers.py
--rw-rw-rw-   0        0        0     1196 2023-03-27 18:37:04.000000 starlette_web-0.1.3/starlette_web/contrib/redis/redislock.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.279315 starlette_web-0.1.3/starlette_web/contrib/scheduler/
--rw-rw-rw-   0        0        0      133 2023-03-04 19:50:46.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/__init__.py
--rw-rw-rw-   0        0        0     2217 2023-03-04 19:50:46.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/app_settings.py
--rw-rw-rw-   0        0        0     2084 2023-04-03 20:00:17.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.283292 starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/
--rw-rw-rw-   0        0        0      843 2023-03-31 19:10:23.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/__init__.py
--rw-rw-rw-   0        0        0     3867 2023-04-09 17:22:30.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/base.py
--rw-rw-rw-   0        0        0     2629 2023-03-31 19:15:23.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/posix.py
--rw-rw-rw-   0        0        0     7287 2023-03-31 19:15:38.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/win32.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.283292 starlette_web-0.1.3/starlette_web/contrib/scheduler/management/
--rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.283292 starlette_web-0.1.3/starlette_web/contrib/scheduler/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1432 2023-03-31 19:14:46.000000 starlette_web-0.1.3/starlette_web/contrib/scheduler/management/commands/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.287316 starlette_web-0.1.3/starlette_web/contrib/staticfiles/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/staticfiles/__init__.py
--rw-rw-rw-   0        0        0      136 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/staticfiles/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.287316 starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.287316 starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/commands/
--rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/commands/__init__.py
--rw-rw-rw-   0        0        0     4229 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/commands/collectstatic.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.291318 starlette_web-0.1.3/starlette_web/tests/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.3/starlette_web/tests/__init__.py
--rw-rw-rw-   0        0        0      202 2023-03-03 17:32:15.000000 starlette_web-0.1.3/starlette_web/tests/apps.py
--rw-rw-rw-   0        0        0     5474 2023-04-06 20:04:06.000000 starlette_web-0.1.3/starlette_web/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.298777 starlette_web-0.1.3/starlette_web/tests/contrib/
--rw-rw-rw-   0        0        0        0 2022-05-03 14:50:29.000000 starlette_web-0.1.3/starlette_web/tests/contrib/__init__.py
--rw-rw-rw-   0        0        0    16572 2023-04-13 18:40:01.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_apispec.py
--rw-rw-rw-   0        0        0    27613 2023-03-30 19:24:14.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_auth.py
--rw-rw-rw-   0        0        0     1966 2022-05-03 14:50:29.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_camel_case.py
--rw-rw-rw-   0        0        0     7677 2023-04-05 19:51:46.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_channels.py
--rw-rw-rw-   0        0        0     1141 2023-04-06 19:30:04.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_constance.py
--rw-rw-rw-   0        0        0      994 2023-03-17 18:16:19.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_password_validators.py
--rw-rw-rw-   0        0        0     1410 2023-03-27 19:00:45.000000 starlette_web-0.1.3/starlette_web/tests/contrib/test_redis_cache.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.302780 starlette_web-0.1.3/starlette_web/tests/core/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.3/starlette_web/tests/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.302780 starlette_web-0.1.3/starlette_web/tests/core/helpers/
--rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.3/starlette_web/tests/core/helpers/__init__.py
--rw-rw-rw-   0        0        0     4350 2023-03-30 21:26:53.000000 starlette_web-0.1.3/starlette_web/tests/core/helpers/base_cache_tester.py
--rw-rw-rw-   0        0        0     5553 2023-02-26 15:17:30.000000 starlette_web-0.1.3/starlette_web/tests/core/test_auth_backends.py
--rw-rw-rw-   0        0        0     4741 2022-12-29 14:13:54.000000 starlette_web-0.1.3/starlette_web/tests/core/test_base.py
--rw-rw-rw-   0        0        0     1434 2023-03-27 18:28:47.000000 starlette_web-0.1.3/starlette_web/tests/core/test_base_caches.py
--rw-rw-rw-   0        0        0      867 2023-03-30 19:24:14.000000 starlette_web-0.1.3/starlette_web/tests/core/test_service.py
--rw-rw-rw-   0        0        0      528 2023-03-23 18:13:37.000000 starlette_web-0.1.3/starlette_web/tests/core/test_settings.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.302780 starlette_web-0.1.3/starlette_web/tests/database/
--rw-rw-rw-   0        0        0        0 2022-05-03 15:41:46.000000 starlette_web-0.1.3/starlette_web/tests/database/__init__.py
--rw-rw-rw-   0        0        0     4712 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/tests/database/test_model_mixin.py
--rw-rw-rw-   0        0        0     1786 2023-02-26 15:17:30.000000 starlette_web-0.1.3/starlette_web/tests/database/test_nested_transaction.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.306780 starlette_web-0.1.3/starlette_web/tests/files/
--rw-rw-rw-   0        0        0        0 2023-03-29 21:09:33.000000 starlette_web-0.1.3/starlette_web/tests/files/__init__.py
--rw-rw-rw-   0        0        0     4532 2023-03-31 18:52:29.000000 starlette_web-0.1.3/starlette_web/tests/files/test_filesystem_storage.py
--rw-rw-rw-   0        0        0      911 2023-03-30 20:24:14.000000 starlette_web-0.1.3/starlette_web/tests/files/test_media_storage.py
--rw-rw-rw-   0        0        0     3432 2023-02-26 14:23:54.000000 starlette_web-0.1.3/starlette_web/tests/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.175212 starlette_web-0.1.3/starlette_web/tests/management/
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.306780 starlette_web-0.1.3/starlette_web/tests/management/commands/
--rw-rw-rw-   0        0        0      287 2022-05-03 14:50:29.000000 starlette_web-0.1.3/starlette_web/tests/management/commands/test_call_command.py
--rw-rw-rw-   0        0        0     1229 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/tests/management/commands/test_channels_publisher.py
--rw-rw-rw-   0        0        0     1326 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/tests/management/commands/test_channels_subscriber.py
--rw-rw-rw-   0        0        0      672 2023-01-28 08:02:03.000000 starlette_web-0.1.3/starlette_web/tests/management/commands/test_db.py
--rw-rw-rw-   0        0        0      722 2023-03-26 10:31:10.000000 starlette_web-0.1.3/starlette_web/tests/management/commands/test_parser.py
--rw-rw-rw-   0        0        0     1089 2022-05-14 13:30:44.000000 starlette_web-0.1.3/starlette_web/tests/mocks.py
--rw-rw-rw-   0        0        0     1641 2023-04-13 18:29:48.000000 starlette_web-0.1.3/starlette_web/tests/routes.py
--rw-rw-rw-   0        0        0     4602 2023-04-14 17:40:22.000000 starlette_web-0.1.3/starlette_web/tests/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.314780 starlette_web-0.1.3/starlette_web/tests/utils/
--rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.3/starlette_web/tests/utils/__init__.py
--rw-rw-rw-   0        0        0     2960 2023-03-18 20:17:51.000000 starlette_web-0.1.3/starlette_web/tests/utils/test_auth_hasher.py
--rw-rw-rw-   0        0        0      768 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/tests/utils/test_json.py
--rw-rw-rw-   0        0        0     1447 2023-03-22 16:53:00.000000 starlette_web-0.1.3/starlette_web/tests/utils/test_redis_pattern_matcher.py
--rw-rw-rw-   0        0        0     1023 2022-05-09 11:25:06.000000 starlette_web-0.1.3/starlette_web/tests/utils/test_serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.314780 starlette_web-0.1.3/starlette_web/tests/views/
--rw-rw-rw-   0        0        0      375 2023-03-23 18:10:52.000000 starlette_web-0.1.3/starlette_web/tests/views/__init__.py
--rw-rw-rw-   0        0        0     2098 2023-03-23 18:10:52.000000 starlette_web-0.1.3/starlette_web/tests/views/http.py
--rw-rw-rw-   0        0        0     6847 2023-04-14 17:57:54.000000 starlette_web-0.1.3/starlette_web/tests/views/websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.318779 starlette_web-0.1.3/starlette_web/tests/websockets/
--rw-rw-rw-   0        0        0     2027 2023-03-12 16:44:21.000000 starlette_web-0.1.3/starlette_web/tests/websockets/test_websocket_chat.py
--rw-rw-rw-   0        0        0     7314 2023-03-15 20:43:06.000000 starlette_web-0.1.3/starlette_web/tests/websockets/test_websocket_endpoint.py
-drwxrwxrwx   0        0        0        0 2023-04-15 08:29:36.187313 starlette_web-0.1.3/starlette_web.egg-info/
--rw-rw-rw-   0        0        0     3430 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9083 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      933 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       73 2023-04-15 08:29:36.000000 starlette_web-0.1.3/starlette_web.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.789461 starlette_web-0.1.4/
+-rw-rw-rw-   0        0        0     1108 2023-04-15 07:48:43.000000 starlette_web-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      260 2023-04-18 20:41:36.000000 starlette_web-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3430 2023-04-18 20:55:02.789461 starlette_web-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2329 2023-03-26 13:41:03.000000 starlette_web-0.1.4/README.md
+-rw-rw-rw-   0        0        0     2383 2023-04-18 20:44:05.000000 starlette_web-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 20:55:02.789461 starlette_web-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.656257 starlette_web-0.1.4/starlette_web/
+-rw-rw-rw-   0        0        0       23 2022-12-29 14:13:54.000000 starlette_web-0.1.4/starlette_web/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.662159 starlette_web-0.1.4/starlette_web/common/
+-rw-rw-rw-   0        0        0       52 2022-04-25 19:06:18.000000 starlette_web-0.1.4/starlette_web/common/__init__.py
+-rw-rw-rw-   0        0        0     5348 2023-03-30 21:26:53.000000 starlette_web-0.1.4/starlette_web/common/app.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.662159 starlette_web-0.1.4/starlette_web/common/authorization/
+-rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.4/starlette_web/common/authorization/__init__.py
+-rw-rw-rw-   0        0        0      856 2023-03-25 08:05:20.000000 starlette_web-0.1.4/starlette_web/common/authorization/backends.py
+-rw-rw-rw-   0        0        0      329 2023-03-25 08:05:20.000000 starlette_web-0.1.4/starlette_web/common/authorization/base_user.py
+-rw-rw-rw-   0        0        0     3025 2023-03-25 08:05:20.000000 starlette_web-0.1.4/starlette_web/common/authorization/permissions.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.666186 starlette_web-0.1.4/starlette_web/common/caches/
+-rw-rw-rw-   0        0        0       80 2023-03-16 18:44:56.000000 starlette_web-0.1.4/starlette_web/common/caches/__init__.py
+-rw-rw-rw-   0        0        0     2162 2023-03-25 08:05:20.000000 starlette_web-0.1.4/starlette_web/common/caches/base.py
+-rw-rw-rw-   0        0        0     3342 2023-04-01 08:01:57.000000 starlette_web-0.1.4/starlette_web/common/caches/base_lock.py
+-rw-rw-rw-   0        0        0     1112 2023-03-16 18:44:56.000000 starlette_web-0.1.4/starlette_web/common/caches/cache_handler.py
+-rw-rw-rw-   0        0        0     5241 2023-03-24 16:47:56.000000 starlette_web-0.1.4/starlette_web/common/caches/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.670162 starlette_web-0.1.4/starlette_web/common/channels/
+-rw-rw-rw-   0        0        0       54 2023-03-12 16:44:21.000000 starlette_web-0.1.4/starlette_web/common/channels/__init__.py
+-rw-rw-rw-   0        0        0     4253 2023-04-01 19:06:23.000000 starlette_web-0.1.4/starlette_web/common/channels/base.py
+-rw-rw-rw-   0        0        0      447 2023-03-12 16:44:21.000000 starlette_web-0.1.4/starlette_web/common/channels/event.py
+-rw-rw-rw-   0        0        0      181 2023-03-22 16:38:31.000000 starlette_web-0.1.4/starlette_web/common/channels/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.674162 starlette_web-0.1.4/starlette_web/common/channels/layers/
+-rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.4/starlette_web/common/channels/layers/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-03-12 16:44:21.000000 starlette_web-0.1.4/starlette_web/common/channels/layers/base.py
+-rw-rw-rw-   0        0        0     1694 2023-03-12 19:30:41.000000 starlette_web-0.1.4/starlette_web/common/channels/layers/local_memory.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.674162 starlette_web-0.1.4/starlette_web/common/conf/
+-rw-rw-rw-   0        0        0     2285 2023-03-30 21:26:53.000000 starlette_web-0.1.4/starlette_web/common/conf/__init__.py
+-rw-rw-rw-   0        0        0     3314 2023-04-13 17:27:54.000000 starlette_web-0.1.4/starlette_web/common/conf/app_manager.py
+-rw-rw-rw-   0        0        0      198 2023-03-03 17:32:15.000000 starlette_web-0.1.4/starlette_web/common/conf/base_app_config.py
+-rw-rw-rw-   0        0        0     1994 2023-04-15 07:17:45.000000 starlette_web-0.1.4/starlette_web/common/conf/global_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.678186 starlette_web-0.1.4/starlette_web/common/database/
+-rw-rw-rw-   0        0        0      359 2022-05-09 11:25:06.000000 starlette_web-0.1.4/starlette_web/common/database/__init__.py
+-rw-rw-rw-   0        0        0     1362 2023-02-26 15:17:29.000000 starlette_web-0.1.4/starlette_web/common/database/columns.py
+-rw-rw-rw-   0        0        0       81 2022-05-09 11:25:06.000000 starlette_web-0.1.4/starlette_web/common/database/model_base.py
+-rw-rw-rw-   0        0        0     9279 2023-04-09 22:15:24.000000 starlette_web-0.1.4/starlette_web/common/database/model_mixin.py
+-rw-rw-rw-   0        0        0     1550 2023-02-17 20:43:07.000000 starlette_web-0.1.4/starlette_web/common/database/session_maker.py
+-rw-rw-rw-   0        0        0     2059 2023-02-18 12:47:03.000000 starlette_web-0.1.4/starlette_web/common/database/types.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.682186 starlette_web-0.1.4/starlette_web/common/email/
+-rw-rw-rw-   0        0        0      169 2022-05-22 18:14:32.000000 starlette_web-0.1.4/starlette_web/common/email/__init__.py
+-rw-rw-rw-   0        0        0     1604 2023-03-28 17:00:26.000000 starlette_web-0.1.4/starlette_web/common/email/base_sender.py
+-rw-rw-rw-   0        0        0     1770 2023-03-27 20:27:55.000000 starlette_web-0.1.4/starlette_web/common/email/email_manager.py
+-rw-rw-rw-   0        0        0     1728 2023-03-30 21:26:53.000000 starlette_web-0.1.4/starlette_web/common/email/smtp.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.682186 starlette_web-0.1.4/starlette_web/common/files/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.4/starlette_web/common/files/__init__.py
+-rw-rw-rw-   0        0        0     7085 2023-03-30 21:26:53.000000 starlette_web-0.1.4/starlette_web/common/files/cache.py
+-rw-rw-rw-   0        0        0     3837 2023-04-01 08:06:20.000000 starlette_web-0.1.4/starlette_web/common/files/filelock.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.686186 starlette_web-0.1.4/starlette_web/common/files/storages/
+-rw-rw-rw-   0        0        0      136 2023-03-30 20:24:14.000000 starlette_web-0.1.4/starlette_web/common/files/storages/__init__.py
+-rw-rw-rw-   0        0        0     6332 2023-03-31 18:48:34.000000 starlette_web-0.1.4/starlette_web/common/files/storages/base.py
+-rw-rw-rw-   0        0        0     4532 2023-04-01 16:31:26.000000 starlette_web-0.1.4/starlette_web/common/files/storages/filesystem.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.692629 starlette_web-0.1.4/starlette_web/common/http/
+-rw-rw-rw-   0        0        0        0 2022-05-03 08:01:50.000000 starlette_web-0.1.4/starlette_web/common/http/__init__.py
+-rw-rw-rw-   0        0        0     6297 2023-04-17 17:33:00.000000 starlette_web-0.1.4/starlette_web/common/http/base_endpoint.py
+-rw-rw-rw-   0        0        0     3782 2023-04-18 20:12:26.000000 starlette_web-0.1.4/starlette_web/common/http/exception_handlers.py
+-rw-rw-rw-   0        0        0     3329 2023-04-18 19:53:48.000000 starlette_web-0.1.4/starlette_web/common/http/exceptions.py
+-rw-rw-rw-   0        0        0     1075 2022-05-09 11:25:06.000000 starlette_web-0.1.4/starlette_web/common/http/renderers.py
+-rw-rw-rw-   0        0        0      336 2022-10-03 19:19:24.000000 starlette_web-0.1.4/starlette_web/common/http/responses.py
+-rw-rw-rw-   0        0        0     1009 2023-04-17 17:33:36.000000 starlette_web-0.1.4/starlette_web/common/http/schemas.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.692629 starlette_web-0.1.4/starlette_web/common/i18n/
+-rw-rw-rw-   0        0        0      163 2023-04-18 19:56:04.000000 starlette_web-0.1.4/starlette_web/common/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.692629 starlette_web-0.1.4/starlette_web/common/management/
+-rw-rw-rw-   0        0        0        0 2022-12-31 10:33:26.000000 starlette_web-0.1.4/starlette_web/common/management/__init__.py
+-rw-rw-rw-   0        0        0     1489 2023-04-15 07:46:58.000000 starlette_web-0.1.4/starlette_web/common/management/admin_util.py
+-rw-rw-rw-   0        0        0     1080 2023-04-06 12:18:07.000000 starlette_web-0.1.4/starlette_web/common/management/alembic_mixin.py
+-rw-rw-rw-   0        0        0     6023 2023-04-13 17:02:30.000000 starlette_web-0.1.4/starlette_web/common/management/base.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.696656 starlette_web-0.1.4/starlette_web/common/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-21 19:56:59.000000 starlette_web-0.1.4/starlette_web/common/management/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.700632 starlette_web-0.1.4/starlette_web/common/management/commands/_app_defaults/
+-rw-rw-rw-   0        0        0        0 2023-03-26 18:53:46.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_app_defaults/__init__.py
+-rw-rw-rw-   0        0        0      376 2023-03-26 18:59:14.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_app_defaults/admin.py
+-rw-rw-rw-   0        0        0      224 2023-03-26 18:55:02.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_app_defaults/apps.py
+-rw-rw-rw-   0        0        0      297 2023-03-26 18:59:20.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_app_defaults/models.py
+-rw-rw-rw-   0        0        0       95 2023-03-26 19:00:40.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_app_defaults/routes.py
+-rw-rw-rw-   0        0        0      154 2023-03-26 19:00:00.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_app_defaults/views.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.700632 starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/
+-rw-rw-rw-   0        0        0        0 2023-03-26 17:54:43.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/__init__.py
+-rw-rw-rw-   0        0        0      466 2023-04-03 20:19:20.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/asgi.py
+-rw-rw-rw-   0        0        0      896 2023-03-26 17:36:41.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/command.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.708661 starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/core/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/core/__init__.py
+-rw-rw-rw-   0        0        0      885 2023-04-13 18:30:43.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/core/routes.py
+-rw-rw-rw-   0        0        0     3354 2023-04-14 17:40:54.000000 starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/core/settings.py
+-rw-rw-rw-   0        0        0     1552 2023-04-06 16:46:50.000000 starlette_web-0.1.4/starlette_web/common/management/commands/makemigrations.py
+-rw-rw-rw-   0        0        0     1294 2023-04-06 16:46:56.000000 starlette_web-0.1.4/starlette_web/common/management/commands/migrate.py
+-rw-rw-rw-   0        0        0     2171 2023-03-30 21:26:53.000000 starlette_web-0.1.4/starlette_web/common/management/commands/startapp.py
+-rw-rw-rw-   0        0        0     3800 2023-04-06 16:47:27.000000 starlette_web-0.1.4/starlette_web/common/management/commands/startproject.py
+-rw-rw-rw-   0        0        0     2019 2023-04-08 06:35:50.000000 starlette_web-0.1.4/starlette_web/common/management/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.712794 starlette_web-0.1.4/starlette_web/common/utils/
+-rw-rw-rw-   0        0        0      506 2023-04-01 19:36:50.000000 starlette_web-0.1.4/starlette_web/common/utils/__init__.py
+-rw-rw-rw-   0        0        0     2578 2022-09-03 15:11:31.000000 starlette_web-0.1.4/starlette_web/common/utils/choices.py
+-rw-rw-rw-   0        0        0     1265 2023-03-18 14:43:23.000000 starlette_web-0.1.4/starlette_web/common/utils/crypto.py
+-rw-rw-rw-   0        0        0      187 2023-04-01 19:33:59.000000 starlette_web-0.1.4/starlette_web/common/utils/encoding.py
+-rw-rw-rw-   0        0        0      633 2023-02-17 20:46:29.000000 starlette_web-0.1.4/starlette_web/common/utils/importing.py
+-rw-rw-rw-   0        0        0      546 2023-03-30 21:26:53.000000 starlette_web-0.1.4/starlette_web/common/utils/inspect.py
+-rw-rw-rw-   0        0        0     2324 2022-05-09 11:25:06.000000 starlette_web-0.1.4/starlette_web/common/utils/json.py
+-rw-rw-rw-   0        0        0     2273 2023-03-30 21:26:53.000000 starlette_web-0.1.4/starlette_web/common/utils/regex.py
+-rw-rw-rw-   0        0        0     1828 2023-03-25 08:05:10.000000 starlette_web-0.1.4/starlette_web/common/utils/serializers.py
+-rw-rw-rw-   0        0        0      246 2022-05-09 11:25:06.000000 starlette_web-0.1.4/starlette_web/common/utils/singleton.py
+-rw-rw-rw-   0        0        0      217 2022-10-03 19:19:24.000000 starlette_web-0.1.4/starlette_web/common/utils/urls.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.712794 starlette_web-0.1.4/starlette_web/common/ws/
+-rw-rw-rw-   0        0        0        0 2022-12-29 14:13:54.000000 starlette_web-0.1.4/starlette_web/common/ws/__init__.py
+-rw-rw-rw-   0        0        0     6919 2023-03-14 17:15:47.000000 starlette_web-0.1.4/starlette_web/common/ws/base_endpoint.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.712794 starlette_web-0.1.4/starlette_web/contrib/
+-rw-rw-rw-   0        0        0        0 2022-05-09 11:25:06.000000 starlette_web-0.1.4/starlette_web/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.716826 starlette_web-0.1.4/starlette_web/contrib/admin/
+-rw-rw-rw-   0        0        0      185 2023-02-26 15:17:29.000000 starlette_web-0.1.4/starlette_web/contrib/admin/__init__.py
+-rw-rw-rw-   0        0        0     3705 2023-03-24 18:55:03.000000 starlette_web-0.1.4/starlette_web/contrib/admin/admin.py
+-rw-rw-rw-   0        0        0      564 2023-03-03 17:32:15.000000 starlette_web-0.1.4/starlette_web/contrib/admin/apps.py
+-rw-rw-rw-   0        0        0     2780 2023-02-26 15:17:29.000000 starlette_web-0.1.4/starlette_web/contrib/admin/auth_provider.py
+-rw-rw-rw-   0        0        0     5122 2023-03-18 20:17:51.000000 starlette_web-0.1.4/starlette_web/contrib/admin/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.724144 starlette_web-0.1.4/starlette_web/contrib/apispec/
+-rw-rw-rw-   0        0        0        0 2022-10-03 19:19:24.000000 starlette_web-0.1.4/starlette_web/contrib/apispec/__init__.py
+-rw-rw-rw-   0        0        0     2017 2023-04-03 20:01:29.000000 starlette_web-0.1.4/starlette_web/contrib/apispec/apps.py
+-rw-rw-rw-   0        0        0     5451 2023-03-03 17:32:15.000000 starlette_web-0.1.4/starlette_web/contrib/apispec/introspection.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.724144 starlette_web-0.1.4/starlette_web/contrib/apispec/marshmallow/
+-rw-rw-rw-   0        0        0      352 2022-10-03 19:19:24.000000 starlette_web-0.1.4/starlette_web/contrib/apispec/marshmallow/__init__.py
+-rw-rw-rw-   0        0        0     1545 2022-10-03 19:19:24.000000 starlette_web-0.1.4/starlette_web/contrib/apispec/marshmallow/converters.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.640226 starlette_web-0.1.4/starlette_web/contrib/apispec/static/
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.724144 starlette_web-0.1.4/starlette_web/contrib/apispec/static/apispec/
+-rw-rw-rw-   0        0        0   879592 2022-10-03 19:19:24.000000 starlette_web-0.1.4/starlette_web/contrib/apispec/static/apispec/redoc.js
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.644229 starlette_web-0.1.4/starlette_web/contrib/apispec/templates/
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.724144 starlette_web-0.1.4/starlette_web/contrib/apispec/templates/apispec/
+-rw-rw-rw-   0        0        0      539 2022-10-03 19:19:24.000000 starlette_web-0.1.4/starlette_web/contrib/apispec/templates/apispec/redoc.html
+-rw-rw-rw-   0        0        0     1889 2023-04-13 18:25:49.000000 starlette_web-0.1.4/starlette_web/contrib/apispec/views.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.731799 starlette_web-0.1.4/starlette_web/contrib/auth/
+-rw-rw-rw-   0        0        0        0 2023-04-13 17:15:05.000000 starlette_web-0.1.4/starlette_web/contrib/auth/__init__.py
+-rw-rw-rw-   0        0        0     3484 2023-02-26 16:10:52.000000 starlette_web-0.1.4/starlette_web/contrib/auth/admin.py
+-rw-rw-rw-   0        0        0      261 2023-03-17 18:16:19.000000 starlette_web-0.1.4/starlette_web/contrib/auth/apps.py
+-rw-rw-rw-   0        0        0     4299 2023-02-26 15:17:29.000000 starlette_web-0.1.4/starlette_web/contrib/auth/backend.py
+-rw-rw-rw-   0        0        0     3981 2023-03-25 08:05:10.000000 starlette_web-0.1.4/starlette_web/contrib/auth/hashers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.731799 starlette_web-0.1.4/starlette_web/contrib/auth/management/
+-rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.4/starlette_web/contrib/auth/management/__init__.py
+-rw-rw-rw-   0        0        0     1308 2023-04-01 16:41:19.000000 starlette_web-0.1.4/starlette_web/contrib/auth/management/auth_command_mixin.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.735793 starlette_web-0.1.4/starlette_web/contrib/auth/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-02-26 15:17:29.000000 starlette_web-0.1.4/starlette_web/contrib/auth/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-04-01 16:41:42.000000 starlette_web-0.1.4/starlette_web/contrib/auth/management/commands/changepassword.py
+-rw-rw-rw-   0        0        0     1459 2023-04-01 16:41:42.000000 starlette_web-0.1.4/starlette_web/contrib/auth/management/commands/createsuperuser.py
+-rw-rw-rw-   0        0        0     3192 2023-02-26 15:17:30.000000 starlette_web-0.1.4/starlette_web/contrib/auth/models.py
+-rw-rw-rw-   0        0        0     3057 2023-03-18 20:17:51.000000 starlette_web-0.1.4/starlette_web/contrib/auth/password_validation.py
+-rw-rw-rw-   0        0        0      624 2023-02-26 15:17:30.000000 starlette_web-0.1.4/starlette_web/contrib/auth/permissions.py
+-rw-rw-rw-   0        0        0      654 2022-05-09 11:25:06.000000 starlette_web-0.1.4/starlette_web/contrib/auth/routes.py
+-rw-rw-rw-   0        0        0     2724 2022-10-01 11:03:47.000000 starlette_web-0.1.4/starlette_web/contrib/auth/schemas.py
+-rw-rw-rw-   0        0        0     1414 2023-03-18 20:17:51.000000 starlette_web-0.1.4/starlette_web/contrib/auth/utils.py
+-rw-rw-rw-   0        0        0    18171 2023-04-17 18:32:16.000000 starlette_web-0.1.4/starlette_web/contrib/auth/views.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.739793 starlette_web-0.1.4/starlette_web/contrib/camel_case/
+-rw-rw-rw-   0        0        0      249 2022-05-03 14:50:29.000000 starlette_web-0.1.4/starlette_web/contrib/camel_case/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-04-09 20:47:08.000000 starlette_web-0.1.4/starlette_web/contrib/camel_case/parser.py
+-rw-rw-rw-   0        0        0      262 2022-05-03 14:50:29.000000 starlette_web-0.1.4/starlette_web/contrib/camel_case/renderer.py
+-rw-rw-rw-   0        0        0     4103 2022-10-03 19:19:24.000000 starlette_web-0.1.4/starlette_web/contrib/camel_case/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.739793 starlette_web-0.1.4/starlette_web/contrib/constance/
+-rw-rw-rw-   0        0        0     3754 2023-04-06 19:52:27.000000 starlette_web-0.1.4/starlette_web/contrib/constance/__init__.py
+-rw-rw-rw-   0        0        0     1144 2023-04-06 20:13:04.000000 starlette_web-0.1.4/starlette_web/contrib/constance/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.743817 starlette_web-0.1.4/starlette_web/contrib/constance/backends/
+-rw-rw-rw-   0        0        0        0 2023-02-20 07:01:30.000000 starlette_web-0.1.4/starlette_web/contrib/constance/backends/__init__.py
+-rw-rw-rw-   0        0        0     1410 2023-04-06 19:49:34.000000 starlette_web-0.1.4/starlette_web/contrib/constance/backends/base.py
+-rw-rw-rw-   0        0        0     1656 2023-04-06 20:18:43.000000 starlette_web-0.1.4/starlette_web/contrib/constance/backends/caching_mixin.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.743817 starlette_web-0.1.4/starlette_web/contrib/constance/backends/database/
+-rw-rw-rw-   0        0        0     1717 2023-03-12 16:44:01.000000 starlette_web-0.1.4/starlette_web/contrib/constance/backends/database/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-03-03 17:32:15.000000 starlette_web-0.1.4/starlette_web/contrib/constance/backends/database/apps.py
+-rw-rw-rw-   0        0        0      368 2023-03-12 16:44:01.000000 starlette_web-0.1.4/starlette_web/contrib/constance/backends/database/models.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.743817 starlette_web-0.1.4/starlette_web/contrib/postgres/
+-rw-rw-rw-   0        0        0        0 2023-03-12 16:44:21.000000 starlette_web-0.1.4/starlette_web/contrib/postgres/__init__.py
+-rw-rw-rw-   0        0        0     3535 2023-04-02 10:14:34.000000 starlette_web-0.1.4/starlette_web/contrib/postgres/channel_layers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.747817 starlette_web-0.1.4/starlette_web/contrib/redis/
+-rw-rw-rw-   0        0        0      137 2022-05-14 13:30:44.000000 starlette_web-0.1.4/starlette_web/contrib/redis/__init__.py
+-rw-rw-rw-   0        0        0     4616 2023-04-01 19:37:06.000000 starlette_web-0.1.4/starlette_web/contrib/redis/cache.py
+-rw-rw-rw-   0        0        0     2261 2023-04-01 19:42:16.000000 starlette_web-0.1.4/starlette_web/contrib/redis/channel_layers.py
+-rw-rw-rw-   0        0        0     1196 2023-03-27 18:37:04.000000 starlette_web-0.1.4/starlette_web/contrib/redis/redislock.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.751793 starlette_web-0.1.4/starlette_web/contrib/scheduler/
+-rw-rw-rw-   0        0        0      133 2023-03-04 19:50:46.000000 starlette_web-0.1.4/starlette_web/contrib/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     2217 2023-03-04 19:50:46.000000 starlette_web-0.1.4/starlette_web/contrib/scheduler/app_settings.py
+-rw-rw-rw-   0        0        0     2084 2023-04-03 20:00:17.000000 starlette_web-0.1.4/starlette_web/contrib/scheduler/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.751793 starlette_web-0.1.4/starlette_web/contrib/scheduler/backends/
+-rw-rw-rw-   0        0        0      843 2023-03-31 19:10:23.000000 starlette_web-0.1.4/starlette_web/contrib/scheduler/backends/__init__.py
+-rw-rw-rw-   0        0        0     3867 2023-04-09 17:22:30.000000 starlette_web-0.1.4/starlette_web/contrib/scheduler/backends/base.py
+-rw-rw-rw-   0        0        0     2629 2023-03-31 19:15:23.000000 starlette_web-0.1.4/starlette_web/contrib/scheduler/backends/posix.py
+-rw-rw-rw-   0        0        0     7287 2023-03-31 19:15:38.000000 starlette_web-0.1.4/starlette_web/contrib/scheduler/backends/win32.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.751793 starlette_web-0.1.4/starlette_web/contrib/scheduler/management/
+-rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.4/starlette_web/contrib/scheduler/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.755793 starlette_web-0.1.4/starlette_web/contrib/scheduler/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-04 19:50:46.000000 starlette_web-0.1.4/starlette_web/contrib/scheduler/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     1432 2023-03-31 19:14:46.000000 starlette_web-0.1.4/starlette_web/contrib/scheduler/management/commands/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.755793 starlette_web-0.1.4/starlette_web/contrib/staticfiles/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.4/starlette_web/contrib/staticfiles/__init__.py
+-rw-rw-rw-   0        0        0      136 2023-03-03 17:32:15.000000 starlette_web-0.1.4/starlette_web/contrib/staticfiles/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.755793 starlette_web-0.1.4/starlette_web/contrib/staticfiles/management/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.4/starlette_web/contrib/staticfiles/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.755793 starlette_web-0.1.4/starlette_web/contrib/staticfiles/management/commands/
+-rw-rw-rw-   0        0        0        0 2023-03-03 17:32:15.000000 starlette_web-0.1.4/starlette_web/contrib/staticfiles/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     4229 2023-03-03 17:32:15.000000 starlette_web-0.1.4/starlette_web/contrib/staticfiles/management/commands/collectstatic.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.759823 starlette_web-0.1.4/starlette_web/tests/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.4/starlette_web/tests/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-03-03 17:32:15.000000 starlette_web-0.1.4/starlette_web/tests/apps.py
+-rw-rw-rw-   0        0        0     5474 2023-04-06 20:04:06.000000 starlette_web-0.1.4/starlette_web/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.767824 starlette_web-0.1.4/starlette_web/tests/contrib/
+-rw-rw-rw-   0        0        0        0 2022-05-03 14:50:29.000000 starlette_web-0.1.4/starlette_web/tests/contrib/__init__.py
+-rw-rw-rw-   0        0        0    23210 2023-04-18 20:25:22.000000 starlette_web-0.1.4/starlette_web/tests/contrib/test_apispec.py
+-rw-rw-rw-   0        0        0    27132 2023-04-18 20:15:42.000000 starlette_web-0.1.4/starlette_web/tests/contrib/test_auth.py
+-rw-rw-rw-   0        0        0     1966 2022-05-03 14:50:29.000000 starlette_web-0.1.4/starlette_web/tests/contrib/test_camel_case.py
+-rw-rw-rw-   0        0        0     7677 2023-04-05 19:51:46.000000 starlette_web-0.1.4/starlette_web/tests/contrib/test_channels.py
+-rw-rw-rw-   0        0        0     1141 2023-04-06 19:30:04.000000 starlette_web-0.1.4/starlette_web/tests/contrib/test_constance.py
+-rw-rw-rw-   0        0        0      994 2023-03-17 18:16:19.000000 starlette_web-0.1.4/starlette_web/tests/contrib/test_password_validators.py
+-rw-rw-rw-   0        0        0     1410 2023-03-27 19:00:45.000000 starlette_web-0.1.4/starlette_web/tests/contrib/test_redis_cache.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.773459 starlette_web-0.1.4/starlette_web/tests/core/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.4/starlette_web/tests/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.773459 starlette_web-0.1.4/starlette_web/tests/core/helpers/
+-rw-rw-rw-   0        0        0        0 2023-03-22 16:53:00.000000 starlette_web-0.1.4/starlette_web/tests/core/helpers/__init__.py
+-rw-rw-rw-   0        0        0     4350 2023-03-30 21:26:53.000000 starlette_web-0.1.4/starlette_web/tests/core/helpers/base_cache_tester.py
+-rw-rw-rw-   0        0        0     5553 2023-02-26 15:17:30.000000 starlette_web-0.1.4/starlette_web/tests/core/test_auth_backends.py
+-rw-rw-rw-   0        0        0     4299 2023-04-18 20:15:24.000000 starlette_web-0.1.4/starlette_web/tests/core/test_base.py
+-rw-rw-rw-   0        0        0     1434 2023-03-27 18:28:47.000000 starlette_web-0.1.4/starlette_web/tests/core/test_base_caches.py
+-rw-rw-rw-   0        0        0      876 2023-04-17 18:43:14.000000 starlette_web-0.1.4/starlette_web/tests/core/test_service.py
+-rw-rw-rw-   0        0        0      528 2023-04-18 20:25:38.000000 starlette_web-0.1.4/starlette_web/tests/core/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.773459 starlette_web-0.1.4/starlette_web/tests/database/
+-rw-rw-rw-   0        0        0        0 2022-05-03 15:41:46.000000 starlette_web-0.1.4/starlette_web/tests/database/__init__.py
+-rw-rw-rw-   0        0        0     4712 2022-05-09 11:25:06.000000 starlette_web-0.1.4/starlette_web/tests/database/test_model_mixin.py
+-rw-rw-rw-   0        0        0     1786 2023-02-26 15:17:30.000000 starlette_web-0.1.4/starlette_web/tests/database/test_nested_transaction.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.777485 starlette_web-0.1.4/starlette_web/tests/files/
+-rw-rw-rw-   0        0        0        0 2023-03-29 21:09:33.000000 starlette_web-0.1.4/starlette_web/tests/files/__init__.py
+-rw-rw-rw-   0        0        0     4532 2023-03-31 18:52:29.000000 starlette_web-0.1.4/starlette_web/tests/files/test_filesystem_storage.py
+-rw-rw-rw-   0        0        0      911 2023-03-30 20:24:14.000000 starlette_web-0.1.4/starlette_web/tests/files/test_media_storage.py
+-rw-rw-rw-   0        0        0     3432 2023-02-26 14:23:54.000000 starlette_web-0.1.4/starlette_web/tests/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.648255 starlette_web-0.1.4/starlette_web/tests/management/
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.777485 starlette_web-0.1.4/starlette_web/tests/management/commands/
+-rw-rw-rw-   0        0        0      287 2022-05-03 14:50:29.000000 starlette_web-0.1.4/starlette_web/tests/management/commands/test_call_command.py
+-rw-rw-rw-   0        0        0     1229 2023-03-12 16:44:21.000000 starlette_web-0.1.4/starlette_web/tests/management/commands/test_channels_publisher.py
+-rw-rw-rw-   0        0        0     1326 2023-03-12 16:44:21.000000 starlette_web-0.1.4/starlette_web/tests/management/commands/test_channels_subscriber.py
+-rw-rw-rw-   0        0        0      672 2023-01-28 08:02:03.000000 starlette_web-0.1.4/starlette_web/tests/management/commands/test_db.py
+-rw-rw-rw-   0        0        0      722 2023-03-26 10:31:10.000000 starlette_web-0.1.4/starlette_web/tests/management/commands/test_parser.py
+-rw-rw-rw-   0        0        0     1089 2022-05-14 13:30:44.000000 starlette_web-0.1.4/starlette_web/tests/mocks.py
+-rw-rw-rw-   0        0        0     1641 2023-04-13 18:29:48.000000 starlette_web-0.1.4/starlette_web/tests/routes.py
+-rw-rw-rw-   0        0        0     4602 2023-04-14 17:40:22.000000 starlette_web-0.1.4/starlette_web/tests/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.785486 starlette_web-0.1.4/starlette_web/tests/utils/
+-rw-rw-rw-   0        0        0        0 2022-04-25 19:06:18.000000 starlette_web-0.1.4/starlette_web/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0     2960 2023-03-18 20:17:51.000000 starlette_web-0.1.4/starlette_web/tests/utils/test_auth_hasher.py
+-rw-rw-rw-   0        0        0      768 2022-05-09 11:25:06.000000 starlette_web-0.1.4/starlette_web/tests/utils/test_json.py
+-rw-rw-rw-   0        0        0     1447 2023-03-22 16:53:00.000000 starlette_web-0.1.4/starlette_web/tests/utils/test_redis_pattern_matcher.py
+-rw-rw-rw-   0        0        0     1023 2022-05-09 11:25:06.000000 starlette_web-0.1.4/starlette_web/tests/utils/test_serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.785486 starlette_web-0.1.4/starlette_web/tests/views/
+-rw-rw-rw-   0        0        0      375 2023-03-23 18:10:52.000000 starlette_web-0.1.4/starlette_web/tests/views/__init__.py
+-rw-rw-rw-   0        0        0     1912 2023-04-17 17:45:30.000000 starlette_web-0.1.4/starlette_web/tests/views/http.py
+-rw-rw-rw-   0        0        0     6847 2023-04-14 17:57:54.000000 starlette_web-0.1.4/starlette_web/tests/views/websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.785486 starlette_web-0.1.4/starlette_web/tests/websockets/
+-rw-rw-rw-   0        0        0     2027 2023-03-12 16:44:21.000000 starlette_web-0.1.4/starlette_web/tests/websockets/test_websocket_chat.py
+-rw-rw-rw-   0        0        0     7314 2023-03-15 20:43:06.000000 starlette_web-0.1.4/starlette_web/tests/websockets/test_websocket_endpoint.py
+drwxrwxrwx   0        0        0        0 2023-04-18 20:55:02.662159 starlette_web-0.1.4/starlette_web.egg-info/
+-rw-rw-rw-   0        0        0     3430 2023-04-18 20:55:02.000000 starlette_web-0.1.4/starlette_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9045 2023-04-18 20:55:02.000000 starlette_web-0.1.4/starlette_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 20:55:02.000000 starlette_web-0.1.4/starlette_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-04-18 20:55:02.000000 starlette_web-0.1.4/starlette_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      934 2023-04-18 20:55:02.000000 starlette_web-0.1.4/starlette_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       73 2023-04-18 20:55:02.000000 starlette_web-0.1.4/starlette_web.egg-info/top_level.txt
```

### Comparing `starlette_web-0.1.3/LICENSE` & `starlette_web-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/PKG-INFO` & `starlette_web-0.1.4/starlette_web.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: starlette_web
-Version: 0.1.3
+Name: starlette-web
+Version: 0.1.4
 Summary: Asynchronous web framework, based on Starlette and inspired by Django
 Author-email: Sergey Sayamov <dolamroth@mail.ru>, Dmitry Burnaev <dmitry.burnaev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/dolamroth/starlette-web
 Project-URL: Issues, https://github.com/dolamroth/starlette-web/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `starlette_web-0.1.3/README.md` & `starlette_web-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/pyproject.toml` & `starlette_web-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "starlette_web"
-version = "0.1.3"
+version = "0.1.4"
 description = "Asynchronous web framework, based on Starlette and inspired by Django"
 readme = "README.md"
 authors = [
     {name = "Sergey Sayamov", email = "dolamroth@mail.ru"},
     {name = "Dmitry Burnaev", email = "dmitry.burnaev@gmail.com"},
 ]
 license = { text = "MIT" }
@@ -56,15 +56,15 @@
     "openapi-spec-validator>=0.5.6,<0.6",
 ]
 admin = ["starlette-admin>=0.7.0,<0.9"]
 auth = ["PyJWT>=2.6,<2.7"]
 postgres = ["asyncpg>=0.27,<0.28"]
 redis = ["redis>=4.5.4,<4.6"]
 scheduler = [
-    "croniter>=1.3.8,<1.4",
+    "croniter>=1.3.14,<1.4",
     "py-win-task-scheduler==0.1.0; sys_platform == 'win32'",
 ]
 deploy = ["gunicorn>=20.1.0,<20.2"]
 develop = ["black~=22.10.0"]
 testing = [
     "pytest>=6.2,<6.3",
     "coverage>=6.2,<6.3",
```

### Comparing `starlette_web-0.1.3/starlette_web/common/app.py` & `starlette_web-0.1.4/starlette_web/common/app.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/authorization/backends.py` & `starlette_web-0.1.4/starlette_web/common/authorization/backends.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/authorization/permissions.py` & `starlette_web-0.1.4/starlette_web/common/authorization/permissions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/caches/base.py` & `starlette_web-0.1.4/starlette_web/common/caches/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/caches/base_lock.py` & `starlette_web-0.1.4/starlette_web/common/caches/base_lock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/caches/cache_handler.py` & `starlette_web-0.1.4/starlette_web/common/caches/cache_handler.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/caches/local_memory.py` & `starlette_web-0.1.4/starlette_web/common/caches/local_memory.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/channels/base.py` & `starlette_web-0.1.4/starlette_web/common/channels/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/channels/layers/base.py` & `starlette_web-0.1.4/starlette_web/common/channels/layers/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/channels/layers/local_memory.py` & `starlette_web-0.1.4/starlette_web/common/channels/layers/local_memory.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/conf/__init__.py` & `starlette_web-0.1.4/starlette_web/common/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/conf/app_manager.py` & `starlette_web-0.1.4/starlette_web/common/conf/app_manager.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/conf/global_settings.py` & `starlette_web-0.1.4/starlette_web/common/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/database/columns.py` & `starlette_web-0.1.4/starlette_web/common/database/columns.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/database/model_mixin.py` & `starlette_web-0.1.4/starlette_web/common/database/model_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/database/session_maker.py` & `starlette_web-0.1.4/starlette_web/common/database/session_maker.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/database/types.py` & `starlette_web-0.1.4/starlette_web/common/database/types.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/email/base_sender.py` & `starlette_web-0.1.4/starlette_web/common/email/base_sender.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/email/email_manager.py` & `starlette_web-0.1.4/starlette_web/common/email/email_manager.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/email/smtp.py` & `starlette_web-0.1.4/starlette_web/common/email/smtp.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/files/cache.py` & `starlette_web-0.1.4/starlette_web/common/files/cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/files/filelock.py` & `starlette_web-0.1.4/starlette_web/common/files/filelock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/files/storages/base.py` & `starlette_web-0.1.4/starlette_web/common/files/storages/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/files/storages/filesystem.py` & `starlette_web-0.1.4/starlette_web/common/files/storages/filesystem.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/http/base_endpoint.py` & `starlette_web-0.1.4/starlette_web/common/http/base_endpoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import sys
-from typing import Type, Union, Iterable, ClassVar, Optional, Mapping, List, Any, Dict
+from typing import Type, Union, Iterable, ClassVar, Optional, Mapping, List
 
 from marshmallow import Schema, ValidationError
 from sqlalchemy.ext.asyncio import AsyncSession
 from starlette import status
 from starlette.background import BackgroundTasks
 from starlette.exceptions import HTTPException
 from starlette.endpoints import HTTPEndpoint
@@ -22,15 +22,14 @@
 from starlette_web.common.http.exceptions import (
     UnexpectedError,
     BaseApplicationError,
     InvalidParameterError,
     PermissionDeniedError,
 )
 from starlette_web.common.http.renderers import BaseRenderer
-from starlette_web.common.http.statuses import ResponseStatus
 from starlette_web.common.database import DBModel
 from starlette_web.common.utils import import_string
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -139,15 +138,14 @@
 
         return cleaned_data
 
     def _response(
         self,
         data: Union[DBModel, Iterable[DBModel], dict] = None,
         status_code: int = status.HTTP_200_OK,
-        response_status: ResponseStatus = ResponseStatus.OK,
         headers: Mapping[str, str] = None,
         background: Optional[BackgroundTasks] = None,
     ) -> BaseRenderer:
         """
         A shorthand for response_renderer plus serializing data and passing text status.
         To be used primarily with JSONRenderer and such.
         """
@@ -157,16 +155,12 @@
                 schema_kwargs["many"] = True
 
             payload = self.response_schema(**schema_kwargs).dump(data)
         else:
             payload = data
 
         return self.response_renderer(
-            self._get_response_content(response_status, payload),
+            payload,
             status_code=status_code,
             headers=headers,
             background=background,
         )
-
-    @staticmethod
-    def _get_response_content(response_status: ResponseStatus, payload: Any) -> Dict:
-        return {"status": response_status, "payload": payload}
```

### Comparing `starlette_web-0.1.3/starlette_web/common/http/exception_handlers.py` & `starlette_web-0.1.4/starlette_web/common/http/exception_handlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
 import logging.config
 from typing import Any, Optional
 
-from starlette import status
+import httpx
 from starlette.requests import Request
 from starlette.responses import BackgroundTask
 from webargs_starlette import WebargsHTTPException
 
 from starlette_web.common.conf import settings
-from starlette_web.common.http.exceptions import BaseApplicationError
+from starlette_web.common.http.exceptions import (
+    BaseApplicationError,
+    InvalidParameterError,
+)
 from starlette_web.common.http.renderers import BaseRenderer, JSONRenderer
 from starlette_web.common.http.schemas import get_error_schema_class
-from starlette_web.common.http.statuses import ResponseStatus, status_is_server_error
 
 
 class BaseExceptionHandler:
     renderer_class: BaseRenderer = JSONRenderer
 
     def _log_message(self, exc: Exception, error_data: dict, level=logging.ERROR):
         logger = logging.getLogger(__name__)
@@ -30,37 +32,34 @@
     def _get_error_message(self, request: Request, exc: Exception) -> str:
         return "Something went wrong!"
 
     def _get_error_details(self, request: Request, exc: Exception) -> str:
         return f"Raised Error: {exc.__class__.__name__}"
 
     def _get_status_code(self, request: Request, exc: Exception) -> int:
-        return getattr(exc, "status_code", status.HTTP_500_INTERNAL_SERVER_ERROR)
-
-    def _get_response_status(self, request: Request, exc: Exception) -> str:
-        return ResponseStatus.INTERNAL_ERROR
+        return getattr(exc, "status_code", BaseApplicationError.message)
 
     def _get_response_data(self, request: Request, exc: Exception) -> Any:
-        error_message = self._get_error_message(request, exc)
-        response_status = self._get_response_status(request, exc)
+        _status_code = self._get_status_code(request, exc)
 
-        payload = {"error": error_message}
-        if settings.APP_DEBUG or response_status == ResponseStatus.INVALID_PARAMETERS:
+        payload = {
+            "error": self._get_error_message(request, exc),
+        }
+        if settings.APP_DEBUG or _status_code == InvalidParameterError.message:
             payload["details"] = self._get_error_details(request, exc)
 
         error_schema = get_error_schema_class()()
-        res = {"status": str(response_status), "payload": payload}
-        return error_schema.dump(res)
+        return error_schema.dump(payload)
 
     def _on_error_action(self, request: Request, exc: Exception):
         status_code = self._get_status_code(request, exc)
         error_message = self._get_error_message(request, exc)
         payload = {"error": error_message}
 
-        log_level = logging.ERROR if status_is_server_error(status_code) else logging.WARNING
+        log_level = logging.ERROR if httpx.codes.is_error(status_code) else logging.WARNING
         self._log_message(exc, payload, log_level)
 
     def _get_headers(self, request: Request, exc: Exception) -> Optional[dict]:
         return None
 
     def _get_background_tasks(self, request: Request, exc: Exception) -> Optional[BackgroundTask]:
         return None
@@ -79,23 +78,17 @@
 class BaseApplicationErrorHandler(BaseExceptionHandler):
     def _get_error_details(self, request: Request, exc: BaseApplicationError) -> str:
         return exc.details
 
     def _get_error_message(self, request: Request, exc: BaseApplicationError) -> str:
         return exc.message
 
-    def _get_response_status(self, request: Request, exc: BaseApplicationError) -> str:
-        return exc.response_status
-
 
 class WebargsHTTPExceptionHandler(BaseExceptionHandler):
     def _get_error_details(self, request: Request, exc: WebargsHTTPException):
         return exc.messages.get("json") or exc.messages.get("form") or exc.messages
 
     def _get_error_message(self, request: Request, exc: WebargsHTTPException) -> str:
-        return "Requested data is not valid."
-
-    def _get_response_status(self, request: Request, exc: WebargsHTTPException) -> str:
-        return ResponseStatus.INVALID_PARAMETERS
+        return InvalidParameterError.message
 
     def _get_status_code(self, request: Request, exc: Exception) -> int:
-        return status.HTTP_400_BAD_REQUEST
+        return InvalidParameterError.status_code
```

### Comparing `starlette_web-0.1.3/starlette_web/common/http/renderers.py` & `starlette_web-0.1.4/starlette_web/common/http/renderers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/http/schemas.py` & `starlette_web-0.1.4/starlette_web/common/http/schemas.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,24 +6,19 @@
 from starlette_web.common.http.exceptions import ImproperlyConfigured
 from starlette_web.common.utils import import_string
 
 
 __ERROR_RESPONSE_SCHEMA = None
 
 
-class ErrorDetailsSchema(Schema):
+class ErrorResponseSchema(Schema):
     error = fields.String(required=True, allow_none=False)
     details = fields.Raw(required=False, allow_none=True)
 
 
-class ErrorResponseSchema(Schema):
-    payload = fields.Nested(ErrorDetailsSchema, required=True)
-    status = fields.String(required=False, allow_none=False)
-
-
 def get_error_schema_class() -> Type[Schema]:
     global __ERROR_RESPONSE_SCHEMA
     if __ERROR_RESPONSE_SCHEMA is not None:
         return __ERROR_RESPONSE_SCHEMA
 
     try:
         __ERROR_RESPONSE_SCHEMA = import_string(settings.ERROR_RESPONSE_SCHEMA)
```

### Comparing `starlette_web-0.1.3/starlette_web/common/management/admin_util.py` & `starlette_web-0.1.4/starlette_web/common/management/admin_util.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/management/alembic_mixin.py` & `starlette_web-0.1.4/starlette_web/common/management/alembic_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/management/base.py` & `starlette_web-0.1.4/starlette_web/common/management/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/command.py` & `starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/command.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/routes.py` & `starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/core/routes.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/management/commands/_project_defaults/core/settings.py` & `starlette_web-0.1.4/starlette_web/common/management/commands/_project_defaults/core/settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/management/commands/makemigrations.py` & `starlette_web-0.1.4/starlette_web/common/management/commands/makemigrations.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/management/commands/migrate.py` & `starlette_web-0.1.4/starlette_web/common/management/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/management/commands/startapp.py` & `starlette_web-0.1.4/starlette_web/common/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/management/commands/startproject.py` & `starlette_web-0.1.4/starlette_web/common/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/management/utils.py` & `starlette_web-0.1.4/starlette_web/common/management/utils.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/utils/choices.py` & `starlette_web-0.1.4/starlette_web/common/utils/choices.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/utils/crypto.py` & `starlette_web-0.1.4/starlette_web/common/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/utils/importing.py` & `starlette_web-0.1.4/starlette_web/common/utils/importing.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/utils/inspect.py` & `starlette_web-0.1.4/starlette_web/common/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/utils/json.py` & `starlette_web-0.1.4/starlette_web/common/utils/json.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/utils/regex.py` & `starlette_web-0.1.4/starlette_web/common/utils/regex.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/utils/serializers.py` & `starlette_web-0.1.4/starlette_web/common/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/common/ws/base_endpoint.py` & `starlette_web-0.1.4/starlette_web/common/ws/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/admin/admin.py` & `starlette_web-0.1.4/starlette_web/contrib/admin/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/admin/apps.py` & `starlette_web-0.1.4/starlette_web/contrib/admin/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/admin/auth_provider.py` & `starlette_web-0.1.4/starlette_web/contrib/admin/auth_provider.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/admin/middleware.py` & `starlette_web-0.1.4/starlette_web/contrib/admin/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/apispec/apps.py` & `starlette_web-0.1.4/starlette_web/contrib/apispec/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/apispec/introspection.py` & `starlette_web-0.1.4/starlette_web/contrib/apispec/introspection.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/apispec/marshmallow/converters.py` & `starlette_web-0.1.4/starlette_web/contrib/apispec/marshmallow/converters.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/apispec/static/apispec/redoc.js` & `starlette_web-0.1.4/starlette_web/contrib/apispec/static/apispec/redoc.js`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/apispec/templates/apispec/redoc.html` & `starlette_web-0.1.4/starlette_web/contrib/apispec/templates/apispec/redoc.html`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/apispec/views.py` & `starlette_web-0.1.4/starlette_web/contrib/apispec/views.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/admin.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/backend.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/backend.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/hashers.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/hashers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/management/auth_command_mixin.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/management/auth_command_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/changepassword.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/management/commands/changepassword.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/management/commands/createsuperuser.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/management/commands/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/models.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/models.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/password_validation.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/password_validation.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/permissions.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/routes.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/routes.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/schemas.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/utils.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/utils.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/auth/views.py` & `starlette_web-0.1.4/starlette_web/contrib/auth/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 from datetime import datetime, timedelta
 from typing import Tuple, Optional, Union
 
 from sqlalchemy.ext.asyncio import AsyncSession
 from starlette import status
 
 from starlette_web.common.conf import settings
-from starlette_web.common.http.statuses import ResponseStatus
 from starlette_web.common.email import send_email, EmailSenderError
 from starlette_web.common.http.base_endpoint import BaseHTTPEndpoint
 from starlette_web.common.http.exceptions import (
     AuthenticationFailedError,
     InvalidParameterError,
     SendRequestError,
+    ConflictError,
+    UnprocessableEntityError,
 )
 from starlette_web.common.utils import get_random_string
 from starlette_web.contrib.auth.models import User, UserSession, UserInvite
 from starlette_web.contrib.auth.backend import JWTAuthenticationBackend
 from starlette_web.contrib.auth.permissions import IsSuperuserPermission
 from starlette_web.contrib.auth.utils import (
     encode_jwt,
@@ -129,22 +130,21 @@
         return self._response(token_collection)
 
     async def authenticate(self, email: str, password: str) -> User:
         user = await User.async_get(db_session=self.db_session, email=email, is_active__is=True)
         if not user:
             logger.info("Not found active user with email [%s]", email)
             raise AuthenticationFailedError(
-                "Not found active user with provided email.",
-                response_status=ResponseStatus.INVALID_PARAMETERS,
+                details="Not found active user with provided email.",
             )
 
         if not user.verify_password(password):
             logger.error("Password didn't verify: email: %s", email)
             raise AuthenticationFailedError(
-                "Email or password is invalid.", response_status=ResponseStatus.INVALID_PARAMETERS
+                details="Email or password is invalid.",
             )
 
         return user
 
 
 class SignUpAPIView(JWTSessionMixin, BaseHTTPEndpoint):
     """Allows creating new user and create his own session"""
@@ -181,15 +181,15 @@
         return self._response(token_collection, status_code=status.HTTP_201_CREATED)
 
     async def _validate(self, request, *_) -> dict:
         cleaned_data = (await super()._validate(request)) or dict()
         email = cleaned_data["email"]
 
         if await User.async_get(self.db_session, email=email):
-            raise InvalidParameterError(details=f"User with email '{email}' already exists")
+            raise ConflictError(details=f"User with email '{email}' already exists")
 
         user_invite = await UserInvite.async_get(
             self.db_session,
             token=cleaned_data["invite_token"],
             is_applied__is=False,
             expired_at__gt=datetime.utcnow(),
         )
@@ -197,15 +197,15 @@
         if not user_invite:
             details = "Invitation link is expired or unavailable"
             logger.error(
                 "Couldn't signup user token: %s | details: %s",
                 cleaned_data["invite_token"],
                 details,
             )
-            raise InvalidParameterError(details=details)
+            raise UnprocessableEntityError(details=details)
 
         if email != user_invite.email:
             raise InvalidParameterError(message="Email does not match with your invitation.")
 
         validate_password(cleaned_data["password_1"], User(email=email))
 
         cleaned_data["user_invite"] = user_invite
```

### Comparing `starlette_web-0.1.3/starlette_web/contrib/camel_case/utils.py` & `starlette_web-0.1.4/starlette_web/contrib/camel_case/utils.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/constance/__init__.py` & `starlette_web-0.1.4/starlette_web/contrib/constance/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/constance/apps.py` & `starlette_web-0.1.4/starlette_web/contrib/constance/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/constance/backends/base.py` & `starlette_web-0.1.4/starlette_web/contrib/constance/backends/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/constance/backends/caching_mixin.py` & `starlette_web-0.1.4/starlette_web/contrib/constance/backends/caching_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/constance/backends/database/__init__.py` & `starlette_web-0.1.4/starlette_web/contrib/constance/backends/database/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/postgres/channel_layers.py` & `starlette_web-0.1.4/starlette_web/contrib/postgres/channel_layers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/redis/cache.py` & `starlette_web-0.1.4/starlette_web/contrib/redis/cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/redis/channel_layers.py` & `starlette_web-0.1.4/starlette_web/contrib/redis/channel_layers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/redis/redislock.py` & `starlette_web-0.1.4/starlette_web/contrib/redis/redislock.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/scheduler/app_settings.py` & `starlette_web-0.1.4/starlette_web/contrib/scheduler/app_settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/scheduler/apps.py` & `starlette_web-0.1.4/starlette_web/contrib/scheduler/apps.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/__init__.py` & `starlette_web-0.1.4/starlette_web/contrib/scheduler/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/base.py` & `starlette_web-0.1.4/starlette_web/contrib/scheduler/backends/base.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/posix.py` & `starlette_web-0.1.4/starlette_web/contrib/scheduler/backends/posix.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/scheduler/backends/win32.py` & `starlette_web-0.1.4/starlette_web/contrib/scheduler/backends/win32.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/scheduler/management/commands/scheduler.py` & `starlette_web-0.1.4/starlette_web/contrib/scheduler/management/commands/scheduler.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/contrib/staticfiles/management/commands/collectstatic.py` & `starlette_web-0.1.4/starlette_web/contrib/staticfiles/management/commands/collectstatic.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/conftest.py` & `starlette_web-0.1.4/starlette_web/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/contrib/test_auth.py` & `starlette_web-0.1.4/starlette_web/tests/contrib/test_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import uuid
 from datetime import datetime, timedelta
 
 import pytest
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from starlette_web.common.conf import settings
-from starlette_web.common.http.statuses import ResponseStatus
 from starlette_web.contrib.auth.models import User, UserSession, UserInvite
 from starlette_web.contrib.auth.utils import (
     decode_jwt,
     encode_jwt,
     TOKEN_TYPE_RESET_PASSWORD,
     TOKEN_TYPE_REFRESH,
     TOKEN_TYPE_ACCESS,
@@ -122,15 +121,14 @@
         }
 
 
 class TestAuthSignInAPIView(BaseTestAPIView):
     url = "/api/auth/sign-in/"
     raw_password = "test-password"
     default_fail_status_code = 401
-    default_fail_response_status = ResponseStatus.INVALID_PARAMETERS
 
     @classmethod
     def setup_class(cls):
         cls.encoded_password = User.make_password(cls.raw_password)
 
     def setup_method(self):
         self.email = f"user_{uuid.uuid4().hex[:10]}@test.com"
@@ -230,15 +228,14 @@
             "details": "Not found active user with provided email.",
         }
 
 
 class TestAuthSignUPAPIView(BaseTestAPIView):
     url = "/api/auth/sign-up/"
     default_fail_status_code = 400
-    default_fail_response_status = ResponseStatus.INVALID_PARAMETERS
 
     @staticmethod
     def _sign_up_data(user_invite: UserInvite):
         return {
             "email": user_invite.email,
             "invite_token": user_invite.token,
             "password_1": "test-password",
@@ -264,17 +261,17 @@
 
     def test_sign_up__user_already_exists__fail(self, client, user_invite, dbs):
         request_data = self._sign_up_data(user_invite)
         user_email = request_data["email"]
 
         await_(User.async_create(dbs, db_commit=True, email=user_email, password="pass"))
         response = client.post(self.url, json=request_data)
-        response_data = self.assert_fail_response(response)
+        response_data = self.assert_fail_response(response, status_code=409)
         assert response_data == {
-            "error": "Requested data is not valid.",
+            "error": "Request conflicts with current state of server.",
             "details": f"User with email '{user_email}' already exists",
         }
 
     @pytest.mark.parametrize(
         "token_update_data",
         [
             {"token": f"outdated-token-{uuid.uuid4().hex[:10]}"},
@@ -283,17 +280,17 @@
         ],
     )
     def test_sign_up__token_problems__fail(self, client, user_invite, token_update_data, dbs):
         request_data = self._sign_up_data(user_invite)
         await_(user_invite.update(dbs, **token_update_data))
         await_(dbs.commit())
         response = client.post(self.url, json=request_data)
-        response_data = self.assert_fail_response(response)
+        response_data = self.assert_fail_response(response, status_code=422)
         assert response_data == {
-            "error": "Requested data is not valid.",
+            "error": "Could not process request due to logical errors in data.",
             "details": "Invitation link is expired or unavailable",
         }
 
     def test_sign_up__email_mismatch_with_token__fail(self, client, user_invite):
         request_data = self._sign_up_data(user_invite)
         request_data["email"] = f"another.email{uuid.uuid4().hex[:10]}@test.com"
         response = client.post(self.url, json=request_data)
@@ -316,15 +313,14 @@
         response = client.delete(self.url)
         assert response.status_code == 200
 
 
 class TestUserInviteApiView(BaseTestAPIView):
     url = "/api/auth/invite-user/"
     default_fail_status_code = 400
-    default_fail_response_status = ResponseStatus.INVALID_PARAMETERS
 
     def setup_method(self):
         self.email = f"user_{uuid.uuid4().hex[:10]}@test.com"
 
     def test_invite__ok(self, client, user, mocked_auth_send, dbs):
         client.login(user)
         response = client.post(self.url, json={"email": self.email})
@@ -445,50 +441,47 @@
         request_user = user
         await_(request_user.update(dbs, is_superuser=True))
         await_(dbs.commit())
 
         client.login(request_user)
         response = client.post(self.url, json={"email": "fake-email@test.com"})
         response_data = self.assert_fail_response(
-            response, status_code=400, response_status=ResponseStatus.INVALID_PARAMETERS
+            response, status_code=400,
         )
         assert response_data == {
             "error": "Requested data is not valid.",
             "details": "User with email=[fake-email@test.com] not found.",
         }
 
     def test_reset_password__user_is_not_superuser__fail(self, client, user):
         client.login(user)
         response = client.post(self.url, json={"email": user.email})
         response_data = self.assert_fail_response(
-            response, status_code=403, response_status=ResponseStatus.FORBIDDEN
+            response, status_code=403,
         )
         assert response_data == {
-            "error": "You don't have permission to perform this action.",
+            "error": "You do not have permission to perform this action.",
             "details": "You don't have an admin privileges.",
         }
 
 
 class TestChangePasswordAPIView(BaseTestAPIView):
     url = "/api/auth/change-password/"
     new_password = "new123456"
 
-    def _assert_fail_response(self, client, token: str, response_status: str = None) -> dict:
+    def _assert_fail_response(self, client, token: str) -> dict:
         request_data = {
             "token": token,
             "password_1": self.new_password,
             "password_2": self.new_password,
         }
         client.logout()
         response = client.post(self.url, json=request_data)
         assert response.status_code == 401
-        response_data = response.json()
-        if response_status:
-            assert response_data["status"] == response_status
-        return response.json()["payload"]
+        return response.json()
 
     def test_change_password__ok(self, client, user, user_session, dbs):
         token, _ = encode_jwt(
             {"user_id": user.id, "session_id": user_session.public_id},
             token_type=TOKEN_TYPE_RESET_PASSWORD,
         )
         request_data = {
@@ -507,16 +500,20 @@
     @pytest.mark.parametrize("invalid_data, error_details", INVALID_CHANGE_PASSWORD_DATA)
     def test_invalid_request__fail(self, client, invalid_data: dict, error_details: dict):
         client.logout()
         self.assert_bad_request(client.post(self.url, json=invalid_data), error_details)
 
     def test__token_expired__fail(self, client, user):
         token, _ = encode_jwt({"user_id": user.id}, expires_in=-10)
-        response_data = self._assert_fail_response(client, token, ResponseStatus.SIGNATURE_EXPIRED)
-        self.assert_auth_invalid(response_data, "JWT signature has been expired for token")
+        response_data = self._assert_fail_response(client, token)
+        self.assert_auth_invalid(
+            response_data,
+            "JWT signature has been expired for token",
+            message="Authentication credentials have expired.",
+        )
 
     def test__token_invalid_type__fail(self, client, user):
         token, _ = encode_jwt({"user_id": user.id}, token_type=TOKEN_TYPE_REFRESH)
         response_data = self._assert_fail_response(client, token)
         self.assert_auth_invalid(
             response_data, "Token type 'reset_password' expected, got 'refresh' instead."
         )
@@ -612,30 +609,28 @@
         )
         self.assert_auth_invalid(response, expected_msg)
 
     @pytest.mark.parametrize("token_type", [TOKEN_TYPE_ACCESS, TOKEN_TYPE_RESET_PASSWORD])
     def test_refresh_token__token_not_refresh__fail(self, client, user, token_type):
         refresh_token, _ = encode_jwt({"user_id": user.id}, token_type=token_type)
         response = client.post(self.url, json={"refresh_token": refresh_token})
-        response_data = self.assert_fail_response(
-            response, status_code=401, response_status=ResponseStatus.AUTH_FAILED
-        )
+        response_data = self.assert_fail_response(response, status_code=401)
         assert response_data == {
             "error": "Authentication credentials are invalid.",
             "details": f"Token type 'refresh' expected, got '{token_type}' instead.",
         }
 
     def test_refresh_token__token_mismatch__fail(self, client, user, dbs):
         user_session = self._prepare_token(dbs, user, is_active=True)
         refresh_token = user_session.refresh_token
         await_(user_session.update(dbs, refresh_token="fake-token"))
         await_(dbs.commit())
         response = client.post(self.url, json={"refresh_token": refresh_token})
         self.assert_auth_invalid(
-            response, "Refresh token does not match with user session.", ResponseStatus.AUTH_FAILED
+            response, "Refresh token does not match with user session.",
         )
 
     def test_refresh_token__fake_jwt__fail(self, client, user):
         response = client.post(self.url, json={"refresh_token": "fake-jwt-token"})
         self.assert_auth_invalid(response, "Token could not be decoded: Not enough segments")
 
     @pytest.mark.parametrize("invalid_data, error_details", INVALID_REFRESH_TOKEN_DATA)
```

### Comparing `starlette_web-0.1.3/starlette_web/tests/contrib/test_camel_case.py` & `starlette_web-0.1.4/starlette_web/tests/contrib/test_camel_case.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/contrib/test_channels.py` & `starlette_web-0.1.4/starlette_web/tests/contrib/test_channels.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/contrib/test_constance.py` & `starlette_web-0.1.4/starlette_web/tests/contrib/test_constance.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/contrib/test_password_validators.py` & `starlette_web-0.1.4/starlette_web/tests/contrib/test_password_validators.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/contrib/test_redis_cache.py` & `starlette_web-0.1.4/starlette_web/tests/contrib/test_redis_cache.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/core/helpers/base_cache_tester.py` & `starlette_web-0.1.4/starlette_web/tests/core/helpers/base_cache_tester.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/core/test_auth_backends.py` & `starlette_web-0.1.4/starlette_web/tests/core/test_auth_backends.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/core/test_base.py` & `starlette_web-0.1.4/starlette_web/tests/core/test_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 from typing import Union, Optional
 
 from httpx import Response
 from starlette.testclient import TestClient
 
+from starlette_web.common.database.model_base import ModelBase
 from starlette_web.contrib.auth.views import JWTSessionMixin
 from starlette_web.contrib.auth.models import UserSession
-from starlette_web.common.database.model_base import ModelBase
-from starlette_web.common.http.statuses import ResponseStatus
 
 
 class BaseTestCase:
     @staticmethod
     def assert_called_with(mock_callable, *args, **kwargs):
         """Check mock object (callable) on call action with provided `args`, `kwargs`"""
 
@@ -23,85 +22,82 @@
             assert key in mock_call_args.kwargs, mock_call_args.kwargs
             assert mock_call_args.kwargs[key] == value
 
 
 class BaseTestAPIView(BaseTestCase):
     url: str = NotImplemented
     default_fail_status_code = 500
-    default_fail_response_status = ResponseStatus.INTERNAL_ERROR
 
     @staticmethod
     def assert_ok_response(response: Response, status_code: int = 200) -> Union[dict, list]:
         assert response.status_code == status_code
 
         try:
             response_data = response.json()
         except Exception:
             raise AssertionError(response.text)
 
-        assert "payload" in response_data, response_data
-        assert response_data["status"] == ResponseStatus.OK
-        return response_data["payload"]
+        assert "error" not in response_data, response_data
+        return response_data
 
     def assert_fail_response(
-        self, response: Response, status_code: int = None, response_status: str = None
+        self, response: Response, status_code: int = None,
     ) -> Union[dict, list]:
 
         response_data = response.json()
         assert response.status_code == (status_code or self.default_fail_status_code)
-        assert "payload" in response_data, response_data
-        assert response_data["status"] == (response_status or self.default_fail_response_status)
-        return response_data["payload"]
+        assert "error" in response_data, response_data
+        assert "details" in response_data, response_data
+        return response_data
 
     @staticmethod
     def assert_bad_request(response: Response, error_details: dict):
         response_data = response.json()
         assert response.status_code == 400
-        assert "payload" in response_data, response_data
-        response_data = response_data["payload"]
-        assert response_data["error"] == "Requested data is not valid."
+        assert "error" in response_data, response_data
+        assert "details" in response_data, response_data
+        assert response_data["error"] in "Requested data is not valid."
+
         for error_field, error_value in error_details.items():
             assert error_field in response_data["details"]
             assert error_value in response_data["details"][error_field]
 
     @staticmethod
     def assert_not_found(response: Response, instance: ModelBase):
         assert response.status_code == 404
         response_data = response.json()
-        assert response_data["status"] == ResponseStatus.NOT_FOUND
-        assert response_data["payload"] == {
+        assert response_data == {
             "error": "Requested object not found.",
             "details": (
                 f"{instance.__class__.__name__} #{instance.id} "
                 f"does not exist or belongs to another user"
             ),
         }
 
     def assert_unauth(self, response: Response):
-        response_data = self.assert_fail_response(
-            response, status_code=401, response_status=ResponseStatus.MISSED_CREDENTIALS
-        )
+        response_data = self.assert_fail_response(response, status_code=401)
         assert response_data == {
             "error": "Authentication is required.",
             "details": "Invalid token header. No credentials provided.",
         }
 
     def assert_auth_invalid(
         self,
         response_data: Union[Response, dict],
         details: Optional[str],
-        response_status=ResponseStatus.AUTH_FAILED,
+        message: Optional[str] = None,
     ):
         if isinstance(response_data, Response):
-            response_data = self.assert_fail_response(
-                response_data, status_code=401, response_status=response_status
-            )
+            response_data = self.assert_fail_response(response_data, status_code=401)
+
+        if message is None:
+            message = "Authentication credentials are invalid."
 
         assert response_data == {
-            "error": "Authentication credentials are invalid.",
+            "error": message,
             "details": details,
         }
 
 
 class BaseTestWSAPI(BaseTestCase):
     url: str = NotImplemented
```

### Comparing `starlette_web-0.1.3/starlette_web/tests/core/test_base_caches.py` & `starlette_web-0.1.4/starlette_web/tests/core/test_base_caches.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/core/test_service.py` & `starlette_web-0.1.4/starlette_web/tests/core/test_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,12 +11,14 @@
         response_data = self.assert_ok_response(response)
         assert response_data == {"services": {"postgres": "ok"}, "errors": []}
 
     @patch("starlette_web.common.database.ModelMixin.async_filter")
     def test_health__fail(self, mock_filter, client):
         mock_filter.side_effect = RuntimeError("Oops")
         response = client.get(self.url)
-        response_data = self.assert_fail_response(response, status_code=503)
+
+        response_data = response.json()
+        assert response.status_code == 503
         assert response_data == {
             "services": {"postgres": "down"},
             "errors": ["Couldn't connect to DB: RuntimeError 'Oops'"],
         }
```

### Comparing `starlette_web-0.1.3/starlette_web/tests/core/test_settings.py` & `starlette_web-0.1.4/starlette_web/tests/core/test_settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/database/test_model_mixin.py` & `starlette_web-0.1.4/starlette_web/tests/database/test_model_mixin.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/database/test_nested_transaction.py` & `starlette_web-0.1.4/starlette_web/tests/database/test_nested_transaction.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/files/test_filesystem_storage.py` & `starlette_web-0.1.4/starlette_web/tests/files/test_filesystem_storage.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/files/test_media_storage.py` & `starlette_web-0.1.4/starlette_web/tests/files/test_media_storage.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/helpers.py` & `starlette_web-0.1.4/starlette_web/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/management/commands/test_channels_publisher.py` & `starlette_web-0.1.4/starlette_web/tests/management/commands/test_channels_publisher.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/management/commands/test_channels_subscriber.py` & `starlette_web-0.1.4/starlette_web/tests/management/commands/test_channels_subscriber.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/management/commands/test_db.py` & `starlette_web-0.1.4/starlette_web/tests/management/commands/test_db.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/management/commands/test_parser.py` & `starlette_web-0.1.4/starlette_web/tests/management/commands/test_parser.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/mocks.py` & `starlette_web-0.1.4/starlette_web/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/routes.py` & `starlette_web-0.1.4/starlette_web/tests/routes.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/settings.py` & `starlette_web-0.1.4/starlette_web/tests/settings.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/utils/test_auth_hasher.py` & `starlette_web-0.1.4/starlette_web/tests/utils/test_auth_hasher.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/utils/test_json.py` & `starlette_web-0.1.4/starlette_web/tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/utils/test_redis_pattern_matcher.py` & `starlette_web-0.1.4/starlette_web/tests/utils/test_redis_pattern_matcher.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/utils/test_serializers.py` & `starlette_web-0.1.4/starlette_web/tests/utils/test_serializers.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/views/websocket.py` & `starlette_web-0.1.4/starlette_web/tests/views/websocket.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/websockets/test_websocket_chat.py` & `starlette_web-0.1.4/starlette_web/tests/websockets/test_websocket_chat.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web/tests/websockets/test_websocket_endpoint.py` & `starlette_web-0.1.4/starlette_web/tests/websockets/test_websocket_endpoint.py`

 * *Files identical despite different names*

### Comparing `starlette_web-0.1.3/starlette_web.egg-info/PKG-INFO` & `starlette_web-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: starlette-web
-Version: 0.1.3
+Name: starlette_web
+Version: 0.1.4
 Summary: Asynchronous web framework, based on Starlette and inspired by Django
 Author-email: Sergey Sayamov <dolamroth@mail.ru>, Dmitry Burnaev <dmitry.burnaev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/dolamroth/starlette-web
 Project-URL: Issues, https://github.com/dolamroth/starlette-web/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `starlette_web-0.1.3/starlette_web.egg-info/SOURCES.txt` & `starlette_web-0.1.4/starlette_web.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 starlette_web/common/http/__init__.py
 starlette_web/common/http/base_endpoint.py
 starlette_web/common/http/exception_handlers.py
 starlette_web/common/http/exceptions.py
 starlette_web/common/http/renderers.py
 starlette_web/common/http/responses.py
 starlette_web/common/http/schemas.py
-starlette_web/common/http/statuses.py
 starlette_web/common/i18n/__init__.py
 starlette_web/common/management/__init__.py
 starlette_web/common/management/admin_util.py
 starlette_web/common/management/alembic_mixin.py
 starlette_web/common/management/base.py
 starlette_web/common/management/utils.py
 starlette_web/common/management/commands/__init__.py
```

### Comparing `starlette_web-0.1.3/starlette_web.egg-info/requires.txt` & `starlette_web-0.1.4/starlette_web.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 [postgres]
 asyncpg<0.28,>=0.27
 
 [redis]
 redis<4.6,>=4.5.4
 
 [scheduler]
-croniter<1.4,>=1.3.8
+croniter<1.4,>=1.3.14
 
 [scheduler:sys_platform == "win32"]
 py-win-task-scheduler==0.1.0
 
 [testing]
 pytest<6.3,>=6.2
 coverage<6.3,>=6.2
```

