# Comparing `tmp/module-build-service-3.8.0.tar.gz` & `tmp/module-build-service-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module-build-service-3.8.0.tar", last modified: Wed Dec  7 18:07:09 2022, max compression
+gzip compressed data, was "module-build-service-3.9.0.tar", last modified: Tue Apr 18 15:15:48 2023, max compression
```

## Comparing `module-build-service-3.8.0.tar` & `module-build-service-3.9.0.tar`

### file list

```diff
@@ -1,335 +1,339 @@
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.363775 module-build-service-3.8.0/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1057 2022-10-28 17:47:14.000000 module-build-service-3.8.0/LICENSE
--rw-r--r--   0 breilly   (1000) breilly   (1000)      394 2022-10-28 17:47:14.000000 module-build-service-3.8.0/MANIFEST.in
--rw-r--r--   0 breilly   (1000) breilly   (1000)      473 2022-12-07 18:07:09.363775 module-build-service-3.8.0/PKG-INFO
--rw-r--r--   0 breilly   (1000) breilly   (1000)    30729 2022-10-28 17:47:14.000000 module-build-service-3.8.0/README.rst
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.325775 module-build-service-3.8.0/client/
--rwxr-xr-x   0 breilly   (1000) breilly   (1000)    11007 2022-10-28 17:47:14.000000 module-build-service-3.8.0/client/mbs-cli
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.326775 module-build-service-3.8.0/conf/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      693 2022-10-28 17:47:14.000000 module-build-service-3.8.0/conf/koji.conf
--rw-r--r--   0 breilly   (1000) breilly   (1000)      491 2022-10-28 17:47:14.000000 module-build-service-3.8.0/conf/mock.cfg
--rw-r--r--   0 breilly   (1000) breilly   (1000)      268 2022-10-28 17:47:14.000000 module-build-service-3.8.0/conf/yum.conf
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.327775 module-build-service-3.8.0/docs/
--rw-r--r--   0 breilly   (1000) breilly   (1000)    21796 2022-12-06 19:51:34.000000 module-build-service-3.8.0/docs/CHANGELOG.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     8811 2022-10-28 17:47:14.000000 module-build-service-3.8.0/docs/CONTRIBUTING.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)    12214 2022-10-28 17:47:14.000000 module-build-service-3.8.0/docs/DEPENDENCY_RESOLUTION.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)      373 2022-10-28 17:47:14.000000 module-build-service-3.8.0/docs/GATING.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)    10279 2022-10-28 17:47:14.000000 module-build-service-3.8.0/docs/HOW_MBS_BUILDS_MODULES.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3741 2022-10-28 17:47:14.000000 module-build-service-3.8.0/docs/KOJI_RESOLVER.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3629 2022-10-28 17:47:14.000000 module-build-service-3.8.0/docs/MODULE_NAMING.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4050 2022-10-28 17:47:14.000000 module-build-service-3.8.0/docs/OFFLINE_LOCAL_BUILDS.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4410 2022-10-28 17:47:14.000000 module-build-service-3.8.0/docs/REBUILD_STRATEGIES.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     5151 2022-10-28 17:47:14.000000 module-build-service-3.8.0/docs/STATIC_CONTEXTS.rst
--rw-r--r--   0 breilly   (1000) breilly   (1000)     5129 2022-10-28 17:47:14.000000 module-build-service-3.8.0/docs/VIRTUAL_MODULES.rst
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.328775 module-build-service-3.8.0/fedmsg.d/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      293 2022-10-28 17:47:14.000000 module-build-service-3.8.0/fedmsg.d/mbs-logging.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)       31 2022-10-28 17:47:14.000000 module-build-service-3.8.0/fedmsg.d/mbs-scheduler.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1746 2022-10-28 17:47:14.000000 module-build-service-3.8.0/fedmsg.d/module_build_service.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.328775 module-build-service-3.8.0/module_build_service/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2161 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/__init__.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.330775 module-build-service-3.8.0/module_build_service/builder/
--rw-r--r--   0 breilly   (1000) breilly   (1000)    36505 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/builder/KojiContentGenerator.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    53262 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/builder/KojiModuleBuilder.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    34564 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/builder/MockModuleBuilder.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      345 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/builder/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    17725 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/builder/base.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    13382 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/builder/utils.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.333775 module-build-service-3.8.0/module_build_service/common/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      355 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    39828 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/config.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      664 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/errors.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     6491 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/koji.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     6213 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/logger.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4786 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/messaging.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    52389 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/models.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      171 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/modulemd.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3323 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/monitor.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      840 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/request_utils.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     8662 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/resolve.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      993 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/retry.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    13555 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/scm.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4863 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     8779 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/common/utils.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      228 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/log_workaround.py
--rwxr-xr-x   0 breilly   (1000) breilly   (1000)    10136 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/manage.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.333775 module-build-service-3.8.0/module_build_service/migrations/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       38 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/README
--rw-r--r--   0 breilly   (1000) breilly   (1000)      800 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/alembic.ini
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2883 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/env.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      412 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/script.py.mako
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.337775 module-build-service-3.8.0/module_build_service/migrations/versions/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      907 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/0b00036c540f_add_log_messages_table.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      423 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/0ef60c3ed440_insert_fake_base_runtime.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      707 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/145347916a56_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      601 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/1817e62719f9_remove_ref_build_context.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1618 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/1a44272e8b4c_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      795 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/229f6f273a56_state_reason.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1246 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/335455a30585_state_reason_history.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      765 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/3b17cd6dc583_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      525 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/40b2c7d988d7_add_reused_module_id_column.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1829 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/440a8a3c0d96_add_indexes_to_models.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      590 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/474697622859_add_optional_columns_for_copr.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      510 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/4d1e2e13e514_buildonly.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      702 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/524c3b1c683c_rebuild_strategy.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4019 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/526fb7d445f7_module_buildrequires.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      604 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/60c6093dde9e_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      677 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/65ad4fcdbce6_add_missing_uniqueness_constraint.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3788 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/6d503efcd2b8_virtual_streams_table.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2025 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/708ac8950f55_set_from_mmd_context.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1186 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/79babdadc942_convert_type_of_modulebuild_stream_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3033 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/9ca1c166f426_contexts.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      573 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/9d5e6938588f_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      809 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/a1fc0736bca8_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1594 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/a7a553e5ca1d_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1871 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/a87264eeb49f_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1082 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/bf861b6af29a_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      665 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/c11a3cfec2a9_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1324 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/c8e2fc555399_add_modulebuild_context.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2524 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/caeae7a4f537_ref_build_context.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      655 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/d5188b4a7bf1_add_fk_reused_module_id.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      454 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/edb537dd1e8c_.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      443 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/migrations/versions/f5b1c5203cce_.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.338775 module-build-service-3.8.0/module_build_service/resolver/
--rw-r--r--   0 breilly   (1000) breilly   (1000)    19442 2022-12-06 19:47:10.000000 module-build-service-3.8.0/module_build_service/resolver/DBResolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    12593 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/resolver/KojiResolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1539 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/resolver/LocalResolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    23000 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/resolver/MBSResolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      569 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/resolver/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4201 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/resolver/base.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.341775 module-build-service-3.8.0/module_build_service/scheduler/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      600 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    12228 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/batches.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    11821 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/consumer.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2686 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/db_session.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    18700 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/default_modules.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4480 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/events.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.341775 module-build-service-3.8.0/module_build_service/scheduler/handlers/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/handlers/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     7698 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/handlers/components.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    19889 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/handlers/modules.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     6133 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/handlers/repos.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3952 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/handlers/tags.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3094 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/local.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4716 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/parser.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    18718 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/producer.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    20367 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/reuse.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2610 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/route.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    24227 2022-12-06 19:47:10.000000 module-build-service-3.8.0/module_build_service/scheduler/submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    10934 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/scheduler/ursine.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.343775 module-build-service-3.8.0/module_build_service/web/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/web/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     7895 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/web/auth.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1286 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/web/backports.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    32526 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/web/mmd_resolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    24166 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/web/mse.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1258 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/web/proxy.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    33713 2022-12-06 19:47:10.000000 module-build-service-3.8.0/module_build_service/web/submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    16184 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/web/utils.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    27146 2022-10-28 17:47:14.000000 module-build-service-3.8.0/module_build_service/web/views.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.329775 module-build-service-3.8.0/module_build_service.egg-info/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      473 2022-12-07 18:07:09.000000 module-build-service-3.8.0/module_build_service.egg-info/PKG-INFO
--rw-r--r--   0 breilly   (1000) breilly   (1000)    11806 2022-12-07 18:07:09.000000 module-build-service-3.8.0/module_build_service.egg-info/SOURCES.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)        1 2022-12-07 18:07:09.000000 module-build-service-3.8.0/module_build_service.egg-info/dependency_links.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)      919 2022-12-07 18:07:09.000000 module-build-service-3.8.0/module_build_service.egg-info/entry_points.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)        1 2022-10-28 17:50:05.000000 module-build-service-3.8.0/module_build_service.egg-info/not-zip-safe
--rw-r--r--   0 breilly   (1000) breilly   (1000)      221 2022-12-07 18:07:09.000000 module-build-service-3.8.0/module_build_service.egg-info/requires.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)       27 2022-12-07 18:07:09.000000 module-build-service-3.8.0/module_build_service.egg-info/top_level.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)      252 2022-10-28 17:47:14.000000 module-build-service-3.8.0/requirements.txt
--rw-r--r--   0 breilly   (1000) breilly   (1000)       38 2022-12-07 18:07:09.363775 module-build-service-3.8.0/setup.cfg
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3097 2022-12-06 19:49:02.000000 module-build-service-3.8.0/setup.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)       55 2022-10-28 17:47:14.000000 module-build-service-3.8.0/test-requirements.txt
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.344775 module-build-service-3.8.0/tests/
--rw-r--r--   0 breilly   (1000) breilly   (1000)    36376 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    10022 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/conftest.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.344775 module-build-service-3.8.0/tests/integration/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     5439 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/integration/example.test.env.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.323775 module-build-service-3.8.0/tests/scm_data/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.345775 module-build-service-3.8.0/tests/scm_data/mariadb/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       23 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/HEAD
--rw-r--r--   0 breilly   (1000) breilly   (1000)       66 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/config
--rw-r--r--   0 breilly   (1000) breilly   (1000)       73 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/description
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.345775 module-build-service-3.8.0/tests/scm_data/mariadb/info/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      240 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/info/exclude
--rw-r--r--   0 breilly   (1000) breilly   (1000)       59 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/info/refs
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.323775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.345775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/34/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/34/a463979786199c1b41ca21eb309cf3ce5ce789
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.345775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/48/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/48/83b004d723a15cdc266c0280fe26c424ae10db
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.346775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/60/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      186 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/60/5345608fcc41d4e297cf062c653ebfdfe52476
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.346775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/6c/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      807 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/6c/d6a18e15a4f23a1eaa7040e7f4da9be1aed36d
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.346775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/6e/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      726 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/6e/a27c8576449ad5a12c1b6d27b50ff32c854ee5
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.346775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/7f/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      435 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/7f/96fc61223e4bc4c93c7c286cca98f6efaa3716
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.346775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/8b/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      223 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/8b/43f38cdafdd773e7d0308e758105bf9f0f67a8
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.346775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/e3/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      192 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/e3/ca243c664440cdb8b704b0d5c32ed433bee4da
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.346775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/e4/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/e4/75d55e2b78ad81f1b08bcb33a0a15ad24ef8a9
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.347775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/e9/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      182 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/e9/742ed681f82e3ef5281fc652b4e68a3826cea6
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.347775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/f7/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      177 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/f7/c5c7218c9a197d7fd245eeb4eee3d7abffd75d
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.347775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/fb/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      808 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/fb/9351bd6f2439a73d78de0822fefe64410f905c
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.347775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/fc/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/fc/399d16e46feb3af72a692b316a241c21bae1d0
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.347775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/info/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       54 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/info/packs
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.347775 module-build-service-3.8.0/tests/scm_data/mariadb/objects/pack/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2584 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.idx
--rw-r--r--   0 breilly   (1000) breilly   (1000)    36836 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.pack
--rw-r--r--   0 breilly   (1000) breilly   (1000)       98 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/packed-refs
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.323775 module-build-service-3.8.0/tests/scm_data/mariadb/refs/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.348775 module-build-service-3.8.0/tests/scm_data/mariadb/refs/heads/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/refs/heads/.placeholder
--rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/refs/heads/master
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.348775 module-build-service-3.8.0/tests/scm_data/mariadb/refs/tags/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/mariadb/refs/tags/.placeholder
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.348775 module-build-service-3.8.0/tests/scm_data/testrepo/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       23 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/HEAD
--rw-r--r--   0 breilly   (1000) breilly   (1000)       66 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/config
--rw-r--r--   0 breilly   (1000) breilly   (1000)       73 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/description
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.348775 module-build-service-3.8.0/tests/scm_data/testrepo/info/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      240 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/info/exclude
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.323775 module-build-service-3.8.0/tests/scm_data/testrepo/objects/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.348775 module-build-service-3.8.0/tests/scm_data/testrepo/objects/17/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       37 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/objects/17/2c8d5a1db52737ebeb50fe5058212b97ac3f82
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.348775 module-build-service-3.8.0/tests/scm_data/testrepo/objects/28/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       29 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/objects/28/ad5b501c13fc618bb395913a2b47ad90e0f51f
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.348775 module-build-service-3.8.0/tests/scm_data/testrepo/objects/54/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      130 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/objects/54/81faa232d66589e660cc301179867fb00842c9
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.348775 module-build-service-3.8.0/tests/scm_data/testrepo/objects/70/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      169 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/objects/70/35bd33614972ac66559ac1fdd019ff6027ad21
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.349775 module-build-service-3.8.0/tests/scm_data/testrepo/objects/b8/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       47 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/objects/b8/f5533d9ab4cbc7a7dee0c1131dfc12e4376524
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.349775 module-build-service-3.8.0/tests/scm_data/testrepo/objects/d5/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       48 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/objects/d5/819330d12885aae9c026081d7959fae78eab03
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.323775 module-build-service-3.8.0/tests/scm_data/testrepo/refs/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.349775 module-build-service-3.8.0/tests/scm_data/testrepo/refs/heads/
--rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/refs/heads/dev
--rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/scm_data/testrepo/refs/heads/master
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.352775 module-build-service-3.8.0/tests/staged_data/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      824 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/bad.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      607 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/build_metadata_module.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      354 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/build_metadata_module_not_processed.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      329 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/fakemodule.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2021 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/formatted_python3-no-components.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1848 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/formatted_testmodule-more-components.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2244 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/formatted_testmodule.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      975 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/includedmodules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.324775 module-build-service-3.8.0/tests/staged_data/local_builds/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.324775 module-build-service-3.8.0/tests/staged_data/local_builds/module-child-master-20170816080815/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.352775 module-build-service-3.8.0/tests/staged_data/local_builds/module-child-master-20170816080815/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1449 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/local_builds/module-child-master-20170816080815/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.324775 module-build-service-3.8.0/tests/staged_data/local_builds/module-parent-master-20170816080815/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.353775 module-build-service-3.8.0/tests/staged_data/local_builds/module-parent-master-20170816080815/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1301 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/local_builds/module-parent-master-20170816080815/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.324775 module-build-service-3.8.0/tests/staged_data/local_builds/module-platform-f28-3/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.353775 module-build-service-3.8.0/tests/staged_data/local_builds/module-platform-f28-3/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1233 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/local_builds/module-platform-f28-3/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.324775 module-build-service-3.8.0/tests/staged_data/local_builds/module-platform-f30-3/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.353775 module-build-service-3.8.0/tests/staged_data/local_builds/module-platform-f30-3/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)      473 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/local_builds/module-platform-f30-3/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.324775 module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.353775 module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1147 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.324775 module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.353775 module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1147 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/modules.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.324775 module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.353775 module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1202 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/modules.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1273 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/nginx_mmd.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      789 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/platform.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1288 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/python3-no-components.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)    43738 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/shared-userspace-570.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)    43738 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/shared-userspace-577.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      783 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/static_context_v2.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule-buildrequires-f30.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1157 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule-dashed-stream.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1205 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule-forbidden-xmd.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      971 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule-local-build.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1114 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule-more-components.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      976 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule-no-base-module.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      598 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule-no-deps.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1222 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule-version-set.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      988 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule-with-filters.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1223 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule-wrong-stream.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1163 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule_br_metadata_module.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2473 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule_dependencies.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule_el8.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1141 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule_el800.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1141 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule_el821.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1341 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule_init.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      993 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule_mse.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      989 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule_platform_f290000.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)      977 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule_v2.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1001 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/testmodule_v2_buildonly.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.353775 module-build-service-3.8.0/tests/staged_data/v3/
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1051 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/staged_data/v3/mmd_packager.yaml
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.353775 module-build-service-3.8.0/tests/test_build/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_build/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    78132 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_build/test_build.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.354775 module-build-service-3.8.0/tests/test_builder/
--rw-r--r--   0 breilly   (1000) breilly   (1000)    25714 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_builder/test_get_generator_json_expected_output.json
--rw-r--r--   0 breilly   (1000) breilly   (1000)    25982 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_builder/test_get_generator_json_expected_output_with_log.json
--rw-r--r--   0 breilly   (1000) breilly   (1000)    26558 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_builder/test_get_generator_json_rpms_in_tag.json
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.356775 module-build-service-3.8.0/tests/test_common/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      507 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_config.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      489 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_koji.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4372 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_logger.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2875 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_messaging.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.356775 module-build-service-3.8.0/tests/test_common/test_models/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_models/__init__.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.357775 module-build-service-3.8.0/tests/test_common/test_models/data/
--rw-r--r--   0 breilly   (1000) breilly   (1000)   465266 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_models/data/base-runtime.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1259 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_models/data/testmodule.yaml
--rw-r--r--   0 breilly   (1000) breilly   (1000)     7947 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_models/test_models.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2995 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_monitor.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     5005 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_resolve.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     5041 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_scm.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1785 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     9519 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_common/test_utils.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     8801 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_manage.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.358775 module-build-service-3.8.0/tests/test_memory/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_memory/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      942 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_memory/mbs_configuration.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     1994 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_memory/mbs_debug.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     3694 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_memory/test_memory.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.359775 module-build-service-3.8.0/tests/test_resolver/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_resolver/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    16076 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_resolver/test_db.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    13897 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_resolver/test_koji.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     2160 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_resolver/test_local.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    26781 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_resolver/test_mbs.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.361775 module-build-service-3.8.0/tests/test_scheduler/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    17214 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_batches.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4257 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_celery_route_task.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4069 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_consumer.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      865 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_db_session.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    22196 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_default_modules.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     7914 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_module_init.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     4111 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_module_states.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     9215 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_module_wait.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    22634 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_poller.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)     9458 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_repo_done.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    22429 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_reuse.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    16164 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    22744 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_tag_tagged.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    14761 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_scheduler/test_ursine.py
-drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2022-12-07 18:07:09.362775 module-build-service-3.8.0/tests/test_web/
--rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_web/__init__.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)      490 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_web/client_secrets.json
--rw-r--r--   0 breilly   (1000) breilly   (1000)    11913 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_web/test_auth.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    18114 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_web/test_mmd_resolver.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    32362 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_web/test_mse.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)    17071 2022-12-06 19:47:10.000000 module-build-service-3.8.0/tests/test_web/test_submit.py
--rw-r--r--   0 breilly   (1000) breilly   (1000)   127739 2022-10-28 17:47:14.000000 module-build-service-3.8.0/tests/test_web/test_views.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.463877 module-build-service-3.9.0/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1057 2023-03-24 19:41:06.000000 module-build-service-3.9.0/LICENSE
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      566 2023-04-04 16:42:49.000000 module-build-service-3.9.0/MANIFEST.in
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      445 2023-04-18 15:15:48.463877 module-build-service-3.9.0/PKG-INFO
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    30837 2023-04-04 16:42:49.000000 module-build-service-3.9.0/README.rst
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.450877 module-build-service-3.9.0/client/
+-rwxr-xr-x   0 breilly   (1000) breilly   (1000)    11007 2023-03-24 19:41:06.000000 module-build-service-3.9.0/client/mbs-cli
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.450877 module-build-service-3.9.0/conf/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      474 2023-03-24 19:41:06.000000 module-build-service-3.9.0/conf/client_secrets.json
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      693 2023-03-24 19:41:06.000000 module-build-service-3.9.0/conf/koji.conf
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      491 2023-03-24 19:41:06.000000 module-build-service-3.9.0/conf/mock.cfg
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      268 2023-03-24 19:41:06.000000 module-build-service-3.9.0/conf/yum.conf
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.451877 module-build-service-3.9.0/docs/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    21939 2023-04-18 15:10:58.000000 module-build-service-3.9.0/docs/CHANGELOG.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     8811 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/CONTRIBUTING.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    12214 2023-03-24 19:41:06.000000 module-build-service-3.9.0/docs/DEPENDENCY_RESOLUTION.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      373 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/GATING.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    10279 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/HOW_MBS_BUILDS_MODULES.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3741 2023-03-24 19:41:06.000000 module-build-service-3.9.0/docs/KOJI_RESOLVER.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3629 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/MODULE_NAMING.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4050 2023-03-24 19:41:06.000000 module-build-service-3.9.0/docs/OFFLINE_LOCAL_BUILDS.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4410 2023-03-24 19:41:06.000000 module-build-service-3.9.0/docs/REBUILD_STRATEGIES.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     5151 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/STATIC_CONTEXTS.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     5129 2023-03-24 19:41:27.000000 module-build-service-3.9.0/docs/VIRTUAL_MODULES.rst
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.451877 module-build-service-3.9.0/fedmsg.d/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      293 2023-03-24 19:41:06.000000 module-build-service-3.9.0/fedmsg.d/mbs-logging.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       31 2023-03-24 19:41:06.000000 module-build-service-3.9.0/fedmsg.d/mbs-scheduler.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1746 2023-03-24 19:41:06.000000 module-build-service-3.9.0/fedmsg.d/module_build_service.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.451877 module-build-service-3.9.0/module_build_service/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2161 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/__init__.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.451877 module-build-service-3.9.0/module_build_service/builder/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    36505 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/builder/KojiContentGenerator.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    53040 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/builder/KojiModuleBuilder.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    34722 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/builder/MockModuleBuilder.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      345 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/builder/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    17795 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/builder/base.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    13522 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/builder/utils.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.452877 module-build-service-3.9.0/module_build_service/common/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      355 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/common/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    40346 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/common/config.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      664 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/errors.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     6359 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/common/koji.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    18951 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/common/logger.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4786 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/messaging.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    52663 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/common/models.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      171 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/common/modulemd.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3323 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/monitor.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      840 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/common/request_utils.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     8662 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/resolve.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      993 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/common/retry.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    13555 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/scm.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4863 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     8779 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/common/utils.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      228 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/log_workaround.py
+-rwxr-xr-x   0 breilly   (1000) breilly   (1000)     9204 2023-04-18 15:04:21.000000 module-build-service-3.9.0/module_build_service/manage.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.452877 module-build-service-3.9.0/module_build_service/migrations/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       38 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/migrations/README
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      800 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/migrations/alembic.ini
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      412 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/migrations/script.py.mako
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.453877 module-build-service-3.9.0/module_build_service/resolver/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    19442 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/resolver/DBResolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    12593 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/resolver/KojiResolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1539 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/resolver/LocalResolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    23085 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/resolver/MBSResolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      569 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/resolver/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4201 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/resolver/base.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.453877 module-build-service-3.9.0/module_build_service/scheduler/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      600 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    12330 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/scheduler/batches.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    11821 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/consumer.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2686 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/db_session.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    18852 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/scheduler/default_modules.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4480 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/events.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.454877 module-build-service-3.9.0/module_build_service/scheduler/handlers/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/handlers/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     7698 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/handlers/components.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    20060 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/scheduler/handlers/modules.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     6133 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/handlers/repos.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3952 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/handlers/tags.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3115 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/scheduler/local.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4716 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/parser.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    18718 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/producer.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    20367 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/scheduler/reuse.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2614 2023-04-18 15:04:21.000000 module-build-service-3.9.0/module_build_service/scheduler/route.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    24249 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/scheduler/submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    10934 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/scheduler/ursine.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.454877 module-build-service-3.9.0/module_build_service/web/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     7895 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/auth.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1286 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/backports.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    32526 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/mmd_resolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    24371 2023-04-04 16:42:49.000000 module-build-service-3.9.0/module_build_service/web/mse.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1258 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/proxy.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    33713 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/web/submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    16184 2023-03-24 19:41:06.000000 module-build-service-3.9.0/module_build_service/web/utils.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    27146 2023-03-24 19:41:27.000000 module-build-service-3.9.0/module_build_service/web/views.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.451877 module-build-service-3.9.0/module_build_service.egg-info/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      445 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/PKG-INFO
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    11007 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/SOURCES.txt
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        1 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/dependency_links.txt
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      917 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/entry_points.txt
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        1 2023-04-18 15:14:27.000000 module-build-service-3.9.0/module_build_service.egg-info/not-zip-safe
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      190 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/requires.txt
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       27 2023-04-18 15:15:48.000000 module-build-service-3.9.0/module_build_service.egg-info/top_level.txt
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      190 2023-04-04 16:42:49.000000 module-build-service-3.9.0/requirements.txt
+-rwxr-xr-x   0 breilly   (1000) breilly   (1000)     3278 2023-03-24 19:41:06.000000 module-build-service-3.9.0/run-unittests.sh
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       38 2023-04-18 15:15:48.463877 module-build-service-3.9.0/setup.cfg
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3096 2023-04-18 15:05:44.000000 module-build-service-3.9.0/setup.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       55 2023-03-24 19:41:06.000000 module-build-service-3.9.0/test-requirements.txt
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.454877 module-build-service-3.9.0/tests/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    36376 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    10022 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/conftest.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/integration/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2513 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/README.rst
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/integration/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3847 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/conftest.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     5439 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/example.test.env.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1160 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_build_stream_collision.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1592 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_buildonly.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1661 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_buildrequire_invalid_module.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1053 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_failed_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1031 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_highest_version_selection.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      347 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_import_module.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      574 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_no_components.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1755 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_normal_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1158 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_normal_build_conflict.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1793 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_rest_build_state.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1550 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_rest_submit_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      994 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_resume_cancelled_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1103 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_reuse_all_components.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1986 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_reuse_components.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4504 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_reuse_components_if_added.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2558 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_reuse_tagged_module.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      953 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_scratch_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1564 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_scratch_final_mmd.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      457 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_static_context.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      538 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/integration/test_stream_expansion.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1545 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_v3_buildrequire.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      360 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_v3_multiple_contexts.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      364 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_v3_no_components.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1478 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/test_v3_normal_build.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    25074 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/integration/utils.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/scm_data/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       23 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/HEAD
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       66 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/config
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       73 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/description
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/info/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      240 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/info/exclude
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       59 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/info/refs
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/34/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/34/a463979786199c1b41ca21eb309cf3ce5ce789
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/48/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/48/83b004d723a15cdc266c0280fe26c424ae10db
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/60/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      186 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/60/5345608fcc41d4e297cf062c653ebfdfe52476
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/6c/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      807 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/6c/d6a18e15a4f23a1eaa7040e7f4da9be1aed36d
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/6e/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      726 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/6e/a27c8576449ad5a12c1b6d27b50ff32c854ee5
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/7f/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      435 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/7f/96fc61223e4bc4c93c7c286cca98f6efaa3716
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/8b/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      223 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/8b/43f38cdafdd773e7d0308e758105bf9f0f67a8
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e3/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      192 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e3/ca243c664440cdb8b704b0d5c32ed433bee4da
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e4/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e4/75d55e2b78ad81f1b08bcb33a0a15ad24ef8a9
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e9/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      182 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/e9/742ed681f82e3ef5281fc652b4e68a3826cea6
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/f7/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      177 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/f7/c5c7218c9a197d7fd245eeb4eee3d7abffd75d
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/fb/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      808 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/fb/9351bd6f2439a73d78de0822fefe64410f905c
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.456877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/fc/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      291 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/fc/399d16e46feb3af72a692b316a241c21bae1d0
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/info/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       54 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/info/packs
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/mariadb/objects/pack/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2584 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.idx
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    36836 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.pack
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       98 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/packed-refs
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/scm_data/mariadb/refs/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/mariadb/refs/heads/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/refs/heads/.placeholder
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/refs/heads/master
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/mariadb/refs/tags/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/mariadb/refs/tags/.placeholder
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       23 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/HEAD
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       66 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/config
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       73 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/description
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/info/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      240 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/info/exclude
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/17/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       37 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/17/2c8d5a1db52737ebeb50fe5058212b97ac3f82
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/28/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       29 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/28/ad5b501c13fc618bb395913a2b47ad90e0f51f
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/54/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      130 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/54/81faa232d66589e660cc301179867fb00842c9
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/70/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      169 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/70/35bd33614972ac66559ac1fdd019ff6027ad21
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/b8/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       47 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/b8/f5533d9ab4cbc7a7dee0c1131dfc12e4376524
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/objects/d5/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       48 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/objects/d5/819330d12885aae9c026081d7959fae78eab03
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/scm_data/testrepo/refs/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.457877 module-build-service-3.9.0/tests/scm_data/testrepo/refs/heads/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/refs/heads/dev
+-rw-r--r--   0 breilly   (1000) breilly   (1000)       41 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/scm_data/testrepo/refs/heads/master
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      824 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/bad.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      607 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/build_metadata_module.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      354 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/build_metadata_module_not_processed.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      329 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/fakemodule.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2021 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/formatted_python3-no-components.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1848 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/formatted_testmodule-more-components.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2244 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/formatted_testmodule.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      975 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/includedmodules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-child-master-20170816080815/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-child-master-20170816080815/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1449 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-child-master-20170816080815/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-parent-master-20170816080815/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-parent-master-20170816080815/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1301 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-parent-master-20170816080815/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f28-3/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f28-3/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1233 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f28-3/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f30-3/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f30-3/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      473 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f30-3/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1147 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.459877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1147 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/modules.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.449877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.460877 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1202 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/modules.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1273 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/staged_data/nginx_mmd.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      789 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/staged_data/platform.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1288 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/python3-no-components.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    43738 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/shared-userspace-570.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    43738 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/shared-userspace-577.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      783 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/staged_data/static_context_v2.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-buildrequires-f30.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1157 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/staged_data/testmodule-dashed-stream.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1205 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-forbidden-xmd.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      971 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-local-build.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1114 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-more-components.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      976 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-no-base-module.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      598 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-no-deps.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1222 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-version-set.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      988 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-with-filters.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1223 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule-wrong-stream.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1163 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_br_metadata_module.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2473 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_dependencies.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1133 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_el8.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1141 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_el800.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1141 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_el821.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1387 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/staged_data/testmodule_init.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      993 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_mse.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      989 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_platform_f290000.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      977 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_v2.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1001 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/staged_data/testmodule_v2_buildonly.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.460877 module-build-service-3.9.0/tests/staged_data/v3/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1051 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/staged_data/v3/mmd_packager.yaml
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.460877 module-build-service-3.9.0/tests/test_build/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_build/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    78132 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_build/test_build.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.460877 module-build-service-3.9.0/tests/test_builder/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_builder/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2202 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_builder/test_base.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    12418 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_builder/test_builder_utils.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    48113 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_builder/test_content_generator.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    25714 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_builder/test_get_generator_json_expected_output.json
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    25982 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_builder/test_get_generator_json_expected_output_with_log.json
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    26558 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_builder/test_get_generator_json_rpms_in_tag.json
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    42030 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_builder/test_koji.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    23966 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_builder/test_mock.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.461877 module-build-service-3.9.0/tests/test_common/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      507 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_config.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      492 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_common/test_koji.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    15595 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_common/test_logger.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2875 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_messaging.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.461877 module-build-service-3.9.0/tests/test_common/test_models/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_models/__init__.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.461877 module-build-service-3.9.0/tests/test_common/test_models/data/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)   465266 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_models/data/base-runtime.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1259 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_models/data/testmodule.yaml
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     7947 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_models/test_models.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2995 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_monitor.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     5005 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_common/test_resolve.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     5041 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_common/test_scm.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1785 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_common/test_submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     9519 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_common/test_utils.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     9109 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_manage.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.461877 module-build-service-3.9.0/tests/test_memory/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_memory/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      942 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_memory/mbs_configuration.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     1994 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_memory/mbs_debug.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     3694 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_memory/test_memory.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.462877 module-build-service-3.9.0/tests/test_resolver/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_resolver/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    16076 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_resolver/test_db.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    13897 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_resolver/test_koji.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2160 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_resolver/test_local.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    26781 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_resolver/test_mbs.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.462877 module-build-service-3.9.0/tests/test_scheduler/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    17275 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_scheduler/test_batches.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4257 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_celery_route_task.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4069 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_consumer.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      865 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_db_session.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    22196 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_default_modules.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     7914 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_module_init.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     4111 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_module_states.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     9215 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_module_wait.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    22637 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_scheduler/test_poller.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     9458 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_repo_done.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    22429 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_reuse.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    16164 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_scheduler/test_submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    22744 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_tag_tagged.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    14761 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_scheduler/test_ursine.py
+drwxr-xr-x   0 breilly   (1000) breilly   (1000)        0 2023-04-18 15:15:48.463877 module-build-service-3.9.0/tests/test_web/
+-rw-r--r--   0 breilly   (1000) breilly   (1000)        0 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_web/__init__.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)      490 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_web/client_secrets.json
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    11913 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_web/test_auth.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    18114 2023-03-24 19:41:06.000000 module-build-service-3.9.0/tests/test_web/test_mmd_resolver.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    32362 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_web/test_mse.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)    17071 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tests/test_web/test_submit.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)   127952 2023-04-04 16:42:49.000000 module-build-service-3.9.0/tests/test_web/test_views.py
+-rw-r--r--   0 breilly   (1000) breilly   (1000)     2916 2023-03-24 19:41:27.000000 module-build-service-3.9.0/tox.ini
```

### Comparing `module-build-service-3.8.0/LICENSE` & `module-build-service-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/README.rst` & `module-build-service-3.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -899,15 +899,17 @@
 - If Flask app running within mod_wsgi is detected,
   ProdConfiguration is assumed.
 - If environment variables determining configuration file/section are found,
   they are used for configuration. Following environment variables are
   recognized:
 
     - ``MBS_CONFIG_FILE``: Overrides default configuration file location,
