# Comparing `tmp/lnhub_rest-0.7rc1.tar.gz` & `tmp/lnhub_rest-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnhub_rest-0.7rc1.tar", last modified: Wed Mar 29 10:58:59 2023, max compression
+gzip compressed data, was "lnhub_rest-0.8.1.tar", last modified: Tue Apr 18 16:22:44 2023, max compression
```

## Comparing `lnhub_rest-0.7rc1.tar` & `lnhub_rest-0.8.1.tar`

### file list

```diff
@@ -1,126 +1,224 @@
--rw-r--r--   0        0        0     1259 2023-02-13 09:20:16.808732 lnhub_rest-0.7rc1/.dockerignore
--rw-r--r--   0        0        0     2724 2023-03-08 16:14:44.728272 lnhub_rest-0.7rc1/.github/workflows/build.yml
--rw-r--r--   0        0        0     4871 2023-03-29 09:08:29.674856 lnhub_rest-0.7rc1/.github/workflows/google-cloudrun-docker.yml
--rw-r--r--   0        0        0      133 2022-12-05 16:31:02.016205 lnhub_rest-0.7rc1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      613 2023-03-08 16:14:44.728725 lnhub_rest-0.7rc1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1212 2023-03-08 16:14:44.728869 lnhub_rest-0.7rc1/.gitignore
--rw-r--r--   0        0        0     1772 2023-03-02 11:17:31.745149 lnhub_rest-0.7rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      134 2023-03-08 16:14:44.728986 lnhub_rest-0.7rc1/Dockerfile
--rw-r--r--   0        0        0     1149 2023-03-29 09:08:29.675283 lnhub_rest-0.7rc1/README.md
--rw-r--r--   0        0        0    12677 2023-02-13 09:20:16.809717 lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-2efe1dee9baf.svg
--rw-r--r--   0        0        0    16617 2023-03-08 16:14:44.729168 lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-a88f5298b8f7.svg
--rw-r--r--   0        0        0    13696 2023-02-13 09:20:16.809873 lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-c13c9dd0f3ae.svg
--rw-r--r--   0        0        0    12677 2023-02-13 09:20:16.809956 lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-e7151581f790.svg
--rw-r--r--   0        0        0    15062 2023-02-13 09:20:16.810073 lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-e7eef9775586.svg
--rw-r--r--   0        0        0    14594 2023-02-13 09:20:16.810196 lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-f2cb77148a6e.svg
--rw-r--r--   0        0        0    12677 2023-02-13 09:20:16.810300 lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-f7ba9352c706.svg
--rw-r--r--   0        0        0    14594 2023-02-13 09:20:16.810415 lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-fe962c9a0ae7.svg
--rw-r--r--   0        0        0     5302 2023-03-14 16:02:39.647880 lnhub_rest-0.7rc1/docs/account/01-signup-signin.ipynb
--rw-r--r--   0        0        0     4484 2023-03-14 16:02:39.645047 lnhub_rest-0.7rc1/docs/account/02-create-account.ipynb
--rw-r--r--   0        0        0     5600 2023-03-14 16:02:39.643723 lnhub_rest-0.7rc1/docs/account/03-update-account.ipynb
--rw-r--r--   0        0        0     6188 2023-03-14 16:02:39.646649 lnhub_rest-0.7rc1/docs/account/04-fetch-account.ipynb
--rw-r--r--   0        0        0     9826 2023-03-14 16:02:39.646731 lnhub_rest-0.7rc1/docs/account/05-rls.ipynb
--rw-r--r--   0        0        0    19381 2023-03-29 10:55:16.837446 lnhub_rest-0.7rc1/docs/changelog.md
--rw-r--r--   0        0        0     1299 2023-03-15 11:16:45.486458 lnhub_rest-0.7rc1/docs/checks/01-check-break-lndb.ipynb
--rw-r--r--   0        0        0       69 2023-02-13 09:20:16.810963 lnhub_rest-0.7rc1/docs/content.md
--rw-r--r--   0        0        0    11226 2023-03-14 16:02:39.646645 lnhub_rest-0.7rc1/docs/instance/01-init-instance.ipynb
--rw-r--r--   0        0        0     5286 2023-03-15 11:18:07.148653 lnhub_rest-0.7rc1/docs/instance/02-load-instance.ipynb
--rw-r--r--   0        0        0     6187 2023-03-14 16:02:39.643793 lnhub_rest-0.7rc1/docs/instance/03-update-instance.ipynb
--rw-r--r--   0        0        0     7063 2023-03-29 10:50:51.815991 lnhub_rest-0.7rc1/docs/instance/04-delete-instance.ipynb
--rw-r--r--   0        0        0     7023 2023-03-29 10:50:51.816594 lnhub_rest-0.7rc1/docs/instance/05-fetch-instance.ipynb
--rw-r--r--   0        0        0    19524 2023-03-29 10:50:58.291610 lnhub_rest-0.7rc1/docs/instance/06-rls.ipynb
--rw-r--r--   0        0        0     6881 2023-03-29 10:50:58.291810 lnhub_rest-0.7rc1/docs/migration/01-migration.ipynb
--rw-r--r--   0        0        0      520 2023-03-02 11:17:31.746920 lnhub_rest-0.7rc1/docs/migrations.md
--rw-r--r--   0        0        0      162 2023-03-02 11:17:31.748210 lnhub_rest-0.7rc1/docs/notes/index.md
--rw-r--r--   0        0        0    26218 2023-03-08 16:14:44.732401 lnhub_rest-0.7rc1/docs/notes/multiple-sign-ups-same-email.ipynb
--rw-r--r--   0        0        0     3866 2023-03-14 16:02:39.643530 lnhub_rest-0.7rc1/docs/storage/01-add-storage.ipynb
--rw-r--r--   0        0        0     9665 2023-03-14 16:02:39.644130 lnhub_rest-0.7rc1/docs/storage/02-rls.ipynb
--rw-r--r--   0        0        0      137 2022-12-05 16:31:02.018378 lnhub_rest-0.7rc1/lamin-project.yaml
--rw-r--r--   0        0        0      226 2023-03-29 10:55:19.550099 lnhub_rest-0.7rc1/lnhub_rest/__init__.py
--rw-r--r--   0        0        0     8143 2023-03-29 10:50:51.817381 lnhub_rest-0.7rc1/lnhub_rest/__main__.py
--rw-r--r--   0        0        0       59 2023-03-08 16:14:44.733412 lnhub_rest-0.7rc1/lnhub_rest/_add_storage.py
--rw-r--r--   0        0        0       64 2023-02-13 09:20:16.812158 lnhub_rest-0.7rc1/lnhub_rest/_assets/__init__.py
--rw-r--r--   0        0        0     1026 2023-02-13 09:20:16.812240 lnhub_rest-0.7rc1/lnhub_rest/_assets/_instances.py
--rw-r--r--   0        0        0     1094 2023-02-13 09:20:16.812323 lnhub_rest-0.7rc1/lnhub_rest/_assets/_schemas.py
--rw-r--r--   0        0        0     1628 2023-03-13 07:50:24.229781 lnhub_rest-0.7rc1/lnhub_rest/_check_breaks_lndb.py
--rw-r--r--   0        0        0     5375 2023-03-08 16:14:44.733769 lnhub_rest-0.7rc1/lnhub_rest/_clean_ci.py
--rw-r--r--   0        0        0       64 2023-03-08 16:14:44.733916 lnhub_rest-0.7rc1/lnhub_rest/_delete_instance.py
--rw-r--r--   0        0        0       45 2023-03-08 16:14:44.734007 lnhub_rest-0.7rc1/lnhub_rest/_engine.py
--rw-r--r--   0        0        0       62 2023-03-08 16:14:44.734105 lnhub_rest-0.7rc1/lnhub_rest/_init_instance.py
--rw-r--r--   0        0        0       62 2023-03-08 16:14:44.734189 lnhub_rest-0.7rc1/lnhub_rest/_load_instance.py
--rw-r--r--   0        0        0       90 2023-02-13 09:20:16.813123 lnhub_rest-0.7rc1/lnhub_rest/_models.py
--rw-r--r--   0        0        0       47 2023-03-08 16:14:44.734275 lnhub_rest-0.7rc1/lnhub_rest/_sbclient.py
--rw-r--r--   0        0        0       61 2023-03-08 16:14:44.734361 lnhub_rest-0.7rc1/lnhub_rest/_signup_signin.py
--rw-r--r--   0        0        0       42 2023-03-08 16:14:44.734489 lnhub_rest-0.7rc1/lnhub_rest/core/__init__.py
--rw-r--r--   0        0        0      251 2023-03-08 16:14:44.734790 lnhub_rest-0.7rc1/lnhub_rest/core/account/__init__.py
--rw-r--r--   0        0        0     1207 2023-03-08 16:14:44.734878 lnhub_rest-0.7rc1/lnhub_rest/core/account/_create_account.py
--rw-r--r--   0        0        0     1062 2023-03-08 16:14:44.734978 lnhub_rest-0.7rc1/lnhub_rest/core/account/_crud.py
--rw-r--r--   0        0        0      735 2023-03-08 16:14:44.735141 lnhub_rest-0.7rc1/lnhub_rest/core/account/_delete_account.py
--rw-r--r--   0        0        0     3314 2023-03-24 15:16:03.675096 lnhub_rest-0.7rc1/lnhub_rest/core/account/_signup_signin.py
--rw-r--r--   0        0        0     1419 2023-03-08 16:14:44.735288 lnhub_rest-0.7rc1/lnhub_rest/core/account/_update_account.py
--rw-r--r--   0        0        0       38 2023-03-29 10:50:58.291948 lnhub_rest-0.7rc1/lnhub_rest/core/collaborator/__init__.py
--rw-r--r--   0        0        0     2710 2023-03-29 10:50:58.292258 lnhub_rest-0.7rc1/lnhub_rest/core/collaborator/_crud.py
--rw-r--r--   0        0        0      243 2023-03-08 16:14:44.735569 lnhub_rest-0.7rc1/lnhub_rest/core/instance/__init__.py
--rw-r--r--   0        0        0     1651 2023-03-13 13:43:06.983275 lnhub_rest-0.7rc1/lnhub_rest/core/instance/_crud.py
--rw-r--r--   0        0        0     1440 2023-03-29 10:50:58.292588 lnhub_rest-0.7rc1/lnhub_rest/core/instance/_delete_instance.py
--rw-r--r--   0        0        0     6477 2023-03-08 16:14:44.735785 lnhub_rest-0.7rc1/lnhub_rest/core/instance/_init_instance.py
--rw-r--r--   0        0        0     1528 2023-03-15 11:18:07.150180 lnhub_rest-0.7rc1/lnhub_rest/core/instance/_load_instance.py
--rw-r--r--   0        0        0     1063 2023-03-29 09:08:29.676385 lnhub_rest-0.7rc1/lnhub_rest/core/instance/_update_instance.py
--rw-r--r--   0        0        0       80 2023-03-08 16:14:44.735963 lnhub_rest-0.7rc1/lnhub_rest/core/storage/__init__.py
--rw-r--r--   0        0        0     2775 2023-03-08 16:14:44.736240 lnhub_rest-0.7rc1/lnhub_rest/core/storage/_add_storage.py
--rw-r--r--   0        0        0     1167 2023-03-08 16:14:44.736339 lnhub_rest-0.7rc1/lnhub_rest/core/storage/_crud.py
--rw-r--r--   0        0        0      742 2023-03-08 16:14:44.736544 lnhub_rest-0.7rc1/lnhub_rest/main.py
--rw-r--r--   0        0        0       11 2023-03-08 16:14:44.736622 lnhub_rest-0.7rc1/lnhub_rest/orm/__init__.py
--rw-r--r--   0        0        0      224 2023-03-08 16:14:44.736695 lnhub_rest-0.7rc1/lnhub_rest/orm/_engine.py
--rw-r--r--   0        0        0     2380 2023-03-29 09:46:37.463552 lnhub_rest-0.7rc1/lnhub_rest/orm/_sbclient.py
--rw-r--r--   0        0        0      157 2023-03-08 16:14:44.736894 lnhub_rest-0.7rc1/lnhub_rest/routers/__init__.py
--rw-r--r--   0        0        0     2724 2023-03-13 07:50:24.229941 lnhub_rest-0.7rc1/lnhub_rest/routers/account.py
--rw-r--r--   0        0        0      538 2023-03-08 16:14:44.737254 lnhub_rest-0.7rc1/lnhub_rest/routers/ci.py
--rw-r--r--   0        0        0      408 2023-03-08 16:14:44.737389 lnhub_rest-0.7rc1/lnhub_rest/routers/dev.py
--rw-r--r--   0        0        0     4397 2023-03-29 09:08:29.676776 lnhub_rest-0.7rc1/lnhub_rest/routers/instance.py
--rw-r--r--   0        0        0     1079 2023-03-08 16:14:44.737615 lnhub_rest-0.7rc1/lnhub_rest/routers/utils.py
--rw-r--r--   0        0        0      245 2023-03-29 10:50:58.292912 lnhub_rest-0.7rc1/lnhub_rest/schema/__init__.py
--rw-r--r--   0        0        0     3925 2023-03-20 08:26:20.388108 lnhub_rest-0.7rc1/lnhub_rest/schema/_core.py
--rw-r--r--   0        0        0      270 2023-03-02 11:17:31.752043 lnhub_rest-0.7rc1/lnhub_rest/schema/_timestamps.py
--rw-r--r--   0        0        0      252 2023-03-02 11:17:31.752112 lnhub_rest-0.7rc1/lnhub_rest/schema/_users.py
--rw-r--r--   0        0        0     1079 2023-03-02 11:17:31.752187 lnhub_rest-0.7rc1/lnhub_rest/schema/_versions.py
--rw-r--r--   0        0        0      674 2023-02-13 09:20:16.814087 lnhub_rest-0.7rc1/lnhub_rest/schema/alembic.ini
--rw-r--r--   0        0        0       48 2023-02-13 09:20:16.814178 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/__init__.py
--rw-r--r--   0        0        0     2977 2023-03-08 16:14:44.737843 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/env.py
--rw-r--r--   0        0        0     1193 2023-03-13 07:50:24.230447 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0       39 2023-03-13 07:50:24.230571 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/function/__init__.py
--rw-r--r--   0        0        0     3940 2023-03-13 07:50:24.230771 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
--rw-r--r--   0        0        0      639 2023-03-24 15:20:21.151607 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
--rw-r--r--   0        0        0      222 2023-03-29 10:50:58.293165 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
--rw-r--r--   0        0        0       33 2023-03-13 07:50:24.230894 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/rls/__init__.py
--rw-r--r--   0        0        0      542 2023-02-13 09:20:16.814349 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/script.py.mako
--rw-r--r--   0        0        0      757 2023-03-08 16:14:44.737944 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/settings.py
--rw-r--r--   0        0        0      170 2023-02-13 09:20:16.814484 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/utils.py
--rw-r--r--   0        0        0     1816 2023-02-13 09:20:16.814592 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-13-53709f2a2043-v0_0_1a.py
--rw-r--r--   0        0        0      935 2023-02-13 09:20:16.814670 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-13-c555c87a640c-v0_0_1.py
--rw-r--r--   0        0        0     5052 2023-02-13 09:20:16.814754 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-14-f7ba9352c706-v0_0_2.py
--rw-r--r--   0        0        0     1401 2023-02-13 09:20:16.814833 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-23-c13c9dd0f3ae-v0_1_4a.py
--rw-r--r--   0        0        0      536 2023-02-13 09:20:16.814901 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-24-e7151581f790-v0_1_4b.py
--rw-r--r--   0        0        0      512 2023-02-13 09:20:16.814968 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-30-2efe1dee9baf-v0_1_4c.py
--rw-r--r--   0        0        0      667 2023-02-13 09:20:16.815042 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-06-95073282294e-v0_1_4e.py
--rw-r--r--   0        0        0      869 2023-02-13 09:20:16.815111 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-06-9c02109e4faa-v0_2_0.py
--rw-r--r--   0        0        0     2190 2023-02-13 09:20:16.815184 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-06-f2cb77148a6e-v0_1_4d.py
--rw-r--r--   0        0        0      458 2023-02-13 09:20:16.815255 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-08-e7eef9775586-0_2_1.py
--rw-r--r--   0        0        0     1220 2023-03-02 11:17:31.752307 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-15-641d1508baab-v0_4_0.py
--rw-r--r--   0        0        0      624 2023-03-02 11:17:31.752395 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
--rw-r--r--   0        0        0      918 2023-03-13 07:50:24.231076 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
--rw-r--r--   0        0        0      575 2023-03-24 15:20:21.152374 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
--rw-r--r--   0        0        0      558 2023-03-29 10:50:58.293373 lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
--rw-r--r--   0        0        0       60 2023-03-02 11:17:31.752459 lnhub_rest-0.7rc1/lnhub_rest/schema/versions.py
--rw-r--r--   0        0        0      171 2023-03-08 16:14:44.738113 lnhub_rest-0.7rc1/lnhub_rest/utils/__init__.py
--rw-r--r--   0        0        0      212 2023-03-08 16:14:44.738175 lnhub_rest-0.7rc1/lnhub_rest/utils/_access_token.py
--rw-r--r--   0        0        0      259 2023-03-08 16:14:44.738231 lnhub_rest-0.7rc1/lnhub_rest/utils/_id.py
--rw-r--r--   0        0        0      109 2023-03-08 16:14:44.738291 lnhub_rest-0.7rc1/lnhub_rest/utils/_query.py
--rw-r--r--   0        0        0     3803 2023-03-24 15:16:03.676926 lnhub_rest-0.7rc1/lnhub_rest/utils/_test.py
--rw-r--r--   0        0        0     1111 2023-03-29 09:08:29.677007 lnhub_rest-0.7rc1/noxfile.py
--rw-r--r--   0        0        0     1302 2023-03-24 15:16:03.677102 lnhub_rest-0.7rc1/pyproject.toml
--rwxr-xr-x   0        0        0       29 2023-03-08 16:14:44.738954 lnhub_rest-0.7rc1/scripts/run.sh
--rw-r--r--   0        0        0       27 2023-03-02 11:17:31.752828 lnhub_rest-0.7rc1/supabase/.gitignore
--rw-r--r--   0        0        0     2548 2023-03-02 11:17:31.752925 lnhub_rest-0.7rc1/supabase/config.toml
--rw-r--r--   0        0        0      760 2023-03-13 07:50:24.231725 lnhub_rest-0.7rc1/tests/test_notebooks.py
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 lnhub_rest-0.7rc1/PKG-INFO
+-rw-r--r--   0        0        0     1259 2023-01-15 12:17:52.329263 lnhub_rest-0.8.1/.dockerignore
+-rw-r--r--   0        0        0     3217 2023-04-18 16:21:04.417331 lnhub_rest-0.8.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     5087 2023-04-18 16:02:04.937394 lnhub_rest-0.8.1/.github/workflows/google-cloudrun-docker.yml
+-rw-r--r--   0        0        0      133 2023-01-15 12:17:52.329501 lnhub_rest-0.8.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      613 2023-04-18 16:02:04.937767 lnhub_rest-0.8.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1212 2023-04-18 16:02:04.938015 lnhub_rest-0.8.1/.gitignore
+-rw-r--r--   0        0        0       73 2023-04-18 16:02:04.938253 lnhub_rest-0.8.1/.gitmodules
+-rw-r--r--   0        0        0     1772 2023-04-18 16:02:04.938593 lnhub_rest-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      157 2023-04-18 16:02:04.938840 lnhub_rest-0.8.1/Dockerfile
+-rw-r--r--   0        0        0     1149 2023-04-18 16:21:04.417682 lnhub_rest-0.8.1/README.md
+-rw-r--r--   0        0        0    12677 2023-04-18 16:21:04.417854 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-2efe1dee9baf.svg
+-rw-r--r--   0        0        0    16617 2023-04-18 16:21:04.418149 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-a88f5298b8f7.svg
+-rw-r--r--   0        0        0    13696 2023-04-18 16:21:04.418591 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-c13c9dd0f3ae.svg
+-rw-r--r--   0        0        0    12677 2023-04-18 16:21:04.418734 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-e7151581f790.svg
+-rw-r--r--   0        0        0    15062 2023-04-18 16:21:04.419104 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-e7eef9775586.svg
+-rw-r--r--   0        0        0    14594 2023-04-18 16:21:04.419540 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-f2cb77148a6e.svg
+-rw-r--r--   0        0        0    12677 2023-04-18 16:21:04.419648 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-f7ba9352c706.svg
+-rw-r--r--   0        0        0    14594 2023-04-18 16:21:04.419768 lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-fe962c9a0ae7.svg
+-rw-r--r--   0        0        0     5302 2023-04-18 16:02:04.940153 lnhub_rest-0.8.1/docs/account/01-signup-signin.ipynb
+-rw-r--r--   0        0        0     4559 2023-04-18 16:02:04.940245 lnhub_rest-0.8.1/docs/account/02-create-account.ipynb
+-rw-r--r--   0        0        0     5606 2023-04-18 16:02:04.940348 lnhub_rest-0.8.1/docs/account/03-update-account.ipynb
+-rw-r--r--   0        0        0     6182 2023-04-18 16:02:04.940428 lnhub_rest-0.8.1/docs/account/04-fetch-account.ipynb
+-rw-r--r--   0        0        0     9084 2023-04-18 16:02:04.940536 lnhub_rest-0.8.1/docs/account/05-rls.ipynb
+-rw-r--r--   0        0        0    21465 2023-04-18 16:22:13.686823 lnhub_rest-0.8.1/docs/changelog.md
+-rw-r--r--   0        0        0     1299 2023-04-18 16:02:04.941369 lnhub_rest-0.8.1/docs/checks/01-check-break-lndb.ipynb
+-rw-r--r--   0        0        0       69 2023-04-18 16:21:04.419847 lnhub_rest-0.8.1/docs/content.md
+-rw-r--r--   0        0        0    11226 2023-04-18 16:02:04.941781 lnhub_rest-0.8.1/docs/instance/01-init-instance.ipynb
+-rw-r--r--   0        0        0     5286 2023-04-18 16:02:04.942110 lnhub_rest-0.8.1/docs/instance/02-load-instance.ipynb
+-rw-r--r--   0        0        0     6191 2023-04-18 16:02:04.942208 lnhub_rest-0.8.1/docs/instance/03-update-instance.ipynb
+-rw-r--r--   0        0        0     8663 2023-04-18 16:02:04.942323 lnhub_rest-0.8.1/docs/instance/04-delete-instance.ipynb
+-rw-r--r--   0        0        0     6993 2023-04-18 16:02:04.942408 lnhub_rest-0.8.1/docs/instance/05-fetch-instance.ipynb
+-rw-r--r--   0        0        0    19485 2023-04-18 16:02:04.942491 lnhub_rest-0.8.1/docs/instance/06-rls.ipynb
+-rw-r--r--   0        0        0     2065 2023-04-18 16:21:04.420117 lnhub_rest-0.8.1/docs/migration/01-migration.ipynb
+-rw-r--r--   0        0        0      520 2023-04-18 16:02:04.943225 lnhub_rest-0.8.1/docs/migrations.md
+-rw-r--r--   0        0        0      162 2023-04-18 16:02:04.943589 lnhub_rest-0.8.1/docs/notes/index.md
+-rw-r--r--   0        0        0    26418 2023-04-18 16:02:04.943698 lnhub_rest-0.8.1/docs/notes/multiple-sign-ups-same-email.ipynb
+-rw-r--r--   0        0        0     3875 2023-04-18 16:02:04.943815 lnhub_rest-0.8.1/docs/organization/01-create-organization.ipynb
+-rw-r--r--   0        0        0     3999 2023-04-18 16:02:04.943880 lnhub_rest-0.8.1/docs/organization/02-manage-members.ipynb
+-rw-r--r--   0        0        0     5888 2023-04-18 16:02:04.944098 lnhub_rest-0.8.1/docs/organization/03-rls.ipynb
+-rw-r--r--   0        0        0     3866 2023-04-18 16:02:04.944372 lnhub_rest-0.8.1/docs/storage/01-add-storage.ipynb
+-rw-r--r--   0        0        0     9833 2023-04-18 16:02:04.944483 lnhub_rest-0.8.1/docs/storage/02-rls.ipynb
+-rw-r--r--   0        0        0      137 2023-01-15 12:17:52.330365 lnhub_rest-0.8.1/lamin-project.yaml
+-rw-r--r--   0        0        0     3832 2023-04-18 13:35:36.828846 lnhub_rest-0.8.1/lndb/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-14 19:46:06.422201 lnhub_rest-0.8.1/lndb/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-14 19:46:06.422302 lnhub_rest-0.8.1/lndb/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-03-14 19:46:06.422406 lnhub_rest-0.8.1/lndb/.gitignore
+-rw-r--r--   0        0        0     1772 2023-03-14 19:46:06.422493 lnhub_rest-0.8.1/lndb/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-14 19:46:06.422598 lnhub_rest-0.8.1/lndb/LICENSE
+-rw-r--r--   0        0        0      173 2023-03-30 17:54:41.276204 lnhub_rest-0.8.1/lndb/README.md
+-rw-r--r--   0        0        0       52 2023-03-14 19:46:06.422755 lnhub_rest-0.8.1/lndb/docs/api.md
+-rw-r--r--   0        0        0    45851 2023-04-18 13:35:36.829219 lnhub_rest-0.8.1/lndb/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-03-14 19:46:06.423210 lnhub_rest-0.8.1/lndb/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-03-14 19:46:06.423317 lnhub_rest-0.8.1/lndb/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-03-30 17:54:41.276594 lnhub_rest-0.8.1/lndb/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-03-30 17:54:41.276682 lnhub_rest-0.8.1/lndb/docs/faq/index.md
+-rw-r--r--   0        0        0     1180 2023-04-18 13:35:36.829371 lnhub_rest-0.8.1/lndb/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-03-14 19:46:06.423689 lnhub_rest-0.8.1/lndb/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-18 13:35:36.829492 lnhub_rest-0.8.1/lndb/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-18 13:35:36.829617 lnhub_rest-0.8.1/lndb/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-03-30 17:54:41.277018 lnhub_rest-0.8.1/lndb/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    10679 2023-04-18 13:35:36.829735 lnhub_rest-0.8.1/lndb/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5573 2023-03-30 17:54:41.277206 lnhub_rest-0.8.1/lndb/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     5290 2023-03-14 19:46:06.424075 lnhub_rest-0.8.1/lndb/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3724 2023-03-30 17:54:41.277308 lnhub_rest-0.8.1/lndb/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-03-30 17:54:41.277655 lnhub_rest-0.8.1/lndb/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     3282 2023-03-30 17:54:41.277763 lnhub_rest-0.8.1/lndb/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-03-14 19:46:06.424331 lnhub_rest-0.8.1/lndb/docs/guide/index.md
+-rw-r--r--   0        0        0     3152 2023-03-30 17:54:41.277866 lnhub_rest-0.8.1/lndb/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-03-14 19:46:06.424475 lnhub_rest-0.8.1/lndb/docs/index.md
+-rw-r--r--   0        0        0      118 2023-03-14 19:46:06.424531 lnhub_rest-0.8.1/lndb/lamin-project.yaml
+-rw-r--r--   0        0        0     1932 2023-04-18 13:35:36.829834 lnhub_rest-0.8.1/lndb/lndb/__init__.py
+-rw-r--r--   0        0        0     4242 2023-03-14 19:46:06.424708 lnhub_rest-0.8.1/lndb/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-03-14 19:46:06.424805 lnhub_rest-0.8.1/lndb/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-18 13:35:36.829911 lnhub_rest-0.8.1/lndb/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      216 2023-04-18 13:35:36.830020 lnhub_rest-0.8.1/lndb/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-18 13:35:36.830147 lnhub_rest-0.8.1/lndb/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-18 13:35:36.830259 lnhub_rest-0.8.1/lndb/lndb/_delete.py
+-rw-r--r--   0        0        0      222 2023-03-14 19:46:06.425064 lnhub_rest-0.8.1/lndb/lndb/_info.py
+-rw-r--r--   0        0        0     5710 2023-04-18 13:35:36.830369 lnhub_rest-0.8.1/lndb/lndb/_init_instance.py
+-rw-r--r--   0        0        0     3980 2023-04-18 13:35:36.830476 lnhub_rest-0.8.1/lndb/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-18 13:35:36.830566 lnhub_rest-0.8.1/lndb/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-18 13:35:36.830658 lnhub_rest-0.8.1/lndb/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3469 2023-04-18 13:35:36.830722 lnhub_rest-0.8.1/lndb/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     6303 2023-04-18 13:35:36.830802 lnhub_rest-0.8.1/lndb/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-03-14 19:46:06.425623 lnhub_rest-0.8.1/lndb/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      341 2023-03-14 19:46:06.425679 lnhub_rest-0.8.1/lndb/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-18 13:35:36.830883 lnhub_rest-0.8.1/lndb/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0     1020 2023-03-14 19:46:06.425742 lnhub_rest-0.8.1/lndb/lndb/_schema.py
+-rw-r--r--   0        0        0     1493 2023-04-18 13:35:36.830975 lnhub_rest-0.8.1/lndb/lndb/_set.py
+-rw-r--r--   0        0        0     2181 2023-04-18 13:35:36.831075 lnhub_rest-0.8.1/lndb/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-03-14 19:46:06.425940 lnhub_rest-0.8.1/lndb/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-03-14 19:46:06.426016 lnhub_rest-0.8.1/lndb/lndb/_settings_store.py
+-rw-r--r--   0        0        0     4927 2023-04-18 13:35:36.831210 lnhub_rest-0.8.1/lndb/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-18 13:35:36.831323 lnhub_rest-0.8.1/lndb/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-03-30 17:54:41.279075 lnhub_rest-0.8.1/lndb/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-18 13:35:36.831429 lnhub_rest-0.8.1/lndb/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-03-14 19:46:06.426451 lnhub_rest-0.8.1/lndb/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-03-14 19:46:06.426542 lnhub_rest-0.8.1/lndb/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-18 13:35:36.831581 lnhub_rest-0.8.1/lndb/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8429 2023-04-18 13:35:36.831706 lnhub_rest-0.8.1/lndb/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-03-30 17:54:41.279257 lnhub_rest-0.8.1/lndb/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-03-14 19:46:06.426936 lnhub_rest-0.8.1/lndb/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-18 13:35:36.831800 lnhub_rest-0.8.1/lndb/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-03-14 19:46:06.427111 lnhub_rest-0.8.1/lndb/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-03-30 17:54:41.279348 lnhub_rest-0.8.1/lndb/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     6997 2023-04-18 13:35:36.831921 lnhub_rest-0.8.1/lndb/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4917 2023-04-18 13:35:36.832173 lnhub_rest-0.8.1/lndb/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-03-14 19:46:06.427525 lnhub_rest-0.8.1/lndb/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-18 13:35:36.832243 lnhub_rest-0.8.1/lndb/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-18 13:35:36.832350 lnhub_rest-0.8.1/lndb/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-03-14 19:46:06.427862 lnhub_rest-0.8.1/lndb/lndb/test/_env.py
+-rw-r--r--   0        0        0     3856 2023-03-30 17:54:41.279631 lnhub_rest-0.8.1/lndb/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-18 13:35:36.832454 lnhub_rest-0.8.1/lndb/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-03-14 19:46:06.428161 lnhub_rest-0.8.1/lndb/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-03-14 19:46:06.428239 lnhub_rest-0.8.1/lndb/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-18 13:35:36.832538 lnhub_rest-0.8.1/lndb/noxfile.py
+-rw-r--r--   0        0        0     1378 2023-04-18 13:35:36.832791 lnhub_rest-0.8.1/lndb/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-18 13:35:36.832925 lnhub_rest-0.8.1/lndb/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-03-14 19:46:06.428637 lnhub_rest-0.8.1/lndb/tests/test_init_instance.py
+-rw-r--r--   0        0        0      385 2023-03-14 19:46:06.428715 lnhub_rest-0.8.1/lndb/tests/test_notebooks.py
+-rw-r--r--   0        0        0      225 2023-04-18 16:02:04.945178 lnhub_rest-0.8.1/lnhub_rest/__init__.py
+-rw-r--r--   0        0        0     8251 2023-04-18 16:21:04.420589 lnhub_rest-0.8.1/lnhub_rest/__main__.py
+-rw-r--r--   0        0        0       59 2023-04-18 16:02:04.945972 lnhub_rest-0.8.1/lnhub_rest/_add_storage.py
+-rw-r--r--   0        0        0       64 2023-01-15 12:17:52.330585 lnhub_rest-0.8.1/lnhub_rest/_assets/__init__.py
+-rw-r--r--   0        0        0     1026 2023-01-15 12:17:52.330665 lnhub_rest-0.8.1/lnhub_rest/_assets/_instances.py
+-rw-r--r--   0        0        0     1094 2023-02-07 14:01:34.054166 lnhub_rest-0.8.1/lnhub_rest/_assets/_schemas.py
+-rw-r--r--   0        0        0     1722 2023-04-18 16:02:04.946281 lnhub_rest-0.8.1/lnhub_rest/_check_breaks_lndb.py
+-rw-r--r--   0        0        0      998 2023-04-18 16:02:04.946668 lnhub_rest-0.8.1/lnhub_rest/_ci.py
+-rw-r--r--   0        0        0     5718 2023-04-18 16:02:04.946827 lnhub_rest-0.8.1/lnhub_rest/_clean_ci.py
+-rw-r--r--   0        0        0       64 2023-04-18 16:02:04.946919 lnhub_rest-0.8.1/lnhub_rest/_delete_instance.py
+-rw-r--r--   0        0        0       45 2023-04-18 16:02:04.947004 lnhub_rest-0.8.1/lnhub_rest/_engine.py
+-rw-r--r--   0        0        0       62 2023-04-18 16:02:04.947118 lnhub_rest-0.8.1/lnhub_rest/_init_instance.py
+-rw-r--r--   0        0        0       62 2023-04-18 16:02:04.947229 lnhub_rest-0.8.1/lnhub_rest/_load_instance.py
+-rw-r--r--   0        0        0       90 2023-01-15 12:17:52.330955 lnhub_rest-0.8.1/lnhub_rest/_models.py
+-rw-r--r--   0        0        0       47 2023-04-18 16:02:04.947314 lnhub_rest-0.8.1/lnhub_rest/_sbclient.py
+-rw-r--r--   0        0        0       61 2023-04-18 16:02:04.947399 lnhub_rest-0.8.1/lnhub_rest/_signup_signin.py
+-rw-r--r--   0        0        0       42 2023-04-18 16:02:04.947562 lnhub_rest-0.8.1/lnhub_rest/core/__init__.py
+-rw-r--r--   0        0        0      285 2023-04-18 16:02:04.947641 lnhub_rest-0.8.1/lnhub_rest/core/account/__init__.py
+-rw-r--r--   0        0        0     2336 2023-04-18 16:02:04.947726 lnhub_rest-0.8.1/lnhub_rest/core/account/_create_account.py
+-rw-r--r--   0        0        0     1062 2023-04-18 16:02:04.947805 lnhub_rest-0.8.1/lnhub_rest/core/account/_crud.py
+-rw-r--r--   0        0        0      735 2023-04-18 16:02:04.948122 lnhub_rest-0.8.1/lnhub_rest/core/account/_delete_account.py
+-rw-r--r--   0        0        0     3314 2023-04-18 16:02:04.948225 lnhub_rest-0.8.1/lnhub_rest/core/account/_signup_signin.py
+-rw-r--r--   0        0        0     1419 2023-04-18 16:02:04.948320 lnhub_rest-0.8.1/lnhub_rest/core/account/_update_account.py
+-rw-r--r--   0        0        0       38 2023-04-18 16:02:04.948381 lnhub_rest-0.8.1/lnhub_rest/core/collaborator/__init__.py
+-rw-r--r--   0        0        0     2735 2023-04-18 16:02:04.948532 lnhub_rest-0.8.1/lnhub_rest/core/collaborator/_crud.py
+-rw-r--r--   0        0        0      243 2023-04-18 16:02:04.948618 lnhub_rest-0.8.1/lnhub_rest/core/instance/__init__.py
+-rw-r--r--   0        0        0     1651 2023-04-18 16:02:04.948683 lnhub_rest-0.8.1/lnhub_rest/core/instance/_crud.py
+-rw-r--r--   0        0        0     1280 2023-04-18 16:02:04.949021 lnhub_rest-0.8.1/lnhub_rest/core/instance/_delete_instance.py
+-rw-r--r--   0        0        0     6471 2023-04-18 16:02:04.949102 lnhub_rest-0.8.1/lnhub_rest/core/instance/_init_instance.py
+-rw-r--r--   0        0        0     1528 2023-04-18 16:02:04.949405 lnhub_rest-0.8.1/lnhub_rest/core/instance/_load_instance.py
+-rw-r--r--   0        0        0     1063 2023-04-18 16:02:04.949739 lnhub_rest-0.8.1/lnhub_rest/core/instance/_update_instance.py
+-rw-r--r--   0        0        0       32 2023-04-18 16:02:04.949819 lnhub_rest-0.8.1/lnhub_rest/core/member/__init__.py
+-rw-r--r--   0        0        0     2078 2023-04-18 16:02:04.949894 lnhub_rest-0.8.1/lnhub_rest/core/member/_crud.py
+-rw-r--r--   0        0        0       80 2023-04-18 16:02:04.949960 lnhub_rest-0.8.1/lnhub_rest/core/storage/__init__.py
+-rw-r--r--   0        0        0     2850 2023-04-18 16:02:04.950032 lnhub_rest-0.8.1/lnhub_rest/core/storage/_add_storage.py
+-rw-r--r--   0        0        0     1167 2023-04-18 16:02:04.950097 lnhub_rest-0.8.1/lnhub_rest/core/storage/_crud.py
+-rw-r--r--   0        0        0      796 2023-04-18 16:02:04.950233 lnhub_rest-0.8.1/lnhub_rest/main.py
+-rw-r--r--   0        0        0       11 2023-04-18 16:02:04.950293 lnhub_rest-0.8.1/lnhub_rest/orm/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-18 16:02:04.950361 lnhub_rest-0.8.1/lnhub_rest/orm/_engine.py
+-rw-r--r--   0        0        0     2543 2023-04-18 16:02:04.950590 lnhub_rest-0.8.1/lnhub_rest/orm/_sbclient.py
+-rw-r--r--   0        0        0      198 2023-04-18 16:02:04.950703 lnhub_rest-0.8.1/lnhub_rest/routers/__init__.py
+-rw-r--r--   0        0        0     4121 2023-04-18 16:02:04.950818 lnhub_rest-0.8.1/lnhub_rest/routers/account.py
+-rw-r--r--   0        0        0      538 2023-04-18 16:02:04.951096 lnhub_rest-0.8.1/lnhub_rest/routers/ci.py
+-rw-r--r--   0        0        0      408 2023-04-18 16:02:04.951160 lnhub_rest-0.8.1/lnhub_rest/routers/dev.py
+-rw-r--r--   0        0        0     4243 2023-04-18 16:02:04.951226 lnhub_rest-0.8.1/lnhub_rest/routers/instance.py
+-rw-r--r--   0        0        0     2617 2023-04-18 16:02:04.951432 lnhub_rest-0.8.1/lnhub_rest/routers/organization.py
+-rw-r--r--   0        0        0     1061 2023-04-18 16:02:04.951701 lnhub_rest-0.8.1/lnhub_rest/routers/utils.py
+-rw-r--r--   0        0        0      249 2023-04-18 16:02:04.952299 lnhub_rest-0.8.1/lnhub_rest/schema/__init__.py
+-rw-r--r--   0        0        0     4986 2023-04-18 16:02:04.952431 lnhub_rest-0.8.1/lnhub_rest/schema/_core.py
+-rw-r--r--   0        0        0      270 2023-02-15 16:43:38.796706 lnhub_rest-0.8.1/lnhub_rest/schema/_timestamps.py
+-rw-r--r--   0        0        0      262 2023-04-18 16:02:04.952506 lnhub_rest-0.8.1/lnhub_rest/schema/_type.py
+-rw-r--r--   0        0        0      252 2023-02-15 16:43:38.796850 lnhub_rest-0.8.1/lnhub_rest/schema/_users.py
+-rw-r--r--   0        0        0     1079 2023-04-18 16:02:04.952789 lnhub_rest-0.8.1/lnhub_rest/schema/_versions.py
+-rw-r--r--   0        0        0      674 2023-04-18 16:01:55.110061 lnhub_rest-0.8.1/lnhub_rest/schema/alembic.ini
+-rw-r--r--   0        0        0       50 2023-04-18 16:02:04.953110 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/__init__.py
+-rw-r--r--   0        0        0     6020 2023-04-18 16:02:04.953355 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/clone.py
+-rw-r--r--   0        0        0     2979 2023-04-18 16:02:04.953601 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/env.py
+-rw-r--r--   0        0        0     1193 2023-04-18 16:02:04.953923 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0     1319 2023-04-18 16:02:04.953987 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1667 2023-04-18 16:02:04.954047 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0       39 2023-04-18 16:02:04.954171 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/__init__.py
+-rw-r--r--   0        0        0     3940 2023-04-18 16:02:04.954327 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py
+-rw-r--r--   0        0        0      639 2023-04-18 16:02:04.954391 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py
+-rw-r--r--   0        0        0      214 2023-04-18 16:02:04.954454 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_03_24_333fd693eac8_v0_6_1b.py
+-rw-r--r--   0        0        0      192 2023-04-18 16:02:04.954511 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_03_30_b5907be59c45_v0_8_dev1.py
+-rw-r--r--   0        0        0     7619 2023-04-18 16:02:04.954572 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev2.py
+-rw-r--r--   0        0        0     1408 2023-04-18 16:02:04.954855 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_04_04_6e7d7a97c233_v0_8_dev3.py
+-rw-r--r--   0        0        0      880 2023-04-18 16:02:04.955067 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_04_18_1092ae46baba_v0_8_1.py
+-rw-r--r--   0        0        0       33 2023-04-18 16:02:04.955245 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/__init__.py
+-rw-r--r--   0        0        0      542 2023-01-15 12:17:52.331616 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/script.py.mako
+-rw-r--r--   0        0        0      757 2023-04-18 16:02:04.955360 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/settings.py
+-rw-r--r--   0        0        0     5549 2023-04-18 16:02:04.955713 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/testing.py
+-rw-r--r--   0        0        0     1816 2023-04-18 16:21:04.420695 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-13-53709f2a2043-v0_0_1a.py
+-rw-r--r--   0        0        0      935 2023-04-18 16:21:04.420776 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-13-c555c87a640c-v0_0_1.py
+-rw-r--r--   0        0        0     5052 2023-04-18 16:21:04.421051 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-14-f7ba9352c706-v0_0_2.py
+-rw-r--r--   0        0        0     1401 2023-04-18 16:21:04.421410 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-23-c13c9dd0f3ae-v0_1_4a.py
+-rw-r--r--   0        0        0      536 2023-04-18 16:21:04.421665 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-24-e7151581f790-v0_1_4b.py
+-rw-r--r--   0        0        0      512 2023-04-18 16:21:04.421743 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-30-2efe1dee9baf-v0_1_4c.py
+-rw-r--r--   0        0        0      667 2023-04-18 16:21:04.421817 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-06-95073282294e-v0_1_4e.py
+-rw-r--r--   0        0        0      869 2023-04-18 16:21:04.422041 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-06-9c02109e4faa-v0_2_0.py
+-rw-r--r--   0        0        0     2190 2023-04-18 16:21:04.422119 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-06-f2cb77148a6e-v0_1_4d.py
+-rw-r--r--   0        0        0      458 2023-04-18 16:21:04.422361 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-08-e7eef9775586-0_2_1.py
+-rw-r--r--   0        0        0     1220 2023-04-18 16:21:04.422588 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-15-641d1508baab-v0_4_0.py
+-rw-r--r--   0        0        0      624 2023-04-18 16:21:04.422993 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py
+-rw-r--r--   0        0        0      918 2023-04-18 16:02:04.956279 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py
+-rw-r--r--   0        0        0      575 2023-04-18 16:02:04.956348 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py
+-rw-r--r--   0        0        0      542 2023-04-18 16:02:04.956406 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py
+-rw-r--r--   0        0        0     1199 2023-04-18 16:02:04.956469 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-03-30-b5907be59c45-v0_8_dev1.py
+-rw-r--r--   0        0        0      733 2023-04-18 16:02:04.956526 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-04-04-6e7d7a97c233-v0_8_dev2.py
+-rw-r--r--   0        0        0     5143 2023-04-18 16:02:04.956591 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-04-05-d0aecf764dbe-v0_8_dev3.py
+-rw-r--r--   0        0        0      593 2023-04-18 16:02:04.956814 lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-04-18-1092ae46baba-v0_8_1.py
+-rw-r--r--   0        0        0       60 2023-02-15 16:43:38.797298 lnhub_rest-0.8.1/lnhub_rest/schema/versions.py
+-rw-r--r--   0        0        0       13 2023-04-18 16:02:04.956879 lnhub_rest-0.8.1/lnhub_rest/utils/__init__.py
+-rw-r--r--   0        0        0      212 2023-04-18 16:02:04.956936 lnhub_rest-0.8.1/lnhub_rest/utils/_access_token.py
+-rw-r--r--   0        0        0      352 2023-04-18 16:02:04.956991 lnhub_rest-0.8.1/lnhub_rest/utils/_id.py
+-rw-r--r--   0        0        0      109 2023-04-18 16:02:04.957042 lnhub_rest-0.8.1/lnhub_rest/utils/_query.py
+-rw-r--r--   0        0        0     3816 2023-04-18 16:02:04.957124 lnhub_rest-0.8.1/lnhub_rest/utils/_test.py
+-rw-r--r--   0        0        0     1758 2023-04-18 16:02:04.957587 lnhub_rest-0.8.1/noxfile.py
+-rw-r--r--   0        0        0     1253 2023-04-18 16:02:04.957709 lnhub_rest-0.8.1/pyproject.toml
+-rwxr-xr-x   0        0        0       29 2023-04-18 16:02:04.957796 lnhub_rest-0.8.1/scripts/run.sh
+-rw-r--r--   0        0        0       27 2023-04-18 16:02:04.957868 lnhub_rest-0.8.1/supabase/.gitignore
+-rw-r--r--   0        0        0     2548 2023-04-18 16:02:04.957934 lnhub_rest-0.8.1/supabase/config.toml
+-rw-r--r--   0        0        0      866 2023-04-18 16:21:04.423121 lnhub_rest-0.8.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2068 1970-01-01 00:00:00.000000 lnhub_rest-0.8.1/PKG-INFO
```

### Comparing `lnhub_rest-0.7rc1/.dockerignore` & `lnhub_rest-0.8.1/.dockerignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/.github/workflows/build.yml` & `lnhub_rest-0.8.1/.github/workflows/build.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 name: build
 
 on:
   push:
-    branches: [main, staging]
+    branches: [main]
   pull_request:
     branches: [main, staging]
 env:
+  BRANCH_NAME: ${{ github.head_ref || github.ref_name }}
   SUPABASE_STAGING_URL: ${{ secrets.SUPABASE_STAGING_URL }}
   SUPABASE_STAGING_ANON_KEY: ${{ secrets.SUPABASE_STAGING_ANON_KEY }}
   SUPABASE_STAGING_SERVICE_ROLE_KEY: ${{ secrets.SUPABASE_STAGING_SERVICE_ROLE_KEY }}
   LNHUB_STAGING_PG_PASSWORD: ${{ secrets.LNHUB_STAGING_PG_PASSWORD }}
   SUPABASE_PROD_URL: ${{ secrets.SUPABASE_PROD_URL }}
   SUPABASE_PROD_ANON_KEY: ${{ secrets.SUPABASE_PROD_ANON_KEY }}
   SUPABASE_PROD_SERVICE_ROLE_KEY: ${{ secrets.SUPABASE_PROD_SERVICE_ROLE_KEY }}
@@ -19,62 +20,76 @@
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9"]
-    timeout-minutes: 10
+        package:
+          - "lnhub-rest"
+          - "lndb"
+    timeout-minutes: 25
 
     steps:
       - name: Checkout main
         uses: actions/checkout@v3
         with:
+          submodules: recursive
+          token: ${{ secrets.ACCESS_TOKEN_ALEX }}
           fetch-depth: 0
       - name: Setup Supabase CLI
         uses: supabase/setup-cli@v1
       - name: Setup Python
         uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
-      - name: Cache pre-commit & nox
+      - name: Cache nox
+        uses: actions/cache@v3
+        with:
+          path: .nox
+          key: nox-${{ runner.os }}
+      - name: Cache pre-commit
         uses: actions/cache@v3
-        env:
-          cache-name: cache-2
         with:
-          path: |
-            .nox
-            ~/.cache/pre-commit
-          key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('.pre-commit-config.yaml') }}-${{ hashFiles('pyproject.yaml') }}
+          path: ~/.cache/pre-commit
+          key: pre-commit-${{ runner.os }}-${{ hashFiles('.pre-commit-config.yaml') }}
       - name: Cache postgres
         id: cache-postgres
         uses: actions/cache@v3
         with:
           path: ~/postgres.tar
           key: cache-postgres-0
       - name: Cache postgres miss
         if: steps.cache-postgres.outputs.cache-hit != 'true'
         run: docker pull postgres:latest && docker image save postgres:latest --output ~/postgres.tar
       - name: Cache postgres use
         if: steps.cache-postgres.outputs.cache-hit == 'true'
         run: docker image load --input ~/postgres.tar
