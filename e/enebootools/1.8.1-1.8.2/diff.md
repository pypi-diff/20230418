# Comparing `tmp/enebootools-1.8.1.tar.gz` & `tmp/enebootools-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enebootools-1.8.1.tar", last modified: Wed Mar  8 13:16:21 2023, max compression
+gzip compressed data, was "enebootools-1.8.2.tar", last modified: Tue Apr 18 07:12:10 2023, max compression
```

## Comparing `enebootools-1.8.1.tar` & `enebootools-1.8.2.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.340517 enebootools-1.8.1/
--rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-1.8.1/AUTHORS
--rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-1.8.1/LICENSE.gplv3
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19874 2023-03-08 13:16:21.340517 enebootools-1.8.1/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-1.8.1/README.rst
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.328516 enebootools-1.8.1/enebootools/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-03-08 13:15:29.000000 enebootools-1.8.1/enebootools/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-1.8.1/enebootools/__init__.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.328516 enebootools-1.8.1/enebootools/assembler/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6000 2022-12-07 09:30:25.000000 enebootools-1.8.1/enebootools/assembler/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/assembler/config.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    29507 2022-12-01 09:57:04.000000 enebootools-1.8.1/enebootools/assembler/database.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/assembler/databasemodels.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-1.8.1/enebootools/assembler/featureconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    23152 2022-12-07 09:51:28.000000 enebootools-1.8.1/enebootools/assembler/kobjects.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/assembler/mypeewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-1.8.1/enebootools/assembler/save_auto.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.328516 enebootools-1.8.1/enebootools/autoconfig/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.1/enebootools/autoconfig/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-1.8.1/enebootools/autoconfig/autoconfig.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/autoconfig/parsers.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.328516 enebootools-1.8.1/enebootools/config/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.1/enebootools/config/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.328516 enebootools-1.8.1/enebootools/crypto/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/crypto/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.332516 enebootools-1.8.1/enebootools/crypto/certificates/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/crypto/certificates/CA_Test_Partners.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/crypto/certificates/Partner_Test.crt
--rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/crypto/certificates/Partner_Test.pem
--rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/crypto/certificates/README.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/crypto/certificates/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-1.8.1/enebootools/crypto/main.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.332516 enebootools-1.8.1/enebootools/databaseadmin/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.1/enebootools/databaseadmin/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.332516 enebootools-1.8.1/enebootools/databaseadmin/dblayer/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/databaseadmin/dblayer/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/databaseadmin/dblayer/drivers.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-1.8.1/enebootools/entry_points.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.332516 enebootools-1.8.1/enebootools/extracttool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/extracttool/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/extracttool/extractfunctions.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.332516 enebootools-1.8.1/enebootools/lib/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.1/enebootools/lib/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.332516 enebootools-1.8.1/enebootools/lib/etree/
--rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-1.8.1/enebootools/lib/etree/ElementInclude.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/lib/etree/ElementPath.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/lib/etree/ElementTree.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-1.8.1/enebootools/lib/etree/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-1.8.1/enebootools/lib/etree/cElementTree.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/lib/peewee.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/lib/utils.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.336516 enebootools-1.8.1/enebootools/mergetool/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    26266 2022-04-29 09:06:06.000000 enebootools-1.8.1/enebootools/mergetool/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.336516 enebootools-1.8.1/enebootools/mergetool/etc/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/mergetool/etc/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.340517 enebootools-1.8.1/enebootools/mergetool/etc/formats/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/mergetool/etc/formats/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/mergetool/etc/formats/aq23-kut.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-1.8.1/enebootools/mergetool/etc/formats/aq23-mtd.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/mergetool/etc/formats/aq23-xml.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/mergetool/etc/formats/qt3-ts.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/mergetool/etc/formats/qt3-ui.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/mergetool/etc/index.xml
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.340517 enebootools-1.8.1/enebootools/mergetool/etc/patch-styles/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/mergetool/etc/patch-styles/__init__.py
--rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
--rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/mergetool/etc/patch-styles/legacy1.xml
--rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-1.8.1/enebootools/mergetool/etc/patch-styles/semantic1.xml
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    31100 2023-03-08 13:14:00.000000 enebootools-1.8.1/enebootools/mergetool/flpatchdir.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    44114 2022-12-01 11:18:08.000000 enebootools-1.8.1/enebootools/mergetool/flpatchlxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-1.8.1/enebootools/mergetool/flpatchmodel.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    76823 2022-09-28 07:55:10.000000 enebootools-1.8.1/enebootools/mergetool/flpatchpy.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77369 2022-03-06 07:56:52.000000 enebootools-1.8.1/enebootools/mergetool/flpatchqs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-1.8.1/enebootools/mergetool/flpatchtest.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/mergetool/flpatchxml.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     3680 2022-12-01 13:23:45.000000 enebootools-1.8.1/enebootools/mergetool/projectbuilder.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.340517 enebootools-1.8.1/enebootools/mergetool/test/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-1.8.1/enebootools/mergetool/test/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-1.8.1/enebootools/mergetool/test/test_mergetool.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.340517 enebootools-1.8.1/enebootools/packager/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-1.8.1/enebootools/packager/__init__.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-1.8.1/enebootools/packager/pkgjoiner.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/packager/pkgsplitter.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-1.8.1/enebootools/parseargs.py
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-1.8.1/enebootools/parseargs.pyc
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.340517 enebootools-1.8.1/enebootools/parser/
--rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-1.8.1/enebootools/parser/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.340517 enebootools-1.8.1/enebootools/vcsworkflow/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-1.8.1/enebootools/vcsworkflow/__init__.py
-drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-03-08 13:16:21.328516 enebootools-1.8.1/enebootools.egg-info/
--rw-rw-r--   0 aulla     (1000) aulla     (1000)    19874 2023-03-08 13:16:21.000000 enebootools-1.8.1/enebootools.egg-info/PKG-INFO
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2836 2023-03-08 13:16:21.000000 enebootools-1.8.1/enebootools.egg-info/SOURCES.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-03-08 13:16:21.000000 enebootools-1.8.1/enebootools.egg-info/dependency_links.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)      311 2023-03-08 13:16:21.000000 enebootools-1.8.1/enebootools.egg-info/entry_points.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-03-08 13:16:21.000000 enebootools-1.8.1/enebootools.egg-info/requires.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-03-08 13:16:21.000000 enebootools-1.8.1/enebootools.egg-info/top_level.txt
--rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-03-08 13:16:21.340517 enebootools-1.8.1/setup.cfg
--rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-1.8.1/setup.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.851783 enebootools-1.8.2/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      259 2019-12-11 07:08:54.000000 enebootools-1.8.2/AUTHORS
+-rw-r--r--   0 aulla     (1000) aulla     (1000)    35146 2019-12-11 07:08:54.000000 enebootools-1.8.2/LICENSE.gplv3
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-04-18 07:12:10.847783 enebootools-1.8.2/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    18665 2022-02-08 10:20:48.000000 enebootools-1.8.2/README.rst
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6052 2023-04-18 07:10:33.000000 enebootools-1.8.2/enebootools/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7116 2020-06-27 08:28:15.000000 enebootools-1.8.2/enebootools/__init__.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools/assembler/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6000 2022-12-07 09:30:25.000000 enebootools-1.8.2/enebootools/assembler/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2584 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/assembler/config.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    29507 2022-12-01 09:57:04.000000 enebootools-1.8.2/enebootools/assembler/database.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1325 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/assembler/databasemodels.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1334 2022-03-05 09:43:22.000000 enebootools-1.8.2/enebootools/assembler/featureconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    23152 2023-04-18 07:09:46.000000 enebootools-1.8.2/enebootools/assembler/kobjects.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2276 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/assembler/mypeewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3124 2022-12-07 11:24:39.000000 enebootools-1.8.2/enebootools/assembler/save_auto.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools/autoconfig/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.2/enebootools/autoconfig/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     7521 2022-03-05 21:54:44.000000 enebootools-1.8.2/enebootools/autoconfig/autoconfig.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1955 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/autoconfig/parsers.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools/config/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.2/enebootools/config/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools/crypto/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3002 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/crypto/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/crypto/certificates/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2244 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1854 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/CA_Test_Partners.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2545 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1285 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/Partner_Test.crt
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      963 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/Partner_Test.pem
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      884 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/crypto/certificates/README.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/crypto/certificates/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    27617 2022-09-12 08:13:27.000000 enebootools-1.8.2/enebootools/crypto/main.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/databaseadmin/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.2/enebootools/databaseadmin/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/databaseadmin/dblayer/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/databaseadmin/dblayer/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4516 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/databaseadmin/dblayer/drivers.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     1507 2022-03-17 10:57:32.000000 enebootools-1.8.2/enebootools/entry_points.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/extracttool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    10935 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/extracttool/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3087 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/extracttool/extractfunctions.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/lib/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:10.000000 enebootools-1.8.2/enebootools/lib/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/lib/etree/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     5062 2020-06-21 07:16:10.000000 enebootools-1.8.2/enebootools/lib/etree/ElementInclude.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     9477 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/lib/etree/ElementPath.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    55969 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/lib/etree/ElementTree.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1604 2020-06-21 07:16:11.000000 enebootools-1.8.2/enebootools/lib/etree/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)       62 2020-06-21 07:16:11.000000 enebootools-1.8.2/enebootools/lib/etree/cElementTree.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    61938 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/lib/peewee.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2395 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/lib/utils.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/mergetool/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    26266 2022-04-29 09:06:06.000000 enebootools-1.8.2/enebootools/mergetool/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/mergetool/etc/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/mergetool/etc/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/mergetool/etc/formats/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1682 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-kut.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2128 2022-02-13 17:42:27.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-mtd.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1629 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-xml.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     1981 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/qt3-ts.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     7419 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/formats/qt3-ui.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      520 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/index.xml
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        0 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/__init__.py
+-rw-r--r--   0 aulla     (1000) aulla     (1000)     2214 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      807 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/legacy1.xml
+-rw-r--r--   0 aulla     (1000) aulla     (1000)      460 2019-12-11 07:08:54.000000 enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/semantic1.xml
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    31100 2023-03-08 13:14:00.000000 enebootools-1.8.2/enebootools/mergetool/flpatchdir.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    44114 2022-12-01 11:18:08.000000 enebootools-1.8.2/enebootools/mergetool/flpatchlxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77764 2022-09-28 07:55:55.000000 enebootools-1.8.2/enebootools/mergetool/flpatchmodel.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    76823 2022-09-28 07:55:10.000000 enebootools-1.8.2/enebootools/mergetool/flpatchpy.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77369 2022-03-06 07:56:52.000000 enebootools-1.8.2/enebootools/mergetool/flpatchqs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    77651 2022-09-28 07:55:13.000000 enebootools-1.8.2/enebootools/mergetool/flpatchtest.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    24828 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/mergetool/flpatchxml.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     3680 2022-12-01 13:23:45.000000 enebootools-1.8.2/enebootools/mergetool/projectbuilder.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/mergetool/test/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      552 2022-03-18 20:43:46.000000 enebootools-1.8.2/enebootools/mergetool/test/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2732 2022-04-29 09:13:12.000000 enebootools-1.8.2/enebootools/mergetool/test/test_mergetool.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/packager/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     4372 2022-09-12 07:54:48.000000 enebootools-1.8.2/enebootools/packager/__init__.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     6767 2023-01-16 11:50:25.000000 enebootools-1.8.2/enebootools/packager/pkgjoiner.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     8238 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/packager/pkgsplitter.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    15388 2022-11-29 10:40:19.000000 enebootools-1.8.2/enebootools/parseargs.py
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    13479 2020-06-27 08:28:15.000000 enebootools-1.8.2/enebootools/parseargs.pyc
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/parser/
+-rw-r--r--   0 aulla     (1000) aulla     (1000)        0 2020-06-21 07:16:13.000000 enebootools-1.8.2/enebootools/parser/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.847783 enebootools-1.8.2/enebootools/vcsworkflow/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      370 2022-02-08 10:20:48.000000 enebootools-1.8.2/enebootools/vcsworkflow/__init__.py
+drwxrwxr-x   0 aulla     (1000) aulla     (1000)        0 2023-04-18 07:12:10.843783 enebootools-1.8.2/enebootools.egg-info/
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)    19837 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/PKG-INFO
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2836 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/SOURCES.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)        1 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/dependency_links.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)      310 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/entry_points.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       21 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/requires.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       12 2023-04-18 07:12:10.000000 enebootools-1.8.2/enebootools.egg-info/top_level.txt
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)       38 2023-04-18 07:12:10.851783 enebootools-1.8.2/setup.cfg
+-rw-rw-r--   0 aulla     (1000) aulla     (1000)     2339 2022-02-08 10:20:48.000000 enebootools-1.8.2/setup.py
```

### Comparing `enebootools-1.8.1/LICENSE.gplv3` & `enebootools-1.8.2/LICENSE.gplv3`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/PKG-INFO` & `enebootools-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 1.8.1
+Version: 1.8.2
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
-License: UNKNOWN
 Keywords: erp pineboo eneboo tools
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -486,9 +484,7 @@
     
 Para conocer todas las opciones de la herramienta::
     
     $ eneboo-packager --help
 
 
 
-
-
```