-      typically ``/etc/module-build-service/config.py``.
+      typically ``/etc/module-build-service/config.py``. If set to the
+      empty string, no configuration file will be read and default
+      values will be used.
     - ``MBS_CONFIG_SECTION``: Overrides configuration section.
 
   It is possible to set these values in httpd using ``SetEnv``,
   anywhere in ``/etc/profile.d/`` etc.
 
 - If test-runtime environment is detected,
   TestConfiguration is used, otherwise...
```

### Comparing `module-build-service-3.8.0/client/mbs-cli` & `module-build-service-3.9.0/client/mbs-cli`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/conf/koji.conf` & `module-build-service-3.9.0/conf/koji.conf`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/docs/CHANGELOG.rst` & `module-build-service-3.9.0/docs/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Change Log
 ==========
 
+v3.9.0
+------
+* Replace flask-script with click
+* Allow krb cache to be configured
+* Provide missing fields in API
+* Local build improvements
+
 v3.8.0
 ------
 * Use branch name as default component ref
 
 v3.7.0
 ------
 * Architecture limited module builds fail to build locally
```

### Comparing `module-build-service-3.8.0/docs/CONTRIBUTING.rst` & `module-build-service-3.9.0/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/docs/DEPENDENCY_RESOLUTION.rst` & `module-build-service-3.9.0/docs/DEPENDENCY_RESOLUTION.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/docs/HOW_MBS_BUILDS_MODULES.rst` & `module-build-service-3.9.0/docs/HOW_MBS_BUILDS_MODULES.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/docs/KOJI_RESOLVER.rst` & `module-build-service-3.9.0/docs/KOJI_RESOLVER.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/docs/MODULE_NAMING.rst` & `module-build-service-3.9.0/docs/MODULE_NAMING.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/docs/OFFLINE_LOCAL_BUILDS.rst` & `module-build-service-3.9.0/docs/OFFLINE_LOCAL_BUILDS.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/docs/REBUILD_STRATEGIES.rst` & `module-build-service-3.9.0/docs/REBUILD_STRATEGIES.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/docs/STATIC_CONTEXTS.rst` & `module-build-service-3.9.0/docs/STATIC_CONTEXTS.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/docs/VIRTUAL_MODULES.rst` & `module-build-service-3.9.0/docs/VIRTUAL_MODULES.rst`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/fedmsg.d/module_build_service.py` & `module-build-service-3.9.0/fedmsg.d/module_build_service.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/__init__.py` & `module-build-service-3.9.0/module_build_service/__init__.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/builder/KojiContentGenerator.py` & `module-build-service-3.9.0/module_build_service/builder/KojiContentGenerator.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/builder/KojiModuleBuilder.py` & `module-build-service-3.9.0/module_build_service/builder/KojiModuleBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from module_build_service.builder.utils import execute_cmd, get_rpm_release, validate_koji_tag
 from module_build_service.common import log, conf, models
 from module_build_service.common.koji import (
     get_session, koji_multicall_map, koji_retrying_multicall_map,
 )
 from module_build_service.common.retry import retry
 from module_build_service.scheduler import events
-from module_build_service.scheduler.db_session import db_session
 from module_build_service.scheduler.reuse import get_reusable_components, get_reusable_module
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 @contextlib.contextmanager
 def set_locale(*args, **kwargs):
@@ -353,28 +352,28 @@
         sources_dir = os.path.join(td, "SOURCES")
         os.mkdir(sources_dir)
         fd = open(os.path.join(sources_dir, "macros.modules"), "w")
         fd.write(macros_content)
         fd.close()
         log.debug("Building %s.spec" % name)
 
-        # We are not interested in the rpmbuild stdout...
+        # We are not interested in the rpmbuild output...
         null_fd = open(os.devnull, "w")
         execute_cmd(
             [
                 "rpmbuild",
                 "-bs",
                 "%s.spec" % name,
                 "--define",
                 "_topdir %s" % td,
                 "--define",
                 "_sourcedir %s" % sources_dir,
             ],
             cwd=td,
-            stdout=null_fd,
+            output=null_fd,
         )
         null_fd.close()
         sdir = os.path.join(td, "SRPMS")
         srpm_paths = glob.glob("%s/*.src.rpm" % sdir)
         assert len(srpm_paths) == 1, "Expected exactly 1 srpm in %s. Got %s" % (sdir, srpm_paths)
 
         log.debug("Wrote srpm into %s" % srpm_paths[0])
@@ -1163,28 +1162,22 @@
             for task in tasks.values():
                 weight += sum([t["weight"] for t in task])
             weights[component_name] = weight
 
         return weights
 
     @classmethod
-    def get_built_rpms_in_module_build(cls, mmd):
+    def get_built_rpms_in_module_build(cls, mmd, koji_tag):
         """
         :param Modulemd mmd: Modulemd to get the built RPMs from.
+        :koji_tag str: koji_tag corresponding to the module
         :return: list of NVRs
         """
-        build = models.ModuleBuild.get_build_from_nsvc(
-            db_session,
-            mmd.get_module_name(),
-            mmd.get_stream_name(),
-            mmd.get_version(),
-            mmd.get_context()
-        )
         koji_session = get_session(conf, login=False)
-        rpms = koji_session.listTaggedRPMS(build.koji_tag, latest=True)[0]
+        rpms = koji_session.listTaggedRPMS(koji_tag, latest=True)[0]
         nvrs = set(kobo.rpmlib.make_nvr(rpm, force_epoch=True) for rpm in rpms)
         return list(nvrs)
 
     def finalize(self, succeeded=True):
         # Only import to koji CG if the module is "build" and not scratch.
         if (
             not self.module.scratch
```

