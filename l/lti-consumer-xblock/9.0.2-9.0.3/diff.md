# Comparing `tmp/lti-consumer-xblock-9.0.2.tar.gz` & `tmp/lti-consumer-xblock-9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lti-consumer-xblock-9.0.2.tar", last modified: Wed Apr 12 16:57:11 2023, max compression
+gzip compressed data, was "lti-consumer-xblock-9.0.3.tar", last modified: Tue Apr 18 20:35:46 2023, max compression
```

## Comparing `lti-consumer-xblock-9.0.2.tar` & `lti-consumer-xblock-9.0.3.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.896233 lti-consumer-xblock-9.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-12 16:57:11.896233 lti-consumer-xblock-9.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.840233 lti-consumer-xblock-9.0.2/lti_consumer/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.844233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.844233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/django.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.844233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.844233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/test_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.848233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/ags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    32216 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.848233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.848233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/nprs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.852233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.852233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.852233 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    39510 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     9305 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    69931 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/lti_xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.864233 lti-consumer-xblock-9.0.2/lti_consumer/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0002_ltiagslineitem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0003_ltiagsscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0005_migrate_keyset_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0007_ltidlcontentitem.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0008_fix_uuid_backfill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0013_auto_20210712_1352.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0014_adds_external_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0015_add_additional_1p3_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/outcomes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.864233 lti-consumer-xblock-9.0.2/lti_consumer/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/plugin/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.868233 lti-consumer-xblock-9.0.2/lti_consumer/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.868233 lti-consumer-xblock-9.0.2/lti_consumer/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/static/css/student.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.868233 lti-consumer-xblock-9.0.2/lti_consumer/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)    10596 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/static/js/xblock_lti_consumer.js
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/static/js/xblock_studio_view.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.868233 lti-consumer-xblock-9.0.2/lti_consumer/static/sass/
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/static/sass/student.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.868233 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.876233 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/dl_response_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/dl_response_saved.html
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_dl_content.html
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_html.html
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_image.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_1p3_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_1p3_permission_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_1p3_studio.html
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_iframe.html
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_launch_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_proctoring_start_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/html/student.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.876233 lti-consumer-xblock-9.0.2/lti_consumer/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templates/xml/outcome_service_response.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.876233 lti-consumer-xblock-9.0.2/lti_consumer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templatetags/get_dl_lti_launch_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/templatetags/lti_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.876233 lti-consumer-xblock-9.0.2/lti_consumer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_proctoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    82946 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_lti_xblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/track.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10720 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.880233 lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.832233 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.884233 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.884233 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.884233 lti-consumer-xblock-9.0.2/lti_consumer/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.884233 lti-consumer-xblock-9.0.2/lti_consumer/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.888233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.888233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.888233 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1349 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.888233 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.892233 lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.836233 lti-consumer-xblock-9.0.2/lti_consumer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.892233 lti-consumer-xblock-9.0.2/lti_consumer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/lti_consumer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.892233 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-12 16:57:11.000000 lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 16:57:11.896233 lti-consumer-xblock-9.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-12 16:57:11.896233 lti-consumer-xblock-9.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-04-12 16:57:08.000000 lti-consumer-xblock-9.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.647995 lti-consumer-xblock-9.0.3/lti_consumer/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/django.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32648 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.655995 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/nprs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.655995 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.655995 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.655995 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39510 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    69931 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.659995 lti-consumer-xblock-9.0.3/lti_consumer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0002_ltiagslineitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0003_ltiagsscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0005_migrate_keyset_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0007_ltidlcontentitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0008_fix_uuid_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0013_auto_20210712_1352.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0014_adds_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0015_add_additional_1p3_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/outcomes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.663996 lti-consumer-xblock-9.0.3/lti_consumer/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/plugin/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.663996 lti-consumer-xblock-9.0.3/lti_consumer/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.639995 lti-consumer-xblock-9.0.3/lti_consumer/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.663996 lti-consumer-xblock-9.0.3/lti_consumer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/static/css/student.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.663996 lti-consumer-xblock-9.0.3/lti_consumer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    10596 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/static/js/xblock_lti_consumer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/static/js/xblock_studio_view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.663996 lti-consumer-xblock-9.0.3/lti_consumer/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/static/sass/student.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.639995 lti-consumer-xblock-9.0.3/lti_consumer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.667996 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.667996 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/dl_response_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/dl_response_saved.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_dl_content.html
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_html.html
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_image.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_1p3_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_1p3_permission_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_1p3_studio.html
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_launch_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_proctoring_start_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/student.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.667996 lti-consumer-xblock-9.0.3/lti_consumer/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/xml/outcome_service_response.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.667996 lti-consumer-xblock-9.0.3/lti_consumer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templatetags/get_dl_lti_launch_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templatetags/lti_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.667996 lti-consumer-xblock-9.0.3/lti_consumer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.671995 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.671995 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_proctoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82946 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_lti_xblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/track.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.671995 lti-consumer-xblock-9.0.3/lti_consumer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.639995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.671995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10720 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.671995 lti-consumer-xblock-9.0.3/lti_consumer/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1349 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/lti_consumer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      171 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-18 20:35:46.683996 lti-consumer-xblock-9.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/setup.py
```

### Comparing `lti-consumer-xblock-9.0.2/LICENSE` & `lti-consumer-xblock-9.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/NOTICE` & `lti-consumer-xblock-9.0.3/NOTICE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/PKG-INFO` & `lti-consumer-xblock-9.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.0.2
+Version: 9.0.3
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.0.2/README.rst` & `lti-consumer-xblock-9.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/admin.py` & `lti-consumer-xblock-9.0.3/lti_consumer/admin.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/api.py` & `lti-consumer-xblock-9.0.3/lti_consumer/api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/apps.py` & `lti-consumer-xblock-9.0.3/lti_consumer/apps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/data.py` & `lti-consumer-xblock-9.0.3/lti_consumer/data.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/filters.py` & `lti-consumer-xblock-9.0.3/lti_consumer/filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/forms.py` & `lti-consumer-xblock-9.0.3/lti_consumer/forms.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/consumer.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/django.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/contrib/tests/test_django.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/oauth.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/test_consumer.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p1/tests/test_oauth.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/ags.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/constants.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/constants.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/consumer.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,18 +413,28 @@
             A dict containing the JSON response containing a JWT and some extra
             parameters required by LTI tools. This token gives access to all
             supported LTI Scopes from this tool.
         """
         # Check if all required claims are present
         for required_claim in LTI_1P3_ACCESS_TOKEN_REQUIRED_CLAIMS:
             if required_claim not in token_request_data.keys():
-                raise exceptions.MissingRequiredClaim(f'The required claim {required_claim} is missing from the JWT.')
+                error_msg = (
+                    f'The required claim {required_claim} is missing from the OAuth 2.0 Client-Credentials '
+                    'Grant JWT.'
+                )
+                log.warning(error_msg)
+                raise exceptions.MissingRequiredClaim(error_msg)
 
         # Check that grant type is `client_credentials`
-        if token_request_data['grant_type'] != 'client_credentials':
+        grant_type = token_request_data['grant_type']
+        if grant_type != 'client_credentials':
+            log.warning(
+                'The required grant_type parameter in the OAuth 2.0 Client-Credentials Grant JWT was expected to be '
+                f'client_credentials but was {grant_type} instead.'
+            )
             raise exceptions.UnsupportedGrantType()
 
         # Validate JWT token
         self.tool_jwt.validate_and_decode(
             token_request_data['client_assertion']
         )
```

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/deep_linking.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/exceptions.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/exceptions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/extensions/rest_framework/utils.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/key_handlers.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/key_handlers.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 This handles validating messages sent by the tool and generating
 access token with LTI scopes.
 """
 import codecs
 import copy
 import time
 import json
