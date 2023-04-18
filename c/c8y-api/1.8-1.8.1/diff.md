# Comparing `tmp/c8y_api-1.8.tar.gz` & `tmp/c8y_api-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c8y_api-1.8.tar", last modified: Fri Apr 14 14:20:08 2023, max compression
+gzip compressed data, was "c8y_api-1.8.1.tar", last modified: Tue Apr 18 07:05:46 2023, max compression
```

## Comparing `c8y_api-1.8.tar` & `c8y_api-1.8.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.355218 c8y_api-1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.331217 c8y_api-1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.335217 c8y_api-1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-14 14:19:56.000000 c8y_api-1.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-14 14:19:56.000000 c8y_api-1.8/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-14 14:19:56.000000 c8y_api-1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-14 14:19:56.000000 c8y_api-1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-14 14:19:56.000000 c8y_api-1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 14:19:56.000000 c8y_api-1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-14 14:20:08.355218 c8y_api-1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-14 14:19:56.000000 c8y_api-1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.335217 c8y_api-1.8/c8y_api/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_main_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.335217 c8y_api-1.8/c8y_api/app/
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.339218 c8y_api-1.8/c8y_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/administration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/binaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    17823 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    17926 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    22887 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/managedobjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/notification2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_api/model/tenant_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.335217 c8y_api-1.8/c8y_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-14 14:20:08.000000 c8y_api-1.8/c8y_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-14 14:20:08.000000 c8y_api-1.8/c8y_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:20:08.000000 c8y_api-1.8/c8y_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-14 14:20:08.000000 c8y_api-1.8/c8y_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 14:20:08.000000 c8y_api-1.8/c8y_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.339218 c8y_api-1.8/c8y_tk/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_tk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.339218 c8y_api-1.8/c8y_tk/notification2/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_tk/notification2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-14 14:19:56.000000 c8y_api-1.8/c8y_tk/notification2/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.343218 c8y_api-1.8/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_alarms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_audits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_binaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_device_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_devicegroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_global_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_inventoryroles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_tenant_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 14:19:56.000000 c8y_api-1.8/integration_tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-04-14 14:19:56.000000 c8y_api-1.8/pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-14 14:19:56.000000 c8y_api-1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-14 14:19:56.000000 c8y_api-1.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.347218 c8y_api-1.8/samples/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/cumulocity-tenant_options.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/cumulocity.json
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/dealing_with_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/handling_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/multi_tenant_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/notification2_asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/notification2_synchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/simple_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/simple_tenant_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/tenant_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/user_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-14 14:19:56.000000 c8y_api-1.8/samples/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-14 14:20:08.355218 c8y_api-1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-14 14:19:56.000000 c8y_api-1.8/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.347218 c8y_api-1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.355218 c8y_api-1.8/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/alarm.json
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/application.json
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/audit_records.json
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/bulk_operations.json
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/device.json
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/event.json
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/global_role.json
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/inventoryrole.json
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/managed_object.json
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/operation.json
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/series.json
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/subscriptions.json
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/tenant_option.json
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_bulk_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_global_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_inventoryrole.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_managedobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_tenant_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    42314 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/model/user.json
--rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/test_base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/test_device_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-14 14:19:56.000000 c8y_api-1.8/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:20:08.355218 c8y_api-1.8/util/
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-14 14:19:56.000000 c8y_api-1.8/util/microservice_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-14 14:19:56.000000 c8y_api-1.8/util/testing_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.873045 c8y_api-1.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.853045 c8y_api-1.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.857045 c8y_api-1.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-18 07:05:33.000000 c8y_api-1.8.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-18 07:05:33.000000 c8y_api-1.8.1/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-18 07:05:33.000000 c8y_api-1.8.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-18 07:05:33.000000 c8y_api-1.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-18 07:05:33.000000 c8y_api-1.8.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 07:05:33.000000 c8y_api-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-18 07:05:46.873045 c8y_api-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-18 07:05:33.000000 c8y_api-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.857045 c8y_api-1.8.1/c8y_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_main_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.857045 c8y_api-1.8.1/c8y_api/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.865045 c8y_api-1.8.1/c8y_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21589 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38043 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/administration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19945 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/binaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17823 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17926 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22887 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/managedobjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22140 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/notification2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18792 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_api/model/tenant_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.857045 c8y_api-1.8.1/c8y_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-04-18 07:05:46.000000 c8y_api-1.8.1/c8y_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-18 07:05:46.000000 c8y_api-1.8.1/c8y_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:05:46.000000 c8y_api-1.8.1/c8y_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 07:05:46.000000 c8y_api-1.8.1/c8y_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 07:05:46.000000 c8y_api-1.8.1/c8y_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.865045 c8y_api-1.8.1/c8y_tk/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_tk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.865045 c8y_api-1.8.1/c8y_tk/notification2/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_tk/notification2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-18 07:05:33.000000 c8y_api-1.8.1/c8y_tk/notification2/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.865045 c8y_api-1.8.1/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_alarms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_audits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_device_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_devicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_global_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_inventoryroles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_tenant_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-18 07:05:33.000000 c8y_api-1.8.1/integration_tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-04-18 07:05:33.000000 c8y_api-1.8.1/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 07:05:33.000000 c8y_api-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-18 07:05:33.000000 c8y_api-1.8.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.865045 c8y_api-1.8.1/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/cumulocity-tenant_options.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/cumulocity.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/dealing_with_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/handling_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/multi_tenant_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/notification2_asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/notification2_synchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/simple_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/simple_tenant_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/tenant_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/user_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-18 07:05:33.000000 c8y_api-1.8.1/samples/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-18 07:05:46.873045 c8y_api-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.869045 c8y_api-1.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.873045 c8y_api-1.8.1/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/alarm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/audit_records.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/bulk_operations.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/event.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/global_role.json
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/inventoryrole.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/managed_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/operation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/series.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/subscriptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/tenant_option.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_bulk_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_global_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_inventoryrole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_managedobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_tenant_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42314 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/model/user.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/test_base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/test_device_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-18 07:05:33.000000 c8y_api-1.8.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:05:46.873045 c8y_api-1.8.1/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-18 07:05:33.000000 c8y_api-1.8.1/util/microservice_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-18 07:05:33.000000 c8y_api-1.8.1/util/testing_util.py
```

### Comparing `c8y_api-1.8/.github/workflows/codeql-analysis.yml` & `c8y_api-1.8.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/.github/workflows/python-publish.yml` & `c8y_api-1.8.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/CHANGELOG.md` & `c8y_api-1.8.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/LICENSE` & `c8y_api-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/PKG-INFO` & `c8y_api-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c8y_api
-Version: 1.8
+Version: 1.8.1
 Summary: Python client for the Cumulocity REST API
 Home-page: https://github.com/SoftwareAG/cumulocity-python-api
 Author: Christoph Souris
 Author-email: christoph.souris@softwareag.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `c8y_api-1.8/README.md` & `c8y_api-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/_auth.py` & `c8y_api-1.8.1/c8y_api/_auth.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/_base_api.py` & `c8y_api-1.8.1/c8y_api/_base_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/_jwt.py` & `c8y_api-1.8.1/c8y_api/_jwt.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/_main_api.py` & `c8y_api-1.8.1/c8y_api/_main_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/_registry_api.py` & `c8y_api-1.8.1/c8y_api/_registry_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/_util.py` & `c8y_api-1.8.1/c8y_api/_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/app/__init__.py` & `c8y_api-1.8.1/c8y_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/__init__.py` & `c8y_api-1.8.1/c8y_api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/_base.py` & `c8y_api-1.8.1/c8y_api/model/_base.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/_parser.py` & `c8y_api-1.8.1/c8y_api/model/_parser.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/_util.py` & `c8y_api-1.8.1/c8y_api/model/_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/administration.py` & `c8y_api-1.8.1/c8y_api/model/administration.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/alarms.py` & `c8y_api-1.8.1/c8y_api/model/alarms.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/applications.py` & `c8y_api-1.8.1/c8y_api/model/applications.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/audit.py` & `c8y_api-1.8.1/c8y_api/model/audit.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/binaries.py` & `c8y_api-1.8.1/c8y_api/model/binaries.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/events.py` & `c8y_api-1.8.1/c8y_api/model/events.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/identity.py` & `c8y_api-1.8.1/c8y_api/model/identity.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/inventory.py` & `c8y_api-1.8.1/c8y_api/model/inventory.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/managedobjects.py` & `c8y_api-1.8.1/c8y_api/model/managedobjects.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/measurements.py` & `c8y_api-1.8.1/c8y_api/model/measurements.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,69 +281,69 @@
 
             # single value
             if value:
                 if not timestamps:
                     # iterate over all values, select value group at specific
                     # index v[i] and extract specific value [value]. The value
                     # group may be undefined (None), hence filter for value v[i]
-                    return [v[i][value] for v in self['values'].values() if v[i]]
+                    return [v[i][value] for v in self['values'].values() if (len(v) > i and v[i])]
                 else:
                     # like above, but include timestamps
-                    return [(parse_timestamp(k), v[i][value]) for k, v in self['values'].items() if v[i]]
+                    return [(parse_timestamp(k), v[i][value]) for k, v in self['values'].items() if (len(v) > i and v[i])]
 
             # all values
             else:
                 if not timestamps:
                     # iterate over all values, select value group at specific
                     # index v[i] and extract both values (min, max). The value
                     # group may be undefined (None), hence filter for value v[i]
-                    return [(v[i]['min'], v[i]['max']) for v in self['values'].values() if v[i]]
+                    return [(v[i]['min'], v[i]['max']) for v in self['values'].values() if (len(v) > i and v[i])]
                 else:
                     # like above, but include timestamps
-                    return [(parse_timestamp(k), v[i]['min'], v[i]['max']) for k, v in self['values'].items() if v[i]]
+                    return [(parse_timestamp(k), v[i]['min'], v[i]['max']) for k, v in self['values'].items() if (len(v) > i and v[i])]
 
         # multiple series
         if isinstance(series, Sequence):
             ii = [indexes_by_name()[s] for s in series]
 
             # single value
             if value:
                 if not timestamps:
                     # iterate over all values, collect specified value groups
                     # at their index v[i] and extract specific value [value].
                     # The value group may be undefined (None) which will result
                     # in a None value in the tuple as well.
                     return [
                         # collect values of all indexes (None of not defined)
-                        tuple(v[i][value] if v[i] else None for i in ii)
+                        tuple(v[i][value] if (len(v) > i and v[i]) else None for i in ii)
                         for v in self['values'].values()
                     ]
                 else:
                     # like above, but prepend with timestamps
                     return [
-                        (parse_timestamp(k), *(v[i][value] if v[i] else None for i in ii))
+                        (parse_timestamp(k), *(v[i][value] if (len(v) > i and v[i]) else None for i in ii))
                         for k, v in self['values'].items()
                     ]
 
             # all values
             else:
                 if not timestamps:
                     # iterate over all values, collect specified value groups
                     # at their index v[i] and extract specific value [value].
                     # The value group may be undefined (None) which will result
                     # in a None value in the tuple as well.
                     return [
                         # collect values of all indexes (None of not defined)
-                        tuple((v[i]['min'], v[i]['max']) if v[i] else None for i in ii)
+                        tuple((v[i]['min'], v[i]['max']) if (len(v) > i and v[i]) else None for i in ii)
                         for v in self['values'].values()
                     ]
                 else:
                     # like above, but prepend with timestamps
                     return [
-                        (parse_timestamp(k), *((v[i]['min'], v[i]['max']) if v[i] else None for i in ii))
+                        (parse_timestamp(k), *((v[i]['min'], v[i]['max']) if (len(v) > i and v[i]) else None for i in ii))
                         for k, v in self['values'].items()
                     ]
 
         raise ValueError("Invalid combination of arguments")
 
 
 class Measurements(CumulocityResource):
```