### Comparing `module-build-service-3.8.0/module_build_service/builder/MockModuleBuilder.py` & `module-build-service-3.9.0/module_build_service/builder/MockModuleBuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # SPDX-License-Identifier: MIT
 from __future__ import absolute_import
 import logging
 import os
 import pipes
 import re
 import subprocess
+from textwrap import dedent
 import threading
 
 import dnf
 import koji
 import kobo.rpmlib
 import platform
 
@@ -18,15 +19,15 @@
 from module_build_service.builder.utils import (
     create_local_repo_from_koji_tag,
     execute_cmd,
     find_srpm,
     get_koji_config,
     validate_koji_tag,
 )
-from module_build_service.common import conf, log, models
+from module_build_service.common import build_logs, conf, log, models
 from module_build_service.common.koji import get_session
 from module_build_service.common.modulemd import Modulemd
 from module_build_service.common.utils import import_mmd, load_mmd_file, mmd_to_str
 from module_build_service.scheduler import events
 from module_build_service.scheduler.db_session import db_session
 
 logging.basicConfig(level=logging.DEBUG)
@@ -404,22 +405,24 @@
         # There is no way to replace the RPM artifacts, so remove any extra RPM artifacts
         for artifact_to_remove in (set(m1_mmd.get_rpm_artifacts()) - artifacts):
             m1_mmd.remove_rpm_artifact(artifact_to_remove)
         for artifact_to_add in (artifacts - set(m1_mmd.get_rpm_artifacts())):
             m1_mmd.add_rpm_artifact(artifact_to_add)
 
         # Generate repo.
-        execute_cmd(["/usr/bin/createrepo_c", "--pkglist", pkglist, path])
+        execute_cmd(["/usr/bin/createrepo_c", "--pkglist", pkglist, path],
+                    output=build_logs.current_log_stream)
 
         # ...and inject modules.yaml there if asked.
         if include_module_yaml:
             mmd_path = os.path.join(path, "modules.yaml")
             with open(mmd_path, "wb") as f:
                 f.write(mmd_to_str(m1_mmd).encode("utf-8"))
-            execute_cmd(["/usr/bin/modifyrepo_c", "--mdtype=modules", mmd_path, repodata_path])
+            execute_cmd(["/usr/bin/modifyrepo_c", "--mdtype=modules", mmd_path, repodata_path],
+                        output=build_logs.current_log_stream)
 
     def _add_repo(self, name, baseurl, extra=""):
         """
         Adds repository to Mock config file. Call _write_mock_config() to
         actually write the config file to filesystem.
         """
         self.yum_conf += "[%s]\n" % name
@@ -464,41 +467,52 @@
                 exec(code)  # nosec
 
                 self.groups = config_opts["chroot_setup_cmd"].split(" ")[1:]
                 self.yum_conf = config_opts["yum.conf"]
                 self.enabled_modules = config_opts["module_enable"]
                 self.releasever = config_opts["releasever"]
 
-    def _write_mock_config(self):
+    def _write_mock_config(self, update_main=False):
         """
         Writes Mock config file to local file.
         """
 
         with MockModuleBuilder._config_lock:
             config = str(MockModuleBuilder.mock_config_template)
             config = config.replace(
                 "$root", "%s-%s" % (self.tag_name, str(threading.current_thread().name)))
             config = config.replace("$arch", self.arch)
             config = config.replace("$group", " ".join(self.groups))
-            config = config.replace("$yum_conf", self.yum_conf)
+            config = config.replace("$yum_conf", self.yum_conf.strip())
             config = config.replace("$enabled_modules", str(self.enabled_modules))
             config = config.replace("$releasever", str(self.releasever))
 
-            # We write the most recent config to "mock.cfg", so thread-related
-            # configs can be later (re-)generated from it using _load_mock_config.
-            outfile = os.path.join(self.configdir, "mock.cfg")
-            with open(outfile, "w") as f:
-                f.write(config)
+            config += dedent("""\
+                config_opts.setdefault('plugin_conf', {})
+                config_opts['plugin_conf'].setdefault('root_cache_opts', {})
+                config_opts['plugin_conf']['root_cache_opts']['dir'] = "{{cache_topdir}}/%s/root_cache/"
+            """) % self.tag_name
+
+            mock_cfg_path = os.path.join(self.configdir, "mock.cfg")
+            if update_main or not os.path.exists(mock_cfg_path):
+                # We write a config to "mock.cfg", so thread-related
+                # configs can be later (re-)generated from it using _load_mock_config.
+                with open(mock_cfg_path, "w") as f:
+                    f.write(config)
+
+            mtime = os.path.getmtime(mock_cfg_path)
 
             # Write the config to thread-related configuration file.
             outfile = os.path.join(
                 self.configdir, "mock-%s.cfg" % str(threading.current_thread().name))
             with open(outfile, "w") as f:
                 f.write(config)
 
+            os.utime(outfile, (mtime, mtime))
+
     def buildroot_connect(self, groups):
         self._load_mock_config()
         self.groups = list(set().union(groups["build"], self.groups))
         log.debug("Mock builder groups: %s" % self.groups)
         self._write_mock_config()
 
     def buildroot_prep(self):
@@ -521,19 +535,19 @@
         # buildroot. We should really install the RPMs belonging to the
         # right source RPM into the buildroot here, but we do not track
         # what RPMs are output of particular SRPM build yet.
         for artifact in artifacts:
             if artifact and artifact.startswith("module-build-macros"):
                 self._load_mock_config()
                 self.groups.append("module-build-macros")
-                self._write_mock_config()
+                self._write_mock_config(update_main=True)
 
         events.scheduler.add(repos_done_handler, ("fake_msg", self.tag_name + "-build"))
 
-    def tag_artifacts(self, artifacts):
+    def tag_artifacts(self, artifacts, dest_tag=False):
         pass
 
     def buildroot_add_repos(self, dependencies):
         self._load_mock_config()
         for source, mmds in dependencies.items():
             # If source starts with mock_resultdir, it means it is path to local
             # module build repository.
@@ -582,15 +596,15 @@
                     should_add_repo = create_local_repo_from_koji_tag(
                         self.config, tag, repo_dir, [self.arch, "noarch"])
                     if not should_add_repo:
                         continue
                     baseurl = "file://" + repo_dir
 
             self._add_repo(repo_name, baseurl)
-        self._write_mock_config()
+        self._write_mock_config(update_main=True)
 
     def _send_build_change(self, state, source, build_id):
         from module_build_service.scheduler.handlers.components import (
             build_task_finalize as build_task_finalize_handler)
         try:
             nvr = kobo.rpmlib.parse_nvr(source)
         except ValueError:
@@ -604,19 +618,23 @@
 
     def _save_log(self, resultsdir, log_name, artifact_name):
         old_log = os.path.join(resultsdir, log_name)
         new_log = os.path.join(resultsdir, artifact_name + "-" + log_name)
         if os.path.exists(old_log):
             os.rename(old_log, new_log)
 
-    def _purge_useless_logs(self):
+    def _purge_useless_logs(self, artifact_name):
         """
         Remove empty or otherwise useless log files
         """
+        prefix = artifact_name + "-"
+
         for logf in os.listdir(self.resultsdir):
+            if not logf.startswith(prefix):
+                continue
 
             log_path = os.path.join(self.resultsdir, logf)
 
             # Remove empty files
             if os.path.isfile(log_path) and os.path.getsize(log_path) == 0:
                 os.remove(log_path)
 