-      - name: Install pip and nox
+      - name: Install CI dependencies
         run: |
-          python -m pip install --upgrade pip
-          pip install nox
+          python -m pip install -U pip
+          pip install -U laminci
+          pip install -U lamindb
+          sudo apt-get -y install graphviz
+          sudo apt-get install sqlite3-tools=3.37.2-2
       - name: Lint
         run: |
           nox -s lint
       - name: Configure AWS
         uses: aws-actions/configure-aws-credentials@v1
         with:
           aws-access-key-id: ${{ secrets.AWS_ACCESS_KEY_ID }}
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
+      - name: Configure Google Cloud
+        id: "auth"
+        uses: "google-github-actions/auth@v0"
+        with:
+          credentials_json: "${{ secrets.GCP_CREDENTIALS }}"
       - name: Build
         run: |
-          nox -s build --python ${{ matrix.python-version }}
+          nox -s "build(package='${{ matrix.package }}')"
       - name: Codecov
         if: matrix.python-version == '3.9'
         uses: codecov/codecov-action@v2
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `lnhub_rest-0.7rc1/.github/workflows/google-cloudrun-docker.yml` & `lnhub_rest-0.8.1/.github/workflows/google-cloudrun-docker.yml`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,20 @@
       contents: "read"
       id-token: "write"
 
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v2
-
+        with:
+          submodules: recursive
+          token: ${{ secrets.ACCESS_TOKEN_ALEX }}
+          fetch-depth: 0
+      # - name: Go back to previous release (before avatar)
+      #   run: git checkout 843af6d
       - name: Google Auth
         id: auth
         uses: "google-github-actions/auth@v1"
         with:
           token_format: "access_token"
           workload_identity_provider: "${{ secrets.WIF_PROVIDER }}" # e.g. - projects/123456789/locations/global/workloadIdentityPools/my-pool/providers/my-provider
           service_account: "${{ secrets.WIF_SERVICE_ACCOUNT }}" # e.g. - my-service-account@my-project.iam.gserviceaccount.com
```

### Comparing `lnhub_rest-0.7rc1/.github/workflows/latest-changes.yml` & `lnhub_rest-0.8.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/.gitignore` & `lnhub_rest-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/.pre-commit-config.yaml` & `lnhub_rest-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/README.md` & `lnhub_rest-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-2efe1dee9baf.svg` & `lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-2efe1dee9baf.svg`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-a88f5298b8f7.svg` & `lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-a88f5298b8f7.svg`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-c13c9dd0f3ae.svg` & `lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-c13c9dd0f3ae.svg`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-e7151581f790.svg` & `lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-e7151581f790.svg`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-e7eef9775586.svg` & `lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-e7eef9775586.svg`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-f2cb77148a6e.svg` & `lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-f2cb77148a6e.svg`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-f7ba9352c706.svg` & `lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-f7ba9352c706.svg`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/_schemas/lnhub-schema-fe962c9a0ae7.svg` & `lnhub_rest-0.8.1/docs/_schemas/lnhub-schema-fe962c9a0ae7.svg`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/account/01-signup-signin.ipynb` & `lnhub_rest-0.8.1/docs/account/01-signup-signin.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/account/02-create-account.ipynb` & `lnhub_rest-0.8.1/docs/account/02-create-account.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946626984126985%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'from lnhub_rest.core.account import "*

 * *            "create_user_account, delete_account\\n'), (1, 'from lnhub_rest.utils._test import "*

 * *            "create_test_auth\\n')], delete: [1, 0]}}, 5: {'source': ['### Call "*

 * *            "`create_user_account`'], 'attachments': OrderedDict()}, 6: {'source': {insert: [(0, "*

 * *            "'message = create_user_account(\\n')], delete: [0]}}, 12: {'source': ['### Call "*

 * *            "`create_user_account` on existing account'],  […]*

```diff
@@ -11,16 +11,16 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "from lnhub_rest.core.account import create_account, delete_account\n",
-                "from lnhub_rest.utils import create_test_auth\n",
+                "from lnhub_rest.core.account import create_user_account, delete_account\n",
+                "from lnhub_rest.utils._test import create_test_auth\n",
                 "from lnhub_rest.main import client\n",
                 "from lnhub_rest._clean_ci import clean_ci"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
@@ -48,29 +48,30 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Create a new account"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Call `create_account`"
+                "### Call `create_user_account`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "message = create_account(\n",
+                "message = create_user_account(\n",
                 "    handle=auth_1[\"handle\"],\n",
                 "    _access_token=access_token_1,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
@@ -115,29 +116,30 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Create a new account using an existing handle"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Call `create_account` on existing account"
+                "### Call `create_user_account` on existing account"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "message = create_account(\n",
+                "message = create_user_account(\n",
                 "    handle=auth_1[\"handle\"],\n",
                 "    _access_token=auth_1[\"access_token\"],\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `lnhub_rest-0.7rc1/docs/account/03-update-account.ipynb` & `lnhub_rest-0.8.1/docs/account/03-update-account.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99987922705314%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'from lnhub_rest.utils._test import create_test_auth, "*

 * *            "create_test_account\\n')], delete: [2]}}}"}*

```diff
@@ -11,15 +11,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lnhub_rest.core.account import update_account, delete_account\n",
                 "from lnhub_rest.core.account._crud import sb_select_account_by_handle\n",
-                "from lnhub_rest.utils import create_test_auth, create_test_account\n",
+                "from lnhub_rest.utils._test import create_test_auth, create_test_account\n",
                 "from lnhub_rest._sbclient import connect_hub\n",
                 "from lnhub_rest.main import client\n",
                 "from lnhub_rest._clean_ci import clean_ci\n",
                 "\n",
                 "hub = connect_hub()"
             ]
         },
```

### Comparing `lnhub_rest-0.7rc1/docs/account/04-fetch-account.ipynb` & `lnhub_rest-0.8.1/docs/account/04-fetch-account.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999547101449275%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(20, \'    role="admin",\\n\')], delete: [20]}}}'}*

```diff
@@ -64,15 +64,15 @@
                 "instance = create_test_instance(storage_id=storage[\"id\"], access_token=access_token)\n",
                 "instance_id = instance[\"id\"]\n",
                 "\n",
                 "# Add account as an admin member\n",
                 "instance_collaborator = add_test_collaborator(\n",
                 "    instance_id=instance_id,\n",
                 "    account_id=account_id,\n",
-                "    permission=\"admin\",\n",
+                "    role=\"admin\",\n",
                 "    access_token=access_token,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `lnhub_rest-0.7rc1/docs/account/05-rls.ipynb` & `lnhub_rest-0.8.1/docs/account/05-rls.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9906994047619048%*

 * *Differences: {"'cells'": '{delete: [12, 11]}', "'metadata'": "{'language_info': {'version': '3.9.12'}}"}*

```diff
@@ -143,42 +143,14 @@
                 "assert \"new row violates row-level security policy\" in error.value.message"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Using non corresponding account authentication"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "with pytest.raises(Exception) as error:\n",
-                "    account = sb_insert_account(\n",
-                "        account_fields={\n",
-                "            \"id\": account_id_1,\n",
-                "            \"user_id\": account_id_1,\n",
-                "            \"lnid\": base62(8),\n",
-                "            \"handle\": account_handle_1,\n",
-                "        },\n",
-                "        supabase_client=account_hub_2,\n",
-                "    )\n",
-                "\n",
-                "\n",
-                "assert \"new row violates row-level security policy\" in error.value.message"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "Using corresponding account authentication"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -402,15 +374,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.12"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.7rc1/docs/changelog.md` & `lnhub_rest-0.8.1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🏗️ Fix local development setup | [174](https://github.com/laminlabs/lnhub-rest/pull/174) | [falexwolf](https://github.com/falexwolf) | 2023-04-18 | 0.8.1
+🗃️ Fix RLS for storage table | [173](https://github.com/laminlabs/lnhub-rest/pull/173) | [fredericenard](https://github.com/fredericenard) | 2023-04-18 |
+✨ Create organization endpoints | [165](https://github.com/laminlabs/lnhub-rest/pull/165) | [bpenteado](https://github.com/bpenteado) | 2023-04-17 |
+👷 Run tests against `lndb` | [143](https://github.com/laminlabs/lnhub-rest/pull/143) | [falexwolf](https://github.com/falexwolf) | 2023-04-13 |
+♻️ Simplify migrations testing | [168](https://github.com/laminlabs/lnhub-rest/pull/168) | [falexwolf](https://github.com/falexwolf) | 2023-04-12 |
+🗃️ Create organization membership table | [163](https://github.com/laminlabs/lnhub-rest/pull/163) | [bpenteado](https://github.com/bpenteado) | 2023-04-11 |
+🗃️ Reset RLS policies | [161](https://github.com/laminlabs/lnhub-rest/pull/161) | [bpenteado](https://github.com/bpenteado) | 2023-04-05 |
+🗃️ Implement cascade deletion on instance table | [158](https://github.com/laminlabs/lnhub-rest/pull/158) | [bpenteado](https://github.com/bpenteado) | 2023-04-04 |
+✨ Create endpoint to fetch an avatar | [167](https://github.com/laminlabs/lnhub-rest/pull/167) | [fredericenard](https://github.com/fredericenard) | 2023-04-07 |
+✨ Create an endpoint to fetch avatar given a list of lnid | [166](https://github.com/laminlabs/lnhub-rest/pull/166) | [fredericenard](https://github.com/fredericenard) | 2023-04-07 | 0.7.3
+🐛 Fix sign in | [160](https://github.com/laminlabs/lnhub-rest/pull/160) | [fredericenard](https://github.com/fredericenard) | 2023-03-31 | 0.7.2
+🐛 Enforce compatibility with new sign in API | [159](https://github.com/laminlabs/lnhub-rest/pull/159) | [fredericenard](https://github.com/fredericenard) | 2023-03-31 | 0.7.1
+🔖 Staging version 0.7.0 | [150](https://github.com/laminlabs/lnhub-rest/pull/150) | [fredericenard](https://github.com/fredericenard) | 2023-03-29 | 0.7.0
 ⚡ Improve instance deletion through RLS | [154](https://github.com/laminlabs/lnhub-rest/pull/154) | [bpenteado](https://github.com/bpenteado) | 2023-03-29 | 0.7rc1
 ✨ Enable instance ownership transfer | [156](https://github.com/laminlabs/lnhub-rest/pull/156) | [bpenteado](https://github.com/bpenteado) | 2023-03-28 |
 Deploy lnhub-rest on Cloud Run using Github actions | [155](https://github.com/laminlabs/lnhub-rest/pull/155) | [lawrlee](https://github.com/lawrlee) | 2023-03-27 |
 🐛 Ensure integrity of RLS for local tests | [152](https://github.com/laminlabs/lnhub-rest/pull/152) | [fredericenard](https://github.com/fredericenard) | 2023-03-24 |
 🐛 Add test to ensure an owner can delete collaborators | [153](https://github.com/laminlabs/lnhub-rest/pull/153) | [fredericenard](https://github.com/fredericenard) | 2023-03-24 |
 ⬆️ Upgrade supabase | [149](https://github.com/laminlabs/lnhub-rest/pull/149) | [fredericenard](https://github.com/fredericenard) | 2023-03-23 |
 🔖 Staging version 0.7.0 | [148](https://github.com/laminlabs/lnhub-rest/pull/148) | [bpenteado](https://github.com/bpenteado) | 2023-03-21 |
```

### Comparing `lnhub_rest-0.7rc1/docs/checks/01-check-break-lndb.ipynb` & `lnhub_rest-0.8.1/docs/checks/01-check-break-lndb.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/instance/01-init-instance.ipynb` & `lnhub_rest-0.8.1/docs/instance/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/instance/02-load-instance.ipynb` & `lnhub_rest-0.8.1/docs/instance/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/instance/03-update-instance.ipynb` & `lnhub_rest-0.8.1/docs/instance/03-update-instance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978472222222222%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'from lnhub_rest.utils._test import (\\n')], delete: "*

 * *            '[3]}}, 3: {\'source\': {insert: [(11, \'    role="admin",\\n\')], delete: [11]}}, 15: '*

 * *            '{\'source\': [\'non_existing_instance_id = instance_id[:-5] + "1aa63"\']}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.12'}}"}*

