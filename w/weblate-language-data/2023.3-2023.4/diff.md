# Comparing `tmp/weblate-language-data-2023.3.tar.gz` & `tmp/weblate-language-data-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblate-language-data-2023.3.tar", last modified: Tue Feb 28 20:57:02 2023, max compression
+gzip compressed data, was "weblate-language-data-2023.4.tar", last modified: Tue Apr 18 16:08:32 2023, max compression
```

## Comparing `weblate-language-data-2023.3.tar` & `weblate-language-data-2023.4.tar`

### file list

```diff
@@ -1,368 +1,368 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1377 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.095659 weblate-language-data-2023.3/weblate_language_data/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/ambiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)   197324 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/check_languages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/country_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/language_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)   185603 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/languages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.079659 weblate-language-data-2023.3/weblate_language_data/locale/ab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/ab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133460 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/ab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.079659 weblate-language-data-2023.3/weblate_language_data/locale/afh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/afh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133461 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/afh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.079659 weblate-language-data-2023.3/weblate_language_data/locale/ang/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/ang/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133461 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/ang/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.079659 weblate-language-data-2023.3/weblate_language_data/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   153192 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/ar_LY/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/ar_LY/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   135634 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/ars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/ars/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133461 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/ars/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/ast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/ast/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142264 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/ast/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/az/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/az/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146118 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/az/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/be/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/be/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   152814 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/be/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/be@latin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/be@latin/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146318 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/be@latin/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/ber/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/ber/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   136567 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/ber/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   150210 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/bn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data/locale/bn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148116 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/bn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/bn_BD/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/bn_BD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148142 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/bo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/bo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   134135 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/bo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/br/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/br/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146509 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/br/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143081 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/ce/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/ce/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141984 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/ce/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/ckb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/ckb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   149055 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/ckb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/crh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/crh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   140636 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/crh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147662 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/cv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/cv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   139002 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/cv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/cy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/cy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142255 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/cy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143852 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144399 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)   133485 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/django.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/dv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/dv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133460 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/dv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   151306 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/en_GB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.103659 weblate-language-data-2023.3/weblate_language_data/locale/en_GB/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141759 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/enm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/enm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133461 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/enm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   145433 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/eo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143341 2023-02-28 20:56:50.000000 weblate-language-data-2023.3/weblate_language_data/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143017 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146829 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/eu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148108 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   152344 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/fil/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/fil/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141933 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/fil/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142800 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/fur/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/fur/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   139072 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/fur/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/fy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/fy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146566 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/fy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.083659 weblate-language-data-2023.3/weblate_language_data/locale/gl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   145891 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147698 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.107659 weblate-language-data-2023.3/weblate_language_data/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146910 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/hi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/hr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143711 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143900 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/hy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/hy/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   145966 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/hy/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/ia/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/ia/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   138933 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ia/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142320 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/ie/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/ie/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133751 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ie/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/is/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/is/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142871 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143172 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   156972 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142099 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ka/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/kab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/kab/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144797 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/kab/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/kk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/kk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146333 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/kk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/km/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/km/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   149286 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/km/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/kmr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/kmr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   145417 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/kmr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.111659 weblate-language-data-2023.3/weblate_language_data/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146757 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/ksh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/ksh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147179 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ksh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/ln/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/ln/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   138486 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ln/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143045 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141248 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/lv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/lzh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/lzh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   134586 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/lzh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/mk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/mk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147110 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/mk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/ml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/ml/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147723 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ml/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/mr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   155875 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/mr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/ms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/ms/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   138627 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ms/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/my/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/my/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   151158 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/my/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144000 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143009 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/nn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/nn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   137835 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/nn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/oc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/oc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   136768 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/oc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/or/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.115659 weblate-language-data-2023.3/weblate_language_data/locale/or/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148872 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/or/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/pa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/pa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   152371 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/pa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/pa_PK/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/pa_PK/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   136729 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.087659 weblate-language-data-2023.3/weblate_language_data/locale/peo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/peo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133461 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/peo/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144029 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/ps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/ps/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141021 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ps/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   142728 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143095 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141864 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143227 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/ro_MD/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/ro_MD/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133463 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   152444 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/sc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/sc/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143096 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/sc/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/si/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/si/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141219 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/si/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148523 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/skr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.119659 weblate-language-data-2023.3/weblate_language_data/locale/skr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141523 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/skr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/sl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/sl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147631 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   145670 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   150950 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/sr_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/sr_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143493 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143029 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   141412 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/ta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   151491 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ta/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/te/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/te/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   143375 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/te/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   154414 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/th/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/tlh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/tlh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133630 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/tlh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/tok/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/tok/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   133470 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/tok/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   144297 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/tt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/tt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   138610 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/tt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/tzm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/tzm/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   137250 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/tzm/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/ug/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.123659 weblate-language-data-2023.3/weblate_language_data/locale/ug/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   151700 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/ug/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/weblate_language_data/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   151899 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/uz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/weblate_language_data/locale/uz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   136275 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/uz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/weblate_language_data/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   148186 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/yue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/weblate_language_data/locale/yue/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   138799 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/yue/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/zgh/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/weblate_language_data/locale/zgh/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   156636 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/zgh/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/weblate_language_data/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   147755 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.091659 weblate-language-data-2023.3/weblate_language_data/locale/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/weblate_language_data/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   146619 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.127659 weblate-language-data-2023.3/weblate_language_data/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/plural_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/plurals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/rtl.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-28 20:56:51.000000 weblate-language-data-2023.3/weblate_language_data/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 20:57:02.099659 weblate-language-data-2023.3/weblate_language_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-02-28 20:57:02.000000 weblate-language-data-2023.3/weblate_language_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-02-28 20:57:02.000000 weblate-language-data-2023.3/weblate_language_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 20:57:02.000000 weblate-language-data-2023.3/weblate_language_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-28 20:57:02.000000 weblate-language-data-2023.3/weblate_language_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-28 20:57:02.000000 weblate-language-data-2023.3/weblate_language_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1377 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/ambiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)   197247 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/check_languages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/country_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/language_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)   186242 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/languages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.454500 weblate-language-data-2023.4/weblate_language_data/locale/ab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/ab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   133937 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.454500 weblate-language-data-2023.4/weblate_language_data/locale/afh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/afh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   133938 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/afh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.454500 weblate-language-data-2023.4/weblate_language_data/locale/ang/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/ang/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   133938 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ang/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.454500 weblate-language-data-2023.4/weblate_language_data/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   153837 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.454500 weblate-language-data-2023.4/weblate_language_data/locale/ar_LY/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data/locale/ar_LY/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   136111 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/ars/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   133938 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ars/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ast/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/ast/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142847 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ast/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/az/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/az/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146730 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/az/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/be/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/be/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   153466 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/be/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/be_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/be_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146896 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ber/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/ber/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   137044 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ber/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   150856 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/bn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/bn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148635 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/bn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/bn_BD/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/bn_BD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148729 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/bo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.486500 weblate-language-data-2023.4/weblate_language_data/locale/bo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134736 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/bo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/br/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/br/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147038 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/br/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143695 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ce/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/ce/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142553 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ce/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/ckb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/ckb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   149665 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ckb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/crh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/crh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   141181 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/crh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148277 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/cv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/cv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139601 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/cv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/cy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/cy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143032 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/cy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144470 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/da/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.458500 weblate-language-data-2023.4/weblate_language_data/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   145026 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)   133962 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/django.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/dv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.490500 weblate-language-data-2023.4/weblate_language_data/locale/dv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   133937 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/dv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   151966 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/en_GB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/en_GB/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142398 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/enm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/enm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   133938 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/enm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146033 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/eo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143955 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142980 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/et/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147445 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/eu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148717 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   152964 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fil/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/fil/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142539 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fil/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.494500 weblate-language-data-2023.4/weblate_language_data/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143416 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/fur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139637 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fur/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/fy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/fy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147096 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/fy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/gl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146504 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/gl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148312 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/he/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147429 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/hi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/hr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143727 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/hr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144519 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/hu/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.462500 weblate-language-data-2023.4/weblate_language_data/locale/hy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/hy/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146547 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/hy/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ia/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/ia/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139500 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ia/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.498500 weblate-language-data-2023.4/weblate_language_data/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142924 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/id/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ie/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/ie/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134228 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ie/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/is/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/is/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143494 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143783 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   157789 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142746 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ka/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/kab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/kab/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   145402 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/kab/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/kk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/kk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146931 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/kk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/km/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/km/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   149887 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/km/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/kmr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/kmr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   145991 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/kmr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147356 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ksh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.502500 weblate-language-data-2023.4/weblate_language_data/locale/ksh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147717 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ksh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ln/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/ln/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139053 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ln/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143582 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   141763 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/lzh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/lzh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   135157 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/lzh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/mk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/mk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147661 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/mk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/ml/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148358 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ml/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/mr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   156534 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/mr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/ms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/ms/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139136 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ms/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.466500 weblate-language-data-2023.4/weblate_language_data/locale/my/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/my/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   151792 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/my/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144618 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.506500 weblate-language-data-2023.4/weblate_language_data/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143628 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/nn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/nn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   138352 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/nn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/oc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/oc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   137315 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/oc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/or/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/or/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   149501 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/or/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   152996 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pa_PK/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pa_PK/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   137206 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/peo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/peo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   133938 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/peo/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144637 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/ps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/ps/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   141532 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ps/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143333 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143711 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   142502 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.510501 weblate-language-data-2023.4/weblate_language_data/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143845 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ro/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/ro_MD/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/ro_MD/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   133948 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   153109 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/sc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sc/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143710 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sc/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/si/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/si/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   141848 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/si/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.470500 weblate-language-data-2023.4/weblate_language_data/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   149137 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/skr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/skr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144779 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/skr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148262 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   146248 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   151618 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sr_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sr_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144111 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.514500 weblate-language-data-2023.4/weblate_language_data/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   143641 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   141993 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/ta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   152126 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ta/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/te/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/te/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144016 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/te/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   155061 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/th/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/tlh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/tlh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   134107 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/tlh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/tok/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/tok/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   133947 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/tok/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   144919 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/tt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/tt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139125 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/tt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/tzm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.518500 weblate-language-data-2023.4/weblate_language_data/locale/tzm/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   137837 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/tzm/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/ug/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/ug/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   152368 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/ug/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   152543 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/uz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/uz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   136858 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/uz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148715 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/yue_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/yue_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   139328 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/zgh/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.522500 weblate-language-data-2023.4/weblate_language_data/locale/zgh/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   157283 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/zgh/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   148360 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.474500 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   147233 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.526501 weblate-language-data-2023.4/weblate_language_data/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/plural_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/plurals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12601 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/rtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 16:08:17.000000 weblate-language-data-2023.4/weblate_language_data/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:08:32.482500 weblate-language-data-2023.4/weblate_language_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-18 16:08:32.000000 weblate-language-data-2023.4/weblate_language_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-04-18 16:08:32.000000 weblate-language-data-2023.4/weblate_language_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:08:32.000000 weblate-language-data-2023.4/weblate_language_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 16:08:32.000000 weblate-language-data-2023.4/weblate_language_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 16:08:32.000000 weblate-language-data-2023.4/weblate_language_data.egg-info/top_level.txt
```

### Comparing `weblate-language-data-2023.3/LICENSE` & `weblate-language-data-2023.4/LICENSE`

 * *Files identical despite different names*

### Comparing `weblate-language-data-2023.3/PKG-INFO` & `weblate-language-data-2023.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weblate-language-data
-Version: 2023.3
+Version: 2023.4
 Summary: Language definitions for Weblate
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/language-data
 Author: Michal Čihař
 Author-email: michal@weblate.org
 License: MIT
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/language-data/issues
@@ -35,15 +35,15 @@
 License-File: LICENSE
 
 .. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
    :alt: Weblate
    :target: https://weblate.org/
    :height: 80px
 
-**Weblate is a copylefted libre software web-based continuous localization system,
+**Weblate is libre software web-based continuous localization system,
 used by over 2500 libre projects and companies in more than 165 countries.**
 
 Language definitions used by `Weblate`_ and free to use by others.
 
 .. image:: https://img.shields.io/badge/website-weblate.org-blue.svg
     :alt: Website
     :target: https://weblate.org/
```

### Comparing `weblate-language-data-2023.3/README.rst` & `weblate-language-data-2023.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
    :alt: Weblate
    :target: https://weblate.org/
    :height: 80px
 
-**Weblate is a copylefted libre software web-based continuous localization system,
+**Weblate is libre software web-based continuous localization system,
 used by over 2500 libre projects and companies in more than 165 countries.**
 
 Language definitions used by `Weblate`_ and free to use by others.
 
 .. image:: https://img.shields.io/badge/website-weblate.org-blue.svg
     :alt: Website
     :target: https://weblate.org/
```

### Comparing `weblate-language-data-2023.3/setup.cfg` & `weblate-language-data-2023.4/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weblate-language-data
-version = 2023.3
+version = 2023.4
 description = Language definitions for Weblate
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://weblate.org/
 author = Michal Čihař
 author_email = michal@weblate.org
 license = MIT
@@ -56,20 +56,11 @@
 	weblate_language_data/plurals.py:E501
 
 [pycodestyle]
 extend-select = E,W1,W2,W3,W504,W505,W6
 exclude = .git,docs,.venv,build,.eggs
 max-line-length = 88
 