@@ -626,32 +644,29 @@
         """
         state = koji.BUILD_STATES["BUILDING"]
 
         # Use the mock config associated with this thread.
         mock_config = os.path.join(
             self.configdir, "mock-%s.cfg" % str(threading.current_thread().name))
 
-        # Open the logs to which we will forward mock stdout/stderr.
-        mock_stdout_log = open(
-            os.path.join(self.resultsdir, artifact_name + "-mock-stdout.log"), "w")
-        mock_stderr_log = open(
-            os.path.join(self.resultsdir, artifact_name + "-mock-stderr.log"), "w")
+        # Open the log to which we will forward mock stdout/stderr.
+        mock_output_log = open(
+            os.path.join(self.resultsdir, artifact_name + "-mock-output.log"), "w")
 
         srpm = artifact_name
         resultsdir = builder.resultsdir
         try:
             # Initialize mock.
             execute_cmd(
-                ["mock", "-v", "-r", mock_config, "--init"],
-                stdout=mock_stdout_log,
-                stderr=mock_stderr_log,
+                ["mock", "-r", mock_config, "--init"],
+                output=mock_output_log,
             )
 
             # Start the build and store results to resultsdir
-            builder.build(mock_stdout_log, mock_stderr_log)
+            builder.build(mock_output_log)
             srpm = find_srpm(resultsdir)
 
             # Emit messages simulating complete build. These messages
             # are put in the scheduler's work queue and are handled
             # by MBS after the build_srpm() method returns and scope gets
             # back to scheduler.main.main() method.
             state = koji.BUILD_STATES["COMPLETE"]
@@ -667,29 +682,28 @@
             # by MBS after the build_srpm() method returns and scope gets
             # back to scheduler.main.main() method.
             state = koji.BUILD_STATES["FAILED"]
             self._send_build_change(state, srpm, build_id)
             with open(os.path.join(resultsdir, "status.log"), "w") as f:
                 f.write("failed\n")
 
-        mock_stdout_log.close()
-        mock_stderr_log.close()
+        mock_output_log.close()
 
         self._save_log(resultsdir, "state.log", artifact_name)
         self._save_log(resultsdir, "root.log", artifact_name)
         self._save_log(resultsdir, "build.log", artifact_name)
         self._save_log(resultsdir, "status.log", artifact_name)
 
-        # Copy files from thread-related resultsdire to the main resultsdir.
+        # Copy files from thread-related resultsdir to the main resultsdir.
         for name in os.listdir(resultsdir):
             os.rename(os.path.join(resultsdir, name), os.path.join(self.resultsdir, name))
 
         # Depending on the configuration settings, remove/keep useless log files
         if conf.mock_purge_useless_logs:
-            self._purge_useless_logs()
+            self._purge_useless_logs(artifact_name)
 
         # We return BUILDING state here even when we know it is already
         # completed or failed, because otherwise utils.start_build_batch
         # would think this component is already built and also tagged, but
         # we have just built it - tagging will happen as result of build
         # change message we are sending above using _send_build_change.
         # It is just to make this backend compatible with other backends,
@@ -749,32 +763,25 @@
         # For successful builds, do one last createrepo, to include
         # the module metadata. We don't want to do this for failed builds,
         # since that makes it impossible to retry a build manually.
         if succeeded:
             self._createrepo(include_module_yaml=True)
 
     @classmethod
-    def get_built_rpms_in_module_build(cls, mmd):
+    def get_built_rpms_in_module_build(cls, mmd, koji_tag):
         """
         :param Modulemd mmd: Modulemd to get the built RPMs from.
         :return: list of NVRs
         """
-        build = models.ModuleBuild.get_build_from_nsvc(
-            db_session,
-            mmd.get_module_name(),
-            mmd.get_stream_name(),
-            mmd.get_version(),
-            mmd.get_context()
-        )
-        if build.koji_tag.startswith("repofile://"):
+        if koji_tag.startswith("repofile://"):
             # Modules from local repository have already the RPMs filled in mmd.
             return mmd.get_rpm_artifacts()
         else:
             koji_session = get_session(conf, login=False)
-            rpms = koji_session.listTaggedRPMS(build.koji_tag, latest=True)[0]
+            rpms = koji_session.listTaggedRPMS(koji_tag, latest=True)[0]
             nvrs = set(kobo.rpmlib.make_nvr(rpm, force_epoch=True) for rpm in rpms)
             return list(nvrs)
 
     def get_average_build_time(self, component):
         """
         Get the average build time of the component from Koji
         :param component: a ComponentBuild object
@@ -795,64 +802,66 @@
                 return 0.0
 
 
 class BaseBuilder(object):
     def __init__(self, config, resultsdir):
         self.config = config
         self.resultsdir = resultsdir
-        self.cmd = ["mock", "-v", "-r", config, "--no-clean", "--resultdir=%s" % resultsdir]
+        self.cmd = ["mock", "-r", config, "--no-clean", "--resultdir=%s" % resultsdir]
 
-    def build(self, stdout, stderr):
-        execute_cmd(self.cmd, stdout=stdout, stderr=stderr)
+    def build(self, output):
+        execute_cmd(self.cmd, output=output)
 
 
 class SRPMBuilder(BaseBuilder):
     def __init__(self, config, resultsdir, source):
         super(SRPMBuilder, self).__init__(config, resultsdir)
         self.cmd.extend(["--rebuild", source])
 
 
 class SCMBuilder(BaseBuilder):
     def __init__(self, config, resultsdir, source, artifact_name):
         super(SCMBuilder, self).__init__(config, resultsdir)
-        with open(config, "a") as f:
-            repo_path, branch = source.split("?#")
-            distgit_cmds = self._get_distgit_commands(source)
-            # Supply the artifact name for "{0}" and the full path to the repo for "{repo_path}"
-            distgit_get = distgit_cmds[0].format(artifact_name, repo_path=repo_path)
-
-            # mock-scm cannot checkout particular commit hash, but only branch.
-            # We therefore use a command that combines the distgit-command with
-            # checking out a particular commit hash.
-            # See https://bugzilla.redhat.com/show_bug.cgi?id=1459437 for
-            # more info. Once mock-scm supports this feature, we can remove
-            # this code.
-            distgit_get_branch = "sh -c {}'; git -C {} checkout {}'".format(
-                pipes.quote(distgit_get), artifact_name, branch)
-
-            f.writelines([
-                "config_opts['scm'] = True\n",
-                "config_opts['scm_opts']['method'] = 'distgit'\n",
-                "config_opts['scm_opts']['package'] = '{}'\n".format(artifact_name),
-                "config_opts['scm_opts']['distgit_get'] = {!r}\n".format(distgit_get_branch),
-            ])
-
-            # Set distgit_src_get only if it's defined.
-            if distgit_cmds[1]:
-                f.write(
-                    "config_opts['scm_opts']['distgit_src_get'] = '{}'\n".format(distgit_cmds[1]))
-
-            # The local git repositories cloned by `fedpkg clone` typically do not have
-            # the tarballs with sources committed in a git repo. They normally live in lookaside
-            # cache on remote server, but we should not try getting them from there for true
-            # local builds.
-            # Instead, get them from local path with git repository by passing that path to Mock
-            # using the `ext_src_dir`.
-            if repo_path.startswith("file://"):
-                src_dir = repo_path[len("file://"):]
-                f.write("config_opts['scm_opts']['ext_src_dir'] = '{}'\n".format(src_dir))
+
+        repo_path, branch = source.split("?#")
+        distgit_cmds = self._get_distgit_commands(source)
+        # Supply the artifact name for "{0}" and the full path to the repo for "{repo_path}"
+        distgit_get = distgit_cmds[0].format(artifact_name, repo_path=repo_path)
+
+        # mock-scm cannot checkout particular commit hash, but only branch.
+        # We therefore use a command that combines the distgit-command with
+        # checking out a particular commit hash.
+        # See https://bugzilla.redhat.com/show_bug.cgi?id=1459437 for
+        # more info. Once mock-scm supports this feature, we can remove
+        # this code.
+        distgit_get_branch = "sh -c {}'; git -C {} checkout {}'".format(
+            pipes.quote(distgit_get), artifact_name, branch)
+
+        scm_options = [
+            ('method', 'distgit'),
+            ('package', artifact_name),
+            ('distgit_get', distgit_get_branch),
+        ]
+
+        # Set distgit_src_get only if it's defined.
+        if distgit_cmds[1]:
+            scm_options.append(('distgit_src_get', distgit_cmds[1]))
+
+        # The local git repositories cloned by `fedpkg clone` typically do not have
+        # the tarballs with sources committed in a git repo. They normally live in lookaside
+        # cache on remote server, but we should not try getting them from there for true
+        # local builds.
+        # Instead, get them from local path with git repository by passing that path to Mock
+        # using the `ext_src_dir`.
+        if repo_path.startswith("file://"):
+            src_dir = repo_path[len("file://"):]
+            scm_options.append(('ext_src_dir', src_dir))
+
+        self.cmd.append('--scm-enable')
+        for name, value in scm_options:
+            self.cmd.extend(('--scm-option', '{}={}'.format(name, value)))
 
     def _get_distgit_commands(self, source):
         for host, cmds in conf.distgits.items():
             if source.startswith(host):
                 return cmds
         raise KeyError("No defined commands for {}".format(source))
```

### Comparing `module-build-service-3.8.0/module_build_service/builder/base.py` & `module-build-service-3.9.0/module_build_service/builder/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,17 +342,18 @@
 
         This method is supposed to list tasks ('active' by default)
         for component builds.
         """
         raise NotImplementedError()
 
     @classmethod
-    def get_built_rpms_in_module_build(cls, mmd):
+    def get_built_rpms_in_module_build(cls, mmd, koji_tag):
         """
         :param Modulemd mmd: Modulemd to get the built RPMs from.
+        :koji_tag str: koji_tag corresponding to the module
         :return: list of NVRs
         """
         raise NotImplementedError()
 
     @classmethod
     def get_module_build_arches(cls, module):
         """
```

### Comparing `module-build-service-3.8.0/module_build_service/builder/utils.py` & `module-build-service-3.9.0/module_build_service/builder/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,54 +9,50 @@
 import os
 import shutil
 import subprocess
 
 import munch
 import requests
 
-from module_build_service.common import conf, log, models
+from module_build_service.common import build_logs, conf, log, models
 from module_build_service.common.errors import ValidationError, ProgrammingError
 
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def find_srpm(cod):
     for f in os.listdir(cod):
         if f.endswith(".src.rpm"):
             return os.path.join(cod, f)
 
 
-def execute_cmd(args, stdout=None, stderr=None, cwd=None):
+def execute_cmd(args, output=None, cwd=None):
     """
-    Executes command defined by `args`. If `stdout` or `stderr` is set to
-    Python file object, the stderr/stdout output is redirecter to that file.
+    Executes command defined by `args`. If `output` is set to
+    Python file object, the stderr and stdout output is redirected to that file.
     If `cwd` is set, current working directory is set accordingly for the
     executed command.
 
     :param args: list defining the command to execute.
-    :param stdout: Python file object to redirect the stdout to.
-    :param stderr: Python file object to redirect the stderr to.
+    :param output: Python file object to redirect the stderr and stdout to.
     :param cwd: string defining the current working directory for command.
     :raises RuntimeError: Raised when command exits with non-zero exit code.
     """
     out_log_msg = ""
-    if stdout and hasattr(stdout, "name"):
-        out_log_msg += ", stdout log: %s" % stdout.name
-    if stderr and hasattr(stderr, "name"):
-        out_log_msg += ", stderr log: %s" % stderr.name
+    if output and hasattr(output, "name"):
+        out_log_msg += ", output log: %s" % output.name
 
     log.info("Executing the command \"%s\"%s" % (" ".join(args), out_log_msg))
-    proc = subprocess.Popen(args, stdout=stdout, stderr=stderr, cwd=cwd)
-    out, err = proc.communicate()
+    proc = subprocess.Popen(args, stdout=output, stderr=output, cwd=cwd)
+    proc.wait()
 
     if proc.returncode != 0:
         err_msg = "Command '%s' returned non-zero value %d%s" % (args, proc.returncode, out_log_msg)
         raise RuntimeError(err_msg)
-    return out, err
 
 
 def get_koji_config(mbs_config):
     """
     Get the Koji config needed for MBS
     :param mbs_config: an MBS config object
     :return: a Munch object of the Koji config
@@ -79,14 +75,16 @@
 
     If the there are no builds associated with the tag, False is returned.
     """
 
     # Placed here to avoid py2/py3 conflicts...
     import koji
 
+    log.local_repo_start(tag)
+
     if not archs:
         archs = ["x86_64", "noarch"]
 
     # Load koji config and create Koji session.
     koji_config = get_koji_config(config)
     address = koji_config.server
     log.debug("Connecting to koji %r" % address)
@@ -96,14 +94,15 @@
     try:
         rpms, builds = session.listTaggedRPMS(tag, latest=True)
     except koji.GenericError:
         log.exception("Failed to list rpms in tag %r" % tag)
 
     if not builds:
         log.debug("No builds are associated with the tag %r", tag)
+        log.local_repo_done(tag, 'No builds to download')
         return False
 
     # Reformat builds so they are dict with build_id as a key.
     builds = {build["build_id"]: build for build in builds}
 
     # Prepare pathinfo we will use to generate the URL.
     pathinfo = koji.PathInfo(topdir=session.opts["topurl"])
@@ -126,56 +125,66 @@
         local_fn = os.path.join(repo_dir, relpath)
         # Download only when the RPM is not downloaded or the size does not match.
         if not os.path.exists(local_fn) or os.path.getsize(local_fn) != rpm["size"]:
             if os.path.exists(local_fn):
                 os.remove(local_fn)
             repo_changed = True
             url = pathinfo.build(build_info) + "/" + fname
-            download_args.append((url, local_fn))
+            download_args.append((tag, url, local_fn))
 
-    log.info("Downloading %d packages from Koji tag %s to %s" % (len(download_args), tag, repo_dir))
+    if repo_changed:
+        log.local_repo_start_downloads(tag, len(download_args), repo_dir)
+    else:
+        log.local_repo_done(tag, 'All builds already downloaded')
 
     # Create the output directory
     try:
         os.makedirs(repo_dir)
     except OSError as exception:
         if exception.errno != errno.EEXIST:
             raise
 
-    def _download_file(url_and_dest):
+    def _download_file(tag_url_and_dest):
         """
         Download a file in a memory efficient manner
-        :param url_and_dest: a tuple containing the URL and the destination to download to
+        :param url_and_dest: a tuple containing the tag, the URL and the destination to download to
         :return: None
         """
-        log.info("Downloading {0}...".format(url_and_dest[0]))
-        if len(url_and_dest) != 2:
-            raise ValueError("url_and_dest must have two values")
+        assert len(tag_url_and_dest) == 3, "tag_url_and_dest must have three values"
+
+        tag, url, dest = tag_url_and_dest
 
-        rv = requests.get(url_and_dest[0], stream=True, timeout=60)
-        with open(url_and_dest[1], "wb") as f:
+        log.local_repo_start_download(tag, url)
+
+        rv = requests.get(url, stream=True, timeout=60)
+        with open(dest, "wb") as f:
             for chunk in rv.iter_content(chunk_size=1024):
                 if chunk:
                     f.write(chunk)
 
+        log.local_repo_done_download(tag, url)
+
     # Download the RPMs four at a time.
     pool = ThreadPool(4)
     try:
         pool.map(_download_file, download_args)
     finally:
         pool.close()
 
     # If we downloaded something, run the createrepo_c.
     if repo_changed:
         repodata_path = os.path.join(repo_dir, "repodata")
         if os.path.exists(repodata_path):
             shutil.rmtree(repodata_path)
 
         log.info("Creating local repository in %s" % repo_dir)
-        execute_cmd(["/usr/bin/createrepo_c", repo_dir])
+        execute_cmd(["/usr/bin/createrepo_c", repo_dir],
+                    output=build_logs.current_log_stream)
+
+        log.local_repo_done(tag, 'Finished downloading packages')
 
     return True
 
 
 def get_rpm_release(db_session, module_build):
     """
     Generates the dist tag for the specified module
```

### Comparing `module-build-service-3.8.0/module_build_service/common/config.py` & `module-build-service-3.9.0/module_build_service/common/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 from __future__ import absolute_import
+import errno
 import imp
 import logging
 import os
 import re
 import sys
 import tempfile
 
@@ -71,17 +72,20 @@
 
 
 class ProdConfiguration(BaseConfiguration):
     pass
 
 
 class LocalBuildConfiguration(BaseConfiguration):
+    SYSTEM = "mock"
+
     CACHE_DIR = "~/modulebuild/cache"
     LOG_LEVEL = "debug"
     MESSAGING = "drop"
+    BUILD_LOGS_NAME_FORMAT = "build.log"
 
     ALLOW_CUSTOM_SCMURLS = True
     RESOLVER = "mbs"
     RPMS_ALLOW_REPOSITORY = True
     MODULES_ALLOW_REPOSITORY = True
 
     # Match the Fedora server-side configuration
@@ -104,23 +108,35 @@
     Create the global MBS configuration.
 
     :return: a tuple with the first index being the configuration and second index as the
         configuration class that was used to initialize the configuration. This can be useful
         to configure Flask with.
     :rtype: tuple(Config, object)
     """
