# Comparing `tmp/idds-server-1.1.5.tar.gz` & `tmp/idds-server-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-server-1.1.5.tar", last modified: Sat Mar  4 21:39:56 2023, max compression
+gzip compressed data, was "idds-server-1.2.0.tar", last modified: Tue Apr 18 09:36:52 2023, max compression
```

## Comparing `idds-server-1.1.5.tar` & `idds-server-1.2.0.tar`

### file list

```diff
@@ -1,245 +1,260 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.897604 idds-server-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-04 21:39:47.000000 idds-server-1.1.5/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-04 21:39:56.897604 idds-server-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-04 21:39:47.000000 idds-server-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-03-04 21:39:47.000000 idds-server-1.1.5/bin/idds-daemon
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-04 21:39:56.000000 idds-server-1.1.5/bin/idds.wsgi
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-04 21:39:47.000000 idds-server-1.1.5/bin/idds.wsgi.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-03-04 21:39:47.000000 idds-server-1.1.5/bin/run-idds
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-04 21:39:47.000000 idds-server-1.1.5/bin/run-idds-fake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/config_default/
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/auth.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/gacl
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/httpd-idds-443-py39-cc7.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/idds.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/panda.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/rucio.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/supervisord_httpd.ini
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/supervisord_idds.ini
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/supervisord_iddsfake.ini
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/supervisord_logrotate.ini
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-03-04 21:39:47.000000 idds-server-1.1.5/config_default/supervisord_syslog-ng.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.873604 idds-server-1.1.5/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/etc/idds/
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/alembic.ini.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/etc/idds/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/auth/auth.cfg.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.873604 idds-server-1.1.5/etc/idds/condor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/etc/idds/condor/client/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/condor/client/00personal_condor.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/etc/idds/condor/server/
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/condor/server/00personal_condor.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/idds.cfg.client.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     3846 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/idds.cfg.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/etc/idds/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/rest/gacl.template
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-03-04 21:39:56.000000 idds-server-1.1.5/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/rest/ssl.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/etc/idds/supervisord.d/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/supervisord.d/idds.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/etc/idds/website/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/website/25-port443.conf
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/idds/website/25-port80.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/etc/sql/
--rw-r--r--   0 runner    (1001) docker     (123)    25596 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/sql/oracle_11.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/sql/oracle_11_test.sql
--rw-r--r--   0 runner    (1001) docker     (123)    22610 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/sql/oracle_19.sql
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/sql/oracle_update.sql
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-04 21:39:47.000000 idds-server-1.1.5/etc/sql/postgresql.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.873604 idds-server-1.1.5/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.877604 idds-server-1.1.5/lib/idds/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/agents/carrier/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/carrier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/carrier/finisher.py
--rw-r--r--   0 runner    (1001) docker     (123)    23756 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/carrier/poller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/carrier/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/carrier/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/carrier/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)    83968 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/carrier/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/agents/clerk/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/clerk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53171 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/clerk/clerk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/agents/common/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/baseagent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/agents/common/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/cache/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/agents/common/eventbus/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/eventbus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/eventbus/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/eventbus/eventbus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/eventbus/localeventbusbackend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/agents/common/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14405 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/plugins/messaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/timerscheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/common/timertask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/agents/conductor/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/conductor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/conductor/conductor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/conductor/consumer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5289 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/agents/marshaller/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/marshaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/marshaller/marshaller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/agents/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40258 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/transformer/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/agents/transporter/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/transporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22626 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/agents/transporter/transporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.881604 idds-server-1.1.5/lib/idds/api/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/api/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/api/contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/api/processings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/api/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/api/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.885604 idds-server-1.1.5/lib/idds/core/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29135 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/core/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/core/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/core/processings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20000 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/core/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/core/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/core/workprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.885604 idds-server-1.1.5/lib/idds/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.885604 idds-server-1.1.5/lib/idds/orm/base/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.885604 idds-server-1.1.5/lib/idds/orm/base/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/base/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/base/alembic/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.885604 idds-server-1.1.5/lib/idds/orm/base/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/base/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/base/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    43800 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/base/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/base/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/base/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    35305 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/contents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16687 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/processings.py
--rw-r--r--   0 runner    (1001) docker     (123)    48740 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    20205 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11283 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/orm/workprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.885604 idds-server-1.1.5/lib/idds/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.889604 idds-server-1.1.5/lib/idds/rest/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/hyperparameteropt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    28102 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/rest/v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.893604 idds-server-1.1.5/lib/idds/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/activelearning_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/auth_test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/cacher_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/catalog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    22179 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/core_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/core_tests_dep_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/core_tests_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/datacarousel_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/doma_build_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/find_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/fix_content_dep_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/fix_trasnform_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/hyperparameteropt_bayesian_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/hyperparameteropt_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/hyperparameteropt_docker_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/hyperparameteropt_docker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/hyperparameteropt_nevergrad_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/jsonload_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/kill_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/logs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/match_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/message_test1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/migrating_requests_v1_to_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/panda_iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/panda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/performance_test_with_cx_oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/performance_test_with_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/relation_map_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/rest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/retry_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/run_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/scaling_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/split_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_activelearning.py
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_atlaspandawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_big_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    34114 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_datacarousel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_domapanda.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_domapanda_pandaclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_domapanda_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_get_dn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_hyperparameteropt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_migrate_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_request_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_running_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_transform_collection_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_transform_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    28166 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_workflow_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    69660 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/test_workflow_condition_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-04 21:39:47.000000 idds-server-1.1.5/lib/idds/tests/trigger_release.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-04 21:39:54.000000 idds-server-1.1.5/lib/idds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.893604 idds-server-1.1.5/lib/idds_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-03-04 21:39:56.000000 idds-server-1.1.5/lib/idds_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-03-04 21:39:56.000000 idds-server-1.1.5/lib/idds_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 21:39:56.000000 idds-server-1.1.5/lib/idds_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-04 21:39:56.000000 idds-server-1.1.5/lib/idds_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-04 21:39:56.000000 idds-server-1.1.5/lib/idds_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-04 21:39:56.897604 idds-server-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-03-04 21:39:47.000000 idds-server-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.873604 idds-server-1.1.5/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 21:39:56.897604 idds-server-1.1.5/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/config_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/config_server
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/create_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/create_postgres_db.sh
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/destroy_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-04 21:39:54.000000 idds-server-1.1.5/tools/env/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/install_env_conda.sh
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/install_idds.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/install_idds_full.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/install_packages.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/merge_configmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/merge_idds_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/setup_dev.sh
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/setup_idds.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-04 21:39:47.000000 idds-server-1.1.5/tools/env/setup_panda.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.438967 idds-server-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-18 09:36:40.000000 idds-server-1.2.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-18 09:36:52.438967 idds-server-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-18 09:36:40.000000 idds-server-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.418967 idds-server-1.2.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1687 2023-04-18 09:36:40.000000 idds-server-1.2.0/bin/idds-daemon
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-18 09:36:52.000000 idds-server-1.2.0/bin/idds.wsgi
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-18 09:36:40.000000 idds-server-1.2.0/bin/idds.wsgi.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-04-18 09:36:40.000000 idds-server-1.2.0/bin/run-idds
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 09:36:40.000000 idds-server-1.2.0/bin/run-idds-fake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.418967 idds-server-1.2.0/config_default/
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/auth.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/gacl
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/httpd-idds-443-py39-cc7.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3679 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/idds.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/panda.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/rucio.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/supervisord_httpd.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/supervisord_idds.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/supervisord_iddsfake.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/supervisord_logrotate.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-18 09:36:40.000000 idds-server-1.2.0/config_default/supervisord_syslog-ng.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.414967 idds-server-1.2.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.418967 idds-server-1.2.0/etc/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/alembic.ini.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.418967 idds-server-1.2.0/etc/idds/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/auth/auth.cfg.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.414967 idds-server-1.2.0/etc/idds/condor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.418967 idds-server-1.2.0/etc/idds/condor/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/condor/client/00personal_condor.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.418967 idds-server-1.2.0/etc/idds/condor/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/condor/server/00personal_condor.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/idds.cfg.client.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3946 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/idds.cfg.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.418967 idds-server-1.2.0/etc/idds/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/rest/gacl.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-18 09:36:52.000000 idds-server-1.2.0/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/rest/ssl.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.418967 idds-server-1.2.0/etc/idds/supervisord.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/supervisord.d/idds.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.418967 idds-server-1.2.0/etc/idds/website/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/website/25-port443.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/idds/website/25-port80.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.422967 idds-server-1.2.0/etc/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)    25596 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/sql/oracle_11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/sql/oracle_11_test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    22610 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/sql/oracle_19.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    16525 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/sql/oracle_update.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    12199 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/sql/postgresql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-18 09:36:40.000000 idds-server-1.2.0/etc/sql/postgresql_init.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.414967 idds-server-1.2.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.422967 idds-server-1.2.0/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.422967 idds-server-1.2.0/lib/idds/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.422967 idds-server-1.2.0/lib/idds/agents/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/archive/archiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/archive/run_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.422967 idds-server-1.2.0/lib/idds/agents/carrier/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/carrier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/carrier/finisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24234 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/carrier/poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/carrier/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/carrier/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/carrier/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88606 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/carrier/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.422967 idds-server-1.2.0/lib/idds/agents/clerk/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/clerk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53880 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/clerk/clerk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.422967 idds-server-1.2.0/lib/idds/agents/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/baseagent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.422967 idds-server-1.2.0/lib/idds/agents/common/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/cache/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.426967 idds-server-1.2.0/lib/idds/agents/common/eventbus/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/eventbus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/eventbus/baseeventbusbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7330 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/eventbus/baseeventbusbackendopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/eventbus/dbeventbusbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/eventbus/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/eventbus/eventbus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/eventbus/msgeventbusbackend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.426967 idds-server-1.2.0/lib/idds/agents/common/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14417 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/plugins/messaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/timerscheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/common/timertask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.426967 idds-server-1.2.0/lib/idds/agents/conductor/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/conductor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/conductor/conductor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/conductor/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.426967 idds-server-1.2.0/lib/idds/agents/coordinator/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/coordinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/coordinator/coordinator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5468 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.426967 idds-server-1.2.0/lib/idds/agents/marshaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/marshaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/marshaller/marshaller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.426967 idds-server-1.2.0/lib/idds/agents/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40926 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/transformer/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.426967 idds-server-1.2.0/lib/idds/agents/transporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/transporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22626 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/agents/transporter/transporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.426967 idds-server-1.2.0/lib/idds/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/api/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/api/contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/api/processings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/api/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/api/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.430967 idds-server-1.2.0/lib/idds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30222 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/core/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/core/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17949 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/core/processings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20378 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/core/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/core/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/core/workprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.430967 idds-server-1.2.0/lib/idds/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.430967 idds-server-1.2.0/lib/idds/orm/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.430967 idds-server-1.2.0/lib/idds/orm/base/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/base/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/base/alembic/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.430967 idds-server-1.2.0/lib/idds/orm/base/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/base/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/base/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51365 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/base/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/base/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39644 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/contents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11642 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16586 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/processings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48600 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20108 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/orm/workprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.430967 idds-server-1.2.0/lib/idds/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.430967 idds-server-1.2.0/lib/idds/rest/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/hyperparameteropt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28102 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/rest/v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.438967 idds-server-1.2.0/lib/idds/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/activelearning_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/auth_test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/cacher_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/catalog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12118 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/core_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/core_tests_dep_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/core_tests_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/datacarousel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/doma_build_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/find_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/fix_content_dep_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/fix_trasnform_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/hyperparameteropt_bayesian_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/hyperparameteropt_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/hyperparameteropt_docker_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/hyperparameteropt_docker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/hyperparameteropt_nevergrad_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/jsonload_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/kill_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/logs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/match_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/message_test1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/migrating_requests_v1_to_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/panda_iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/panda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/performance_test_with_cx_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/performance_test_with_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/relation_map_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/rest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/retry_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/run_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/scaling_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/split_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_activelearning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_atlaspandawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_big_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34114 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_datacarousel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_domapanda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_domapanda_pandaclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_domapanda_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_get_dn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_hyperparameteropt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_merge_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_migrate_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_request_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_running_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_transform_collection_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_transform_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28166 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_workflow_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69660 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/test_workflow_condition_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-18 09:36:40.000000 idds-server-1.2.0/lib/idds/tests/trigger_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-18 09:36:49.000000 idds-server-1.2.0/lib/idds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.438967 idds-server-1.2.0/lib/idds_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-18 09:36:52.000000 idds-server-1.2.0/lib/idds_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-04-18 09:36:52.000000 idds-server-1.2.0/lib/idds_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:36:52.000000 idds-server-1.2.0/lib/idds_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-18 09:36:52.000000 idds-server-1.2.0/lib/idds_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 09:36:52.000000 idds-server-1.2.0/lib/idds_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-18 09:36:52.438967 idds-server-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-04-18 09:36:40.000000 idds-server-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.414967 idds-server-1.2.0/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:36:52.438967 idds-server-1.2.0/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/config_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/config_server
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/create_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/create_postgres_db.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/destroy_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/dump_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-18 09:36:49.000000 idds-server-1.2.0/tools/env/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/install_env_conda.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/install_idds.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/install_idds_full.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      152 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/install_packages.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/merge_configmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/merge_idds_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/setup_dev.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/setup_idds.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-18 09:36:40.000000 idds-server-1.2.0/tools/env/setup_panda.sh
```

### Comparing `idds-server-1.1.5/LICENSE.rst` & `idds-server-1.2.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/PKG-INFO` & `idds-server-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-server
-Version: 1.1.5
+Version: 1.2.0
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-server-1.1.5/bin/idds-daemon` & `idds-server-1.2.0/bin/idds-daemon`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/bin/idds.wsgi` & `idds-server-1.2.0/bin/idds.wsgi.template`

 * *Files 16% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 # - Wen Guan, <wen.guan@cern.ch>, 2019
 
 """----------------------
    Web service startup
 ----------------------"""
 
 import os
-os.environ['IDDS_CONFIG'] = '/opt/hostedtoolcache/Python/3.11.2/x64/etc/idds/idds.cfg'
+os.environ['IDDS_CONFIG'] = '{idds_config_path}'
 
 from idds.rest.v1.app import create_app  # noqa: E402
 
 
 application = create_app()
```

### Comparing `idds-server-1.1.5/bin/idds.wsgi.template` & `idds-server-1.2.0/bin/idds.wsgi`

 * *Files 26% similar despite different names*

```diff
@@ -9,13 +9,13 @@
 # - Wen Guan, <wen.guan@cern.ch>, 2019
 
 """----------------------
    Web service startup
 ----------------------"""
 
 import os
-os.environ['IDDS_CONFIG'] = '{idds_config_path}'
+os.environ['IDDS_CONFIG'] = '/opt/hostedtoolcache/Python/3.11.3/x64/etc/idds/idds.cfg'
 
 from idds.rest.v1.app import create_app  # noqa: E402
 
 
 application = create_app()
```

### Comparing `idds-server-1.1.5/bin/run-idds` & `idds-server-1.2.0/bin/run-idds`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/config_default/alembic.ini` & `idds-server-1.2.0/config_default/alembic.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/config_default/gacl` & `idds-server-1.2.0/config_default/gacl`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/config_default/httpd-idds-443-py39-cc7.conf` & `idds-server-1.2.0/config_default/httpd-idds-443-py39-cc7.conf`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/config_default/idds.cfg` & `idds-server-1.2.0/config_default/idds.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 #
 # Authors:
-# - Wen Guan, <wen.guan@cern.ch>, 2019
+# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
 [common]
 #logdir = /var/log/idds
 # loglevel = DEBUG
 loglevel = INFO
 
 [database]
@@ -19,15 +19,25 @@
 
 [rest]
 host = https://localhost:443/idds
 cacher_dir = /var/log/idds
 
 [main]
 # agents = clerk, transformer, carrier, conductor
-agents = clerk, transformer, submitter, poller, receiver, trigger, finisher, conductor
+# agents = clerk, transformer, submitter, poller, receiver, trigger, finisher, conductor
+agents = clerk, transformer, submitter, poller, receiver, trigger, finisher, conductor, archiver, coordinator
+
+[eventbus]
+# backend = database
+backend = message
+# debug = True
+
+[coordinator]
+coordination_interval_delay = 300
+
 
 [clerk]
 num_threads = 4
 poll_period = 1800
 new_poll_period = 10
 update_poll_period = 1800
 new_command_poll_period = 10
@@ -108,7 +118,13 @@
                                         "broker_timeout": 360},
                             "ContentExt": {"brokers": ["atlas-test-mb.cern.ch:61013"],
                                            "destination": "/queue/atlas.idds",
                                            "username": "user",
                                            "password": "password",
                                            "broker_timeout": 360}
                            }
+
+[archiver]
+# days
+older_than = 60
+poll_period = 1
+
```

### Comparing `idds-server-1.1.5/config_default/rucio.cfg` & `idds-server-1.2.0/config_default/rucio.cfg`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/config_default/supervisord_httpd.ini` & `idds-server-1.2.0/config_default/supervisord_httpd.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/config_default/supervisord_idds.ini` & `idds-server-1.2.0/config_default/supervisord_idds.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/config_default/supervisord_iddsfake.ini` & `idds-server-1.2.0/config_default/supervisord_iddsfake.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/config_default/supervisord_logrotate.ini` & `idds-server-1.2.0/config_default/supervisord_logrotate.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/config_default/supervisord_syslog-ng.ini` & `idds-server-1.2.0/config_default/supervisord_syslog-ng.ini`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/alembic.ini.template` & `idds-server-1.2.0/etc/idds/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/auth/auth.cfg.template` & `idds-server-1.2.0/etc/idds/auth/auth.cfg.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/condor/client/00personal_condor.config` & `idds-server-1.2.0/etc/idds/condor/client/00personal_condor.config`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/condor/server/00personal_condor.config` & `idds-server-1.2.0/etc/idds/condor/server/00personal_condor.config`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/idds.cfg.client.template` & `idds-server-1.2.0/etc/idds/idds.cfg.client.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/idds.cfg.template` & `idds-server-1.2.0/etc/idds/idds.cfg.template`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,21 @@
 #plugin.<plugin_name>.<attr1> = <value1>
 #plugin.<plugin_name>.<attr2> = <value2>
 
 [main]
 # agents = clerk, marshaller, transformer, carrier, conductor, consumer
 agents = clerk, transformer, carrier, conductor
 
+[eventbus]
+# backend = database
+backend = message
+
+[coordinator]
+coordination_interval_delay = 300
+
 [clerk]
 num_threads = 3
 poll_time_period = 120
 poll_operation_time_period = 120
 retrieve_bulk_size = 3
 pending_time = 3
```

### Comparing `idds-server-1.1.5/etc/idds/rest/gacl.template` & `idds-server-1.2.0/etc/idds/rest/gacl.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template` & `idds-server-1.2.0/etc/idds/rest/httpd-idds-443-py36-cc7.conf.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template` & `idds-server-1.2.0/etc/idds/rest/httpd-idds-443-py36-cc7_normal.conf.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template` & `idds-server-1.2.0/etc/idds/rest/httpd-idds-443-py39-cc7.conf.install_template`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 # # LoadModule dir_module           /usr/lib64/httpd/modules/mod_dir.so
 # # LoadModule alias_module         /usr/lib64/httpd/modules/mod_alias.so
 # # LoadModule cgi_module           /usr/lib64/httpd/modules/mod_cgi.so
 
 # External modules
 LoadModule gridsite_module /usr/lib64/httpd/modules/mod_gridsite.so
 #LoadModule wsgi_module /usr/lib64/httpd/modules/mod_wsgi.so
-LoadModule wsgi_module /opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages/mod_wsgi/server/mod_wsgi-py39.cpython-39-x86_64-linux-gnu.so
+LoadModule wsgi_module /opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages/mod_wsgi/server/mod_wsgi-py39.cpython-39-x86_64-linux-gnu.so
 
-WSGIPythonHome /opt/hostedtoolcache/Python/3.11.2/x64
-WSGIPythonPath /opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages
+WSGIPythonHome /opt/hostedtoolcache/Python/3.11.3/x64
+WSGIPythonPath /opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages
 
 <IfModule mod_wsgi.c>
-    WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home=/opt/hostedtoolcache/Python/3.11.2/x64 python-path=/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages
+    WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home=/opt/hostedtoolcache/Python/3.11.3/x64 python-path=/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages
     WSGIProcessGroup idds_daemon
     WSGIApplicationGroup %GLOBAL
-    WSGIScriptAlias /idds /opt/hostedtoolcache/Python/3.11.2/x64/bin/idds.wsgi
+    WSGIScriptAlias /idds /opt/hostedtoolcache/Python/3.11.3/x64/bin/idds.wsgi
     # WSGIScriptAliasMatch ^/idds/(.+)$ /opt/idds/etc/idds/rest/test.wsgi
     WSGISocketPrefix /var/log/idds/wsgisocks/wsgi
     # WSGISocketPrefix /tmp/idds/wsgisocks/wsgi
     WSGIPassAuthorization On
 </IfModule>
 
 Listen 443
@@ -71,18 +71,18 @@
     SSLHonorCipherOrder on
 
     LogLevel debug
     ErrorLog /var/log/idds/httpd_error_log
     TransferLog /var/log/idds/httpd_access_log
 
     <IfModule mod_wsgi.c>
-        WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home=/opt/hostedtoolcache/Python/3.11.2/x64 python-path=/opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages
+        WSGIDaemonProcess idds_daemon processes=25 threads=2 request-timeout=600 queue-timeout=600 python-home=/opt/hostedtoolcache/Python/3.11.3/x64 python-path=/opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages
         WSGIProcessGroup idds_daemon
         WSGIApplicationGroup %GLOBAL
-        WSGIScriptAlias /idds /opt/hostedtoolcache/Python/3.11.2/x64/bin/idds.wsgi
+        WSGIScriptAlias /idds /opt/hostedtoolcache/Python/3.11.3/x64/bin/idds.wsgi
         # WSGIScriptAliasMatch ^/idds/(.+)$ /opt/idds/etc/idds/rest/test.wsgi
         # WSGISocketPrefix /var/log/idds/wsgisocks/wsgi
         WSGISocketPrefix /tmp/idds/wsgisocks/wsgi
         WSGIPassAuthorization On
     </IfModule>
 
     # Proxy authentication via mod_gridsite
@@ -101,21 +101,21 @@
         GridSiteDNlists /etc/grid-security/dn-lists/
         GridSiteGSIProxyLimit 16
         GridSiteEnvs on
         GridSiteACLPath /opt/idds/etc/idds/rest/gacl
         # GridSiteMethods GET
     </LocationMatch>
 
-    <Directory /opt/hostedtoolcache/Python/3.11.2/x64/lib/python3.11/site-packages>
+    <Directory /opt/hostedtoolcache/Python/3.11.3/x64/lib/python3.11/site-packages>
         # Order deny,allow
         # Allow from all
         # Require all granted
     </Directory>
 
-    <Directory /opt/hostedtoolcache/Python/3.11.2/x64/bin>
+    <Directory /opt/hostedtoolcache/Python/3.11.3/x64/bin>
         Order deny,allow
         Allow from all
         Require all granted
     </Directory>
 
     <Directory /opt/idds/website/data>
         Order deny,allow
```