-[isort]
-multi_line_output = 3
-include_trailing_comma = True
-force_grid_wrap = 0
-use_parentheses = True
-line_length = 88
-known_first_party = weblate_language_data
-known_third_party = xdg,responses,requests,dateutil,requests_toolbelt,argcomplete
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `weblate-language-data-2023.3/setup.py` & `weblate-language-data-2023.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,13 +39,13 @@
                 convertmo(pofile, mofile, None)
 
 
 class WeblateBuild(build):
     """Override the default build with new subcommands."""
 
     # The build_mo has to be before build_data
-    sub_commands = [("build_mo", lambda self: True)] + build.sub_commands
+    sub_commands = [("build_mo", lambda self: True), *build.sub_commands]
 
 
 setup(
     cmdclass={"build_mo": BuildMo, "build": WeblateBuild},
 )
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/aliases.py` & `weblate-language-data-2023.4/weblate_language_data/aliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © Michal Čihař <michal@weblate.org>
 #
 # SPDX-License-Identifier: MIT
 
-"""Language data definitions.
+"""
+Language data definitions.
 
 This is an automatically generated file, see scripts/generate-language-data
 
 Do not edit, please adjust language definitions in following repository:
 https://github.com/WeblateOrg/language-data
 """
 # pylint: disable=line-too-long,too-many-lines
@@ -37,14 +38,15 @@
     "nb_nb": "nb_NO",
     "no_no": "nb_NO",
     "es_eu": "eu",
     "ru_r": "ru",
     "ru_rr": "ru",
     "ar_ar": "ar",
     "jp": "ja",
+    "jp_jpn": "ja",
     "ba_ck": "ba",
     "ca_ps": "ca",
     "by": "be",
     "ua": "uk",
     "ua_ua": "uk",
     "uk_uk": "uk",
     "en_en": "en",
@@ -55,14 +57,16 @@
     "ko_ko": "ko",
     "cs_cs": "cs",
     "la_la": "la",
     "da_da": "da",
     "et_et": "et",
     "fil_fil": "fil",
     "he_he": "he",
+    "ca_ca": "ca",
+    "ht_ht": "ht",
     "in": "id",
     "iw": "he",
     "iw_il": "he",
     "iw_he": "he",
     "in_id": "id",
     "ji": "yi",
     "jw": "jv",
@@ -84,18 +88,21 @@
     "sr@latin": "sr_Latn",
     "sr_rs@latin": "sr_Latn",
     "sr@cyrillic": "sr_Cyrl",
     "sr_rs@cyrillic": "sr_Cyrl",
     "uz@latin": "uz_Latn",
     "uz@latn": "uz_Latn",
     "uz@cyrillic": "uz",
+    "yue": "yue_Hant",
+    "nan": "nan_Hant",
     "zh": "zh_Hans",
     "zhcn": "zh_Hans",
     "zh_cn": "zh_Hans",
     "zh_chs": "zh_Hans",
+    "zh_cht": "zh_Hant",
     "zh_sg": "zh_Hans_SG",
     "zhtw": "zh_Hant",
     "zh_tw": "zh_Hant",
     "zh_hant_tw": "zh_Hant",
     "zh_hant@zh": "zh_Hant",
     "cmn": "zh_Hans",
     "zh_hk": "zh_Hant_HK",
@@ -140,14 +147,28 @@
     "eg": "ar_EG",
     "ca_es@valencia": "ca@valencia",
     "ca_xv": "ca@valencia",
     "ca_valencia": "ca@valencia",
     "va": "ca@valencia",
     "ang@latin": "ang",
     "cz": "cs",
+    "eng_gb": "en_GB",
+    "fin_fi": "fi",
+    "fra_fr": "fr",
+    "glg_es": "gl",
+    "deu_de": "de",
+    "ita_it": "it",
+    "jpn_jp": "ja",
+    "kab_kab": "kab",
+    "kor_kr": "ko",
+    "fas_ir": "fa",
+    "por_br": "pt_BR",
+    "por_pt": "pt",
+    "swe_se": "sv",
+    "ur_ur": "ur",
     "svk": "sk",
     "ptb": "pt_BR",
     "enu": "en_US",
     "bgr": "bg",
     "ptg": "pt",
     "esp": "es",
     "cht": "zh_Hant",
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/check_languages.py` & `weblate-language-data-2023.4/weblate_language_data/check_languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © Michal Čihař <michal@weblate.org>
 #
 # SPDX-License-Identifier: MIT
 
-"""Language data definitions.
+"""
+Language data definitions.
 
 This is an automatically generated file, see scripts/generate-language-data
 
 Do not edit, please adjust language definitions in following repository:
 https://github.com/WeblateOrg/language-data
 """
 # pylint: disable=line-too-long,too-many-lines
@@ -29,14 +30,15 @@
     "abanyom",
     "abar",
     "abau",
     "abawa",
     "abaza",
     "abaúj",
     "abbès",
+    "abeena",
     "abellen",
     "aberdeen",
     "aberdeenshire",
     "abertawe",
     "abia",
     "abidjan",
     "abidji",
@@ -89,14 +91,15 @@
     "acquaviva",
     "acre",
     "acroá",
     "adai",
     "adamaoua",
     "adamawa",
     "adamorobe",
+    "adan",
     "adana",
     "adang",
     "adangbe",
     "adangme",
     "adara",
     "adasen",
     "adb",
@@ -217,14 +220,16 @@
     "aizkraukles",
     "aizputes",
     "aja",
     "ajaria",
     "ajawa",
     "ajdovščina",
     "ajië",
+    "ajlūn",
+    "ajmān",
     "ajumbu",
     "ajyíninka",
     "aka",
     "akan",
     "akar",
     "akaselem",
     "akawaio",
@@ -396,14 +401,15 @@
     "amol",
     "amolatar",
     "amoltepec",
     "ampanang",
     "ampara",
     "ampari",
     "amri",
+    "amrān",
     "amto",
     "amudat",
     "amundava",
     "amurdak",
     "amuria",
     "amurskaja",
     "amuru",
@@ -457,14 +463,15 @@
     "aneityum",
     "anem",
     "aneme",
     "anenii",
     "anetan",
     "anfillo",
     "ang",
+    "anga",
     "angaataha",
     "angad",
     "angaité",
     "angal",
     "angami",
     "angaur",
     "angguruk",
@@ -569,14 +576,15 @@
     "apure",
     "apurimaq",
     "apurinã",
     "apurucayali",
     "apurímac",
     "aput",
     "aputai",
+    "aqabah",
     "aquila",
     "aquitaine",
     "aquitanian",
     "arab",
     "araba",
     "arabana",
     "arabela",
@@ -875,24 +883,26 @@
     "azha",
     "azhe",
     "azilal",
     "azoyú",
     "aztecan",
     "azua",
     "azuay",
+    "azur",
     "az̧",
     "açores",
     "aïn",
     "ağcabədi",
     "ağdam",
     "ağdaş",
     "ağrı",
     "ağstafa",
     "ağsu",
     "aşgabat",
+    "a̅şimah",
     "aḩmad",
     "aḩmadī",
     "aḩmar",
     "baalbek",
     "baan",
     "baangi",
     "baat",
@@ -1020,15 +1030,15 @@
     "balkarskaja",
     "balkh",
     "balo",
     "balochi",
     "balochistan",
     "baloi",
     "balong",
-    "balqā’",
+    "balqā",
     "baltazar",
     "balti",
     "baltic",
     "baltinavas",
     "baltistan",
     "baluan",
     "baluchi",
@@ -1230,20 +1240,20 @@
     "bayern",
     "baygo",
     "bayobiri",
     "bayono",
     "bayot",
     "bayrūt",
     "bayungu",
-    "bayḑā’",
+    "bayḑā",
     "bazar",
     "bazigar",
     "bazèga",
     "başrah",
-    "baţḩā’",
+    "baţḩā",
     "baḥri",
     "baḩr",
     "bce",
     "bceao",
     "bea",
     "beac",
     "beami",
@@ -1461,15 +1471,15 @@
     "binukidnon",
     "binumarien",
     "biobío",
     "bioko",
     "biombo",
     "bipi",
     "bipim",
-    "biqā‘",
+    "biqā",
     "bira",
     "birale",
     "birao",
     "birgit",
     "birgu",
     "birhor",
     "biri",
@@ -2158,15 +2168,15 @@
     "cebaara",
     "cebu",
     "cebuano",
     "cedi",
     "celje",
     "celtiberian",
     "celtic",
-    "cemet’",
+    "cemet",
     "cemuhî",
     "cen",
     "cent",
     "centar",
     "central",
     "centrale",
     "centre",
@@ -2917,14 +2927,15 @@
     "dingli",
     "dinguiraye",
     "dinka",
     "dionisio",
     "dios",
     "dioula",
     "diourbel",
+    "diq",
     "dirasha",
     "dire",
     "dirham",
     "diri",
     "diriku",
     "dirim",
     "disa",
@@ -3149,15 +3160,14 @@
     "düzce",
     "dādra",
     "dākhilīyah",
     "dāykundī",
     "děčín",
     "dīn",
     "dương",
-    "d’azur",
     "ealing",
     "ebira",
     "eblan",
     "ebo",
     "ebon",
     "ebonyi",
     "ebrié",
@@ -3258,14 +3268,15 @@
     "enfield",
     "enga",
     "engdewu",
     "engenni",
     "enggano",
     "england",
     "english",
+    "english‑based",
     "engordany",
     "engures",
     "eni",
     "enlhet",
     "enna",
     "ennedi",
     "enrekang",
@@ -3369,14 +3380,15 @@
     "extremadura",
     "extremaduran",
     "exuma",
     "eyak",
     "eyja",
     "eyjafjarðarsveit",
     "eystra",
+    "eyyĭḥ",
     "ezaa",
     "eşfahān",
     "faadhippolhu",
     "faen",
     "faetano",
     "fagani",
     "fahs",
@@ -3398,15 +3410,15 @@
     "fanbak",
     "fang",
     "fania",
     "fanti",
     "far",
     "faranah",
     "farefare",
-    "farg‘ona",
+    "farg",
     "faridpur",
     "faro",
     "faroe",
     "faroese",
     "fars",
     "farwānīyah",
     "farāh",
@@ -3526,14 +3538,15 @@
     "françaises",
     "fraser",
     "free",
     "freeport",
     "freetown",
     "freiburg",
     "french",
+    "french‑based",
     "fria",
     "frisian",
     "friuli",
     "friulian",
     "frosinone",
     "fryslân",
     "frýdek",
@@ -4725,14 +4738,15 @@
     "isparta",
     "israel",
     "israeli",
     "issas",
     "issyk",
     "istarska",
     "isthmus",
+    "iston",
     "istriot",
     "istro",
     "isu",
     "isukha",
     "isère",
     "italian",
     "italic",
@@ -4797,15 +4811,15 @@
     "jadgali",
     "jadida",
     "jadīd",
     "jaffna",
     "jafārah",
     "jah",
     "jahanka",
-    "jahrā’",
+    "jahrā",
     "jaintia",
     "jair",
     "jaitmatang",
     "jakarta",
     "jakati",
     "jakattoe",
     "jakun",
@@ -5301,15 +5315,15 @@
     "karang",
     "karanga",
     "karankawa",
     "karao",
     "karas",
     "karata",
     "karawa",
-    "karbalā’",
+    "karbalā",
     "karbi",
     "karbinci",
     "kardzhali",
     "kare",
     "karekare",
     "karelian",
     "karelija",
@@ -6233,16 +6247,14 @@
     "kırıkkale",
     "kırşehir",
     "kŭhistoni",
     "kǝngǝrli",
     "kəlbəcər",
     "kɛlɛngaxo",
     "kạn",
-    "k’abeena",
-    "k’eyyĭḥ",
     "laal",
     "laali",
     "laari",
     "laba",
     "label",
     "labem",
     "labir",
@@ -7390,16 +7402,14 @@
     "mazurskie",
     "mačvanski",
     "małopolskie",
     "maţrūḩ",
     "mažeikiai",
     "maḩwīt",
     "maḩāl",
-    "ma‘ān",
-    "ma’rib",
     "mba",
     "mbaaru",
     "mbala",
     "mbalanhu",
     "mbale",
     "mbandja",
     "mbangala",
@@ -8064,15 +8074,14 @@
     "mālpils",
     "mārupes",
     "māzandarān",
     "mērsraga",
     "mělník",
     "město",
     "mġarr",
-    "m’diq",
     "naaba",
     "naama",
     "naami",
     "naasioi",
     "naba",
     "nabak",
     "nabataean",
@@ -8790,15 +8799,14 @@
     "nīcas",
     "nīmrōz",
     "nīnawá",
     "nūristān",
     "nǁng",
     "nẵng",
     "nội",
-    "n’ko",
     "oaxaca",
     "obanliku",
     "oberösterreich",
     "obispeño",
     "oblast",
     "obleševo",
     "oblo",
@@ -9271,15 +9279,14 @@
     "pawnee",
     "paynamar",
     "pays",
     "paysandú",
     "paz",
     "pazardzhik",
     "pazeh",
-    "pa’anga",
     "pear",
     "pearling",
     "pech",
     "pecheneg",
     "pedernales",
     "pedi",
     "pedro",
@@ -9773,15 +9780,15 @@
     "qila",
     "qimant",
     "qinghai",
     "qinā",
     "qiubei",
     "qobustan",
     "qom",
-    "qoraqalpog‘iston",
+    "qoraqalpog",
     "qormi",
     "qrendi",
     "quang",
     "quapaw",
     "quba",
     "qubadlı",
     "quds",
@@ -9916,15 +9923,14 @@
     "rayón",
     "razajerdi",
     "razgrad",
     "razkrižje",
     "rače",
     "raški",
     "raẕavī",
-    "ra’s",
     "reab",
     "reading",
     "real",
     "red",
     "redange",
     "redbridge",
     "redcar",
@@ -9985,14 +9991,15 @@
     "rhodesia",
     "rhondda",
     "rhône",
     "rial",
     "riang",
     "riantana",
     "riau",
+    "rib",
     "ribeira",
     "ribnica",
     "ribun",
     "rica",
     "rican",
     "richmond",
     "rico",
@@ -10430,15 +10437,14 @@
     "saxon",
     "saxwe",
     "saya",
     "sayula",
     "sayyid",
     "saïda",
     "saône",
-    "sa‘īd",
     "schaan",
     "schaffhausen",
     "schellenberg",
     "schleswig",
     "schwyz",
     "scilly",
     "scotia",
@@ -10679,15 +10685,15 @@
     "shwai",
     "shwe",
     "shyghys",
     "shymkent",
     "shéfa",
     "shāriqah",
     "shārqī",
-    "shāţi’",
+    "shāţi",
     "shīḩānīyah",
     "sialum",
     "siamou",
     "sian",
     "siane",
     "siang",
     "siar",
@@ -11163,14 +11169,15 @@
     "syenara",
     "sylhet",
     "sylheti",
     "syllabaries",
     "syllabics",
     "syloti",
     "symbols",
+    "syria",
     "syriac",
     "syrian",
     "syunik",
     "szabolcs",
     "szatmár",
     "szeged",
     "szekszárd",
@@ -13208,15 +13215,15 @@
     "zaqatala",
     "zaragoza",
     "zaramo",
     "zarasai",
     "zari",
     "zarma",
     "zarphatic",
-    "zarqā’",
+    "zarqā",
     "zauzou",
     "zavrč",
     "zawgyi",
     "zawr",
     "zay",
     "zayein",
     "zayse",
@@ -13302,16 +13309,16 @@
     "záparo",
     "zóchi",
     "zürich",
     "zābul",
     "zāwiyah",
     "zəngilan",
     "zərdab",
+    "z̧a",
     "z̧aby",
-    "z̧a‘āyin",
     "z̧ufār",
     "z̧āhirah",
     "²ggŏ",
     "¹baw",
     "àhàn",
     "ágion",
     "água",
@@ -13343,15 +13350,17 @@
     "örebro",
     "östergötlands",
     "övörhangay",
     "ústecký",
     "ústí",
     "þingeyjarsveit",
     "ādažu",
+    "āyin",
     "āz̄ārbāyjān",
+    "āşimah",
     "čair",
     "čaška",
     "česká",
     "české",
     "český",
     "češinovo",
     "črenšovci",
@@ -13374,15 +13383,15 @@
     "śāradā",
     "şabran",
     "şahbuz",
     "şalāl",
     "şalāḩ",
     "şamaxı",
     "şanlıurfa",
-    "şanʻā’",
+    "şanʻā",
     "şirvan",
     "şuşa",
     "şāʻdah",
     "şırnak",
     "şəki",
     "şəmkir",
     "şərur",
@@ -13442,28 +13451,21 @@
     "ǁgana",
     "ǁxegwi",
     "ǂhua",
     "ǂungkue",
     "ǃxóõ",
     "șoldănești",
     "ștefan",
-    "ḑāli‘",
+    "ḑāli",
     "ḩajjah",
     "ḩalab",
     "ḩamāh",
     "ḩasakah",
     "ḩawallī",
     "ḩayāt",
     "ḩaḑramawt",
     "ḩimş",
     "ḩudaydah",
     "ḩudūd",
     "ṭākrī",
     "ṭāṅkrī",
-    "‘adan",
-    "‘ajlūn",
-    "‘ajmān",
-    "‘amrān",
-    "‘aqabah",
-    "‘a̅şimah",
-    "‘āşimah",
 }
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/countries.py` & `weblate-language-data-2023.4/weblate_language_data/countries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © Michal Čihař <michal@weblate.org>
 #
 # SPDX-License-Identifier: MIT
 
-"""Language data definitions.
+"""
+Language data definitions.
 
 This is an automatically generated file, see scripts/generate-language-data
 
 Do not edit, please adjust language definitions in following repository:
 https://github.com/WeblateOrg/language-data
 """
 # pylint: disable=line-too-long,too-many-lines
@@ -123,8 +124,9 @@
     "xh_za",
     "yi_us",
     "zu_za",
     "ast_es",
     "gug_py",
     "kab_dz",
     "sc_it",
+    "ug_cn",
 )
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/country_codes.py` & `weblate-language-data-2023.4/weblate_language_data/country_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © Michal Čihař <michal@weblate.org>
 #
 # SPDX-License-Identifier: MIT
 
-"""Language data definitions.
+"""
+Language data definitions.
 
 This is an automatically generated file, see scripts/generate-language-data
 
 Do not edit, please adjust language definitions in following repository:
 https://github.com/WeblateOrg/language-data
 """
 # pylint: disable=line-too-long,too-many-lines
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/language_codes.py` & `weblate-language-data-2023.4/weblate_language_data/language_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © Michal Čihař <michal@weblate.org>
 #
 # SPDX-License-Identifier: MIT
 
-"""Language data definitions.
+"""
+Language data definitions.
 
 This is an automatically generated file, see scripts/generate-language-data
 
 Do not edit, please adjust language definitions in following repository:
 https://github.com/WeblateOrg/language-data
 """
 # pylint: disable=line-too-long,too-many-lines
@@ -134,14 +135,15 @@
     "bur",
     "by",
     "by_lat",
     "byn",
     "ca",
     "ca@valencia",
     "ca_ad",
+    "ca_ca",
     "ca_es@valencia",
     "ca_ps",
     "ca_valencia",
     "ca_xv",
     "cad",
     "cak",
     "car",
@@ -214,14 +216,15 @@
     "de_fo",
     "de_form",
     "de_lu",
     "del",
     "den",
     "des",
     "deu",
+    "deu_de",
     "dgo",
     "dgr",
     "din",
     "div",
     "dk",
     "doi",
     "dry",
@@ -258,14 +261,15 @@
     "en_shaw_gb",
     "en_shaw_us",
     "en_us",
     "en_xa",
     "en_za",
     "ena",
     "eng",
+    "eng_gb",
     "english_uk",
     "enm",
     "enp",
     "enu",
     "eo",
     "epo",
     "es",
@@ -300,21 +304,23 @@
     "ewo",
     "ext",
     "fa",
     "fa_af",
     "fan",
     "fao",
     "fas",
+    "fas_ir",
     "fat",
     "ff",
     "fi",
     "fij",
     "fil",
     "fil_fil",
     "fin",
+    "fin_fi",
     "fj",
     "flemish",
     "fo",
     "fon",
     "fr",
     "fr@formal",
     "fr@informal",
@@ -325,14 +331,15 @@
     "fr_fo",
     "fr_form",
     "fr_fr_x_formal",
     "fr_fr_x_informal",
     "fr_lu",
     "fr_sn",
     "fra",
+    "fra_fr",
     "frb",
     "frc",
     "fre",
     "frm",
     "fro",
     "frp",
     "frr",
@@ -352,14 +359,15 @@
     "ger",
     "gez",
     "gil",
     "gl",
     "gla",
     "gle",
     "glg",
+    "glg_es",
     "glk",
     "glv",
     "gmh",
     "gn",
     "goh",
     "gon",
     "gor",
@@ -401,14 +409,15 @@
     "hne",
     "ho",
     "hr",
     "hrv",
     "hrx",
     "hsb",
     "ht",
+    "ht_ht",
     "hu",
     "hun",
     "hup",
     "hus",
     "hy",
     "hye",
     "hz",
@@ -436,14 +445,15 @@
     "is",
     "isl",
     "it",
     "it@formal",
     "it@informal",
     "it_ch",
     "ita",
+    "ita_it",
     "its",
     "iu",
     "iw",
     "iw_he",
     "iw_il",
     "ja",
     "ja_ja",
@@ -451,22 +461,25 @@
     "jam",
     "jav",
     "jbo",
     "jgo",
     "ji",
     "jmc",
     "jp",
+    "jp_jpn",
     "jpn",
+    "jpn_jp",
     "jpr",
     "jrb",
     "jv",
     "jw",
     "ka",
     "kaa",
     "kab",
+    "kab_kab",
     "kac",
     "kaj",
     "kal",
     "kam",
     "kan",
     "kas",
     "kat",
@@ -499,14 +512,15 @@
     "kn",
     "ko",
     "ko_ko",
     "kok",
     "kom",
     "kon",
     "kor",
+    "kor_kr",
     "kos",
     "kpe",
     "kr",
     "krc",
     "krl",
     "kru",
     "ks",
@@ -618,14 +632,16 @@
     "my",
     "my@zawgyi",
     "mya",
     "myv",
     "na",
     "nah",
     "nan",
+    "nan_hant",
+    "nan_latn",
     "nap",
     "naq",
     "nau",
     "nav",
     "nb",
     "nb_nb",
     "nb_no",
@@ -706,14 +722,16 @@
     "pli",
     "plk",
     "pms",
     "pnb",
     "pol",
     "pon",
     "por",
+    "por_br",
+    "por_pt",
     "portuguese_br",
     "portuguese_portugal",
     "pr",
     "prg",
     "pro",
     "ps",
     "pt",
@@ -859,14 +877,15 @@
     "sve",
     "svk",
     "sw",
     "sw_cd",
     "sw_tz",
     "swa",
     "swe",
+    "swe_se",
     "swg",
     "sxu",
     "syc",
     "syr",
     "szl",
     "ta",
     "ta_lk",
@@ -934,14 +953,15 @@
     "uk_uk",
     "ukr",
     "umb",
     "und",
     "ur",
     "ur_in",
     "ur_pk",
+    "ur_ur",
     "urd",
     "us",
     "uz",
     "uz@cyrillic",
     "uz@latin",
     "uz@latn",
     "uz_latn",
@@ -982,21 +1002,24 @@
     "yap",
     "yi",
     "yid",
     "yo",
     "yor",
     "yua",
     "yue",
+    "yue_hans",
+    "yue_hant",
     "za",
     "zap",
     "zbl",
     "zen",
     "zgh",
     "zh",
     "zh_chs",
+    "zh_cht",
     "zh_cmn_hans",
     "zh_cmn_hant",
     "zh_cn",
     "zh_hans",
     "zh_hans_cn",
     "zh_hans_sg",
     "zh_hant",
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/languages.py` & `weblate-language-data-2023.4/weblate_language_data/languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © Michal Čihař <michal@weblate.org>
 #
 # SPDX-License-Identifier: MIT
 
-"""Language data definitions.
+"""
+Language data definitions.
 
 This is an automatically generated file, see scripts/generate-language-data
 
 Do not edit, please adjust language definitions in following repository:
 https://github.com/WeblateOrg/language-data
 """
 # pylint: disable=line-too-long,too-many-lines
@@ -3631,19 +3632,28 @@
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
         _("Nahuatl"),
         2,
         "n != 1",
     ),
     (
-        "nan",
-        # Translators: Language name for ISO code "nan". The parenthesis clarifies
+        "nan_Hant",
+        # Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
+        # variant of the language. It could contain a region, age (Old, Middle, ...)
+        # or other variant.
+        _("Chinese (Min Nan, Traditional)"),
+        2,
+        "n != 1",
+    ),
+    (
+        "nan_Latn",
+        # Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
-        _("Chinese (Min Nan)"),
+        _("Chinese (Min Nan, Latin)"),
         2,
         "n != 1",
     ),
     (
         "nap",
         # Translators: Language name for ISO code "nap". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
@@ -5701,19 +5711,28 @@
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
         _("Yucateco"),
         2,
         "n != 1",
     ),
     (
-        "yue",
-        # Translators: Language name for ISO code "yue". The parenthesis clarifies
+        "yue_Hans",
+        # Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+        # variant of the language. It could contain a region, age (Old, Middle, ...)
+        # or other variant.
+        _("Yue (Simplified)"),
+        1,
+        "0",
+    ),
+    (
+        "yue_Hant",
+        # Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
         # or other variant.
-        _("Yue"),
+        _("Yue (Traditional)"),
         1,
         "0",
     ),
     (
         "za",
         # Translators: Language name for ISO code "za". The parenthesis clarifies
         # variant of the language. It could contain a region, age (Old, Middle, ...)
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ab/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/bo/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: ab\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2022-12-01 18:52+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Tibetan <https://hosted.weblate.org/projects/weblate/"
+"languages/bo/>\n"
+"Language: bo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 4.15-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr ""
 
@@ -424,15 +427,15 @@
 msgid "Bantu (Other)"
 msgstr ""
 
 #. Translators: Language name for ISO code "bo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tibetan"
-msgstr ""
+msgstr "བོད་སྐད་"
 
 #. Translators: Language name for ISO code "bo_CN". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tibetan (China)"
 msgstr ""
 
@@ -850,15 +853,15 @@
 msgid "Dyula"
 msgstr ""
 
 #. Translators: Language name for ISO code "dz". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dzongkha"
-msgstr ""
+msgstr "རྫོང་ཁ"
 
 #. Translators: Language name for ISO code "ee". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ewe"
 msgstr ""
 
@@ -898,15 +901,15 @@
 msgid "Elamite"
 msgstr ""
 
 #. Translators: Language name for ISO code "en". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "English"
-msgstr ""
+msgstr "དབྱིན་ཇིའི་སྐད།"
 
 #. Translators: Language name for ISO code "en@pirate". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "English (Pirate)"
 msgstr ""
 
@@ -1510,15 +1513,15 @@
 msgid "Hebrew (Israel)"
 msgstr ""
 
 #. Translators: Language name for ISO code "hi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hindi"
-msgstr ""
+msgstr "ཧིན་དི"
 
 #. Translators: Language name for ISO code "hi_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hindi (latin)"
 msgstr ""
 
@@ -1702,15 +1705,15 @@
 msgid "Inuktitut"
 msgstr ""
 
 #. Translators: Language name for ISO code "ja". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Japanese"
-msgstr ""
+msgstr "ཉི་ཧོང་སྐད་"
 
 #. Translators: Language name for ISO code "ja_KS". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Japanese (Kansai)"
 msgstr ""
 
@@ -2326,15 +2329,15 @@
 msgid "Mandinka"
 msgstr ""
 
 #. Translators: Language name for ISO code "mnw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mon"
-msgstr ""
+msgstr "ཟླ་བ།"
 
 #. Translators: Language name for ISO code "moe". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Innu"
 msgstr ""
 
@@ -2424,19 +2427,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "རྒྱ་སྐད་"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "རྒྱ་སྐད་"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
 
@@ -2464,15 +2477,15 @@
 msgid "German (Low)"
 msgstr ""
 
 #. Translators: Language name for ISO code "ne". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nepali"
-msgstr ""
+msgstr "ནེ་པ་ལི"
 
 #. Translators: Language name for ISO code "new". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Newari"
 msgstr ""
 
@@ -2920,21 +2933,23 @@
 msgid "Romany"
 msgstr ""
 
 #. Translators: Language name for ISO code "ru". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian"
-msgstr ""
+msgstr "ཨུ་རུ་སུ་སྐད་"
 
 #. Translators: Language name for ISO code "ru@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
+#, fuzzy
+#| msgid "Russian"
 msgid "Russian (formal)"
-msgstr ""
+msgstr "ཨུ་རུ་སུ་སྐད་"
 
 #. Translators: Language name for ISO code "ru@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian (informal)"
 msgstr ""
 
@@ -3741,22 +3756,26 @@
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
+#, fuzzy
+#| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
-msgstr ""
+msgstr "རྒྱ་སྐད་ (རྒྱ་ཡིག་གསར་པ།)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
+#, fuzzy
+#| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
-msgstr ""
+msgstr "རྒྱ་སྐད་ (རྒྱ་ཡིག་རྙིང་པ།)"
 
 #. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wolof"
 msgstr ""
 
@@ -3804,18 +3823,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
@@ -3886,8 +3911,8 @@
 msgid "Zuni"
 msgstr ""
 
 #. Translators: Language name for ISO code "zza". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zaza"
-msgstr ""
+msgstr "ཟ་ཟའ་སྐད།"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/afh/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/django.pot`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: afh\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
@@ -2424,18 +2425,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3804,18 +3811,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ang/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/tlh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the Weblate Language Data package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# This file is distributed under the same license as the PACKAGE package.
+# Christine Long <lilmamachrislong33@gmail.com>, 2022.
 msgid ""
 msgstr ""
-"Project-Id-Version: Weblate Language Data\n"
+"Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: ang\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2022-01-26 17:54+0000\n"
+"Last-Translator: Christine Long <lilmamachrislong33@gmail.com>\n"
+"Language-Team: Klingon <https://hosted.weblate.org/projects/weblate/"
+"languages/tlh/>\n"
+"Language: tlh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 4.11-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
-msgstr ""
+msgstr "'ay'"
 
 #. Translators: Language name for ISO code "ab". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Abkhazian"
-msgstr ""
+msgstr "'atlham"
 
 #. Translators: Language name for ISO code "ace". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Acehnese"
 msgstr ""
 
