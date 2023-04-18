# Comparing `tmp/module-build-service-3.9.0.tar.gz` & `tmp/module-build-service-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module-build-service-3.9.0.tar", last modified: Tue Apr 18 15:15:48 2023, max compression
+gzip compressed data, was "module-build-service-3.9.2.tar", last modified: Tue Apr 18 16:25:36 2023, max compression
```

## Comparing `module-build-service-3.9.0.tar` & `module-build-service-3.9.2.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.463877 module-build-service-3.9.0/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1057 2023-03-24 19:41:06.000000 module-build-service-3.9.0/LICENSE
--rw-r--r--   0 breilly   (1000) breilly   (1000)      566 2023-04-04 16:42:49.000000 module-build-service-3.9.0/MANIFEST.in
--rw-r--r--   0 breilly   (1000) breilly   (1000)      445 2023-04-18 15:15:48.463877 module-build-service-3.9.0/PKG-INFO
--rw-r--r--   0 breilly   (1000) breilly   (1000)    30837 2023-04-04 16:42:49.000000 module-build-service-3.9.0/README.rst
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.450877 module-build-service-3.9.0/client/
--rwxr-xr-x   0 breilly   (1000) breilly   (1000)    11007 2023-03-24 19:41:06.000000 module-build-service-3.9.0/client/mbs-cli
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.450877 module-build-service-3.9.0/conf/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      474 2023-03-24 19:41:06.000000 module-build-service-3.9.0/conf/client_secrets.json
--rw-r--r--   0 breilly   (1000) breilly   (1000)      693 2023-03-24 19:41:06.000000 module-build-service-3.9.0/conf/koji.conf
--rw-r--r--   0 breilly   (1000) breilly   (1000)      491 2023-03-24 19:41:06.000000 module-build-service-3.9.0/conf/mock.cfg
--rw-r--r--   0 breilly   (1000) breilly   (1000)      268 2023-03-24 19:41:06.000000 module-build-service-3.9.0/conf/yum.conf
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.451877 module-build-service-3.9.0/docs/
--rw-r--r--   0 breilly   (1000) breilly   (1000)    21939 2023-04-18 15:10:58.000000 module-build-service-3.9.0/docs/CHANGELOG.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     8811 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/CONTRIBUTING.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)    12214 2023-03-24 19:41:06.000000 module-build-service-3.9.0/docs/DEPENDENCY_RESOLUTION.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)      373 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/GATING.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)    10279 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/HOW_MBS_BUILDS_MODULES.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3741 2023-03-24 19:41:06.000000 module-build-service-3.9.0/docs/KOJI_RESOLVER.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3629 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/MODULE_NAMING.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4050 2023-03-24 19:41:06.000000 module-build-service-3.9.0/docs/OFFLINE_LOCAL_BUILDS.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4410 2023-03-24 19:41:06.000000 module-build-service-3.9.0/docs/REBUILD_STRATEGIES.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     5151 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/STATIC_CONTEXTS.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     5129 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/VIRTUAL_MODULES.rst
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.451877 module-build-service-3.9.0/fedmsg.d/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      293 2023-03-24 19:41:06.000000 module-build-service-3.9.0/fedmsg.d/mbs-logging.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)       31 2023-03-24 19:41:06.000000 module-build-service-3.9.0/fedmsg.d/mbs-scheduler.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1746 2023-03-24 19:41:06.000000 module-build-service-3.9.0/fedmsg.d/module_build_service.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.451877 module-build-service-3.9.0/module_build_service/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2161 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/__init__.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.451877 module-build-service-3.9.0/module_build_service/builder/
--rw-r--r--   0 breilly   (1000) breilly   (1000)    36505 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/builder/KojiContentGenerator.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    53040 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/builder/KojiModuleBuilder.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    34722 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/builder/MockModuleBuilder.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      345 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/builder/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    17795 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/builder/base.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    13522 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/builder/utils.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.452877 module-build-service-3.9.0/module_build_service/common/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      355 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/common/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    40346 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/common/config.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      664 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/errors.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     6359 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/common/koji.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    18951 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/common/logger.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4786 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/messaging.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    52663 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/common/models.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      171 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/common/modulemd.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3323 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/monitor.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      840 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/common/request_utils.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     8662 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/resolve.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      993 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/common/retry.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    13555 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/scm.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4863 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     8779 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/utils.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      228 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/log_workaround.py
--rwxr-xr-x   0 breilly   (1000) breilly   (1000)     9204 2023-04-18 15:04:21.000000 module-build-service-3.9.0/module_build_service/manage.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.452877 module-build-service-3.9.0/module_build_service/migrations/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       38 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/migrations/README
--rw-r--r--   0 breilly   (1000) breilly   (1000)      800 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/migrations/alembic.ini
--rw-r--r--   0 breilly   (1000) breilly   (1000)      412 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/migrations/script.py.mako
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.453877 module-build-service-3.9.0/module_build_service/resolver/
--rw-r--r--   0 breilly   (1000) breilly   (1000)    19442 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/resolver/DBResolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    12593 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/resolver/KojiResolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1539 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/resolver/LocalResolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    23085 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/resolver/MBSResolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      569 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/resolver/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4201 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/resolver/base.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.453877 module-build-service-3.9.0/module_build_service/scheduler/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      600 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    12330 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/scheduler/batches.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    11821 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/consumer.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2686 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/db_session.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    18852 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/scheduler/default_modules.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4480 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/events.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.454877 module-build-service-3.9.0/module_build_service/scheduler/handlers/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/handlers/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     7698 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/handlers/components.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    20060 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/scheduler/handlers/modules.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     6133 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/handlers/repos.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3952 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/handlers/tags.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3115 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/scheduler/local.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4716 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/parser.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    18718 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/producer.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    20367 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/reuse.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2614 2023-04-18 15:04:21.000000 module-build-service-3.9.0/module_build_service/scheduler/route.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    24249 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/scheduler/submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    10934 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/ursine.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.454877 module-build-service-3.9.0/module_build_service/web/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     7895 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/auth.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1286 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/backports.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    32526 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/mmd_resolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    24371 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/web/mse.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1258 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/proxy.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    33713 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/web/submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    16184 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/utils.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    27146 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/web/views.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.451877 module-build-service-3.9.0/module_build_service.egg-info/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      445 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/PKG-INFO
--rw-r--r--   0 breilly   (1000) breilly   (1000)    11007 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/SOURCES.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)        1 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/dependency_links.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)      917 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/entry_points.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)        1 2023-04-18 15:14:27.000000 module-build-service-3.9.0/module_build_service.egg-info/not-zip-safe
--rw-r--r--   0 breilly   (1000) breilly   (1000)      190 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/requires.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)       27 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/top_level.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)      190 2023-04-04 16:42:49.000000 module-build-service-3.9.0/requirements.txt
--rwxr-xr-x   0 breilly   (1000) breilly   (1000)     3278 2023-03-24 19:41:06.000000 module-build-service-3.9.0/run-unittests.sh
--rw-r--r--   0 breilly   (1000) breilly   (1000)       38 2023-04-18 15:15:48.463877 module-build-service-3.9.0/setup.cfg
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3096 2023-04-18 15:05:44.000000 module-build-service-3.9.0/setup.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)       55 2023-03-24 19:41:06.000000 module-build-service-3.9.0/test-requirements.txt
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.454877 module-build-service-3.9.0/tests/
--rw-r--r--   0 breilly   (1000) breilly   (1000)    36376 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    10022 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/conftest.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/integration/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2513 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/README.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/integration/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3847 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/conftest.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     5439 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/example.test.env.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1160 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_build_stream_collision.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1592 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_buildonly.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1661 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_buildrequire_invalid_module.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1053 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_failed_build.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1031 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_highest_version_selection.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      347 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_import_module.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      574 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_no_components.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1755 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_normal_build.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1158 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_normal_build_conflict.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1793 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_rest_build_state.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1550 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_rest_submit_build.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      994 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_resume_cancelled_build.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1103 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_reuse_all_components.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1986 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_reuse_components.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4504 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_reuse_components_if_added.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2558 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_reuse_tagged_module.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      953 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_scratch_build.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1564 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_scratch_final_mmd.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      457 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_static_context.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      538 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_stream_expansion.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1545 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_v3_buildrequire.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      360 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_v3_multiple_contexts.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      364 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_v3_no_components.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1478 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_v3_normal_build.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    25074 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/utils.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/scm_data/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       23 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/HEAD
--rw-r--r--   0 breilly   (1000) breilly   (1000)       66 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/config
--rw-r--r--   0 breilly   (1000) breilly   (1000)       73 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/description
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/info/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      240 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/info/exclude
--rw-r--r--   0 breilly   (1000) breilly   (1000)       59 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/info/refs
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/34/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/34/a463979786199c1b41ca21eb309cf3ce5ce789
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/48/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/48/83b004d723a15cdc266c0280fe26c424ae10db
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/60/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      186 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/60/5345608fcc41d4e297cf062c653ebfdfe52476
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/6c/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      807 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/6c/d6a18e15a4f23a1eaa7040e7f4da9be1aed36d
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/6e/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      726 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/6e/a27c8576449ad5a12c1b6d27b50ff32c854ee5
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/7f/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      435 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/7f/96fc61223e4bc4c93c7c286cca98f6efaa3716
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/8b/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      223 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/8b/43f38cdafdd773e7d0308e758105bf9f0f67a8
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e3/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      192 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e3/ca243c664440cdb8b704b0d5c32ed433bee4da
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e4/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e4/75d55e2b78ad81f1b08bcb33a0a15ad24ef8a9
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e9/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      182 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e9/742ed681f82e3ef5281fc652b4e68a3826cea6
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/f7/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      177 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/f7/c5c7218c9a197d7fd245eeb4eee3d7abffd75d
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/fb/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      808 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/fb/9351bd6f2439a73d78de0822fefe64410f905c
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/fc/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/fc/399d16e46feb3af72a692b316a241c21bae1d0
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/info/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       54 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/info/packs
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/pack/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2584 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.idx
--rw-r--r--   0 breilly   (1000) breilly   (1000)    36836 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.pack
--rw-r--r--   0 breilly   (1000) breilly   (1000)       98 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/packed-refs
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/scm_data/mariadb/refs/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/mariadb/refs/heads/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/refs/heads/.placeholder
--rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/refs/heads/master
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/mariadb/refs/tags/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/refs/tags/.placeholder
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       23 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/HEAD
--rw-r--r--   0 breilly   (1000) breilly   (1000)       66 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/config
--rw-r--r--   0 breilly   (1000) breilly   (1000)       73 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/description
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/info/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      240 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/info/exclude
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/17/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       37 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/17/2c8d5a1db52737ebeb50fe5058212b97ac3f82
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/28/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       29 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/28/ad5b501c13fc618bb395913a2b47ad90e0f51f
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/54/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      130 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/54/81faa232d66589e660cc301179867fb00842c9
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/70/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      169 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/70/35bd33614972ac66559ac1fdd019ff6027ad21
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/b8/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       47 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/b8/f5533d9ab4cbc7a7dee0c1131dfc12e4376524
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/d5/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       48 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/d5/819330d12885aae9c026081d7959fae78eab03
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/scm_data/testrepo/refs/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/refs/heads/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/refs/heads/dev
--rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/refs/heads/master
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      824 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/bad.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      607 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/build_metadata_module.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      354 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/build_metadata_module_not_processed.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      329 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/fakemodule.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2021 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/formatted_python3-no-components.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1848 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/formatted_testmodule-more-components.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2244 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/formatted_testmodule.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      975 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/includedmodules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-child-master-20170816080815/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-child-master-20170816080815/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1449 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-child-master-20170816080815/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-parent-master-20170816080815/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-parent-master-20170816080815/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1301 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-parent-master-20170816080815/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f28-3/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f28-3/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1233 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f28-3/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f30-3/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f30-3/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      473 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f30-3/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1147 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1147 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.460877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1202 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/modules.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1273 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/staged_data/nginx_mmd.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      789 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/staged_data/platform.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1288 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/python3-no-components.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)    43738 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/shared-userspace-570.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)    43738 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/shared-userspace-577.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      783 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/staged_data/static_context_v2.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-buildrequires-f30.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1157 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/staged_data/testmodule-dashed-stream.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1205 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-forbidden-xmd.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      971 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-local-build.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1114 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-more-components.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      976 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-no-base-module.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      598 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-no-deps.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1222 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-version-set.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      988 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-with-filters.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1223 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-wrong-stream.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1163 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_br_metadata_module.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2473 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_dependencies.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_el8.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1141 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_el800.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1141 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_el821.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1387 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/staged_data/testmodule_init.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      993 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_mse.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      989 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_platform_f290000.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      977 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_v2.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1001 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_v2_buildonly.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.460877 module-build-service-3.9.0/tests/staged_data/v3/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1051 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/staged_data/v3/mmd_packager.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.460877 module-build-service-3.9.0/tests/test_build/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_build/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    78132 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_build/test_build.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.460877 module-build-service-3.9.0/tests/test_builder/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_builder/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2202 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_builder/test_base.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    12418 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_builder/test_builder_utils.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    48113 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_builder/test_content_generator.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    25714 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_builder/test_get_generator_json_expected_output.json
--rw-r--r--   0 breilly   (1000) breilly   (1000)    25982 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_builder/test_get_generator_json_expected_output_with_log.json
--rw-r--r--   0 breilly   (1000) breilly   (1000)    26558 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_builder/test_get_generator_json_rpms_in_tag.json
--rw-r--r--   0 breilly   (1000) breilly   (1000)    42030 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_builder/test_koji.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    23966 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_builder/test_mock.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.461877 module-build-service-3.9.0/tests/test_common/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      507 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_config.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      492 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_common/test_koji.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    15595 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_common/test_logger.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2875 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_messaging.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.461877 module-build-service-3.9.0/tests/test_common/test_models/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_models/__init__.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.461877 module-build-service-3.9.0/tests/test_common/test_models/data/
--rw-r--r--   0 breilly   (1000) breilly   (1000)   465266 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_models/data/base-runtime.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1259 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_models/data/testmodule.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     7947 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_models/test_models.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2995 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_monitor.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     5005 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_common/test_resolve.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     5041 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_scm.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1785 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_common/test_submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     9519 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_common/test_utils.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     9109 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_manage.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.461877 module-build-service-3.9.0/tests/test_memory/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_memory/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      942 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_memory/mbs_configuration.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1994 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_memory/mbs_debug.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3694 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_memory/test_memory.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.462877 module-build-service-3.9.0/tests/test_resolver/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_resolver/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    16076 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_resolver/test_db.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    13897 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_resolver/test_koji.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2160 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_resolver/test_local.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    26781 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_resolver/test_mbs.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.462877 module-build-service-3.9.0/tests/test_scheduler/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    17275 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_scheduler/test_batches.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4257 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_celery_route_task.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4069 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_consumer.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      865 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_db_session.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    22196 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_default_modules.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     7914 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_module_init.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4111 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_module_states.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     9215 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_module_wait.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    22637 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_scheduler/test_poller.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     9458 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_repo_done.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    22429 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_reuse.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    16164 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    22744 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_tag_tagged.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    14761 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_ursine.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.463877 module-build-service-3.9.0/tests/test_web/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_web/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      490 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_web/client_secrets.json
--rw-r--r--   0 breilly   (1000) breilly   (1000)    11913 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_web/test_auth.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    18114 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_web/test_mmd_resolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    32362 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_web/test_mse.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    17071 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_web/test_submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)   127952 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_web/test_views.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2916 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tox.ini
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.303656 module-build-service-3.9.2/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1057 2023-03-24 19:41:06.000000 module-build-service-3.9.2/LICENSE
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      566 2023-04-04 16:42:49.000000 module-build-service-3.9.2/MANIFEST.in
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      445 2023-04-18 16:25:36.303656 module-build-service-3.9.2/PKG-INFO
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    30837 2023-04-04 16:42:49.000000 module-build-service-3.9.2/README.rst
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.291656 module-build-service-3.9.2/client/
+-rwxr-xr-x   0 breilly   (1000) breilly   (1000)    11007 2023-03-24 19:41:06.000000 module-build-service-3.9.2/client/mbs-cli
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.291656 module-build-service-3.9.2/conf/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      474 2023-03-24 19:41:06.000000 module-build-service-3.9.2/conf/client_secrets.json
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      693 2023-03-24 19:41:06.000000 module-build-service-3.9.2/conf/koji.conf
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      491 2023-03-24 19:41:06.000000 module-build-service-3.9.2/conf/mock.cfg
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      268 2023-03-24 19:41:06.000000 module-build-service-3.9.2/conf/yum.conf
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.291656 module-build-service-3.9.2/docs/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    22032 2023-04-18 16:24:06.000000 module-build-service-3.9.2/docs/CHANGELOG.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     8811 2023-03-24 19:41:27.000000 module-build-service-3.9.2/docs/CONTRIBUTING.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    12214 2023-03-24 19:41:06.000000 module-build-service-3.9.2/docs/DEPENDENCY_RESOLUTION.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      373 2023-03-24 19:41:27.000000 module-build-service-3.9.2/docs/GATING.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    10279 2023-03-24 19:41:27.000000 module-build-service-3.9.2/docs/HOW_MBS_BUILDS_MODULES.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3741 2023-03-24 19:41:06.000000 module-build-service-3.9.2/docs/KOJI_RESOLVER.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3629 2023-03-24 19:41:27.000000 module-build-service-3.9.2/docs/MODULE_NAMING.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4050 2023-03-24 19:41:06.000000 module-build-service-3.9.2/docs/OFFLINE_LOCAL_BUILDS.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4410 2023-03-24 19:41:06.000000 module-build-service-3.9.2/docs/REBUILD_STRATEGIES.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     5151 2023-03-24 19:41:27.000000 module-build-service-3.9.2/docs/STATIC_CONTEXTS.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     5129 2023-03-24 19:41:27.000000 module-build-service-3.9.2/docs/VIRTUAL_MODULES.rst
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.292656 module-build-service-3.9.2/fedmsg.d/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      293 2023-03-24 19:41:06.000000 module-build-service-3.9.2/fedmsg.d/mbs-logging.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       31 2023-03-24 19:41:06.000000 module-build-service-3.9.2/fedmsg.d/mbs-scheduler.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1746 2023-03-24 19:41:06.000000 module-build-service-3.9.2/fedmsg.d/module_build_service.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.292656 module-build-service-3.9.2/module_build_service/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2161 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/__init__.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.292656 module-build-service-3.9.2/module_build_service/builder/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    36505 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/builder/KojiContentGenerator.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    53040 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/builder/KojiModuleBuilder.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    34722 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/builder/MockModuleBuilder.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      345 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/builder/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    17795 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/builder/base.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    13522 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/builder/utils.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.293656 module-build-service-3.9.2/module_build_service/common/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      355 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/common/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    40346 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/common/config.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      664 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/common/errors.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     6359 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/common/koji.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    18951 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/common/logger.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4786 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/common/messaging.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    52663 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/common/models.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      171 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/common/modulemd.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3323 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/common/monitor.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      840 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/common/request_utils.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     8662 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/common/resolve.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      993 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/common/retry.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    13555 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/common/scm.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4863 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/common/submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     8779 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/common/utils.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      228 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/log_workaround.py
+-rwxr-xr-x   0 breilly   (1000) breilly   (1000)     9430 2023-04-18 16:19:11.000000 module-build-service-3.9.2/module_build_service/manage.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.293656 module-build-service-3.9.2/module_build_service/migrations/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       38 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/migrations/README
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      800 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/migrations/alembic.ini
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      412 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/migrations/script.py.mako
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.294656 module-build-service-3.9.2/module_build_service/resolver/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    19442 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/resolver/DBResolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    12593 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/resolver/KojiResolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1539 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/resolver/LocalResolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    23085 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/resolver/MBSResolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      569 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/resolver/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4201 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/resolver/base.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.294656 module-build-service-3.9.2/module_build_service/scheduler/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      600 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/scheduler/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    12330 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/scheduler/batches.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    11821 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/scheduler/consumer.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2686 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/scheduler/db_session.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    18852 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/scheduler/default_modules.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4480 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/scheduler/events.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.294656 module-build-service-3.9.2/module_build_service/scheduler/handlers/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/scheduler/handlers/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     7698 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/scheduler/handlers/components.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    20060 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/scheduler/handlers/modules.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     6133 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/scheduler/handlers/repos.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3952 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/scheduler/handlers/tags.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3115 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/scheduler/local.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4716 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/scheduler/parser.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    18718 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/scheduler/producer.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    20367 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/scheduler/reuse.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2614 2023-04-18 15:04:21.000000 module-build-service-3.9.2/module_build_service/scheduler/route.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    24249 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/scheduler/submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    10934 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/scheduler/ursine.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.295656 module-build-service-3.9.2/module_build_service/web/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/web/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     7895 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/web/auth.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1286 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/web/backports.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    32526 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/web/mmd_resolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    24371 2023-04-04 16:42:49.000000 module-build-service-3.9.2/module_build_service/web/mse.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1258 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/web/proxy.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    33713 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/web/submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    16184 2023-03-24 19:41:06.000000 module-build-service-3.9.2/module_build_service/web/utils.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    27146 2023-03-24 19:41:27.000000 module-build-service-3.9.2/module_build_service/web/views.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.292656 module-build-service-3.9.2/module_build_service.egg-info/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      445 2023-04-18 16:25:35.000000 module-build-service-3.9.2/module_build_service.egg-info/PKG-INFO
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    11007 2023-04-18 16:25:36.000000 module-build-service-3.9.2/module_build_service.egg-info/SOURCES.txt
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        1 2023-04-18 16:25:36.000000 module-build-service-3.9.2/module_build_service.egg-info/dependency_links.txt
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      917 2023-04-18 16:25:36.000000 module-build-service-3.9.2/module_build_service.egg-info/entry_points.txt
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        1 2023-04-18 15:14:27.000000 module-build-service-3.9.2/module_build_service.egg-info/not-zip-safe
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      190 2023-04-18 16:25:36.000000 module-build-service-3.9.2/module_build_service.egg-info/requires.txt
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       27 2023-04-18 16:25:36.000000 module-build-service-3.9.2/module_build_service.egg-info/top_level.txt
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      190 2023-04-04 16:42:49.000000 module-build-service-3.9.2/requirements.txt
+-rwxr-xr-x   0 breilly   (1000) breilly   (1000)     3278 2023-03-24 19:41:06.000000 module-build-service-3.9.2/run-unittests.sh
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       38 2023-04-18 16:25:36.303656 module-build-service-3.9.2/setup.cfg
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3096 2023-04-18 16:23:44.000000 module-build-service-3.9.2/setup.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       55 2023-03-24 19:41:06.000000 module-build-service-3.9.2/test-requirements.txt
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.295656 module-build-service-3.9.2/tests/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    36376 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    10022 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/conftest.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.296656 module-build-service-3.9.2/tests/integration/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2513 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/README.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/integration/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3847 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/conftest.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     5439 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/example.test.env.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1160 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_build_stream_collision.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1592 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/test_buildonly.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1661 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_buildrequire_invalid_module.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1053 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_failed_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1031 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_highest_version_selection.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      347 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_import_module.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      574 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_no_components.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1755 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_normal_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1158 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_normal_build_conflict.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1793 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/test_rest_build_state.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1550 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/test_rest_submit_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      994 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_resume_cancelled_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1103 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_reuse_all_components.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1986 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_reuse_components.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4504 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/test_reuse_components_if_added.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2558 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_reuse_tagged_module.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      953 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_scratch_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1564 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/test_scratch_final_mmd.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      457 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/test_static_context.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      538 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/integration/test_stream_expansion.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1545 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/test_v3_buildrequire.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      360 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/test_v3_multiple_contexts.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      364 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/test_v3_no_components.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1478 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/test_v3_normal_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    25074 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/integration/utils.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.289656 module-build-service-3.9.2/tests/scm_data/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       23 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/HEAD
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       66 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/config
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       73 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/description
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/info/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      240 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/info/exclude
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       59 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/info/refs
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.289656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/34/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/34/a463979786199c1b41ca21eb309cf3ce5ce789
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/48/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/48/83b004d723a15cdc266c0280fe26c424ae10db
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/60/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      186 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/60/5345608fcc41d4e297cf062c653ebfdfe52476
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/6c/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      807 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/6c/d6a18e15a4f23a1eaa7040e7f4da9be1aed36d
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/6e/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      726 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/6e/a27c8576449ad5a12c1b6d27b50ff32c854ee5
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/7f/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      435 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/7f/96fc61223e4bc4c93c7c286cca98f6efaa3716
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/8b/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      223 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/8b/43f38cdafdd773e7d0308e758105bf9f0f67a8
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/e3/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      192 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/e3/ca243c664440cdb8b704b0d5c32ed433bee4da
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/e4/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/e4/75d55e2b78ad81f1b08bcb33a0a15ad24ef8a9
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/e9/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      182 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/e9/742ed681f82e3ef5281fc652b4e68a3826cea6
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/f7/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      177 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/f7/c5c7218c9a197d7fd245eeb4eee3d7abffd75d
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/fb/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      808 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/fb/9351bd6f2439a73d78de0822fefe64410f905c
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/fc/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/fc/399d16e46feb3af72a692b316a241c21bae1d0
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/info/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       54 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/info/packs
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.297656 module-build-service-3.9.2/tests/scm_data/mariadb/objects/pack/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2584 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.idx
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    36836 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.pack
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       98 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/packed-refs
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.289656 module-build-service-3.9.2/tests/scm_data/mariadb/refs/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/mariadb/refs/heads/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/refs/heads/.placeholder
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/refs/heads/master
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/mariadb/refs/tags/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/mariadb/refs/tags/.placeholder
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/testrepo/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       23 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/HEAD
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       66 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/config
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       73 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/description
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/testrepo/info/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      240 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/info/exclude
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.289656 module-build-service-3.9.2/tests/scm_data/testrepo/objects/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/testrepo/objects/17/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       37 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/objects/17/2c8d5a1db52737ebeb50fe5058212b97ac3f82
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/testrepo/objects/28/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       29 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/objects/28/ad5b501c13fc618bb395913a2b47ad90e0f51f
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/testrepo/objects/54/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      130 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/objects/54/81faa232d66589e660cc301179867fb00842c9
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/testrepo/objects/70/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      169 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/objects/70/35bd33614972ac66559ac1fdd019ff6027ad21
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/testrepo/objects/b8/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       47 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/objects/b8/f5533d9ab4cbc7a7dee0c1131dfc12e4376524
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/testrepo/objects/d5/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       48 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/objects/d5/819330d12885aae9c026081d7959fae78eab03
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.289656 module-build-service-3.9.2/tests/scm_data/testrepo/refs/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.298656 module-build-service-3.9.2/tests/scm_data/testrepo/refs/heads/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/refs/heads/dev
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/scm_data/testrepo/refs/heads/master
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.300656 module-build-service-3.9.2/tests/staged_data/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      824 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/bad.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      607 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/build_metadata_module.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      354 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/build_metadata_module_not_processed.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      329 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/fakemodule.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2021 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/formatted_python3-no-components.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1848 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/formatted_testmodule-more-components.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2244 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/formatted_testmodule.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      975 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/includedmodules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.290656 module-build-service-3.9.2/tests/staged_data/local_builds/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.290656 module-build-service-3.9.2/tests/staged_data/local_builds/module-child-master-20170816080815/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.300656 module-build-service-3.9.2/tests/staged_data/local_builds/module-child-master-20170816080815/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1449 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/local_builds/module-child-master-20170816080815/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.290656 module-build-service-3.9.2/tests/staged_data/local_builds/module-parent-master-20170816080815/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.300656 module-build-service-3.9.2/tests/staged_data/local_builds/module-parent-master-20170816080815/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1301 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/local_builds/module-parent-master-20170816080815/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.290656 module-build-service-3.9.2/tests/staged_data/local_builds/module-platform-f28-3/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.300656 module-build-service-3.9.2/tests/staged_data/local_builds/module-platform-f28-3/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1233 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/local_builds/module-platform-f28-3/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.290656 module-build-service-3.9.2/tests/staged_data/local_builds/module-platform-f30-3/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.300656 module-build-service-3.9.2/tests/staged_data/local_builds/module-platform-f30-3/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      473 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/local_builds/module-platform-f30-3/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.290656 module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule-master-20170816080815/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.300656 module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1147 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.290656 module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule-master-20170816080816/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.300656 module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1147 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.290656 module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.300656 module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1202 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/modules.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1273 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/staged_data/nginx_mmd.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      789 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/staged_data/platform.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1288 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/python3-no-components.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    43738 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/shared-userspace-570.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    43738 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/shared-userspace-577.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      783 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/staged_data/static_context_v2.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule-buildrequires-f30.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1157 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/staged_data/testmodule-dashed-stream.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1205 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule-forbidden-xmd.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      971 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule-local-build.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1114 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule-more-components.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      976 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule-no-base-module.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      598 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule-no-deps.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1222 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule-version-set.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      988 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule-with-filters.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1223 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule-wrong-stream.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1163 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule_br_metadata_module.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2473 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule_dependencies.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule_el8.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1141 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule_el800.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1141 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule_el821.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1387 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/staged_data/testmodule_init.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      993 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule_mse.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      989 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule_platform_f290000.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      977 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule_v2.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1001 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/staged_data/testmodule_v2_buildonly.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.300656 module-build-service-3.9.2/tests/staged_data/v3/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1051 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/staged_data/v3/mmd_packager.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.300656 module-build-service-3.9.2/tests/test_build/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_build/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    78132 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_build/test_build.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.301656 module-build-service-3.9.2/tests/test_builder/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_builder/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2202 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_builder/test_base.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    12418 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_builder/test_builder_utils.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    48113 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_builder/test_content_generator.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    25714 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_builder/test_get_generator_json_expected_output.json
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    25982 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_builder/test_get_generator_json_expected_output_with_log.json
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    26558 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_builder/test_get_generator_json_rpms_in_tag.json
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    42030 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_builder/test_koji.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    23966 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_builder/test_mock.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.301656 module-build-service-3.9.2/tests/test_common/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_common/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      507 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_common/test_config.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      492 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_common/test_koji.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    15595 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_common/test_logger.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2875 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_common/test_messaging.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.301656 module-build-service-3.9.2/tests/test_common/test_models/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_common/test_models/__init__.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.302656 module-build-service-3.9.2/tests/test_common/test_models/data/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)   465266 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_common/test_models/data/base-runtime.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1259 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_common/test_models/data/testmodule.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     7947 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_common/test_models/test_models.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2995 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_common/test_monitor.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     5005 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_common/test_resolve.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     5041 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_common/test_scm.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1785 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_common/test_submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     9519 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_common/test_utils.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     9109 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_manage.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.302656 module-build-service-3.9.2/tests/test_memory/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_memory/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      942 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_memory/mbs_configuration.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1994 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_memory/mbs_debug.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3694 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_memory/test_memory.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.302656 module-build-service-3.9.2/tests/test_resolver/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_resolver/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    16076 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_resolver/test_db.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    13897 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_resolver/test_koji.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2160 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_resolver/test_local.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    26781 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_resolver/test_mbs.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.303656 module-build-service-3.9.2/tests/test_scheduler/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_scheduler/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    17275 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_scheduler/test_batches.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4257 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_scheduler/test_celery_route_task.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4069 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_scheduler/test_consumer.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      865 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_scheduler/test_db_session.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    22196 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_scheduler/test_default_modules.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     7914 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_scheduler/test_module_init.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4111 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_scheduler/test_module_states.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     9215 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_scheduler/test_module_wait.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    22637 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_scheduler/test_poller.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     9458 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_scheduler/test_repo_done.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    22429 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_scheduler/test_reuse.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    16164 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_scheduler/test_submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    22744 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_scheduler/test_tag_tagged.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    14761 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_scheduler/test_ursine.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 16:25:36.303656 module-build-service-3.9.2/tests/test_web/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_web/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      490 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_web/client_secrets.json
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    11913 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_web/test_auth.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    18114 2023-03-24 19:41:06.000000 module-build-service-3.9.2/tests/test_web/test_mmd_resolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    32362 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_web/test_mse.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    17071 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tests/test_web/test_submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)   127952 2023-04-04 16:42:49.000000 module-build-service-3.9.2/tests/test_web/test_views.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2916 2023-03-24 19:41:27.000000 module-build-service-3.9.2/tox.ini
```

### Comparing `module-build-service-3.9.0/LICENSE` & `module-build-service-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/MANIFEST.in` & `module-build-service-3.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/README.rst` & `module-build-service-3.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/client/mbs-cli` & `module-build-service-3.9.2/client/mbs-cli`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/conf/koji.conf` & `module-build-service-3.9.2/conf/koji.conf`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/docs/CHANGELOG.rst` & `module-build-service-3.9.2/docs/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Change Log
 ==========
 