-    config_file = os.environ.get("MBS_CONFIG_FILE", "/etc/module-build-service/config.py")
+    env_config_file = os.environ.get("MBS_CONFIG_FILE")
+    if env_config_file is None:
+        config_file = "/etc/module-build-service/config.py"
+    else:
+        config_file = env_config_file
+
+    config_module = None
+
+    # MBS_CONFIG_FILE="" entirely suppresses looking a config file
+    if config_file != "":
+        try:
+            config_module = imp.load_source("mbs_runtime_config", config_file)
+            log.info("Using the configuration file at %s", config_file)
+        except OSError as e:
+            if e.errno != errno.ENOENT or env_config_file:
+                log.error("Can't open config file: %s", e)
 
-    try:
-        config_module = imp.load_source("mbs_runtime_config", config_file)
-        log.info("Using the configuration file at %s", config_file)
-    except Exception:
-        log.warning("The configuration file at %s was not present", config_file)
+    if config_module is None:
         # Default to this file as the configuration module
         config_module = sys.modules[__name__]
+        log.debug("Using default configuration")
 
     true_options = ("1", "on", "true", "y", "yes")
     if any(["py.test" in arg or "pytest" in arg for arg in sys.argv]):
         config_section = "TestConfiguration"
         # Get the configuration from this module
         config_module = sys.modules[__name__]
     elif os.environ.get("MODULE_BUILD_SERVICE_DEVELOPER_ENV", "").lower() in true_options:
@@ -316,14 +332,15 @@
             "desc": (
                 "Format of a module build log's name. Use `Build` attributes as formatting "
                 "kwargs"
             ),
         },
         "krb_keytab": {"type": None, "default": None, "desc": ""},
         "krb_principal": {"type": None, "default": None, "desc": ""},
+        'krb_ccache': {"type": None, "default": "KEYRING:thread:mbs", "desc": ""},
         "messaging": {"type": str, "default": "fedmsg", "desc": "The messaging system to use."},
         "messaging_topic_prefix": {
             "type": list,
             "default": ["org.fedoraproject.prod"],
             "desc": "The messaging system topic prefixes which we are interested in.",
         },
         "distgits": {
```

### Comparing `module-build-service-3.8.0/module_build_service/common/errors.py` & `module-build-service-3.9.0/module_build_service/common/errors.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/common/koji.py` & `module-build-service-3.9.0/module_build_service/common/koji.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,31 +131,26 @@
 
     if not login:
         return koji_session
 
     authtype = koji_config.authtype
     log.info("Authenticate session with %r.", authtype)
     if authtype == "kerberos":
-        try:
-            import krbV
-            # We want to create a context per thread to avoid Kerberos cache corruption
-            ctx = krbV.Context()
-        except ImportError:
-            # If no krbV, we can assume GSSAPI auth is available
-            ctx = None
         keytab = getattr(config, "krb_keytab", None)
         principal = getattr(config, "krb_principal", None)
         if not keytab and principal:
             raise ValueError(
                 "The Kerberos keytab and principal aren't set for Koji authentication")
         log.debug("  keytab: %r, principal: %r" % (keytab, principal))
         # We want to use the thread keyring for the ccache to ensure we have one cache per
         # thread to avoid Kerberos cache corruption
-        ccache = "KEYRING:thread:mbs"
-        koji_session.krb_login(principal=principal, keytab=keytab, ctx=ctx, ccache=ccache)
+        # Keyring may be inaccessible in containers, so let's allow it to be configured
+        ccache = getattr(config, "krb_ccache", None)
+        log.debug("  ccache: %r" % (ccache))
+        koji_session.gssapi_login(principal=principal, keytab=keytab, ccache=ccache)
     elif authtype == "ssl":
         koji_session.ssl_login(
             os.path.expanduser(koji_config.cert), None, os.path.expanduser(koji_config.serverca)
         )
     else:
         raise ValueError("Unrecognized koji authtype %r" % authtype)
```

### Comparing `module-build-service-3.8.0/module_build_service/common/messaging.py` & `module-build-service-3.9.0/module_build_service/common/messaging.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/common/models.py` & `module-build-service-3.9.0/module_build_service/common/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -602,14 +602,18 @@
             u"release": "{0}.{1}".format(self.version, self.context)
         }
 
     @property
     def nvr_string(self):
         return kobo.rpmlib.make_nvr(self.nvr)
 