### Comparing `c8y_api-1.8/c8y_api/model/notification2.py` & `c8y_api-1.8.1/c8y_api/model/notification2.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/operations.py` & `c8y_api-1.8.1/c8y_api/model/operations.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api/model/tenant_options.py` & `c8y_api-1.8.1/c8y_api/model/tenant_options.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_api.egg-info/PKG-INFO` & `c8y_api-1.8.1/c8y_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c8y-api
-Version: 1.8
+Version: 1.8.1
 Summary: Python client for the Cumulocity REST API
 Home-page: https://github.com/SoftwareAG/cumulocity-python-api
 Author: Christoph Souris
 Author-email: christoph.souris@softwareag.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `c8y_api-1.8/c8y_api.egg-info/SOURCES.txt` & `c8y_api-1.8.1/c8y_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/c8y_tk/notification2/listener.py` & `c8y_api-1.8.1/c8y_tk/notification2/listener.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/conftest.py` & `c8y_api-1.8.1/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_alarms.py` & `c8y_api-1.8.1/integration_tests/test_alarms.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_applications.py` & `c8y_api-1.8.1/integration_tests/test_applications.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_audits.py` & `c8y_api-1.8.1/integration_tests/test_audits.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_binaries.py` & `c8y_api-1.8.1/integration_tests/test_binaries.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_bulk_operations.py` & `c8y_api-1.8.1/integration_tests/test_bulk_operations.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_device_registry.py` & `c8y_api-1.8.1/integration_tests/test_device_registry.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_devicegroups.py` & `c8y_api-1.8.1/integration_tests/test_devicegroups.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_events.py` & `c8y_api-1.8.1/integration_tests/test_events.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_global_roles.py` & `c8y_api-1.8.1/integration_tests/test_global_roles.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_identity.py` & `c8y_api-1.8.1/integration_tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_inventory.py` & `c8y_api-1.8.1/integration_tests/test_inventory.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_inventoryroles.py` & `c8y_api-1.8.1/integration_tests/test_inventoryroles.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_measurements.py` & `c8y_api-1.8.1/integration_tests/test_measurements.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_operations.py` & `c8y_api-1.8.1/integration_tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_tenant_options.py` & `c8y_api-1.8.1/integration_tests/test_tenant_options.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/integration_tests/test_users.py` & `c8y_api-1.8.1/integration_tests/test_users.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/pylintrc` & `c8y_api-1.8.1/pylintrc`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/build.sh` & `c8y_api-1.8.1/samples/build.sh`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/dealing_with_measurements.py` & `c8y_api-1.8.1/samples/dealing_with_measurements.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/handling_events.py` & `c8y_api-1.8.1/samples/handling_events.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/multi_tenant_app.py` & `c8y_api-1.8.1/samples/multi_tenant_app.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/notification2_asynchronous.py` & `c8y_api-1.8.1/samples/notification2_asynchronous.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/notification2_synchronous.py` & `c8y_api-1.8.1/samples/notification2_synchronous.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/simple_agent.py` & `c8y_api-1.8.1/samples/simple_agent.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/simple_tenant_app.py` & `c8y_api-1.8.1/samples/simple_tenant_app.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/tenant_options.py` & `c8y_api-1.8.1/samples/tenant_options.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/user_sessions.py` & `c8y_api-1.8.1/samples/user_sessions.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/samples/util.py` & `c8y_api-1.8.1/samples/util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/setup.cfg` & `c8y_api-1.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tasks.py` & `c8y_api-1.8.1/tasks.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/alarm.json` & `c8y_api-1.8.1/tests/model/alarm.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/application.json` & `c8y_api-1.8.1/tests/model/application.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/audit_records.json` & `c8y_api-1.8.1/tests/model/audit_records.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/bulk_operations.json` & `c8y_api-1.8.1/tests/model/bulk_operations.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/device.json` & `c8y_api-1.8.1/tests/model/device.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/event.json` & `c8y_api-1.8.1/tests/model/event.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/global_role.json` & `c8y_api-1.8.1/tests/model/global_role.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/inventoryrole.json` & `c8y_api-1.8.1/tests/model/inventoryrole.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/managed_object.json` & `c8y_api-1.8.1/tests/model/managed_object.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/series.json` & `c8y_api-1.8.1/tests/model/series.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'values'": "{'2023-04-04T16:00:00.000Z': {delete: [1]}}"}*

```diff
@@ -43,16 +43,15 @@
                 "min": 5
             }
         ],
         "2023-04-04T16:00:00.000Z": [
             {
                 "max": 39.0,
                 "min": 10.0
-            },
-            {}
+            }
         ],
         "2023-04-04T17:00:00.000Z": [
             {},
             {
                 "max": 6,
                 "min": 5
             }
```

### Comparing `c8y_api-1.8/tests/model/subscriptions.json` & `c8y_api-1.8.1/tests/model/subscriptions.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/tenant_option.json` & `c8y_api-1.8.1/tests/model/tenant_option.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_alarm.py` & `c8y_api-1.8.1/tests/model/test_alarm.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_application.py` & `c8y_api-1.8.1/tests/model/test_application.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_audit.py` & `c8y_api-1.8.1/tests/model/test_audit.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_base.py` & `c8y_api-1.8.1/tests/model/test_base.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_bulk_operation.py` & `c8y_api-1.8.1/tests/model/test_bulk_operation.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_device.py` & `c8y_api-1.8.1/tests/model/test_device.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_event.py` & `c8y_api-1.8.1/tests/model/test_event.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_global_role.py` & `c8y_api-1.8.1/tests/model/test_global_role.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_inventory.py` & `c8y_api-1.8.1/tests/model/test_inventory.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_inventoryrole.py` & `c8y_api-1.8.1/tests/model/test_inventoryrole.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_managedobject.py` & `c8y_api-1.8.1/tests/model/test_managedobject.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_measurements.py` & `c8y_api-1.8.1/tests/model/test_measurements.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_operation.py` & `c8y_api-1.8.1/tests/model/test_operation.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_parser.py` & `c8y_api-1.8.1/tests/model/test_parser.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_resource.py` & `c8y_api-1.8.1/tests/model/test_resource.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_subscription.py` & `c8y_api-1.8.1/tests/model/test_subscription.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_tenant_option.py` & `c8y_api-1.8.1/tests/model/test_tenant_option.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/test_user.py` & `c8y_api-1.8.1/tests/model/test_user.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/model/user.json` & `c8y_api-1.8.1/tests/model/user.json`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/test_app.py` & `c8y_api-1.8.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/test_auth.py` & `c8y_api-1.8.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/test_base_api.py` & `c8y_api-1.8.1/tests/test_base_api.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/test_device_registry.py` & `c8y_api-1.8.1/tests/test_device_registry.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/test_util.py` & `c8y_api-1.8.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/tests/utils.py` & `c8y_api-1.8.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/util/microservice_util.py` & `c8y_api-1.8.1/util/microservice_util.py`

 * *Files identical despite different names*

### Comparing `c8y_api-1.8/util/testing_util.py` & `c8y_api-1.8.1/util/testing_util.py`

 * *Files identical despite different names*