+v3.9.2
+------
+* Handle help option in mbs-upgradedb
+
+v3.9.1
+------
+* Include migrations dir
+
 v3.9.0
 ------
 * Replace flask-script with click
 * Allow krb cache to be configured
 * Provide missing fields in API
 * Local build improvements
```

### Comparing `module-build-service-3.9.0/docs/CONTRIBUTING.rst` & `module-build-service-3.9.2/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/docs/DEPENDENCY_RESOLUTION.rst` & `module-build-service-3.9.2/docs/DEPENDENCY_RESOLUTION.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/docs/HOW_MBS_BUILDS_MODULES.rst` & `module-build-service-3.9.2/docs/HOW_MBS_BUILDS_MODULES.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/docs/KOJI_RESOLVER.rst` & `module-build-service-3.9.2/docs/KOJI_RESOLVER.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/docs/MODULE_NAMING.rst` & `module-build-service-3.9.2/docs/MODULE_NAMING.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/docs/OFFLINE_LOCAL_BUILDS.rst` & `module-build-service-3.9.2/docs/OFFLINE_LOCAL_BUILDS.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/docs/REBUILD_STRATEGIES.rst` & `module-build-service-3.9.2/docs/REBUILD_STRATEGIES.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/docs/STATIC_CONTEXTS.rst` & `module-build-service-3.9.2/docs/STATIC_CONTEXTS.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/docs/VIRTUAL_MODULES.rst` & `module-build-service-3.9.2/docs/VIRTUAL_MODULES.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/fedmsg.d/module_build_service.py` & `module-build-service-3.9.2/fedmsg.d/module_build_service.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/__init__.py` & `module-build-service-3.9.2/module_build_service/__init__.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/builder/KojiContentGenerator.py` & `module-build-service-3.9.2/module_build_service/builder/KojiContentGenerator.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/builder/KojiModuleBuilder.py` & `module-build-service-3.9.2/module_build_service/builder/KojiModuleBuilder.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/builder/MockModuleBuilder.py` & `module-build-service-3.9.2/module_build_service/builder/MockModuleBuilder.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/builder/base.py` & `module-build-service-3.9.2/module_build_service/builder/base.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/builder/utils.py` & `module-build-service-3.9.2/module_build_service/builder/utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/config.py` & `module-build-service-3.9.2/module_build_service/common/config.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/errors.py` & `module-build-service-3.9.2/module_build_service/common/errors.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/koji.py` & `module-build-service-3.9.2/module_build_service/common/koji.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/logger.py` & `module-build-service-3.9.2/module_build_service/common/logger.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/messaging.py` & `module-build-service-3.9.2/module_build_service/common/messaging.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/models.py` & `module-build-service-3.9.2/module_build_service/common/models.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/monitor.py` & `module-build-service-3.9.2/module_build_service/common/monitor.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/request_utils.py` & `module-build-service-3.9.2/module_build_service/common/request_utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/resolve.py` & `module-build-service-3.9.2/module_build_service/common/resolve.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/retry.py` & `module-build-service-3.9.2/module_build_service/common/retry.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/scm.py` & `module-build-service-3.9.2/module_build_service/common/scm.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/submit.py` & `module-build-service-3.9.2/module_build_service/common/submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/common/utils.py` & `module-build-service-3.9.2/module_build_service/common/utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/manage.py` & `module-build-service-3.9.2/module_build_service/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import absolute_import, print_function
 from collections import defaultdict
 import click
 import getpass
 import logging
 import os
 import sys