+    @property
+    def nsvc(self):
+        return "{}:{}:{}:{}".format(self.name, self.stream, self.version, self.context)
+
     @classmethod
     def create(
         cls,
         db_session,
         conf,
         name,
         stream,
@@ -777,17 +781,19 @@
 
     def json(self, db_session, show_tasks=True):
         mmd = self.mmd()
         xmd = mmd.get_xmd()
         buildrequires = xmd.get("mbs", {}).get("buildrequires", {})
         rv = self.short_json()
         rv.update({
+            "batch": self.batch,
             "component_builds": [build.id for build in self.component_builds],
             "koji_tag": self.koji_tag,
             "owner": self.owner,
+            "new_repo_task_id": self.new_repo_task_id,
             "rebuild_strategy": self.rebuild_strategy,
             "scmurl": self.scmurl,
             "srpms": json.loads(self.srpms or "[]"),
             "siblings": self.siblings(db_session),
             "state_reason": self.state_reason,
             "time_completed": _utc_datetime_to_iso(self.time_completed),
             "time_modified": _utc_datetime_to_iso(self.time_modified),
@@ -810,14 +816,15 @@
         state_url = None
         if show_state_url:
             state_url = get_url_for("module_build", api_version=api_version, id=self.id)
 
         rv.update({
             "base_module_buildrequires": [br.short_json(True, False) for br in self.buildrequires],
             "build_context": self.build_context,
+            "build_context_no_bms": self.build_context_no_bms,
             "modulemd": self.modulemd,
             "reused_module_id": self.reused_module_id,
             "runtime_context": self.runtime_context,
             "state_trace": [
                 {
                     "time": _utc_datetime_to_iso(record.state_time),
                     "state": record.state,
```

### Comparing `module-build-service-3.8.0/module_build_service/common/monitor.py` & `module-build-service-3.9.0/module_build_service/common/monitor.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/common/request_utils.py` & `module-build-service-3.9.0/module_build_service/common/request_utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/common/resolve.py` & `module-build-service-3.9.0/module_build_service/common/resolve.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/common/retry.py` & `module-build-service-3.9.0/module_build_service/common/retry.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/common/scm.py` & `module-build-service-3.9.0/module_build_service/common/scm.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/common/submit.py` & `module-build-service-3.9.0/module_build_service/common/submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/common/utils.py` & `module-build-service-3.9.0/module_build_service/common/utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/manage.py` & `module-build-service-3.9.0/module_build_service/manage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,107 +1,67 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 from __future__ import absolute_import, print_function
 from collections import defaultdict
-from functools import wraps
+import click
 import getpass
 import logging
 import os
 import sys
-import textwrap
 
 import flask_migrate
-from flask_script import Manager, prompt_bool
+from flask.cli import FlaskGroup
 from werkzeug.datastructures import FileStorage
 
 from module_build_service import app, db
 from module_build_service.builder.MockModuleBuilder import (
     import_builds_from_local_dnf_repos, load_local_builds
 )
-from module_build_service.common import conf, models
+from module_build_service.common import build_logs, conf, models
 from module_build_service.common.errors import StreamAmbigous, StreamNotXyz
-from module_build_service.common.logger import level_flags
 from module_build_service.common.utils import load_mmd_file, import_mmd
 import module_build_service.scheduler.consumer
 from module_build_service.scheduler.db_session import db_session
 import module_build_service.scheduler.local
 from module_build_service.web.submit import submit_module_build_from_yaml
 
-
-def create_app(debug=False, verbose=False, quiet=False):
-    # logging (intended for flask-script, see manage.py)
-    log = logging.getLogger(__name__)
-    if debug:
-        log.setLevel(level_flags["debug"])
-    elif verbose:
-        log.setLevel(level_flags["verbose"])
-    elif quiet:
-        log.setLevel(level_flags["quiet"])
-
-    return app
-
-
-manager = Manager(create_app)
-help_args = ("-?", "--help")
-manager.help_args = help_args
-migrations_dir = os.path.join(os.path.abspath(os.path.dirname(__file__)),
-                              'migrations')
+migrations_dir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "migrations")
 migrate = flask_migrate.Migrate(app, db, directory=migrations_dir)
-manager.add_command("db", flask_migrate.MigrateCommand)
-manager.add_option("-d", "--debug", dest="debug", action="store_true")
-manager.add_option("-v", "--verbose", dest="verbose", action="store_true")
-manager.add_option("-q", "--quiet", dest="quiet", action="store_true")
-
-
-def console_script_help(f):
-    @wraps(f)
-    def wrapped(*args, **kwargs):
-        import sys
-
-        if any([arg in help_args for arg in sys.argv[1:]]):
-            command = os.path.basename(sys.argv[0])
-            print(textwrap.dedent(
-                """\
-                    {0}
-
-                    Usage: {0} [{1}]
-
-                    See also:
-                    mbs-manager(1)
-                """).strip().format(command, "|".join(help_args))
-            )
-            sys.exit(2)
-        r = f(*args, **kwargs)
-        return r
 
-    return wrapped
+
+@click.group(cls=FlaskGroup, create_app=lambda *args, **kwargs: app)
+def cli():
+    """MBS manager"""
 
 
-@console_script_help
-@manager.command
+@cli.command("upgradedb")
 def upgradedb():
     """ Upgrades the database schema to the latest revision
     """
     app.config["SERVER_NAME"] = "localhost"
-    # TODO: configurable?
-    migrations_dir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "migrations")
     with app.app_context():
         flask_migrate.upgrade(directory=migrations_dir)
 
 
-@manager.command
+def upgradedb_entrypoint():
+    """Entrypoint for command mbs-upgradedb"""
+    # Work around issue with FlaskGroup not being initiated
+    cli(["upgradedb"])
+
+
+@cli.command("cleardb")
 def cleardb():
     """ Clears the database
     """
     models.ModuleBuild.query.delete()
     models.ComponentBuild.query.delete()
 
 
-@console_script_help
-@manager.command
+@cli.command("import_module")
+@click.argument("mmd_file", type=click.Path(exists=True))
 def import_module(mmd_file):
     """ Imports the module from mmd_file
     """
     mmd = load_mmd_file(mmd_file)
     import_mmd(db.session, mmd)
 
 
@@ -113,57 +73,75 @@
             raise ValueError("dependency overrides must be in the form name:stream")
         name, stream = parts
         collected[name].append(stream)
 
     return collected
 
 
-@manager.option("--stream", action="store", dest="stream")
-@manager.option("--file", action="store", dest="yaml_file")
-@manager.option("--srpm", action="append", default=[], dest="srpms", metavar="SRPM")
-@manager.option("--skiptests", action="store_true", dest="skiptests")
-@manager.option("--offline", action="store_true", dest="offline")
-@manager.option(
-    '--buildrequires', action='append', metavar='name:stream',
-    dest='buildrequires', default=[],
+@cli.command("build_module_locally")
+@click.option("--stream", metavar="STREAM")
+@click.option(
+    "--file", "yaml_file",
+    metavar="FILE",
+    required=True,
+    type=click.Path(exists=True),
+)
+@click.option("--srpm", "srpms", metavar="SRPM", multiple=True)
+@click.option("--skiptests", is_flag=True)
+@click.option("--offline", is_flag=True)
+@click.option(
+    '--buildrequires', "buildrequires", multiple=True,
+    metavar='name:stream', default=[],
     help='Buildrequires to override in the form of "name:stream"'
 )
-@manager.option(
-    '--requires', action='append', metavar='name:stream',
-    dest='requires', default=[],
+@click.option(
+    '--requires', "requires", multiple=True,
+    metavar='name:stream', default=[],
     help='Requires to override in the form of "name:stream"'
 )
-@manager.option("-d", "--debug", action="store_true", dest="log_debug")
-@manager.option("-l", "--add-local-build", action="append", default=None, dest="local_build_nsvs")
-@manager.option("-s", "--set-stream", action="append", default=[], dest="default_streams")
-@manager.option(
-    "-r", "--platform-repo-file", action="append", default=[], dest="platform_repofiles"
+@click.option("-d", "--debug", "log_debug", is_flag=True)
+@click.option(
+    "-l", "--add-local-build", "local_build_nsvs",
+    metavar="NSV", multiple=True
+)
+@click.option(
+    "-s", "--set-stream", "default_streams",
+    metavar="STREAM", multiple=True
+)
+@click.option(
+    "-r", "--platform-repo-file", "platform_repofiles",
+    metavar="FILE",
+    type=click.Path(exists=True),
+    multiple=True
 )
-@manager.option("-p", "--platform-id", action="store", default=None, dest="platform_id")
+@click.option("-p", "--platform-id", metavar="PLATFORM_ID")
 def build_module_locally(
-    local_build_nsvs=None,
+    stream=None,
     yaml_file=None,
     srpms=None,
-    stream=None,
     skiptests=False,
-    default_streams=None,
     offline=False,
+    log_debug=False,
+    local_build_nsvs=None,
+    default_streams=None,
     platform_repofiles=None,
     platform_id=None,
     requires=None,
     buildrequires=None,
-    log_debug=False,
 ):
     """ Performs local module build using Mock
     """
+    # accumulate initial log messages in memory - we'll output them to a log in the
+    # module build directories when we know what they are
+    build_logs.buffer_initially()
+
     # if debug is not specified, set log level of console to INFO
-    if not log_debug:
+    if log_debug:
         for handler in logging.getLogger().handlers:
-            if isinstance(handler, logging.StreamHandler):
-                handler.setLevel(logging.INFO)
+            handler.setLevel(logging.DEBUG)
 
     if "SERVER_NAME" not in app.config or not app.config["SERVER_NAME"]:
         app.config["SERVER_NAME"] = "localhost"
 
         if conf.resolver == "db":
             raise ValueError(
                 "Please set RESOLVER to 'mbs' in your configuration for local builds.")
@@ -229,22 +207,19 @@
     try:
         module_build_service.scheduler.local.main(module_build_ids)
     except module_build_service.scheduler.local.BuildFailed as e:
         logging.error("%s", e)
         sys.exit(1)
 
 
-@manager.option(
-    "identifier",
-    metavar="NAME:STREAM[:VERSION[:CONTEXT]]",
-    help="Identifier for selecting module builds to retire",
-)
-@manager.option(
+@cli.command("retire")
+@click.argument("identifier", metavar="NAME:STREAM[:VERSION[:CONTEXT]]")
+@click.option(
     "--confirm",
-    action="store_true",
+    is_flag=True,
     default=False,
     help="Perform retire operation without prompting",
 )
 def retire(identifier, confirm=False):
     """ Retire module build(s) by placing them into 'garbage' state.
     """
     # Parse identifier and build query
@@ -269,42 +244,41 @@
         return
 
     logging.info("Found %d module builds:", len(module_builds))
     for build in module_builds:
         logging.info("\t%s", ":".join((build.name, build.stream, build.version, build.context)))
 
     # Prompt for confirmation
-    is_confirmed = confirm or prompt_bool("Retire {} module builds?".format(len(module_builds)))
+    confirm_msg = "Retire {} module builds?".format(len(module_builds))
+    is_confirmed = confirm or click.confirm(confirm_msg, abort=False)
     if not is_confirmed:
         logging.info("Module builds were NOT retired.")
         return
 
     # Retire module builds
     for build in module_builds:
         build.transition(
             db_session, conf, models.BUILD_STATES["garbage"], "Module build retired")
 
     db_session.commit()
 
     logging.info("Module builds retired.")
 
 
-@console_script_help
-@manager.command
+@cli.command("run")
+@click.option("-h", "--host", metavar="HOST", help="Bind to this host.")
+@click.option("-p", "--port", metavar="PORT", help="Bind to this port along with --host.")
+@click.option("-d", "--debug", is_flag=True, default=False, help="Run frontend in debug mode.")
 def run(host=None, port=None, debug=None):
     """ Runs the Flask app, locally. Intended for dev instances, should not be used for production.
     """
     host = host or conf.host
     port = port or conf.port
     debug = debug or conf.debug
 
     logging.info("Starting Module Build Service frontend")
 
     app.run(host=host, port=port, debug=debug)
 
 
-def manager_wrapper():
-    manager.run()
-
-
 if __name__ == "__main__":
-    manager_wrapper()
+    cli()
```

### Comparing `module-build-service-3.8.0/module_build_service/migrations/alembic.ini` & `module-build-service-3.9.0/module_build_service/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/resolver/DBResolver.py` & `module-build-service-3.9.0/module_build_service/resolver/DBResolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/resolver/KojiResolver.py` & `module-build-service-3.9.0/module_build_service/resolver/KojiResolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/resolver/LocalResolver.py` & `module-build-service-3.9.0/module_build_service/resolver/LocalResolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/resolver/MBSResolver.py` & `module-build-service-3.9.0/module_build_service/resolver/MBSResolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 """MBS handler functions."""
 
 from __future__ import absolute_import
-import logging
 
 import dogpile.cache
 
-from module_build_service.common import models
+from module_build_service.common import log, models
 from module_build_service.common.config import conf
 from module_build_service.common.errors import StreamNotXyz, UnprocessableEntity
 from module_build_service.common.request_utils import requests_session
 from module_build_service.common.utils import load_mmd, import_mmd
 from module_build_service.resolver.KojiResolver import KojiResolver
 
-log = logging.getLogger()
-
 
 def _canonicalize_state(state):
     if isinstance(state, int):
         return models.INVERSE_BUILD_STATES[state]
     else:
         return state
 
@@ -437,14 +434,16 @@
         else:
             version = str(version)
             log.debug(
                 "get_module_build_dependencies(%s, strict=%r)"
                 % (", ".join([name, stream, str(version), context]), strict)
             )
 
+        log.long_running_start("Loading build dependencies")
+
         # This is the set we're going to build up and return.
         module_tags = {}
 
         if mmd:
             queried_mmd = mmd
         else:
             queried_module = self.get_module(name, stream, version, context, strict=strict)
@@ -481,14 +480,16 @@
             # If the buildrequire is a meta-data only module with no Koji tag set, then just
             # skip it
             if m["koji_tag"] is None:
                 continue
             module_tags.setdefault(m["koji_tag"], [])
             module_tags[m["koji_tag"]].append(load_mmd(m["modulemd"]))
 
+        log.long_running_end("Loading build dependencies")
+
         return module_tags
 
     def resolve_requires(self, requires):
         """
         Resolves the requires list of N:S or N:S:V:C to a dictionary with keys as
         the module name and the values as a dictionary with keys of ref,
         stream, version.
```

### Comparing `module-build-service-3.8.0/module_build_service/resolver/__init__.py` & `module-build-service-3.9.0/module_build_service/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/resolver/base.py` & `module-build-service-3.9.0/module_build_service/resolver/base.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/__init__.py` & `module-build-service-3.9.0/module_build_service/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/batches.py` & `module-build-service-3.9.0/module_build_service/scheduler/batches.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,17 @@
         log.info(
             "Not starting new batch, not all of %r are in the buildroot. Waiting." % artifacts)
         return []
 
     # This is used to determine if it's worth checking if a component can be
     # reused later on in the code
     all_reused_in_prev_batch = all(
-        c.reused_component_id is not None for c in module.component_builds)
+        c.reused_component_id is not None for c in module.component_builds
+        if c.batch == module.batch
+    )
 
     # Although this variable isn't necessary, it is easier to read code later on with it
     prev_batch = module.batch
     module.batch += 1
 
     # The user can either pass in a list of components to 'seed' the batch, or
     # if none are provided then we just select everything that hasn't
@@ -249,15 +251,17 @@
 
     # If there are no components to build, skip the batch and start building
     # the new one. This can happen when resubmitting the failed module build.
     if not unbuilt_components and not components:
         log.info("Skipping build of batch %d, no component to build.", module.batch)
         return start_next_batch_build(config, module, builder)
 
-    log.info("Starting build of next batch %d, %s" % (module.batch, unbuilt_components))
+    log.console("Starting build of next batch %d: %s",
+                module.batch,
+                ', '.join(c.package for c in unbuilt_components))
 
     # Attempt to reuse any components possible in the batch before attempting to build any
     unbuilt_components_after_reuse = []
     components_reused = False
     should_try_reuse = True
     # If the rebuild strategy is "changed-and-after", try to figure out if it's worth checking if
     # the components can be reused to save on resources
```

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/consumer.py` & `module-build-service-3.9.0/module_build_service/scheduler/consumer.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/db_session.py` & `module-build-service-3.9.0/module_build_service/scheduler/db_session.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/default_modules.py` & `module-build-service-3.9.0/module_build_service/scheduler/default_modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -239,14 +239,16 @@
             "The necessary conflicts could not be generated due to RHBZ#1693683. "
             "Some RPMs from the base modules (%s) may end up being used over modular RPMs. "
             "This may result in different behavior than a production build.",
             ", ".join(conf.base_module_names)
         )
         return
 
+    log.long_running_start("Finding RPMs to exclude from the base modules")
+
     log.info("Finding any buildrequired modules that collide with the RPMs in the base modules")
     bm_tags = set()
     non_bm_tags = set()
     xmd = mmd.get_xmd()
     buildrequires = xmd["mbs"]["buildrequires"]
     for name, info in buildrequires.items():
         if not info["koji_tag"]:
@@ -296,14 +298,16 @@
                 conflicts = conflicts | nevras
 
     # Add the conflicting NEVRAs to `ursine_rpms` so the Conflicts are later generated for them
     # in the KojiModuleBuilder.
     xmd["mbs"]["ursine_rpms"] = list(conflicts)
     mmd.set_xmd(xmd)
 
+    log.long_running_end("Finding RPMs to exclude from the base modules")
+
 
 def _get_rpms_from_tags(koji_session, tags, arches):
     """
     Get the RPMs in NEVRA form (tagged or external repos) of the input tags.
 
     :param koji.ClientSession koji_session: the Koji session to use to query
     :param list tags: the list of tags to get the RPMs from
```

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/events.py` & `module-build-service-3.9.0/module_build_service/scheduler/events.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/handlers/components.py` & `module-build-service-3.9.0/module_build_service/scheduler/handlers/components.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/handlers/modules.py` & `module-build-service-3.9.0/module_build_service/scheduler/handlers/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,16 @@
             return
 
     # Scratch builds stay in 'done' state
     if not build.scratch:
         build.transition(db_session, conf, state=models.BUILD_STATES["ready"])
         db_session.commit()
 
+    log.console("Finished building %s", build.nsvc)
+
     build_logs.stop(build)
     GenericBuilder.clear_cache(build)
 
 
 @celery_app.task
 @events.mbs_event_handler
 def init(msg_id, module_build_id, module_build_state):
@@ -177,15 +179,16 @@
         build_tag_name = generate_module_build_koji_tag(build)
         mock_resultsdir = os.path.join(conf.mock_resultsdir, build_tag_name)
         if not os.path.exists(mock_resultsdir):
             os.makedirs(mock_resultsdir)
         build_logs.build_logs_dir = mock_resultsdir
 
     build_logs.start(db_session, build)
-    log.info("Start to handle %s which is in init state.", build.mmd().get_nsvc())
+    log.console("Starting to build %s", build.nsvc)
+    log.console("Logging to %s", build_logs.path(db_session, build))
 
     error_msg = ""
     failure_reason = "unspec"
     try:
         mmd = build.mmd()
         record_module_build_arches(mmd, build)
         arches = [arch.name for arch in build.arches]
@@ -409,34 +412,36 @@
             db_session, conf,
             state=models.BUILD_STATES["failed"],
             state_reason=reason, failure_type="infra")
         db_session.commit()
         raise
 
     if not build.component_builds:
-        log.info("There are no components in module %r, skipping build" % build)
+        log.console("There are no components in module %s, skipping build",
+                    build.nsvc)
         build.transition(db_session, conf, state=models.BUILD_STATES["build"])
         db_session.add(build)
         db_session.commit()
         # Return a KojiRepoChange message so that the build can be transitioned to done
         # in the repos handler
         from module_build_service.scheduler.handlers.repos import done as repos_done_handler
         events.scheduler.add(repos_done_handler, ("fake_msg", builder.module_build_tag["name"]))
         return
 
     # If all components in module build will be reused, we don't have to build
     # module-build-macros, because there won't be any build done.
     if attempt_to_reuse_all_components(builder, build):
-        log.info("All components have been reused for module %r, skipping build" % build)
+        log.console("All components have been reused for module %s, skipping build",
+                    build.nsvc)
         build.transition(db_session, conf, state=models.BUILD_STATES["build"])
         db_session.add(build)
         db_session.commit()
         return []
 
-    log.debug("Starting build batch 1")
+    log.console("Starting build of batch 1: module-build-macros")
     build.batch = 1
     db_session.commit()
 
     artifact_name = "module-build-macros"
 
     component_build = models.ComponentBuild.from_component_name(db_session, artifact_name, build.id)
     srpm = builder.get_disttag_srpm(
```

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/handlers/repos.py` & `module-build-service-3.9.0/module_build_service/scheduler/handlers/repos.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/handlers/tags.py` & `module-build-service-3.9.0/module_build_service/scheduler/handlers/tags.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/local.py` & `module-build-service-3.9.0/module_build_service/scheduler/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """
     builds = db_session.query(models.ModuleBuild).filter(
         models.ModuleBuild.id.in_(module_build_ids)).all()
     has_failed_build = False
     for build in builds:
         if build.state == models.BUILD_STATES["failed"]:
             with set_current_module_build_id(build.id):
-                modules_failed_handler("fake_msg_id", build.id, "failed")
+                modules_failed_handler("fake_msg_id", build.id, models.BUILD_STATES["failed"])
             has_failed_build = True
     if has_failed_build:
         raise BuildFailed("Local module build failed.")
 
 
 def main(module_build_ids):
     """
```

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/parser.py` & `module-build-service-3.9.0/module_build_service/scheduler/parser.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/producer.py` & `module-build-service-3.9.0/module_build_service/scheduler/producer.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/reuse.py` & `module-build-service-3.9.0/module_build_service/scheduler/reuse.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/route.py` & `module-build-service-3.9.0/module_build_service/scheduler/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     num_workers = conf.num_workers
 
     module, handler_name = name.rsplit(".", 1)
     handler = getattr(__import__(module, fromlist=[handler_name]), handler_name)
     # handlers can be decorated, inspect the original function
     while getattr(handler, "__wrapped__", None):
         handler = handler.__wrapped__
-    handler_args = inspect.getargspec(handler).args
+    handler_args = inspect.getfullargspec(handler).args
 
     def _get_handler_arg(name):
         index = handler_args.index(name)
         arg_value = kwargs.get(name, None)
         if arg_value is None and len(args) > index:
             arg_value = args[index]
         return arg_value
```

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/submit.py` & `module-build-service-3.9.0/module_build_service/scheduler/submit.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
         req_mmd = resolver.get_module_modulemds(
             req_name, req_data["stream"], req_data["version"], req_data["context"], True)[0]
 
         # Find out the particular NVR of filtered packages
         filtered_rpms = []
         rpm_filter = req_mmd.get_rpm_filters()
         if rpm_filter:
-            built_nvrs = builder.get_built_rpms_in_module_build(req_mmd)
+            built_nvrs = builder.get_built_rpms_in_module_build(req_mmd, req_data["koji_tag"])
             for nvr in built_nvrs:
                 parsed_nvr = kobo.rpmlib.parse_nvr(nvr)
                 if parsed_nvr["name"] in rpm_filter:
                     filtered_rpms.append(nvr)
         req_data["filtered_rpms"] = filtered_rpms
 
         new_buildrequires[req_name] = req_data
```

### Comparing `module-build-service-3.8.0/module_build_service/scheduler/ursine.py` & `module-build-service-3.9.0/module_build_service/scheduler/ursine.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/web/auth.py` & `module-build-service-3.9.0/module_build_service/web/auth.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/web/backports.py` & `module-build-service-3.9.0/module_build_service/web/backports.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/web/mmd_resolver.py` & `module-build-service-3.9.0/module_build_service/web/mmd_resolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/web/mse.py` & `module-build-service-3.9.0/module_build_service/web/mse.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,14 +251,16 @@
     :param bool static_context: When True will use a predefined context from the mmd yaml file
         and will not generate a new one. Also it will set `static_context` property in the `mbs`
         property to True.
     """
     if not default_streams:
         default_streams = {}
 
+    log.long_running_start("Expanding module streams to determine build requirements")
+
     # Create local copy of mmd, because we will expand its dependencies,
     # which would change the module.
     current_mmd = mmd.copy()
 
     # if a static context is set the generated context will be overridden by the one
     # defined in the mmd of the module.
     if static_context:
@@ -280,15 +282,15 @@
     # Show log.info message with the NSVCs we have added to mmd_resolver.
     nsvcs_to_solve = [m.get_nsvc() for m in mmds_for_resolving]
     log.info("Starting resolving with following input modules: %r", nsvcs_to_solve)
 
     # Resolve the dependencies between modules and get the list of all valid
     # combinations in which we can build this module.
     requires_combinations = mmd_resolver.solve(current_mmd)
-    log.info("Resolving done, possible requires: %r", requires_combinations)
+    log.long_running_end("Expanding module streams to determine build requirements")
 
     # This is where we are going to store the generated MMDs.
     mmds = []
     for requires in requires_combinations:
         # Each generated MMD must be new Module object...
         mmd_copy = mmd.copy()
         xmd = mmd_copy.get_xmd()
@@ -379,14 +381,17 @@
         for nsvca in requires:
             if nsvca == self_nsvca:
                 continue
             # Remove the arch from nsvca
             nsvc = ":".join(nsvca.split(":")[:-1])
             br_list.append(nsvc)
 
+        log.console("Build requirements #%s:\n  %s",
+                    len(mmds) + 1, ", ".join(br_list))
+
         # Resolve the buildrequires and store the result in XMD.
         if "mbs" not in xmd:
             xmd["mbs"] = {}
         resolver = GenericResolver.create(db_session, conf)
         xmd["mbs"]["buildrequires"] = resolver.resolve_requires(br_list)
 
         xmd["mbs"]["mse"] = True
```

### Comparing `module-build-service-3.8.0/module_build_service/web/proxy.py` & `module-build-service-3.9.0/module_build_service/web/proxy.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/web/submit.py` & `module-build-service-3.9.0/module_build_service/web/submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/web/utils.py` & `module-build-service-3.9.0/module_build_service/web/utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service/web/views.py` & `module-build-service-3.9.0/module_build_service/web/views.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/module_build_service.egg-info/SOURCES.txt` & `module-build-service-3.9.0/module_build_service.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
+run-unittests.sh
 setup.py
 test-requirements.txt
+tox.ini
 client/mbs-cli
+conf/client_secrets.json
 conf/koji.conf
 conf/mock.cfg
 conf/yum.conf
 docs/CHANGELOG.rst
 docs/CONTRIBUTING.rst
 docs/DEPENDENCY_RESOLUTION.rst
 docs/GATING.rst
@@ -51,47 +54,15 @@
 module_build_service/common/resolve.py
 module_build_service/common/retry.py
 module_build_service/common/scm.py
 module_build_service/common/submit.py
 module_build_service/common/utils.py
 module_build_service/migrations/README
 module_build_service/migrations/alembic.ini
-module_build_service/migrations/env.py
 module_build_service/migrations/script.py.mako
-module_build_service/migrations/versions/0b00036c540f_add_log_messages_table.py
-module_build_service/migrations/versions/0ef60c3ed440_insert_fake_base_runtime.py
-module_build_service/migrations/versions/145347916a56_.py
-module_build_service/migrations/versions/1817e62719f9_remove_ref_build_context.py
-module_build_service/migrations/versions/1a44272e8b4c_.py
-module_build_service/migrations/versions/229f6f273a56_state_reason.py
-module_build_service/migrations/versions/335455a30585_state_reason_history.py
-module_build_service/migrations/versions/3b17cd6dc583_.py
-module_build_service/migrations/versions/40b2c7d988d7_add_reused_module_id_column.py
-module_build_service/migrations/versions/440a8a3c0d96_add_indexes_to_models.py
-module_build_service/migrations/versions/474697622859_add_optional_columns_for_copr.py
-module_build_service/migrations/versions/4d1e2e13e514_buildonly.py
-module_build_service/migrations/versions/524c3b1c683c_rebuild_strategy.py
-module_build_service/migrations/versions/526fb7d445f7_module_buildrequires.py
-module_build_service/migrations/versions/60c6093dde9e_.py
-module_build_service/migrations/versions/65ad4fcdbce6_add_missing_uniqueness_constraint.py
-module_build_service/migrations/versions/6d503efcd2b8_virtual_streams_table.py
-module_build_service/migrations/versions/708ac8950f55_set_from_mmd_context.py
-module_build_service/migrations/versions/79babdadc942_convert_type_of_modulebuild_stream_.py
-module_build_service/migrations/versions/9ca1c166f426_contexts.py
-module_build_service/migrations/versions/9d5e6938588f_.py
-module_build_service/migrations/versions/a1fc0736bca8_.py
-module_build_service/migrations/versions/a7a553e5ca1d_.py
-module_build_service/migrations/versions/a87264eeb49f_.py
-module_build_service/migrations/versions/bf861b6af29a_.py
-module_build_service/migrations/versions/c11a3cfec2a9_.py
-module_build_service/migrations/versions/c8e2fc555399_add_modulebuild_context.py
-module_build_service/migrations/versions/caeae7a4f537_ref_build_context.py
-module_build_service/migrations/versions/d5188b4a7bf1_add_fk_reused_module_id.py
-module_build_service/migrations/versions/edb537dd1e8c_.py
-module_build_service/migrations/versions/f5b1c5203cce_.py
 module_build_service/resolver/DBResolver.py
 module_build_service/resolver/KojiResolver.py
 module_build_service/resolver/LocalResolver.py
 module_build_service/resolver/MBSResolver.py
 module_build_service/resolver/__init__.py
 module_build_service/resolver/base.py
 module_build_service/scheduler/__init__.py
@@ -120,15 +91,43 @@
 module_build_service/web/proxy.py
 module_build_service/web/submit.py
 module_build_service/web/utils.py
 module_build_service/web/views.py
 tests/__init__.py
 tests/conftest.py
 tests/test_manage.py
+tests/integration/README.rst
+tests/integration/__init__.py
+tests/integration/conftest.py
 tests/integration/example.test.env.yaml
+tests/integration/test_build_stream_collision.py
+tests/integration/test_buildonly.py
+tests/integration/test_buildrequire_invalid_module.py
+tests/integration/test_failed_build.py
+tests/integration/test_highest_version_selection.py
+tests/integration/test_import_module.py
+tests/integration/test_no_components.py
+tests/integration/test_normal_build.py
+tests/integration/test_normal_build_conflict.py
+tests/integration/test_rest_build_state.py
+tests/integration/test_rest_submit_build.py
+tests/integration/test_resume_cancelled_build.py
+tests/integration/test_reuse_all_components.py
+tests/integration/test_reuse_components.py
+tests/integration/test_reuse_components_if_added.py
+tests/integration/test_reuse_tagged_module.py
+tests/integration/test_scratch_build.py
+tests/integration/test_scratch_final_mmd.py
+tests/integration/test_static_context.py
+tests/integration/test_stream_expansion.py
+tests/integration/test_v3_buildrequire.py
+tests/integration/test_v3_multiple_contexts.py
+tests/integration/test_v3_no_components.py
+tests/integration/test_v3_normal_build.py
+tests/integration/utils.py
 tests/scm_data/mariadb/HEAD
 tests/scm_data/mariadb/config
 tests/scm_data/mariadb/description
 tests/scm_data/mariadb/packed-refs
 tests/scm_data/mariadb/info/exclude
 tests/scm_data/mariadb/info/refs
 tests/scm_data/mariadb/objects/34/a463979786199c1b41ca21eb309cf3ce5ce789
@@ -203,17 +202,23 @@
 tests/staged_data/local_builds/module-platform-f30-3/results/modules.yaml
 tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/modules.yaml
 tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/modules.yaml
 tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/modules.yaml
 tests/staged_data/v3/mmd_packager.yaml
 tests/test_build/__init__.py
 tests/test_build/test_build.py
+tests/test_builder/__init__.py
+tests/test_builder/test_base.py
+tests/test_builder/test_builder_utils.py
+tests/test_builder/test_content_generator.py
 tests/test_builder/test_get_generator_json_expected_output.json
 tests/test_builder/test_get_generator_json_expected_output_with_log.json
 tests/test_builder/test_get_generator_json_rpms_in_tag.json
+tests/test_builder/test_koji.py
+tests/test_builder/test_mock.py
 tests/test_common/__init__.py
 tests/test_common/test_config.py
 tests/test_common/test_koji.py
 tests/test_common/test_logger.py
 tests/test_common/test_messaging.py
 tests/test_common/test_monitor.py
 tests/test_common/test_resolve.py
```

### Comparing `module-build-service-3.8.0/module_build_service.egg-info/entry_points.txt` & `module-build-service-3.9.0/module_build_service.egg-info/entry_points.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [console_scripts]
 mbs-frontend = module_build_service.manage:run
-mbs-manager = module_build_service.manage:manager_wrapper
-mbs-upgradedb = module_build_service.manage:upgradedb
+mbs-manager = module_build_service.manage:cli
+mbs-upgradedb = module_build_service.manage:upgradedb_entrypoint
 
 [mbs.builder_backends]
 koji = module_build_service.builder.KojiModuleBuilder:KojiModuleBuilder
 mock = module_build_service.builder.MockModuleBuilder:MockModuleBuilder
 
 [mbs.messaging_backends]
 drop = module_build_service.common.messaging:_drop_backend
@@ -16,8 +16,7 @@
 db = module_build_service.resolver.DBResolver:DBResolver
 koji = module_build_service.resolver.KojiResolver:KojiResolver
 local = module_build_service.resolver.LocalResolver:LocalResolver
 mbs = module_build_service.resolver.MBSResolver:MBSResolver
 
 [moksha.consumer]
 mbsconsumer = module_build_service.scheduler.consumer:MBSConsumer
-
```

### Comparing `module-build-service-3.8.0/setup.py` & `module-build-service-3.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,32 +20,32 @@
 setup_py_path = path.dirname(path.realpath(__file__))
 install_requires, deps_links = read_requirements(path.join(setup_py_path, "requirements.txt"))
 tests_require, _ = read_requirements(path.join(setup_py_path, "test-requirements.txt"))
 
 setup(
     name="module-build-service",
     description="The Module Build Service for Modularity",
-    version="3.8.0",
+    version="3.9.0",
     classifiers=["Programming Language :: Python", "Topic :: Software Development :: Build Tools"],
     keywords="module build service fedora modularity koji mock rpm",
     author="The Factory 2.0 Team",
     author_email="module-build-service-owner@fedoraproject.org",
     url="https://pagure.io/fm-orchestrator/",
     license="MIT",
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     install_requires=install_requires,
     tests_require=tests_require,
     dependency_links=deps_links,
     entry_points={
         "console_scripts": [
-            "mbs-upgradedb = module_build_service.manage:upgradedb",
+            "mbs-upgradedb = module_build_service.manage:upgradedb_entrypoint",
             "mbs-frontend = module_build_service.manage:run",
-            "mbs-manager = module_build_service.manage:manager_wrapper",
+            "mbs-manager = module_build_service.manage:cli",
         ],
         "moksha.consumer": "mbsconsumer = module_build_service.scheduler.consumer:MBSConsumer",
         "mbs.messaging_backends": [
             "fedmsg = module_build_service.common.messaging:_fedmsg_backend",
             "in_memory = module_build_service.common.messaging:_in_memory_backend",
             "drop = module_build_service.common.messaging:_drop_backend",
             # 'custom = your_organization:_custom_backend',
```

### Comparing `module-build-service-3.8.0/tests/__init__.py` & `module-build-service-3.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/conftest.py` & `module-build-service-3.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/integration/example.test.env.yaml` & `module-build-service-3.9.0/tests/integration/example.test.env.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/scm_data/mariadb/objects/6c/d6a18e15a4f23a1eaa7040e7f4da9be1aed36d` & `module-build-service-3.9.0/tests/scm_data/mariadb/objects/6c/d6a18e15a4f23a1eaa7040e7f4da9be1aed36d`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/scm_data/mariadb/objects/6e/a27c8576449ad5a12c1b6d27b50ff32c854ee5` & `module-build-service-3.9.0/tests/scm_data/mariadb/objects/6e/a27c8576449ad5a12c1b6d27b50ff32c854ee5`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/scm_data/mariadb/objects/fb/9351bd6f2439a73d78de0822fefe64410f905c` & `module-build-service-3.9.0/tests/scm_data/mariadb/objects/fb/9351bd6f2439a73d78de0822fefe64410f905c`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.idx` & `module-build-service-3.9.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.idx`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.pack` & `module-build-service-3.9.0/tests/scm_data/mariadb/objects/pack/pack-92fbbdbf4fa07dc9cab035120eb248da930e0bd6.pack`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/bad.yaml` & `module-build-service-3.9.0/tests/staged_data/bad.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/build_metadata_module.yaml` & `module-build-service-3.9.0/tests/staged_data/build_metadata_module.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/formatted_python3-no-components.yaml` & `module-build-service-3.9.0/tests/staged_data/formatted_python3-no-components.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/formatted_testmodule-more-components.yaml` & `module-build-service-3.9.0/tests/staged_data/formatted_testmodule-more-components.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/formatted_testmodule.yaml` & `module-build-service-3.9.0/tests/staged_data/formatted_testmodule.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/includedmodules.yaml` & `module-build-service-3.9.0/tests/staged_data/includedmodules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/local_builds/module-child-master-20170816080815/results/modules.yaml` & `module-build-service-3.9.0/tests/staged_data/local_builds/module-child-master-20170816080815/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/local_builds/module-parent-master-20170816080815/results/modules.yaml` & `module-build-service-3.9.0/tests/staged_data/local_builds/module-parent-master-20170816080815/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/local_builds/module-platform-f28-3/results/modules.yaml` & `module-build-service-3.9.0/tests/staged_data/local_builds/module-platform-f28-3/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/modules.yaml` & `module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080815/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/modules.yaml` & `module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule-master-20170816080816/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/modules.yaml` & `module-build-service-3.9.0/tests/staged_data/local_builds/module-testmodule2-master-20170816093656/results/modules.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/nginx_mmd.yaml` & `module-build-service-3.9.0/tests/staged_data/nginx_mmd.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/platform.yaml` & `module-build-service-3.9.0/tests/staged_data/platform.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/python3-no-components.yaml` & `module-build-service-3.9.0/tests/staged_data/python3-no-components.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/shared-userspace-570.yaml` & `module-build-service-3.9.0/tests/staged_data/shared-userspace-570.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/shared-userspace-577.yaml` & `module-build-service-3.9.0/tests/staged_data/shared-userspace-577.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/static_context_v2.yaml` & `module-build-service-3.9.0/tests/staged_data/static_context_v2.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule-buildrequires-f30.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule-buildrequires-f30.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule-dashed-stream.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule-dashed-stream.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule-forbidden-xmd.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule-forbidden-xmd.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule-local-build.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule-local-build.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule-more-components.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule-more-components.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule-no-base-module.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule-no-base-module.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule-no-deps.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule-no-deps.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule-version-set.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule-version-set.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule-with-filters.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule-with-filters.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule-wrong-stream.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule-wrong-stream.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule_br_metadata_module.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule_br_metadata_module.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule_dependencies.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule_dependencies.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule_el8.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule_el8.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule_el800.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule_el800.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule_el821.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule_el821.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule_init.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule_v2_buildonly.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 document: modulemd
-version: 1
+version: 2
 data:
-    summary: A test module in all its beautiful beauty
-    description: >-
-        This module demonstrates how to write simple modulemd files And
-        can be used for testing the build and release pipeline. ’
-    license:
-        module: [ MIT ]
-    dependencies:
-        buildrequires:
-            platform: f28
-        requires:
-            platform: f28
-    references:
-        community: https://docs.pagure.org/modularity/
-        documentation: https://fedoraproject.org/wiki/Fedora_Packaging_Guidelines_for_Modules
-    profiles:
-        default:
-            rpms:
-            - tangerine
-    xmd:
-        mbs:
-            buildrequires:
-               platform:
-                   ref: virtual
-                   stream: f28
-                   version: '3'
-                   context: '00000000'
-    api:
-        rpms:
-        - perl-Tangerine
-        - tangerine
-    components:
-        rpms:
-            perl-List-Compare:
-                rationale: A dependency of tangerine.
-                ref: master
-            perl-Tangerine:
-                rationale: Provides API for this module and is a dependency of tangerine.
-                ref: master
-            tangerine:
-                rationale: Provides API for this module.
-                buildorder: 10
-                ref: master
+  summary: A test module in all its beautiful beauty
+  description: >-
+    This module demonstrates how to write simple modulemd files And can be used for
+    testing the build and release pipeline. ’
+  license:
+    module:
+    - MIT
+  dependencies:
+  - buildrequires:
+      platform: [f28]
+    requires:
+      platform: [f28]
+  references:
+    community: https://docs.pagure.org/modularity/
+    documentation: https://fedoraproject.org/wiki/Fedora_Packaging_Guidelines_for_Modules
+  profiles:
+    default:
+      rpms:
+      - tangerine
+  api:
+    rpms:
+    - perl-Tangerine
+    - tangerine
+  components:
+    rpms:
+      perl-List-Compare:
+        rationale: A dependency of tangerine.
+        ref: master
+        buildonly: true
+      perl-Tangerine:
+        rationale: Provides API for this module and is a dependency of tangerine.
+        ref: master
+      tangerine:
+        rationale: Provides API for this module.
+        ref: master
+        buildorder: 10
```

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule_mse.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule_mse.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule_platform_f290000.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule_platform_f290000.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule_v2.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule_v2.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/staged_data/testmodule_v2_buildonly.yaml` & `module-build-service-3.9.0/tests/test_common/test_models/data/testmodule.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 document: modulemd
-version: 2
+version: 1
 data:
-  summary: A test module in all its beautiful beauty
-  description: >-
-    This module demonstrates how to write simple modulemd files And can be used for
-    testing the build and release pipeline. ’
-  license:
-    module:
-    - MIT
-  dependencies:
-  - buildrequires:
-      platform: [f28]
-    requires:
-      platform: [f28]
-  references:
-    community: https://docs.pagure.org/modularity/
-    documentation: https://fedoraproject.org/wiki/Fedora_Packaging_Guidelines_for_Modules
-  profiles:
-    default:
-      rpms:
-      - tangerine
-  api:
-    rpms:
-    - perl-Tangerine
-    - tangerine
-  components:
-    rpms:
-      perl-List-Compare:
-        rationale: A dependency of tangerine.
-        ref: master
-        buildonly: true
-      perl-Tangerine:
-        rationale: Provides API for this module and is a dependency of tangerine.
-        ref: master
-      tangerine:
-        rationale: Provides API for this module.
-        ref: master
-        buildorder: 10
+    name: testmodule
+    stream: master
+    version: 1
+    summary: A test module in all its beautiful beauty
+    description: This module demonstrates how to write simple modulemd files And can be used for testing the build and release pipeline.
+    license:
+        module: [ MIT ]
+    dependencies:
+        buildrequires:
+            base-runtime: master
+        requires:
+            base-runtime: master
+    references:
+        community: https://fedoraproject.org/wiki/Modularity
+        documentation: https://fedoraproject.org/wiki/Fedora_Packaging_Guidelines_for_Modules
+        tracker: https://taiga.fedorainfracloud.org/project/modularity
+    profiles:
+        default:
+            rpms:
+                - tangerine
+    api:
+        rpms:
+            - perl-Tangerine
+            - tangerine
+    components:
+        rpms:
+            perl-List-Compare:
+                rationale: A dependency of tangerine.
+                ref: f25
+            perl-Tangerine:
+                rationale: Provides API for this module and is a dependency of tangerine.
+                ref: f25
+            tangerine:
+                rationale: Provides API for this module.
+                buildorder: 10
+                ref: f25
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `module-build-service-3.8.0/tests/staged_data/v3/mmd_packager.yaml` & `module-build-service-3.9.0/tests/staged_data/v3/mmd_packager.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_build/test_build.py` & `module-build-service-3.9.0/tests/test_build/test_build.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_builder/test_get_generator_json_expected_output.json` & `module-build-service-3.9.0/tests/test_builder/test_get_generator_json_expected_output.json`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_builder/test_get_generator_json_expected_output_with_log.json` & `module-build-service-3.9.0/tests/test_builder/test_get_generator_json_expected_output_with_log.json`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_builder/test_get_generator_json_rpms_in_tag.json` & `module-build-service-3.9.0/tests/test_builder/test_get_generator_json_rpms_in_tag.json`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_common/test_messaging.py` & `module-build-service-3.9.0/tests/test_common/test_messaging.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_common/test_models/data/base-runtime.yaml` & `module-build-service-3.9.0/tests/test_common/test_models/data/base-runtime.yaml`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_common/test_models/data/testmodule.yaml` & `module-build-service-3.9.0/tests/staged_data/testmodule_init.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 document: modulemd
 version: 1
 data:
-    name: testmodule
-    stream: master
-    version: 1
     summary: A test module in all its beautiful beauty
-    description: This module demonstrates how to write simple modulemd files And can be used for testing the build and release pipeline.
+    description: >-
+        This module demonstrates how to write simple modulemd files And
+        can be used for testing the build and release pipeline. ’
     license:
         module: [ MIT ]
     dependencies:
         buildrequires:
-            base-runtime: master
+            platform: f28
         requires:
-            base-runtime: master
+            platform: f28
     references:
-        community: https://fedoraproject.org/wiki/Modularity
+        community: https://docs.pagure.org/modularity/
         documentation: https://fedoraproject.org/wiki/Fedora_Packaging_Guidelines_for_Modules
-        tracker: https://taiga.fedorainfracloud.org/project/modularity
     profiles:
         default:
             rpms:
-                - tangerine
+            - tangerine
+    xmd:
+        mbs:
+            buildrequires:
+               platform:
+                   ref: virtual
+                   stream: f28
+                   version: '3'
+                   context: '00000000'
+                   koji_tag: module-f28-build
     api:
         rpms:
-            - perl-Tangerine
-            - tangerine
+        - perl-Tangerine
+        - tangerine
     components:
         rpms:
             perl-List-Compare:
                 rationale: A dependency of tangerine.
-                ref: f25
+                ref: master
             perl-Tangerine:
                 rationale: Provides API for this module and is a dependency of tangerine.
-                ref: f25
+                ref: master
             tangerine:
                 rationale: Provides API for this module.
                 buildorder: 10
-                ref: f25
+                ref: master
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `module-build-service-3.8.0/tests/test_common/test_models/test_models.py` & `module-build-service-3.9.0/tests/test_common/test_models/test_models.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_common/test_monitor.py` & `module-build-service-3.9.0/tests/test_common/test_monitor.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_common/test_resolve.py` & `module-build-service-3.9.0/tests/test_common/test_resolve.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_common/test_scm.py` & `module-build-service-3.9.0/tests/test_common/test_scm.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_common/test_submit.py` & `module-build-service-3.9.0/tests/test_common/test_submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_common/test_utils.py` & `module-build-service-3.9.0/tests/test_common/test_utils.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_manage.py` & `module-build-service-3.9.0/tests/test_manage.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 # SPDX-License-Identifier: MIT
 from __future__ import absolute_import
 
 import logging
 from mock import patch
 import pytest
 
-from module_build_service import app
+from module_build_service import app, manage as mbs_manager
 from module_build_service.common import models
 from module_build_service.common.models import BUILD_STATES, ModuleBuild
-from module_build_service.manage import manager_wrapper, retire
 from module_build_service.scheduler.db_session import db_session
 from module_build_service.web.utils import deps_to_dict
 from tests import clean_database, staged_data_filename
 
 
 @pytest.mark.usefixtures("provide_test_data")
 class TestMBSManage:
@@ -27,34 +26,36 @@
             ("spam:bacon:eggs", True),
             ("spam:bacon:eggs:ham", True),
             ("spam:bacon:eggs:ham:sausage", False),
         ),
     )
     def test_retire_identifier_validation(self, identifier, is_valid):
         if is_valid:
-            retire(identifier)
+            with pytest.raises(SystemExit) as exc_info:
+                mbs_manager.cli(["retire", identifier])
+                assert 0 == exc_info
         else:
             with pytest.raises(ValueError):
-                retire(identifier)
+                mbs_manager.cli(["retire", identifier])
 
     @pytest.mark.parametrize(
         ("overrides", "identifier", "changed_count"),
         (
             ({"name": "pickme"}, "pickme:eggs", 1),
             ({"stream": "pickme"}, "spam:pickme", 1),
             ({"version": "pickme"}, "spam:eggs:pickme", 1),
             ({"context": "pickme"}, "spam:eggs:ham:pickme", 1),
             ({}, "spam:eggs", 2),
             ({"version": "pickme"}, "spam:eggs", 2),
             ({"context": "pickme"}, "spam:eggs:ham", 2),
         ),
     )
-    @patch("module_build_service.manage.prompt_bool")
-    def test_retire_build(self, prompt_bool, overrides, identifier, changed_count):
-        prompt_bool.return_value = True
+    @patch("click.confirm")
+    def test_retire_build(self, confirm, overrides, identifier, changed_count):
+        confirm.return_value = True
 
         module_builds = (
             db_session.query(ModuleBuild)
             .filter_by(state=BUILD_STATES["ready"])
             .order_by(ModuleBuild.id.desc())
             .all()
         )
@@ -68,15 +69,18 @@
             build.context = str(x)
 
         for attr, value in overrides.items():
             setattr(module_builds[0], attr, value)
 
         db_session.commit()
 
-        retire(identifier)
+        with pytest.raises(SystemExit) as exc_info:
+            mbs_manager.cli(["retire", identifier])
+            assert 0 == exc_info.value
+
         retired_module_builds = (
             db_session.query(ModuleBuild)
             .filter_by(state=BUILD_STATES["garbage"])
             .order_by(ModuleBuild.id.desc())
             .all()
         )
 
@@ -90,36 +94,38 @@
         (
             (True, False, True),
             (True, True, True),
             (False, False, False),
             (False, True, True)
         ),
     )
-    @patch("module_build_service.manage.prompt_bool")
+    @patch("click.confirm")
     def test_retire_build_confirm_prompt(
-        self, prompt_bool, confirm_prompt, confirm_arg, confirm_expected
+        self, confirm, confirm_prompt, confirm_arg, confirm_expected
     ):
-        prompt_bool.return_value = confirm_prompt
+        confirm.return_value = confirm_prompt
 
         module_builds = db_session.query(ModuleBuild).filter_by(state=BUILD_STATES["ready"]).all()
         # Verify our assumption of the amount of ModuleBuilds in database
         assert len(module_builds) == 2
 
         for x, build in enumerate(module_builds):
             build.name = "spam" + str(x) if x > 0 else "spam"
             build.stream = "eggs"
-
         db_session.commit()
 
-        retire("spam:eggs", confirm_arg)
+        cmd = ["retire", "spam:eggs"] + (["--confirm"] if confirm_arg else [])
+        with pytest.raises(SystemExit) as exc_info:
+            mbs_manager.cli(cmd)
+            assert 0 == exc_info.value
+
+        expected_changed_count = 1 if confirm_expected else 0
         retired_module_builds = (
             db_session.query(ModuleBuild).filter_by(state=BUILD_STATES["garbage"]).all()
         )
-
-        expected_changed_count = 1 if confirm_expected else 0
         assert len(retired_module_builds) == expected_changed_count
 
 
 class TestCommandBuildModuleLocally:
     """Test mbs-manager subcommand build_module_locally"""
 
     def setup_method(self, test_method):
@@ -153,15 +159,15 @@
     def _run_manager_wrapper(self, cli_cmd):
         # build_module_locally changes database uri to a local SQLite database file.
         # Restore the uri to original one in order to not impact the database
         # session in subsequent tests.
         original_db_uri = app.config["SQLALCHEMY_DATABASE_URI"]
         try:
             with patch("sys.argv", new=cli_cmd):
-                manager_wrapper()
+                mbs_manager.cli()
         finally:
             app.config["SQLALCHEMY_DATABASE_URI"] = original_db_uri
 
     @patch("module_build_service.scheduler.local.main")
     def test_set_stream(self, main):
         cli_cmd = [
             "mbs-manager", "build_module_locally",
```

### Comparing `module-build-service-3.8.0/tests/test_memory/mbs_configuration.py` & `module-build-service-3.9.0/tests/test_memory/mbs_configuration.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_memory/mbs_debug.py` & `module-build-service-3.9.0/tests/test_memory/mbs_debug.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_memory/test_memory.py` & `module-build-service-3.9.0/tests/test_memory/test_memory.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_resolver/test_db.py` & `module-build-service-3.9.0/tests/test_resolver/test_db.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_resolver/test_koji.py` & `module-build-service-3.9.0/tests/test_resolver/test_koji.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_resolver/test_local.py` & `module-build-service-3.9.0/tests/test_resolver/test_local.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_resolver/test_mbs.py` & `module-build-service-3.9.0/tests/test_resolver/test_mbs.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_batches.py` & `module-build-service-3.9.0/tests/test_scheduler/test_batches.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,11 +417,13 @@
         module_build = models.ModuleBuild.get_by_id(db_session, 3)
         module_build.batch = 1
         db_session.commit()
 
         builder = mock.MagicMock()
         builder.buildroot_ready.return_value = False
 
+        start_next_batch_build(conf, module_build, builder)
+
         module_build = models.ModuleBuild.get_by_id(db_session, 3)
 
         # Batch number should not increase.
         assert module_build.batch == 1
```

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_celery_route_task.py` & `module-build-service-3.9.0/tests/test_scheduler/test_celery_route_task.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_consumer.py` & `module-build-service-3.9.0/tests/test_scheduler/test_consumer.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_db_session.py` & `module-build-service-3.9.0/tests/test_scheduler/test_db_session.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_default_modules.py` & `module-build-service-3.9.0/tests/test_scheduler/test_default_modules.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_module_init.py` & `module-build-service-3.9.0/tests/test_scheduler/test_module_init.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_module_states.py` & `module-build-service-3.9.0/tests/test_scheduler/test_module_states.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_module_wait.py` & `module-build-service-3.9.0/tests/test_scheduler/test_module_wait.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_poller.py` & `module-build-service-3.9.0/tests/test_scheduler/test_poller.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
         ]
 
         with patch.object(conf, "koji_tag_prefixes", new=["module", "another-prefix"]):
             with patch.object(conf, "koji_target_delete_time", new=60):
                 producer.delete_old_koji_targets()
 
             koji_session.deleteBuildTarget.assert_called_once_with(1)
-            koji_session.krb_login.assert_called_once()
+            koji_session.gssapi_login.assert_called_once()
 
     @patch("koji.ClientSession")
     def test_cant_delete_build_target_if_not_reach_delete_time(
         self, ClientSession, create_builder, dbg
     ):
         module_build_2 = models.ModuleBuild.get_by_id(db_session, 2)
         # Only module build 1's build target should be deleted.
```

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_repo_done.py` & `module-build-service-3.9.0/tests/test_scheduler/test_repo_done.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_reuse.py` & `module-build-service-3.9.0/tests/test_scheduler/test_reuse.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_submit.py` & `module-build-service-3.9.0/tests/test_scheduler/test_submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_tag_tagged.py` & `module-build-service-3.9.0/tests/test_scheduler/test_tag_tagged.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_scheduler/test_ursine.py` & `module-build-service-3.9.0/tests/test_scheduler/test_ursine.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_web/test_auth.py` & `module-build-service-3.9.0/tests/test_web/test_auth.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_web/test_mmd_resolver.py` & `module-build-service-3.9.0/tests/test_web/test_mmd_resolver.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_web/test_mse.py` & `module-build-service-3.9.0/tests/test_web/test_mse.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_web/test_submit.py` & `module-build-service-3.9.0/tests/test_web/test_submit.py`

 * *Files identical despite different names*

### Comparing `module-build-service-3.8.0/tests/test_web/test_views.py` & `module-build-service-3.9.0/tests/test_web/test_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,19 +257,21 @@
         assert meta_data["page"] == 2
 
     def test_query_builds(self):
         rv = self.client.get("/module-build-service/1/module-builds/?per_page=2")
         items = json.loads(rv.data)["items"]
         expected = [
             {
+                "batch": 0,
                 "component_builds": [11, 12],
                 "context": "00000000",
                 "id": 7,
                 "koji_tag": None,
                 "name": "testmodule",
+                "new_repo_task_id": None,
                 "owner": "some_other_user",
                 "rebuild_strategy": "changed-and-after",
                 "scmurl": (
                     "git://pkgs.domain.local/modules/testmodule"
                     "?#ca95886c7a443b36a9ce31abda1f9bef22f2f8c9"
                 ),
                 "scratch": False,
@@ -298,19 +300,21 @@
                 "time_completed": None,
                 "time_modified": "2016-09-03T12:38:40Z",
                 "time_submitted": "2016-09-03T12:38:33Z",
                 "version": "7",
                 "buildrequires": {},
             },
             {
+                "batch": 2,
                 "component_builds": [9, 10],
                 "context": "00000000",
                 "id": 6,
                 "koji_tag": "module-postgressql-1.2",
                 "name": "postgressql",
+                "new_repo_task_id": None,
                 "owner": "some_user",
                 "rebuild_strategy": "changed-and-after",
                 "scmurl": (
                     "git://pkgs.domain.local/modules/postgressql"
                     "?#aa95886c7a443b36a9ce31abda1f9bef22f2f8c9"
                 ),
                 "scratch": False,
@@ -454,15 +458,15 @@
         assert results[0]["koji_tag"] == "module-testmodule-master-20170219191323-c40c156c"
         assert results[1]["koji_tag"] == "module-testmodule-master-20170109091357-78e4a6fd"
 
         mock_session.getRPM.assert_called_once_with(
             "module-build-macros-0.1-1.testmodule_master_20170303190726.src.rpm")
         mock_session.listTags.assert_called_once_with(mock_rpm_md["build_id"])
 
-        mock_session.krb_login.assert_not_called()
+        mock_session.gssapi_login.assert_not_called()
 
     @pytest.mark.parametrize(
         "provide_test_data", [{"data_size": 1, "contexts": True}], indirect=True
     )
     @pytest.mark.usefixtures("provide_test_data")  # cleans the database
     def test_query_builds_with_context(self):
         rv = self.client.get("/module-build-service/1/module-builds/?context=3a4057d2")
@@ -472,19 +476,21 @@
         # Get component build ids dynamically rather than hardcode inside expected output.
         component_build_ids = db_session.query(ComponentBuild).filter(
             ComponentBuild.module_id == checking_build_id
         ).order_by(ComponentBuild.id).options(load_only("id")).all()
 
         expected = [
             {
+                "batch": 2,
                 "component_builds": [cb.id for cb in component_build_ids],
                 "context": "3a4057d2",
                 "id": checking_build_id,
                 "koji_tag": "module-nginx-1.2",
                 "name": "nginx",
+                "new_repo_task_id": None,
                 "owner": "Moe Szyslak",
                 "rebuild_strategy": "changed-and-after",
                 "scmurl": (
                     "git://pkgs.domain.local/modules/nginx"
                     "?#ba95886c7a443b36a9ce31abda1f9bef22f2f8c9"
                 ),
                 "scratch": False,
```

