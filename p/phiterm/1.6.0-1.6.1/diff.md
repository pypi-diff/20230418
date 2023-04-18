# Comparing `tmp/phiterm-1.6.0.tar.gz` & `tmp/phiterm-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.6.0.tar", last modified: Tue Apr 18 12:04:04 2023, max compression
+gzip compressed data, was "phiterm-1.6.1.tar", last modified: Tue Apr 18 15:39:39 2023, max compression
```

## Comparing `phiterm-1.6.0.tar` & `phiterm-1.6.1.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.229396 phiterm-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-18 12:03:44.000000 phiterm-1.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 12:04:04.229396 phiterm-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 12:03:44.000000 phiterm-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35058 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26450 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.229396 phiterm-1.6.0/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.229396 phiterm-1.6.0/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.229396 phiterm-1.6.0/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    40282 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-18 12:03:44.000000 phiterm-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 12:04:04.229396 phiterm-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 12:03:44.000000 phiterm-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.229396 phiterm-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 12:03:44.000000 phiterm-1.6.0/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.585495 phiterm-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-18 15:39:18.000000 phiterm-1.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 15:39:39.585495 phiterm-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 15:39:18.000000 phiterm-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35058 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.569496 phiterm-1.6.1/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.577495 phiterm-1.6.1/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.581495 phiterm-1.6.1/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.585495 phiterm-1.6.1/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40282 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-18 15:39:18.000000 phiterm-1.6.1/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.573495 phiterm-1.6.1/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 15:39:39.000000 phiterm-1.6.1/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-18 15:39:18.000000 phiterm-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:39:39.585495 phiterm-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 15:39:18.000000 phiterm-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:39:39.585495 phiterm-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 15:39:18.000000 phiterm-1.6.1/tests/test_backend_api.py
```

### Comparing `phiterm-1.6.0/LICENSE.md` & `phiterm-1.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/api/client.py` & `phiterm-1.6.1/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/api/routes.py` & `phiterm-1.6.1/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/api/user.py` & `phiterm-1.6.1/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/api/workspace.py` & `phiterm-1.6.1/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/aws/aws_operator.py` & `phiterm-1.6.1/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/cli/cli_app.py` & `phiterm-1.6.1/phiterm/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/cli/cli_operator.py` & `phiterm-1.6.1/phiterm/cli/cli_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/cli/dx/dx_app.py` & `phiterm-1.6.1/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.6.1/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.6.1/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.6.1/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/cli/wf/wf_app.py` & `phiterm-1.6.1/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/cli/ws/ws_app.py` & `phiterm-1.6.1/phiterm/cli/ws/ws_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/conf/auth.py` & `phiterm-1.6.1/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/conf/constants.py` & `phiterm-1.6.1/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/conf/phi_conf.py` & `phiterm-1.6.1/phiterm/conf/phi_conf.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/databox/databox_operator.py` & `phiterm-1.6.1/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/docker/docker_operator.py` & `phiterm-1.6.1/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/enums/user.py` & `phiterm-1.6.1/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/k8s/k8s_operator.py` & `phiterm-1.6.1/phiterm/k8s/k8s_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,23 @@
 from phidata.infra.config import InfraConfig
 from phidata.k8s.api_client import K8sApiClient
 from phidata.k8s.config import K8sConfig
 from phidata.k8s.exceptions import K8sConfigException
 from phidata.k8s.manager import K8sManager
 from phidata.k8s.resource.types import K8sResourceType, K8sResource
 from phidata.k8s.resource.group import K8sResourceGroup
-from phidata.k8s.resource.utils import (
-    get_k8s_resources_from_group,
-    filter_and_flatten_k8s_resource_groups,
-)
+from phidata.k8s.resource.utils import get_k8s_resources_from_group
 from phidata.product import DataProduct
 from phidata.workflow import Workflow
 from phidata.types.context import PathContext, RunContext
-from phidata.utils.prep_infra_config import prep_infra_config
 
 from phiterm.workspace.phi_ws_data import PhiWsData
-from phiterm.workspace.ws_enums import WorkspaceEnv, WorkspaceConfigType
+from phiterm.workspace.ws_enums import WorkspaceConfigType
 from phiterm.workspace.ws_operator import filter_and_prep_configs