+import logging
 
 from Cryptodome.PublicKey import RSA
 from jwkest import BadSignature, BadSyntax, WrongNumberOfParts, jwk
 from jwkest.jwk import RSAKey, load_jwks_from_url
-from jwkest.jws import JWS, NoSuitableSigningKeys
+from jwkest.jws import JWS, NoSuitableSigningKeys, UnknownAlgorithm
 from jwkest.jwt import JWT
 
 from . import exceptions
 
+log = logging.getLogger(__name__)
+
 
 class ToolKeyHandler:
     """
     LTI 1.3 Tool Jwt Handler.
 
     Uses a tool public keys or keysets URL to retrieve
     a key and validate a message sent by the tool.
@@ -52,14 +55,18 @@
                 # Unescape key before importing it
                 raw_key = codecs.decode(public_key, 'unicode_escape')
 
                 # Import Key and save to internal state
                 new_key.load_key(RSA.import_key(raw_key))
                 self.public_key = new_key
             except ValueError as err:
+                log.warning(
+                    'An error was encountered while loading the LTI tool\'s key from the public key. '
+                    'The RSA key could not parsed.'
+                )
                 raise exceptions.InvalidRsaKey() from err
 
     def _get_keyset(self, kid=None):
         """
         Get keyset from available sources.
 
         If using a RSA key, forcefully set the key id