```diff
@@ -12,15 +12,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lnhub_rest.core.account import delete_account\n",
                 "from lnhub_rest.core.instance import update_instance, delete_instance\n",
                 "from lnhub_rest.core.instance._crud import sb_select_instance\n",
-                "from lnhub_rest.utils import (\n",
+                "from lnhub_rest.utils._test import (\n",
                 "    create_test_auth,\n",
                 "    create_test_account,\n",
                 "    create_test_instance,\n",
                 "    create_test_storage,\n",
                 "    add_test_collaborator,\n",
                 ")\n",
                 "from lnhub_rest._sbclient import connect_hub_with_auth\n",
@@ -48,15 +48,15 @@
                 "instance = create_test_instance(storage_id=storage[\"id\"], access_token=access_token)\n",
                 "\n",
                 "instance_id = instance[\"id\"]\n",
                 "\n",
                 "add_test_collaborator(\n",
                 "    instance_id=instance_id,\n",
                 "    account_id=account[\"id\"],\n",
-                "    permission=\"admin\",\n",
+                "    role=\"admin\",\n",
                 "    access_token=access_token,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -164,15 +164,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "non_existing_instance_id = instance_id[:-1] + \"1\""
+                "non_existing_instance_id = instance_id[:-5] + \"1aa63\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -262,15 +262,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
+            "version": "3.9.12"
         },
         "vscode": {
             "interpreter": {
                 "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
             }
         }
     },
```

### Comparing `lnhub_rest-0.7rc1/docs/instance/04-delete-instance.ipynb` & `lnhub_rest-0.8.1/docs/instance/04-delete-instance.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9789850809889173%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'from lnhub_rest.core.instance._crud import (\\n'), (3, "*

 * *            "'    sb_select_instance_by_name,\\n'), (4, '    sb_select_instance,\\n'), (5, '    "*

 * *            "sb_delete_instance,\\n'), (6, ')\\n'), (7, 'from lnhub_rest.core.collaborator._crud "*

 * *            "import sb_select_collaborators\\n')], delete: [2]}}, 4: {'source': {insert: [(14, "*

 * *            "'account_hub_2 = connect_hub_with_auth(access_token=access_token_2)\\n'), (38, '    "*

 * *            'role=" […]*

```diff
@@ -11,15 +11,20 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from lnhub_rest.core.account import delete_account\n",
                 "from lnhub_rest.core.instance import init_instance, delete_instance\n",
-                "from lnhub_rest.core.instance._crud import sb_select_instance_by_name\n",
+                "from lnhub_rest.core.instance._crud import (\n",
+                "    sb_select_instance_by_name,\n",
+                "    sb_select_instance,\n",
+                "    sb_delete_instance,\n",
+                ")\n",
+                "from lnhub_rest.core.collaborator._crud import sb_select_collaborators\n",
                 "from lnhub_rest.routers.instance import get_instance_accounts\n",
                 "from lnhub_rest._clean_ci import delete_ci_instances\n",
                 "import sqlmodel as sqm\n",
                 "from lnhub_rest.schema import Instance\n",
                 "from lnhub_rest.main import client\n",
                 "import string, secrets\n",
                 "from lnhub_rest._sbclient import connect_hub, connect_hub_with_auth\n",
@@ -66,14 +71,15 @@
                 "account_hub_1 = connect_hub_with_auth(access_token=access_token_1)\n",
                 "\n",
                 "# Create account 2\n",
                 "auth_2 = create_test_auth()\n",
                 "access_token_2 = auth_2[\"access_token\"]\n",
                 "account_2 = create_test_account(handle=auth_2[\"handle\"], access_token=access_token_2)\n",
                 "handle_2 = account_2[\"handle\"]\n",
+                "account_hub_2 = connect_hub_with_auth(access_token=access_token_2)\n",
                 "\n",
                 "existing_storage_root = \"s3://lndb-setup-ci\"\n",
                 "\n",
                 "instance_name_1 = f\"lamin.ci.instance.{base26(6)}\"\n",
                 "db_1 = f\"postgresql://postgres:pwd@0.0.0.0:5432/{instance_name_1}\"\n",
                 "\n",
                 "instance_name_2 = f\"lamin.ci.instance.{base26(6)}\"\n",
@@ -89,15 +95,15 @@
                 ")\n",
                 "instance_1 = sb_select_instance_by_name(\n",
                 "    account_id=account_1[\"id\"], name=instance_name_1, supabase_client=account_hub_1\n",
                 ")\n",
                 "instance_collaborator = add_test_collaborator(\n",
                 "    instance_id=instance_1[\"id\"],\n",
                 "    account_id=account_2[\"id\"],\n",
-                "    permission=\"admin\",\n",
+                "    role=\"admin\",\n",
                 "    access_token=access_token_1,\n",
                 ")\n",
                 "\n",
                 "# Init instance 2\n",
                 "init_instance(\n",
                 "    owner=handle_1,\n",
                 "    name=instance_name_2,\n",
@@ -105,23 +111,78 @@
                 "    db=db_2,\n",
                 "    _access_token=access_token_1,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "## Delete an instance"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "### Test cascade delete"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "sb_delete_instance(instance_1[\"id\"], account_hub_2)\n",
+                "\n",
+                "instance = sb_select_instance(instance_1[\"id\"], account_hub_1)\n",
+                "assert instance is None\n",
+                "\n",
+                "collaborators = sb_select_collaborators(instance_1[\"id\"], account_hub_1)\n",
+                "assert collaborators is None"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Restore instance."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "init_instance(\n",
+                "    owner=handle_1,\n",
+                "    name=instance_name_1,\n",
+                "    storage=existing_storage_root,\n",
+                "    db=db_1,\n",
+                "    _access_token=access_token_1,\n",
+                ")\n",
+                "instance_1 = sb_select_instance_by_name(\n",
+                "    account_id=account_1[\"id\"], name=instance_name_1, supabase_client=account_hub_1\n",
+                ")\n",
+                "instance_collaborator = add_test_collaborator(\n",
+                "    instance_id=instance_1[\"id\"],\n",
+                "    account_id=account_2[\"id\"],\n",
+                "    role=\"admin\",\n",
+                "    access_token=access_token_1,\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "### Call `delete_instance`"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `lnhub_rest-0.7rc1/docs/instance/05-fetch-instance.ipynb` & `lnhub_rest-0.8.1/docs/instance/05-fetch-instance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996701032885243%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(29, \'    role="admin",\\n\'), (33, \'# Add account 2 as '*

 * *            'a member with read role\\n\'), (38, \'    role="read",\\n\')], delete: [38, 33, '*

 * *            '29]}}, 5: {\'source\': {insert: [(6, \'    "role": "admin",\\n\')], delete: [6]}}, '*

 * *            '11: {\'source\': {insert: [(11, \'    "role": "admin",\\n\')], delete: [11]}}}'}*