### Comparing `enebootools-1.8.1/README.rst` & `enebootools-1.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/__init__.py` & `enebootools-1.8.2/enebootools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os.path
 import sys
 import traceback
 from pprint import pformat
 import enebootools.parseargs as pa
 
 
-__VERSION__ = "1.8.1"
+__VERSION__ = "1.8.2"
 QS_EXTEND_MODE = "legacy"
 
 
 def ustr(value):
     """Ustr."""
     if isinstance(value, str):
         return value
```

### Comparing `enebootools-1.8.1/enebootools/__init__.pyc` & `enebootools-1.8.2/enebootools/__init__.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/assembler/__init__.py` & `enebootools-1.8.2/enebootools/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/assembler/config.py` & `enebootools-1.8.2/enebootools/assembler/config.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/assembler/database.py` & `enebootools-1.8.2/enebootools/assembler/database.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/assembler/databasemodels.py` & `enebootools-1.8.2/enebootools/assembler/databasemodels.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/assembler/featureconfig.py` & `enebootools-1.8.2/enebootools/assembler/featureconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/assembler/kobjects.py` & `enebootools-1.8.2/enebootools/assembler/kobjects.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         if self.all_required_modules:
             return self.all_required_modules
         req = []
         myreq = []
         for modname in self.required_modules:
             obj = ModuleObject.find(modname)
             if obj is None:
-                self.iface.warn("Modulo con nombre %s no encontrado" % modname)
+                self.iface.info("Modulo con nombre %s no encontrado" % modname)
                 continue
             new_reqs = [
                 modulename
                 for modulename in obj._get_full_required_modules()
                 if modulename not in req
             ]
             if self.type == "prj":
@@ -101,15 +101,15 @@
             myreq.append(obj.formal_name())
 
         self.all_required_features = self._get_full_required_features()
 
         for featname in self.all_required_features:
             obj = FeatureObject.find(featname)
             if obj is None:
-                self.iface.warn("Funcionalidad con nombre %s no encontrada" % featname)
+                self.iface.info("Funcionalidad con nombre %s no encontrada" % featname)
                 continue
             new_reqs = [
                 modulename
                 for modulename in obj._get_full_required_modules()
                 if modulename not in req
             ]
             if self.type == "prj":
@@ -130,15 +130,15 @@
         if self.all_required_features:
             return self.all_required_features
         req = []
         myreq = []
         for featname in self.required_features:
             obj = FeatureObject.find(featname)
             if obj is None:
-                self.iface.warn("Funcionalidad con nombre %s no encontrada" % featname)
+                self.iface.info("Funcionalidad con nombre %s no encontrada" % featname)
                 continue
             new_reqs = [
                 featurename
                 for featurename in obj._get_full_required_features()
                 if featurename not in req
             ]
             if self.type == "prj":