+from phiterm.workspace.ws_utils import get_ws_config_dir_path
 from phiterm.types.run_status import RunStatus
 from phiterm.utils.filesystem import delete_files_in_dir
 from phiterm.utils.cli_console import (
     print_error,
     print_heading,
     print_subheading,
     print_info,
@@ -226,19 +223,19 @@
 
         # Step 2: Get the K8sManager
         k8s_manager: K8sManager = config.get_k8s_manager()
         if k8s_manager is None:
             raise K8sConfigException("K8sManager unavailable")
 
         # Step 3: Prep the directory to write to
-        workspace_config_file_path: Optional[Path] = ws_data.ws_config_file_path
-        if workspace_config_file_path is None:
-            print_error("workspace_config_file_path invalid")
+        ws_root_path: Optional[Path] = ws_data.ws_root_path
+        if ws_root_path is None:
+            print_error("ws_root_path invalid")
             continue
-        workspace_config_dir: Path = workspace_config_file_path.parent.resolve()
+        workspace_config_dir: Optional[Path] = get_ws_config_dir_path(ws_root_path)
         if workspace_config_dir is None:
             print_error("workspace_config_dir invalid")
             continue
 
         resources_dir: Path = workspace_config_dir.joinpath(config.resources_dir)
         if config.env is not None:
             resources_dir = resources_dir.joinpath(config.env)
```

### Comparing `phiterm-1.6.0/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.6.1/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.6.1/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.6.1/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.6.1/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/local/local_operator.py` & `phiterm-1.6.1/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/release/release_schemas.py` & `phiterm-1.6.1/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/release/ws_releases.py` & `phiterm-1.6.1/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/schemas/user.py` & `phiterm-1.6.1/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/schemas/user_schemas.py` & `phiterm-1.6.1/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/schemas/workspace.py` & `phiterm-1.6.1/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.6.1/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.6.1/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.6.1/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.6.1/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.6.1/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.6.1/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.6.1/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.6.1/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.6.1/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.6.1/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/cli_auth_server.py` & `phiterm-1.6.1/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/cli_console.py` & `phiterm-1.6.1/phiterm/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/common.py` & `phiterm-1.6.1/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/dttm.py` & `phiterm-1.6.1/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/enums.py` & `phiterm-1.6.1/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/filesystem.py` & `phiterm-1.6.1/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/git.py` & `phiterm-1.6.1/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/load_env.py` & `phiterm-1.6.1/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/log.py` & `phiterm-1.6.1/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/pyproject.py` & `phiterm-1.6.1/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/utils/ws_filter.py` & `phiterm-1.6.1/phiterm/utils/ws_filter.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/workflow/wf_operator.py` & `phiterm-1.6.1/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/workflow/wf_utils.py` & `phiterm-1.6.1/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/workspace/phi_ws_data.py` & `phiterm-1.6.1/phiterm/workspace/phi_ws_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/workspace/ws_enums.py` & `phiterm-1.6.1/phiterm/workspace/ws_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/workspace/ws_loader.py` & `phiterm-1.6.1/phiterm/workspace/ws_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from pathlib import Path
 from typing import Optional, List, Dict
 
-from pydantic import ValidationError
-from phidata.workspace.config import WorkspaceConfig, WorkspaceSettings
-from phiterm.workspace.ws_utils import (
-    get_ws_config_file_path,
-    get_ws_config_dir_path,
-)
+from phidata.workspace.config import WorkspaceConfig
+from phiterm.workspace.ws_utils import get_ws_config_dir_path
 
-from phiterm.workspace.exceptions import WorkspaceException
-from phiterm.utils.cli_console import print_error, print_info, print_validation_errors
 from phiterm.utils.log import logger
 
 
 def add_ws_dir_to_path(ws_root_path: Path) -> None:
     # Add ws_root_path to sys.path so is treated as a package
     try:
         import sys
```

### Comparing `phiterm-1.6.0/phiterm/workspace/ws_operator.py` & `phiterm-1.6.1/phiterm/workspace/ws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/workspace/ws_schemas.py` & `phiterm-1.6.1/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm/workspace/ws_utils.py` & `phiterm-1.6.1/phiterm/workspace/ws_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/phiterm.egg-info/SOURCES.txt` & `phiterm-1.6.1/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.0/pyproject.toml` & `phiterm-1.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.6.0"
+version = "1.6.1"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