@@ -71,14 +78,18 @@
             try:
                 keys = load_jwks_from_url(self.keyset_url)
             except Exception as err:
                 # Broad Exception is required here because jwkest raises
                 # an Exception object explicitly.
                 # Beware that many different scenarios are being handled
                 # as an invalid key when the JWK loading fails.
+                log.warning(
+                    'An error was encountered while importing the LTI tool\'s keys from a JWKS URL. '
+                    'The RSA keys could not be loaded.'
+                )
                 raise exceptions.NoSuitableKeys() from err
             keyset.extend(keys)
 
         if self.public_key and kid:
             # Fill in key id of stored key.
             # This is needed because if the JWS is signed with a
             # key with a kid, pyjwkest doesn't match them with
@@ -109,26 +120,42 @@
                 keys=self._get_keyset(
                     jwt.headers.get('kid')
                 )
             )
 
             # If message is valid, check expiration from JWT
             if 'exp' in message and message['exp'] < time.time():
+                log.warning(
+                    'An error was encountered while verifying the OAuth 2.0 Client-Credentials Grant JWT. '
+                    'The JWT has expired.'
+                )
                 raise exceptions.TokenSignatureExpired()
 
             # TODO: Validate other JWT claims
 
             # Else returns decoded message
             return message
 
         except NoSuitableSigningKeys as err:
+            log.warning(
+                'An error was encountered while verifying the OAuth 2.0 Client-Credentials Grant JWT. '
+                'There is no suitable signing key.'
+            )
             raise exceptions.NoSuitableKeys() from err
         except (BadSyntax, WrongNumberOfParts) as err:
+            log.warning(
+                'An error was encountered while verifying the OAuth 2.0 Client-Credentials Grant JWT. '
+                'The JWT is malformed.'
+            )
             raise exceptions.MalformedJwtToken() from err
         except BadSignature as err:
+            log.warning(
+                'An error was encountered while verifying the OAuth 2.0 Client-Credentials Grant JWT. '
+                'The JWT signature is incorrect.'
+            )
             raise exceptions.BadJwtSignature() from err
 
 
 class PlatformKeyHandler:
     """
     Platform RSA Key handler.
 
@@ -143,27 +170,36 @@
 
         if key_pem:
             # Import JWK from RSA key
             try:
                 self.key = RSAKey(
                     # Using the same key ID as client id
                     # This way we can easily serve multiple public
-                    # keys on teh same endpoint and keep all
+                    # keys on the same endpoint and keep all
                     # LTI 1.3 blocks working
                     kid=kid,
                     key=RSA.import_key(key_pem)
                 )
             except ValueError as err:
+                log.warning(
+                    'An error was encountered while loading the LTI platform\'s key. '
+                    'The RSA key could not be loaded.'
+                )
                 raise exceptions.InvalidRsaKey() from err
 
     def encode_and_sign(self, message, expiration=None):
         """
         Encode and sign JSON with RSA key
         """
+
         if not self.key:
+            log.warning(
+                'An error was encountered while loading the LTI platform\'s key. '
+                'The RSA key is not set.'
+            )
             raise exceptions.RsaKeyNotSet()
 
         _message = copy.deepcopy(message)
 
         # Set iat and exp if expiration is set
         if expiration:
             _message.update({
@@ -171,16 +207,29 @@
                 "exp": int(round(time.time()) + expiration),
             })
 
         # The class instance that sets up the signing operation
         # An RS 256 key is required for LTI 1.3
         _jws = JWS(_message, alg="RS256", cty="JWT")
 
-        # Encode and sign LTI message
-        return _jws.sign_compact([self.key])
+        try:
+            # Encode and sign LTI message
+            return _jws.sign_compact([self.key])
+        except NoSuitableSigningKeys as err:
+            log.warning(
+                'An error was encountered while signing the OAuth 2.0 access token JWT. '
+                'There is no suitable signing key.'
+            )
+            raise exceptions.NoSuitableKeys() from err
+        except UnknownAlgorithm as err:
+            log.warning(
+                'An error was encountered while signing the OAuth 2.0 access token JWT. '
+                'There algorithm is unknown.'
+            )
+            raise exceptions.MalformedJwtToken() from err
 
     def get_public_jwk(self):
         """
         Export Public JWK
         """
         public_keys = jwk.KEYS()
 
@@ -199,27 +248,47 @@
         """
         try:
             # Verify message signature
             message = JWS().verify_compact(token, keys=[self.key])
 
             # If message is valid, check expiration from JWT
             if 'exp' in message and message['exp'] < time.time():