```diff
@@ -71,24 +71,24 @@
                 "instance_name_1 = instance_1[\"name\"]\n",
                 "\n",
                 "# Add account 1 as an admin member\n",
                 "\n",
                 "instance_collaborator_1 = add_test_collaborator(\n",
                 "    instance_id=instance_account_id_1,\n",
                 "    account_id=account_id_1,\n",
-                "    permission=\"admin\",\n",
+                "    role=\"admin\",\n",
                 "    access_token=access_token_1,\n",
                 ")\n",
                 "\n",
-                "# Add account 2 as a member with read permission\n",
+                "# Add account 2 as a member with read role\n",
                 "\n",
                 "instance_collaborator_2 = add_test_collaborator(\n",
                 "    instance_id=instance_account_id_1,\n",
                 "    account_id=account_id_2,\n",
-                "    permission=\"read\",\n",
+                "    role=\"read\",\n",
                 "    access_token=access_token_1,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -104,15 +104,15 @@
             "source": [
                 "instance_expected = {\n",
                 "    \"instance\": {\n",
                 "        **instance_1,\n",
                 "        \"storage\": {\"root\": storage[\"root\"]},\n",
                 "        \"account\": {\"handle\": account_handle_, \"id\": account_id_1},\n",
                 "    },\n",
-                "    \"permission\": \"admin\",\n",
+                "    \"role\": \"admin\",\n",
                 "}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -171,15 +171,15 @@
                 "            \"account\": account_1,\n",
                 "        },\n",
                 "        {\n",
                 "            **instance_collaborator_2,\n",
                 "            \"account\": account_2,\n",
                 "        },\n",
                 "    ],\n",
-                "    \"permission\": \"admin\",\n",
+                "    \"role\": \"admin\",\n",
                 "}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `lnhub_rest-0.7rc1/docs/instance/06-rls.ipynb` & `lnhub_rest-0.8.1/docs/instance/06-rls.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996942806322934%*

 * *Differences: {"'cells'": '{9: {\'source\': {insert: [(4, \'        "role": "admin",\\n\')], delete: [4]}}, 13: '*

 * *            '{\'source\': {insert: [(4, \'        "role": "admin",\\n\')], delete: [4]}}, 14: '*

 * *            "{'source': ['A admin can add a collaborator with a read role.'], 'attachments': "*

 * *            'OrderedDict()}, 15: {\'source\': {insert: [(4, \'        "role": "read",\\n\')], '*

 * *            'delete: [4]}}, 16: {\'source\': ["A collaborator with a read role can\'t add a '*

 * *            'collaborator."], \ […]*

```diff
@@ -160,15 +160,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "sb_insert_collaborator(\n",
                 "    account_instance_fields={\n",
                 "        \"account_id\": account_id_1,\n",
                 "        \"instance_id\": instance[\"id\"],\n",
-                "        \"permission\": \"admin\",\n",
+                "        \"role\": \"admin\",\n",
                 "    },\n",
                 "    supabase_client=account_hub_1,\n",
                 ")\n",
                 "\n",
                 "assert (\n",
                 "    sb_select_collaborator(\n",
                 "        instance_id=instance[\"id\"],\n",
@@ -206,15 +206,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "sb_insert_collaborator(\n",
                 "    account_instance_fields={\n",
                 "        \"account_id\": account_id_2,\n",
                 "        \"instance_id\": instance[\"id\"],\n",
-                "        \"permission\": \"admin\",\n",
+                "        \"role\": \"admin\",\n",
                 "    },\n",
                 "    supabase_client=account_hub_1,\n",
                 ")\n",
                 "\n",
                 "assert (\n",
                 "    sb_select_collaborator(\n",
                 "        instance_id=instance[\"id\"],\n",
@@ -222,33 +222,34 @@
                 "        supabase_client=account_hub_1,\n",
                 "    )\n",
                 "    is not None\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "A admin can add a collaborator with a read permission."
+                "A admin can add a collaborator with a read role."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "sb_insert_collaborator(\n",
                 "    account_instance_fields={\n",
                 "        \"account_id\": account_id_3,\n",
                 "        \"instance_id\": instance[\"id\"],\n",
-                "        \"permission\": \"read\",\n",
+                "        \"role\": \"read\",\n",
                 "    },\n",
                 "    supabase_client=account_hub_2,\n",
                 ")\n",
                 "\n",
                 "assert (\n",
                 "    sb_select_collaborator(\n",
                 "        instance_id=instance[\"id\"],\n",
@@ -256,32 +257,33 @@
                 "        supabase_client=account_hub_2,\n",
                 "    )\n",
                 "    is not None\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "A collaborator with a read permission can't add a collaborator."
+                "A collaborator with a read role can't add a collaborator."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "with pytest.raises(Exception) as error:\n",
                 "    sb_insert_collaborator(\n",
                 "        account_instance_fields={\n",
                 "            \"account_id\": account_id_4,\n",
                 "            \"instance_id\": instance[\"id\"],\n",
-                "            \"permission\": \"read\",\n",
+                "            \"role\": \"read\",\n",
                 "        },\n",
                 "        supabase_client=account_hub_3,\n",
                 "    )\n",
                 "\n",
                 "assert \"new row violates row-level security policy\" in error.value.message"
             ]
         },
@@ -299,15 +301,15 @@
             "outputs": [],
             "source": [
                 "with pytest.raises(Exception) as error:\n",
                 "    sb_insert_collaborator(\n",
                 "        account_instance_fields={\n",
                 "            \"account_id\": account_id_4,\n",
                 "            \"instance_id\": instance[\"id\"],\n",
-                "            \"permission\": \"read\",\n",
+                "            \"role\": \"read\",\n",
                 "        },\n",
                 "        supabase_client=account_hub_4,\n",
                 "    )\n",
                 "\n",
                 "assert \"new row violates row-level security policy\" in error.value.message"
             ]
         },
@@ -330,54 +332,55 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sb_update_collaborator(\n",
                 "    account_id=account_id_3,\n",
                 "    instance_id=instance[\"id\"],\n",
-                "    permission=\"read-write\",\n",
+                "    role=\"write\",\n",
                 "    supabase_client=account_hub_2,\n",
                 ")\n",
                 "\n",
                 "assert (\n",
                 "    sb_select_collaborator(\n",
                 "        account_id=account_id_3,\n",
                 "        instance_id=instance[\"id\"],\n",
                 "        supabase_client=account_hub_2,\n",
-                "    )[\"permission\"]\n",
-                "    == \"read-write\"\n",
+                "    )[\"role\"]\n",
+                "    == \"write\"\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "A member with a non admin permission can't update a collaborator."
+                "A member with a non admin role can't update a collaborator."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "sb_update_collaborator(\n",
                 "    account_id=account_id_3,\n",
                 "    instance_id=instance[\"id\"],\n",
-                "    permission=\"read-write\",\n",
+                "    role=\"write\",\n",
                 "    supabase_client=account_hub_3,\n",
                 ")\n",
                 "\n",
                 "assert (\n",
                 "    sb_select_collaborator(\n",
                 "        account_id=account_id_2,\n",
                 "        instance_id=instance[\"id\"],\n",
                 "        supabase_client=account_hub_3,\n",
-                "    )[\"permission\"]\n",
+                "    )[\"role\"]\n",
                 "    == \"admin\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -448,15 +451,15 @@
                 "    supabase_client=account_hub_1,\n",
                 ")\n",
                 "\n",
                 "sb_insert_collaborator(\n",
                 "    account_instance_fields={\n",
                 "        \"account_id\": account_id_2,\n",
                 "        \"instance_id\": instance[\"id\"],\n",
-                "        \"permission\": \"admin\",\n",
+                "        \"role\": \"admin\",\n",
                 "    },\n",
                 "    supabase_client=account_hub_1,\n",
                 ")\n",
                 "\n",
                 "sb_delete_collaborator(\n",
                 "    account_id=account_id_2, instance_id=instance[\"id\"], supabase_client=account_hub_1\n",
                 ")\n",
@@ -527,15 +530,15 @@
                 "    supabase_client=account_hub_1,\n",
                 ")\n",
                 "\n",
                 "sb_insert_collaborator(\n",
                 "    account_instance_fields={\n",
                 "        \"account_id\": account_id_1,\n",
                 "        \"instance_id\": private_instance[\"id\"],\n",
-                "        \"permission\": \"read\",\n",
+                "        \"role\": \"read\",\n",
                 "    },\n",
                 "    supabase_client=account_hub_1,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
@@ -591,15 +594,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "sb_insert_collaborator(\n",
                 "    account_instance_fields={\n",
                 "        \"account_id\": account_id_3,\n",
                 "        \"instance_id\": instance[\"id\"],\n",
-                "        \"permission\": \"admin\",\n",
+                "        \"role\": \"admin\",\n",
                 "    },\n",
                 "    supabase_client=account_hub_1,\n",
                 ")\n",
                 "\n",
                 "sb_update_instance(\n",
                 "    instance_id=instance[\"id\"],\n",
                 "    instance_fields={\"description\": \"Description\"},\n",
```

### Comparing `lnhub_rest-0.7rc1/docs/migration/01-migration.ipynb` & `lnhub_rest-0.8.1/docs/organization/03-rls.ipynb`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8784058452276157%*

 * *Differences: {"'cells'": "{0: {'source': ['# Test RLS on organization membership management (organization_user "*

 * *            "table)']}, 1: {'metadata': {replace: OrderedDict()}, 'source': {insert: [(0, 'import "*

 * *            "sqlmodel as sqm\\n'), (1, 'import pytest\\n'), (3, '# Test assets\\n'), (4, 'from "*

 * *            "lnhub_rest.core.account import create_organization_account\\n'), (5, '\\n'), (6, '# "*

 * *            "Test utils\\n'), (7, 'from lnhub_rest.utils._test import create_test_auth, "*

 * *            "create_test_a […]*

```diff
@@ -1,210 +1,221 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Test migration"
+                "# Test RLS on organization membership management (organization_user table)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "import os\n",
+                "import sqlmodel as sqm\n",
+                "import pytest\n",
+                "\n",
+                "# Test assets\n",
+                "from lnhub_rest.core.account import create_organization_account\n",
                 "\n",
-                "os.chdir(\"../../\")"
+                "# Test utils\n",
+                "from lnhub_rest.utils._test import create_test_auth, create_test_account\n",
+                "from lnhub_rest._sbclient import connect_hub_with_auth\n",
+                "from lnhub_rest.main import client\n",
+                "from lnhub_rest._clean_ci import clean_ci\n",
+                "from lnhub_rest.utils._id import base62"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Parametrize"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "import time\n",
-                "from subprocess import run\n",
-                "from typing import Optional\n",
-                "\n",
-                "import erdiagram\n",
-                "import sqlalchemy as sa\n",
-                "from lamin_logger import logger\n",
-                "from lndb._settings import InstanceSettings, settings\n",
-                "from lndb.test import get_package_name\n",
-                "from lndb.test._migrations_unit import (\n",
-                "    execute_model_definitions_match_ddl,\n",
-                "    get_migration_config,\n",
-                "    get_migration_id_from_scripts,\n",
-                "    migration_id_is_consistent,\n",
-                ")\n",
-                "from pytest_alembic.executor import CommandExecutor, ConnectionExecutor\n",
-                "from pytest_alembic.runner import MigrationContext\n",
-                "from sqlalchemy import MetaData, create_engine, func, select\n",
-                "\n",
-                "from lnhub_rest import engine\n",
-                "from lnhub_rest.schema._core import SQLModel  # updated registry in it!\n",
-                "from lnhub_rest.schema.migrations.settings import PROD_URL\n",
-                "from lnhub_rest.schema.migrations.utils import include_name\n",
-                "from lndb.dev._clone import clone_test\n",
-                "\n",
-                "from sqlalchemy import text\n",
-                "\n",
-                "from lnhub_rest.schema.migrations.function._2023_02_21_a88f5298b8f7_v0_4_2 import (\n",
-                "    sql_functions,\n",
-                ")\n",
-                "from lnhub_rest.schema.migrations.rls._2023_02_21_a88f5298b8f7_v0_4_2 import (\n",
-                "    sql_rls_account,\n",
-                "    sql_rls_account_instance,\n",
-                "    sql_rls_instance,\n",
-                "    sql_rls_migration,\n",
-                "    sql_rls_storage,\n",
-                "    sql_rls_version,\n",
+                "# Create account 1\n",
+                "auth_1 = create_test_auth()\n",
+                "access_token_1 = auth_1[\"access_token\"]\n",
+                "account_1 = create_test_account(handle=auth_1[\"handle\"], access_token=access_token_1)\n",
+                "\n",
+                "# Create account 2\n",
+                "auth_2 = create_test_auth()\n",
+                "access_token_2 = auth_2[\"access_token\"]\n",
+                "account_2 = create_test_account(handle=auth_2[\"handle\"], access_token=access_token_2)\n",
+                "\n",
+                "# Create account 3\n",
+                "auth_3 = create_test_auth()\n",
+                "access_token_3 = auth_3[\"access_token\"]\n",
+                "account_3 = create_test_account(handle=auth_3[\"handle\"], access_token=access_token_3)\n",
+                "\n",
+                "# Create organization account\n",
+                "org_handle_1 = f\"lamin.ci.org.{base62(8)}\"\n",
+                "organization = create_organization_account(\n",
+                "    handle=org_handle_1, _access_token=access_token_1\n",
                 ")\n",
-                "from lnhub_rest.schema.migrations.rls._2023_03_09_0c4d4fe5f2c6_v0_6_1 import (\n",
-                "    sql_rls_migration as sql_rls_migration_2,\n",
-                "    sql_rls_version as sql_rls_version_2,\n",
-                ")\n",
-                "from lnhub_rest.schema.migrations.rls._2023_03_24_333fd693eac8_v0_6_1b import (\n",
-                "    sql_rls_owner_select_collaborators,\n",
+                "hub = connect_hub_with_auth(access_token=access_token_1)\n",
+                "organization_id = (\n",
+                "    hub.table(\"account\").select(\"id\").eq(\"handle\", org_handle_1).execute().data[0][\"id\"]\n",
                 ")"
             ]
         },
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Enable members to select other members"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Add a member to the organization."
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "package_name = get_package_name()\n",
-                "schema_package_loc = f\"./{package_name}/schema\""
+                "client.post(\n",
+                "    f\"organization/resources/members/{organization_id}/?user_id={account_2['id']}\",\n",
+                "    headers={\"authentication\": f\"Bearer {access_token_1}\"},\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Member should be able to select all members of the organization."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "def get_migration_context(schema_package_loc):\n",
-                "    src_settings = InstanceSettings(\n",
-                "        storage_root=\"teststore\",\n",
-                "        db=PROD_URL,\n",
-                "        name=\"testdb\",\n",
-                "        owner=\"testuser1\",\n",
-                "    )\n",
-                "    connection_string = clone_test(src_settings=src_settings, supabase=True)\n",
-                "    engine = sa.create_engine(connection_string, future=True)\n",
-                "    target_metadata = SQLModel.metadata\n",
-                "    config = get_migration_config(\n",
-                "        schema_package_loc,\n",
-                "        target_metadata=target_metadata,\n",
-                "        include_schemas=True,\n",
-                "        include_name=include_name,\n",
-                "    )\n",
-                "    command_executor = CommandExecutor.from_config(config)\n",
-                "    command_executor.configure(connection=engine)\n",
-                "    migration_context = MigrationContext.from_config(\n",
-                "        config, command_executor, ConnectionExecutor(), engine\n",
-                "    )\n",
-                "    # clone_test is currently only copying tables\n",
-                "    # so we need to create existing RLS and functions manually\n",
-                "    create_functions_and_rls(engine)\n",
-                "    return migration_context\n",
-                "\n",
-                "\n",
-                "def create_functions_and_rls(engine):\n",
-                "    with engine.connect() as conn:\n",
-                "        conn.execute(text(sql_functions))\n",
-                "        conn.execute(text(sql_rls_account))\n",
-                "        conn.execute(text(sql_rls_account_instance))\n",
-                "        conn.execute(text(sql_rls_instance))\n",
-                "        conn.execute(text(sql_rls_migration))\n",
-                "        conn.execute(text(sql_rls_storage))\n",
-                "        conn.execute(text(sql_rls_version))\n",
-                "        conn.execute(text(sql_rls_migration_2))\n",
-                "        conn.execute(text(sql_rls_version_2))\n",
-                "        # conn.execute(text(sql_rls_owner_select_collaborators))\n",
-                "        conn.commit()\n",
-                "\n",
+                "response = client.get(\n",
+                "    f\"organization/resources/members/{organization_id}\",\n",
+                "    headers={\"authentication\": f\"Bearer {access_token_2}\"},\n",
+                ").json()\n",
                 "\n",
-                "def test_migration_id_is_consistent():\n",
-                "    assert migration_id_is_consistent(schema_package_loc)\n",
-                "\n",
-                "\n",
-                "def test_model_definitions_match_ddl_postgres():\n",
-                "    migration_context = get_migration_context(schema_package_loc)\n",
-                "    execute_model_definitions_match_ddl(migration_context)\n",
-                "\n",
-                "\n",
-                "def test_export_schema():\n",
-                "    migration_id = get_migration_id_from_scripts(schema_package_loc)\n",
-                "    metadata = sa.MetaData(bind=engine)\n",
-                "    metadata.reflect()\n",
-                "    graph = erdiagram.create_schema_graph(\n",
-                "        metadata=metadata,\n",
-                "        show_datatypes=False,\n",
-                "        show_indexes=False,\n",
-                "        rankdir=\"LR\",\n",
-                "        concentrate=True,\n",
-                "    )\n",
-                "    try:\n",
-                "        graph.write_svg(f\"./docs/_schemas/lnhub-schema-{migration_id}.svg\")\n",
-                "    except FileNotFoundError:\n",
-                "        print(\"Did not write schema graph.\")"
+                "assert len(response) == 2"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Enable owners to add members"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Non-owner member should not be able to add other members."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from lnhub_rest.schema.migrations.versions import *"
+                "with pytest.raises(Exception) as error:\n",
+                "    response = client.post(\n",
+                "        f\"organization/resources/members/{organization_id}/?user_id={account_3['id']}\",\n",
+                "        headers={\"authentication\": f\"Bearer {access_token_2}\"},\n",
+                "    ).json()\n",
+                "\n",
+                "assert \"new row violates row-level security policy\" in error.value.message"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Enable owners to update members"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Non-owner member should not be able to update other members."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "test_migration_id_is_consistent()"
+                "response = client.put(\n",
+                "    f\"organization/resources/members/{organization_id}/?user_id={account_1['id']}&role=member\",\n",
+                "    headers={\"authentication\": f\"Bearer {access_token_2}\"},\n",
+                ").json()\n",
+                "\n",
+                "assert response == \"member-not-updated\""
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Enable owners to delete members"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Non-owner member should not be able to delete other members."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {
-                "tags": []
-            },
+            "metadata": {},
             "outputs": [],
             "source": [
-                "test_model_definitions_match_ddl_postgres()"
+                "response = client.delete(\n",
+                "    f\"organization/resources/members/{organization_id}/?user_id={account_1['id']}\",\n",
+                "    headers={\"authentication\": f\"Bearer {access_token_2}\"},\n",
+                ").json()\n",
+                "\n",
+                "assert response == \"member-not-deleted\""
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Clean up test assets"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "test_export_schema()"
+                "clean_ci()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -216,18 +227,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.13"
-        },
-        "vscode": {
-            "interpreter": {
-                "hash": "2841734f87827db3a7b3181a6051fe720e9968e703956c2bd6988b5a29362801"
-            }
+            "version": "3.9.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `lnhub_rest-0.7rc1/docs/migrations.md` & `lnhub_rest-0.8.1/docs/migrations.md`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/notes/multiple-sign-ups-same-email.ipynb` & `lnhub_rest-0.8.1/docs/notes/multiple-sign-ups-same-email.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994918699186992%*

 * *Differences: {"'cells'": "{37: {'source': ['hub.auth.sign_in_with_password(\\n', '    {\\n', '        "*

 * *            '"email": settings.email,\\n\', \'        "password": password1,\\n\', \'    }\\n\', '*

 * *            "')']}, 39: {'source': ['hub.auth.sign_in_with_password(\\n', '    {\\n', '        "*

 * *            '"email": settings.email,\\n\', \'        "password": password2,\\n\', \'    }\\n\', '*

 * *            "')']}}"}*

```diff
@@ -553,15 +553,20 @@
                     },
                     "execution_count": 31,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "hub.auth.sign_in(email=settings.email, password=password1)"
+                "hub.auth.sign_in_with_password(\n",
+                "    {\n",
+                "        \"email\": settings.email,\n",
+                "        \"password\": password1,\n",
+                "    }\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e41c4704-0a74-4be6-8a93-c24e41bfb4b2",
             "metadata": {},
             "source": [
@@ -593,15 +598,20 @@
                         "File \u001b[0;32m/opt/anaconda3/envs/base1/lib/python3.9/site-packages/gotrue/types.py:26\u001b[0m, in \u001b[0;36mBaseModelFromResponse.parse_response\u001b[0;34m(cls, response)\u001b[0m\n\u001b[1;32m     24\u001b[0m \u001b[38;5;129m@classmethod\u001b[39m\n\u001b[1;32m     25\u001b[0m \u001b[38;5;28;01mdef\u001b[39;00m \u001b[38;5;21mparse_response\u001b[39m(\u001b[38;5;28mcls\u001b[39m: Type[T], response: Response) \u001b[38;5;241m-\u001b[39m\u001b[38;5;241m>\u001b[39m T:\n\u001b[0;32m---> 26\u001b[0m     \u001b[43mcheck_response\u001b[49m\u001b[43m(\u001b[49m\u001b[43mresponse\u001b[49m\u001b[43m)\u001b[49m\n\u001b[1;32m     27\u001b[0m     \u001b[38;5;28;01mreturn\u001b[39;00m \u001b[38;5;28mcls\u001b[39m\u001b[38;5;241m.\u001b[39mparse_obj(response\u001b[38;5;241m.\u001b[39mjson())\n",
                         "File \u001b[0;32m/opt/anaconda3/envs/base1/lib/python3.9/site-packages/gotrue/helpers.py:18\u001b[0m, in \u001b[0;36mcheck_response\u001b[0;34m(response)\u001b[0m\n\u001b[1;32m     16\u001b[0m     response\u001b[38;5;241m.\u001b[39mraise_for_status()\n\u001b[1;32m     17\u001b[0m \u001b[38;5;28;01mexcept\u001b[39;00m HTTPError:\n\u001b[0;32m---> 18\u001b[0m     \u001b[38;5;28;01mraise\u001b[39;00m APIError\u001b[38;5;241m.\u001b[39mfrom_dict(response\u001b[38;5;241m.\u001b[39mjson())\n",
                         "\u001b[0;31mAPIError\u001b[0m: "
                     ]
                 }
             ],
             "source": [
-                "hub.auth.sign_in(email=settings.email, password=password2)"
+                "hub.auth.sign_in_with_password(\n",
+                "    {\n",
+                "        \"email\": settings.email,\n",
+                "        \"password\": password2,\n",
+                "    }\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "21b389b7-b362-41d0-8944-60df78e465ee",
             "metadata": {},
```

### Comparing `lnhub_rest-0.7rc1/docs/storage/01-add-storage.ipynb` & `lnhub_rest-0.8.1/docs/storage/01-add-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/docs/storage/02-rls.ipynb` & `lnhub_rest-0.8.1/docs/storage/02-rls.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993885281385282%*

 * *Differences: {"'cells'": "{6: {'source': ['storage_id = uuid4().hex\\n', 'storage_lnid = (base62(8),)']}, 8: "*

 * *            '{\'source\': {insert: [(4, \'            "lnid": storage_lnid,\\n\'), (5, '*

 * *            '\'            "created_by": account_id_1,\\n\')], delete: [4]}}, 10: {\'source\': '*

 * *            '{insert: [(4, \'            "lnid": storage_lnid,\\n\'), (5, \'            '*

 * *            '"created_by": account_id_1,\\n\')], delete: [4]}}, 12: {\'source\': {insert: [(3, '*

 * *            '\'        "lnid": storage_ln […]*

```diff
@@ -90,15 +90,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "storage_id = uuid4().hex"
+                "storage_id = uuid4().hex\n",
+                "storage_lnid = (base62(8),)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "With an anonymous Supabase client"
@@ -110,15 +111,16 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "with pytest.raises(Exception) as error:\n",
                 "    storage = sb_insert_storage(\n",
                 "        storage_fields={\n",
                 "            \"id\": storage_id,\n",
-                "            \"account_id\": account_id_1,\n",
+                "            \"lnid\": storage_lnid,\n",
+                "            \"created_by\": account_id_1,\n",
                 "            \"root\": f\"lamin.ci.storage.{base62(6)}\",\n",
                 "            \"region\": \"us-east-1\",\n",
                 "            \"type\": \"s3\",\n",
                 "        },\n",
                 "        supabase_client=hub,\n",
                 "    )\n",
                 "\n",
@@ -138,15 +140,16 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "with pytest.raises(Exception) as error:\n",
                 "    storage = sb_insert_storage(\n",
                 "        storage_fields={\n",
                 "            \"id\": storage_id,\n",
-                "            \"account_id\": account_id_1,\n",
+                "            \"lnid\": storage_lnid,\n",
+                "            \"created_by\": account_id_1,\n",
                 "            \"root\": f\"lamin.ci.storage.{base62(6)}\",\n",
                 "            \"region\": \"us-east-1\",\n",
                 "            \"type\": \"s3\",\n",
                 "        },\n",
                 "        supabase_client=account_hub_2,\n",
                 "    )\n",
                 "\n",
@@ -165,15 +168,16 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "storage = sb_insert_storage(\n",
                 "    storage_fields={\n",
                 "        \"id\": storage_id,\n",
-                "        \"account_id\": account_id_1,\n",
+                "        \"lnid\": storage_lnid,\n",
+                "        \"created_by\": account_id_1,\n",
                 "        \"root\": f\"lamin.ci.storage.{base62(6)}\",\n",
                 "        \"region\": \"us-east-1\",\n",
                 "        \"type\": \"s3\",\n",
                 "    },\n",
                 "    supabase_client=account_hub_1,\n",
                 ")\n",
                 "\n",
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/__main__.py` & `lnhub_rest-0.8.1/lnhub_rest/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import Literal, Optional
 
 import sqlmodel as sqm
 from lamin_logger import logger
 from packaging.version import parse as vparse
 from typeguard import typechecked
 
+from lnhub_rest._ci import start_local_supabase
+
 description_cli = "Manage hub."
 parser = argparse.ArgumentParser(
     description=description_cli, formatter_class=argparse.RawTextHelpFormatter
 )
 subparsers = parser.add_subparsers(dest="command")
 
 # migrate
@@ -116,15 +118,14 @@
         shell=True,
     )
 
 
 @typechecked
 def deploy(breaks_lndb: Optional[Literal["y", "n"]] = None):
     from lndb import settings
-
     from lnhub_rest._engine import engine
     from lnhub_rest.schema import __version__, _migration
     from lnhub_rest.schema.versions import version_cbwk
 
     if len(__version__.split(".")) != 3:
         raise RuntimeError("Your __version__ string is not of form X.X.X")
 
@@ -187,14 +188,16 @@
             ss.commit()
 
         logger.success("Successfully migrated hub.")
 
 
 def run_server():
     lamin_env = check_lamin_env()
+    if lamin_env == "local":
+        start_local_supabase()
     check_env_supabase_url(lamin_env)
     check_env_supabase_anon_key(lamin_env)
 
     run(
         "python3 ./lnhub_rest/main.py",
         shell=True,
     )
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/_assets/_instances.py` & `lnhub_rest-0.8.1/lnhub_rest/_assets/_instances.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/_assets/_schemas.py` & `lnhub_rest-0.8.1/lnhub_rest/_assets/_schemas.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/_check_breaks_lndb.py` & `lnhub_rest-0.8.1/lnhub_rest/_check_breaks_lndb.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Union
 
+from lamin_logger import logger
 from packaging.version import parse as vparse
 
 from lnhub_rest import __version__ as installed_version
 
 
 def check_breaks_lndb(hub) -> Union[bool, str]:
     """Check whether lndb client breaks because it's not up-to-date."""
@@ -32,11 +33,12 @@
 
 
 def check_breaks_lndb_and_error(hub) -> None:
     result = check_breaks_lndb(hub)
     if isinstance(result, str):
         raise RuntimeError(result)
     elif result:
-        raise SystemExit(
-            "Your lnhub_rest installation is out-of-date.\n"
-            "Please upgrade: pip install lnhub_rest -U"
+        logger.warning(
+            "Your lamindb installation is out-of-date and "
+            "might produce errors when interacting with the hub.\n"
+            "Please upgrade: pip install lamindb -U"
         )
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/_clean_ci.py` & `lnhub_rest-0.8.1/lnhub_rest/_clean_ci.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,29 +108,40 @@
         delete
         from storage
         where root like 'lamin.ci.storage.%'
         and created_at < '{str(datetime.now() - timedelta(minutes=20))}';
 
         delete
         from storage
-        where account_id in (
+        where created_by in (
           select id
           from account
           where handle like 'lamin.ci.user.%'
           and created_at < '{str(datetime.now() - timedelta(minutes=20))}'
         );
 
-        -- 4. delete entries from account
+        -- 4. delete entries from organization_user
+
+        delete
+        from organization_user
+        where organization_id in (
+          select id
+          from account
+          where handle like 'lamin.ci.org.%'
+          and created_at < '{str(datetime.now() - timedelta(minutes=20))}'
+        );
+
+        -- 5. delete entries from account
 
         delete
         from account
-        where handle like 'lamin.ci.user.%'
+        where (handle like 'lamin.ci.user.%' or handle like 'lamin.ci.org.%')
         and created_at < '{str(datetime.now() - timedelta(minutes=20))}';
 
-        -- 5. delete entries from auth.users
+        -- 6. delete entries from auth.users
 
         delete
         from auth.users
         where email like 'lamin.ci.user.%'
         and created_at < '{str(datetime.now() - timedelta(minutes=20))}';
     """
 
@@ -178,15 +189,15 @@
 
         delete
         from storage
         where root like 'lamin.ci.storage.{runId}'
 
         delete
         from storage
-        where account_id in (
+        where created_by in (
           select id
           from account
           where handle like 'lamin.ci.user.{runId}'
         );
 
         -- 4. delete entries from account
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/account/_create_account.py` & `lnhub_rest-0.8.1/lnhub_rest/core/account/_create_account.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,85 @@
-from typing import Optional, Union
+from typing import Union
+from uuid import uuid4
 
 from postgrest.exceptions import APIError
 
 from lnhub_rest._sbclient import connect_hub_with_auth
 from lnhub_rest.core.account._crud import sb_insert_account
+from lnhub_rest.core.member._crud import sb_insert_member
 from lnhub_rest.utils._access_token import extract_id
 from lnhub_rest.utils._id import base62
 
 
-def create_account(
+def create_user_account(
     _access_token: str,
     handle: str,
-    organization: Optional[bool] = False,
 ) -> Union[None, str]:
     hub = connect_hub_with_auth(access_token=_access_token)
     try:
         lnid = base62(8)
         id = extract_id(_access_token)
 
         account = sb_insert_account(
             {
                 "id": id,
-                "user_id": id if not organization else None,
+                "user_id": id,
                 "lnid": lnid,
                 "handle": handle,
             },
             hub,
         )
         assert account is not None
 
         return None
     except APIError as api_error:
         usermeta_pkey_error = (
             'duplicate key value violates unique constraint "usermeta_pkey"'
         )
         if api_error.message == usermeta_pkey_error:
+            return "handle-exists-already"
+        raise api_error
+    except Exception as e:
+        raise e
+    finally:
+        hub.auth.sign_out()
+
+
+def create_organization_account(handle: str, _access_token: str) -> Union[None, str]:
+    hub = connect_hub_with_auth(access_token=_access_token)
+    try:
+        lnid = base62(8)
+
+        organization = sb_insert_account(
+            {
+                "id": uuid4().hex,
+                "user_id": None,
+                "lnid": lnid,
+                "handle": handle,
+            },
+            hub,
+        )
+        assert organization is not None
+
+        user_id = extract_id(_access_token)
+        member = sb_insert_member(
+            {
+                "organization_id": organization["id"],
+                "user_id": user_id,
+                "role": "owner",
+            },
+            hub,
+        )
+        assert member is not None
+
+        return None
+    except APIError as api_error:
+        usermeta_pkey_error = (
+            'duplicate key value violates unique constraint "usermeta_pkey"'
+        )
+        if api_error.message == usermeta_pkey_error:
             return "handle-exists-already"
         raise api_error
     except Exception as e:
         raise e
     finally:
         hub.auth.sign_out()
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/account/_crud.py` & `lnhub_rest-0.8.1/lnhub_rest/core/account/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/account/_delete_account.py` & `lnhub_rest-0.8.1/lnhub_rest/core/account/_delete_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/account/_signup_signin.py` & `lnhub_rest-0.8.1/lnhub_rest/core/account/_signup_signin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from lamin_logger import logger
 
 from lnhub_rest import check_breaks_lndb_and_error
+from lnhub_rest.utils._id import secret
 
 from ..._sbclient import connect_hub, get_lamin_site_base_url
 
 
 def sign_up_hub(email) -> str:
     from lndb._settings_store import settings_dir
-    from lnschema_core.dev import id
 
     hub = connect_hub()
     check_breaks_lndb_and_error(hub)
-    password = id.secret()  # generate new password
+    password = secret()  # generate new password
     auth_response = hub.auth.sign_up(
         {
             "email": email,
             "password": password,
             "options": {"redirect_to": f"{get_lamin_site_base_url()}/signup"},
         }
     )
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/account/_update_account.py` & `lnhub_rest-0.8.1/lnhub_rest/core/account/_update_account.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/collaborator/_crud.py` & `lnhub_rest-0.8.1/lnhub_rest/core/collaborator/_crud.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     data = (
         supabase_client.table("account_instance")
         .select("*")
         .eq("instance_id", instance_id)
         .execute()
         .data
     )
+    if len(data) == 0:
+        return None
     return data
 
 
 def sb_select_collaborator(
     instance_id: str,
     account_id: str,
     supabase_client: Client,
@@ -52,20 +54,20 @@
         return None
     return data[0]
 
 
 def sb_update_collaborator(
     instance_id: str,
     account_id: str,
-    permission: str,
+    role: str,
     supabase_client: Client,
 ):
     data = (
         supabase_client.table("account_instance")
-        .update({"permission": permission})
+        .update({"role": role})
         .eq("instance_id", instance_id)
         .eq("account_id", account_id)
         .execute()
         .data
     )
     if len(data) == 0:
         return None
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/instance/_crud.py` & `lnhub_rest-0.8.1/lnhub_rest/core/instance/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/instance/_delete_instance.py` & `lnhub_rest-0.8.1/lnhub_rest/core/instance/_delete_instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Optional, Union
 
 from lnhub_rest import check_breaks_lndb_and_error
 from lnhub_rest._sbclient import connect_hub_with_auth
 from lnhub_rest.core.account._crud import sb_select_account_by_handle
-from lnhub_rest.core.collaborator._crud import sb_delete_all_collaborators_from_instance
 from lnhub_rest.core.instance._crud import (
     sb_delete_instance,
     sb_select_instance_by_name,
 )
 
 
 def delete_instance(
@@ -29,15 +28,14 @@
             return "account-not-exists"
 
         # get instance
         instance = sb_select_instance_by_name(account["id"], name, hub)
         if instance is None:
             return "instance-not-reachable"
 
-        sb_delete_all_collaborators_from_instance(instance["id"], hub)
         sb_delete_instance(instance["id"], hub)
 
         # TODO: delete storage if no other instances use it
         return None
     except Exception as e:
         return str(e)
     finally:
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/instance/_init_instance.py` & `lnhub_rest-0.8.1/lnhub_rest/core/instance/_init_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             hub,
         )
 
         sb_insert_collaborator(
             {
                 "instance_id": instance_id,
                 "account_id": account["id"],
-                "permission": "admin",
+                "role": "admin",
             },
             hub,
         )
 
         # upon successful insert of a new row in the instance table
         # (and all associated tables), return None
         # clients test for this return value, hence, don't change it
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/instance/_load_instance.py` & `lnhub_rest-0.8.1/lnhub_rest/core/instance/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/instance/_update_instance.py` & `lnhub_rest-0.8.1/lnhub_rest/core/instance/_update_instance.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/storage/_add_storage.py` & `lnhub_rest-0.8.1/lnhub_rest/core/storage/_add_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from typing import Optional, Tuple
 from uuid import UUID, uuid4
 
 from lnhub_rest import check_breaks_lndb_and_error
 from lnhub_rest.core.storage._crud import sb_insert_storage, sb_select_storage_by_root
+from lnhub_rest.utils._id import base62
 
 from ..._sbclient import connect_hub_with_auth
 
 
 def add_storage(
     root: str, account_handle: str, _access_token: Optional[str] = None
 ) -> Tuple[Optional[UUID], Optional[str]]:
@@ -32,15 +33,16 @@
             storage_region = None
         else:
             storage_region = get_storage_region(root)
         storage_type = get_storage_type(root)
         storage = sb_insert_storage(
             {
                 "id": uuid4().hex,
-                "account_id": account["id"],
+                "lnid": base62(8),
+                "created_by": account["id"],
                 "root": root,
                 "region": storage_region,
                 "type": storage_type,
             },
             hub,
         )
         assert storage is not None
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/core/storage/_crud.py` & `lnhub_rest-0.8.1/lnhub_rest/core/storage/_crud.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/orm/_sbclient.py` & `lnhub_rest-0.8.1/lnhub_rest/orm/_sbclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from typing import Optional
 from urllib.request import urlretrieve
 
 from pydantic import BaseSettings
 
+from lnhub_rest._ci import SUPABASE_LOCAL_ANON_KEY_FILE
 from supabase import create_client
 
 
 class Connector(BaseSettings):
     url: str
     key: str
 
@@ -22,15 +23,15 @@
 
 
 def connect_hub():
     if "LAMIN_ENV" in os.environ:
         if os.environ["LAMIN_ENV"] == "local":
             return create_client(
                 "http://localhost:54321",
-                open("../../.supabase_local_anon_key").read(),
+                open(SUPABASE_LOCAL_ANON_KEY_FILE).read(),
             )
         if os.environ["LAMIN_ENV"] == "staging":
             return create_client(
                 os.environ["SUPABASE_STAGING_URL"],
                 os.environ["SUPABASE_STAGING_ANON_KEY"],
             )
     connector_file, _ = urlretrieve(
@@ -70,11 +71,16 @@
         os.environ["SUPABASE_PROD_SERVICE_ROLE_KEY"],
     )
 
 
 def get_access_token(email: Optional[str] = None, password: Optional[str] = None):
     hub = connect_hub()
     try:
-        session = hub.auth.sign_in(email=email, password=password)
-        return session.access_token
+        auth_response = hub.auth.sign_in_with_password(
+            {
+                "email": email,
+                "password": password,
+            }
+        )
+        return auth_response.session.access_token
     finally:
         hub.auth.sign_out()
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/routers/account.py` & `lnhub_rest-0.8.1/lnhub_rest/routers/account.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,94 @@
-from typing import Union
+from typing import Annotated, Union
 
-from fastapi import APIRouter, Header
+from fastapi import APIRouter, Header, Query
 
-from ..core.account._create_account import create_account as create_account_base
+from ..core.account._create_account import (
+    create_organization_account,
+    create_user_account,
+)
 from ..core.account._update_account import update_account as update_account_base
 from .utils import extract_access_token, get_supabase_client, supabase_client
 
 router = APIRouter(prefix="/account")
 
 
+@router.post("/")
+def create_account(
+    handle: str,
+    organization: Union[bool, None] = False,
+    authentication: Union[str, None] = Header(default=None),
+):
+    access_token = extract_access_token(authentication)
+    if organization:
+        message = create_organization_account(
+            handle=handle,
+            _access_token=access_token,
+        )
+    else:
+        message = create_user_account(
+            handle=handle,
+            _access_token=access_token,
+        )
+    if message is None:
+        return "success"
+    return message
+
+
+@router.put("/")
+def update_account(
+    handle: Union[str, None] = None,
+    name: Union[str, None] = None,
+    bio: Union[str, None] = None,
+    github_handle: Union[str, None] = None,
+    linkedin_handle: Union[str, None] = None,
+    twitter_handle: Union[str, None] = None,
+    website: Union[str, None] = None,
+    authentication: Union[str, None] = Header(default=None),
+):
+    access_token = extract_access_token(authentication)
+    message = update_account_base(
+        handle=handle,
+        name=name,
+        bio=bio,
+        github_handle=github_handle,
+        linkedin_handle=linkedin_handle,
+        twitter_handle=twitter_handle,
+        website=website,
+        _access_token=access_token,
+    )
+    if message is None:
+        return "success"
+    return message
+
+
+@router.get("/bulk/avatars")
+def get_account_avatars(lnids: Annotated[list[str], Query()]):
+    data = (
+        supabase_client.table("account")
+        .select("lnid, avatar_url")
+        .in_("lnid", lnids)
+        .execute()
+        .data
+    )
+    return data if len(data) > 0 else []
+
+
+@router.get("/avatar")
+def get_account_avatar(lnid: str):
+    data = (
+        supabase_client.table("account")
+        .select("avatar_url")
+        .eq("lnid", lnid)
+        .execute()
+        .data
+    )
+    return data[0]["avatar_url"] if len(data) > 0 else None
+
+
 @router.get("/{id}")
 def get_account_by_id(id: str):
     data = supabase_client.table("account").select("*").eq("id", id).execute().data
     return data[0] if len(data) > 0 else None
 
 
 @router.get("/handle/{handle}")
@@ -46,49 +122,27 @@
 
         return account_instances
 
     finally:
         supabase_client.auth.sign_out()
 
 
-@router.post("/")
-def create_account(
-    handle: str,
-    organization: Union[bool, None] = False,
-    authentication: Union[str, None] = Header(default=None),
+@router.get("/resources/organizations/{handle}")
+def get_account_organizations(
+    handle: str, authentication: Union[str, None] = Header(default=None)
 ):
     access_token = extract_access_token(authentication)
-    message = create_account_base(
-        handle=handle,
-        organization=organization,
-        _access_token=access_token,
-    )
-    if message is None:
-        return "success"
-    return message
+    supabase_client = get_supabase_client(access_token)
 
+    try:
+        user_id = get_account_by_handle(handle)["id"]
+        organizations_user = (
+            supabase_client.table("organization_user")
+            .select()
+            .eq("user_id", user_id)
+            .execute()
+            .data
+        )
+        return organizations_user if len(organizations_user) > 0 else None
 
-@router.put("/")
-def update_account(
-    handle: Union[str, None] = None,
-    name: Union[str, None] = None,
-    bio: Union[str, None] = None,
-    github_handle: Union[str, None] = None,
-    linkedin_handle: Union[str, None] = None,
-    twitter_handle: Union[str, None] = None,
-    website: Union[str, None] = None,
-    authentication: Union[str, None] = Header(default=None),
-):
-    access_token = extract_access_token(authentication)
-    message = update_account_base(
-        handle=handle,
-        name=name,
-        bio=bio,
-        github_handle=github_handle,
-        linkedin_handle=linkedin_handle,
-        twitter_handle=twitter_handle,
-        website=website,
-        _access_token=access_token,
-    )
-    if message is None:
-        return "success"
-    return message
+    finally:
+        supabase_client.auth.sign_out()
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/routers/ci.py` & `lnhub_rest-0.8.1/lnhub_rest/routers/ci.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/routers/instance.py` & `lnhub_rest-0.8.1/lnhub_rest/routers/instance.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .._delete_instance import delete_instance as delete_instance_base
 from .._init_instance import init_instance as init_instance_base
 from ..core.instance._update_instance import update_instance as update_instance_base
 from .account import get_account_by_handle
 from .utils import (
     extract_access_token,
-    get_account_permission_for_instance,
+    get_account_role_for_instance,
     get_supabase_client,
 )
 
 router = APIRouter(prefix="/instance")
 
 
 @router.get("/{account_handle}/{name}")
@@ -36,24 +36,22 @@
             .execute()
             .data
         )
 
         if len(data) > 0:
             instance = data[0]
             if authentication is not None:
-                permission = get_account_permission_for_instance(
-                    data[0]["id"], access_token
-                )
+                role = get_account_role_for_instance(data[0]["id"], access_token)
             else:
-                permission = None
+                role = None
         else:
             instance = None
-            permission = None
+            role = None
 
-        return {"instance": instance, "permission": permission}
+        return {"instance": instance, "role": role}
 
     finally:
         supabase_client.auth.sign_out()
 
 
 @router.get("/resources/accounts/{account_handle}/{name}")
 def get_instance_accounts(
@@ -73,24 +71,22 @@
             .eq("name", name)
             .execute()
             .data
         )
         if len(data) > 0:
             account_instances = data[0]["account_instance"]
             if authentication is not None:
-                permission = get_account_permission_for_instance(
-                    data[0]["id"], access_token
-                )
+                role = get_account_role_for_instance(data[0]["id"], access_token)
             else:
-                permission = None
+                role = None
         else:
             account_instances = None
-            permission = None
+            role = None
 
-        return {"accounts": account_instances, "permission": permission}
+        return {"accounts": account_instances, "role": role}
 
     finally:
         supabase_client.auth.sign_out()
 
 
 @router.post("/")
 def create_instance(
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/routers/utils.py` & `lnhub_rest-0.8.1/lnhub_rest/routers/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 from fastapi import Header
 
 from .._sbclient import connect_hub, connect_hub_with_auth
 
 supabase_client = connect_hub()
 
 
-def get_account_permission_for_instance(instance_id: str, access_token: str):
+def get_account_role_for_instance(instance_id: str, access_token: str):
     supabase_client = connect_hub_with_auth(access_token=access_token)
     session_payload = jwt.decode(
         access_token, algorithms="HS256", options={"verify_signature": False}
     )
     data = (
         supabase_client.table("account_instance")
-        .select("permission")
+        .select("role")
         .eq("account_id", session_payload["sub"])
         .eq("instance_id", instance_id)
         .execute()
         .data
     )
-    return data[0]["permission"] if len(data) > 0 else None
+    return data[0]["role"] if len(data) > 0 else None
 
 
 def extract_access_token(authentication: Union[str, None] = Header(default=None)):
     if authentication is not None:
         return authentication.split(" ")[1]
     return None
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/_versions.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/_versions.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/alembic.ini` & `lnhub_rest-0.8.1/lnhub_rest/schema/alembic.ini`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/env.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
     "pk": "pk_%(table_name)s",
 }
 
 from lnhub_rest.schema import *  # noqa
 from lnhub_rest.schema import _schema_id  # noqa
 from lnhub_rest.schema.migrations.settings import SUPABASE_DB_URL as URL  # noqa
-from lnhub_rest.schema.migrations.utils import include_name  # noqa
+from lnhub_rest.schema.migrations.testing import include_name  # noqa
 
 
 def run_migrations_offline() -> None:
     """Run migrations in 'offline' mode.
 
     This configures the context with just a URL
     and not an Engine, though an Engine is acceptable
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/function/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_02_21_a88f5298b8f7_v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/rls/_2023_03_09_0c4d4fe5f2c6_v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/script.py.mako` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/settings.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/settings.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-13-53709f2a2043-v0_0_1a.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-13-53709f2a2043-v0_0_1a.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-13-c555c87a640c-v0_0_1.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-13-c555c87a640c-v0_0_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-14-f7ba9352c706-v0_0_2.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-14-f7ba9352c706-v0_0_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-23-c13c9dd0f3ae-v0_1_4a.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-23-c13c9dd0f3ae-v0_1_4a.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-24-e7151581f790-v0_1_4b.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-24-e7151581f790-v0_1_4b.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-01-30-2efe1dee9baf-v0_1_4c.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-01-30-2efe1dee9baf-v0_1_4c.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-06-95073282294e-v0_1_4e.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-06-95073282294e-v0_1_4e.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-06-9c02109e4faa-v0_2_0.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-06-9c02109e4faa-v0_2_0.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-06-f2cb77148a6e-v0_1_4d.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-06-f2cb77148a6e-v0_1_4d.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-15-641d1508baab-v0_4_0.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-15-641d1508baab-v0_4_0.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-16-1fdc05837919-v0_4_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-02-21-a88f5298b8f7-v0_4_2.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-03-09-0c4d4fe5f2c6-v0_6_1.py`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py` & `lnhub_rest-0.8.1/lnhub_rest/schema/migrations/versions/2023-03-24-333fd693eac8-v0_6_1b.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 
 """
 import sqlalchemy as sa  # noqa
 import sqlmodel  # noqa
 from alembic import op
 
 from lnhub_rest.schema.migrations.rls._2023_03_24_333fd693eac8_v0_6_1b import (
-    sql_rls_owner_select_collaborators,
+    sql_rls_account_instance_2,
 )
 
 # revision identifiers, used by Alembic.
 revision = "333fd693eac8"
 down_revision = "0c4d4fe5f2c6"
 branch_labels = None
 depends_on = None
 
 
 def upgrade() -> None:
-    op.execute(sql_rls_owner_select_collaborators)
+    op.execute(sql_rls_account_instance_2)
 
 
 def downgrade() -> None:
     pass
```

### Comparing `lnhub_rest-0.7rc1/lnhub_rest/utils/_test.py` & `lnhub_rest-0.8.1/lnhub_rest/utils/_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,16 @@
 
     root = f"lamin.ci.storage.{base62(6)}"
     account_id = extract_id(access_token)
 
     storage = sb_insert_storage(
         {
             "id": uuid.uuid4().hex,
-            "account_id": account_id,
+            "lnid": base62(8),
+            "created_by": account_id,
             "root": root,
             "region": "us-east-1",
             "type": "s3",
         },
         hub,
     )
 
@@ -133,24 +134,24 @@
 
     return storage
 
 
 def add_test_collaborator(
     instance_id: str,
     account_id: str,
-    permission: str,
+    role: str,
     access_token: str,
 ):
     hub = connect_hub_with_auth(access_token=access_token)
 
     collaborator = sb_insert_collaborator(
         {
             "instance_id": instance_id,
             "account_id": account_id,
-            "permission": permission,
+            "role": role,
         },
         hub,
     )
 
     hub.auth.sign_out()
 
     return collaborator
```

### Comparing `lnhub_rest-0.7rc1/noxfile.py` & `lnhub_rest-0.8.1/noxfile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,68 @@
 import os
 
 import nox
+from lamin_logger import logger
+from laminci.nox import login_testuser1, login_testuser2
 
 nox.options.reuse_existing_virtualenvs = True
 
+
+if "BRANCH_NAME" in os.environ:
+    branch_name = os.environ["BRANCH_NAME"]
+    logger.info(f"Using BRANCH_NAME {branch_name}")
+else:
+    logger.info("Env variable BRANCH_NAME not found")
+
+
 lamin_env = "local"
-if "GITHUB_REF_NAME" in os.environ:
-    if os.environ["GITHUB_REF_NAME"] == "main":
+if branch_name is not None:
+    if branch_name == "main":
         lamin_env = "prod"
-    # if running in GI and branch is not main, then always use staging credentials
-    else:
+    elif branch_name == "staging":
         lamin_env = "staging"
+    else:
+        lamin_env = "local"
 elif "LAMIN_ENV" in os.environ:
     lamin_env = os.environ["LAMIN_ENV"]
 
+logger.info(f"Setting LAMIN_ENV to {lamin_env}")
+
 
 @nox.session
 def lint(session: nox.Session) -> None:
     session.install("pre-commit")
     session.run("pre-commit", "install")
     session.run("pre-commit", "run", "--all-files")
 
 
-@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
-def build(session):
+@nox.session
+@nox.parametrize("package", ["lnhub-rest", "lndb"])
+def build(session: nox.Session, package: str):
+    session.install("./lndb[dev,test]")
     session.install(".[dev,test]")
     session.run(
         "pytest",
         "-s",
         "--cov=lnhub_rest",
         "--cov-append",
         "--cov-report=term-missing",
         env={"LN_SERVER_DEPLOY": "1", "LAMIN_ENV": lamin_env},
     )
-    # session.run("coverage", "xml")
+    if package == "lndb":
+        login_testuser1(session)
+        login_testuser2(session)
+        os.chdir(f"./{package}")
+        session.run(
+            "pytest",
+            "-s",
+            "./tests",
+            "--ignore",
+            "./tests/test_migrations.py",
+            env={"LAMIN_ENV": lamin_env},
+        )
 
 
 @nox.session
 def supabase_stop(session: nox.Session) -> None:
     session.run("supabase", "db", "reset", external=True)
     session.run("supabase", "stop", external=True)
```

### Comparing `lnhub_rest-0.7rc1/pyproject.toml` & `lnhub_rest-0.8.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,14 @@
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "nox",
 ]
 test = [
-    "lndb>=0.36.0",
-    "lnschema-core>=0.26.1",
     "pytest>=6.0",
     "pytest-cov",
     "nbproject",
 ]
 
 [project.scripts]
 lnhub = "lnhub_rest.__main__:main"