+import argparse
 
 import flask_migrate
 from flask.cli import FlaskGroup
 from werkzeug.datastructures import FileStorage
 
 from module_build_service import app, db
 from module_build_service.builder.MockModuleBuilder import (
@@ -41,14 +42,20 @@
     with app.app_context():
         flask_migrate.upgrade(directory=migrations_dir)
 
 
 def upgradedb_entrypoint():
     """Entrypoint for command mbs-upgradedb"""
     # Work around issue with FlaskGroup not being initiated
+    # Argparse to catch --help
+    parser = argparse.ArgumentParser(
+        prog='mbs-upgradedb',
+        description='Upgrades the database schema to the latest revision'
+    )
+    args = parser.parse_args()
     cli(["upgradedb"])
 
 
 @cli.command("cleardb")
 def cleardb():
     """ Clears the database
     """
```

### Comparing `module-build-service-3.9.0/module_build_service/migrations/alembic.ini` & `module-build-service-3.9.2/module_build_service/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/resolver/DBResolver.py` & `module-build-service-3.9.2/module_build_service/resolver/DBResolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/resolver/KojiResolver.py` & `module-build-service-3.9.2/module_build_service/resolver/KojiResolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/resolver/LocalResolver.py` & `module-build-service-3.9.2/module_build_service/resolver/LocalResolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/resolver/MBSResolver.py` & `module-build-service-3.9.2/module_build_service/resolver/MBSResolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/resolver/__init__.py` & `module-build-service-3.9.2/module_build_service/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/resolver/base.py` & `module-build-service-3.9.2/module_build_service/resolver/base.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/__init__.py` & `module-build-service-3.9.2/module_build_service/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/batches.py` & `module-build-service-3.9.2/module_build_service/scheduler/batches.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/consumer.py` & `module-build-service-3.9.2/module_build_service/scheduler/consumer.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/db_session.py` & `module-build-service-3.9.2/module_build_service/scheduler/db_session.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/default_modules.py` & `module-build-service-3.9.2/module_build_service/scheduler/default_modules.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/events.py` & `module-build-service-3.9.2/module_build_service/scheduler/events.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/handlers/components.py` & `module-build-service-3.9.2/module_build_service/scheduler/handlers/components.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/handlers/modules.py` & `module-build-service-3.9.2/module_build_service/scheduler/handlers/modules.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/handlers/repos.py` & `module-build-service-3.9.2/module_build_service/scheduler/handlers/repos.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/handlers/tags.py` & `module-build-service-3.9.2/module_build_service/scheduler/handlers/tags.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/local.py` & `module-build-service-3.9.2/module_build_service/scheduler/local.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/parser.py` & `module-build-service-3.9.2/module_build_service/scheduler/parser.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/producer.py` & `module-build-service-3.9.2/module_build_service/scheduler/producer.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/reuse.py` & `module-build-service-3.9.2/module_build_service/scheduler/reuse.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/route.py` & `module-build-service-3.9.2/module_build_service/scheduler/route.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/submit.py` & `module-build-service-3.9.2/module_build_service/scheduler/submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/scheduler/ursine.py` & `module-build-service-3.9.2/module_build_service/scheduler/ursine.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/web/auth.py` & `module-build-service-3.9.2/module_build_service/web/auth.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/web/backports.py` & `module-build-service-3.9.2/module_build_service/web/backports.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/web/mmd_resolver.py` & `module-build-service-3.9.2/module_build_service/web/mmd_resolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/web/mse.py` & `module-build-service-3.9.2/module_build_service/web/mse.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/web/proxy.py` & `module-build-service-3.9.2/module_build_service/web/proxy.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/web/submit.py` & `module-build-service-3.9.2/module_build_service/web/submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/web/utils.py` & `module-build-service-3.9.2/module_build_service/web/utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service/web/views.py` & `module-build-service-3.9.2/module_build_service/web/views.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service.egg-info/SOURCES.txt` & `module-build-service-3.9.2/module_build_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/module_build_service.egg-info/entry_points.txt` & `module-build-service-3.9.2/module_build_service.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/run-unittests.sh` & `module-build-service-3.9.2/run-unittests.sh`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/setup.py` & `module-build-service-3.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 setup_py_path = path.dirname(path.realpath(__file__))
 install_requires, deps_links = read_requirements(path.join(setup_py_path, "requirements.txt"))
 tests_require, _ = read_requirements(path.join(setup_py_path, "test-requirements.txt"))
 
 setup(
     name="module-build-service",
     description="The Module Build Service for Modularity",
-    version="3.9.0",
+    version="3.9.2",
     classifiers=["Programming Language :: Python", "Topic :: Software Development :: Build Tools"],
     keywords="module build service fedora modularity koji mock rpm",
     author="The Factory 2.0 Team",
     author_email="module-build-service-owner@fedoraproject.org",
     url="https://pagure.io/fm-orchestrator/",
     license="MIT",
     packages=find_packages(),
```

### Comparing `module-build-service-3.9.0/tests/__init__.py` & `module-build-service-3.9.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/conftest.py` & `module-build-service-3.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/README.rst` & `module-build-service-3.9.2/tests/integration/README.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/conftest.py` & `module-build-service-3.9.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/example.test.env.yaml` & `module-build-service-3.9.2/tests/integration/example.test.env.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_build_stream_collision.py` & `module-build-service-3.9.2/tests/integration/test_build_stream_collision.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_buildonly.py` & `module-build-service-3.9.2/tests/integration/test_buildonly.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_buildrequire_invalid_module.py` & `module-build-service-3.9.2/tests/integration/test_buildrequire_invalid_module.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_failed_build.py` & `module-build-service-3.9.2/tests/integration/test_failed_build.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_highest_version_selection.py` & `module-build-service-3.9.2/tests/integration/test_highest_version_selection.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_no_components.py` & `module-build-service-3.9.2/tests/integration/test_no_components.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_normal_build.py` & `module-build-service-3.9.2/tests/integration/test_normal_build.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_normal_build_conflict.py` & `module-build-service-3.9.2/tests/integration/test_normal_build_conflict.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_rest_build_state.py` & `module-build-service-3.9.2/tests/integration/test_rest_build_state.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_rest_submit_build.py` & `module-build-service-3.9.2/tests/integration/test_rest_submit_build.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_resume_cancelled_build.py` & `module-build-service-3.9.2/tests/integration/test_resume_cancelled_build.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_reuse_all_components.py` & `module-build-service-3.9.2/tests/integration/test_reuse_all_components.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_reuse_components.py` & `module-build-service-3.9.2/tests/integration/test_reuse_components.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_reuse_components_if_added.py` & `module-build-service-3.9.2/tests/integration/test_reuse_components_if_added.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_reuse_tagged_module.py` & `module-build-service-3.9.2/tests/integration/test_reuse_tagged_module.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_scratch_build.py` & `module-build-service-3.9.2/tests/integration/test_scratch_build.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_scratch_final_mmd.py` & `module-build-service-3.9.2/tests/integration/test_scratch_final_mmd.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_stream_expansion.py` & `module-build-service-3.9.2/tests/integration/test_stream_expansion.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_v3_buildrequire.py` & `module-build-service-3.9.2/tests/integration/test_v3_buildrequire.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/test_v3_normal_build.py` & `module-build-service-3.9.2/tests/integration/test_v3_normal_build.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/integration/utils.py` & `module-build-service-3.9.2/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/scm_data/mariadb/objects/6c/d6a18e15a4f23a1eaa7040e7f4da9be1aed36d` & `module-build-service-3.9.2/tests/scm_data/mariadb/objects/6c/d6a18e15a4f23a1eaa7040e7f4da9be1aed36d`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/scm_data/mariadb/objects/6e/a27c8576449ad5a12c1b6d27b50ff32c854ee5` & `module-build-service-3.9.2/tests/scm_data/mariadb/objects/6e/a27c8576449ad5a12c1b6d27b50ff32c854ee5`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/scm_data/mariadb/objects/fb/9351bd6f2439a73d78de0822fefe64410f905c` & `module-build-service-3.9.2/tests/scm_data/mariadb/objects/fb/9351bd6f2439a73d78de0822fefe64410f905c`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.idx` & `module-build-service-3.9.2/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.idx`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.pack` & `module-build-service-3.9.2/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.pack`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/bad.yaml` & `module-build-service-3.9.2/tests/staged_data/bad.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/build_metadata_module.yaml` & `module-build-service-3.9.2/tests/staged_data/build_metadata_module.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/formatted_python3-no-components.yaml` & `module-build-service-3.9.2/tests/staged_data/formatted_python3-no-components.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/formatted_testmodule-more-components.yaml` & `module-build-service-3.9.2/tests/staged_data/formatted_testmodule-more-components.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/formatted_testmodule.yaml` & `module-build-service-3.9.2/tests/staged_data/formatted_testmodule.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/includedmodules.yaml` & `module-build-service-3.9.2/tests/staged_data/includedmodules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/local_builds/module-child-master-20170816080815/results/modules.yaml` & `module-build-service-3.9.2/tests/staged_data/local_builds/module-child-master-20170816080815/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/local_builds/module-parent-master-20170816080815/results/modules.yaml` & `module-build-service-3.9.2/tests/staged_data/local_builds/module-parent-master-20170816080815/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f28-3/results/modules.yaml` & `module-build-service-3.9.2/tests/staged_data/local_builds/module-platform-f28-3/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/modules.yaml` & `module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/modules.yaml` & `module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/modules.yaml` & `module-build-service-3.9.2/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/nginx_mmd.yaml` & `module-build-service-3.9.2/tests/staged_data/nginx_mmd.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/platform.yaml` & `module-build-service-3.9.2/tests/staged_data/platform.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/python3-no-components.yaml` & `module-build-service-3.9.2/tests/staged_data/python3-no-components.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/shared-userspace-570.yaml` & `module-build-service-3.9.2/tests/staged_data/shared-userspace-570.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/shared-userspace-577.yaml` & `module-build-service-3.9.2/tests/staged_data/shared-userspace-577.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/static_context_v2.yaml` & `module-build-service-3.9.2/tests/staged_data/static_context_v2.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule-buildrequires-f30.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule-buildrequires-f30.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule-dashed-stream.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule-dashed-stream.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule-forbidden-xmd.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule-forbidden-xmd.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule-local-build.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule-local-build.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule-more-components.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule-more-components.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule-no-base-module.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule-no-base-module.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule-no-deps.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule-no-deps.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule-version-set.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule-version-set.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule-with-filters.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule-with-filters.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule-wrong-stream.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule-wrong-stream.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule_br_metadata_module.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule_br_metadata_module.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule_dependencies.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule_dependencies.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule_el8.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule_el8.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule_el800.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule_el800.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule_el821.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule_el821.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule_init.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule_init.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule_mse.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule_mse.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule_platform_f290000.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule_platform_f290000.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule_v2.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule_v2.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/testmodule_v2_buildonly.yaml` & `module-build-service-3.9.2/tests/staged_data/testmodule_v2_buildonly.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/staged_data/v3/mmd_packager.yaml` & `module-build-service-3.9.2/tests/staged_data/v3/mmd_packager.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_build/test_build.py` & `module-build-service-3.9.2/tests/test_build/test_build.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_builder/test_base.py` & `module-build-service-3.9.2/tests/test_builder/test_base.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_builder/test_builder_utils.py` & `module-build-service-3.9.2/tests/test_builder/test_builder_utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_builder/test_content_generator.py` & `module-build-service-3.9.2/tests/test_builder/test_content_generator.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_builder/test_get_generator_json_expected_output.json` & `module-build-service-3.9.2/tests/test_builder/test_get_generator_json_expected_output.json`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_builder/test_get_generator_json_expected_output_with_log.json` & `module-build-service-3.9.2/tests/test_builder/test_get_generator_json_expected_output_with_log.json`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_builder/test_get_generator_json_rpms_in_tag.json` & `module-build-service-3.9.2/tests/test_builder/test_get_generator_json_rpms_in_tag.json`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_builder/test_koji.py` & `module-build-service-3.9.2/tests/test_builder/test_koji.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_builder/test_mock.py` & `module-build-service-3.9.2/tests/test_builder/test_mock.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_common/test_logger.py` & `module-build-service-3.9.2/tests/test_common/test_logger.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_common/test_messaging.py` & `module-build-service-3.9.2/tests/test_common/test_messaging.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_common/test_models/data/base-runtime.yaml` & `module-build-service-3.9.2/tests/test_common/test_models/data/base-runtime.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_common/test_models/data/testmodule.yaml` & `module-build-service-3.9.2/tests/test_common/test_models/data/testmodule.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_common/test_models/test_models.py` & `module-build-service-3.9.2/tests/test_common/test_models/test_models.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_common/test_monitor.py` & `module-build-service-3.9.2/tests/test_common/test_monitor.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_common/test_resolve.py` & `module-build-service-3.9.2/tests/test_common/test_resolve.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_common/test_scm.py` & `module-build-service-3.9.2/tests/test_common/test_scm.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_common/test_submit.py` & `module-build-service-3.9.2/tests/test_common/test_submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_common/test_utils.py` & `module-build-service-3.9.2/tests/test_common/test_utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_manage.py` & `module-build-service-3.9.2/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_memory/mbs_configuration.py` & `module-build-service-3.9.2/tests/test_memory/mbs_configuration.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_memory/mbs_debug.py` & `module-build-service-3.9.2/tests/test_memory/mbs_debug.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_memory/test_memory.py` & `module-build-service-3.9.2/tests/test_memory/test_memory.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_resolver/test_db.py` & `module-build-service-3.9.2/tests/test_resolver/test_db.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_resolver/test_koji.py` & `module-build-service-3.9.2/tests/test_resolver/test_koji.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_resolver/test_local.py` & `module-build-service-3.9.2/tests/test_resolver/test_local.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_resolver/test_mbs.py` & `module-build-service-3.9.2/tests/test_resolver/test_mbs.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_batches.py` & `module-build-service-3.9.2/tests/test_scheduler/test_batches.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_celery_route_task.py` & `module-build-service-3.9.2/tests/test_scheduler/test_celery_route_task.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_consumer.py` & `module-build-service-3.9.2/tests/test_scheduler/test_consumer.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_db_session.py` & `module-build-service-3.9.2/tests/test_scheduler/test_db_session.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_default_modules.py` & `module-build-service-3.9.2/tests/test_scheduler/test_default_modules.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_module_init.py` & `module-build-service-3.9.2/tests/test_scheduler/test_module_init.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_module_states.py` & `module-build-service-3.9.2/tests/test_scheduler/test_module_states.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_module_wait.py` & `module-build-service-3.9.2/tests/test_scheduler/test_module_wait.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_poller.py` & `module-build-service-3.9.2/tests/test_scheduler/test_poller.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_repo_done.py` & `module-build-service-3.9.2/tests/test_scheduler/test_repo_done.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_reuse.py` & `module-build-service-3.9.2/tests/test_scheduler/test_reuse.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_submit.py` & `module-build-service-3.9.2/tests/test_scheduler/test_submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_tag_tagged.py` & `module-build-service-3.9.2/tests/test_scheduler/test_tag_tagged.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_scheduler/test_ursine.py` & `module-build-service-3.9.2/tests/test_scheduler/test_ursine.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_web/test_auth.py` & `module-build-service-3.9.2/tests/test_web/test_auth.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_web/test_mmd_resolver.py` & `module-build-service-3.9.2/tests/test_web/test_mmd_resolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_web/test_mse.py` & `module-build-service-3.9.2/tests/test_web/test_mse.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_web/test_submit.py` & `module-build-service-3.9.2/tests/test_web/test_submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tests/test_web/test_views.py` & `module-build-service-3.9.2/tests/test_web/test_views.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.9.0/tox.ini` & `module-build-service-3.9.2/tox.ini`

 * *Files identical despite different names*