+                log.warning(
+                    'An error was encountered while verifying the OAuth 2.0 access token. '
+                    'The JWT has expired.'
+                )
                 raise exceptions.TokenSignatureExpired()
 
             # Validate issuer claim (if present)
+            log_message_base = 'An error was encountered while verifying the OAuth 2.0 access token. '
             if iss:
                 if 'iss' not in message or message['iss'] != iss:
-                    raise exceptions.InvalidClaimValue('The required iss claim is either missing or does '
-                                                       'not match the expected iss value.')
+                    error_message = 'The required iss claim is missing or does not match the expected iss value. '
+                    log_message = log_message_base + error_message
+
+                    log.warning(log_message)
+                    raise exceptions.InvalidClaimValue(error_message)
 
             # Validate audience claim (if present)
             if aud:
                 if 'aud' not in message or aud not in message['aud']:
-                    raise exceptions.InvalidClaimValue('The required aud claim is missing.')
+                    error_message = 'The required aud claim is missing.'
+                    log_message = log_message_base + error_message
+
+                    log.warning(log_message)
+                    raise exceptions.InvalidClaimValue(error_message)
 
             # Else return token contents
             return message
 
         except NoSuitableSigningKeys as err:
+            log.warning(
+                'An error was encountered while verifying the OAuth 2.0 access token. '
+                'There is no suitable signing key.'
+            )
             raise exceptions.NoSuitableKeys() from err
         except BadSyntax as err:
+            log.warning(
+                'An error was encountered while verifying the OAuth 2.0 access token. '
+                'The JWT is malformed.'
+            )
             raise exceptions.MalformedJwtToken() from err