### Comparing `idds-server-1.1.5/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template` & `idds-server-1.2.0/etc/idds/rest/httpd-idds-443-py39-cc7.conf.template`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/rest/ssl.conf` & `idds-server-1.2.0/etc/idds/rest/ssl.conf`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/idds/website/25-port443.conf` & `idds-server-1.2.0/etc/idds/website/25-port443.conf`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/sql/oracle_11.sql` & `idds-server-1.2.0/etc/sql/oracle_11.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/sql/oracle_11_test.sql` & `idds-server-1.2.0/etc/sql/oracle_11_test.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/sql/oracle_19.sql` & `idds-server-1.2.0/etc/sql/oracle_19.sql`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/etc/sql/oracle_update.sql` & `idds-server-1.2.0/etc/sql/oracle_update.sql`

 * *Files 16% similar despite different names*

```diff
@@ -307,7 +307,95 @@
 CREATE OR REPLACE procedure update_contents_to_others(request_id_in NUMBER, transform_id_in NUMBER) AS
 BEGIN
     update (select c.content_id, c.substatus as c_substatus, t.substatus as t_substatus from  
     (select content_id, substatus, content_dep_id from contents where request_id = request_id_in and content_relation_type = 3) c inner join
     (select content_id, substatus from contents where request_id = request_id_in and transform_id = transform_id_in and content_relation_type = 1) t
     on c.content_dep_id = t.content_id where c.substatus != t.substatus) set c_substatus = t_substatus;
 END;
+
+
+
+--- 2023.03.06
+drop index PROCESSINGS_STATUS_POLL_IDX;
+drop index CONTENTS_REL_IDX;
+drop index CONTENTS_TF_IDX;
+drop index CONTENTS_EXT_RTW_IDX;
+drop index CONTENTS_EXT_RTM_IDX;
+drop index COMMANDS_STATUS_IDX;
+drop index MESSAGES_ST_IDX;
+drop index MESSAGES_TYPE_STU_IDX;
+drop index REQUESTS_STATUS_POLL_IDX;
+drop index TRANSFORMS_REQ_IDX;
+drop index TRANSFORMS_STATUS_POLL_IDX;
+drop index COLLECTIONS_REQ_IDX;
+
+CREATE INDEX PROCESSINGS_STATUS_POLL_IDX ON PROCESSINGS (status, processing_id, locking, updated_at, new_poll_period, update_poll_period, created_at) COMPRESS 3 LOCAL;
+
+CREATE INDEX CONTENTS_REL_IDX ON CONTENTS  (request_id, content_relation_type, transform_id, substatus) COMPRESS 3 LOCAL;
+CREATE INDEX CONTENTS_TF_IDX ON CONTENTS  (transform_id, request_id, coll_id, content_relation_type, map_id) COMPRESS 4 LOCAL;
+
+CREATE INDEX CONTENTS_EXT_RTW_IDX ON contents_ext (request_id, transform_id, workload_id) COMPRESS 3 ;
+CREATE INDEX CONTENTS_EXT_RTM_IDX ON contents_ext (request_id, transform_id, map_id) COMPRESS 2;
+
+CREATE INDEX COMMANDS_STATUS_IDX on commands (status, locking, updated_at) COMPRESS 2;
+
+CREATE INDEX MESSAGES_ST_IDX on messages (status, destination, created_at) COMPRESS 2;
+CREATE INDEX MESSAGES_TYPE_STU_IDX on messages (msg_type, status, destination, retries, updated_at, created_at) COMPRESS 3;
+
+CREATE INDEX REQUESTS_STATUS_POLL_IDX on REQUESTS (status, request_id, locking, priority, updated_at, new_poll_period, update_poll_period, next_poll_at, created_at) COMPRESS 3 LOCAL;
+
+CREATE INDEX TRANSFORMS_REQ_IDX on transforms (request_id, transform_id) COMPRESS 2;
+CREATE INDEX TRANSFORMS_STATUS_POLL_IDX on transforms (status, transform_id, locking, updated_at, new_poll_period, update_poll_period, created_at) COMPRESS 3 LOCAL;
+
+CREATE INDEX COLLECTIONS_REQ_IDX on collections (request_id, transform_id, updated_at) COMPRESS 2;
+
+
+-- 2023.03.10
+
+CREATE SEQUENCE EVENT_ID_SEQ MINVALUE 1 INCREMENT BY 1 START WITH 1 NOCACHE ORDER NOCYCLE GLOBAL;
+CREATE TABLE EVENTS
+(
+    event_id NUMBER(12) DEFAULT ON NULL EVENT_ID_SEQ.NEXTVAL constraint EVENT_ID_NN NOT NULL,
+    event_type NUMBER(12),
+    event_actual_id NUMBER(12),
+    priority NUMBER(12),
+    status NUMBER(2),
+    created_at DATE DEFAULT SYS_EXTRACT_UTC(systimestamp(0)),
+    processing_at DATE DEFAULT SYS_EXTRACT_UTC(systimestamp(0)),
+    processed_at DATE DEFAULT SYS_EXTRACT_UTC(systimestamp(0)),
+    content CLOB,
+    CONSTRAINT EVENTS_PK PRIMARY KEY (event_id) -- USING INDEX LOCAL,
+);
+
+CREATE TABLE EVENTS_ARCHIVE
+(
+    event_id NUMBER(12),
+    event_type NUMBER(12),
+    event_actual_id NUMBER(12),
+    priority NUMBER(12),
+    status NUMBER(2),
+    created_at DATE DEFAULT SYS_EXTRACT_UTC(systimestamp(0)),
+    processing_at DATE DEFAULT SYS_EXTRACT_UTC(systimestamp(0)),
+    processed_at DATE DEFAULT SYS_EXTRACT_UTC(systimestamp(0)),
+    content CLOB,
+    CONSTRAINT EVENTS_AR_PK PRIMARY KEY (event_id) -- USING INDEX LOCAL,
+);
+
+CREATE TABLE EVENTS_PRIORITY
+(
+    event_type NUMBER(12),
+    event_actual_id NUMBER(12),
+    priority NUMBER(12),
+    last_processed_at DATE DEFAULT SYS_EXTRACT_UTC(systimestamp(0)),
+    updated_at DATE DEFAULT SYS_EXTRACT_UTC(systimestamp(0)),
+    CONSTRAINT EVENTS_PR_PK PRIMARY KEY (event_type, event_actual_id) -- USING INDEX LOCAL,
+);
+
+
+--- 2023.03.16
+alter table HEALTH add (status NUMBER(2));
+alter table contents_update add content_metadata CLOB;
+alter table health modify payload VARCHAR2(2048);
+
+
+--- 2023.03.29
+alter table contents_update add fetch_status NUMBER(2) DEFAULT 0;
```

### Comparing `idds-server-1.1.5/lib/idds/agents/carrier/finisher.py` & `idds-server-1.2.0/lib/idds/agents/carrier/finisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
-# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2022
+# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
 import traceback
 