@@ -2326,15 +2328,15 @@
 msgid "Mandinka"
 msgstr ""
 
 #. Translators: Language name for ISO code "mnw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mon"
-msgstr ""
+msgstr "jach"
 
 #. Translators: Language name for ISO code "moe". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Innu"
 msgstr ""
 
@@ -2424,18 +2426,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3804,18 +3812,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ar/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ar/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # tamer dab <dabsantamer@yahoo.com>, 2020.
 # Hakim Oubouali <hakim.oubouali.skr@gmail.com>, 2020.
 # thami simo <simo.azad@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: thami simo <simo.azad@gmail.com>\n"
 "Language-Team: Arabic <https://hosted.weblate.org/projects/weblate/languages/"
 "ar/>\n"
 "Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2564,18 +2564,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "ناواتل"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "الصينية (التقليدية)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "الصينية (مين نان)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "النابولية"
@@ -4036,19 +4046,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "صينية يؤ (المبسطة)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "صينية يؤ"
+msgid "Yue (Traditional)"
+msgstr "صينية يؤ (التقليدية)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "الزهيونج"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 # Ayoub Rejal <ayoubrejal@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2020-06-19 09:20+0000\n"
 "Last-Translator: Ayoub Rejal <ayoubrejal@gmail.com>\n"
 "Language-Team: Arabic (Libya) <https://hosted.weblate.org/projects/weblate/"
 "languages/ar_LY/>\n"
 "Language: ar_LY\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2451,18 +2451,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3839,18 +3845,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ars/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ab/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: ars\n"
+"Language: ab\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
@@ -2424,18 +2424,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3804,18 +3810,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ast/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ast/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Asturian <https://hosted.weblate.org/projects/weblate/"
 "languages/ast/>\n"
 "Language: ast\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2567,19 +2567,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Min Nan"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinese, Min Nan"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Min Nan"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Chinese, Min Nan"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "napolitanu"
 
@@ -4021,18 +4031,24 @@
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Yucateco"
 msgstr "Aguacateco"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/az/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/az/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Meki <mekismith77@gmail.com>, 2020.
 # Nizami <nizamismidov4@gmail.com>, 2022.
 # Ariz Mirzəzadə <by.ariz@bk.ru>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-11-07 18:05+0000\n"
 "Last-Translator: Ariz Mirzəzadə <by.ariz@bk.ru>\n"
 "Language-Team: Azerbaijani <https://hosted.weblate.org/projects/weblate/"
 "languages/az/>\n"
 "Language: az\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2568,18 +2568,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Çin (Ənənəvi)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Çin (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "neapolital dili"
@@ -4041,19 +4051,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (Sadələşdirilmiş)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (Ənənəvi)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "çjuan"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/be/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/be/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Zmicer Turok <zmicerturok@gmail.com>, 2019.
 # Zmicer Turok <nashtlumach@gmail.com>, 2019, 2020, 2021.
 # Alex Ky <esthomolupus@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Belarusian <https://hosted.weblate.org/projects/weblate/"
 "languages/be/>\n"
 "Language: be\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2544,18 +2544,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Нахуатль"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Кітайская (традыцыйная)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Кітайская (Мінь Нань)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Неапалітанская"
@@ -3998,19 +4008,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Юэ (спрошчаная)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Юэ"
+msgid "Yue (Traditional)"
+msgstr "Юэ (традыцыйная)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Чжуанская"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/be@latin/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 # Viktar Vauchkevich <victorenator@gmail.com>, 2018, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Belarusian (latin) <https://hosted.weblate.org/projects/"
 "weblate/languages/be_Latn/>\n"
 "Language: be@latin\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2594,20 +2594,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "nachuatĺ"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "kitajskaja (tradycyjnaja)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Mandarin)"
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "kitajskaja (mandaryn)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "nieapalіtanskaja"
@@ -4064,19 +4072,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Jue (sproščanaja)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Jue"
+msgid "Yue (Traditional)"
+msgstr "Jue (tradycyjnaja)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "čžuanskaja"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ber/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ber/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Hakim Oubouali <hakim.oubouali.skr@gmail.com>, 2020.
 # ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ زهير أمازيغ <zouhirdehbi56@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-01-22 20:54+0000\n"
 "Last-Translator: ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ زهير أمازيغ <zouhirdehbi56@gmail.com>\n"
 "Language-Team: Berber <https://hosted.weblate.org/projects/weblate/languages/"
 "ber/>\n"
 "Language: ber\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2435,18 +2435,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3817,18 +3823,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/bg/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/bg/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Georgi Georgiev <g.georgiev.shumen@gmail.com>, 2021.
 # 109247019824 <stoyan@gmx.com>, 2022.
 # Ясен Арсов <jarsov@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-01-31 01:49+0000\n"
 "Last-Translator: Любомир Василев <lyubomirv@gmx.com>\n"
 "Language-Team: Bulgarian <https://hosted.weblate.org/projects/weblate/"
 "languages/bg/>\n"
 "Language: bg\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2432,18 +2432,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Науатъл"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Китайски (традиционен)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Китайски (Мин Нан)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Неаполитански"
@@ -3812,19 +3822,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Юкатекски"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Юе (опростен)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Юе"
+msgid "Yue (Traditional)"
+msgstr "Юе (традиционен)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Джуански"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/bn/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/bn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 # Oymate <dhruboadittya96@gmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-06-14 05:12+0000\n"
 "Last-Translator: Oymate <dhruboadittya96@gmail.com>\n"
 "Language-Team: Bengali <https://hosted.weblate.org/projects/weblate/"
 "languages/bn/>\n"
 "Language: bn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2528,19 +2528,27 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "চিনা"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Chinese (Min Nan, Latin)"
+msgstr "চিনা"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "নেয়াপোলিটান"
 
@@ -3971,18 +3979,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "ঝু্য়াঙ"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Atikur Rahman <arahman.dcc2@gmail.com>, 2019.
 # Anonymous <noreply@weblate.org>, 2020.
 # Oymate <dhruboadittya96@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Bengali (Bangladesh) <https://hosted.weblate.org/projects/"
 "weblate/languages/bn_BD/>\n"
 "Language: bn_BD\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2567,18 +2567,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "নাহুয়াটি"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "চীনা (মিন নান)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "চীনা (মিন নান)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "নেয়াপোলিটান"
@@ -4005,18 +4015,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/bo/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/afh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2022-12-01 18:52+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Tibetan <https://hosted.weblate.org/projects/weblate/"
-"languages/bo/>\n"
-"Language: bo\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: Automatically generated\n"
+"Language-Team: none\n"
+"Language: afh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.15-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr ""
 
@@ -427,15 +424,15 @@
 msgid "Bantu (Other)"
 msgstr ""
 
 #. Translators: Language name for ISO code "bo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tibetan"
-msgstr "བོད་སྐད་"
+msgstr ""
 
 #. Translators: Language name for ISO code "bo_CN". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tibetan (China)"
 msgstr ""
 
@@ -853,15 +850,15 @@
 msgid "Dyula"
 msgstr ""
 
 #. Translators: Language name for ISO code "dz". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dzongkha"
-msgstr "རྫོང་ཁ"
+msgstr ""
 
 #. Translators: Language name for ISO code "ee". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ewe"
 msgstr ""
 
@@ -901,15 +898,15 @@
 msgid "Elamite"
 msgstr ""
 
 #. Translators: Language name for ISO code "en". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "English"
-msgstr "དབྱིན་ཇིའི་སྐད།"
+msgstr ""
 
 #. Translators: Language name for ISO code "en@pirate". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "English (Pirate)"
 msgstr ""
 
@@ -1513,15 +1510,15 @@
 msgid "Hebrew (Israel)"
 msgstr ""
 
 #. Translators: Language name for ISO code "hi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hindi"
-msgstr "ཧིན་དི"
+msgstr ""
 
 #. Translators: Language name for ISO code "hi_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Hindi (latin)"
 msgstr ""
 
@@ -1705,15 +1702,15 @@
 msgid "Inuktitut"
 msgstr ""
 
 #. Translators: Language name for ISO code "ja". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Japanese"
-msgstr "ཉི་ཧོང་སྐད་"
+msgstr ""
 
 #. Translators: Language name for ISO code "ja_KS". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Japanese (Kansai)"
 msgstr ""
 
@@ -2329,15 +2326,15 @@
 msgid "Mandinka"
 msgstr ""
 
 #. Translators: Language name for ISO code "mnw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mon"
-msgstr "ཟླ་བ།"
+msgstr ""
 
 #. Translators: Language name for ISO code "moe". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Innu"
 msgstr ""
 
@@ -2427,18 +2424,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -2467,15 +2470,15 @@
 msgid "German (Low)"
 msgstr ""
 
 #. Translators: Language name for ISO code "ne". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nepali"
-msgstr "ནེ་པ་ལི"
+msgstr ""
 
 #. Translators: Language name for ISO code "new". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Newari"
 msgstr ""
 
@@ -2923,23 +2926,21 @@
 msgid "Romany"
 msgstr ""
 
 #. Translators: Language name for ISO code "ru". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian"
-msgstr "ཨུ་རུ་སུ་སྐད་"
+msgstr ""
 
 #. Translators: Language name for ISO code "ru@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Russian"
 msgid "Russian (formal)"
-msgstr "ཨུ་རུ་སུ་སྐད་"
+msgstr ""
 
 #. Translators: Language name for ISO code "ru@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian (informal)"
 msgstr ""
 
@@ -3746,26 +3747,22 @@
 #. or other variant.
 msgid "Westphalien"
 msgstr ""
 
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
-msgstr "རྒྱ་སྐད་ (རྒྱ་ཡིག་གསར་པ།)"
+msgstr ""
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
-msgstr "རྒྱ་སྐད་ (རྒྱ་ཡིག་རྙིང་པ།)"
+msgstr ""
 
 #. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wolof"
 msgstr ""
 
@@ -3813,18 +3810,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
@@ -3895,8 +3898,8 @@
 msgid "Zuni"
 msgstr ""
 
 #. Translators: Language name for ISO code "zza". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zaza"