```

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/nprs.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/nprs.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_ags.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_consumer.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_deep_linking.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_key_handlers.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_key_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from unittest.mock import patch
 
 import ddt
 from Cryptodome.PublicKey import RSA
 from django.test.testcases import TestCase
 from jwkest import BadSignature
 from jwkest.jwk import RSAKey, load_jwks
-from jwkest.jws import JWS
+from jwkest.jws import JWS, NoSuitableSigningKeys, UnknownAlgorithm
+
 
 from lti_consumer.lti_1p3 import exceptions
 from lti_consumer.lti_1p3.key_handlers import PlatformKeyHandler, ToolKeyHandler
 
 from .utils import create_jwt
 
 
@@ -79,14 +80,38 @@
             {
                 "test": "test",
                 "iat": 1000,
                 "exp": 2000
             }
         )
 
+    def test_encode_and_sign_no_suitable_keys(self):
+        """
+        Test if an exception is raised when there are no suitable keys when signing the JWT.
+        """
+        message = {
+            "test": "test"
+        }
+
+        with patch('lti_consumer.lti_1p3.key_handlers.JWS.sign_compact', side_effect=NoSuitableSigningKeys):
+            with self.assertRaises(exceptions.NoSuitableKeys):
+                self.key_handler.encode_and_sign(message)
+
+    def test_encode_and_sign_unknown_algorithm(self):
+        """
+        Test if an exception is raised when the signing algorithm is unknown when signing the JWT.
+        """
+        message = {
+            "test": "test"
+        }
+
+        with patch('lti_consumer.lti_1p3.key_handlers.JWS.sign_compact', side_effect=UnknownAlgorithm):
+            with self.assertRaises(exceptions.MalformedJwtToken):
+                self.key_handler.encode_and_sign(message)
+
     def test_invalid_rsa_key(self):
         """
         Check that class raises when trying to import invalid RSA Key.
         """
         with self.assertRaises(exceptions.InvalidRsaKey):
             PlatformKeyHandler(key_pem="invalid PEM input")
```

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_1p3/tests/test_nrps.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/lti_xblock.py` & `lti-consumer-xblock-9.0.3/lti_consumer/lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0001_initial.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0002_ltiagslineitem.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0002_ltiagslineitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0003_ltiagsscore.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0003_ltiagsscore.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0004_keyset_mgmt_to_model.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0004_keyset_mgmt_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0005_migrate_keyset_to_model.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0005_migrate_keyset_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0007_ltidlcontentitem.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0007_ltidlcontentitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0008_fix_uuid_backfill.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0008_fix_uuid_backfill.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0009_backfill-empty-string-config-id.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0009_backfill-empty-string-config-id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0013_auto_20210712_1352.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0013_auto_20210712_1352.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0014_adds_external_id.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0014_adds_external_id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0015_add_additional_1p3_fields.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0015_add_additional_1p3_fields.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py` & `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/models.py` & `lti-consumer-xblock-9.0.3/lti_consumer/models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/outcomes.py` & `lti-consumer-xblock-9.0.3/lti_consumer/outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/plugin/compat.py` & `lti-consumer-xblock-9.0.3/lti_consumer/plugin/compat.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/plugin/urls.py` & `lti-consumer-xblock-9.0.3/lti_consumer/plugin/urls.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/plugin/views.py` & `lti-consumer-xblock-9.0.3/lti_consumer/plugin/views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/signals/signals.py` & `lti-consumer-xblock-9.0.3/lti_consumer/signals/signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/static/css/student.css` & `lti-consumer-xblock-9.0.3/lti_consumer/static/css/student.css`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/static/js/xblock_lti_consumer.js` & `lti-consumer-xblock-9.0.3/lti_consumer/static/js/xblock_lti_consumer.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/static/js/xblock_studio_view.js` & `lti-consumer-xblock-9.0.3/lti_consumer/static/js/xblock_studio_view.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/static/sass/student.scss` & `lti-consumer-xblock-9.0.3/lti_consumer/static/sass/student.scss`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_dl_content.html` & `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_dl_content.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_image.html` & `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_image.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti-dl/render_link.html` & `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_link.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_1p3_launch.html` & `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_1p3_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_1p3_studio.html` & `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_1p3_studio.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/lti_launch.html` & `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/templates/html/student.html` & `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/student.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/templates/xml/outcome_service_response.xml` & `lti-consumer-xblock-9.0.3/lti_consumer/templates/xml/outcome_service_response.xml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/templatetags/get_dl_lti_launch_url.py` & `lti-consumer-xblock-9.0.3/lti_consumer/templatetags/get_dl_lti_launch_url.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/templatetags/lti_sanitize.py` & `lti-consumer-xblock-9.0.3/lti_consumer/templatetags/lti_sanitize.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/test_utils.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_proctoring.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_proctoring.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_ags.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_api.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_filters.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_lti_xblock.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_models.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_outcomes.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_signals.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/tests/unit/test_utils.py` & `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/ar/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/en/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/es_419/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/fr/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/he/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/he/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/hi/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/ru/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.3/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer/utils.py` & `lti-consumer-xblock-9.0.3/lti_consumer/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/PKG-INFO` & `lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.0.2
+Version: 9.0.3
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.0.2/lti_consumer_xblock.egg-info/SOURCES.txt` & `lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.2/setup.py` & `lti-consumer-xblock-9.0.3/setup.py`

 * *Files identical despite different names*