-from idds.common.constants import (Sections, ProcessingStatus, ProcessingLocking)
+from idds.common.constants import (Sections, ReturnCode, ProcessingStatus, ProcessingLocking)
 from idds.common.utils import setup_logging, truncate_string
 from idds.agents.common.eventbus.event import (EventType,
                                                UpdateProcessingEvent,
                                                UpdateTransformEvent)
 
 from .utils import (handle_abort_processing,
                     handle_resume_processing,
@@ -77,37 +77,45 @@
             update_processing['parameters']['errors'].update(error)
             ret = {'update_processing': update_processing}
             return ret
         return None
 
     def process_sync_processing(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
                 self.logger.info("process_sync_processing: event: %s" % event)
                 pr = self.get_processing(processing_id=event._processing_id, locking=True)
                 if not pr:
                     self.logger.error("Cannot find processing for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(pr)
 
                     self.logger.info(log_pre + "process_sync_processing")
                     ret = self.handle_sync_processing(pr, log_prefix=log_pre)
-                    self.logger.info(log_pre + "process_sync_processing result: %s" % str(ret))
+                    ret_copy = {}
+                    for ret_key in ret:
+                        if ret_key != 'messages':
+                            ret_copy[ret_key] = ret[ret_key]
+                    self.logger.info(log_pre + "process_sync_processing result: %s" % str(ret_copy))
 
                     self.update_processing(ret, pr)
 
                     # no need to update transform
                     # self.logger.info(log_pre + "UpdateTransformEvent(transform_id: %s)" % pr['transform_id'])
                     # event = UpdateTransformEvent(publisher_id=self.id, transform_id=pr['transform_id'])
                     # self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def handle_terminated_processing(self, processing, log_prefix=""):
         """
         process terminated processing
         """
         try:
             processing, update_collections, messages = sync_processing(processing, self.agent_attributes, terminate=True, logger=self.logger, log_prefix=log_prefix)
@@ -131,44 +139,53 @@
             update_processing['parameters']['errors'].update(error)
             ret = {'update_processing': update_processing}
             return ret
         return None
 
     def process_terminated_processing(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
                 if event._counter > 3:
                     self.logger.warn("Event counter is bigger than 3, skip event: %s" % str(event))
                 else:
                     original_event = event
                     pr = self.get_processing(processing_id=event._processing_id, locking=True)
                     if not pr:
                         self.logger.error("Cannot find processing for event: %s" % str(event))
+                        pro_ret = ReturnCode.Locked.value
                     else:
                         log_pre = self.get_log_prefix(pr)
 
                         self.logger.info(log_pre + "process_terminated_processing")
                         ret = self.handle_terminated_processing(pr, log_prefix=log_pre)
-                        self.logger.info(log_pre + "process_terminated_processing result: %s" % str(ret))
+                        ret_copy = {}
+                        for ret_key in ret:
+                            if ret_key != 'messages':
+                                ret_copy[ret_key] = ret[ret_key]
+                        self.logger.info(log_pre + "process_terminated_processing result: %s" % str(ret_copy))
 
                         self.update_processing(ret, pr)
                         self.logger.info(log_pre + "UpdateTransformEvent(transform_id: %s)" % pr['transform_id'])
                         event = UpdateTransformEvent(publisher_id=self.id, transform_id=pr['transform_id'])
                         self.event_bus.send(event)
 
                         if pr['status'] not in [ProcessingStatus.Finished, ProcessingStatus.Failed, ProcessingStatus.SubFinished]:
                             # some files are missing, poll it.
                             self.logger.info(log_pre + "UpdateProcessingEvent(processing_id: %s)" % pr['processing_id'])
                             event = UpdateProcessingEvent(publisher_id=self.id, processing_id=pr['processing_id'], counter=original_event._counter + 1)
+                            event.set_terminating()
                             self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def handle_abort_processing(self, processing, log_prefix=""):
         """
         process abort processing
         """
         try:
             processing, update_collections, update_contents, messages = handle_abort_processing(processing, self.agent_attributes, logger=self.logger, log_prefix=log_prefix)
@@ -193,47 +210,56 @@
             update_processing['parameters']['errors'].update(error)
             ret = {'update_processing': update_processing}
             return ret
         return None
 
     def process_abort_processing(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
                 processing_status = [ProcessingStatus.Finished, ProcessingStatus.Failed,
                                      ProcessingStatus.Lost, ProcessingStatus.Cancelled,
                                      ProcessingStatus.Suspended, ProcessingStatus.Expired,
                                      ProcessingStatus.Broken]
 
                 pr = self.get_processing(processing_id=event._processing_id, locking=True)
 
                 if not pr:
                     self.logger.error("Cannot find processing for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(pr)
                     self.logger.info(log_pre + "process_abort_processing")
 
                     if pr and pr['status'] in processing_status:
                         update_processing = {'processing_id': pr['processing_id'],
                                              'parameters': {'locking': ProcessingLocking.Idle,
                                                             'errors': {'abort_err': {'msg': truncate_string("Processing is already terminated. Cannot be aborted", length=200)}}}}
                         ret = {'update_processing': update_processing}
                         self.logger.info(log_pre + "process_abort_processing result: %s" % str(ret))
                         self.update_processing(ret, pr)
                     elif pr:
                         ret = self.handle_abort_processing(pr, log_prefix=log_pre)
-                        self.logger.info(log_pre + "process_abort_processing result: %s" % str(ret))
+                        ret_copy = {}
+                        for ret_key in ret:
+                            if ret_key != 'messages':
+                                ret_copy[ret_key] = ret[ret_key]
+                        self.logger.info(log_pre + "process_abort_processing result: %s" % str(ret_copy))
+
                         self.update_processing(ret, pr)
                         self.logger.info(log_pre + "UpdateTransformEvent(transform_id: %s)" % pr['transform_id'])
                         event = UpdateTransformEvent(publisher_id=self.id, transform_id=pr['transform_id'], content=event._content)
                         self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def handle_resume_processing(self, processing, log_prefix=""):
         """
         process resume processing
         """
         try:
             processing, update_collections, update_contents = handle_resume_processing(processing, self.agent_attributes, logger=self.logger, log_prefix=log_prefix)
@@ -257,22 +283,24 @@
             update_processing['parameters']['errors'].update(error)
             ret = {'update_processing': update_processing}
             return ret
         return None
 
     def process_resume_processing(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
                 processing_status = [ProcessingStatus.Finished]
 
                 pr = self.get_processing(processing_id=event._processing_id, locking=True)
 
                 if not pr:
                     self.logger.error("Cannot find processing for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(pr)
                     self.logger.info(log_pre + "process_resume_processing")
 
                     if pr and pr['status'] in processing_status:
                         update_processing = {'processing_id': pr['processing_id'],
                                              'parameters': {'locking': ProcessingLocking.Idle,
@@ -290,15 +318,17 @@
 
                         self.logger.info(log_pre + "UpdateTransformEvent(transform_id: %s)" % pr['transform_id'])
                         event = UpdateTransformEvent(publisher_id=self.id, transform_id=pr['transform_id'], content=event._content)
                         self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def init_event_function_map(self):
         self.event_func_map = {
             EventType.SyncProcessing: {
                 'pre_check': self.is_ok_to_run_more_processings,
                 'exec_func': self.process_sync_processing
             },
@@ -318,14 +348,15 @@
 
     def run(self):
         """
         Main run function.
         """
         try:
             self.logger.info("Starting main thread")
+            self.init_thread_info()
 
             self.load_plugins()
             self.init()
 
             self.add_default_tasks()
 
             self.init_event_function_map()
```

### Comparing `idds-server-1.1.5/lib/idds/agents/carrier/poller.py` & `idds-server-1.2.0/lib/idds/agents/carrier/poller.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 import datetime
 import random
 import time
 import traceback
 
 from idds.common import exceptions
-from idds.common.constants import Sections, ProcessingStatus, ProcessingLocking
-from idds.common.utils import setup_logging, truncate_string
+from idds.common.constants import Sections, ReturnCode, ProcessingStatus, ProcessingLocking
+from idds.common.utils import setup_logging, truncate_string, json_dumps
 from idds.core import processings as core_processings
 from idds.agents.common.baseagent import BaseAgent
 from idds.agents.common.eventbus.event import (EventType,
                                                UpdateProcessingEvent,
                                                TriggerProcessingEvent,
                                                SyncProcessingEvent,
                                                TerminatedProcessingEvent)
@@ -229,14 +229,15 @@
                         else:
                             # self.logger.error(ex)
                             # self.logger.error(traceback.format_exc())
                             raise ex
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            self.logger.warn("Failed to update_processings: %s" % json_dumps(processing))
             try:
                 processing_id = processing['update_processing']['processing_id']
 
                 parameters = {'status': processing['update_processing']['parameters']['status'],
                               'locking': ProcessingLocking.Idle}
                 if 'new_retries' in processing['update_processing']['parameters']:
                     parameters['new_retries'] = processing['update_processing']['parameters']['new_retries']
@@ -355,22 +356,24 @@
 
             ret = {'update_processing': update_processing,
                    'update_contents': []}
         return ret
 
     def process_update_processing(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
                 original_event = event
                 self.logger.info("process_update_processing, event: %s" % str(event))
 
                 pr = self.get_processing(processing_id=event._processing_id, status=None, locking=True)
                 if not pr:
                     self.logger.error("Cannot find processing for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(pr)
 
                     self.logger.info(log_pre + "process_update_processing")
                     ret = self.handle_update_processing(pr)
                     # self.logger.info(log_pre + "process_update_processing result: %s" % str(ret))
 
@@ -378,37 +381,42 @@
 
                     if 'processing_status' in ret and ret['processing_status'] == ProcessingStatus.Triggering:
                         event_content = {}
                         if (('update_contents' in ret and ret['update_contents']) or ('new_contents' in ret and ret['new_contents'])):
                             event_content['has_updates'] = True
                         if is_process_terminated(pr['substatus']):
                             event_content['Terminated'] = True
+                            event_content['is_terminating'] = True
                         self.logger.info(log_pre + "TriggerProcessingEvent(processing_id: %s)" % pr['processing_id'])
                         event = TriggerProcessingEvent(publisher_id=self.id, processing_id=pr['processing_id'], content=event_content,
                                                        counter=original_event._counter)
                         self.event_bus.send(event)
                     elif 'processing_status' in ret and ret['processing_status'] == ProcessingStatus.Terminating:
                         self.logger.info(log_pre + "TerminatedProcessingEvent(processing_id: %s)" % pr['processing_id'])
                         event = TerminatedProcessingEvent(publisher_id=self.id, processing_id=pr['processing_id'],
                                                           counter=original_event._counter)
+                        event.set_terminating()
                         self.event_bus.send(event)
                     else:
                         if (('update_contents' in ret and ret['update_contents'])
                             or ('new_contents' in ret and ret['new_contents'])       # noqa W503
                             or ('new_contents_ext' in ret and ret['new_contents_ext'])       # noqa W503
                             or ('update_contents_ext' in ret and ret['update_contents_ext'])       # noqa W503
                             or ('messages' in ret and ret['messages'])):             # noqa E129
                             self.logger.info(log_pre + "SyncProcessingEvent(processing_id: %s)" % pr['processing_id'])
                             event = SyncProcessingEvent(publisher_id=self.id, processing_id=pr['processing_id'],
                                                         counter=original_event._counter)
+                            event.set_has_updates()
                             self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def clean_locks(self):
         self.logger.info("clean locking")
         core_processings.clean_locking()
 
     def init_event_function_map(self):
         self.event_func_map = {
@@ -420,14 +428,15 @@
 
     def run(self):
         """
         Main run function.
         """
         try:
             self.logger.info("Starting main thread")
+            self.init_thread_info()
 
             self.load_plugins()
             self.init()
 
             self.add_default_tasks()
 
             self.init_event_function_map()
```

### Comparing `idds-server-1.1.5/lib/idds/agents/carrier/submitter.py` & `idds-server-1.2.0/lib/idds/agents/carrier/submitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,18 +155,20 @@
                     # self.logger.info(log_pre + "process_new_processing result: %s" % str(ret))
 
                     self.update_processing(ret, pr)
 
                     self.logger.info(log_pre + "UpdateTransformEvent(transform_id: %s)" % pr['transform_id'])
                     submit_event_content = {'event': 'submitted'}
                     event = UpdateTransformEvent(publisher_id=self.id, transform_id=pr['transform_id'], content=submit_event_content)
+                    event.set_has_updates()
                     self.event_bus.send(event)
 
                     self.logger.info(log_pre + "SyncProcessingEvent(processing_id: %s)" % pr['processing_id'])
                     event = SyncProcessingEvent(publisher_id=self.id, processing_id=pr['processing_id'])
+                    event.set_has_updates()
                     self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
         self.number_workers -= 1
 
     def init_event_function_map(self):
@@ -179,14 +181,15 @@
 
     def run(self):
         """
         Main run function.
         """
         try:
             self.logger.info("Starting main thread")
+            self.init_thread_info()
 
             self.load_plugins()
             self.init()
 
             self.add_default_tasks()
 
             self.init_event_function_map()
```

### Comparing `idds-server-1.1.5/lib/idds/agents/carrier/trigger.py` & `idds-server-1.2.0/lib/idds/agents/carrier/trigger.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 #
 # Authors:
 # - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
 import traceback
 
 from idds.common import exceptions
-from idds.common.constants import ProcessingStatus, ProcessingLocking
+from idds.common.constants import ProcessingStatus, ProcessingLocking, ReturnCode
 from idds.common.utils import setup_logging, truncate_string
-from idds.core import catalog as core_catalog
 from idds.core import processings as core_processings
 from idds.agents.common.eventbus.event import (EventType,
                                                UpdateTransformEvent,
                                                TriggerProcessingEvent,
                                                TerminatedProcessingEvent,
                                                SyncProcessingEvent)
 
-from .utils import handle_trigger_processing, is_process_terminated
+from .utils import (handle_trigger_processing,
+                    is_process_terminated)
 from .poller import Poller
 
 setup_logging(__name__)
 
 
 class Trigger(Poller):
     """
@@ -162,41 +162,44 @@
             update_processing['parameters'] = self.load_poll_period(processing, update_processing['parameters'])
 
             ret = {'update_processing': update_processing,
                    'update_contents': []}
         return ret
 
     def process_trigger_processing_real(self, event):
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
                 original_event = event
                 # pr_status = [ProcessingStatus.New]
                 self.logger.info("process_trigger_processing, event: %s" % str(event))
                 pr = self.get_processing(processing_id=event._processing_id, status=None, locking=True)
                 if not pr:
                     self.logger.error("Cannot find processing for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(pr)
                     self.logger.info(log_pre + "process_trigger_processing")
                     ret = self.handle_trigger_processing(pr)
                     # self.logger.info(log_pre + "process_trigger_processing result: %s" % str(ret))
 
-                    new_update_contents = ret.get('new_update_contents', None)
+                    # new_update_contents = ret.get('new_update_contents', None)
                     ret['new_update_contents'] = None
-                    ret_update_contents = ret.get('update_contents', None)
+                    # ret_update_contents = ret.get('update_contents', None)
                     self.update_processing(ret, pr)
 
-                    if new_update_contents or ret_update_contents:
+                    update_transforms = ret.get('update_transforms', None)
+                    if update_transforms:
                         # self.logger.info(log_pre + "update_contents_to_others_by_dep_id")
                         # core_catalog.update_contents_to_others_by_dep_id(request_id=pr['request_id'], transform_id=pr['transform_id'])
                         # self.logger.info(log_pre + "update_contents_to_others_by_dep_id done")
 
                         # core_catalog.delete_contents_update(request_id=pr['request_id'], transform_id=pr['transform_id'])
-                        update_transforms = core_catalog.get_updated_transforms_by_content_status(request_id=pr['request_id'],
-                                                                                                  transform_id=pr['transform_id'])
+                        # update_transforms = get_updated_transforms_by_content_status(request_id=pr['request_id'],
+                        #                                                              transform_id=pr['transform_id'])
                         self.logger.info(log_pre + "update_transforms: %s" % str(update_transforms))
                         for update_transform in update_transforms:
                             if 'transform_id' in update_transform:
                                 update_transform_id = update_transform['transform_id']
                                 if update_transform_id != pr['transform_id']:
                                     event = UpdateTransformEvent(publisher_id=self.id,
                                                                  transform_id=update_transform_id,
@@ -207,37 +210,43 @@
                     if (('processing_status' in ret and ret['processing_status'] == ProcessingStatus.Terminating)
                         or (event._content and 'Terminated' in event._content and event._content['Terminated'])):   # noqa W503
                         self.logger.info(log_pre + "TerminatedProcessingEvent(processing_id: %s)" % pr['processing_id'])
                         event = TerminatedProcessingEvent(publisher_id=self.id,
                                                           processing_id=pr['processing_id'],
                                                           content=event._content,
                                                           counter=original_event._counter)
+                        event.set_terminating()
                         self.event_bus.send(event)
                     else:
                         if ((event._content and 'has_updates' in event._content and event._content['has_updates'])
                             or ('update_contents' in ret and ret['update_contents'])    # noqa W503
                             or ('new_contents' in ret and ret['new_contents'])          # noqa W503
                             or ('messages' in ret and ret['messages'])):                # noqa E129
                             self.logger.info(log_pre + "SyncProcessingEvent(processing_id: %s)" % pr['processing_id'])
                             event = SyncProcessingEvent(publisher_id=self.id, processing_id=pr['processing_id'],
+                                                        content=event._content,
                                                         counter=original_event._counter)
                             self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
+        return pro_ret
 
     def process_trigger_processing(self, event):
         self.number_workers += 1
-        self.process_trigger_processing_real(event)
+        ret = self.process_trigger_processing_real(event)
         self.number_workers -= 1
+        return ret
 
     def process_msg_trigger_processing(self, event):
         self.number_msg_workers += 1
-        self.process_trigger_processing_real(event)
+        ret = self.process_trigger_processing_real(event)
         self.number_msg_workers -= 1
+        return ret
 
     def init_event_function_map(self):
         self.event_func_map = {
             EventType.TriggerProcessing: {
                 'pre_check': self.is_ok_to_run_more_processings,
                 'exec_func': self.process_trigger_processing
             },
@@ -249,14 +258,15 @@
 
     def run(self):
         """
         Main run function.
         """
         try:
             self.logger.info("Starting main thread")
+            self.init_thread_info()
 
             self.load_plugins()
             self.init()
 
             self.add_default_tasks()
 
             self.init_event_function_map()
```

### Comparing `idds-server-1.1.5/lib/idds/agents/carrier/utils.py` & `idds-server-1.2.0/lib/idds/agents/carrier/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -966,14 +966,40 @@
         msgs = generate_messages(request_id, transform_id, workload_id, work, msg_type='file',
                                  files=updated_contents_full, relation_type='output')
         ret_msgs = ret_msgs + msgs
 
     return process_status, new_contents, new_input_dependency_contents, ret_msgs, content_updates + content_updates_missing, parameters, new_contents_ext, update_contents_ext
 
 
+def get_transform_id_dependency_map(transform_id, logger=None, log_prefix=''):
+    cache = get_redis_cache()
+    transform_id_dependcy_map_key = "transform_id_dependcy_map_%s" % transform_id
+    transform_id_dependcy_map = cache.get(transform_id_dependcy_map_key, default=[])
+    return transform_id_dependcy_map
+
+
+def set_transform_id_dependency_map(transform_id, transform_id_dependcy_map, logger=None, log_prefix=''):
+    cache = get_redis_cache()
+    transform_id_dependcy_map_key = "transform_id_dependcy_map_%s" % transform_id
+    cache.set(transform_id_dependcy_map_key, transform_id_dependcy_map)
+
+
+def get_updated_transforms_by_content_status(request_id=None, transform_id=None, logger=None, log_prefix=''):
+    logger = get_logger(logger)
+    logger.debug("get_updated_transforms_by_content_status starts")
+
+    update_transforms = get_transform_id_dependency_map(transform_id=transform_id, logger=logger, log_prefix=log_prefix)
+    if not update_transforms:
+        update_transforms = core_catalog.get_updated_transforms_by_content_status(request_id=request_id,
+                                                                                  transform_id=transform_id)
+        set_transform_id_dependency_map(transform_id, update_transforms, logger=logger, log_prefix=log_prefix)
+    logger.debug("get_updated_transforms_by_content_status ends")
+    return update_transforms
+
+
 def handle_trigger_processing(processing, agent_attributes, trigger_new_updates=False, logger=None, log_prefix=''):
     logger = get_logger(logger)
 
     ret_msgs = []
     content_updates = []
     ret_update_transforms = []
 
@@ -990,16 +1016,35 @@
     else:
         if trigger_new_updates:
             # delete information in the contents_update table, to invoke the trigger.
             # ret_update_transforms = core_catalog.delete_contents_update(request_id=request_id, transform_id=transform_id)
             # logger.debug(log_prefix + "delete_contents_update: %s" % str(ret_update_transforms))
             pass
 
+        logger.debug(log_prefix + "sync contents_update to contents")
+        core_catalog.set_fetching_contents_update(request_id=request_id, transform_id=transform_id, fetch=True)
+        contents_update_list = core_catalog.get_contents_update(request_id=request_id, transform_id=transform_id, fetch=True)
+        new_contents_update_list = []
+        # contents_id_list = []
+        for con in contents_update_list:
+            con_dict = {'content_id': con['content_id'],
+                        'substatus': con['substatus']}
+            if 'content_metadata' in con and con['content_metadata']:
+                con_dict['content_metadata'] = con['content_metadata']
+            new_contents_update_list.append(con_dict)
+            # contents_id_list.append(con['content_id'])
+        core_catalog.update_contents(new_contents_update_list)
+        # core_catalog.delete_contents_update(contents=contents_id_list)
+        core_catalog.delete_contents_update(request_id=request_id, transform_id=transform_id, fetch=True)
+        logger.debug(log_prefix + "sync contents_update to contents done")
+
         logger.debug(log_prefix + "update_contents_from_others_by_dep_id")
-        core_catalog.update_contents_from_others_by_dep_id(request_id=request_id, transform_id=transform_id)
+        # core_catalog.update_contents_from_others_by_dep_id(request_id=request_id, transform_id=transform_id)
+        to_triggered_contents = core_catalog.get_update_contents_from_others_by_dep_id(request_id=request_id, transform_id=transform_id)
+        core_catalog.update_contents(to_triggered_contents)
         logger.debug(log_prefix + "update_contents_from_others_by_dep_id done")
 
         input_output_maps = get_input_output_maps(transform_id, work)
         logger.debug(log_prefix + "input_output_maps.keys[:2]: %s" % str(list(input_output_maps.keys())[:2]))
 
         updated_contents_ret = get_updated_contents_by_input_output_maps(input_output_maps=input_output_maps, logger=logger, log_prefix=log_prefix)
 
@@ -1015,14 +1060,19 @@
             # if the content is updated by receiver, here is the place to broadcast the messages
             msgs = generate_messages(request_id, transform_id, workload_id, work, msg_type='file',
                                      files=updated_contents_full_output, relation_type='output')
             ret_msgs = ret_msgs + msgs
 
         content_updates = content_updates + updated_contents
 
+        if content_updates or new_update_contents:
+            ret_update_transforms = get_updated_transforms_by_content_status(request_id=request_id,
+                                                                             transform_id=transform_id,
+                                                                             logger=logger,
+                                                                             log_prefix=log_prefix)
     # update_dep_contents_status_name = {}
     # update_dep_contents_status = {}
     # for content in new_update_contents:
     #     if content['substatus'] not in update_dep_contents_status_name:
     #         update_dep_contents_status_name[content['substatus'].name] = content['substatus']
     #         update_dep_contents_status[content['substatus'].name] = []
     #     update_dep_contents_status[content['substatus'].name].append(content['content_id'])
@@ -1145,27 +1195,34 @@
         return None
     else:
         workload_id_lock.release()
 
     return workload_id_transform_id_map[workload_id_str]
 
 
+content_id_lock = threading.Lock()
+
+
 def get_input_name_content_id_map(request_id, workload_id, transform_id):
     cache = get_redis_cache()
     input_name_content_id_map_key = "transform_input_contentid_map_%s" % transform_id
     input_name_content_id_map = cache.get(input_name_content_id_map_key, default={})
 
     if not input_name_content_id_map:
+        content_id_lock.acquire()
+
         contents = core_catalog.get_contents_by_request_transform(request_id=request_id, transform_id=transform_id)
         input_name_content_id_map = {}
         for content in contents:
             if content['content_relation_type'] == ContentRelationType.Output:
                 input_name_content_id_map[content['name']] = content['content_id']
 
         cache.set(input_name_content_id_map_key, input_name_content_id_map)
+
+        content_id_lock.release()
     return input_name_content_id_map
 
 
 def get_jobid_content_id_map(request_id, workload_id, transform_id, job_id, inputs):
     cache = get_redis_cache()
     jobid_content_id_map_key = "transform_jobid_contentid_map_%s" % transform_id
     jobid_content_id_map = cache.get(jobid_content_id_map_key, default={})
@@ -1247,39 +1304,40 @@
         ret = True
 
     keys = list(update_processing_map.keys())
     for key in keys:
         if update_processing_map[key] + 86400 < time.time():
             del update_processing_map[key]
 
-    cache.set(update_processing_map_key, default=update_processing_map)
+    cache.set(update_processing_map_key, update_processing_map, expire_seconds=86400)
     update_processing_lock.release()
     return ret
 
 
 def handle_messages_processing(messages, logger=None, log_prefix='', update_processing_interval=300):
     logger = get_logger(logger)
     if not log_prefix:
         log_prefix = "<Message>"
 
     update_processings = []
+    update_processings_by_job = []
     terminated_processings = []
     update_contents = []
 
     for ori_msg in messages:
         msg = json.loads(ori_msg)
         if 'taskid' not in msg or not msg['taskid']:
             continue
 
-        logger.debug(log_prefix + "Received message: %s" % str(ori_msg))
-
         if msg['msg_type'] in ['task_status']:
             workload_id = msg['taskid']
             status = msg['status']
-            if status in ['pending']:   # 'prepared'
+            if status in ['pending1']:   # 'prepared'
+                logger.debug(log_prefix + "Received message: %s" % str(ori_msg))
+
                 ret_req_tf_pr_id = get_workload_id_transform_id_map(workload_id, logger=logger, log_prefix=log_prefix)
                 if not ret_req_tf_pr_id:
                     # request is submitted by some other instances
                     logger.debug(log_prefix + "No matched workload_id, discard message: %s" % str(ori_msg))
                     continue
 
                 logger.debug(log_prefix + "(request_id, transform_id, processing_id, status, substatus): %s" % str(ret_req_tf_pr_id))
@@ -1288,14 +1346,16 @@
                     # new_processings.append((req_id, tf_id, processing_id, workload_id, status))
                     if processing_id not in update_processings:
                         update_processings.append(processing_id)
                         logger.debug(log_prefix + "Add to update processing: %s" % str(processing_id))
                 else:
                     logger.debug(log_prefix + "Processing %s is already processed, not add it to update processing" % (str(processing_id)))
             elif status in ['finished', 'done']:
+                logger.debug(log_prefix + "Received message: %s" % str(ori_msg))
+
                 ret_req_tf_pr_id = get_workload_id_transform_id_map(workload_id, logger=logger, log_prefix=log_prefix)
                 if not ret_req_tf_pr_id:
                     # request is submitted by some other instances
                     logger.debug(log_prefix + "No matched workload_id, discard message: %s" % str(ori_msg))
                     continue
 
                 logger.debug(log_prefix + "(request_id, transform_id, processing_id, status, substatus): %s" % str(ret_req_tf_pr_id))
@@ -1307,46 +1367,55 @@
 
         if msg['msg_type'] in ['job_status']:
             workload_id = msg['taskid']
             job_id = msg['jobid']
             status = msg['status']
             inputs = msg['inputs']
             if inputs and status in ['finished']:
+                logger.debug(log_prefix + "Received message: %s" % str(ori_msg))
+
                 ret_req_tf_pr_id = get_workload_id_transform_id_map(workload_id, logger=logger, log_prefix=log_prefix)
                 if not ret_req_tf_pr_id:
                     # request is submitted by some other instances
                     logger.debug(log_prefix + "No matched workload_id, discard message: %s" % str(ori_msg))
                     continue
 
                 logger.debug(log_prefix + "(request_id, transform_id, processing_id, status, substatus): %s" % str(ret_req_tf_pr_id))
 
                 req_id, tf_id, processing_id, r_status, r_substatus = ret_req_tf_pr_id
                 content_id, to_update_jobid = get_content_id_from_job_id(req_id, workload_id, tf_id, job_id, inputs)
                 if content_id:
                     if to_update_jobid:
                         u_content = {'content_id': content_id,
+                                     'request_id': req_id,
+                                     'transform_id': tf_id,
+                                     'workload_id': workload_id,
                                      # 'status': get_content_status_from_panda_msg_status(status),
                                      'substatus': get_content_status_from_panda_msg_status(status),
                                      'content_metadata': {'panda_id': job_id}}
                     else:
                         u_content = {'content_id': content_id,
+                                     'request_id': req_id,
+                                     'transform_id': tf_id,
+                                     'workload_id': workload_id,
                                      'substatus': get_content_status_from_panda_msg_status(status)}
                         #             # 'status': get_content_status_from_panda_msg_status(status)}
 
                     update_contents.append(u_content)
                     # if processing_id not in update_processings:
-                    if processing_id not in update_processings and whether_to_update_processing(processing_id, update_processing_interval):
-                        update_processings.append(processing_id)
-                        logger.debug(log_prefix + "Add to update processing: %s" % str(processing_id))
+                    # if processing_id not in update_processings and whether_to_update_processing(processing_id, update_processing_interval):
+                    if processing_id not in update_processings_by_job:
+                        update_processings_by_job.append(processing_id)
+                        logger.debug(log_prefix + "Add to update processing by job: %s" % str(processing_id))
 
-    return update_processings, terminated_processings, update_contents, []
+    return update_processings, update_processings_by_job, terminated_processings, update_contents, []
 
 
 def sync_collection_status(request_id, transform_id, workload_id, work, input_output_maps=None,
-                           close_collection=False, force_close_collection=False, terminate=False):
+                           close_collection=False, force_close_collection=False, abort=False, terminate=False):
     if input_output_maps is None:
         input_output_maps = get_input_output_maps(transform_id, work)
 
     all_updates_flushed = True
     coll_status = {}
     messages = []
     for map_id in input_output_maps:
@@ -1387,15 +1456,16 @@
         for content in contents_ext:
             coll_status[content['coll_id']]['ext_files'] += 1
 
             if content['status'] in [ContentStatus.Available, ContentStatus.Mapped,
                                      ContentStatus.Available.value, ContentStatus.Mapped.value,
                                      ContentStatus.FakeAvailable, ContentStatus.FakeAvailable.value]:
                 coll_status[content['coll_id']]['processed_ext_files'] += 1
-            elif content['status'] in [ContentStatus.Failed, ContentStatus.FinalFailed]:
+            # elif content['status'] in [ContentStatus.Failed, ContentStatus.FinalFailed]:
+            elif content['status'] in [ContentStatus.FinalFailed]:
                 coll_status[content['coll_id']]['failed_ext_files'] += 1
             elif content['status'] in [ContentStatus.Lost, ContentStatus.Deleted, ContentStatus.Missing]:
                 coll_status[content['coll_id']]['missing_ext_files'] += 1
 
     input_collections = work.get_input_collections(poll_externel=True)
     output_collections = work.get_output_collections()
     log_collections = work.get_log_collections()
@@ -1452,24 +1522,34 @@
                     coll.status = CollectionStatus.Closed
                     coll.substatus = CollectionStatus.Closed
 
                     msgs = generate_messages(request_id, transform_id, workload_id, work, msg_type='collection', files=[coll], relation_type='input')
                     messages += msgs
 
         if terminate:
-            if coll in output_collections and work.require_ext_contents():
-                if coll.processed_files == coll.processed_ext_files and coll.failed_files == coll.failed_ext_files:
+            all_files_monitored = False
+            if coll.total_files == coll.processed_files + coll.failed_files + coll.missing_files:
+                all_files_monitored = True
+
+            if abort:
+                u_coll['status'] = CollectionStatus.Closed
+                u_coll['substatus'] = CollectionStatus.Closed
+                coll.status = CollectionStatus.Closed
+                coll.substatus = CollectionStatus.Closed
+            elif coll in output_collections:
+                if (not work.require_ext_contents() or (work.require_ext_contents()
+                    and coll.processed_files == coll.processed_ext_files and coll.failed_files == coll.failed_ext_files)):     # noqa E129, W503
                     all_ext_updated = True
-                if (force_close_collection or (close_collection and all_updates_flushed and all_ext_updated)
+                if (force_close_collection or (close_collection and all_updates_flushed and all_ext_updated and all_files_monitored)
                    or coll.status == CollectionStatus.Closed):        # noqa W503
                     u_coll['status'] = CollectionStatus.Closed
                     u_coll['substatus'] = CollectionStatus.Closed
                     coll.status = CollectionStatus.Closed
                     coll.substatus = CollectionStatus.Closed
-            elif force_close_collection or close_collection and all_updates_flushed or coll.status == CollectionStatus.Closed:
+            elif force_close_collection or (close_collection and all_updates_flushed and all_files_monitored) or coll.status == CollectionStatus.Closed:
                 u_coll['status'] = CollectionStatus.Closed
                 u_coll['substatus'] = CollectionStatus.Closed
                 coll.status = CollectionStatus.Closed
                 coll.substatus = CollectionStatus.Closed
 
         update_collections.append(u_coll)
     return update_collections, all_updates_flushed, messages
@@ -1497,41 +1577,41 @@
             work.status = WorkStatus.Finished
         elif is_all_files_failed:
             work.status = WorkStatus.Failed
         else:
             work.status = WorkStatus.SubFinished
 
 
-def sync_processing(processing, agent_attributes, terminate=False, logger=None, log_prefix=""):
+def sync_processing(processing, agent_attributes, terminate=False, abort=False, logger=None, log_prefix=""):
     logger = get_logger()
 
     request_id = processing['request_id']
     transform_id = processing['transform_id']
     workload_id = processing['workload_id']
 
     proc = processing['processing_metadata']['processing']
     work = proc.work
     work.set_agent_attributes(agent_attributes, processing)
 
     messages = []
     input_output_maps = get_input_output_maps(transform_id, work)
     update_collections, all_updates_flushed, msgs = sync_collection_status(request_id, transform_id, workload_id, work,
                                                                            input_output_maps=input_output_maps,
-                                                                           close_collection=True, terminate=terminate)
+                                                                           close_collection=True, abort=abort, terminate=terminate)
 
     messages += msgs
 
     sync_work_status(request_id, transform_id, workload_id, work)
     logger.info(log_prefix + "sync_processing: work status: %s" % work.get_status())
     if terminate and work.is_terminated():
         msgs = generate_messages(request_id, transform_id, workload_id, work, msg_type='work')
         messages += msgs
         if work.is_finished():
-            # processing['status'] = ProcessingStatus.Finished
-            processing['status'] = processing['substatus']
+            processing['status'] = ProcessingStatus.Finished
+            # processing['status'] = processing['substatus']
         elif work.is_subfinished():
             processing['status'] = ProcessingStatus.SubFinished
         elif work.is_failed():
             processing['status'] = ProcessingStatus.Failed
         else:
             processing['status'] = ProcessingStatus.SubFinished
 
@@ -1568,15 +1648,15 @@
     # update_collections, all_updates_flushed = sync_collection_status(request_id, transform_id, workload_id, work,
     #                                                                  input_output_maps=None, close_collection=True,
     #                                                                  force_close_collection=True)
 
     # for coll in input_collections + output_collections + log_collections:
     #     coll.status = CollectionStatus.Closed
     #     coll.substatus = CollectionStatus.Closed
-    processing, update_collections, messages = sync_processing(processing, agent_attributes, terminate=True, logger=logger, log_prefix=log_prefix)
+    processing, update_collections, messages = sync_processing(processing, agent_attributes, terminate=True, abort=True, logger=logger, log_prefix=log_prefix)
     update_contents = []
 
     # processing['status'] = ProcessingStatus.Cancelled
     return processing, update_collections, update_contents, messages
 
 
 def reactive_contents(request_id, transform_id, workload_id, work, input_output_maps):
```

### Comparing `idds-server-1.1.5/lib/idds/agents/clerk/clerk.py` & `idds-server-1.2.0/lib/idds/agents/clerk/clerk.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 import datetime
 import random
 import time
 import traceback
 
 from idds.common import exceptions
-from idds.common.constants import (Sections, RequestStatus, RequestLocking,
+from idds.common.constants import (Sections, ReturnCode,
+                                   RequestStatus, RequestLocking,
                                    TransformStatus, CommandType,
                                    CommandStatus, CommandLocking)
 from idds.common.utils import setup_logging, truncate_string
 from idds.core import (requests as core_requests,
                        transforms as core_transforms,
                        commands as core_commands)
 from idds.agents.common.baseagent import BaseAgent
@@ -771,26 +772,29 @@
             ret_req['parameters']['errors'].update(error)
             log_pre = self.get_log_prefix(req)
             self.logger.warn(log_pre + "Handle new request exception result: %s" % str(ret_req))
         return ret_req
 
     def process_update_request(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
-                req_status = [RequestStatus.Transforming, RequestStatus.ToCancel, RequestStatus.Cancelling,
-                              RequestStatus.ToSuspend, RequestStatus.Suspending,
-                              RequestStatus.ToExpire, RequestStatus.Expiring,
-                              RequestStatus.ToFinish, RequestStatus.ToForceFinish,
-                              RequestStatus.ToResume, RequestStatus.Resuming,
-                              RequestStatus.Building]
+                # req_status = [RequestStatus.Transforming, RequestStatus.ToCancel, RequestStatus.Cancelling,
+                #               RequestStatus.ToSuspend, RequestStatus.Suspending,
+                #               RequestStatus.ToExpire, RequestStatus.Expiring,
+                #               RequestStatus.ToFinish, RequestStatus.ToForceFinish,
+                #               RequestStatus.ToResume, RequestStatus.Resuming,
+                #               RequestStatus.Building]
 
-                req = self.get_request(request_id=event._request_id, status=req_status, locking=True)
+                # req = self.get_request(request_id=event._request_id, status=req_status, locking=True)
+                req = self.get_request(request_id=event._request_id, locking=True)
                 if not req:
                     self.logger.error("Cannot find request for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(req)
                     ret = self.handle_update_request(req, event=event)
                     new_tf_ids, update_tf_ids = self.update_request(ret)
                     for tf_id in new_tf_ids:
                         self.logger.info(log_pre + "NewTransformEvent(transform_id: %s)" % tf_id)
                         event = NewTransformEvent(publisher_id=self.id, transform_id=tf_id, content=event._content)
@@ -798,15 +802,17 @@
                     for tf_id in update_tf_ids:
                         self.logger.info(log_pre + "UpdateTransformEvent(transform_id: %s)" % tf_id)
                         event = UpdateTransformEvent(publisher_id=self.id, transform_id=tf_id, content=event._content)
                         self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def handle_abort_request(self, req, event):
         """
         process abort request
         """
         try:
             log_pre = self.get_log_prefix(req)
@@ -862,19 +868,21 @@
                          'locking': CommandLocking.Idle}
             if errors:
                 u_command['errors'] = errors
             core_commands.update_commands([u_command])
 
     def process_abort_request(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
                 req = self.get_request(request_id=event._request_id, locking=True)
                 if not req:
                     self.logger.error("Cannot find request for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(req)
                     self.logger.info(log_pre + "process_abort_request event: %s" % str(event))
 
                     if req['status'] in [RequestStatus.Finished, RequestStatus.SubFinished,
                                          RequestStatus.Failed, RequestStatus.Cancelled,
                                          RequestStatus.Suspended, RequestStatus.Expired]:
@@ -919,18 +927,21 @@
 
                         self.handle_command(event, cmd_status=CommandStatus.Processed, errors=None)
         except AssertionError as ex:
             self.logger.error("process_abort_request, Failed to process event: %s" % str(event))
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
             self.handle_command(event, cmd_status=CommandStatus.Processed, errors=str(ex))
+            pro_ret = ReturnCode.Failed.value
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def handle_resume_request(self, req):
         """
         process resume request
         """
         try:
             req_status = RequestStatus.Resuming
@@ -956,19 +967,21 @@
                                       'locking': RequestLocking.Idle,
                                       'errors': req['errors'] if req['errors'] else {}}}
             ret_req['parameters']['errors'].update(error)
         return ret_req
 
     def process_resume_request(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
                 req = self.get_request(request_id=event._request_id, locking=True)
                 if not req:
                     self.logger.error("Cannot find request for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(req)
                     self.logger.info(log_pre + "process_resume_request event: %s" % str(event))
 
                     if req['status'] in [RequestStatus.Finished]:
                         ret = {'request_id': req['request_id'],
                                'parameters': {'locking': RequestLocking.Idle,
@@ -999,15 +1012,17 @@
                             event = UpdateRequestEvent(publisher_id=self.id, request_id=req['request_id'], content=event._content)
                             self.event_bus.send(event)
 
                         self.handle_command(event, cmd_status=CommandStatus.Processed, errors=None)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def clean_locks(self):
         self.logger.info("clean locking")
         core_requests.clean_locking()
 
     def init_event_function_map(self):
         self.event_func_map = {
@@ -1035,14 +1050,15 @@
 
     def run(self):
         """
         Main run function.
         """
         try:
             self.logger.info("Starting main thread")
+            self.init_thread_info()
 
             self.load_plugins()
 
             self.add_default_tasks()
 
             self.init_event_function_map()
```

### Comparing `idds-server-1.1.5/lib/idds/agents/common/cache/redis.py` & `idds-server-1.2.0/lib/idds/agents/common/cache/redis.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/agents/common/eventbus/eventbus.py` & `idds-server-1.2.0/lib/idds/agents/common/eventbus/baseeventbusbackend.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,90 +2,112 @@
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
-# - Wen Guan, <wen.guan@cern.ch>, 2022
+# - Wen Guan, <wen.guan@cern.ch>, 2023
 
 import logging
+import time
+import threading
+import traceback
 import uuid
 
-from idds.common.constants import Sections
-from idds.common.config import config_has_section, config_list_options
+from .event import StateClaimEvent, EventBusState
 
-from .localeventbusbackend import LocalEventBusBackend
 
+class BaseEventBusBackend(threading.Thread):
+    """
+    Base Event Bus Backend
+    """
 
-class Singleton(object):
-    _instance = None
+    def __init__(self, logger=None, **kwargs):
+        super(BaseEventBusBackend, self).__init__()
+        self._id = str(uuid.uuid4())[:8]
+        self._state_claim_wait = 60
+        self._state_claim = StateClaimEvent(self._id, EventBusState.New, time.time())
 
-    def __new__(class_, *args, **kwargs):
-        if not isinstance(class_._instance, class_):
-            class_._instance = object.__new__(class_, *args, **kwargs)
-            class_._instance._initialized = False
-        return class_._instance
+        self.graceful_stop = threading.Event()
 
+        self._events = {}
+        self._events_index = {}
 
-class EventBus(Singleton):
-    """
-    Event Bus
-    """
+        self._lock = threading.RLock()
 
-    def __init__(self, logger=None):
-        if not self._initialized:
-            self._initialized = True
-
-            super(EventBus, self).__init__()
-            self._id = str(uuid.uuid4())[:8]
-            self.setup_logger(logger)
-            self.config_section = Sections.EventBus
-            attrs = self.load_attributes()
-            if 'backend' in attrs and attrs['backend'] == 'message':
-                # ToBeDone
-                # self.backend = MsgEventBusBackend(**attrs)
-                pass
-            else:
-                self.backend = LocalEventBusBackend(logger=self.logger, **attrs)
+        self.setup_logger(logger)
+
+        self.coordinator = None
 
     def setup_logger(self, logger=None):
         """
         Setup logger
         """
         if logger:
             self.logger = logger
         else:
             self.logger = logging.getLogger(self.get_class_name())
 
     def get_class_name(self):
         return self.__class__.__name__
 
-    def load_attributes(self):
-        self.logger.info("Loading config for section: %s" % self.config_section)
-        attrs = {}
-        if config_has_section(self.config_section):
-            options = config_list_options(self.config_section)
-            for option, value in options:
-                if isinstance(value, str) and value.lower() == 'true':
-                    value = True
-                if isinstance(value, str) and value.lower() == 'false':
-                    value = False
-                attrs[option] = value
-        return attrs
-
-    def publish_event(self, event):
-        self.backend.send(event)
-
-    def get_event(self, event_type):
-        # demand_event = DemandEvent(event._event_type, self._id)
-        event = self.backend.get(event_type, wait=10)
-        return event
-
-    def get(self, event_type):
-        return self.get_event(event_type)
+    def stop(self, signum=None, frame=None):
+        self.graceful_stop.set()
 
     def send(self, event):
-        return self.publish_event(event)
+        if self.get_coordinator():
+            return self.get_coordinator().send(event)
+        else:
+            with self._lock:
+                if event._event_type not in self._events:
+                    self._events[event._event_type] = {}
+                    self._events_index[event._event_type] = []
+                self._events[event._event_type][event._id] = event
+                self._events_index[event._event_type].append(event._id)
+
+    def get(self, event_type, wait=0):
+        if self.get_coordinator():
+            return self.get_coordinator().get(event_type, wait)
+        else:
+            with self._lock:
+                if event_type in self._events_index and self._events_index[event_type]:
+                    event_id = self._events_index[event_type].pop(0)
+                    event = self._events[event_type][event_id]
+                    del self._events[event_type][event_id]
+                    return event
+                return None
+
+    def send_report(self, event, status, start_time, end_time, source, result):
+        if self.get_coordinator():
+            return self.get_coordinator().send_report(event, status, start_time, end_time, source, result)
+
+    def clean_event(self, event):
+        pass
+
+    def fail_event(self, event):
+        pass
+
+    def set_manager(self, manager):
+        pass
+
+    def get_manager(self):
+        return None
+
+    def set_coordinator(self, coordinator):
+        self.coordinator = coordinator
+
+    def get_coordinator(self):
+        return self.coordinator
+
+    def is_ok(self):
+        return True
+
+    def execute(self):
+        while not self.graceful_stop.is_set():
+            try:
+                self.graceful_stop.wait(0.1)
+            except Exception as error:
+                self.logger.critical("Caught an exception: %s\n%s" % (str(error), traceback.format_exc()))
 
-    def stop(self):
-        self.backend.stop()
+    def run(self):
+        self.execute()
```

### Comparing `idds-server-1.1.5/lib/idds/agents/common/plugins/messaging.py` & `idds-server-1.2.0/lib/idds/agents/common/plugins/messaging.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
 # - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
 
 import logging
-import json
 import random
 import socket
 import threading
 import time
 import traceback
 import stomp
 
 from idds.common.plugin.plugin_base import PluginBase
-from idds.common.utils import setup_logging, get_logger
+from idds.common.utils import setup_logging, get_logger, json_dumps, json_loads
 
 
 setup_logging(__name__)
 logging.getLogger("stomp").setLevel(logging.CRITICAL)
 
 
 class MessagingListener(stomp.ConnectionListener):
@@ -65,15 +64,15 @@
         self.graceful_stop = threading.Event()
         self.request_queue = None
         self.output_queue = None
         self.response_queue = None
 
         if not hasattr(self, 'channels'):
             raise Exception('"channels" is required but not defined.')
-        self.channels = json.loads(self.channels)
+        self.channels = json_loads(self.channels)
 
         self.broker_timeout = 3600
 
         if not hasattr(self, 'timetolive'):
             self.timetolive = 12 * 3600 * 1000     # milliseconds
         else:
             self.timetolive = int(self.timetolive)
@@ -190,16 +189,16 @@
 
     def send_message(self, msg):
         destination = msg['destination'] if 'destination' in msg else 'default'
         conn, queue_dest, destination = self.get_connection(destination)
 
         if conn:
             self.logger.info("Sending message to message broker(%s): %s" % (destination, msg['msg_id']))
-            self.logger.debug("Sending message to message broker(%s): %s" % (destination, json.dumps(msg['msg_content'])))
-            conn.send(body=json.dumps(msg['msg_content']),
+            self.logger.debug("Sending message to message broker(%s): %s" % (destination, json_dumps(msg['msg_content'])))
+            conn.send(body=json_dumps(msg['msg_content']),
                       destination=queue_dest,
                       id='atlas-idds-messaging',
                       ack='auto',
                       headers={'persistent': 'true',
                                'ttl': self.timetolive,
                                'vo': 'atlas',
                                'msg_type': str(msg['msg_type']).lower()})
```

### Comparing `idds-server-1.1.5/lib/idds/agents/common/timerscheduler.py` & `idds-server-1.2.0/lib/idds/agents/common/timerscheduler.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,38 +2,68 @@
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
-# - Wen Guan, <wen.guan@cern.ch>, 2020
+# - Wen Guan, <wen.guan@cern.ch>, 2020 - 2023
 
 
 import heapq
 import threading
 import traceback
 from concurrent import futures
 
 from .timertask import TimerTask
 
 
+class IDDSThreadPoolExecutor(futures.ThreadPoolExecutor):
+    def __init__(self, max_workers=None, thread_name_prefix='',
+                 initializer=None, initargs=()):
+        self.futures = []
+        self._lock = threading.RLock()
+        super(IDDSThreadPoolExecutor, self).__init__(max_workers=max_workers,
+                                                     thread_name_prefix=thread_name_prefix,
+                                                     initializer=initializer,
+                                                     initargs=initargs)
+
+    def submit(self, fn, *args, **kwargs):
+        future = super(IDDSThreadPoolExecutor, self).submit(fn, *args, **kwargs)
+        with self._lock:
+            self.futures.append(future)
+        return future
+
+    def get_max_workers(self):
+        return self._max_workers
+
+    def get_num_workers(self):
+        with self._lock:
+            for future in self.futures.copy():
+                if future.done():
+                    self.futures.remove(future)
+            return len(self.futures)
+
+    def has_free_workers(self):
+        return self.get_num_workers() < self._max_workers
+
+
 class TimerScheduler(threading.Thread):
     """
     The base class to schedule Task which will be executed after some time
     """
 
     def __init__(self, num_threads, name=None, logger=None):
         super(TimerScheduler, self).__init__(name=name)
         self.num_threads = int(num_threads)
         if self.num_threads < 1:
             self.num_threads = 1
         self.graceful_stop = threading.Event()
-        self.executors = futures.ThreadPoolExecutor(max_workers=self.num_threads,
-                                                    thread_name_prefix=name)
+        self.executors = IDDSThreadPoolExecutor(max_workers=self.num_threads,
+                                                thread_name_prefix=name)
 
         self._task_queue = []
         self._lock = threading.RLock()
 
         self.logger = logger
 
     def set_logger(self, logger):
```

### Comparing `idds-server-1.1.5/lib/idds/agents/common/timertask.py` & `idds-server-1.2.0/lib/idds/agents/common/timertask.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/agents/conductor/conductor.py` & `idds-server-1.2.0/lib/idds/agents/conductor/conductor.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 class Conductor(BaseAgent):
     """
     Conductor works to notify workload management that the data is available.
     """
 
     def __init__(self, num_threads=1, retrieve_bulk_size=1000, threshold_to_release_messages=None,
-                 random_delay=None, delay=60, replay_times=3, **kwargs):
+                 random_delay=None, delay=60, interval_delay=10, replay_times=3, **kwargs):
         super(Conductor, self).__init__(num_threads=num_threads, name='Conductor', **kwargs)
         self.config_section = Sections.Conductor
         self.retrieve_bulk_size = int(retrieve_bulk_size)
         self.message_queue = Queue()
         self.output_message_queue = Queue()
         if threshold_to_release_messages is None:
             self.threshold_to_release_messages = None
@@ -51,14 +51,17 @@
                 self.random_delay = 5
         if delay is None:
             delay = 60
         self.delay = int(delay)
         if replay_times is None:
             replay_times = 3
         self.replay_times = int(replay_times)
+        if not interval_delay:
+            interval_delay = 10
+        self.interval_delay = int(interval_delay)
         self.logger = get_logger(self.__class__.__name__)
 
     def __del__(self):
         self.stop_notifier()
 
     def get_messages(self):
         """
@@ -131,27 +134,32 @@
 
     def run(self):
         """
         Main run function.
         """
         try:
             self.logger.info("Starting main thread")
+            self.init_thread_info()
             self.load_plugins()
 
+            self.add_default_tasks()
+
             self.start_notifier()
 
             # self.add_health_message_task()
 
             while not self.graceful_stop.is_set():
                 # execute timer task
-                self.execute_once()
+                self.execute_schedules()
 
                 try:
                     num_contents = 0
                     messages = self.get_messages()
+                    if not messages:
+                        time.sleep(self.interval_delay)
                     for message in messages:
                         message['destination'] = message['destination'].name
 
                         num_contents += message['num_contents']
                         self.message_queue.put(message)
                     while not self.message_queue.empty():
                         time.sleep(1)
```

### Comparing `idds-server-1.1.5/lib/idds/agents/conductor/consumer.py` & `idds-server-1.2.0/lib/idds/agents/conductor/consumer.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/agents/main.py` & `idds-server-1.2.0/lib/idds/agents/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
-# - Wen Guan, <wen.guan@cern.ch>, 2019
+# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
 """
 Main start entry point for iDDS service
 """
 
 
 import logging
@@ -34,15 +34,17 @@
     'transporter': ['idds.agents.transporter.transporter.Transporter', Sections.Transporter],
     'submitter': ['idds.agents.carrier.submitter.Submitter', Sections.Carrier],
     'poller': ['idds.agents.carrier.poller.Poller', Sections.Carrier],
     'receiver': ['idds.agents.carrier.receiver.Receiver', Sections.Carrier],
     'trigger': ['idds.agents.carrier.trigger.Trigger', Sections.Carrier],
     'finisher': ['idds.agents.carrier.finisher.Finisher', Sections.Carrier],
     'conductor': ['idds.agents.conductor.conductor.Conductor', Sections.Conductor],
-    'consumer': ['idds.agents.conductor.consumer.Consumer', Sections.Consumer]
+    'consumer': ['idds.agents.conductor.consumer.Consumer', Sections.Consumer],
+    'archiver': ['idds.agents.archive.archiver.Archiver', Sections.Archiver],
+    'coordinator': ['idds.agents.coordinator.coordinator.Coordinator', Sections.Coordinator]
 }
 
 RUNNING_AGENTS = []
 
 
 def load_config_agents():
     if config_has_section(Sections.Main) and config_has_option(Sections.Main, 'agents'):
```

### Comparing `idds-server-1.1.5/lib/idds/agents/marshaller/marshaller.py` & `idds-server-1.2.0/lib/idds/agents/marshaller/marshaller.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/agents/transformer/transformer.py` & `idds-server-1.2.0/lib/idds/agents/transformer/transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import copy
 import datetime
 import random
 import time
 import traceback
 
 from idds.common import exceptions
-from idds.common.constants import (Sections, TransformStatus, TransformLocking,
+from idds.common.constants import (Sections, ReturnCode,
+                                   TransformStatus, TransformLocking,
                                    CommandType, ProcessingStatus)
 from idds.common.utils import setup_logging, truncate_string
 from idds.core import (transforms as core_transforms,
                        processings as core_processings)
 from idds.agents.common.baseagent import BaseAgent
 from idds.agents.common.eventbus.event import (EventType,
                                                NewTransformEvent,
@@ -521,25 +522,28 @@
 
             ret = {'transform': transform, 'transform_parameters': transform_parameters}
             self.logger.warn(log_pre + "handle_update_transform exception result: %s" % str(ret))
         return ret, False, None
 
     def process_update_transform(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
-                tf_status = [TransformStatus.Transforming,
-                             TransformStatus.ToCancel, TransformStatus.Cancelling,
-                             TransformStatus.ToSuspend, TransformStatus.Suspending,
-                             TransformStatus.ToExpire, TransformStatus.Expiring,
-                             TransformStatus.ToResume, TransformStatus.Resuming,
-                             TransformStatus.ToFinish, TransformStatus.ToForceFinish]
-                tf = self.get_transform(transform_id=event._transform_id, status=tf_status, locking=True)
+                # tf_status = [TransformStatus.Transforming,
+                #              TransformStatus.ToCancel, TransformStatus.Cancelling,
+                #              TransformStatus.ToSuspend, TransformStatus.Suspending,
+                #              TransformStatus.ToExpire, TransformStatus.Expiring,
+                #              TransformStatus.ToResume, TransformStatus.Resuming,
+                #              TransformStatus.ToFinish, TransformStatus.ToForceFinish]
+                # tf = self.get_transform(transform_id=event._transform_id, status=tf_status, locking=True)
+                tf = self.get_transform(transform_id=event._transform_id, locking=True)
                 if not tf:
                     self.logger.error("Cannot find transform for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(tf)
 
                     ret, is_terminated, ret_processing_id = self.handle_update_transform(tf, event)
                     new_pr_ids, update_pr_ids = self.update_transform(ret)
 
                     if is_terminated or (event._content and 'event' in event._content and event._content['event'] == 'submitted'):
@@ -557,15 +561,17 @@
                     if ret_processing_id and (event._content and 'event' in event._content and event._content['event'] == 'Trigger'):
                         self.logger.info(log_pre + "UpdateProcessingEvent(processing_id: %s)" % ret_processing_id)
                         event = UpdateProcessingEvent(publisher_id=self.id, processing_id=ret_processing_id)
                         self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def handle_abort_transform(self, transform):
         """
         process abort transform
         """
         try:
             work = transform['transform_metadata']['work']
@@ -596,20 +602,22 @@
             transform_parameters['errors'].update(error)
             ret = {'transform': transform, 'transform_parameters': transform_parameters}
             return ret
         return None
 
     def process_abort_transform(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
                 self.logger.info("process_abort_transform: event: %s" % event)
                 tf = self.get_transform(transform_id=event._transform_id, locking=True)
                 if not tf:
                     self.logger.error("Cannot find transform for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(tf)
                     self.logger.info(log_pre + "process_abort_transform")
 
                     if tf['status'] in [TransformStatus.Finished, TransformStatus.SubFinished,
                                         TransformStatus.Failed, TransformStatus.Cancelled,
                                         TransformStatus.Suspended, TransformStatus.Expired]:
@@ -636,15 +644,17 @@
                         if processing and processing.processing_id:
                             self.logger.info(log_pre + "AbortProcessingEvent(processing_id: %s)" % processing.processing_id)
                             event = AbortProcessingEvent(publisher_id=self.id, processing_id=processing.processing_id, content=event._content)
                             self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def handle_resume_transform(self, transform):
         """
         process resume transform
         """
         try:
             work = transform['transform_metadata']['work']
@@ -668,20 +678,22 @@
             transform_parameters['errors'].update(error)
             ret = {'transform': transform, 'transform_parameters': transform_parameters}
             return ret
         return None
 
     def process_resume_transform(self, event):
         self.number_workers += 1
+        pro_ret = ReturnCode.Ok.value
         try:
             if event:
                 self.logger.info("process_resume_transform: event: %s" % event)
                 tf = self.get_transform(transform_id=event._transform_id, locking=True)
                 if not tf:
                     self.logger.error("Cannot find transform for event: %s" % str(event))
+                    pro_ret = ReturnCode.Locked.value
                 else:
                     log_pre = self.get_log_prefix(tf)
 
                     if tf['status'] in [TransformStatus.Finished]:
                         ret = {'transform': tf,
                                'transform_parameters': {'locking': TransformLocking.Idle,
                                                         'errors': {'extra_msg': "Transform is already finished. Cannot be resumed"}}}
@@ -711,15 +723,17 @@
                             event = UpdateTransformEvent(publisher_id=self.id,
                                                          transform_id=tf['transform_id'],
                                                          content=event._content)
                             self.event_bus.send(event)
         except Exception as ex:
             self.logger.error(ex)
             self.logger.error(traceback.format_exc())
+            pro_ret = ReturnCode.Failed.value
         self.number_workers -= 1
+        return pro_ret
 
     def clean_locks(self):
         self.logger.info("clean locking")
         core_transforms.clean_locking()
 
     def init_event_function_map(self):
         self.event_func_map = {
@@ -743,14 +757,15 @@
 
     def run(self):
         """
         Main run function.
         """
         try:
             self.logger.info("Starting main thread")
+            self.init_thread_info()
 
             self.load_plugins()
 
             self.add_default_tasks()
 
             self.init_event_function_map()
```

### Comparing `idds-server-1.1.5/lib/idds/agents/transporter/transporter.py` & `idds-server-1.2.0/lib/idds/agents/transporter/transporter.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/api/catalog.py` & `idds-server-1.2.0/lib/idds/api/catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/api/collections.py` & `idds-server-1.2.0/lib/idds/api/collections.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/api/contents.py` & `idds-server-1.2.0/lib/idds/api/contents.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/api/processings.py` & `idds-server-1.2.0/lib/idds/api/processings.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/api/requests.py` & `idds-server-1.2.0/lib/idds/api/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/api/transforms.py` & `idds-server-1.2.0/lib/idds/api/transforms.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/core/catalog.py` & `idds-server-1.2.0/lib/idds/core/catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -652,14 +652,25 @@
 
     :param request_id: The Request id.
     :param transfomr_id: The transform id.
     """
     return orm_contents.update_contents_from_others_by_dep_id(request_id=request_id, transform_id=transform_id, session=session)
 
 
+@read_session
+def get_update_contents_from_others_by_dep_id(request_id=None, transform_id=None, session=None):
+    """
+    Update contents from others by content_dep_id
+
+    :param request_id: The Request id.
+    :param transfomr_id: The transform id.
+    """
+    return orm_contents.get_update_contents_from_others_by_dep_id(request_id=request_id, transform_id=transform_id, session=session)
+
+
 @transactional_session
 def add_contents_update(contents, bulk_size=10000, session=None):
     """
     Add contents update.
 
     :param contents: dict of contents.
     :param session: session.
@@ -669,24 +680,44 @@
 
     :returns: content ids.
     """
     return orm_contents.add_contents_update(contents, bulk_size=bulk_size, session=session)
 
 
 @transactional_session
-def delete_contents_update(request_id=None, transform_id=None, session=None):
+def set_fetching_contents_update(request_id=None, transform_id=None, fetch=False, session=None):
+    """
+    Set fetching contents update.
+
+    :param session: session.
+    """
+    return orm_contents.set_fetching_contents_update(request_id=request_id, transform_id=transform_id, fetch=fetch, session=session)
+
+
+@read_session
+def get_contents_update(request_id=None, transform_id=None, fetch=False, session=None):
+    """
+    Get contents update.
+
+    :param session: session.
+    """
+    return orm_contents.get_contents_update(request_id=request_id, transform_id=transform_id, fetch=fetch, session=session)
+
+
+@transactional_session
+def delete_contents_update(request_id=None, transform_id=None, contents=[], fetch=False, session=None):
     """
     delete a content.
 
     :param session: The database session in use.
 
     :raises NoObject: If no content is founded.
     :raises DatabaseException: If there is a database error.
     """
-    return orm_contents.delete_contents_update(request_id=request_id, transform_id=transform_id, session=session)
+    return orm_contents.delete_contents_update(request_id=request_id, transform_id=transform_id, contents=contents, fetch=fetch, session=session)
 
 
 def get_contents_ext_maps():
     return orm_contents.get_contents_ext_maps()
 
 
 @transactional_session
```

### Comparing `idds-server-1.1.5/lib/idds/core/commands.py` & `idds-server-1.2.0/lib/idds/core/commands.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/core/messages.py` & `idds-server-1.2.0/lib/idds/core/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
-# - Wen Guan, <wen.guan@cern.ch>, 2019
+# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
 
 """
 operations related to Messages.
 """
 
 from idds.common.constants import MessageDestination, MessageType, MessageStatus
@@ -110,7 +110,17 @@
 def update_messages(messages, session=None):
     """
     Update all messages status with the given IDs.
 
     :param messages: The messages to be updated as a list of dictionaries.
     """
     return orm_messages.update_messages(messages=messages, session=session)
+
+
+@transactional_session
+def clean_old_messages(request_id, session=None):
+    """
+    Delete messages whose request id is older than request_id.
+
+    :param request_id: request id..
+    """
+    return orm_messages.clean_old_messages(request_id=request_id, session=session)
```

### Comparing `idds-server-1.1.5/lib/idds/core/processings.py` & `idds-server-1.2.0/lib/idds/core/processings.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/core/requests.py` & `idds-server-1.2.0/lib/idds/core/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # You may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 # http://www.apache.org/licenses/LICENSE-2.0OA
 #
 # Authors:
-# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2022
+# - Wen Guan, <wen.guan@cern.ch>, 2019 - 2023
 
 
 """
 operations related to Requests.
 """
 
 import copy
@@ -450,7 +450,20 @@
 def clean_next_poll_at(status, session=None):
     """
     Clearn next_poll_at.
 
     :param status: status of the request
     """
     orm_requests.clean_next_poll_at(status=status, session=session)
+
+
+@read_session
+def get_last_request_id(status, older_than=None, session=None):
+    """
+    Get last request id which is older than a timestamp.
+
+    :param status: status of the request.
+    :param older_than: days older than current timestamp.
+
+    :returns request_id
+    """
+    return orm_requests.get_last_request_id(status=status, older_than=older_than, session=session)
```

### Comparing `idds-server-1.1.5/lib/idds/core/transforms.py` & `idds-server-1.2.0/lib/idds/core/transforms.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/core/workprogress.py` & `idds-server-1.2.0/lib/idds/core/workprogress.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/orm/base/alembic/env.py` & `idds-server-1.2.0/lib/idds/orm/base/alembic/env.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/orm/base/enum.py` & `idds-server-1.2.0/lib/idds/orm/base/enum.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/orm/base/models.py` & `idds-server-1.2.0/lib/idds/orm/base/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 
 from idds.common.constants import (RequestType, RequestStatus, RequestLocking,
                                    WorkprogressStatus, WorkprogressLocking,
                                    TransformType, TransformStatus, TransformLocking,
                                    ProcessingStatus, ProcessingLocking,
                                    CollectionStatus, CollectionLocking, CollectionType,
                                    CollectionRelationType, ContentType, ContentRelationType,
-                                   ContentStatus, ContentLocking, GranularityType,
+                                   ContentStatus, ContentFetchStatus, ContentLocking, GranularityType,
                                    MessageType, MessageStatus, MessageLocking,
                                    MessageSource, MessageDestination,
                                    CommandType, CommandStatus, CommandLocking,
-                                   CommandLocation)
+                                   CommandLocation, HealthStatus)
+from idds.common.event import (EventType, EventStatus)
 from idds.common.utils import date_to_str
 from idds.orm.base.enum import EnumSymbol
 from idds.orm.base.types import JSON, JSONString, EnumWithValue
 from idds.orm.base.session import BASE, DEFAULT_SCHEMA_NAME
 from idds.common.constants import (SCOPE_LENGTH, NAME_LENGTH, LONG_NAME_LENGTH)
 
 
@@ -132,26 +133,26 @@
 class Request(BASE, ModelBase):
     """Represents a pre-cache request from other service"""
     __tablename__ = 'requests'
     request_id = Column(BigInteger().with_variant(Integer, "sqlite"), Sequence('REQUEST_ID_SEQ', schema=DEFAULT_SCHEMA_NAME), primary_key=True)
     scope = Column(String(SCOPE_LENGTH))
     name = Column(String(NAME_LENGTH))
     requester = Column(String(20))
-    request_type = Column(EnumWithValue(RequestType))
+    request_type = Column(EnumWithValue(RequestType), nullable=False)
     username = Column(String(20))
     userdn = Column(String(200))
     transform_tag = Column(String(20))
     workload_id = Column(Integer())
     priority = Column(Integer())
-    status = Column(EnumWithValue(RequestStatus))
+    status = Column(EnumWithValue(RequestStatus), nullable=False)
     substatus = Column(EnumWithValue(RequestStatus), default=0)
     oldstatus = Column(EnumWithValue(RequestStatus), default=0)
-    locking = Column(EnumWithValue(RequestLocking))
-    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow)
-    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
+    locking = Column(EnumWithValue(RequestLocking), nullable=False)
+    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
+    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow, nullable=False)
     next_poll_at = Column("next_poll_at", DateTime, default=datetime.datetime.utcnow)
     accessed_at = Column("accessed_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
     expired_at = Column("expired_at", DateTime)
     new_retries = Column(Integer(), default=0)
     update_retries = Column(Integer(), default=0)
     max_new_retries = Column(Integer(), default=3)
     max_update_retries = Column(Integer(), default=0)
@@ -237,15 +238,16 @@
             del values['processing_metadata']
         super(Request, self).update(values, flush, session)
 
     _table_args = (PrimaryKeyConstraint('request_id', name='REQUESTS_PK'),
                    CheckConstraint('status IS NOT NULL', name='REQUESTS_STATUS_ID_NN'),
                    # UniqueConstraint('name', 'scope', 'requester', 'request_type', 'transform_tag', 'workload_id', name='REQUESTS_NAME_SCOPE_UQ '),
                    Index('REQUESTS_SCOPE_NAME_IDX', 'name', 'scope', 'workload_id'),
-                   Index('REQUESTS_STATUS_PRIO_IDX', 'status', 'priority', 'request_id', 'locking', 'updated_at', 'next_poll_at', 'created_at'))
+                   Index('REQUESTS_STATUS_PRIO_IDX', 'status', 'priority', 'request_id', 'locking', 'updated_at', 'next_poll_at', 'created_at'),
+                   Index('REQUESTS_STATUS_POLL_IDX', 'status', 'priority', 'locking', 'updated_at', 'new_poll_period', 'update_poll_period', 'created_at', 'request_id'))
 
 
 class Workprogress(BASE, ModelBase):
     """Represents a workprogress which monitors the progress of a workflow"""
     __tablename__ = 'workprogresses'
     workprogress_id = Column(BigInteger().with_variant(Integer, "sqlite"), Sequence('WORKPROGRESS_ID_SEQ', schema=DEFAULT_SCHEMA_NAME), primary_key=True)
     request_id = Column(BigInteger().with_variant(Integer, "sqlite"))
@@ -277,27 +279,27 @@
                    Index('WORKPROGRESS_STATUS_PRIO_IDX', 'status', 'priority', 'workprogress_id', 'locking', 'updated_at', 'next_poll_at', 'created_at'))
 
 
 class Transform(BASE, ModelBase):
     """Represents a transform"""
     __tablename__ = 'transforms'
     transform_id = Column(BigInteger().with_variant(Integer, "sqlite"), Sequence('TRANSFORM_ID_SEQ', schema=DEFAULT_SCHEMA_NAME), primary_key=True)
-    request_id = Column(BigInteger().with_variant(Integer, "sqlite"))
+    request_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
     workload_id = Column(Integer())
-    transform_type = Column(EnumWithValue(TransformType))
+    transform_type = Column(EnumWithValue(TransformType), nullable=False)
     transform_tag = Column(String(20))
     priority = Column(Integer())
     safe2get_output_from_input = Column(Integer())
-    status = Column(EnumWithValue(TransformStatus))
+    status = Column(EnumWithValue(TransformStatus), nullable=False)
     substatus = Column(EnumWithValue(TransformStatus), default=0)
     oldstatus = Column(EnumWithValue(TransformStatus), default=0)
-    locking = Column(EnumWithValue(TransformLocking))
+    locking = Column(EnumWithValue(TransformLocking), nullable=False)
     retries = Column(Integer(), default=0)
-    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow)
-    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
+    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
+    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow, nullable=False)
     next_poll_at = Column("next_poll_at", DateTime, default=datetime.datetime.utcnow)
     started_at = Column("started_at", DateTime)
     finished_at = Column("finished_at", DateTime)
     expired_at = Column("expired_at", DateTime)
     new_retries = Column(Integer(), default=0)
     update_retries = Column(Integer(), default=0)
     max_new_retries = Column(Integer(), default=3)
@@ -361,15 +363,17 @@
             values['_running_metadata'] = values['running_metadata']
             del values['running_metadata']
         super(Transform, self).update(values, flush, session)
 
     _table_args = (PrimaryKeyConstraint('transform_id', name='TRANSFORMS_PK'),
                    CheckConstraint('status IS NOT NULL', name='TRANSFORMS_STATUS_ID_NN'),
                    Index('TRANSFORMS_TYPE_TAG_IDX', 'transform_type', 'transform_tag', 'transform_id'),
-                   Index('TRANSFORMS_STATUS_UPDATED_AT_IDX', 'status', 'locking', 'updated_at', 'next_poll_at', 'created_at'))
+                   Index('TRANSFORMS_STATUS_UPDATED_AT_IDX', 'status', 'locking', 'updated_at', 'next_poll_at', 'created_at'),
+                   Index('TRANSFORMS_REQ_IDX', 'request_id', 'transform_id'),
+                   Index('TRANSFORMS_STATUS_POLL_IDX', 'status', 'locking', 'updated_at', 'new_poll_period', 'update_poll_period', 'created_at', 'transform_id'))
 
 
 class Workprogress2transform(BASE, ModelBase):
     """Represents a workprogress to transform"""
     __tablename__ = 'wp2transforms'
     workprogress_id = Column(BigInteger().with_variant(Integer, "sqlite"), primary_key=True)
     transform_id = Column(BigInteger().with_variant(Integer, "sqlite"), primary_key=True)
@@ -379,27 +383,27 @@
                    ForeignKeyConstraint(['transform_id'], ['transforms.transform_id'], name='WP2TRANSFORM_TRANS_ID_FK'))
 
 
 class Processing(BASE, ModelBase):
     """Represents a processing"""
     __tablename__ = 'processings'
     processing_id = Column(BigInteger().with_variant(Integer, "sqlite"), Sequence('PROCESSING_ID_SEQ', schema=DEFAULT_SCHEMA_NAME), primary_key=True)
-    transform_id = Column(BigInteger().with_variant(Integer, "sqlite"))
-    request_id = Column(BigInteger().with_variant(Integer, "sqlite"))
+    transform_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
+    request_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
     workload_id = Column(Integer())
-    status = Column(EnumWithValue(ProcessingStatus))
+    status = Column(EnumWithValue(ProcessingStatus), nullable=False)
     substatus = Column(EnumWithValue(ProcessingStatus), default=0)
     oldstatus = Column(EnumWithValue(ProcessingStatus), default=0)
-    locking = Column(EnumWithValue(ProcessingLocking))
+    locking = Column(EnumWithValue(ProcessingLocking), nullable=False)
     submitter = Column(String(20))
     submitted_id = Column(Integer())
     granularity = Column(Integer())
     granularity_type = Column(EnumWithValue(GranularityType))
-    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow)
-    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
+    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
+    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow, nullable=False)
     next_poll_at = Column("next_poll_at", DateTime, default=datetime.datetime.utcnow)
     poller_updated_at = Column("poller_updated_at", DateTime, default=datetime.datetime.utcnow)
     submitted_at = Column("submitted_at", DateTime)
     finished_at = Column("finished_at", DateTime)
     expired_at = Column("expired_at", DateTime)
     new_retries = Column(Integer(), default=0)
     update_retries = Column(Integer(), default=0)
@@ -465,81 +469,83 @@
             del values['running_metadata']
         super(Transform, self).update(values, flush, session)
 
     _table_args = (PrimaryKeyConstraint('processing_id', name='PROCESSINGS_PK'),
                    ForeignKeyConstraint(['transform_id'], ['transforms.transform_id'], name='PROCESSINGS_TRANSFORM_ID_FK'),
                    CheckConstraint('status IS NOT NULL', name='PROCESSINGS_STATUS_ID_NN'),
                    CheckConstraint('transform_id IS NOT NULL', name='PROCESSINGS_TRANSFORM_ID_NN'),
-                   Index('PROCESSINGS_STATUS_UPDATED_IDX', 'status', 'locking', 'updated_at', 'next_poll_at', 'created_at'))
+                   Index('PROCESSINGS_STATUS_UPDATED_IDX', 'status', 'locking', 'updated_at', 'next_poll_at', 'created_at'),
+                   Index('PROCESSINGS_STATUS_POLL_IDX', 'status', 'processing_id', 'locking', 'updated_at', 'new_poll_period', 'update_poll_period', 'created_at'))
 
 
 class Collection(BASE, ModelBase):
     """Represents a collection"""
     __tablename__ = 'collections'
     coll_id = Column(BigInteger().with_variant(Integer, "sqlite"), Sequence('COLLECTION_ID_SEQ', schema=DEFAULT_SCHEMA_NAME), primary_key=True)
-    request_id = Column(BigInteger().with_variant(Integer, "sqlite"))
+    request_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
     workload_id = Column(Integer())
-    transform_id = Column(BigInteger().with_variant(Integer, "sqlite"))
-    coll_type = Column(EnumWithValue(CollectionType))
-    relation_type = Column(EnumWithValue(CollectionRelationType))
+    transform_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
+    coll_type = Column(EnumWithValue(CollectionType), nullable=False)
+    relation_type = Column(EnumWithValue(CollectionRelationType), nullable=False)
     scope = Column(String(SCOPE_LENGTH))
     name = Column(String(NAME_LENGTH))
     bytes = Column(Integer())
-    status = Column(EnumWithValue(CollectionStatus))
+    status = Column(EnumWithValue(CollectionStatus), nullable=False)
     substatus = Column(EnumWithValue(CollectionStatus), default=0)
-    locking = Column(EnumWithValue(CollectionLocking))
+    locking = Column(EnumWithValue(CollectionLocking), nullable=False)
     total_files = Column(Integer())
     storage_id = Column(Integer())
     new_files = Column(Integer())
     processed_files = Column(Integer())
     processing_files = Column(Integer())
     failed_files = Column(Integer())
     missing_files = Column(Integer())
     ext_files = Column(Integer())
     processed_ext_files = Column(Integer())
     failed_ext_files = Column(Integer())
     missing_ext_files = Column(Integer())
     processing_id = Column(Integer())
     retries = Column(Integer(), default=0)
-    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow)
-    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
+    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
+    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow, nullable=False)
     next_poll_at = Column("next_poll_at", DateTime, default=datetime.datetime.utcnow)
     accessed_at = Column("accessed_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
     expired_at = Column("expired_at", DateTime)
     coll_metadata = Column(JSON())
 
     _table_args = (PrimaryKeyConstraint('coll_id', name='COLLECTIONS_PK'),
                    UniqueConstraint('name', 'scope', 'transform_id', 'relation_type', name='COLLECTIONS_NAME_SCOPE_UQ'),
                    ForeignKeyConstraint(['transform_id'], ['transforms.transform_id'], name='COLLECTIONS_TRANSFORM_ID_FK'),
                    CheckConstraint('status IS NOT NULL', name='COLLECTIONS_STATUS_ID_NN'),
                    CheckConstraint('transform_id IS NOT NULL', name='COLLECTIONS_TRANSFORM_ID_NN'),
                    Index('COLLECTIONS_STATUS_RELAT_IDX', 'status', 'relation_type'),
                    Index('COLLECTIONS_TRANSFORM_IDX', 'transform_id', 'coll_id'),
-                   Index('COLLECTIONS_STATUS_UPDATED_IDX', 'status', 'locking', 'updated_at', 'next_poll_at', 'created_at'))
+                   Index('COLLECTIONS_STATUS_UPDATED_IDX', 'status', 'locking', 'updated_at', 'next_poll_at', 'created_at'),
+                   Index('COLLECTIONS_REQ_IDX', 'request_id', 'transform_id', 'updated_at'),)
 
 
 class Content(BASE, ModelBase):
     """Represents a content"""
     __tablename__ = 'contents'
     content_id = Column(BigInteger().with_variant(Integer, "sqlite"), Sequence('CONTENT_ID_SEQ', schema=DEFAULT_SCHEMA_NAME), primary_key=True)
-    transform_id = Column(BigInteger().with_variant(Integer, "sqlite"))
-    coll_id = Column(BigInteger().with_variant(Integer, "sqlite"))
-    request_id = Column(BigInteger().with_variant(Integer, "sqlite"))
+    transform_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
+    coll_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
+    request_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
     workload_id = Column(Integer())
-    map_id = Column(BigInteger().with_variant(Integer, "sqlite"), default=0)
+    map_id = Column(BigInteger().with_variant(Integer, "sqlite"), default=0, nullable=False)
     content_dep_id = Column(BigInteger())
     scope = Column(String(SCOPE_LENGTH))
     name = Column(String(LONG_NAME_LENGTH))
     min_id = Column(Integer(), default=0)
     max_id = Column(Integer(), default=0)
-    content_type = Column(EnumWithValue(ContentType))
-    content_relation_type = Column(EnumWithValue(ContentRelationType), default=0)
-    status = Column(EnumWithValue(ContentStatus))
+    content_type = Column(EnumWithValue(ContentType), nullable=False)
+    content_relation_type = Column(EnumWithValue(ContentRelationType), default=0, nullable=False)
+    status = Column(EnumWithValue(ContentStatus), nullable=False)
     substatus = Column(EnumWithValue(ContentStatus))
-    locking = Column(EnumWithValue(ContentLocking))
+    locking = Column(EnumWithValue(ContentLocking), nullable=False)
     bytes = Column(Integer())
     md5 = Column(String(32))
     adler32 = Column(String(8))
     processing_id = Column(Integer())
     storage_id = Column(Integer())
     retries = Column(Integer(), default=0)
     path = Column(String(4000))
@@ -557,38 +563,42 @@
                    ForeignKeyConstraint(['transform_id'], ['transforms.transform_id'], name='CONTENTS_TRANSFORM_ID_FK'),
                    ForeignKeyConstraint(['coll_id'], ['collections.coll_id'], name='CONTENTS_COLL_ID_FK'),
                    CheckConstraint('status IS NOT NULL', name='CONTENTS_STATUS_ID_NN'),
                    CheckConstraint('coll_id IS NOT NULL', name='CONTENTS_COLL_ID_NN'),
                    Index('CONTENTS_STATUS_UPDATED_IDX', 'status', 'locking', 'updated_at', 'created_at'),
                    Index('CONTENTS_ID_NAME_IDX', 'coll_id', 'scope', 'name', 'status'),
                    Index('CONTENTS_DEP_IDX', 'request_id', 'transform_id', 'content_dep_id'),
+                   Index('CONTENTS_REL_IDX', 'request_id', 'content_relation_type', 'transform_id', 'substatus'),
+                   Index('CONTENTS_TF_IDX', 'transform_id', 'request_id', 'coll_id', 'map_id', 'content_relation_type'),
                    Index('CONTENTS_REQ_TF_COLL_IDX', 'request_id', 'transform_id', 'workload_id', 'coll_id', 'content_relation_type', 'status', 'substatus'))
 
 
 class Content_update(BASE, ModelBase):
     """Represents a content update"""
     __tablename__ = 'contents_update'
     content_id = Column(BigInteger().with_variant(Integer, "sqlite"), primary_key=True)
     substatus = Column(EnumWithValue(ContentStatus))
     request_id = Column(BigInteger().with_variant(Integer, "sqlite"))
     transform_id = Column(BigInteger().with_variant(Integer, "sqlite"))
     workload_id = Column(Integer())
+    fetch_status = Column(EnumWithValue(ContentFetchStatus), default=0, nullable=False)
     coll_id = Column(BigInteger().with_variant(Integer, "sqlite"))
+    content_metadata = Column(JSONString(100))
 
 
 class Content_ext(BASE, ModelBase):
     """Represents a content extension"""
     __tablename__ = 'contents_ext'
     content_id = Column(BigInteger().with_variant(Integer, "sqlite"), primary_key=True)
-    transform_id = Column(BigInteger().with_variant(Integer, "sqlite"))
-    coll_id = Column(BigInteger().with_variant(Integer, "sqlite"))
-    request_id = Column(BigInteger().with_variant(Integer, "sqlite"))
+    transform_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
+    coll_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
+    request_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
     workload_id = Column(Integer())
-    map_id = Column(BigInteger().with_variant(Integer, "sqlite"), default=0)
-    status = Column(EnumWithValue(ContentStatus))
+    map_id = Column(BigInteger().with_variant(Integer, "sqlite"), default=0, nullable=False)
+    status = Column(EnumWithValue(ContentStatus), nullable=False)
     panda_id = Column(BigInteger())
     job_definition_id = Column(BigInteger())
     scheduler_id = Column(String(128))
     pilot_id = Column(String(200))
     creation_time = Column(DateTime)
     modification_time = Column(DateTime)
     start_time = Column(DateTime)
@@ -654,90 +664,227 @@
     hs06 = Column(Integer())
     hs06sec = Column(Integer())
     memory_leak = Column(String(10))
     memory_leak_x2 = Column(String(10))
     job_label = Column(String(20))
 
     _table_args = (PrimaryKeyConstraint('content_id', name='CONTENTS_EXT_PK'),
-                   Index('CONTENTS_EXT_RTF_IDX', 'request_id', 'transform_id', 'workload_id', 'coll_id', 'content_id', 'panda_id', 'status'))
+                   Index('CONTENTS_EXT_RTF_IDX', 'request_id', 'transform_id', 'workload_id', 'coll_id', 'content_id', 'panda_id', 'status'),
+                   Index('CONTENTS_EXT_RTW_IDX', 'request_id', 'transform_id', 'workload_id'),
+                   Index('CONTENTS_EXT_RTM_IDX', 'request_id', 'transform_id', 'map_id'))
 
 
 class Health(BASE, ModelBase):
     """Represents the status of the running agents"""
     __tablename__ = 'health'
     health_id = Column(BigInteger().with_variant(Integer, "sqlite"),
                        Sequence('HEALTH_ID_SEQ', schema=DEFAULT_SCHEMA_NAME),
                        primary_key=True)
     agent = Column(String(30))
-    hostname = Column(String(127))
+    hostname = Column(String(500))
     pid = Column(Integer, autoincrement=False)
+    status = Column(EnumWithValue(HealthStatus), default=0, nullable=False)
     thread_id = Column(BigInteger, autoincrement=False)
     thread_name = Column(String(255))
-    payload = Column(String(255))
+    payload = Column(String(2048))
     created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow)
     updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
+    payload = Column(String(2048))
     _table_args = (PrimaryKeyConstraint('health_id', name='HEALTH_PK'),
                    UniqueConstraint('agent', 'hostname', 'pid', 'thread_id', name='HEALTH_UK'))
 
 
 class Message(BASE, ModelBase):
     """Represents the event messages"""
     __tablename__ = 'messages'
     msg_id = Column(BigInteger().with_variant(Integer, "sqlite"),
                     Sequence('MESSAGE_ID_SEQ', schema=DEFAULT_SCHEMA_NAME),
                     primary_key=True)
-    msg_type = Column(EnumWithValue(MessageType))
-    status = Column(EnumWithValue(MessageStatus))
+    msg_type = Column(EnumWithValue(MessageType), nullable=False)
+    status = Column(EnumWithValue(MessageStatus), nullable=False)
     substatus = Column(Integer())
-    locking = Column(EnumWithValue(MessageLocking))
-    source = Column(EnumWithValue(MessageSource))
-    destination = Column(EnumWithValue(MessageDestination))
-    request_id = Column(BigInteger().with_variant(Integer, "sqlite"))
+    locking = Column(EnumWithValue(MessageLocking), nullable=False)
+    source = Column(EnumWithValue(MessageSource), nullable=False)
+    destination = Column(EnumWithValue(MessageDestination), nullable=False)
+    request_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
     workload_id = Column(Integer())
-    transform_id = Column(Integer())
-    processing_id = Column(Integer())
+    transform_id = Column(Integer(), nullable=False)
+    processing_id = Column(Integer(), nullable=False)
     num_contents = Column(Integer())
     retries = Column(Integer(), default=0)
-    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow)
-    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
+    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
+    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow, nullable=False)
     msg_content = Column(JSON())
 
     _table_args = (PrimaryKeyConstraint('msg_id', name='MESSAGES_PK'),
                    Index('MESSAGES_TYPE_ST_IDX', 'msg_type', 'status', 'destination', 'request_id'),
                    Index('MESSAGES_TYPE_ST_TF_IDX', 'msg_type', 'status', 'destination', 'transform_id'),
-                   Index('MESSAGES_TYPE_ST_PR_IDX', 'msg_type', 'status', 'destination', 'processing_id'))
+                   Index('MESSAGES_TYPE_ST_PR_IDX', 'msg_type', 'status', 'destination', 'processing_id'),
+                   Index('MESSAGES_ST_IDX', 'status', 'destination', 'created_at'),
+                   Index('MESSAGES_TYPE_STU_IDX', 'msg_type', 'status', 'destination', 'retries', 'updated_at', 'created_at'))
 
 
 class Command(BASE, ModelBase):
     """Represents the operations commands"""
     __tablename__ = 'commands'
     cmd_id = Column(BigInteger().with_variant(Integer, "sqlite"),
                     Sequence('COMMAND_ID_SEQ', schema=DEFAULT_SCHEMA_NAME),
                     primary_key=True)
-    request_id = Column(BigInteger().with_variant(Integer, "sqlite"))
+    request_id = Column(BigInteger().with_variant(Integer, "sqlite"), nullable=False)
     workload_id = Column(Integer())
     transform_id = Column(Integer())
     processing_id = Column(Integer())
     cmd_type = Column(EnumWithValue(CommandType))
-    status = Column(EnumWithValue(CommandStatus))
+    status = Column(EnumWithValue(CommandStatus), nullable=False)
     substatus = Column(Integer())
-    locking = Column(EnumWithValue(CommandLocking))
+    locking = Column(EnumWithValue(CommandLocking), nullable=False)
     username = Column(String(50))
     retries = Column(Integer(), default=0)
     source = Column(EnumWithValue(CommandLocation))
     destination = Column(EnumWithValue(CommandLocation))
-    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow)
-    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow)
+    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
+    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow, nullable=False)
     cmd_content = Column(JSON())
     errors = Column(JSONString(1024))
 
     _table_args = (PrimaryKeyConstraint('cmd_id', name='COMMANDS_PK'),
                    Index('COMMANDS_TYPE_ST_IDX', 'cmd_type', 'status', 'destination', 'request_id'),
                    Index('COMMANDS_TYPE_ST_TF_IDX', 'cmd_type', 'status', 'destination', 'transform_id'),
-                   Index('COMMANDS_TYPE_ST_PR_IDX', 'cmd_type', 'status', 'destination', 'processing_id'))
+                   Index('COMMANDS_TYPE_ST_PR_IDX', 'cmd_type', 'status', 'destination', 'processing_id'),
+                   Index('COMMANDS_STATUS_IDX', 'status', 'locking', 'updated_at'))
+
+
+class EventPriority(BASE, ModelBase):
+    """Represents the operations events"""
+    __tablename__ = 'events_priority'
+    event_type = Column(EnumWithValue(EventType), primary_key=True, nullable=False)
+    event_actual_id = Column(Integer(), primary_key=True, nullable=False)
+    priority = Column(Integer(), default=1000, nullable=False)
+    last_processed_at = Column("last_processed_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
+    updated_at = Column("updated_at", DateTime, default=datetime.datetime.utcnow, onupdate=datetime.datetime.utcnow, nullable=False)
+
+    _table_args = (PrimaryKeyConstraint('event_type', 'event_actual_id', name='EVENTS_PR_PK'))
+
+
+class Event(BASE, ModelBase):
+    """Represents the operations events"""
+    __tablename__ = 'events'
+    event_id = Column(BigInteger().with_variant(Integer, "sqlite"),
+                      Sequence('EVENT_ID_SEQ', schema=DEFAULT_SCHEMA_NAME),
+                      primary_key=True)
+    event_type = Column(EnumWithValue(EventType), nullable=False)
+    event_actual_id = Column(Integer(), nullable=False)
+    priority = Column(Integer())
+    status = Column(EnumWithValue(EventStatus), nullable=False)
+    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
+    processing_at = Column("processing_at", DateTime, default=None)
+    processed_at = Column("processed_at", DateTime, default=None)
+    content = Column(JSON())
+
+    @property
+    def _id(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event']._id
+        return None
+
+    @property
+    def _publisher_id(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event']._publisher_id
+        return None
+
+    @property
+    def _event_type(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event']._event_type
+        return None
+
+    @property
+    def _timestamp(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event']._timestamp
+        return None
+
+    @property
+    def _counter(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event']._counter
+        return None
+
+    @property
+    def _content(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event']._content
+        return None
+
+    @property
+    def has_changes(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event'].has_changes
+        return None
+
+    def get_event_id(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event'].get_event_id()
+        return None
+
+    def able_to_merge(self, event):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event'].able_to_merge(event)
+        return False
+
+    def changed(self):
+        return self.has_changes
+
+    def merge(self, event):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event'].merge(event)
+        return False, event
+
+    @property
+    def _request_id(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event']._request_id
+        return None
+
+    @property
+    def _command_id(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event']._command_id
+        return None
+
+    @property
+    def _transform_id(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event']._transform_id
+        return None
+
+    @property
+    def _processing_id(self):
+        if self.content and 'event' in self.content and self.content['event']:
+            return self.content['event']._processing_id
+        return None
+
+    _table_args = (PrimaryKeyConstraint('event_id', name='EVENTS_PK'))
+
+
+class EventArchive(BASE, ModelBase):
+    """Represents the operations events"""
+    __tablename__ = 'events_archive'
+    event_id = Column(BigInteger(), primary_key=True)
+    event_type = Column(EnumWithValue(EventType), nullable=False)
+    event_actual_id = Column(Integer(), nullable=False)
+    priority = Column(Integer())
+    status = Column(EnumWithValue(EventStatus), nullable=False)
+    created_at = Column("created_at", DateTime, default=datetime.datetime.utcnow, nullable=False)
+    processing_at = Column("processing_at", DateTime, default=None)
+    processed_at = Column("processed_at", DateTime, default=None)
+    content = Column(JSON())
+
+    _table_args = (PrimaryKeyConstraint('event_id', name='EVENTS_AR_PK'))
 
 
 def create_trigger():
     func = DDL("""
         SET search_path TO %s;
         CREATE OR REPLACE FUNCTION update_dep_contents_status()
         RETURNS TRIGGER AS $$
```

### Comparing `idds-server-1.1.5/lib/idds/orm/base/session.py` & `idds-server-1.2.0/lib/idds/orm/base/session.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/orm/base/types.py` & `idds-server-1.2.0/lib/idds/orm/base/types.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/orm/base/utils.py` & `idds-server-1.2.0/lib/idds/orm/base/utils.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/orm/collections.py` & `idds-server-1.2.0/lib/idds/orm/collections.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/orm/commands.py` & `idds-server-1.2.0/lib/idds/orm/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,22 +94,14 @@
     :param session: The database session.
 
     :returns command: List of dictionaries
     """
     command = []
     try:
         query = session.query(models.Command)
-        if request_id is not None:
-            query = query.with_hint(models.Command, "INDEX(COMMANDS COMMANDS_TYPE_ST_IDX)", 'oracle')
-        elif transform_id:
-            query = query.with_hint(models.Command, "INDEX(COMMANDS COMMANDS_TYPE_ST_TF_IDX)", 'oracle')
-        elif processing_id is not None:
-            query = query.with_hint(models.Command, "INDEX(COMMANDS COMMANDS_TYPE_ST_PR_IDX)", 'oracle')
-        else:
-            query = query.with_hint(models.Command, "INDEX(COMMANDS COMMANDS_TYPE_ST_IDX)", 'oracle')
 
         if cmd_type is not None:
             query = query.filter_by(cmd_type=cmd_type)
         if status is not None:
             query = query.filter_by(status=status)
         if source is not None:
             query = query.filter_by(source=source)
@@ -147,15 +139,14 @@
     command_condition = []
     for command in command:
         command_condition.append(models.Command.cmd_id == command['cmd_id'])
 
     try:
         if command_condition:
             session.query(models.Command).\
-                with_hint(models.Command, "index(command COMMANDS_PK)", 'oracle').\
                 filter(or_(*command_condition)).\
                 delete(synchronize_session=False)
     except IntegrityError as e:
         raise exceptions.DatabaseException(e.args)
 
 
 @transactional_session
```

### Comparing `idds-server-1.1.5/lib/idds/orm/contents.py` & `idds-server-1.2.0/lib/idds/orm/contents.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from sqlalchemy import and_
 from sqlalchemy import func
 from sqlalchemy.exc import DatabaseError, IntegrityError
 from sqlalchemy.sql.expression import asc
 
 from idds.common import exceptions
 from idds.common.constants import (ContentType, ContentStatus, ContentLocking,
-                                   ContentRelationType)
+                                   ContentFetchStatus, ContentRelationType)
 from idds.orm.base.session import read_session, transactional_session
 from idds.orm.base import models
 
 
 def create_content(request_id, workload_id, transform_id, coll_id, map_id, scope, name,
                    min_id, max_id, content_type=ContentType.File,
                    status=ContentStatus.New, content_relation_type=ContentRelationType.Input,
@@ -189,22 +189,20 @@
     try:
         if content_id:
             query = session.query(models.Content)\
                            .filter(models.Content.content_id == content_id)
         else:
             if content_type in [ContentType.File, ContentType.File.value]:
                 query = session.query(models.Content)\
-                               .with_hint(models.Content, "INDEX(CONTENTS CONTENTS_ID_NAME_IDX)", 'oracle')\
                                .filter(models.Content.coll_id == coll_id)\
                                .filter(models.Content.scope == scope)\
                                .filter(models.Content.name == name)\
                                .filter(models.Content.content_type == content_type)
             else:
                 query = session.query(models.Content)\
-                               .with_hint(models.Content, "INDEX(CONTENTS CONTENTS_ID_NAME_IDX)", 'oracle')\
                                .filter(models.Content.coll_id == coll_id)\
                                .filter(models.Content.scope == scope)\
                                .filter(models.Content.name == name)\
                                .filter(models.Content.min_id == min_id)\
                                .filter(models.Content.max_id == max_id)
                 if content_type:
                     query = query.filter(models.Content.content_type == content_type)
@@ -242,15 +240,14 @@
     :raises NoObject: If no content is founded.
 
     :returns: list of Content ids.
     """
 
     try:
         query = session.query(models.Content)\
-                       .with_hint(models.Content, "INDEX(CONTENTS CONTENTS_ID_NAME_IDX)", 'oracle')\
                        .filter(models.Content.coll_id == coll_id)\
                        .filter(models.Content.scope == scope)\
                        .filter(models.Content.name.like(name.replace('*', '%')))
 
         if content_type is not None:
             query = query.filter(models.Content.content_tye == content_type)
         if min_id is not None:
@@ -301,15 +298,14 @@
         if coll_id is not None:
             if not isinstance(coll_id, (tuple, list)):
                 coll_id = [coll_id]
             if len(coll_id) == 1:
                 coll_id = [coll_id[0], coll_id[0]]
 
         query = session.query(models.Content)
-        query = query.with_hint(models.Content, "INDEX(CONTENTS CONTENTS_ID_NAME_IDX)", 'oracle')
 
         if transform_id:
             query = query.filter(models.Content.transform_id == transform_id)
         if coll_id:
             query = query.filter(models.Content.coll_id.in_(coll_id))
         if scope:
             query = query.filter(models.Content.scope == scope)
@@ -356,15 +352,14 @@
 
     try:
         if status is not None:
             if not isinstance(status, (tuple, list)):
                 status = [status]
 
         query = session.query(models.Content)
-        query = query.with_hint(models.Content, "INDEX(CONTENTS CONTENTS_REQ_TF_COLL_IDX)", 'oracle')
         if request_id:
             query = query.filter(models.Content.request_id == request_id)
         if transform_id:
             query = query.filter(models.Content.transform_id == transform_id)
         if workload_id:
             query = query.filter(models.Content.workload_id == workload_id)
         if status is not None:
@@ -394,15 +389,14 @@
     :param coll_id: Collection id.
     :param session: The database session in use.
 
     :returns: statistics group by status, as a dict.
     """
     try:
         query = session.query(models.Content.status, func.count(models.Content.content_id))
-        query = query.with_hint(models.Content, "INDEX(CONTENTS CONTENTS_ID_NAME_IDX)", 'oracle')
         if coll_id:
             query = query.filter(models.Content.coll_id == coll_id)
         query = query.group_by(models.Content.status)
         tmp = query.all()
         rets = {}
         if tmp:
             for status, count in tmp:
@@ -468,15 +462,15 @@
     :raises DatabaseException: If there is a database error.
 
     """
     try:
         params = {'substatus': status}
         chunks = [content_dep_ids[i:i + bulk_size] for i in range(0, len(content_dep_ids), bulk_size)]
         for chunk in chunks:
-            session.query(models.Content).with_hint(models.Content, "INDEX(CONTENTS CONTENTS_DEP_IDX)", "oracle")\
+            session.query(models.Content)\
                    .filter(models.Content.request_id == request_id)\
                    .filter(models.Content.content_id.in_(chunk))\
                    .update(params, synchronize_session=False)
     except sqlalchemy.orm.exc.NoResultFound as error:
         raise exceptions.NoObject('Content cannot be found: %s' % (error))
 
 
@@ -524,45 +518,85 @@
         idds_proc = sqlalchemy.text("CALL %s.update_contents_from_others(:request_id, :transform_id)" % session.schema)
         session.execute(idds_proc, {"request_id": request_id, "transform_id": transform_id})
     except Exception as ex:
         raise ex
 
 
 @read_session
-def get_updated_transforms_by_content_status(request_id=None, transform_id=None, session=None):
+def get_update_contents_from_others_by_dep_id(request_id=None, transform_id=None, session=None):
+    """
+    Get contents to update from others by content_dep_id
+
+    :param request_id: The Request id.
+    :param transfomr_id: The transform id.
+    """
+    try:
+        subquery = session.query(models.Content.content_id,
+                                 models.Content.substatus)
+        if request_id:
+            subquery = subquery.filter(models.Content.request_id == request_id)
+        subquery = subquery.filter(models.Content.content_relation_type == 1)\
+                           .filter(models.Content.substatus != ContentStatus.New)
+        subquery = subquery.subquery()
+
+        query = session.query(models.Content.content_id,
+                              subquery.c.substatus)
+        if request_id:
+            query = query.filter(models.Content.request_id == request_id)
+        if transform_id:
+            query = query.filter(models.Content.transform_id == transform_id)
+        query = query.filter(models.Content.content_relation_type == 3)
+        query = query.join(subquery, and_(models.Content.content_dep_id == subquery.c.content_id,
+                                          models.Content.substatus != subquery.c.substatus))
+
+        tmp = query.distinct()
+        rets = []
+        if tmp:
+            for t in tmp:
+                t2 = dict(zip(t.keys(), t))
+                rets.append(t2)
+        return rets
+    except Exception as ex:
+        raise ex
+
+
+@read_session
+def get_updated_transforms_by_content_status(request_id=None, transform_id=None, check_substatus=False, session=None):
     """
     Get updated transform ids by content status
 
     :param request_id: The Request id.
 
     :returns list
     """
     try:
         subquery = session.query(models.Content.content_id,
                                  models.Content.substatus)
-        subquery = subquery.with_hint(models.Content, "INDEX(CONTENTS CONTENTS_REQ_TF_COLL_IDX)", 'oracle')
+        # subquery = subquery.with_hint(models.Content, "INDEX(CONTENTS CONTENTS_REQ_TF_COLL_IDX)", 'oracle')
         if request_id:
             subquery = subquery.filter(models.Content.request_id == request_id)
         if transform_id:
             subquery = subquery.filter(models.Content.transform_id == transform_id)
         subquery = subquery.filter(models.Content.content_relation_type == 1)
         subquery = subquery.subquery()
 
         query = session.query(models.Content.request_id,
                               models.Content.transform_id,
                               models.Content.workload_id,
                               models.Content.coll_id)
-        query = query.with_hint(models.Content, "INDEX(CONTENTS CONTENTS_REQ_TF_COLL_IDX)", 'oracle')
+        # query = query.with_hint(models.Content, "INDEX(CONTENTS CONTENTS_REQ_TF_COLL_IDX)", 'oracle')
 
         if request_id:
             query = query.filter(models.Content.request_id == request_id)
         query = query.filter(models.Content.content_relation_type == 3)
-        query = query.join(subquery, and_(models.Content.content_dep_id == subquery.c.content_id,
-                                          models.Content.substatus != subquery.c.substatus))
-
+        if check_substatus:
+            query = query.join(subquery, and_(models.Content.content_dep_id == subquery.c.content_id,
+                                              models.Content.substatus != subquery.c.substatus))
+        else:
+            query = query.join(subquery, and_(models.Content.content_dep_id == subquery.c.content_id))
         tmp = query.distinct()
 
         rets = []
         if tmp:
             for t in tmp:
                 t2 = dict(zip(t.keys(), t))
                 rets.append(t2)
@@ -650,31 +684,111 @@
     except IntegrityError as error:
         raise exceptions.DuplicatedObject('Duplicated objects: %s' % (error))
     except DatabaseError as error:
         raise exceptions.DatabaseException(error)
 
 
 @transactional_session
-def delete_contents_update(request_id=None, transform_id=None, session=None):
+def set_fetching_contents_update(request_id=None, transform_id=None, fetch=True, session=None):
+    """
+    Set fetching contents update.
+
+    :param session: session.
+    """
+    try:
+        if fetch:
+            query = session.query(models.Content_update)
+            if request_id:
+                query = query.filter(models.Content_update.request_id == request_id)
+            if transform_id:
+                query = query.filter(models.Content_update.transform_id == transform_id)
+            query.update({'fetch_status': ContentFetchStatus.Fetching})
+    except sqlalchemy.orm.exc.NoResultFound as error:
+        raise exceptions.NoObject('No record can be found with (transform_id=%s): %s' %
+                                  (transform_id, error))
+    except Exception as error:
+        raise error
+
+
+@read_session
+def get_contents_update(request_id=None, transform_id=None, fetch=False, session=None):
+    """
+    Get contents update.
+
+    :param session: session.
+    """
+    try:
+        if fetch:
+            query = session.query(models.Content_update)
+            if request_id:
+                query = query.filter(models.Content_update.request_id == request_id)
+            if transform_id:
+                query = query.filter(models.Content_update.transform_id == transform_id)
+            query = query.filter(models.Content_update.fetch_status == ContentFetchStatus.Fetching)
+        else:
+            query = session.query(models.Content_update)
+            if request_id:
+                query = query.filter(models.Content_update.request_id == request_id)
+            if transform_id:
+                query = query.filter(models.Content_update.transform_id == transform_id)
+
+        tmp = query.all()
+        rets = []
+        if tmp:
+            for t in tmp:
+                rets.append(t.to_dict())
+        return rets
+    except sqlalchemy.orm.exc.NoResultFound as error:
+        raise exceptions.NoObject('No record can be found with (transform_id=%s): %s' %
+                                  (transform_id, error))
+    except Exception as error:
+        raise error
+
+
+@transactional_session
+def delete_contents_update(request_id=None, transform_id=None, contents=[], bulk_size=1000, fetch=False, session=None):
     """
     delete a content.
 
     :param session: The database session in use.
 
     :raises NoObject: If no content is founded.
     :raises DatabaseException: If there is a database error.
     """
     try:
-        del_query = session.query(models.Content_update)
-        if request_id:
-            del_query = del_query.filter(models.Content_update.request_id == request_id)
-        if transform_id:
-            del_query = del_query.filter(models.Content_update.transform_id == transform_id)
-        del_query.with_for_update(nowait=True, skip_locked=True)
-        del_query.delete()
+        if fetch:
+            del_query = session.query(models.Content_update)
+            if request_id:
+                del_query = del_query.filter(models.Content_update.request_id == request_id)
+            if transform_id:
+                del_query = del_query.filter(models.Content_update.transform_id == transform_id)
+            del_query = del_query.filter(models.Content_update.fetch_status == ContentFetchStatus.Fetching)
+            del_query.delete()
+        else:
+            if contents:
+                contents_sub_params = [contents[i:i + bulk_size] for i in range(0, len(contents), bulk_size)]
+
+                for contents_sub_param in contents_sub_params:
+                    del_query = session.query(models.Content_update)
+                    if request_id:
+                        del_query = del_query.filter(models.Content_update.request_id == request_id)
+                    if transform_id:
+                        del_query = del_query.filter(models.Content_update.transform_id == transform_id)
+                    if contents_sub_param:
+                        del_query = del_query.filter(models.Content_update.content_id.in_(contents_sub_param))
+                    del_query.with_for_update(nowait=True, skip_locked=True)
+                    del_query.delete()
+            else:
+                del_query = session.query(models.Content_update)
+                if request_id:
+                    del_query = del_query.filter(models.Content_update.request_id == request_id)
+                if transform_id:
+                    del_query = del_query.filter(models.Content_update.transform_id == transform_id)
+                del_query.with_for_update(nowait=True, skip_locked=True)
+                del_query.delete()
     except Exception as error:
         raise exceptions.NoObject('Content_update deletion error: %s' % (error))
 
 
 @transactional_session
 def add_contents_ext(contents, bulk_size=10000, session=None):
     """
@@ -745,15 +859,14 @@
 
     try:
         if status is not None:
             if not isinstance(status, (tuple, list)):
                 status = [status]
 
         query = session.query(models.Content_ext)
-        query = query.with_hint(models.Content_ext, "INDEX(CONTENTS_EXT CONTENTS_EXT_RTF_IDX)", "oracle")
         if request_id:
             query = query.filter(models.Content_ext.request_id == request_id)
         if transform_id:
             query = query.filter(models.Content_ext.transform_id == transform_id)
         if workload_id:
             query = query.filter(models.Content_ext.workload_id == workload_id)
         if coll_id:
@@ -799,15 +912,14 @@
         query = session.query(models.Content_ext.request_id,
                               models.Content_ext.transform_id,
                               models.Content_ext.workload_id,
                               models.Content_ext.coll_id,
                               models.Content_ext.content_id,
                               models.Content_ext.panda_id,
                               models.Content_ext.status)
-        query = query.with_hint(models.Content_ext, "INDEX(CONTENTS_EXT CONTENTS_EXT_RTF_IDX)", "oracle")
         if request_id:
             query = query.filter(models.Content_ext.request_id == request_id)
         if transform_id:
             query = query.filter(models.Content_ext.transform_id == transform_id)
         if workload_id:
             query = query.filter(models.Content_ext.workload_id == workload_id)
         if coll_id:
```

### Comparing `idds-server-1.1.5/lib/idds/orm/health.py` & `idds-server-1.2.0/lib/idds/orm/health.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 """
 operations related to Health.
 """
 
 import datetime
+import re
 
 from sqlalchemy.exc import DatabaseError, IntegrityError
 
 from idds.common import exceptions
 from idds.orm.base import models
 from idds.orm.base.session import read_session, transactional_session
 
@@ -38,20 +39,24 @@
 
     try:
         counts = session.query(models.Health)\
                         .filter(models.Health.agent == agent)\
                         .filter(models.Health.hostname == hostname)\
                         .filter(models.Health.pid == pid)\
                         .filter(models.Health.thread_id == thread_id)\
-                        .update({'updated_at': datetime.datetime.utcnow()})
+                        .update({'updated_at': datetime.datetime.utcnow(),
+                                 'payload': payload})
         if not counts:
             new_h = models.Health(agent=agent, hostname=hostname, pid=pid,
                                   thread_id=thread_id, thread_name=thread_name,
                                   payload=payload)
             new_h.save(session=session)
+    except IntegrityError as e:
+        if re.match('.*ORA-00001.*', e.args[0]) or re.match('.*unique constraint.*', e.args[0]):
+            print("unique constraintviolated: %s" % str(e))
     except DatabaseError as e:
         raise exceptions.DatabaseException('Could not persist message: %s' % str(e))
 
 
 @read_session
 def retrieve_health_items(session=None):
     """
@@ -71,17 +76,32 @@
                 items.append(t.to_dict())
         return items
     except IntegrityError as e:
         raise exceptions.DatabaseException(e.args)
 
 
 @transactional_session
-def clean_health(older_than=3600, session=None):
+def clean_health(older_than=3600, hostname=None, pids=[], session=None):
     """
     Clearn items which is older than the time.
 
     :param older_than in seconds
     """
 
+    query = session.query(models.Health)
+    if older_than:
+        query = query.filter(models.Health.updated_at < datetime.datetime.utcnow() - datetime.timedelta(seconds=older_than))
+    if hostname:
+        query = query.filter(models.Health.hostname == hostname)
+    if pids:
+        query = query.filter(models.Health.pid.in_(pids))
+    query.delete()
+
+
+@transactional_session
+def update_health_item_status(item, status, session=None):
     session.query(models.Health)\
-           .filter(models.Health.updated_at < datetime.datetime.utcnow() - datetime.timedelta(seconds=older_than))\
-           .delete()
+           .filter(models.Health.agent == item['agent'])\
+           .filter(models.Health.hostname == item['hostname'])\
+           .filter(models.Health.pid == item['pid'])\
+           .filter(models.Health.thread_id == item['thread_id'])\
+           .update({'status': status, 'updated_at': item['updated_at']})
```

### Comparing `idds-server-1.1.5/lib/idds/orm/messages.py` & `idds-server-1.2.0/lib/idds/orm/messages.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,22 +140,14 @@
         if msg_type is not None:
             if not isinstance(msg_type, (list, tuple)):
                 msg_type = [msg_type]
             if len(msg_type) == 1:
                 msg_type = [msg_type[0], msg_type[0]]
 
         query = session.query(models.Message)
-        if request_id is not None:
-            query = query.with_hint(models.Message, "INDEX(MESSAGES MESSAGES_TYPE_ST_IDX)", 'oracle')
-        elif transform_id:
-            query = query.with_hint(models.Message, "INDEX(MESSAGES MESSAGES_TYPE_ST_TF_IDX)", 'oracle')
-        elif processing_id is not None:
-            query = query.with_hint(models.Message, "INDEX(MESSAGES MESSAGES_TYPE_ST_PR_IDX)", 'oracle')
-        else:
-            query = query.with_hint(models.Message, "INDEX(MESSAGES MESSAGES_TYPE_ST_IDX)", 'oracle')
 
         if msg_type is not None:
             query = query.filter(models.Message.msg_type.in_(msg_type))
         if status is not None:
             query = query.filter_by(status=status)
         if source is not None:
             query = query.filter_by(source=source)
@@ -197,21 +189,31 @@
     message_condition = []
     for message in messages:
         message_condition.append(models.Message.msg_id == message['msg_id'])
 
     try:
         if message_condition:
             session.query(models.Message).\
-                with_hint(models.Message, "index(messages MESSAGES_PK)", 'oracle').\
                 filter(or_(*message_condition)).\
                 delete(synchronize_session=False)
     except IntegrityError as e:
         raise exceptions.DatabaseException(e.args)
 
 
+@transactional_session
+def clean_old_messages(request_id, session=None):
+    """
+    Delete messages whose request id is older than request_id.
+
+    :param request_id: request id..
+    """
+    session.query(models.Message)\
+           .filter(models.Message.request_id <= request_id)\
+           .delete(synchronize_session=False)
+
 # @transactional_session
 # def update_messages(messages, session=None):
 #     """
 #     Update all messages status with the given IDs.
 #
 #     :param messages: The messages to be updated as a list of dictionaries.
 #     """
```

### Comparing `idds-server-1.1.5/lib/idds/orm/processings.py` & `idds-server-1.2.0/lib/idds/orm/processings.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,16 +153,16 @@
 
     :raises NoObject: If no request is founded.
 
     :returns: Processing.
     """
 
     try:
-        query = session.query(models.Processing).with_hint(models.Processing, "INDEX(PROCESSINGS PROCESSINGS_PK)", 'oracle')\
-                                                .filter(models.Processing.processing_id == processing_id)
+        query = session.query(models.Processing)\
+                       .filter(models.Processing.processing_id == processing_id)
 
         if status:
             if not isinstance(status, (list, tuple)):
                 status = [status]
             if len(status) == 1:
                 status = [status[0], status[0]]
             query = query.filter(models.Processing.status.in_(status))
```

### Comparing `idds-server-1.1.5/lib/idds/orm/requests.py` & `idds-server-1.2.0/lib/idds/orm/requests.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,15 +156,14 @@
     """
 
     if workload_id is None:
         return exceptions.WrongParameterException("workload_id should not be None")
 
     try:
         query = session.query(models.Request.request_id)\
-                       .with_hint(models.Request, "INDEX(REQUESTS REQUESTS_SCOPE_NAME_IDX)", 'oracle')\
                        .filter(models.Request.workload_id == workload_id)
         tmp = query.all()
         ret_ids = []
         if tmp:
             for req in tmp:
                 ret_ids.append(req[0])
         return ret_ids
@@ -182,15 +181,14 @@
 
     :raises NoObject: If no request is founded.
 
     :returns: Request {name:id} dict.
     """
     try:
         query = session.query(models.Request.request_id, models.Request.name)\
-                       .with_hint(models.Request, "INDEX(REQUESTS REQUESTS_SCOPE_NAME_IDX)", "oracle")\
                        .filter(models.Request.name.like(name.replace('*', '%')))
         tmp = query.all()
         ret_ids = {}
         if tmp:
             for req in tmp:
                 ret_ids[req[1]] = req[0]
         return ret_ids
@@ -228,16 +226,16 @@
 
     :raises NoObject: If no request is founded.
 
     :returns: Request.
     """
 
     try:
-        query = session.query(models.Request).with_hint(models.Request, "INDEX(REQUESTS REQUESTS_SCOPE_NAME_IDX)", 'oracle')\
-                                             .filter(models.Request.request_id == request_id)
+        query = session.query(models.Request)\
+                       .filter(models.Request.request_id == request_id)
 
         ret = query.first()
         if not ret:
             return None
         else:
             if to_json:
                 return ret.to_dict_json()
@@ -260,16 +258,16 @@
 
     :raises NoObject: If no request is founded.
 
     :returns: Request.
     """
 
     try:
-        query = session.query(models.Request).with_hint(models.Request, "INDEX(REQUESTS REQUESTS_PK)", 'oracle')\
-                                             .filter(models.Request.request_id == request_id)
+        query = session.query(models.Request)\
+                       .filter(models.Request.request_id == request_id)
 
         if status:
             if not isinstance(status, (list, tuple)):
                 status = [status]
             if len(status) == 1:
                 status = [status[0], status[0]]
             query = query.filter(models.Request.status.in_(status))
@@ -301,16 +299,15 @@
     :raises NoObject: If no request is founded.
 
     :returns: Request.
     """
     try:
         if with_request or not (with_transform or with_processing or with_detail or with_metadata):
             if with_metadata:
-                query = session.query(models.Request)\
-                               .with_hint(models.Request, "INDEX(REQUESTS REQUESTS_SCOPE_NAME_IDX)", 'oracle')
+                query = session.query(models.Request)
 
                 if request_id:
                     query = query.filter(models.Request.request_id == request_id)
                 if workload_id:
                     query = query.filter(models.Request.workload_id == workload_id)
 
                 tmp = query.all()
@@ -338,16 +335,15 @@
                                       models.Request.substatus,
                                       models.Request.locking,
                                       models.Request.created_at,
                                       models.Request.updated_at,
                                       models.Request.next_poll_at,
                                       models.Request.accessed_at,
                                       models.Request.expired_at,
-                                      models.Request.errors)\
-                               .with_hint(models.Request, "INDEX(REQUESTS REQUESTS_SCOPE_NAME_IDX)", 'oracle')
+                                      models.Request.errors)
 
                 if request_id:
                     query = query.filter(models.Request.request_id == request_id)
                 if workload_id:
                     query = query.filter(models.Request.workload_id == workload_id)
 
                 tmp = query.all()
@@ -763,15 +759,14 @@
     :raises NoObject: If no request is founded.
 
     :returns: list of Request.
     """
 
     try:
         query = session.query(models.Request)\
-                       .with_hint(models.Request, "INDEX(REQUESTS REQUESTS_SCOPE_NAME_IDX)", 'oracle')\
                        .filter(models.Request.requester == requester)\
                        .filter(models.Request.scope == scope)\
                        .filter(models.Request.name.like(name.replace('*', '%')))
         tmp = query.all()
         rets = []
         if tmp:
             for req in tmp:
@@ -806,19 +801,17 @@
         if status:
             if not isinstance(status, (list, tuple)):
                 status = [status]
             if len(status) == 1:
                 status = [status[0], status[0]]
 
         if only_return_id:
-            query = session.query(models.Request.request_id)\
-                           .with_hint(models.Request, "INDEX(REQUESTS REQUESTS_SCOPE_NAME_IDX)", 'oracle')
+            query = session.query(models.Request.request_id)
         else:
-            query = session.query(models.Request)\
-                           .with_hint(models.Request, "INDEX(REQUESTS REQUESTS_SCOPE_NAME_IDX)", 'oracle')
+            query = session.query(models.Request)
 
         if status:
             if by_substatus:
                 query = query.filter(models.Request.substatus.in_(status))
             else:
                 query = query.filter(models.Request.status.in_(status))
         if new_poll:
@@ -958,7 +951,33 @@
         status = [status]
     if len(status) == 1:
         status = [status[0], status[0]]
 
     params = {'next_poll_at': datetime.datetime.utcnow()}
     session.query(models.Request).filter(models.Request.status.in_(status))\
            .update(params, synchronize_session=False)
+
+
+@read_session
+def get_last_request_id(status, older_than=None, session=None):
+    """
+    Get last request id which is older than a timestamp.
+
+    :param status: status of the request.
+    :param older_than: days older than current timestamp.
+
+    :returns request_id
+    """
+    if not isinstance(status, (list, tuple)):
+        status = [status]
+    if len(status) == 1:
+        status = [status[0], status[0]]
+
+    query = session.query(models.Request.request_id)
+    if status:
+        query = query.filter(models.Request.status.in_(status))
+    query = query.filter(models.Request.updated_at <= datetime.datetime.utcnow() - datetime.timedelta(days=older_than))
+    query = query.order_by(desc(models.Request.request_id))
+    ret = query.first()
+    if ret:
+        return ret[0]
+    return ret
```

### Comparing `idds-server-1.1.5/lib/idds/orm/transforms.py` & `idds-server-1.2.0/lib/idds/orm/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,16 +195,16 @@
 
     :raises NoObject: If no request is founded.
 
     :returns: Transform.
     """
 
     try:
-        query = session.query(models.Transform).with_hint(models.Transform, "INDEX(TRANSFORMS TRANSFORMS_PK)", 'oracle')\
-                                               .filter(models.Transform.transform_id == transform_id)
+        query = session.query(models.Transform)\
+                       .filter(models.Transform.transform_id == transform_id)
 
         if status:
             if not isinstance(status, (list, tuple)):
                 status = [status]
             if len(status) == 1:
                 status = [status[0], status[0]]
             query = query.filter(models.Transform.status.in_(status))
```

### Comparing `idds-server-1.1.5/lib/idds/orm/workprogress.py` & `idds-server-1.2.0/lib/idds/orm/workprogress.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,16 +131,15 @@
 
     :raises NoObject: If no workprogress is founded.
 
     :returns: list of workprogresses.
     """
 
     try:
-        query = session.query(models.Workprogress)\
-                       .with_hint(models.Workprogress, "INDEX(WORKPROGRESSES WORKPROGRESS_PK)", 'oracle')
+        query = session.query(models.Workprogress)
         if request_id is not None:
             query = query.filter(models.Workprogress.request_id == request_id)
         tmp = query.all()
         rets = []
         if tmp:
             for t in tmp:
                 if to_json:
@@ -165,15 +164,14 @@
     :raises NoObject: If no workprogress is founded.
 
     :returns: Workprogress.
     """
 
     try:
         query = session.query(models.Workprogress)\
-                       .with_hint(models.Workprogress, "INDEX(WORKPROGRESSES WORKPROGRESS_PK)", 'oracle')\
                        .filter(models.Workprogress.workprogress_id == workprogress_id)
 
         ret = query.first()
         if not ret:
             return None
         else:
             if to_json:
@@ -204,15 +202,14 @@
             raise exceptions.WrongParameterException("status should not be None")
         if not isinstance(status, (list, tuple)):
             status = [status]
         if len(status) == 1:
             status = [status[0], status[0]]
 
         query = session.query(models.Workprogress)\
-                       .with_hint(models.Workprogress, "INDEX(WORKPROGRESSES WORKPROGRESS_STATUS_PRIO_IDX)", 'oracle')\
                        .filter(models.Workprogress.status.in_(status))\
                        .filter(models.Workprogress.next_poll_at < datetime.datetime.utcnow())
 
         if period is not None:
             query = query.filter(models.Workprogress.updated_at < datetime.datetime.utcnow() - datetime.timedelta(seconds=period))
         if locking:
             query = query.filter(models.Workprogress.locking == WorkprogressLocking.Idle)
```

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/app.py` & `idds-server-1.2.0/lib/idds/rest/v1/app.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/auth.py` & `idds-server-1.2.0/lib/idds/rest/v1/auth.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/cacher.py` & `idds-server-1.2.0/lib/idds/rest/v1/cacher.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/catalog.py` & `idds-server-1.2.0/lib/idds/rest/v1/catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/controller.py` & `idds-server-1.2.0/lib/idds/rest/v1/controller.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/hyperparameteropt.py` & `idds-server-1.2.0/lib/idds/rest/v1/hyperparameteropt.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/logs.py` & `idds-server-1.2.0/lib/idds/rest/v1/logs.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/messages.py` & `idds-server-1.2.0/lib/idds/rest/v1/messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/monitor.py` & `idds-server-1.2.0/lib/idds/rest/v1/monitor.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/ping.py` & `idds-server-1.2.0/lib/idds/rest/v1/ping.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/requests.py` & `idds-server-1.2.0/lib/idds/rest/v1/requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/rest/v1/utils.py` & `idds-server-1.2.0/lib/idds/rest/v1/utils.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/activelearning_test.py` & `idds-server-1.2.0/lib/idds/tests/activelearning_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/auth_test_script.py` & `idds-server-1.2.0/lib/idds/tests/auth_test_script.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/cacher_test.py` & `idds-server-1.2.0/lib/idds/tests/cacher_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/catalog_test.py` & `idds-server-1.2.0/lib/idds/tests/catalog_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/client_test.py` & `idds-server-1.2.0/lib/idds/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/common.py` & `idds-server-1.2.0/lib/idds/tests/common.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/core_tests.py` & `idds-server-1.2.0/lib/idds/tests/core_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,27 +167,34 @@
 # reqs = get_requests(request_id=372678, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=373602, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=376086, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=380474, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=381520, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=28182323, with_request=True, with_detail=False, with_metadata=True)
 # reqs = get_requests(request_id=385554, with_request=True, with_detail=False, with_metadata=True)
-reqs = get_requests(request_id=474, with_request=True, with_detail=False, with_metadata=True)
+reqs = get_requests(request_id=458999, with_request=True, with_detail=False, with_metadata=True)
 for req in reqs:
     # print(req['request_id'])
     # print(req)
     # print(rets)
     # print(json_dumps(req, sort_keys=True, indent=4))
     # show_works(req)
     pass
-    workflow = req['request_metadata']['build_workflow']
-    # workflow.get_new_works()
-    print(workflow.runs.keys())
-    # print(workflow.runs["1"])
-    print(json_dumps(workflow.runs["1"], sort_keys=True, indent=4))
+    if 'build_workflow' in req['request_metadata']:
+        workflow = req['request_metadata']['build_workflow']
+        # workflow.get_new_works()
+        print(workflow.runs.keys())
+        # print(workflow.runs["1"])
+        print(json_dumps(workflow.runs["1"], sort_keys=True, indent=4))
+    elif 'workflow' in req['request_metadata']:
+        workflow = req['request_metadata']['workflow']
+        # workflow.get_new_works()
+        print(workflow.runs.keys())
+        # print(workflow.runs["1"])
+        print(json_dumps(workflow.runs["1"], sort_keys=True, indent=4))
 
     # print(workflow.runs["1"].works.keys())
     # print(workflow.runs["1"].has_loop_condition())
     # print(workflow.runs["1"].works["7aa1ec08"])
     # print(json_dumps(workflow.runs["1"].works["048a1811"], indent=4))
     # print(workflow.runs["1"].works["7aa1ec08"].runs.keys())
     # print(workflow.runs["1"].works["7aa1ec08"].runs["1"].has_loop_condition())
@@ -204,18 +211,21 @@
     print('new_works:' + str(new_works))
     all_works = workflow.get_all_works()
     print('all_works:' + str(all_works))
     for work in all_works:
         print("work %s signature: %s" % (work.get_work_id(), work.signature))
 
     # print("workflow template")
-    # print_workflow_template(workflow)
+    print_workflow_template(workflow)
 
     # workflow.sync_works()
 
+    print("workflow template")
+    print(json_dumps(workflow.template, sort_keys=True, indent=4))
+
 sys.exit(0)
 
 reqs = get_requests(request_id=28182323, with_request=False, with_detail=True, with_metadata=False)
 for req in reqs:
     print(json_dumps(req, sort_keys=True, indent=4))
 
 # sys.exit(0)
```

### Comparing `idds-server-1.1.5/lib/idds/tests/core_tests_dep_id.py` & `idds-server-1.2.0/lib/idds/tests/core_tests_dep_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/core_tests_stat.py` & `idds-server-1.2.0/lib/idds/tests/core_tests_stat.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/datacarousel_test.py` & `idds-server-1.2.0/lib/idds/tests/datacarousel_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/doma_build_test.py` & `idds-server-1.2.0/lib/idds/tests/doma_build_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/find_dependencies.py` & `idds-server-1.2.0/lib/idds/tests/find_dependencies.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/fix_content_dep_id.py` & `idds-server-1.2.0/lib/idds/tests/fix_content_dep_id.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/fix_trasnform_name.py` & `idds-server-1.2.0/lib/idds/tests/fix_trasnform_name.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/hyperparameteropt_bayesian_test.py` & `idds-server-1.2.0/lib/idds/tests/hyperparameteropt_bayesian_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/hyperparameteropt_client_test.py` & `idds-server-1.2.0/lib/idds/tests/hyperparameteropt_client_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/hyperparameteropt_docker_local_test.py` & `idds-server-1.2.0/lib/idds/tests/hyperparameteropt_docker_local_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/hyperparameteropt_docker_test.py` & `idds-server-1.2.0/lib/idds/tests/hyperparameteropt_docker_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/hyperparameteropt_nevergrad_test.py` & `idds-server-1.2.0/lib/idds/tests/hyperparameteropt_nevergrad_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/jsonload_test.py` & `idds-server-1.2.0/lib/idds/tests/jsonload_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/kill_workflow_task.py` & `idds-server-1.2.0/lib/idds/tests/kill_workflow_task.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/logs_test.py` & `idds-server-1.2.0/lib/idds/tests/logs_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/match_test.py` & `idds-server-1.2.0/lib/idds/tests/match_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/message_test.py` & `idds-server-1.2.0/lib/idds/tests/message_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/message_test1.py` & `idds-server-1.2.0/lib/idds/tests/message_test1.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/migrating_requests_v1_to_v2.py` & `idds-server-1.2.0/lib/idds/tests/migrating_requests_v1_to_v2.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/panda_iam_test.py` & `idds-server-1.2.0/lib/idds/tests/panda_iam_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/panda_test.py` & `idds-server-1.2.0/lib/idds/tests/panda_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,20 @@
 # task_ids = [3834, 3835, 3836]
 # task_ids = [i for i in range(141294, 142200)] + [i for i in range(141003, 141077)] + [i for i in range(141145, 141255)]
 # task_ids = [140954, 140955, 142228]
 # task_ids = [i for i in range(142507, 142651)]
 # task_ids = [i for i in range(140349, 140954)] + [142268, 142651]
 # task_ids = [1851] + [i for i in range(4336, 4374)] + [i for i in range(133965, 136025)]
 # task_ids = [832, 2347, 3045, 66860, 67036] + [i for i in range(121273, 140349)]
-task_ids = [i for i in range(144088, 144111)] + [144891, 144892]
+# task_ids = [i for i in range(144088, 144111)] + [144891, 144892]
+# task_ids = [i for i in range(150050, 150065)]
+# task_ids = [150607, 150619, 150649, 150637, 150110, 150111]
+# task_ids = [150864, 150897, 150910]
+# task_ids = [151114, 151115]
+task_ids = [i for i in range(151444, 151453)]
 # task_ids = []
 for task_id in task_ids:
     print("Killing %s" % task_id)
     Client.killTask(task_id)
 
 """
 jobids = []
```

### Comparing `idds-server-1.1.5/lib/idds/tests/performance_test_with_cx_oracle.py` & `idds-server-1.2.0/lib/idds/tests/performance_test_with_cx_oracle.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/performance_test_with_sqlalchemy.py` & `idds-server-1.2.0/lib/idds/tests/performance_test_with_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/relation_map_test.py` & `idds-server-1.2.0/lib/idds/tests/relation_map_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/rest_test.py` & `idds-server-1.2.0/lib/idds/tests/rest_test.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/run_sql.py` & `idds-server-1.2.0/lib/idds/tests/run_sql.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/scaling_checks.py` & `idds-server-1.2.0/lib/idds/tests/scaling_checks.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/split_messages.py` & `idds-server-1.2.0/lib/idds/tests/split_messages.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_activelearning.py` & `idds-server-1.2.0/lib/idds/tests/test_activelearning.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_atlaspandawork.py` & `idds-server-1.2.0/lib/idds/tests/test_atlaspandawork.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_auth.py` & `idds-server-1.2.0/lib/idds/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_big_request.py` & `idds-server-1.2.0/lib/idds/tests/test_big_request.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_catalog.py` & `idds-server-1.2.0/lib/idds/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_client.py` & `idds-server-1.2.0/lib/idds/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_datacarousel.py` & `idds-server-1.2.0/lib/idds/tests/test_datacarousel.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_domapanda.py` & `idds-server-1.2.0/lib/idds/tests/test_domapanda.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_domapanda_pandaclient.py` & `idds-server-1.2.0/lib/idds/tests/test_domapanda_pandaclient.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_domapanda_workflow.py` & `idds-server-1.2.0/lib/idds/tests/test_domapanda_workflow.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_get_dn.py` & `idds-server-1.2.0/lib/idds/tests/test_get_dn.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,22 +16,26 @@
 # /DC=ch/DC=cern/OU=Organic Units/OU=Users/CN=wguan/CN=667815/CN=Wen Guan/CN=1883443395
 def get_user_name_from_dn1(dn):
     try:
         up = re.compile('/(DC|O|OU|C|L)=[^\/]+')        # noqa W605
         username = up.sub('', dn)
         up2 = re.compile('/CN=[0-9]+')
         username = up2.sub('', username)
-        up3 = re.compile(' [0-9]+')
-        username = up3.sub('', username)
-        up4 = re.compile('_[0-9]+')
+        up4 = re.compile(' [0-9]+')
         username = up4.sub('', username)
+        up5 = re.compile('_[0-9]+')
+        username = up5.sub('', username)
         username = username.replace('/CN=proxy', '')
         username = username.replace('/CN=limited proxy', '')
         username = username.replace('limited proxy', '')
+        username = re.sub('/CN=Robot:[^/]+,', ',', username)
         username = re.sub('/CN=Robot:[^/]+', '', username)
+        username = re.sub('/CN=Robot[^/]+,', ',', username)
+        username = re.sub('/CN=Robot[^/]+', '', username)
+        username = re.sub('/CN=nickname:[^/]+,', ',', username)
         username = re.sub('/CN=nickname:[^/]+', '', username)
         pat = re.compile('.*/CN=([^\/]+)/CN=([^\/]+)')         # noqa W605
         mat = pat.match(username)
         if mat:
             username = mat.group(2)
         else:
             username = username.replace('/CN=', '')
@@ -52,22 +56,28 @@
 # 'CN=203633261,CN=Wen Guan,CN=667815,CN=wguan,OU=Users,OU=Organic Units,DC=cern,DC=ch'
 def get_user_name_from_dn2(dn):
     try:
         up = re.compile(',(DC|O|OU|C|L)=[^\,]+')        # noqa W605
         username = up.sub('', dn)
         up2 = re.compile(',CN=[0-9]+')
         username = up2.sub('', username)
-        up3 = re.compile(' [0-9]+')
-        username = up3.sub('', username)
-        up4 = re.compile('_[0-9]+')
+        up3 = re.compile('CN=[0-9]+,')
+        username = up3.sub(',', username)
+        up4 = re.compile(' [0-9]+')
         username = up4.sub('', username)
+        up5 = re.compile('_[0-9]+')
+        username = up5.sub('', username)
         username = username.replace(',CN=proxy', '')
         username = username.replace(',CN=limited proxy', '')
         username = username.replace('limited proxy', '')
+        username = re.sub(',CN=Robot:[^/]+,', ',', username)
         username = re.sub(',CN=Robot:[^/]+', '', username)
+        username = re.sub(',CN=Robot[^/]+,', ',', username)
+        username = re.sub(',CN=Robot[^/]+', '', username)
+        username = re.sub(',CN=nickname:[^/]+,', ',', username)
         username = re.sub(',CN=nickname:[^/]+', '', username)
         pat = re.compile('.*,CN=([^\,]+),CN=([^\,]+)')         # noqa W605
         mat = pat.match(username)
         if mat:
             username = mat.group(1)
         else:
             username = username.replace(',CN=', '')
@@ -105,7 +115,13 @@
     print("auth: " + username)
 
     dn = "/DC=ch/DC=cern/OU=Organic+Units/OU=Users/CN=atlpilo1/CN=614260/CN=Robot%3A+ATLAS+Pilot1"
     username = get_user_name_from_dn(dn)
     print(username)
     username = authentication.get_user_name_from_dn(dn)
     print("auth: " + username)
+
+    dn = "CN=1316551436,CN=Robot: ATLAS Panda Server1,CN=663551,CN=pandasv1,OU=Users,OU=Organic Units,DC=cern,DC=ch"
+    username = get_user_name_from_dn(dn)
+    print(username)
+    username = authentication.get_user_name_from_dn(dn)
+    print("auth: " + username)
```

### Comparing `idds-server-1.1.5/lib/idds/tests/test_hyperparameteropt.py` & `idds-server-1.2.0/lib/idds/tests/test_hyperparameteropt.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_logger.py` & `idds-server-1.2.0/lib/idds/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_migrate_requests.py` & `idds-server-1.2.0/lib/idds/tests/test_migrate_requests.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,26 +50,30 @@
     old_request_id = 2400
     old_request_id = 371204
     old_request_id = 372930
     old_request_id = 2603
     old_request_id = 2802
     old_request_id = 2816       # big tasks
     # old_request_id = 3178     # 125 tasks
+    old_request_id = 3578
+    old_request_id = 3612
+    old_request_id = 3628
 
+    old_request_ids = [3628]
     # old_request_id = 1
     # for old_request_id in [152]:
     # for old_request_id in [60]:    # noqa E115
     # for old_request_id in [200]:    # noqa E115
-    for old_request_id in [old_request_id]:    # noqa E115  # doma 183
+    for old_request_id in old_request_ids:    # noqa E115  # doma 183
         reqs = cm1.get_requests(request_id=old_request_id, with_metadata=True)
 
-        # cm2 = ClientManager(host=dev_host)
+        cm2 = ClientManager(host=dev_host)
         # cm2 = ClientManager(host=doma_host)
         # cm2 = ClientManager(host=atlas_host)
-        cm2 = ClientManager(host=slac_k8s_dev_host)
+        # cm2 = ClientManager(host=slac_k8s_dev_host)
         # cm2 = ClientManager(host=cern_k8s_dev_host)
         # print(reqs)
 
         print("num requests: %s" % len(reqs))
         for req in reqs[:1]:
             # print(req)
             # workflow = req['request_metadata']['workflow']
```

### Comparing `idds-server-1.1.5/lib/idds/tests/test_request_transform.py` & `idds-server-1.2.0/lib/idds/tests/test_request_transform.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_requests.py` & `idds-server-1.2.0/lib/idds/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_running_data.py` & `idds-server-1.2.0/lib/idds/tests/test_running_data.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_scaling.py` & `idds-server-1.2.0/lib/idds/tests/test_scaling.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_transform_collection_content.py` & `idds-server-1.2.0/lib/idds/tests/test_transform_collection_content.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_transform_processing.py` & `idds-server-1.2.0/lib/idds/tests/test_transform_processing.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_workflow.py` & `idds-server-1.2.0/lib/idds/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_workflow_condition.py` & `idds-server-1.2.0/lib/idds/tests/test_workflow_condition.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/test_workflow_condition_v2.py` & `idds-server-1.2.0/lib/idds/tests/test_workflow_condition_v2.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds/tests/trigger_release.py` & `idds-server-1.2.0/lib/idds/tests/trigger_release.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/lib/idds_server.egg-info/PKG-INFO` & `idds-server-1.2.0/lib/idds_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-server
-Version: 1.1.5
+Version: 1.2.0
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-server-1.1.5/lib/idds_server.egg-info/SOURCES.txt` & `idds-server-1.2.0/lib/idds_server.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,18 +35,22 @@
 etc/idds/website/25-port443.conf
 etc/idds/website/25-port80.conf
 etc/sql/oracle_11.sql
 etc/sql/oracle_11_test.sql
 etc/sql/oracle_19.sql
 etc/sql/oracle_update.sql
 etc/sql/postgresql.sql
+etc/sql/postgresql_init.sql
 lib/idds/__init__.py
 lib/idds/version.py
 lib/idds/agents/__init__.py
 lib/idds/agents/main.py
+lib/idds/agents/archive/__init__.py
+lib/idds/agents/archive/archiver.py
+lib/idds/agents/archive/run_archive.py
 lib/idds/agents/carrier/__init__.py
 lib/idds/agents/carrier/finisher.py
 lib/idds/agents/carrier/poller.py
 lib/idds/agents/carrier/receiver.py
 lib/idds/agents/carrier/submitter.py
 lib/idds/agents/carrier/trigger.py
 lib/idds/agents/carrier/utils.py
@@ -55,22 +59,27 @@
 lib/idds/agents/common/__init__.py
 lib/idds/agents/common/baseagent.py
 lib/idds/agents/common/timerscheduler.py
 lib/idds/agents/common/timertask.py
 lib/idds/agents/common/cache/__init__.py
 lib/idds/agents/common/cache/redis.py
 lib/idds/agents/common/eventbus/__init__.py
+lib/idds/agents/common/eventbus/baseeventbusbackend.py
+lib/idds/agents/common/eventbus/baseeventbusbackendopt.py
+lib/idds/agents/common/eventbus/dbeventbusbackend.py
 lib/idds/agents/common/eventbus/event.py
 lib/idds/agents/common/eventbus/eventbus.py
-lib/idds/agents/common/eventbus/localeventbusbackend.py
+lib/idds/agents/common/eventbus/msgeventbusbackend.py
 lib/idds/agents/common/plugins/__init__.py
 lib/idds/agents/common/plugins/messaging.py
 lib/idds/agents/conductor/__init__.py
 lib/idds/agents/conductor/conductor.py
 lib/idds/agents/conductor/consumer.py
+lib/idds/agents/coordinator/__init__.py
+lib/idds/agents/coordinator/coordinator.py
 lib/idds/agents/marshaller/__init__.py
 lib/idds/agents/marshaller/marshaller.py
 lib/idds/agents/transformer/__init__.py
 lib/idds/agents/transformer/transformer.py
 lib/idds/agents/transporter/__init__.py
 lib/idds/agents/transporter/transporter.py
 lib/idds/api/__init__.py
@@ -79,24 +88,26 @@
 lib/idds/api/contents.py
 lib/idds/api/processings.py
 lib/idds/api/requests.py
 lib/idds/api/transforms.py
 lib/idds/core/__init__.py
 lib/idds/core/catalog.py
 lib/idds/core/commands.py
+lib/idds/core/events.py
 lib/idds/core/health.py
 lib/idds/core/messages.py
 lib/idds/core/processings.py
 lib/idds/core/requests.py
 lib/idds/core/transforms.py
 lib/idds/core/workprogress.py
 lib/idds/orm/__init__.py
 lib/idds/orm/collections.py
 lib/idds/orm/commands.py
 lib/idds/orm/contents.py
+lib/idds/orm/events.py
 lib/idds/orm/health.py
 lib/idds/orm/messages.py
 lib/idds/orm/processings.py
 lib/idds/orm/requests.py
 lib/idds/orm/transforms.py
 lib/idds/orm/workprogress.py
 lib/idds/orm/base/__init__.py
@@ -168,14 +179,15 @@
 lib/idds/tests/test_datacarousel.py
 lib/idds/tests/test_domapanda.py
 lib/idds/tests/test_domapanda_pandaclient.py
 lib/idds/tests/test_domapanda_workflow.py
 lib/idds/tests/test_get_dn.py
 lib/idds/tests/test_hyperparameteropt.py
 lib/idds/tests/test_logger.py
+lib/idds/tests/test_merge_dict.py
 lib/idds/tests/test_migrate_requests.py
 lib/idds/tests/test_property.py
 lib/idds/tests/test_request_transform.py
 lib/idds/tests/test_requests.py
 lib/idds/tests/test_running_data.py
 lib/idds/tests/test_scaling.py
 lib/idds/tests/test_transform_collection_content.py
@@ -190,14 +202,15 @@
 lib/idds_server.egg-info/requires.txt
 lib/idds_server.egg-info/top_level.txt
 tools/env/config_monitor.py
 tools/env/config_server
 tools/env/create_database.py
 tools/env/create_postgres_db.sh
 tools/env/destroy_database.py
+tools/env/dump_database.py
 tools/env/environment.yml
 tools/env/install_env_conda.sh
 tools/env/install_idds.sh
 tools/env/install_idds_full.sh
 tools/env/install_packages.sh
 tools/env/merge_configmap.py
 tools/env/merge_idds_configs.py
```

### Comparing `idds-server-1.1.5/setup.py` & `idds-server-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/tools/env/config_monitor.py` & `idds-server-1.2.0/tools/env/config_monitor.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/tools/env/create_database.py` & `idds-server-1.2.0/tools/env/create_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/tools/env/destroy_database.py` & `idds-server-1.2.0/tools/env/destroy_database.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/tools/env/environment.yml` & `idds-server-1.2.0/tools/env/environment.yml`

 * *Files 4% similar despite different names*

```diff
@@ -24,10 +24,12 @@
   - sphinx-rtd-theme                 # sphinx readthedoc theme
   - nevergrad                        # nevergrad hyper parameter optimization
   - psycopg2-binary
   - pyjwt
   - cryptography
   - redis
   - alembic
-  - idds-common==1.1.5
-  - idds-workflow==1.1.5
-  - idds-client==1.1.5
+  - deepdiff
+  - pyzmq
+  - idds-common==1.2.0
+  - idds-workflow==1.2.0
+  - idds-client==1.2.0
```

### Comparing `idds-server-1.1.5/tools/env/install_env_conda.sh` & `idds-server-1.2.0/tools/env/install_env_conda.sh`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/tools/env/install_idds_full.sh` & `idds-server-1.2.0/tools/env/install_idds_full.sh`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/tools/env/merge_configmap.py` & `idds-server-1.2.0/tools/env/merge_configmap.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/tools/env/merge_idds_configs.py` & `idds-server-1.2.0/tools/env/merge_idds_configs.py`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/tools/env/setup_dev.sh` & `idds-server-1.2.0/tools/env/setup_dev.sh`

 * *Files identical despite different names*

### Comparing `idds-server-1.1.5/tools/env/setup_panda.sh` & `idds-server-1.2.0/tools/env/setup_panda.sh`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     export PANDA_VERIFY_HOST=off
     export PANDA_URL_SSL=https://rubin-panda-server-dev.slac.stanford.edu:8443/server/panda
     export PANDA_URL=http://rubin-panda-server-dev.slac.stanford.edu:80/server/panda
     export PANDAMON_URL=https://rubin-panda-bigmon-dev.slac.stanford.edu
     export PANDA_AUTH_VO=Rubin
 
     export PANDACACHE_URL=$PANDA_URL_SSL
+    export PANDA_SYS=/afs/cern.ch/user/w/wguan/workdisk/iDDS/.conda/iDDS/
+
     # export PANDA_CONFIG_ROOT=/afs/cern.ch/user/w/wguan/workdisk/iDDS/main/etc/panda/
     export PANDA_CONFIG_ROOT=~/.panda/
 else
     export PANDA_AUTH=oidc
     export PANDA_URL_SSL=https://pandaserver-doma.cern.ch:25443/server/panda
     export PANDA_URL=http://pandaserver-doma.cern.ch:25080/server/panda
     export PANDAMON_URL=https://panda-doma.cern.ch
```