-msgstr "ཟ་ཟའ་སྐད།"
+msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/br/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/br/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2016-01-14 15:07+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Breton <https://hosted.weblate.org/projects/weblate/master/br/"
 ">\n"
 "Language: br\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2648,20 +2648,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Taiwan)"
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Sinaeg (Taiwan)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Taiwan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Sinaeg (Taiwan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitaneg"
@@ -4134,18 +4142,24 @@
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Yucateco"
 msgstr "Aguakateko"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ca/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ca/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Adolfo Jayme Barrientos <fitojb@ubuntu.com>, 2020.
 # Ecron <ecron_89@hotmail.com>, 2020.
 # Maite Guix <maite.guix@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-14 11:39+0000\n"
 "Last-Translator: Eduard Ereza Martínez <eduard@ereza.cat>\n"
 "Language-Team: Catalan <https://hosted.weblate.org/projects/weblate/"
 "languages/ca/>\n"
 "Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2430,18 +2430,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "nàhuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "xinès (tradicional)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "xinès (min nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "napolità"
@@ -3810,19 +3820,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "maia yucatec"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "cantonès (simplificat)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "cantonès"
+msgid "Yue (Traditional)"
+msgstr "cantonès (tradicional)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ce/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ce/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ce\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2505,19 +2505,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "цийн"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "цийн"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "неаполитанойн"
 
@@ -3935,18 +3945,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ckb/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ckb/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Jwtiyar Nariman <jwtiyar@gmail.com>, 2020.
 # Kurd As <kurd68587@gmail.com>, 2020, 2021.
 # Rener kaka <Rabarajax51@gmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Kurdish (Central) <https://hosted.weblate.org/projects/"
 "weblate/languages/ckb/>\n"
 "Language: ckb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2466,18 +2466,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "نەهواتڵ"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "چینی (کۆن)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "چینی (مین نان)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "ناپۆلی"
@@ -3880,19 +3890,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "یوو (ئاسانکراو)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "یوو"
+msgid "Yue (Traditional)"
+msgstr "یوو (کۆن)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "یونگ"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/crh/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/crh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: crh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2510,19 +2510,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Çince"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Çince"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapolitan"
 
@@ -3941,18 +3951,24 @@
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Yucateco"
 msgstr "Aguacateco"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/cs/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/cs/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Michal Čihař <michal@weblate.org>, 2020, 2021.
 # Jonáš Loskot <ltvlcihory@gmail.com>, 2020.
 # Milan <mobrcian@hotmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/weblate/languages/"
 "cs/>\n"
 "Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2518,18 +2518,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl (Aztéčtina)"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Čínština (tradiční)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Čínština (min-nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapolština"
@@ -3983,19 +3993,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Jüe (zjednodušená)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Jüe"
+msgid "Yue (Traditional)"
+msgstr "Jüe (tradiční)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Čuangština"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/cv/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/cv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # İlle <derasetad@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Chuvash <https://hosted.weblate.org/projects/weblate/"
 "languages/cv/>\n"
 "Language: cv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2498,19 +2498,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "ҫурҫӗр китай"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "ҫурҫӗр китай"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
 
@@ -3916,18 +3926,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/cy/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/cy/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
+# dreigiau <sterilgrimed23@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2021-11-14 00:02+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2023-03-09 22:56+0000\n"
+"Last-Translator: dreigiau <sterilgrimed23@gmail.com>\n"
 "Language-Team: Welsh <https://hosted.weblate.org/projects/weblate/languages/"
 "cy/>\n"
 "Language: cy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=(n==0) ? 0 : (n==1) ? 1 : (n==2) ? 2 : "
 "(n==3) ? 3 :(n==6) ? 4 : 5;\n"
-"X-Generator: Weblate 4.9.1-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Affareg"
 
@@ -31,21 +32,21 @@
 msgid "Abkhazian"
 msgstr "Abchaseg"
 
 #. Translators: Language name for ISO code "ace". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Acehnese"
-msgstr ""
+msgstr "Acehneseg"
 
 #. Translators: Language name for ISO code "ach". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Acholi"
-msgstr ""
+msgstr "Acholi"
 
 #. Translators: Language name for ISO code "ada". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Adangme"
 msgstr "Adangmëeg"
 
@@ -66,31 +67,29 @@
 #. or other variant.
 msgid "Afrikaans"
 msgstr "Affricâneg"
 
 #. Translators: Language name for ISO code "afh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Maithili"
 msgid "Afrihili"
-msgstr "Maithili"
+msgstr "Afrihili"
 
 #. Translators: Language name for ISO code "aii". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Assyrian Neo-Aramaic"
 msgstr "Serbeg"
 
 #. Translators: Language name for ISO code "ain". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ainu (Japan)"
-msgstr ""
+msgstr "Ainw (Siapan)"
 
 #. Translators: Language name for ISO code "ajp". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Arabic (Bahrain)"
 msgid "Arabic (South Levantine)"
@@ -115,15 +114,15 @@
 msgid "Aleut"
 msgstr "Alewteg"
 
 #. Translators: Language name for ISO code "alt". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Altai (Southern)"
-msgstr ""
+msgstr "Altai (Deheuol)"
 
 #. Translators: Language name for ISO code "am". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Amharic"
 msgstr "Amhareg"
 
@@ -132,18 +131,16 @@
 #. or other variant.
 msgid "Aragonese"
 msgstr "Aragoneg"
 
 #. Translators: Language name for ISO code "ang". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "English"
 msgid "English (Old)"
-msgstr "Saesneg"
+msgstr "Saesneg (Hen)"
 
 #. Translators: Language name for ISO code "anp". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Angika"
 msgstr "Angika"
 
@@ -195,15 +192,15 @@
 msgid "Arabic (Saudi Arabia)"
 msgstr "Arabeg (Saudi Arabia)"
 
 #. Translators: Language name for ISO code "ar_XB". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Arabic (XB pseudolocale)"
-msgstr ""
+msgstr "Arabeg (XB pseudolocale)"
 
 #. Translators: Language name for ISO code "ar_YE". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Arabic (Yemen)"
 msgstr "Arabeg (Yemen)"
 
@@ -226,15 +223,15 @@
 msgid "Arapaho"
 msgstr "Arapaho"
 
 #. Translators: Language name for ISO code "ars". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Arabic (Najdi)"
-msgstr ""
+msgstr "Arabeg (Najdi)"
 
 #. Translators: Language name for ISO code "arw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Arawak"
 msgstr "Arawaceg"
 
@@ -331,27 +328,27 @@
 msgid "Bavarian"
 msgstr "Bwlgareg"
 
 #. Translators: Language name for ISO code "bas". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Basa (Cameroon)"
-msgstr ""
+msgstr "Basa (Camerŵn)"
 
 #. Translators: Language name for ISO code "be". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Belarusian"
 msgstr "Belarwseg"
 
 #. Translators: Language name for ISO code "be_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Belarusian (latin)"
-msgstr ""
+msgstr "Belarwseg (lladin)"
 
 #. Translators: Language name for ISO code "bej". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Beja"
 msgstr "Bejäeg"
 
@@ -361,15 +358,15 @@
 msgid "Bemba"
 msgstr "Bembeg"
 
 #. Translators: Language name for ISO code "ber". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Berber"
-msgstr ""
+msgstr "Berber"
 
 #. Translators: Language name for ISO code "bez". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bena"
 msgstr "Bena"
 
@@ -379,15 +376,15 @@
 msgid "Bulgarian"
 msgstr "Bwlgareg"
 
 #. Translators: Language name for ISO code "bh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bihari"
-msgstr ""
+msgstr "Bihari"
 
 #. Translators: Language name for ISO code "bho". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bhojpuri"
 msgstr "Bhojpuri"
 
@@ -397,15 +394,15 @@
 msgid "Bislama"
 msgstr "Bislama"
 
 #. Translators: Language name for ISO code "bik". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bikol"
-msgstr ""
+msgstr "Bicol"
 
 #. Translators: Language name for ISO code "bin". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Bini"
 msgstr "Hindi"
@@ -440,15 +437,15 @@
 msgid "Bengali (India)"
 msgstr "Bengali (India)"
 
 #. Translators: Language name for ISO code "bnt". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bantu (Other)"
-msgstr ""
+msgstr "Bantw (Arall)"
 
 #. Translators: Language name for ISO code "bo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tibetan"
 msgstr "Tibeteg"
 
@@ -472,21 +469,21 @@
 msgid "Breton"
 msgstr "Llydaweg"
 
 #. Translators: Language name for ISO code "bra". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Braj"
-msgstr ""
+msgstr "Braj"
 
 #. Translators: Language name for ISO code "brb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Brao"
-msgstr ""
+msgstr "Brao"
 
 #. Translators: Language name for ISO code "brx". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bodo"
 msgstr "Bodo"
 
@@ -496,21 +493,21 @@
 msgid "Bosnian"
 msgstr "Bosnieg"
 
 #. Translators: Language name for ISO code "bs_Cyrl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bosnian (cyrillic)"
-msgstr ""
+msgstr "Bosnieg (cyrillig)"
 
 #. Translators: Language name for ISO code "bs_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bosnian (latin)"
-msgstr ""
+msgstr "Bosnieg (lladin)"
 
 #. Translators: Language name for ISO code "bua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Buriat"
 msgstr "Bwlgareg"
@@ -522,33 +519,34 @@
 msgid "Buginese"
 msgstr "Tsieinëeg"
 
 #. Translators: Language name for ISO code "byn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bilen"
-msgstr ""
+msgstr "Bilen"
 
 #. Translators: Language name for ISO code "ca". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Catalan"
 msgstr "Catalaneg"
 
 #. Translators: Language name for ISO code "ca@valencia". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
+#, fuzzy
 msgid "Valencian"
-msgstr ""
+msgstr "Falensianeg"
 
 #. Translators: Language name for ISO code "ca_AD". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Catalan (Andorra)"
-msgstr ""
+msgstr "Catalaneg (Andorra)"
 
 #. Translators: Language name for ISO code "cad". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Caddo"
 msgstr "Cado"
 
@@ -591,21 +589,21 @@
 msgid "Chamorro"
 msgstr "Tsiamorro"
 
 #. Translators: Language name for ISO code "chb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chibcha"
-msgstr ""
+msgstr "Chibcha"
 
 #. Translators: Language name for ISO code "chg". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chagatai"
-msgstr ""
+msgstr "Chagatai"
 
 #. Translators: Language name for ISO code "chk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Chuukese"
 msgstr "Tsieinëeg"
@@ -616,15 +614,15 @@
 msgid "Mari"
 msgstr "Marieg"
 
 #. Translators: Language name for ISO code "chn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chinook jargon"
-msgstr ""
+msgstr "Chinŵc"
 
 #. Translators: Language name for ISO code "cho". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Choctaw"
 msgstr "Siocto"
 
@@ -664,15 +662,15 @@
 msgid "Kurdish (Central, Iran)"
 msgstr ""
 
 #. Translators: Language name for ISO code "cnr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Montenegrin"
-msgstr ""
+msgstr "Montenegreg"
 
 #. Translators: Language name for ISO code "cnr_Cyrl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Montenegrin (cyrillic)"
 msgstr ""
 
@@ -2559,19 +2557,27 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Tsieinëeg"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Tsieinëeg"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Naplieg"
 
@@ -4024,18 +4030,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/da/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/da/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # scootergrisen <scootergrisen@gmail.com>, 2018, 2019, 2020, 2021.
 # Aputsiak Niels Janussen <aputtu@gmail.com>, 2021.
 # Aputsiaĸ Niels Janussen <aj@isit.gl>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Danish <https://hosted.weblate.org/projects/weblate/languages/"
 "da/>\n"
 "Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2467,18 +2467,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Kinesisk (traditionelt)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Kinesisk (minnan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitansk"
@@ -3878,19 +3888,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Kantonesisk (forenklet)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Kantonesisk"
+msgid "Yue (Traditional)"
+msgstr "Kantonesisk (traditionelt)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/de/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Christian Eichert <c@zp1.net>, 2021.
 # VfBFan <drop0815@posteo.de>, 2021, 2023.
 # Andrej Shadura <andrew@shadura.me>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: VfBFan <drop0815@posteo.de>\n"
 "Language-Team: German <https://hosted.weblate.org/projects/weblate/languages/"
 "de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2441,18 +2441,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl/Aztekisch"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinesisch (traditionell)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Min Nan/Minnan"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapolitanisch"
@@ -3821,19 +3831,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Mayathan"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Kantonesisch/Yue (vereinfacht)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Kantonesisch/Yue"
+msgid "Yue (Traditional)"
+msgstr "Kantonesisch/Yue (traditionell)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/django.pot` & `weblate-language-data-2023.4/weblate_language_data/locale/ang/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"Last-Translator: Automatically generated\n"
+"Language-Team: none\n"
+"Language: ang\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
@@ -2425,18 +2424,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3805,18 +3810,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/dv/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ars/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: dv\n"
+"Language: ars\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
@@ -2424,18 +2424,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3804,18 +3810,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/el/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/el/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Eugenia Russell <eugenia.russell2019@gmail.com>, 2021.
 # J. Lavoie <j.lavoie@net-c.ca>, 2021.
 # george kitsoukakis <norhorn@gmail.com>, 2021, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-02-05 15:59+0000\n"
 "Last-Translator: george kitsoukakis <norhorn@gmail.com>\n"
 "Language-Team: Greek <https://hosted.weblate.org/projects/weblate/languages/"
 "el/>\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2455,18 +2455,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Νάουατλ"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Κινέζικα (Παραδοσιακά)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Κινέζικα (Μιν Ναν)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Ναπολιτανικά"
@@ -3863,19 +3873,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Γιούε (Απλοποιημένα)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Γιούε"
+msgid "Yue (Traditional)"
+msgstr "Γιούε (Παραδοσιακά)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Ζουάνγκ"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/en_GB/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Adolfo Jayme Barrientos <fitojb@ubuntu.com>, 2021.
 # Andrej Shadura <andrew@shadura.me>, 2022.
+# Andi Chandler <andi@gowling.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2022-11-25 19:42+0000\n"
-"Last-Translator: Andrej Shadura <andrew@shadura.me>\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2023-04-02 13:34+0000\n"
+"Last-Translator: Andi Chandler <andi@gowling.com>\n"
 "Language-Team: English (United Kingdom) <https://hosted.weblate.org/projects/"
 "weblate/languages/en_GB/>\n"
 "Language: en_GB\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -79,35 +80,33 @@
 msgid "Assyrian Neo-Aramaic"
 msgstr "Assyrian Neo-Aramaic"
 
 #. Translators: Language name for ISO code "ain". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ainu (Japan)"
-msgstr ""
+msgstr "Ainu (Japan)"
 
 #. Translators: Language name for ISO code "ajp". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Arabic (Bahrain)"
 msgid "Arabic (South Levantine)"
-msgstr "Arabic (Bahrain)"
+msgstr "Arabic (South Levantine)"
 
 #. Translators: Language name for ISO code "ak". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Akan"
 msgstr "Akan"
 
 #. Translators: Language name for ISO code "akk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Akkadian"
-msgstr ""
+msgstr "Akkadian"
 
 #. Translators: Language name for ISO code "ale". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Aleut"
 msgstr ""
 
@@ -2467,18 +2466,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinese (Traditional)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Chinese (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapolitan"
@@ -3881,19 +3890,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (Simplified)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (Traditional)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/enm/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/dv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
-"Language: enm\n"
+"Language: dv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
@@ -2424,18 +2424,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3804,18 +3810,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/eo/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/eo/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Pierre Soubourou <pierre.soubourou@gmail.com>, 2019.
 # tuxayo/Victor Grousset <victor@tuxayo.net>, 2019.
 # Nikolay Korotkiy <sikmir@gmail.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Esperanto <https://hosted.weblate.org/projects/weblate/"
 "languages/eo/>\n"
 "Language: eo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2584,18 +2584,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Naŭatla"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Ĉina (tradicia)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Ĉina (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napola"
@@ -4052,19 +4062,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (simpligita)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (tradicia)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "ĝuanga"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/es/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/es/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # David Leal <halfpacho@gmail.com>, 2021.
 # Pablo Hinojosa <pablohn6@gmail.com>, 2022.
 # gallegonovato <fran-carro@hotmail.es>, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-03 18:36+0000\n"
 "Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
 "Language-Team: Spanish <https://hosted.weblate.org/projects/weblate/"
 "languages/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2432,18 +2432,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Náhuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chino (tradicional)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Chino (min nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitano"
@@ -3812,19 +3822,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Yucateco (Idioma Maya)"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Chino cantonés (simplificado)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Chino cantonés (yue)"
+msgid "Yue (Traditional)"
+msgstr "Chino cantonés (tradicional)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Chuan (zhuang)"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/et/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/et/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Janar Leas <janar.leas@gmail.com>, 2019.
-# Priit Jõerüüt <hwlate@joeruut.com>, 2020, 2021, 2022.
+# Priit Jõerüüt <hwlate@joeruut.com>, 2020, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2022-11-21 23:49+0000\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2023-03-10 11:02+0000\n"
 "Last-Translator: Priit Jõerüüt <hwlate@joeruut.com>\n"
 "Language-Team: Estonian <https://hosted.weblate.org/projects/weblate/"
 "languages/et/>\n"
 "Language: et\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "afari"
 
@@ -457,15 +457,15 @@
 msgid "Braj"
 msgstr "bradži"
 
 #. Translators: Language name for ISO code "brb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Brao"
-msgstr ""
+msgstr "lave"
 
 #. Translators: Language name for ISO code "brx". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Bodo"
 msgstr "bodo"
 
@@ -870,17 +870,16 @@
 #. or other variant.
 msgid "Efik"
 msgstr "efiki"
 
 #. Translators: Language name for ISO code "egl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
 msgid "Emilian"
-msgstr "Rumeenia"
+msgstr "emiilia"
 
 #. Translators: Language name for ISO code "egy". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Egyptian (Ancient)"
 msgstr "egiptuse"
 
@@ -1015,26 +1014,22 @@
 #. or other variant.
 msgid "Spanish"
 msgstr "hispaania"
 
 #. Translators: Language name for ISO code "es@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Spanish (Colombia)"
 msgid "Spanish (formal)"
-msgstr "hispaania (Colombia)"
+msgstr "hispaania (ametlik)"
 
 #. Translators: Language name for ISO code "es@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Spanish (Panama)"
 msgid "Spanish (informal)"
-msgstr "hispaania (Panama)"
+msgstr "hispaania (mitteametlik)"
 
 #. Translators: Language name for ISO code "es_419". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Spanish (Latin America)"
 msgstr "hispaania (Ladina Ameerika)"
 
@@ -1686,26 +1681,22 @@
 #. or other variant.
 msgid "Italian"
 msgstr "itaalia"
 
 #. Translators: Language name for ISO code "it@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "German (formal)"
 msgid "Italian (formal)"
-msgstr "saksa (ametlik)"
+msgstr "itaalia (ametlik)"
 
 #. Translators: Language name for ISO code "it@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "German (informal)"
 msgid "Italian (informal)"
-msgstr "saksa (mitteametlik)"
+msgstr "itaalia (mitteametlik)"
 
 #. Translators: Language name for ISO code "it_CH". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Italian (Switzerland)"
 msgstr "itaalia (Šveits)"
 
@@ -2347,15 +2338,15 @@
 msgid "Mon"
 msgstr "moni"
 
 #. Translators: Language name for ISO code "moe". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Innu"
-msgstr ""
+msgstr "innu"
 
 #. Translators: Language name for ISO code "moh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mohawk"
 msgstr "mohoogi"
 
@@ -2440,18 +2431,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "nahuatli"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "hiina (traditsiooniline)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "hiina (Lõuna Fujian)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "napoli"
@@ -2515,26 +2516,22 @@
 #. or other variant.
 msgid "Dutch"
 msgstr "hollandi"
 
 #. Translators: Language name for ISO code "nl@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "French (formal)"
 msgid "Dutch (formal)"
-msgstr "prantsuse (ametlik)"
+msgstr "hollandi (ametlik)"
 
 #. Translators: Language name for ISO code "nl@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "French (informal)"
 msgid "Dutch (informal)"
-msgstr "prantsuse (mitteametlik)"
+msgstr "hollandi (mitteametlik)"
 
 #. Translators: Language name for ISO code "nl_BE". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dutch (Belgium)"
 msgstr "hollandi (Belgia)"
 
@@ -2580,15 +2577,15 @@
 msgid "Pedi"
 msgstr "suuto"
 
 #. Translators: Language name for ISO code "nuk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nuu-chah-nulth"
-msgstr ""
+msgstr "nuutšanulti"
 
 #. Translators: Language name for ISO code "nv". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Navaho"
 msgstr "navajo"
 
@@ -2675,18 +2672,16 @@
 #. or other variant.
 msgid "Kokturk"
 msgstr "Kok-türgi"
 
 #. Translators: Language name for ISO code "ovd". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Italian"
 msgid "Elfdalian"
-msgstr "itaalia"
+msgstr "älvdali"
 
 #. Translators: Language name for ISO code "pa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Punjabi"
 msgstr "pandžabi"
 
@@ -2755,26 +2750,22 @@
 #. or other variant.
 msgid "Polish"
 msgstr "poola"
 
 #. Translators: Language name for ISO code "pl@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "French (formal)"
 msgid "Polish (formal)"
-msgstr "prantsuse (ametlik)"
+msgstr "poola (ametlik)"
 
 #. Translators: Language name for ISO code "pl@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "French (informal)"
 msgid "Polish (informal)"
-msgstr "prantsuse (mitteametlik)"
+msgstr "poola (mitteametlik)"
 
 #. Translators: Language name for ISO code "pms". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Piemontese"
 msgstr "piemonte"
 
@@ -2807,26 +2798,22 @@
 #. or other variant.
 msgid "Portuguese"
 msgstr "portugali"
 
 #. Translators: Language name for ISO code "pt@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Portuguese (Portugal)"
 msgid "Portuguese (formal)"
-msgstr "portugali (Portugal)"
+msgstr "portugali (ametlik)"
 
 #. Translators: Language name for ISO code "pt@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Portuguese (Portugal)"
 msgid "Portuguese (informal)"
-msgstr "portugali (Portugal)"
+msgstr "portugali (mitteametlik)"
 
 #. Translators: Language name for ISO code "pt_AO". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (Angola)"
 msgstr "portugali (Angola)"
 
@@ -2835,26 +2822,22 @@
 #. or other variant.
 msgid "Portuguese (Brazil)"
 msgstr "portugali (Brasiilia)"
 
 #. Translators: Language name for ISO code "pt_BR@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Portuguese (Portugal)"
 msgid "Portuguese (Brazil, formal)"
-msgstr "portugali (Portugal)"
+msgstr "Brasiilia portugali (ametlik)"
 
 #. Translators: Language name for ISO code "pt_BR@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Portuguese (Portugal)"
 msgid "Portuguese (Brazil, informal)"
-msgstr "portugali (Portugal)"
+msgstr "Brasiilia portugali (mitteametlik)"
 
 #. Translators: Language name for ISO code "pt_PT". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (Portugal)"
 msgstr "portugali (Portugal)"
 
@@ -2959,26 +2942,22 @@
 #. or other variant.
 msgid "Russian"
 msgstr "vene"
 
 #. Translators: Language name for ISO code "ru@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Russian (Ukraine)"
 msgid "Russian (formal)"
-msgstr "vene (Ukraina)"
+msgstr "vene (ametlik)"
 
 #. Translators: Language name for ISO code "ru@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "German (informal)"
 msgid "Russian (informal)"
-msgstr "saksa (mitteametlik)"
+msgstr "vene (mitteametlik)"
 
 #. Translators: Language name for ISO code "ru_UA". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian (Ukraine)"
 msgstr "vene (Ukraina)"
 
@@ -3150,32 +3129,29 @@
 #. or other variant.
 msgid "Sidamo"
 msgstr "sidamo"
 
 #. Translators: Language name for ISO code "sjd". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Sami, Kildin"
 msgid "Sami (Kildin)"
 msgstr "Kildini saami"
 
 #. Translators: Language name for ISO code "sk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Slovak"
 msgstr "slovaki"
 
 # src/trans.h:99
 #. Translators: Language name for ISO code "skr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
 msgid "Saraiki"
-msgstr "seriifideta"
+msgstr "seraiki"
 
 #. Translators: Language name for ISO code "sl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Slovenian"
 msgstr "sloveeni"
 
@@ -3364,23 +3340,22 @@
 #. or other variant.
 msgid "Swahili (Tanzania)"
 msgstr "suahiili (Tansaania)"
 
 #. Translators: Language name for ISO code "swg". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
 msgid "Swabian"
-msgstr "Serbia"
+msgstr "švaabi"
 
 #. Translators: Language name for ISO code "sxu". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Saxon (Upper)"
-msgstr ""
+msgstr "ülemsaksi"
 
 #. Translators: Language name for ISO code "syc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Syriac (Classical)"
 msgstr "vanasüüria (klassikaline)"
 
@@ -3785,26 +3760,22 @@
 #. or other variant.
 msgid "Westphalien"
 msgstr "westfaleni"
 
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
-msgstr "hiina (lihtsustatud)"
+msgstr "uu (lihtsustatud)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
-msgstr "hiina (traditsiooniline)"
+msgstr "uu (traditsiooniline)"
 
 #. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wolof"
 msgstr "volofi"
 
@@ -3850,21 +3821,27 @@
 msgid "Yoruba"
 msgstr "joruba"
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
-msgstr ""
+msgstr "maaja"
+
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "yue (lihtsustatud)"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "yue"
+msgid "Yue (Traditional)"
+msgstr "yue (traditsiooniline)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "tšuangi"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/eu/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/eu/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # S <sendoasojo@gmail.com>, 2019.
 # Osoitz <oelkoro@gmail.com>, 2020.
 # Iñigo Zendegi Urzelai <izendegi@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Basque <https://hosted.weblate.org/projects/weblate/languages/"
 "eu/>\n"
 "Language: eu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2584,18 +2584,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatlera"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Txinera (tradizionala)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Txinera (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "napoliera"
@@ -4052,19 +4062,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yuera (sinplifikatuta)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yuera"
+msgid "Yue (Traditional)"
+msgstr "Yuera (tradizionala)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuangera"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/fa/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/fa/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Abbas Baharforoosh <abahar1996@gmail.com>, 2020.
 # Mostafa Ahangarha <ahangarha@gmail.com>, 2020.
 # Mokhtar Garmehi <Mokhtar_garmeh@yahoo.com>, 2021, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-02-23 00:57+0000\n"
 "Last-Translator: Mokhtar Garmehi <Mokhtar_garmeh@yahoo.com>\n"
 "Language-Team: Persian <https://hosted.weblate.org/projects/weblate/"
 "languages/fa/>\n"
 "Language: fa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2508,18 +2508,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "ناهواتل"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "چینی (سنتی)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "چینی (مین نان)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "ناپلی"
@@ -3947,19 +3957,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "یو (ساده شده)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "یو"
+msgid "Yue (Traditional)"
+msgstr "یو (سنتی)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "چوانگی"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/fi/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/fi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Demian Wright <wright.demian+weblate@gmail.com>, 2021.
 # Jiri Nakola <github@nakola.fi>, 2022.
 # J. Lavoie <j.lavoie@net-c.ca>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-01-05 16:51+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Finnish <https://hosted.weblate.org/projects/weblate/"
 "languages/fi/>\n"
 "Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2444,18 +2444,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Kiina (perinteinen)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Kiina (Minnan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napoli"
@@ -3854,19 +3864,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Kantoninkiina (yksinkertainen)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Kantoninkiina"
+msgid "Yue (Traditional)"
+msgstr "Kantoninkiina (perinteinen)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/fil/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/fil/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 # Marco Santos <enum.scima@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-08-19 03:21+0000\n"
 "Last-Translator: Marco Santos <enum.scima@gmail.com>\n"
 "Language-Team: Filipino <https://hosted.weblate.org/projects/weblate/"
 "languages/fil/>\n"
 "Language: fil\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2438,18 +2438,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Tsino (Tradisyonal)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Tsino (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapolitan"
@@ -3850,19 +3860,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (Pinasimple)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (Tradisyonal)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/fr/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/fr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # J. Lavoie <j.lavoie@net-c.ca>, 2020, 2021, 2022.
 # Simon Picot <simonpicot06@gmail.com>, 2021.
 # tachyglossues <tachyglossues@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-01-31 01:05+0000\n"
 "Last-Translator: tachyglossues <tachyglossues@gmail.com>\n"
 "Language-Team: French <https://hosted.weblate.org/projects/weblate/languages/"
 "fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2431,18 +2431,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinois (Traditionnel)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Minnan"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitain"
@@ -3811,19 +3821,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "yucateco"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Cantonais (Simplifié)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Cantonais"
+msgid "Yue (Traditional)"
+msgstr "Cantonais (Traditionnel)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/fur/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/fur/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 # adecorte <adecorte@gmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-12-24 02:14+0000\n"
 "Last-Translator: adecorte <adecorte@gmail.com>\n"
 "Language-Team: Friulian <https://hosted.weblate.org/projects/weblate/"
 "languages/fur/>\n"
 "Language: fur\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2497,19 +2497,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "cinês"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "cinês"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "napoletan"
 
@@ -3919,18 +3929,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/fy/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/fy/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Frisian <https://hosted.weblate.org/projects/weblate/"
 "languages/fy/>\n"
 "Language: fy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2649,20 +2649,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Taiwan)"
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Sineesk (Taiwan)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Taiwan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Sineesk (Taiwan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitaansk"
@@ -4139,18 +4147,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/gl/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/gl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Iván Seoane <ivanrsm1997@gmail.com>, 2018, 2019.
 # Iváns <ivanrsm1997@gmail.com>, 2019, 2020.
 # gallegonovato <fran-carro@hotmail.es>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-11-25 19:42+0000\n"
 "Last-Translator: gallegonovato <fran-carro@hotmail.es>\n"
 "Language-Team: Galician <https://hosted.weblate.org/projects/weblate/"
 "languages/gl/>\n"
 "Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2522,18 +2522,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Náhuatl ou azteca"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinés (Tradicional)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Chinés (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitano"
@@ -3990,19 +4000,25 @@
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Yucateco"
 msgstr "Aguacateco"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Chinés cantonés (Sinxelo)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue (Chinés cantonés)"
+msgid "Yue (Traditional)"
+msgstr "Chinés cantonés (Tradicional)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/he/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/he/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Omeritzics Games <omeritzicschwartz@gmail.com>, 2020.
 # Omer I.S. <omeritzicschwartz@gmail.com>, 2021.
 # Tzvika <mmm_45@walla.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-01-31 01:49+0000\n"
 "Last-Translator: Yaron Shahrabani <sh.yaron@gmail.com>\n"
 "Language-Team: Hebrew <https://hosted.weblate.org/projects/weblate/languages/"
 "he/>\n"
 "Language: he\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2429,18 +2429,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "נאוואטל"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "סינית מסורתית"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "סינית (מין של האי נאן)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "נפוליטנית"
@@ -3809,19 +3819,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "יוקטקו"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "יו מפושטת"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "יו"
+msgid "Yue (Traditional)"
+msgstr "יו מסורתית"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "ג׳ואנג"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/hi/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/hi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # Deepak Mathur <deepakmathur174@gmail.com>, 2020.
 # KushagraKarira <kushagrakarira@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-12-17 17:49+0000\n"
 "Last-Translator: KushagraKarira <kushagrakarira@gmail.com>\n"
 "Language-Team: Hindi <https://hosted.weblate.org/projects/weblate/languages/"
 "hi/>\n"
 "Language: hi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2517,19 +2517,27 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "चीनी"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Chinese (Min Nan, Latin)"
+msgstr "चीनी"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "नीपोलिटन"
 
@@ -3974,18 +3982,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "ज़ुआंग"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/hr/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/hr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Marino <mrabach@gmail.com>, 2019, 2020.
 # Milo Ivir <mail@milotype.de>, 2019, 2020, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2023-01-19 06:18+0000\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2023-03-03 21:37+0000\n"
 "Last-Translator: Milo Ivir <mail@milotype.de>\n"
 "Language-Team: Croatian <https://hosted.weblate.org/projects/weblate/"
 "languages/hr/>\n"
 "Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
 "%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.15.1-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afarski"
 
@@ -1015,26 +1015,22 @@
 #. or other variant.
 msgid "Spanish"
 msgstr "Španjolski"
 
 #. Translators: Language name for ISO code "es@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Spanish (Colombia)"
 msgid "Spanish (formal)"
-msgstr "Španjolski (Kolumbija)"
+msgstr "Španjolski (službeni)"
 
 #. Translators: Language name for ISO code "es@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Spanish (Panama)"
 msgid "Spanish (informal)"
-msgstr "Španjolski (Panama)"
+msgstr "Španjolski (neslužbeni)"
 
 #. Translators: Language name for ISO code "es_419". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Spanish (Latin America)"
 msgstr "Španjolski (Latinska Amerika)"
 
@@ -1685,26 +1681,22 @@
 #. or other variant.
 msgid "Italian"
 msgstr "Talijanski"
 
 #. Translators: Language name for ISO code "it@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "German (formal)"
 msgid "Italian (formal)"
-msgstr "Njemački (službeni)"
+msgstr "Talijanski (službeni)"
 
 #. Translators: Language name for ISO code "it@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "German (informal)"
 msgid "Italian (informal)"
-msgstr "Njemački (neslužbeni)"
+msgstr "Talijanski (neslužbeni)"
 
 #. Translators: Language name for ISO code "it_CH". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Italian (Switzerland)"
 msgstr "Talijanski (Švicarska)"
 
@@ -2436,18 +2428,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatlski"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Kineski (tradicionalni)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Kineski (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitanski"
@@ -2511,26 +2513,22 @@
 #. or other variant.
 msgid "Dutch"
 msgstr "Nizozemski"
 
 #. Translators: Language name for ISO code "nl@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "French (formal)"
 msgid "Dutch (formal)"
-msgstr "Francuski (službeni)"
+msgstr "Nizozemski (službeni)"
 
 #. Translators: Language name for ISO code "nl@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "French (informal)"
 msgid "Dutch (informal)"
-msgstr "Francuski (neslužbeni)"
+msgstr "Nizozemski (neslužbeni)"
 
 #. Translators: Language name for ISO code "nl_BE". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dutch (Belgium)"
 msgstr "Nizozemski (Belgija)"
 
@@ -2749,26 +2747,22 @@
 #. or other variant.
 msgid "Polish"
 msgstr "Poljski"
 
 #. Translators: Language name for ISO code "pl@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "French (formal)"
 msgid "Polish (formal)"
-msgstr "Francuski (službeni)"
+msgstr "Poljski (službeni)"
 
 #. Translators: Language name for ISO code "pl@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "French (informal)"
 msgid "Polish (informal)"
-msgstr "Francuski (neslužbeni)"
+msgstr "Poljski (neslužbeni)"
 
 #. Translators: Language name for ISO code "pms". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Piemontese"
 msgstr "Pijemontski"
 
@@ -2801,26 +2795,22 @@
 #. or other variant.
 msgid "Portuguese"
 msgstr "Portugalski"
 
 #. Translators: Language name for ISO code "pt@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Portuguese (Portugal)"
 msgid "Portuguese (formal)"
-msgstr "Portugalski (Portugal)"
+msgstr "Portugalski (službeni)"
 
 #. Translators: Language name for ISO code "pt@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Portuguese (Portugal)"
 msgid "Portuguese (informal)"
-msgstr "Portugalski (Portugal)"
+msgstr "Portugalski (neslužbeni)"
 
 #. Translators: Language name for ISO code "pt_AO". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (Angola)"
 msgstr "Portugalski (Angola)"
 
@@ -2829,26 +2819,22 @@
 #. or other variant.
 msgid "Portuguese (Brazil)"
 msgstr "Portugalski (Brazil)"
 
 #. Translators: Language name for ISO code "pt_BR@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Portuguese (Portugal)"
 msgid "Portuguese (Brazil, formal)"
-msgstr "Portugalski (Portugal)"
+msgstr "Portugalski (Brazil, službeni)"
 
 #. Translators: Language name for ISO code "pt_BR@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Portuguese (Portugal)"
 msgid "Portuguese (Brazil, informal)"
-msgstr "Portugalski (Portugal)"
+msgstr "Portugalski (Brazil, neslužbeni)"
 
 #. Translators: Language name for ISO code "pt_PT". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (Portugal)"
 msgstr "Portugalski (Portugal)"
 
@@ -2953,26 +2939,22 @@
 #. or other variant.
 msgid "Russian"
 msgstr "Ruski"
 
 #. Translators: Language name for ISO code "ru@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Russian (Ukraine)"
 msgid "Russian (formal)"
-msgstr "Ruski (Ukrajina)"
+msgstr "Ruski (službeni)"
 
 #. Translators: Language name for ISO code "ru@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "German (informal)"
 msgid "Russian (informal)"
-msgstr "Njemački (neslužbeni)"
+msgstr "Ruski (neslužbeni)"
 
 #. Translators: Language name for ISO code "ru_UA". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian (Ukraine)"
 msgstr "Ruski (Ukrajina)"
 
@@ -3156,15 +3138,15 @@
 msgid "Slovak"
 msgstr "Slovački"
 
 #. Translators: Language name for ISO code "skr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Saraiki"
-msgstr ""
+msgstr "Saraiki"
 
 #. Translators: Language name for ISO code "sl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Slovenian"
 msgstr "Slovenski"
 
@@ -3773,26 +3755,22 @@
 #. or other variant.
 msgid "Westphalien"
 msgstr "Vestfalski"
 
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Simplified)"
 msgid "Wu (Simplified)"
-msgstr "Kineski (pojednostavljeni)"
+msgstr "Wu (pojednostavljeni)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Chinese (Traditional)"
 msgid "Wu (Traditional)"
-msgstr "Kineski (tradicionalni)"
+msgstr "Wu (tradicionalni)"
 
 #. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wolof"
 msgstr "Volof"
 
@@ -3840,19 +3818,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Yucateco"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (pojednostavljeni)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (tradicionalni)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/hu/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/hu/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # ovari <ovari123@zoho.com>, 2020.
 # Balázs Meskó <meskobalazs@mailbox.org>, 2021, 2022.
 # f3rr31 <5920873@disroot.org>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-01-25 02:44+0000\n"
 "Last-Translator: Balázs Meskó <meskobalazs@mailbox.org>\n"
 "Language-Team: Hungarian <https://hosted.weblate.org/projects/weblate/"
 "languages/hu/>\n"
 "Language: hu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2472,18 +2472,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Navatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Kínai (hagyományos)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Kínai (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Nápolyi"
@@ -3894,19 +3904,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Kantoni (egyszerűsített)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Kantoni"
+msgid "Yue (Traditional)"
+msgstr "Kantoni (hagyományos)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Csuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/hy/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/hy/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2015.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2016-01-14 14:59+0000\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Armenian <https://hosted.weblate.org/projects/weblate/master/"
 "hy/>\n"
 "Language: hy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2579,19 +2579,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "չինարեն"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "չինարեն"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "նեապոլերեն"
 
@@ -4033,18 +4043,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "ժուանգ"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ia/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ia/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ia\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2505,19 +2505,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "chinese"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "chinese"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "napolitano"
 
@@ -3935,18 +3945,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/id/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/id/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Linerly <linerly@protonmail.com>, 2022, 2023.
 # Taufik A. Wicaksono <taufikadi.wicaksono@tutamail.com>, 2022.
 # Taufik Adi Wicaksono <taufikadi.wicaksono@tutamail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: Linerly <linerly@protonmail.com>\n"
 "Language-Team: Indonesian <https://hosted.weblate.org/projects/weblate/"
 "languages/id/>\n"
 "Language: id\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2433,18 +2433,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Cina (Tradisional)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Cina (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapolitan"
@@ -3813,19 +3823,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Yucateco"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (Sederhana)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (Tradisional)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ie/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/enm/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
-# OIS <mistresssilvara@hotmail.com>, 2021.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2021-03-26 11:37+0000\n"
-"Last-Translator: OIS <mistresssilvara@hotmail.com>\n"
-"Language-Team: Occidental <https://hosted.weblate.org/projects/weblate/"
-"languages/ie/>\n"
-"Language: ie\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: Automatically generated\n"
+"Language-Team: none\n"
+"Language: enm\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.5.2\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr ""
 
@@ -1626,15 +1624,15 @@
 msgid "Indonesian"
 msgstr ""
 
 #. Translators: Language name for ISO code "ie". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Occidental"
-msgstr "Interlingue"
+msgstr ""
 
 #. Translators: Language name for ISO code "ig". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Igbo"
 msgstr ""
 
@@ -2426,18 +2424,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -2922,37 +2926,33 @@
 msgid "Romany"
 msgstr ""
 
 #. Translators: Language name for ISO code "ru". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian"
-msgstr "Russ"
+msgstr ""
 
 #. Translators: Language name for ISO code "ru@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Russian (Ukraine)"
 msgid "Russian (formal)"
-msgstr "Russ (Ukraina)"
+msgstr ""
 
 #. Translators: Language name for ISO code "ru@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Russian (Ukraine)"
 msgid "Russian (informal)"
-msgstr "Russ (Ukraina)"
+msgstr ""
 
 #. Translators: Language name for ISO code "ru_UA". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian (Ukraine)"
-msgstr "Russ (Ukraina)"
+msgstr ""
 
 #. Translators: Language name for ISO code "rue". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Rusyn"
 msgstr ""
 
@@ -3810,18 +3810,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/is/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/is/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Weblate <noreply@weblate.org>, 2020.
 # Sveinn í Felli <sv1@fellsnet.is>, 2020, 2021, 2022, 2023.
 # Þórhalla Guðmundsdóttir Beck <plergux@outlook.com>, 2020, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: Sveinn í Felli <sv1@fellsnet.is>\n"
 "Language-Team: Icelandic <https://hosted.weblate.org/projects/weblate/"
 "languages/is/>\n"
 "Language: is\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2428,18 +2428,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Kínverska (hefðbundin)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Kínverska (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapólíska"
@@ -3808,19 +3818,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Yucateco (Maya)"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue-kínverska (einfölduð)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue-kínverska"
+msgid "Yue (Traditional)"
+msgstr "Yue-kínverska (hefðbundin)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhúang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/it/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/it/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # giuseppe <g.pecoraro@odissea.at>, 2021.
 # ROBERTO BORIOTTI <roberto.boriotti@gmail.com>, 2021.
 # bovirus <roberto.boriotti@canon.it>, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: bovirus <roberto.boriotti@canon.it>\n"
 "Language-Team: Italian <https://hosted.weblate.org/projects/weblate/"
 "languages/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2435,18 +2435,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Cinese (Tradizionale)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Cinese (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napoletano"
@@ -3815,19 +3825,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Yucateco"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (Semplificato)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (Tradizionale)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ja/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 # ht1722 <taichi_19990611@yahoo.co.jp>, 2022.
 # amano <amano@users.noreply.hosted.weblate.org>, 2023.
 # SAIHAZE <saihaze@outlook.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2023-02-05 17:22+0000\n"
-"Last-Translator: amano <amano@users.noreply.hosted.weblate.org>\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2023-04-02 00:21+0000\n"
+"Last-Translator: Kyotaro Iijima <kyotaro.eyes@gmail.com>\n"
 "Language-Team: Japanese <https://hosted.weblate.org/projects/weblate/"
 "languages/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.17-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "アファル語"
 
@@ -813,21 +813,21 @@
 msgid "German"
 msgstr "ドイツ語"
 
 #. Translators: Language name for ISO code "de@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "German (formal)"
-msgstr "ドイツ語 (敬称)"
+msgstr "ドイツ語 (フォーマル)"
 
 #. Translators: Language name for ISO code "de@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "German (informal)"
-msgstr "ドイツ語 (親称)"
+msgstr "ドイツ語 (インフォーマル)"
 
 #. Translators: Language name for ISO code "de_1901". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "German (old spelling)"
 msgstr "ドイツ語 (古いスペル)"
 
@@ -1092,21 +1092,21 @@
 msgid "Spanish"
 msgstr "スペイン語"
 
 #. Translators: Language name for ISO code "es@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Spanish (formal)"
-msgstr "スペイン語 (敬称)"
+msgstr "スペイン語 (フォーマル)"
 
 #. Translators: Language name for ISO code "es@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Spanish (informal)"
-msgstr "スペイン語 (親称)"
+msgstr "スペイン語 (インフォーマル)"
 
 #. Translators: Language name for ISO code "es_419". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Spanish (Latin America)"
 msgstr "スペイン語 (ラテンアメリカ)"
 
@@ -1299,21 +1299,21 @@
 msgid "French"
 msgstr "フランス語"
 
 #. Translators: Language name for ISO code "fr@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "French (formal)"
-msgstr "フランス語 (敬称)"
+msgstr "フランス語 (フォーマル)"
 
 #. Translators: Language name for ISO code "fr@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "French (informal)"
-msgstr "フランス語 (親称)"
+msgstr "フランス語 (インフォーマル)"
 
 #. Translators: Language name for ISO code "fr_AG". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "French (Antigua and Barbuda)"
 msgstr "フランス語 (アンティグア・バーブーダ)"
 
@@ -1791,21 +1791,21 @@
 msgid "Italian"
 msgstr "イタリア語"
 
 #. Translators: Language name for ISO code "it@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Italian (formal)"
-msgstr "イタリア語 (敬称)"
+msgstr "イタリア語 (フォーマル)"
 
 #. Translators: Language name for ISO code "it@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Italian (informal)"
-msgstr "イタリア語 (親称)"
+msgstr "イタリア語 (インフォーマル)"
 
 #. Translators: Language name for ISO code "it_CH". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Italian (Switzerland)"
 msgstr "イタリア語 (スイス)"
 
@@ -2604,18 +2604,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "ナワトル語"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "中国語 (繁体字)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "中国語 (ビン南)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "ナポリ語"
@@ -2684,21 +2694,21 @@
 msgid "Dutch"
 msgstr "オランダ語"
 
 #. Translators: Language name for ISO code "nl@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dutch (formal)"
-msgstr "オランダ語 (敬称)"
+msgstr "オランダ語 (フォーマル)"
 
 #. Translators: Language name for ISO code "nl@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dutch (informal)"
-msgstr "オランダ語 (親称)"
+msgstr "オランダ語 (インフォーマル)"
 
 #. Translators: Language name for ISO code "nl_BE". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dutch (Belgium)"
 msgstr "オランダ語 (ベルギー)"
 
@@ -2930,21 +2940,21 @@
 msgid "Polish"
 msgstr "ポーランド語"
 
 #. Translators: Language name for ISO code "pl@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Polish (formal)"
-msgstr "ポーランド語 (敬称)"
+msgstr "ポーランド語 (フォーマル)"
 
 #. Translators: Language name for ISO code "pl@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Polish (informal)"
-msgstr "ポーランド語 (親称)"
+msgstr "ポーランド語 (インフォーマル)"
 
 #. Translators: Language name for ISO code "pms". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Piemontese"
 msgstr "ピエモンテ語"
 
@@ -2981,21 +2991,21 @@
 msgid "Portuguese"
 msgstr "ポルトガル語"
 
 #. Translators: Language name for ISO code "pt@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (formal)"
-msgstr "ポルトガル語 (敬称)"
+msgstr "ポルトガル語 (フォーマル)"
 
 #. Translators: Language name for ISO code "pt@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (informal)"
-msgstr "ポルトガル語 (親称)"
+msgstr "ポルトガル語 (インフォーマル)"
 
 #. Translators: Language name for ISO code "pt_AO". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (Angola)"
 msgstr "ポルトガル語 (アンゴラ)"
 
@@ -3005,21 +3015,21 @@
 msgid "Portuguese (Brazil)"
 msgstr "ポルトガル語 (ブラジル)"
 
 #. Translators: Language name for ISO code "pt_BR@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (Brazil, formal)"
-msgstr "ポルトガル語 (ブラジル、敬称)"
+msgstr "ポルトガル語 (ブラジル、フォーマル)"
 
 #. Translators: Language name for ISO code "pt_BR@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (Brazil, informal)"
-msgstr "ポルトガル語 (ブラジル、親称)"
+msgstr "ポルトガル語 (ブラジル、インフォーマル)"
 
 #. Translators: Language name for ISO code "pt_PT". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (Portugal)"
 msgstr "ポルトガル語 (ポルトガル)"
 
@@ -3133,21 +3143,21 @@
 msgid "Russian"
 msgstr "ロシア語"
 
 #. Translators: Language name for ISO code "ru@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian (formal)"
-msgstr "ロシア語 (敬称)"
+msgstr "ロシア語 (フォーマル)"
 
 #. Translators: Language name for ISO code "ru@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian (informal)"
-msgstr "ロシア語 (親称)"
+msgstr "ロシア語 (インフォーマル)"
 
 #. Translators: Language name for ISO code "ru_UA". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian (Ukraine)"
 msgstr "ロシア語 (ウクライナ)"
 
@@ -4073,19 +4083,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "ユカテコ語"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "粤語 (簡体字)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "粤語"
+msgid "Yue (Traditional)"
+msgstr "粤語 (繁体字)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "チワン語"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ka/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ka/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # George Salukvadze <giosal90@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-08-25 13:17+0000\n"
 "Last-Translator: George Salukvadze <giosal90@gmail.com>\n"
 "Language-Team: Georgian <https://hosted.weblate.org/projects/weblate/"
 "languages/ka/>\n"
 "Language: ka\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2430,19 +2430,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "ჩინური, მანდარინი"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "ჩინური, მანდარინი"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "ნეაპოლიტური"
 
@@ -3824,18 +3834,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/kab/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/kab/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Muḥend Belqasem <belkacem77@gmail.com>, 2020.
 # Ouchene <merzouk.ouchene@laposte.net>, 2020.
 # Kahina Messaoudi <messaoudikahina02@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Kabyle <https://hosted.weblate.org/projects/weblate/languages/"
 "kab/>\n"
 "Language: kab\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2550,18 +2550,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Tanuhatit"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Tacinwat (Tamansayt)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Tacinwat (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Tanapolitant"
@@ -4002,19 +4012,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (Taḥerfit)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (Tamansayt)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/kk/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/kk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Weblate <noreply@weblate.org>, 2019.
 # WWWesten <wwwesten@gmail.com>, 2019.
 # Kuwanish Orinbay <firstpeople111@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Kazakh <https://hosted.weblate.org/projects/weblate/languages/"
 "kk/>\n"
 "Language: kk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2588,18 +2588,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuátl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Hanzý (dástúr)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Hanzý (Mın-Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapolıtan"
@@ -4056,19 +4066,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Iýe (jeńil)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Iýe"
+msgid "Yue (Traditional)"
+msgstr "Iýe (dástúr)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Juań"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/km/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/km/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # ប៉ុកណូ រ៉ូយ៉ាល់ <royalpokno68@gmail.com>, 2019, 2020, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Khmer (Central) <https://hosted.weblate.org/projects/weblate/"
 "languages/km/>\n"
 "Language: km\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2558,19 +2558,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "ចិនកុកងឺ"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "ចិនកុកងឺ"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "នាប៉ូលីតាន"
 
@@ -4010,18 +4020,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "ហ្សួង"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/kmr/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/kmr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Pêşeroja paşerojê <cyax1@protonmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-01-14 19:28+0000\n"
 "Last-Translator: Pêşeroja paşerojê <cyax1@protonmail.com>\n"
 "Language-Team: Kurdish (Northern) <https://hosted.weblate.org/projects/"
 "weblate/languages/kmr/>\n"
 "Language: kmr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2596,20 +2596,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahwatlî"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Çînî (Kevneşopî)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Mandarin)"
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Çînî (Mandarîn)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolîtanî"
@@ -4062,19 +4070,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Kantonî (Sadekirî)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Kantonî"
+msgid "Yue (Traditional)"
+msgstr "Kantonî (Kevneşopî)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ko/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ko/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Hoseok Seo <ddinghoya@gmail.com>, 2022.
 # 이정희 <daemul72@gmail.com>, 2023.
 # Yi Yunseok <ironyunseok@protonmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-13 06:26+0000\n"
 "Last-Translator: 이정희 <daemul72@gmail.com>\n"
 "Language-Team: Korean <https://hosted.weblate.org/projects/weblate/languages/"
 "ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2434,18 +2434,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "나우아틀어"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "중국어 (번체)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "중국어 (북경)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "나폴리어"
@@ -3816,19 +3826,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "유카텍어"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "웨어 (간체)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "웨어"
+msgid "Yue (Traditional)"
+msgstr "웨어 (번체)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "주앙어"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ksh/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ksh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Automatically generated, 2014.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2014-10-01 09:41+0200\n"
 "Last-Translator: Michal Čihař <michal@cihar.com>\n"
 "Language-Team: Colognian <https://hosted.weblate.org/projects/weblate/master/"
 "ksh/>\n"
 "Language: ksh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2648,20 +2648,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Taiwan)"
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Schenehsesch (us Taiwan)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Taiwan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Schenehsesch (us Taiwan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Nappulitahnesch"
@@ -4130,18 +4138,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ln/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ln/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Lingala <https://hosted.weblate.org/projects/weblate/"
 "languages/ln/>\n"
 "Language: ln\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2553,19 +2553,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "lisinwa"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "lisinwa"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
 
@@ -3981,18 +3991,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/lt/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/lt/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Lithuanian <https://hosted.weblate.org/projects/weblate/"
 "languages/lt/>\n"
 "Language: lt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2571,20 +2571,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Traditional)"
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "kinų (tradicinė)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "kinų (tradicinė)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "neapoliečių"
@@ -4028,18 +4036,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "chuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/lv/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/lv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # Coool (github.com/Coool) <coool@mail.lv>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-11-01 13:11+0000\n"
 "Last-Translator: Coool (github.com/Coool) <coool@mail.lv>\n"
 "Language-Team: Latvian <https://hosted.weblate.org/projects/weblate/"
 "languages/lv/>\n"
 "Language: lv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2490,19 +2490,27 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Ķīniešu"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Ķīniešu"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapoliešu"
 
@@ -3949,18 +3957,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/lzh/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/lzh/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # Xiang Heng Wei <yylteam@hotmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-01-21 09:23+0000\n"
 "Last-Translator: Xiang Heng Wei <yylteam@hotmail.com>\n"
 "Language-Team: Chinese (Literary) <https://hosted.weblate.org/projects/"
 "weblate/languages/lzh/>\n"
 "Language: lzh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2434,18 +2434,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "中文(繁体)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "中文(闽南)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3836,18 +3846,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/mk/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/mk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Macedonian <https://hosted.weblate.org/projects/weblate/"
 "languages/mk/>\n"
 "Language: mk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2586,20 +2586,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 #| msgid "Chinese (Hong Kong)"
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Кинески (Хонг Конг)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Hong Kong)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Кинески (Хонг Конг)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "неаполски"
@@ -4053,18 +4061,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "џуаншки"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ml/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ml/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ml\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2505,19 +2505,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "ചൈനീസ്, മാൻഡറിൻ"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "ചൈനീസ്, മാൻഡറിൻ"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "നെപ്പോളിറ്റന്‍"
 
@@ -3939,18 +3949,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "സ്വാംഗ്"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/mr/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/mr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 # Prachi Joshi <josprachi@yahoo.com>, 2019, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Marathi <https://hosted.weblate.org/projects/weblate/"
 "languages/mr/>\n"
 "Language: mr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2556,18 +2556,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "नावातल"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "चीनी (पारंपारिक)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "चायनीज, मिन नान"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "नेपोलिटान"
@@ -4016,19 +4026,25 @@
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Yucateco"
 msgstr "अगुआकटेको"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "यू (सरलीकृत)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "यू"
+msgid "Yue (Traditional)"
+msgstr "यू (पारंपारिक)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "झुआंग"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ms/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ms/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ms\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2540,19 +2540,27 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinese"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Chinese"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Neapolitan"
 msgstr "_Alias baru"
@@ -4004,18 +4012,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/my/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/my/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Sithu Aung <sithu.aung015@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Burmese <https://hosted.weblate.org/projects/weblate/"
 "languages/my/>\n"
 "Language: my\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2546,19 +2546,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "တရုတ် (ရိုးရာ)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Pinyin)"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "တရုတ် (ဖင်းရင်း)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "နပိုလီတန်"
 
@@ -3988,18 +3998,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/nb/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/nb/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Kurt Eilertsen <kurt@kheds.com>, 2018.
 # Petter Reinholdtsen <pere-weblate@hungry.com>, 2019.
 # FTno <ft-002@tutanota.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-09-30 22:09+0000\n"
 "Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/weblate/"
 "languages/nb_NO/>\n"
 "Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2525,18 +2525,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Aztekisk"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Kinesisk (Tradisjonell)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Kinesisk (Minnan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitansk"
@@ -3973,19 +3983,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Kantonesisk (Forenklet)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Kantonesisk"
+msgid "Yue (Traditional)"
+msgstr "Kantonesisk (Tradisjonell)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/nl/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/nl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Jaimie85 <alsemgeest@gmail.com>, 2020.
 # Heimen Stoffels <vistausss@outlook.com>, 2020, 2021.
 # Heimen Stoffels <vistausss@fastmail.com>, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-01-31 01:49+0000\n"
 "Last-Translator: Heimen Stoffels <vistausss@fastmail.com>\n"
 "Language-Team: Dutch <https://hosted.weblate.org/projects/weblate/languages/"
 "nl/>\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2430,18 +2430,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinees (traditioneel)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Chinees (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitaans"
@@ -3810,19 +3820,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Yucateco"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Kantonees (vereenvoudigd)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Kantonees"
+msgid "Yue (Traditional)"
+msgstr "Kantonees (traditioneel)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/nn/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/nn/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: nn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -1706,15 +1706,14 @@
 msgid "Italian"
 msgstr "Italiensk"
 
 #. Translators: Language name for ISO code "it@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
-#| msgid "Italian"
 msgid "Italian (formal)"
 msgstr "Italiensk"
 
 #. Translators: Language name for ISO code "it@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Italian (informal)"
@@ -2375,15 +2374,15 @@
 msgid "Mandinka"
 msgstr ""
 
 #. Translators: Language name for ISO code "mnw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mon"
-msgstr ""
+msgstr "må."
 
 #. Translators: Language name for ISO code "moe". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Innu"
 msgstr ""
 
@@ -2475,19 +2474,27 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Kinesisk"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Kinesisk"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitansk"
 
@@ -2713,15 +2720,14 @@
 msgid "Kokturk"
 msgstr ""
 
 #. Translators: Language name for ISO code "ovd". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
-#| msgid "Italian"
 msgid "Elfdalian"
 msgstr "Italiensk"
 
 #. Translators: Language name for ISO code "pa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Punjabi"
@@ -2843,23 +2849,21 @@
 msgid "Portuguese"
 msgstr "Portugisisk"
 
 #. Translators: Language name for ISO code "pt@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
-#| msgid "Portuguese"
 msgid "Portuguese (formal)"
 msgstr "Portugisisk"
 
 #. Translators: Language name for ISO code "pt@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
-#| msgid "Portuguese"
 msgid "Portuguese (informal)"
 msgstr "Portugisisk"
 
 #. Translators: Language name for ISO code "pt_AO". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (Angola)"
@@ -2871,23 +2875,21 @@
 msgid "Portuguese (Brazil)"
 msgstr ""
 
 #. Translators: Language name for ISO code "pt_BR@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
-#| msgid "Portuguese"
 msgid "Portuguese (Brazil, formal)"
 msgstr "Portugisisk"
 
 #. Translators: Language name for ISO code "pt_BR@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
-#| msgid "Portuguese"
 msgid "Portuguese (Brazil, informal)"
 msgstr "Portugisisk"
 
 #. Translators: Language name for ISO code "pt_PT". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Portuguese (Portugal)"
@@ -3839,23 +3841,21 @@
 msgid "Westphalien"
 msgstr ""
 
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
-#| msgid "Simplified Chinese"
 msgid "Wu (Simplified)"
 msgstr "forenkla kinesisk"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
-#| msgid "Traditional Chinese"
 msgid "Wu (Traditional)"
 msgstr "tradisjonell kinesisk"
 
 #. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wolof"
@@ -3907,18 +3907,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "zhuang"
@@ -3992,15 +3998,20 @@
 #. Translators: Language name for ISO code "zza". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Zaza"
 msgstr "Kasakhisk"
 
+#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan)"
+msgstr ""
+
 #, fuzzy
 #~ msgid "Wu"
 #~ msgstr "Naurisk"
 
 #, fuzzy
-#~| msgid "Portuguese"
 #~ msgid "Portuguese (Brazil"
 #~ msgstr "Portugisisk"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/oc/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/oc/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: oc\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2495,19 +2495,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinés"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Chinés"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
 
@@ -3914,18 +3924,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/or/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/or/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2019.
 # Pro Neon <proneon267@gmail.com>, 2019.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2019-08-11 12:03+0000\n"
 "Last-Translator: Pro Neon <proneon267@gmail.com>\n"
 "Language-Team: Odia <https://hosted.weblate.org/projects/weblate/languages/"
 "or/>\n"
 "Language: or\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2532,19 +2532,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Min Nan"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "ଚାଇନୀଜ, ମିନ ନାନ"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Min Nan"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "ଚାଇନୀଜ, ମିନ ନାନ"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "ନୀପୋଲିଟାନ୍"
 
@@ -3980,18 +3990,24 @@
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Yucateco"
 msgstr "ଆଗୁଆକାଟେକୋ"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "ଜୁଆଙ୍ଗ"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/pa/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/pa/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Aman ALam <alam.yellow@gmail.com>, 2019, 2020.
 # bgo-eiu <huyaqoob+toolforge@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-11-02 08:51+0000\n"
 "Last-Translator: bgo-eiu <huyaqoob+toolforge@gmail.com>\n"
 "Language-Team: Punjabi <https://hosted.weblate.org/projects/weblate/"
 "languages/pa/>\n"
 "Language: pa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2557,19 +2557,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "ਚੀਨੀ (ਰਿਵਾਇਤੀ)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Min Nan"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "ਚੀਨੀ, ਮਿਨ ਨਾਨ"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "ਨਿਆਪੋਲੀਟਨ"
 
@@ -4015,18 +4025,24 @@
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Yucateco"
 msgstr "ਅਗੂਆਕਾਟੇਕੋ"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "ਜ਼ਹੂਆਂਗ"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/pa_PK/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # bgo-eiu <huyaqoob+toolforge@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-10-29 21:05+0000\n"
 "Last-Translator: bgo-eiu <huyaqoob+toolforge@gmail.com>\n"
 "Language-Team: Punjabi (Pakistan) <https://hosted.weblate.org/projects/"
 "weblate/languages/pa_PK/>\n"
 "Language: pa_PK\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2435,18 +2435,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3819,18 +3825,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/peo/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/peo/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: peo\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2424,18 +2424,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3804,18 +3810,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/pl/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/pl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Stanisław Stefan Krukowski <pet209a1@riseup.net>, 2020.
 # Damian Tokarski <damianwolennicy@gmail.com>, 2021.
 # Agnieszka C <aga_04@o2.pl>, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-01-31 01:49+0000\n"
 "Last-Translator: Agnieszka C <aga_04@o2.pl>\n"
 "Language-Team: Polish <https://hosted.weblate.org/projects/weblate/languages/"
 "pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2435,18 +2435,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "chiński (tradycyjny)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "chiński (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "neapolitański"
@@ -3815,19 +3825,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "maya"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "yue (uproszczony)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "yue"
+msgid "Yue (Traditional)"
+msgstr "yue (tradycyjny)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ps/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ps/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ps\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2509,19 +2509,27 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "چیني"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Chinese (Min Nan, Latin)"
+msgstr "چیني"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "نيپالين"
 
@@ -3946,18 +3954,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/pt/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/pt/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 # Pedro Albuquerque <pmra@gmx.com>, 2019.
 # Manuela Silva <mmsrs@sky.com>, 2019, 2020.
 # rummsi <rummsi@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2023-02-05 17:22+0000\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2023-03-13 13:15+0000\n"
 "Last-Translator: ssantos <ssantos@web.de>\n"
 "Language-Team: Portuguese <https://hosted.weblate.org/projects/weblate/"
 "languages/pt/>\n"
 "Language: pt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -2429,18 +2429,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinês (Tradicional)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Chinês (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitano"
@@ -3128,17 +3138,16 @@
 #. or other variant.
 msgid "Slovak"
 msgstr "Eslovaco"
 
 #. Translators: Language name for ISO code "skr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
 msgid "Saraiki"
-msgstr "waray"
+msgstr "Seraiki"
 
 #. Translators: Language name for ISO code "sl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Slovenian"
 msgstr "Esloveno"
 
@@ -3810,19 +3819,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Iucateque"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (Simplificado)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (Tradicional)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Fred Maranhão <fred.maranhao@gmail.com>, 2021.
 # Claudio Filho F Filho <filhocf@gmail.com>, 2022.
 # Luckumi <lipezinhofilipe@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-01-31 01:49+0000\n"
 "Last-Translator: Rafael Fontenelle <rafaelff@gnome.org>\n"
 "Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
 "weblate/languages/pt_BR/>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2433,18 +2433,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Náuatle"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinês (tradicional)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Chinês (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitano"
@@ -3813,19 +3823,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Lucateque"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Cantonês (simplificado)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Cantonês"
+msgid "Yue (Traditional)"
+msgstr "Cantonês (tradicional)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Weblate <noreply@weblate.org>, 2020.
 # ssantos <ssantos@web.de>, 2020, 2021, 2022, 2023.
 # Dinis Medeiros <dinismedeiros@gmail.com>, 2021.
+# Hugo Carvalho <hugokarvalho@hotmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2023-02-05 17:22+0000\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2023-03-13 13:15+0000\n"
 "Last-Translator: ssantos <ssantos@web.de>\n"
 "Language-Team: Portuguese (Portugal) <https://hosted.weblate.org/projects/"
 "weblate/languages/pt_PT/>\n"
 "Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Afar"
 
@@ -2428,18 +2429,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chinês (Tradicional)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Chinês (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitano"
@@ -3127,18 +3138,16 @@
 #. or other variant.
 msgid "Slovak"
 msgstr "Eslovaco"
 
 #. Translators: Language name for ISO code "skr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-#, fuzzy
-#| msgid "Darai"
 msgid "Saraiki"
-msgstr "Darai"
+msgstr "Seraiki"
 
 #. Translators: Language name for ISO code "sl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Slovenian"
 msgstr "Esloveno"
 
@@ -3810,19 +3819,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Iucateque"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (Simplificado)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (Tradicional)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ro/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ro/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Christian Eichert <c@zp1.net>, 2021.
 # Licaon Kter <licaon.kter@protonmail.com>, 2021, 2022.
 # Simona Iacob <s@zp1.net>, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-10 20:35+0000\n"
 "Last-Translator: Simona Iacob <s@zp1.net>\n"
 "Language-Team: Romanian <https://hosted.weblate.org/projects/weblate/"
 "languages/ro/>\n"
 "Language: ro\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2440,18 +2440,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Chineză (tradițională)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Chineză (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "napolitană"
@@ -3848,19 +3858,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (simplificată)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (tradițională)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ro_MD/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: ro_MD\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2424,18 +2424,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3712,15 +3718,15 @@
 msgid "German (Walser)"
 msgstr ""
 
 #. Translators: Language name for ISO code "wal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wolaytta"
-msgstr ""
+msgstr "wolaytta"
 
 #. Translators: Language name for ISO code "war". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Waray (Philippines)"
 msgstr ""
 
@@ -3804,18 +3810,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ru/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 # Viktor <xasertop@gmail.com>, 2022.
 # Vin <k3kelm4vw@mozmail.com>, 2022, 2023.
 # S3aBreeze <S3aBreeze@users.noreply.hosted.weblate.org>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: S3aBreeze <S3aBreeze@users.noreply.hosted.weblate.org>\n"
 "Language-Team: Russian <https://hosted.weblate.org/projects/weblate/"
 "languages/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
+"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "X-Generator: Weblate 4.16-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "Афарский"
@@ -2444,18 +2444,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Науатль"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Китайский (традиционный)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Китайский (миньнань)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Неаполитанский"
@@ -3824,19 +3834,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Юкатека"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Кантонский (упрощённый)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Юэ (кантонский)"
+msgid "Yue (Traditional)"
+msgstr "Кантонский (традиционный)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Чжуанский"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/sc/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/sc/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Ajeje Brazorf <lmelonimamo@yahoo.it>, 2018, 2019, 2020, 2021, 2022, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: Ajeje Brazorf <lmelonimamo@yahoo.it>\n"
 "Language-Team: Sardinian <https://hosted.weblate.org/projects/weblate/"
 "languages/sc/>\n"
 "Language: sc\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2426,18 +2426,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Tzinesu (Traditzionale)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Tzinesu (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napoletanu"
@@ -3806,19 +3816,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Yucateco"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (Semplificadu)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (Traditzionale)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/si/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/si/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # HelaBasa <R45XvezA@protonmail.ch>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-03-06 07:50+0000\n"
 "Last-Translator: HelaBasa <R45XvezA@protonmail.ch>\n"
 "Language-Team: Sinhala <https://hosted.weblate.org/projects/weblate/"
 "languages/si/>\n"
 "Language: si\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2444,19 +2444,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "චීන, මැන්ඩරීන්"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "චීන, මැන්ඩරීන්"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "නියාපොලිටන්"
 
@@ -3844,18 +3854,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/sk/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/sk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Ivan Pleva <ivan.pleva@tutanota.com>, 2020.
 # Marek freezy Víger <marek.viger@gmail.com>, 2020.
 # Milan <mobrcian@hotmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Slovak <https://hosted.weblate.org/projects/weblate/languages/"
 "sk/>\n"
 "Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2567,18 +2567,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Aztéčina (Nahuatl)"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Čínština (tradičná)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Čínština (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Neapolština"
@@ -4039,19 +4049,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (zlednodušená)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (tradičná)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "čuangčina"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/skr/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/skr/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
 # پرویز قادر <mpqadir@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2023-02-26 16:37+0000\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2023-03-01 14:17+0000\n"
 "Last-Translator: پرویز قادر <mpqadir@gmail.com>\n"
 "Language-Team: Saraiki <https://hosted.weblate.org/projects/weblate/"
 "languages/skr/>\n"
 "Language: skr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 4.16-rc\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "افار"
 
@@ -2220,51 +2220,51 @@
 msgid "Mandar"
 msgstr "منڈار"
 
 #. Translators: Language name for ISO code "men". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mende (Sierra Leone)"
-msgstr ""
+msgstr "مینڈے (سیرا لیون)"
 
 #. Translators: Language name for ISO code "mfe". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Morisyen"
-msgstr ""
+msgstr "موریسئن"
 
 #. Translators: Language name for ISO code "mg". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Malagasy"
 msgstr "مالاگاسی"
 
 #. Translators: Language name for ISO code "mga". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Irish (Middle)"
-msgstr ""
+msgstr "آئرش (مڈل)"
 
 #. Translators: Language name for ISO code "mgo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Metaʼ"
 msgstr "میٹا'"
 
 #. Translators: Language name for ISO code "mh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Marshallese"
-msgstr ""
+msgstr "مارشلیس"
 
 #. Translators: Language name for ISO code "mhr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Meadow Mari"
-msgstr ""
+msgstr "میڈوو مری"
 
 #. Translators: Language name for ISO code "mi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Maori"
 msgstr "مَوری"
 
@@ -2274,21 +2274,21 @@
 msgid "Miami"
 msgstr "میامی"
 
 #. Translators: Language name for ISO code "mic". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mi'kmaq"
-msgstr ""
+msgstr "میکماق"
 
 #. Translators: Language name for ISO code "min". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Minangkabau"
-msgstr ""
+msgstr "منانگکابا"
 
 #. Translators: Language name for ISO code "mjw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Karbi"
 msgstr "کربی"
 
@@ -2328,15 +2328,15 @@
 msgid "Mandinka"
 msgstr "منڈنکا"
 
 #. Translators: Language name for ISO code "mnw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mon"
-msgstr "سون٘و"
+msgstr "مون"
 
 #. Translators: Language name for ISO code "moe". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Innu"
 msgstr "اِنّو"
 
@@ -2426,25 +2426,35 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "ناہوٹی"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "چینی (روایتی)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "چینی (من نان)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
-msgstr ""
+msgstr "نیپولیٹں"
 
 #. Translators: Language name for ISO code "naq". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nama"
 msgstr "ناما"
 
@@ -2490,15 +2500,15 @@
 msgid "Nias"
 msgstr "نیاس"
 
 #. Translators: Language name for ISO code "niu". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Niuean"
-msgstr ""
+msgstr "نیوئن"
 
 #. Translators: Language name for ISO code "nl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Dutch"
 msgstr "ڈچ"
 
@@ -2526,15 +2536,15 @@
 msgid "Norwegian Nynorsk"
 msgstr "ناروی نورسک"
 
 #. Translators: Language name for ISO code "nnh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ngiemboon"
-msgstr ""
+msgstr "نیگم بُون"
 
 #. Translators: Language name for ISO code "nog". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nogai"
 msgstr "نوگائی"
 
@@ -2562,69 +2572,69 @@
 msgid "Pedi"
 msgstr "پیڈی"
 
 #. Translators: Language name for ISO code "nuk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nuu-chah-nulth"
-msgstr ""
+msgstr "نوچاہ نُلتھ"
 
 #. Translators: Language name for ISO code "nv". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Navaho"
-msgstr ""
+msgstr "نواہو"
 
 #. Translators: Language name for ISO code "nwc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Newari (Classical)"
 msgstr "نیواری (کلاسیکل)"
 
 #. Translators: Language name for ISO code "ny". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nyanja"
-msgstr ""
+msgstr "نینجا"
 
 #. Translators: Language name for ISO code "nym". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nyamwezi"
-msgstr ""
+msgstr "نیامویزی"
 
 #. Translators: Language name for ISO code "nyn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nyankole"
-msgstr ""
+msgstr "نیان کول"
 
 #. Translators: Language name for ISO code "nyo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nyoro"
 msgstr "نائیورو"
 
 #. Translators: Language name for ISO code "nzi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nzima"
-msgstr ""
+msgstr "نزیما"
 
 #. Translators: Language name for ISO code "oc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Occitan"
-msgstr ""
+msgstr "اوکسیٹن"
 
 #. Translators: Language name for ISO code "oj". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ojibwe"
-msgstr ""
+msgstr "اوجیبوی"
 
 #. Translators: Language name for ISO code "om". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Oromo"
 msgstr "ارومو"
 
@@ -2658,15 +2668,15 @@
 msgid "Kokturk"
 msgstr "کوکترک"
 
 #. Translators: Language name for ISO code "ovd". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Elfdalian"
-msgstr ""
+msgstr "ایلفڈالی"
 
 #. Translators: Language name for ISO code "pa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Punjabi"
 msgstr "پنجابی"
 
@@ -2688,21 +2698,21 @@
 msgid "Pahlavi"
 msgstr "پہلوی"
 
 #. Translators: Language name for ISO code "pam". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Pampanga"
-msgstr ""
+msgstr "پام پنگا"
 
 #. Translators: Language name for ISO code "pap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Papiamento"
-msgstr ""
+msgstr "پاپیامنٹو"
 
 #. Translators: Language name for ISO code "pau". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Palauan"
 msgstr "پالوان"
 
@@ -2748,33 +2758,33 @@
 msgid "Polish (informal)"
 msgstr "پولسی (غیر رسمی)"
 
 #. Translators: Language name for ISO code "pms". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Piemontese"
-msgstr ""
+msgstr "پیمونٹی"
 
 #. Translators: Language name for ISO code "pon". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Pohnpeian"
-msgstr ""
+msgstr "پون پئین"
 
 #. Translators: Language name for ISO code "prg". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Prussian"
 msgstr "پروسی"
 
 #. Translators: Language name for ISO code "pro". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Provençal (Old)"
-msgstr ""
+msgstr "پرووینسل (قدیمی)"
 
 #. Translators: Language name for ISO code "ps". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Pashto"
 msgstr "پشتو"
 
@@ -2826,69 +2836,69 @@
 msgid "Portuguese (Portugal)"
 msgstr "پرتگیزی (پرتگال)"
 
 #. Translators: Language name for ISO code "qdt". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Eskimo (Pacific Coast Alaskan)"
-msgstr ""
+msgstr "ایسکیمو (کاہل ساحلی الاسکی)"
 
 #. Translators: Language name for ISO code "qtp". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Gayón"
-msgstr ""
+msgstr "گائیون"
 
 #. Translators: Language name for ISO code "qu". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Quechua"
-msgstr ""
+msgstr "کیچوا"
 
 #. Translators: Language name for ISO code "qu_EC". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Quechua (Ecuador)"
-msgstr ""
+msgstr "کیچوا (ایکواڈور)"
 
 #. Translators: Language name for ISO code "quc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "K'iche'"
-msgstr ""
+msgstr "کیچی"
 
 #. Translators: Language name for ISO code "qya". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Quenya"
-msgstr ""
+msgstr "کینیا"
 
 #. Translators: Language name for ISO code "raj". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Rajasthani"
 msgstr "راجھستانی"
 
 #. Translators: Language name for ISO code "rap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Rapanui"
-msgstr ""
+msgstr "رپنوئی"
 
 #. Translators: Language name for ISO code "rar". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Rarotongan"
-msgstr ""
+msgstr "راروٹونگن"
 
 #. Translators: Language name for ISO code "rcf". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Réunion Creole"
-msgstr ""
+msgstr "ری یونین کریول"
 
 #. Translators: Language name for ISO code "rm". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Romansh"
 msgstr "رومانش"
 
@@ -2946,27 +2956,27 @@
 msgid "Russian (Ukraine)"
 msgstr "روسی (یوکرائن)"
 
 #. Translators: Language name for ISO code "rue". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Rusyn"
-msgstr ""
+msgstr "رسائن"
 
 #. Translators: Language name for ISO code "rup". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Macedo-Romanian"
-msgstr ""
+msgstr "میکیڈو رومانی"
 
 #. Translators: Language name for ISO code "rw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kinyarwanda"
-msgstr ""
+msgstr "کینیاروانڈا"
 
 #. Translators: Language name for ISO code "rwk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Rwa"
 msgstr "روا"
 
@@ -2988,21 +2998,21 @@
 msgid "Yakut"
 msgstr "یاکوت"
 
 #. Translators: Language name for ISO code "sai". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "South American Indian (Other)"
-msgstr ""
+msgstr "جنوبی امریکی ہندی (ٻئی)"
 
 #. Translators: Language name for ISO code "sam". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Samaritan Aramaic"
-msgstr ""
+msgstr "سماریٹن آرامائیک"
 
 #. Translators: Language name for ISO code "saq". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Samburu"
 msgstr "سمبرو"
 
@@ -3024,15 +3034,15 @@
 msgid "Sardinian"
 msgstr "سردینی"
 
 #. Translators: Language name for ISO code "scn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sicilian"
-msgstr ""
+msgstr "سسیلی"
 
 #. Translators: Language name for ISO code "sco". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Scots"
 msgstr "سکاٹش"
 
@@ -3060,93 +3070,93 @@
 msgid "Sena"
 msgstr "سینا"
 
 #. Translators: Language name for ISO code "sel". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Selkup"
-msgstr ""
+msgstr "سلک اپ"
 
 #. Translators: Language name for ISO code "ses". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Koyraboro Senni"
-msgstr ""
+msgstr "کوئرابورو سینی"
 
 #. Translators: Language name for ISO code "sg". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sango"
 msgstr "سانگو"
 
 #. Translators: Language name for ISO code "sga". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Irish (Old)"
-msgstr ""
+msgstr "آئرش (قدیم))"
 
 #. Translators: Language name for ISO code "sgn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sign Languages"
-msgstr ""
+msgstr "اشاراتی زباناں"
 
 #. Translators: Language name for ISO code "shi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tachelhit"
-msgstr ""
+msgstr "ٹاچل ہِٹ"
 
 #. Translators: Language name for ISO code "shn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Shan"
-msgstr ""
+msgstr "شان"
 
 #. Translators: Language name for ISO code "si". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sinhala"
 msgstr "سنہالا"
 
 #. Translators: Language name for ISO code "sid". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sidamo"
-msgstr ""
+msgstr "سدامو"
 
 #. Translators: Language name for ISO code "sjd". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sami (Kildin)"
-msgstr ""
+msgstr "سامی (کلڈن)"
 
 #. Translators: Language name for ISO code "sk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Slovak"
-msgstr ""
+msgstr "سلواک"
 
 #. Translators: Language name for ISO code "skr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Saraiki"
 msgstr "سرائیکی"
 
 #. Translators: Language name for ISO code "sl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Slovenian"
-msgstr ""
+msgstr "سلوینی"
 
 #. Translators: Language name for ISO code "sm". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Samoan"
-msgstr ""
+msgstr "سمائون"
 
 #. Translators: Language name for ISO code "sma". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sami (Southern)"
 msgstr "سامی (جنوبی)"
 
@@ -3156,63 +3166,63 @@
 msgid "Sami"
 msgstr "سامی"
 
 #. Translators: Language name for ISO code "smj". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sami (Lule)"
-msgstr ""
+msgstr "سامی (لول)"
 
 #. Translators: Language name for ISO code "sml". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sama (Central)"
-msgstr ""
+msgstr "ساما (مرکزی)"
 
 #. Translators: Language name for ISO code "smn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sami (Inari)"
-msgstr ""
+msgstr "سامی (اِناری)"
 
 #. Translators: Language name for ISO code "sms". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sami (Skolt)"
-msgstr ""
+msgstr "سامی (سکلوٹ)"
 
 #. Translators: Language name for ISO code "sn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Shona"
 msgstr "شونا"
 
 #. Translators: Language name for ISO code "snk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Soninke"
-msgstr ""
+msgstr "سوننکی"
 
 #. Translators: Language name for ISO code "so". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Somali"
 msgstr "صومالی"
 
 #. Translators: Language name for ISO code "sog". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sogdian"
-msgstr ""
+msgstr "سوگڈیان"
 
 #. Translators: Language name for ISO code "son". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Songhai"
-msgstr ""
+msgstr "سونغائی"
 
 #. Translators: Language name for ISO code "sq". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Albanian"
 msgstr "البانی"
 
@@ -3222,674 +3232,680 @@
 msgid "Serbian"
 msgstr "سربی"
 
 #. Translators: Language name for ISO code "sr@ijekavian". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Serbian (Ijekavian)"
-msgstr ""
+msgstr "سربی (ایجیکاوی)"
 
 #. Translators: Language name for ISO code "sr@ijekavian_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Serbian (Ijekavian, latin)"
-msgstr ""
+msgstr "سربی (ایجیکاوی، لاطینی)"
 
 #. Translators: Language name for ISO code "sr_Cyrl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Serbian (cyrillic)"
-msgstr ""
+msgstr "سربی (سیریلیک)"
 
 #. Translators: Language name for ISO code "sr_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Serbian (latin)"
 msgstr "سربی (لاطینی)"
 
 #. Translators: Language name for ISO code "srn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sranan Tongo"
-msgstr ""
+msgstr "سرانن ٹونگو"
 
 #. Translators: Language name for ISO code "srr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Serer"
-msgstr ""
+msgstr "سیریر"
 
 #. Translators: Language name for ISO code "ss". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Swati"
-msgstr ""
+msgstr "سواٹی"
 
 #. Translators: Language name for ISO code "ssy". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Saho"
-msgstr ""
+msgstr "ساہو"
 
 #. Translators: Language name for ISO code "st". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sotho (Southern)"
-msgstr ""
+msgstr "سوٹھو (جنوبی)"
 
 #. Translators: Language name for ISO code "su". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sundanese"
-msgstr ""
+msgstr "سنڈانی"
 
 #. Translators: Language name for ISO code "suk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sukuma"
-msgstr ""
+msgstr "سکوما"
 
 #. Translators: Language name for ISO code "sus". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Susu"
-msgstr ""
+msgstr "سوسو"
 
 #. Translators: Language name for ISO code "sux". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sumerian"
-msgstr ""
+msgstr "سمیری"
 
 #. Translators: Language name for ISO code "sv". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Swedish"
-msgstr ""
+msgstr "سویڈش"
 
 #. Translators: Language name for ISO code "sw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Swahili"
-msgstr ""
+msgstr "سواحلی"
 
 #. Translators: Language name for ISO code "sw_CD". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Swahili (Congo)"
-msgstr ""
+msgstr "سواحلی (کانگو)"
 
 #. Translators: Language name for ISO code "sw_TZ". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Swahili (Tanzania)"
-msgstr ""
+msgstr "سواحلی (تنزانیہ)"
 
 #. Translators: Language name for ISO code "swg". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Swabian"
-msgstr ""
+msgstr "سوابی"
 
 #. Translators: Language name for ISO code "sxu". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Saxon (Upper)"
-msgstr ""
+msgstr "سیکسون (اُتلی)"
 
 #. Translators: Language name for ISO code "syc". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Syriac (Classical)"
-msgstr ""
+msgstr "سائریاک (کلاسیکل)"
 
 #. Translators: Language name for ISO code "syr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Syriac"
-msgstr ""
+msgstr "سائریاک"
 
 #. Translators: Language name for ISO code "szl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Silesian"
-msgstr ""
+msgstr "سیلسی"
 
 #. Translators: Language name for ISO code "ta". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tamil"
-msgstr ""
+msgstr "تامل"
 
 #. Translators: Language name for ISO code "ta_LK". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tamil (Sri Lanka)"
-msgstr ""
+msgstr "تامل (سری لنکا)"
 
 #. Translators: Language name for ISO code "te". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Telugu"
-msgstr ""
+msgstr "تیلگو"
 
 #. Translators: Language name for ISO code "tem". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Timne"
-msgstr ""
+msgstr "ٹیمنے"
 
 #. Translators: Language name for ISO code "teo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Teso"
-msgstr ""
+msgstr "تیسو"
 
 #. Translators: Language name for ISO code "ter". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tereno"
-msgstr ""
+msgstr "ٹیرینو"
 
 #. Translators: Language name for ISO code "tet". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tetum"
-msgstr ""
+msgstr "ٹیٹم"
 
 #. Translators: Language name for ISO code "tg". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tajik"
-msgstr ""
+msgstr "تاجک"
 
 #. Translators: Language name for ISO code "th". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Thai"
-msgstr ""
+msgstr "تھائی"
 
 #. Translators: Language name for ISO code "ti". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tigrinya"
-msgstr ""
+msgstr "ٹِگرینا"
 
 #. Translators: Language name for ISO code "tig". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tigre"
-msgstr ""
+msgstr "ٹیگر"
 
 #. Translators: Language name for ISO code "tiv". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tiv"
-msgstr ""
+msgstr "ٹیوی"
 
 #. Translators: Language name for ISO code "tk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Turkmen"
-msgstr ""
+msgstr "ترکمن"
 
 #. Translators: Language name for ISO code "tkl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tokelau"
-msgstr ""
+msgstr "ٹوکے لاؤ"
 
 #. Translators: Language name for ISO code "tl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tagalog"
-msgstr ""
+msgstr "ٹیگا لاگ"
 
 #. Translators: Language name for ISO code "tlh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Klingon"
-msgstr ""
+msgstr "کلینگون"
 
 #. Translators: Language name for ISO code "tlh-qaak". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Klingon (pIqaD)"
-msgstr ""
+msgstr "کلنگون (پلکاڈ)"
 
 #. Translators: Language name for ISO code "tli". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tlingit"
-msgstr ""
+msgstr "ٹلنگِٹ"
 
 #. Translators: Language name for ISO code "tmh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tamashek"
-msgstr ""
+msgstr "ٹاماشک"
 
 #. Translators: Language name for ISO code "tn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tswana"
-msgstr ""
+msgstr "ٹسوانا"
 
 #. Translators: Language name for ISO code "to". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tongan"
-msgstr ""
+msgstr "ٹونگن"
 
 #. Translators: Language name for ISO code "tog". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tonga (Nyasa)"
-msgstr ""
+msgstr "ٹونگا (نیاسا)"
 
 #. Translators: Language name for ISO code "tok". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Toki Pona"
-msgstr ""
+msgstr "ٹوکی پونا"
 
 #. Translators: Language name for ISO code "tpi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tok Pisin"
-msgstr ""
+msgstr "ٹوک پیسن"
 
 #. Translators: Language name for ISO code "tr". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Turkish"
-msgstr ""
+msgstr "ترکی"
 
 #. Translators: Language name for ISO code "trv". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Taroko"
-msgstr ""
+msgstr "ٹروکو"
 
 #. Translators: Language name for ISO code "ts". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tsonga"
-msgstr ""
+msgstr "سونگا"
 
 #. Translators: Language name for ISO code "tsi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tsimshian"
-msgstr ""
+msgstr "ٹسمیشی"
 
 #. Translators: Language name for ISO code "tsj". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tshangla"
-msgstr ""
+msgstr "تشانگلا"
 
 #. Translators: Language name for ISO code "tt". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tatar"
-msgstr ""
+msgstr "تاتار"
 
 #. Translators: Language name for ISO code "tt@iqtelif". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tatar (IQTElif)"
-msgstr ""
+msgstr "تاتار (ایکٹیلیف)"
 
 #. Translators: Language name for ISO code "tum". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tumbuka"
-msgstr ""
+msgstr "ٹم بوکا"
 
 #. Translators: Language name for ISO code "tvl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tuvalu"
-msgstr ""
+msgstr "توالو"
 
 #. Translators: Language name for ISO code "tw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Twi"
-msgstr ""
+msgstr "ٹوی"
 
 #. Translators: Language name for ISO code "ty". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tahitian"
-msgstr ""
+msgstr "ٹاہیٹی"
 
 #. Translators: Language name for ISO code "tyv". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tuvinian"
-msgstr ""
+msgstr "توینی"
 
 #. Translators: Language name for ISO code "tzj". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tz'utujil"
-msgstr ""
+msgstr "ٹزوٹوجیل"
 
 #. Translators: Language name for ISO code "tzl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Talossan"
-msgstr ""
+msgstr "ٹالوسان"
 
 #. Translators: Language name for ISO code "tzm". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tamazight (Central Atlas)"
-msgstr ""
+msgstr "ٹمازیگھٹ (مرکزی اٹلس)"
 
 #. Translators: Language name for ISO code "udm". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Udmurt"
-msgstr ""
+msgstr "اُڈمورت"
 
 #. Translators: Language name for ISO code "ug". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Uyghur"
-msgstr ""
+msgstr "یغور"
 
 #. Translators: Language name for ISO code "uga". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ugaritic"
-msgstr ""
+msgstr "یوگراٹک"
 
 #. Translators: Language name for ISO code "uk". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Ukrainian"
-msgstr ""
+msgstr "یوکرائن"
 
 #. Translators: Language name for ISO code "umb". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Umbundu"
-msgstr ""
+msgstr "امبنڈُو"
 
 #. Translators: Language name for ISO code "und". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Undetermined"
-msgstr ""
+msgstr "غیرمتعین"
 
 #. Translators: Language name for ISO code "ur". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Urdu"
-msgstr ""
+msgstr "اردو"
 
 #. Translators: Language name for ISO code "ur_IN". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Urdu (India)"
-msgstr ""
+msgstr "اردو (بھارت)"
 
 #. Translators: Language name for ISO code "ur_PK". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Urdu (Pakistan)"
-msgstr ""
+msgstr "اردو (پاکستان)"
 
 #. Translators: Language name for ISO code "uz". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Uzbek"
-msgstr ""
+msgstr "ازبک"
 
 #. Translators: Language name for ISO code "uz_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Uzbek (latin)"
-msgstr ""
+msgstr "ازبک (لاطینی)"
 
 #. Translators: Language name for ISO code "vai". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Vai"
-msgstr ""
+msgstr "وائی"
 
 #. Translators: Language name for ISO code "ve". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Venda"
-msgstr ""
+msgstr "وینڈا"
 
 #. Translators: Language name for ISO code "vec". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Venetian"
-msgstr ""
+msgstr "وینیشی"
 
 #. Translators: Language name for ISO code "vi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Vietnamese"
-msgstr ""
+msgstr "ویت نامی"
 
 #. Translators: Language name for ISO code "vls". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Flemish (West)"
-msgstr ""
+msgstr "فلیمش (مغربی)"
 
 #. Translators: Language name for ISO code "vo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Volapük"
-msgstr ""
+msgstr "وولاپوک"
 
 #. Translators: Language name for ISO code "vot". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Votic"
-msgstr ""
+msgstr "ووٹک"
 
 #. Translators: Language name for ISO code "vun". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Vunjo"
-msgstr ""
+msgstr "وُنجو"
 
 #. Translators: Language name for ISO code "wa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Walloon"
-msgstr ""
+msgstr "والُون"
 
 #. Translators: Language name for ISO code "wae". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "German (Walser)"
-msgstr ""
+msgstr "جرمن (والسر)"
 
 #. Translators: Language name for ISO code "wal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wolaytta"
-msgstr ""
+msgstr "وولیٹا"
 
 #. Translators: Language name for ISO code "war". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Waray (Philippines)"
-msgstr ""
+msgstr "وریا (فلپینی)"
 
 #. Translators: Language name for ISO code "was". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Washo"
-msgstr ""
+msgstr "واشو"
 
 #. Translators: Language name for ISO code "wen". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Sorbian"
-msgstr ""
+msgstr "سوربی"
 
 #. Translators: Language name for ISO code "wep". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Westphalien"
-msgstr ""
+msgstr "ویسٹ فالین"
 
 #. Translators: Language name for ISO code "wuu_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Simplified)"
-msgstr ""
+msgstr "وو (سادہ)"
 
 #. Translators: Language name for ISO code "wuu_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wu (Traditional)"
-msgstr ""
+msgstr "وو (رواٰیتی)"
 
 #. Translators: Language name for ISO code "wo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Wolof"
-msgstr ""
+msgstr "وولوف"
 
 #. Translators: Language name for ISO code "xal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Kalmyk"
-msgstr ""
+msgstr "کلمیاک"
 
 #. Translators: Language name for ISO code "xh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Xhosa"
-msgstr ""
+msgstr "ہوسا"
 
 #. Translators: Language name for ISO code "xog". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Soga"
-msgstr ""
+msgstr "سوگا"
 
 #. Translators: Language name for ISO code "yao". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yao"
-msgstr ""
+msgstr "یاؤ"
 
 #. Translators: Language name for ISO code "yap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yapese"
-msgstr ""
+msgstr "یاپیسے"
 
 #. Translators: Language name for ISO code "yi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yiddish"
-msgstr ""
+msgstr "یِدیش"
 
 #. Translators: Language name for ISO code "yo". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yoruba"
-msgstr ""
+msgstr "یوربا"
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
-msgstr ""
+msgstr "یوکاٹیکو"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr ""
+msgid "Yue (Simplified)"
+msgstr "یوئے (سادہ)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Traditional)"
+msgstr "یوئے (روایتی)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
-msgstr ""
+msgstr "یوانگ"
 
 #. Translators: Language name for ISO code "zap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zapotec"
-msgstr ""
+msgstr "زاپوٹک"
 
 #. Translators: Language name for ISO code "zbl". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Blissymbols"
-msgstr ""
+msgstr "بلس سمبلز"
 
 #. Translators: Language name for ISO code "zen". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zenaga"
-msgstr ""
+msgstr "زیناگا"
 
 #. Translators: Language name for ISO code "zgh". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tamazight (Standard Moroccan)"
-msgstr ""
+msgstr "ٹمازیگھاٹ (معیاری موراکی)"
 
 #. Translators: Language name for ISO code "zh_Hans". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chinese (Simplified)"
-msgstr ""
+msgstr "چینی (سادہ)"
 
 #. Translators: Language name for ISO code "zh_Hans_SG". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chinese (Simplified, Singapore)"
-msgstr ""
+msgstr "چینی (سادہ، سنگاپور)"
 
 #. Translators: Language name for ISO code "zh_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chinese (Traditional)"
-msgstr ""
+msgstr "چینی (روایتی)"
 
 #. Translators: Language name for ISO code "zh_Hant_HK". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chinese (Traditional, Hong Kong)"
-msgstr ""
+msgstr "چینی (روایتی، ہانگ کانگ)"
 
 #. Translators: Language name for ISO code "zh_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Chinese (Pinyin)"
-msgstr ""
+msgstr "چینی (پنین)"
 
 #. Translators: Language name for ISO code "zu". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zulu"
-msgstr ""
+msgstr "زولو"
 
 #. Translators: Language name for ISO code "zun". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zuni"
-msgstr ""
+msgstr "زونی"
 
 #. Translators: Language name for ISO code "zza". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zaza"
-msgstr ""
+msgstr "زازا"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/sl/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/sl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Štefan Baebler <stefan.baebler@gmail.com>, 2020.
 # Domen <mitenem@outlook.com>, 2020.
 # Martin Srebotnjak <miles@filmsi.net>, 2020, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Slovenian <https://hosted.weblate.org/projects/weblate/"
 "languages/sl/>\n"
 "Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2522,18 +2522,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "kitajščina (tradicionalno)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "kitajščina (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "napolitanščina"
@@ -3970,19 +3980,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "kantonščina (poenostavljeno)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "kantonščina"
+msgid "Yue (Traditional)"
+msgstr "kantonščina (tradicionalno)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Zhuang"
 msgstr "šanščina"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/sq/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/sq/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Automatically generated, 2014.
 #
 # Besnik Bleta <besnik@programeshqip.org>, 2020, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Besnik Bleta <besnik@programeshqip.org>\n"
 "Language-Team: Albanian <https://hosted.weblate.org/projects/weblate/"
 "languages/sq/>\n"
 "Language: sq\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2561,18 +2561,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Kineze (Tradicionale)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Kineze (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Naplitançe"
@@ -4011,18 +4021,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/sr/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/sr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # markomi1 <okram.je.car.4@gmail.com>, 2020.
 # Слободан Симић(Slobodan Simić) <slsimic@gmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Serbian <https://hosted.weblate.org/projects/weblate/"
 "languages/sr/>\n"
 "Language: sr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2471,18 +2471,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "науатл"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "кинески (традиционални)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "кинески (Минан)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "неаполитански"
@@ -3886,19 +3896,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "јуе (поједностављени)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "јуе"
+msgid "Yue (Traditional)"
+msgstr "јуе (традиционални)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "џуаншки"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/sr_Latn/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Weblate <noreply@weblate.org>, 2019.
 # Mihajlo Djordjevic <djordjevic.mihajlo@gmail.com>, 2019.
 # Слободан Симић(Slobodan Simić) <slsimic@gmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Serbian (latin) <https://hosted.weblate.org/projects/weblate/"
 "languages/sr_Latn/>\n"
 "Language: sr_Latn\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2471,18 +2471,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "nauatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "kineski (tradicionalni)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "kineski (Minan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "neapolitanski"
@@ -3885,19 +3895,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "jue (pojednostavljeni)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "jue"
+msgid "Yue (Traditional)"
+msgstr "jue (tradicionalni)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "džuanški"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/sv/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/sv/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Filip Bengtsson <filipbengtsson@live.se>, 2019.
 # Mattias Münster <mattiasmun@gmail.com>, 2019.
 # tygyh <jonis9898@hotmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-11 13:41+0000\n"
 "Last-Translator: Johan Jacobsson <johan.jacobsson@telia.com>\n"
 "Language-Team: Swedish <https://hosted.weblate.org/projects/weblate/"
 "languages/sv/>\n"
 "Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2427,18 +2427,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Kinesiska (traditionell)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Kinesiska (Minnan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolitanska"
@@ -3808,19 +3818,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Yukatek"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue (förenklad)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue"
+msgid "Yue (Traditional)"
+msgstr "Yue (traditionell)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Zhuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/sw/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/sw/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2564,19 +2564,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Kichina sanifu"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Kichina sanifu"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Kinapoli"
 
@@ -4008,18 +4018,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ta/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ta/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Tamil <https://hosted.weblate.org/projects/weblate/languages/"
 "ta/>\n"
 "Language: ta\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2567,19 +2567,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Min Nan"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "சைனீஸ், மின் நன்"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Min Nan"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "சைனீஸ், மின் நன்"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "நியோபோலிடன்"
 
@@ -4021,18 +4031,24 @@
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 #, fuzzy
 msgid "Yucateco"
 msgstr "அகுவகேடிகோ"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "ஜுவாங்"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/te/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/te/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: te\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2444,19 +2444,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "చైనీస్, మాండరిన్"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "చైనీస్, మాండరిన్"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "నియోపొలిటన్"
 
@@ -3846,18 +3856,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "జువాన్"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/th/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/th/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # AefghThreenine <aefgh39622@gmail.com>, 2020, 2021.
 # ทรงพล คำผุย <songpon.ming@gmail.com>, 2022.
 # BANKUU <bankuu@gorutan.net>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-10-12 18:26+0000\n"
 "Last-Translator: BANKUU <bankuu@gorutan.net>\n"
 "Language-Team: Thai <https://hosted.weblate.org/projects/weblate/languages/"
 "th/>\n"
 "Language: th\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2448,18 +2448,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "นาฮัทเทิล"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "จีน (ตัวเต็ม)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "จีน (หมิ่นใต้)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "นาโปลี"
@@ -3856,19 +3866,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "เยว่ (ตัวย่อ)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "เยว่"
+msgid "Yue (Traditional)"
+msgstr "เยว่ (ตัวเต็ม)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "จ้วง"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/tlh/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/tok/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# Christine Long <lilmamachrislong33@gmail.com>, 2022.
+# This file is distributed under the same license as the Weblate Language Data package.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
-"Project-Id-Version: Weblate 4.3\n"
+"Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: 2022-01-26 17:54+0000\n"
-"Last-Translator: Christine Long <lilmamachrislong33@gmail.com>\n"
-"Language-Team: Klingon <https://hosted.weblate.org/projects/weblate/"
-"languages/tlh/>\n"
-"Language: tlh\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: Automatically generated\n"
+"Language-Team: none\n"
+"Language: tok\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.11-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
-msgstr "'ay'"
+msgstr ""
 
 #. Translators: Language name for ISO code "ab". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Abkhazian"
-msgstr "'atlham"
+msgstr ""
 
 #. Translators: Language name for ISO code "ace". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Acehnese"
 msgstr ""
 
@@ -2328,15 +2326,15 @@
 msgid "Mandinka"
 msgstr ""
 
 #. Translators: Language name for ISO code "mnw". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Mon"
-msgstr "jach"
+msgstr ""
 
 #. Translators: Language name for ISO code "moe". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Innu"
 msgstr ""
 
@@ -2426,18 +2424,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -3486,15 +3490,15 @@
 msgid "Tonga (Nyasa)"
 msgstr ""
 
 #. Translators: Language name for ISO code "tok". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Toki Pona"
-msgstr ""
+msgstr "Toki Pona"
 
 #. Translators: Language name for ISO code "tpi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tok Pisin"
 msgstr ""
 
@@ -3806,18 +3810,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/tok/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ie/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the Weblate Language Data package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# OIS <mistresssilvara@hotmail.com>, 2021.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: Automatically generated\n"
-"Language-Team: none\n"
-"Language: tok\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
+"PO-Revision-Date: 2021-03-26 11:37+0000\n"
+"Last-Translator: OIS <mistresssilvara@hotmail.com>\n"
+"Language-Team: Occidental <https://hosted.weblate.org/projects/weblate/"
+"languages/ie/>\n"
+"Language: ie\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 4.5.2\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr ""
 
@@ -1624,15 +1626,15 @@
 msgid "Indonesian"
 msgstr ""
 
 #. Translators: Language name for ISO code "ie". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Occidental"
-msgstr ""
+msgstr "Interlingue"
 
 #. Translators: Language name for ISO code "ig". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Igbo"
 msgstr ""
 
@@ -2424,18 +2426,24 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr ""
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
@@ -2920,33 +2928,37 @@
 msgid "Romany"
 msgstr ""
 
 #. Translators: Language name for ISO code "ru". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian"
-msgstr ""
+msgstr "Russ"
 
 #. Translators: Language name for ISO code "ru@formal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
+#, fuzzy
+#| msgid "Russian (Ukraine)"
 msgid "Russian (formal)"
-msgstr ""
+msgstr "Russ (Ukraina)"
 
 #. Translators: Language name for ISO code "ru@informal". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
+#, fuzzy
+#| msgid "Russian (Ukraine)"
 msgid "Russian (informal)"
-msgstr ""
+msgstr "Russ (Ukraina)"
 
 #. Translators: Language name for ISO code "ru_UA". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Russian (Ukraine)"
-msgstr ""
+msgstr "Russ (Ukraina)"
 
 #. Translators: Language name for ISO code "rue". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Rusyn"
 msgstr ""
 
@@ -3484,15 +3496,15 @@
 msgid "Tonga (Nyasa)"
 msgstr ""
 
 #. Translators: Language name for ISO code "tok". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Toki Pona"
-msgstr "Toki Pona"
+msgstr ""
 
 #. Translators: Language name for ISO code "tpi". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Tok Pisin"
 msgstr ""
 
@@ -3804,18 +3816,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/tr/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/tr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Burak Yavuz <hitowerdigit@hotmail.com>, 2020, 2021, 2022.
 # Oğuz Ersen <oguz@ersen.moe>, 2023.
 # Kaya Zeren <kayazeren@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: Kaya Zeren <kayazeren@gmail.com>\n"
 "Language-Team: Turkish <https://hosted.weblate.org/projects/weblate/"
 "languages/tr/>\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2438,18 +2438,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "Nahuatl"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Çince (Geleneksel)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "Çince (Min Nan)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Napolice"
@@ -3822,19 +3832,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "Yukatekçe"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "Yue Çincesi (Basitleştirilmiş)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "Yue Çincesi"
+msgid "Yue (Traditional)"
+msgstr "Yue Çincesi (Geleneksel)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Çuang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/tt/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/tt/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: tt\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2475,19 +2475,27 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Чинчә"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Чинчә"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
 
@@ -3908,18 +3916,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/tzm/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/tzm/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # Weblate <noreply@weblate.org>, 2020.
 # Hakim Oubouali <hakim.oubouali.skr@gmail.com>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Tamazight (Central Atlas) <https://hosted.weblate.org/"
 "projects/weblate/languages/tzm/>\n"
 "Language: tzm\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2497,19 +2497,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Tacinwit,Mandarin"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Tacinwit,Mandarin"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr ""
 
@@ -3911,18 +3921,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/ug/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/ug/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Abdusalam <1810010207@s.upc.edu.cn>, 2020.
 # Anonymous <noreply@weblate.org>, 2020.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2021-11-14 00:02+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Uyghur <https://hosted.weblate.org/projects/weblate/languages/"
 "ug/>\n"
 "Language: ug\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2561,18 +2561,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "ناخۇاتىلچە"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "خەنزۇچە (ئەنئەنىۋى)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "خەنزۇچە (مىن نەن)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "ناپولىچە"
@@ -4013,19 +4023,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "گۇاڭدۇڭچە (ئاددىيلاشتۇرۇلغان)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "گۇاڭدۇڭچە"
+msgid "Yue (Traditional)"
+msgstr "گۇاڭدۇڭچە (ئەنئەنىۋى)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "جۇاڭچە"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/uk/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 # Ihor Hordiichuk <igor_ck@outlook.com>, 2020, 2021, 2023.
 # Tymofii Lytvynenko <till.svit@gmail.com>, 2023.
 # Skrripy <rozihrash.ya6w7@simplelogin.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-10 20:35+0000\n"
 "Last-Translator: Skrripy <rozihrash.ya6w7@simplelogin.com>\n"
 "Language-Team: Ukrainian <https://hosted.weblate.org/projects/weblate/"
 "languages/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=n==1 ? 3 : n%10==1 && n%100!=11 ? 0 : "
-"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
+"Plural-Forms: nplurals=4; plural=n==1 ? 3 : n%10==1 && n%100!=11 ? 0 : n"
+"%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
 "X-Generator: Weblate 4.16-dev\n"
 
 #. Translators: Language name for ISO code "aa". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Afar"
 msgstr "афарська"
@@ -2435,18 +2435,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "науатль"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "китайська (традиційна)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "китайська (мінь-нан)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "неаполітанська"
@@ -3815,19 +3825,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "юкатеко"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "юе (спрощена)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "юе"
+msgid "Yue (Traditional)"
+msgstr "юе (традиційна)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "чуанг"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/uz/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/uz/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: uz\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2442,19 +2442,29 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "xitoy, mandarin"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese, Mandarin"
+msgid "Chinese (Min Nan, Latin)"
+msgstr "xitoy, mandarin"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "neapolitan"
 
@@ -3842,18 +3852,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr ""
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/vi/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/vi/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Victor Tran <vicr12345@gmail.com>, 2019.
 # bruh <quangtrung02hn16@gmail.com>, 2021.
 # Ngô Quốc Đạt <datlechin@gmail.com>, 2022.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2022-01-23 23:35+0000\n"
 "Last-Translator: Ngô Quốc Đạt <datlechin@gmail.com>\n"
 "Language-Team: Vietnamese <https://hosted.weblate.org/projects/weblate/"
 "languages/vi/>\n"
 "Language: vi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2576,19 +2576,27 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
-msgstr ""
+#, fuzzy
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "Tiếng Trung Hoa"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+msgid "Chinese (Min Nan, Latin)"
+msgstr "Tiếng Trung Hoa"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "Tiếng Napoli"
 
@@ -4055,18 +4063,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "Tiếng Choang"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/yue/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: Automatically generated\n"
 "Language-Team: none\n"
 "Language: yue\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -2428,18 +2428,26 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr ""
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Traditional Chinese"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "繁體中文"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Chinese (Min Nan, Latin)"
 msgstr ""
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "拿波里文"
@@ -3828,18 +3836,24 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr ""
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr ""
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
+msgid "Yue (Traditional)"
 msgstr ""
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "壯文"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/zgh/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/zgh/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the Weblate Language Data package.
 # ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ زهير أمازيغ <zouhirdehbi56@gmail.com>, 2023.
 # ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ ZOUHIR DEHBI <zouhirdehbi56@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate Language Data\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-10 20:35+0000\n"
 "Last-Translator: ⵣⵓⵀⵉⵔ ⴰⵎⴰⵣⵉⵖ ZOUHIR DEHBI <zouhirdehbi56@gmail.com>\n"
 "Language-Team: Tamazight (Standard Moroccan) <https://hosted.weblate.org/"
 "projects/weblate/languages/zgh/>\n"
 "Language: zgh\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2427,18 +2427,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "ⵜⴰⵏⴰⵀⵡⴰⵜⵍⵜ"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "ⵜⴰⵛⵉⵏⵡⵉⵜ (ⵜⴰⵣⴰⵢⴽⵓⵜ)"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "ⵜⴰⵛⵉⵏⵡⵉⵜ (ⵎⵉⵏ ⵏⴰⵏ)"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "ⵜⴰⵏⴰⴱⵓⵍⵉⵜ"
@@ -3807,19 +3817,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "ⵜⴰⵢⵓⴽⴰⵜⵉⴽⵓⵜ"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "ⵜⴰⵢⵓⵜ (ⵜⴰⴼⵔⴰⵔⵜ)"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "ⵜⴰⵢⵓⵜ (ⵜⴰⵛⵉⵏⵡⵉⵜ)"
+msgid "Yue (Traditional)"
+msgstr "ⵜⴰⵢⵓⵜ (ⵜⴰⵣⴰⵢⴽⵓⵜ)"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "ⵜⴰⵣⵀⵓⵏⴳⵜ"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # Eric <hamburger1024@duck.com>, 2022.
 # Eric <hamburger2048@users.noreply.hosted.weblate.org>, 2023.
 # SAIHAZE <saihaze@outlook.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: SAIHAZE <saihaze@outlook.com>\n"
 "Language-Team: Chinese (Simplified) <https://hosted.weblate.org/projects/"
 "weblate/languages/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2448,18 +2448,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "纳瓦特尔语"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "中文（繁体）"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "中文（闽南语）"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "那不勒斯语"
@@ -3828,19 +3838,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "尤卡坦玛雅语"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "粤语（简体）"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "粤语"
+msgid "Yue (Traditional)"
+msgstr "粤语（繁体）"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "壮语"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po` & `weblate-language-data-2023.4/weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # yangyangdaji <1504305527@qq.com>, 2022.
 # Toomore Chiang <toomore0929@gmail.com>, 2022.
 # SAIHAZE <saihaze@outlook.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: Weblate 4.3\n"
 "Report-Msgid-Bugs-To: https://github.com/WeblateOrg/language-data/issues/\n"
-"POT-Creation-Date: 2023-01-30 15:07+0100\n"
+"POT-Creation-Date: 2023-04-18 13:19+0200\n"
 "PO-Revision-Date: 2023-02-01 03:03+0000\n"
 "Last-Translator: Chang-Chia Tseng <pswo10680@gmail.com>\n"
 "Language-Team: Chinese (Traditional) <https://hosted.weblate.org/projects/"
 "weblate/languages/zh_Hant/>\n"
 "Language: zh_Hant\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
@@ -2437,18 +2437,28 @@
 
 #. Translators: Language name for ISO code "nah". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Nahuatl"
 msgstr "納瓦特爾語"
 
-#. Translators: Language name for ISO code "nan". The parenthesis clarifies
+#. Translators: Language name for ISO code "nan_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Chinese (Min Nan)"
+#, fuzzy
+#| msgid "Chinese (Traditional)"
+msgid "Chinese (Min Nan, Traditional)"
+msgstr "漢語（正體字）"
+
+#. Translators: Language name for ISO code "nan_Latn". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+#, fuzzy
+#| msgid "Chinese (Min Nan)"
+msgid "Chinese (Min Nan, Latin)"
 msgstr "閩南語"
 
 #. Translators: Language name for ISO code "nap". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Neapolitan"
 msgstr "那不勒斯語"
@@ -3817,19 +3827,25 @@
 
 #. Translators: Language name for ISO code "yua". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Yucateco"
 msgstr "猶加敦馬雅語"
 
-#. Translators: Language name for ISO code "yue". The parenthesis clarifies
+#. Translators: Language name for ISO code "yue_Hans". The parenthesis clarifies
+#. variant of the language. It could contain a region, age (Old, Middle, ...)
+#. or other variant.
+msgid "Yue (Simplified)"
+msgstr "粵語（簡體字）"
+
+#. Translators: Language name for ISO code "yue_Hant". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
-msgid "Yue"
-msgstr "粵語"
+msgid "Yue (Traditional)"
+msgstr "粵語（正體字）"
 
 #. Translators: Language name for ISO code "za". The parenthesis clarifies
 #. variant of the language. It could contain a region, age (Old, Middle, ...)
 #. or other variant.
 msgid "Zhuang"
 msgstr "壯語"
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/plural_tags.py` & `weblate-language-data-2023.4/weblate_language_data/plural_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © Michal Čihař <michal@weblate.org>
 #
 # SPDX-License-Identifier: MIT
 
-"""Language data definitions.
+"""
+Language data definitions.
 
 This is an automatically generated file, see scripts/generate-language-data
 
 Do not edit, please adjust language definitions in following repository:
 https://github.com/WeblateOrg/language-data
 """
 # pylint: disable=line-too-long,too-many-lines
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/plurals.py` & `weblate-language-data-2023.4/weblate_language_data/plurals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © Michal Čihař <michal@weblate.org>
 #
 # SPDX-License-Identifier: MIT
 
-"""Language data definitions.
+"""
+Language data definitions.
 
 This is an automatically generated file, see scripts/generate-language-data
 
 Do not edit, please adjust language definitions in following repository:
 https://github.com/WeblateOrg/language-data
 """
 # pylint: disable=line-too-long,too-many-lines
```

### Comparing `weblate-language-data-2023.3/weblate_language_data/population.py` & `weblate-language-data-2023.4/weblate_language_data/population.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © Michal Čihař <michal@weblate.org>
 #
 # SPDX-License-Identifier: MIT
 
-"""Language data definitions.
+"""
+Language data definitions.
 
 This is an automatically generated file, see scripts/generate-language-data
 
 Do not edit, please adjust language definitions in following repository:
 https://github.com/WeblateOrg/language-data
 """
 # pylint: disable=line-too-long,too-many-lines
@@ -412,15 +413,16 @@
     "mwl": 0,
     "mwr": 15913080,
     "my": 36559231,
     "my@Zawgyi": 36559231,
     "myv": 439338,
     "na": 6930,
     "nah": 0,
-    "nan": 26486380,
+    "nan_Hant": 26486380,
+    "nan_Latn": 26486380,
     "nap": 605306,
     "naq": 289307,
     "nb_NO": 5467440,
     "nd": 1745556,
     "nds": 11520008,
     "ne": 20903374,
     "new": 1000820,
@@ -642,15 +644,16 @@
     "xh": 10182944,
     "xog": 2292409,
     "yao": 722356,
     "yap": 6555,
     "yi": 997213,
     "yo": 28685568,
     "yua": 861955,
-    "yue": 7165718,
+    "yue_Hans": 72489040,
+    "yue_Hant": 7165718,
     "za": 4321462,
     "zap": 0,
     "zbl": 0,
     "zen": 0,
     "zgh": 7823574,
     "zh_Hans": 1266066359,
     "zh_Hans_SG": 4781438,
```

### Comparing `weblate-language-data-2023.3/weblate_language_data.egg-info/PKG-INFO` & `weblate-language-data-2023.4/weblate_language_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weblate-language-data
-Version: 2023.3
+Version: 2023.4
 Summary: Language definitions for Weblate
 Home-page: https://weblate.org/
 Download-URL: https://github.com/WeblateOrg/language-data
 Author: Michal Čihař
 Author-email: michal@weblate.org
 License: MIT
 Project-URL: Issue Tracker, https://github.com/WeblateOrg/language-data/issues
@@ -35,15 +35,15 @@
 License-File: LICENSE
 
 .. image:: https://s.weblate.org/cdn/Logo-Darktext-borders.png
    :alt: Weblate
    :target: https://weblate.org/
    :height: 80px
 
-**Weblate is a copylefted libre software web-based continuous localization system,
+**Weblate is libre software web-based continuous localization system,
 used by over 2500 libre projects and companies in more than 165 countries.**
 
 Language definitions used by `Weblate`_ and free to use by others.
 
 .. image:: https://img.shields.io/badge/website-weblate.org-blue.svg
     :alt: Website
     :target: https://weblate.org/
```

### Comparing `weblate-language-data-2023.3/weblate_language_data.egg-info/SOURCES.txt` & `weblate-language-data-2023.4/weblate_language_data.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 weblate_language_data/locale/ang/LC_MESSAGES/django.po
 weblate_language_data/locale/ar/LC_MESSAGES/django.po
 weblate_language_data/locale/ar_LY/LC_MESSAGES/django.po
 weblate_language_data/locale/ars/LC_MESSAGES/django.po
 weblate_language_data/locale/ast/LC_MESSAGES/django.po
 weblate_language_data/locale/az/LC_MESSAGES/django.po
 weblate_language_data/locale/be/LC_MESSAGES/django.po
-weblate_language_data/locale/be@latin/LC_MESSAGES/django.po
+weblate_language_data/locale/be_Latn/LC_MESSAGES/django.po
 weblate_language_data/locale/ber/LC_MESSAGES/django.po
 weblate_language_data/locale/bg/LC_MESSAGES/django.po
 weblate_language_data/locale/bn/LC_MESSAGES/django.po
 weblate_language_data/locale/bn_BD/LC_MESSAGES/django.po
 weblate_language_data/locale/bo/LC_MESSAGES/django.po
 weblate_language_data/locale/br/LC_MESSAGES/django.po
 weblate_language_data/locale/ca/LC_MESSAGES/django.po
@@ -133,12 +133,12 @@
 weblate_language_data/locale/tr/LC_MESSAGES/django.po
 weblate_language_data/locale/tt/LC_MESSAGES/django.po
 weblate_language_data/locale/tzm/LC_MESSAGES/django.po
 weblate_language_data/locale/ug/LC_MESSAGES/django.po
 weblate_language_data/locale/uk/LC_MESSAGES/django.po
 weblate_language_data/locale/uz/LC_MESSAGES/django.po
 weblate_language_data/locale/vi/LC_MESSAGES/django.po
-weblate_language_data/locale/yue/LC_MESSAGES/django.po
+weblate_language_data/locale/yue_Hant/LC_MESSAGES/django.po
 weblate_language_data/locale/zgh/LC_MESSAGES/django.po
 weblate_language_data/locale/zh_Hans/LC_MESSAGES/django.po
 weblate_language_data/locale/zh_Hant/LC_MESSAGES/django.po
 weblate_language_data/migrations/__init__.py
```