```

### Comparing `enebootools-1.8.1/enebootools/assembler/mypeewee.py` & `enebootools-1.8.2/enebootools/assembler/mypeewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/assembler/save_auto.py` & `enebootools-1.8.2/enebootools/assembler/save_auto.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/autoconfig/autoconfig.py` & `enebootools-1.8.2/enebootools/autoconfig/autoconfig.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/autoconfig/parsers.py` & `enebootools-1.8.2/enebootools/autoconfig/parsers.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/crypto/__init__.py` & `enebootools-1.8.2/enebootools/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt` & `enebootools-1.8.2/enebootools/crypto/certificates/CA_Partners_Gestiweb.crt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/crypto/certificates/CA_Test_Partners.crt` & `enebootools-1.8.2/enebootools/crypto/certificates/CA_Test_Partners.crt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt` & `enebootools-1.8.2/enebootools/crypto/certificates/Eneboo_Open_Source_ERP.crt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/crypto/certificates/Partner_Test.crt` & `enebootools-1.8.2/enebootools/crypto/certificates/Partner_Test.crt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/crypto/certificates/Partner_Test.pem` & `enebootools-1.8.2/enebootools/crypto/certificates/Partner_Test.pem`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/crypto/certificates/README.txt` & `enebootools-1.8.2/enebootools/crypto/certificates/README.txt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/crypto/main.py` & `enebootools-1.8.2/enebootools/crypto/main.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/databaseadmin/dblayer/drivers.py` & `enebootools-1.8.2/enebootools/databaseadmin/dblayer/drivers.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/entry_points.py` & `enebootools-1.8.2/enebootools/entry_points.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/extracttool/__init__.py` & `enebootools-1.8.2/enebootools/extracttool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/extracttool/extractfunctions.py` & `enebootools-1.8.2/enebootools/extracttool/extractfunctions.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/lib/etree/ElementInclude.py` & `enebootools-1.8.2/enebootools/lib/etree/ElementInclude.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/lib/etree/ElementPath.py` & `enebootools-1.8.2/enebootools/lib/etree/ElementPath.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/lib/etree/ElementTree.py` & `enebootools-1.8.2/enebootools/lib/etree/ElementTree.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/lib/etree/__init__.py` & `enebootools-1.8.2/enebootools/lib/etree/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/lib/peewee.py` & `enebootools-1.8.2/enebootools/lib/peewee.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/lib/utils.py` & `enebootools-1.8.2/enebootools/lib/utils.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/__init__.py` & `enebootools-1.8.2/enebootools/mergetool/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/etc/formats/aq23-kut.xml` & `enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-kut.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/etc/formats/aq23-mtd.xml` & `enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-mtd.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/etc/formats/aq23-xml.xml` & `enebootools-1.8.2/enebootools/mergetool/etc/formats/aq23-xml.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/etc/formats/qt3-ts.xml` & `enebootools-1.8.2/enebootools/mergetool/etc/formats/qt3-ts.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/etc/formats/qt3-ui.xml` & `enebootools-1.8.2/enebootools/mergetool/etc/formats/qt3-ui.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/etc/index.xml` & `enebootools-1.8.2/enebootools/mergetool/etc/index.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl` & `enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/legacy1-savepatch1.xsl`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/etc/patch-styles/legacy1.xml` & `enebootools-1.8.2/enebootools/mergetool/etc/patch-styles/legacy1.xml`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/flpatchdir.py` & `enebootools-1.8.2/enebootools/mergetool/flpatchdir.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/flpatchlxml.py` & `enebootools-1.8.2/enebootools/mergetool/flpatchlxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/flpatchmodel.py` & `enebootools-1.8.2/enebootools/mergetool/flpatchmodel.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/flpatchpy.py` & `enebootools-1.8.2/enebootools/mergetool/flpatchpy.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/flpatchqs.py` & `enebootools-1.8.2/enebootools/mergetool/flpatchqs.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/flpatchtest.py` & `enebootools-1.8.2/enebootools/mergetool/flpatchtest.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/flpatchxml.py` & `enebootools-1.8.2/enebootools/mergetool/flpatchxml.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/projectbuilder.py` & `enebootools-1.8.2/enebootools/mergetool/projectbuilder.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/test/__init__.py` & `enebootools-1.8.2/enebootools/mergetool/test/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/mergetool/test/test_mergetool.py` & `enebootools-1.8.2/enebootools/mergetool/test/test_mergetool.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/packager/__init__.py` & `enebootools-1.8.2/enebootools/packager/__init__.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/packager/pkgjoiner.py` & `enebootools-1.8.2/enebootools/packager/pkgjoiner.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/packager/pkgsplitter.py` & `enebootools-1.8.2/enebootools/packager/pkgsplitter.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/parseargs.py` & `enebootools-1.8.2/enebootools/parseargs.py`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools/parseargs.pyc` & `enebootools-1.8.2/enebootools/parseargs.pyc`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/enebootools.egg-info/PKG-INFO` & `enebootools-1.8.2/enebootools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: enebootools
-Version: 1.8.1
+Version: 1.8.2
 Summary: ERP tools for Eneboo
 Home-page: https://github.com/aulla/eneboo-tools
 Author: David Martínez Martí, José A. Fernández Fernández
 Author-email: deavidsedice@gmail.com, aullasistemas@gmail.com
-License: UNKNOWN
 Keywords: erp pineboo eneboo tools
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -486,9 +484,7 @@
     
 Para conocer todas las opciones de la herramienta::
     
     $ eneboo-packager --help
 
 
 
-
-
```

### Comparing `enebootools-1.8.1/enebootools.egg-info/SOURCES.txt` & `enebootools-1.8.2/enebootools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enebootools-1.8.1/setup.py` & `enebootools-1.8.2/setup.py`

 * *Files identical despite different names*