```

### Comparing `lnhub_rest-0.7rc1/supabase/config.toml` & `lnhub_rest-0.8.1/supabase/config.toml`

 * *Files identical despite different names*

### Comparing `lnhub_rest-0.7rc1/tests/test_notebooks.py` & `lnhub_rest-0.8.1/tests/test_notebooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,7 +20,10 @@
     test.execute_notebooks(docs_folder / "account/", write=True)
 
     logger.debug("\ninstance")
     test.execute_notebooks(docs_folder / "instance/", write=True)
 
     logger.debug("\nstorage")
     test.execute_notebooks(docs_folder / "storage/", write=True)
+
+    logger.debug("\norganization")
+    test.execute_notebooks(docs_folder / "organization/", write=True)
```

### Comparing `lnhub_rest-0.7rc1/PKG-INFO` & `lnhub_rest-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lnhub_rest
-Version: 0.7rc1
+Version: 0.8.1
 Summary: Rest API for the hub.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: supabase==1.0.2
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
@@ -18,16 +18,14 @@
 Requires-Dist: natsort
 Requires-Dist: pytest_alembic==0.9.1
 Requires-Dist: boto3==1.24.59
 Requires-Dist: botocore==1.27.59
 Requires-Dist: deepdiff
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
-Requires-Dist: lndb>=0.36.0 ; extra == "test"
-Requires-Dist: lnschema-core>=0.26.1 ; extra == "test"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lnhub-rest
 Provides-Extra: dev
 Provides-Extra: test
```

