# Comparing `tmp/phiterm-1.5.9.tar.gz` & `tmp/phiterm-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.5.9.tar", last modified: Tue Apr 11 01:49:29 2023, max compression
+gzip compressed data, was "phiterm-1.6.0.tar", last modified: Tue Apr 18 12:04:04 2023, max compression
```

## Comparing `phiterm-1.5.9.tar` & `phiterm-1.6.0.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.183017 phiterm-1.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-11 01:49:04.000000 phiterm-1.5.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 01:49:29.183017 phiterm-1.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-11 01:49:04.000000 phiterm-1.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.167016 phiterm-1.5.9/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.171016 phiterm-1.5.9/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.175016 phiterm-1.5.9/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.175016 phiterm-1.5.9/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.175016 phiterm-1.5.9/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26450 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.175016 phiterm-1.5.9/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.175016 phiterm-1.5.9/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.175016 phiterm-1.5.9/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.167016 phiterm-1.5.9/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.179017 phiterm-1.5.9/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.179017 phiterm-1.5.9/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.179017 phiterm-1.5.9/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.179017 phiterm-1.5.9/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.179017 phiterm-1.5.9/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.183017 phiterm-1.5.9/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.183017 phiterm-1.5.9/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.183017 phiterm-1.5.9/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    41711 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12664 2023-04-11 01:49:04.000000 phiterm-1.5.9/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.167016 phiterm-1.5.9/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-11 01:49:29.000000 phiterm-1.5.9/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-11 01:49:29.000000 phiterm-1.5.9/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:49:29.000000 phiterm-1.5.9/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-11 01:49:29.000000 phiterm-1.5.9/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-11 01:49:29.000000 phiterm-1.5.9/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 01:49:29.000000 phiterm-1.5.9/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-11 01:49:04.000000 phiterm-1.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:49:29.183017 phiterm-1.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-11 01:49:04.000000 phiterm-1.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:49:29.183017 phiterm-1.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-11 01:49:04.000000 phiterm-1.5.9/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.229396 phiterm-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-18 12:03:44.000000 phiterm-1.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 12:04:04.229396 phiterm-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 12:03:44.000000 phiterm-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35058 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26450 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.221396 phiterm-1.6.0/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.225396 phiterm-1.6.0/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.229396 phiterm-1.6.0/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.229396 phiterm-1.6.0/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.229396 phiterm-1.6.0/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40282 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-04-18 12:03:44.000000 phiterm-1.6.0/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.217396 phiterm-1.6.0/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 12:04:04.000000 phiterm-1.6.0/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-18 12:03:44.000000 phiterm-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 12:04:04.229396 phiterm-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 12:03:44.000000 phiterm-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:04:04.229396 phiterm-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 12:03:44.000000 phiterm-1.6.0/tests/test_backend_api.py
```

### Comparing `phiterm-1.5.9/LICENSE.md` & `phiterm-1.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/api/client.py` & `phiterm-1.6.0/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/api/routes.py` & `phiterm-1.6.0/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/api/user.py` & `phiterm-1.6.0/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/api/workspace.py` & `phiterm-1.6.0/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/aws/aws_operator.py` & `phiterm-1.6.0/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/cli/cli_app.py` & `phiterm-1.6.0/phiterm/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/cli/cli_operator.py` & `phiterm-1.6.0/phiterm/cli/cli_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/cli/dx/dx_app.py` & `phiterm-1.6.0/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.6.0/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.6.0/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.6.0/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/cli/wf/wf_app.py` & `phiterm-1.6.0/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/cli/ws/ws_app.py` & `phiterm-1.6.0/phiterm/cli/ws/ws_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,40 +33,40 @@
     invoke_without_command=True,
     options_metavar="\b",
     subcommand_metavar="<command>",
 )
 
 
 @ws_app.command(short_help="Create a new workspace in the current directory.")
-def init(
+def create(
     ws_name: str = typer.Option(
         None, "-ws", help="Name of the new workspace", show_default=False
     ),
     template: str = typer.Option(
-        "aws-data-platform",
+        "ml-app",
         "-t",
         "--template",
-        help="Choose a starter template which comes pre-populated with defaults",
+        help="Choose a starter template for the workspace",
         show_default=True,
     ),
     print_debug_log: bool = typer.Option(
         False,
         "-d",
         "--debug",
         help="Print debug logs.",
     ),
 ):
     """\b
     Creates a new workspace in the current directory using the selected starter template
-    [default: aws-data-platform]
+    [default: ml-app]
 
     \b
     Examples:
-    $ phi ws init                 -> Create a new workspace
-    $ phi ws init -ws data        -> Create a workspace named data using the default starter template (aws)
+    $ phi ws init            -> Create a new workspace
+    $ phi ws init -ws ml     -> Create a workspace named data using the default starter template (aws)
     """
     from phiterm.workspace.ws_operator import (
         create_new_workspace,
         initialize_workspace,
     )
 
     if print_debug_log:
```

### Comparing `phiterm-1.5.9/phiterm/conf/auth.py` & `phiterm-1.6.0/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/conf/constants.py` & `phiterm-1.6.0/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/conf/phi_conf.py` & `phiterm-1.6.0/phiterm/conf/phi_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     # END
     ######################################################
 
     def add_new_ws_to_config(
         self,
         ws_name: str,
         ws_root_path: Path,
-        ws_config_file_path: Path,
+        ws_config_file_path: Optional[Path] = None,
     ) -> None:
         """Adds a newly created workspace to the PhiConf"""
         self._add_or_update_ws_data(
             ws_name=ws_name,
             ws_root_path=ws_root_path,
             ws_config_file_path=ws_config_file_path,
         )
```

### Comparing `phiterm-1.5.9/phiterm/databox/databox_operator.py` & `phiterm-1.6.0/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/docker/docker_operator.py` & `phiterm-1.6.0/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/enums/user.py` & `phiterm-1.6.0/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/k8s/k8s_operator.py` & `phiterm-1.6.0/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.6.0/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.6.0/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.6.0/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.6.0/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/local/local_operator.py` & `phiterm-1.6.0/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/release/release_schemas.py` & `phiterm-1.6.0/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/release/ws_releases.py` & `phiterm-1.6.0/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/schemas/user.py` & `phiterm-1.6.0/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/schemas/user_schemas.py` & `phiterm-1.6.0/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/schemas/workspace.py` & `phiterm-1.6.0/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.6.0/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.6.0/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.6.0/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.6.0/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.6.0/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.6.0/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.6.0/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.6.0/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.6.0/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.6.0/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/utils/cli_auth_server.py` & `phiterm-1.6.0/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/utils/cli_console.py` & `phiterm-1.6.0/phiterm/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/utils/common.py` & `phiterm-1.6.0/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/utils/dttm.py` & `phiterm-1.6.0/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/utils/enums.py` & `phiterm-1.6.0/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/utils/filesystem.py` & `phiterm-1.6.0/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/utils/git.py` & `phiterm-1.6.0/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/utils/load_env.py` & `phiterm-1.6.0/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/utils/log.py` & `phiterm-1.6.0/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/utils/pyproject.py` & `phiterm-1.6.0/phiterm/utils/pyproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
 from typing import Optional, Dict
 
 from phiterm.utils.log import logger
 
 
 def read_pyproject_phidata(pyproject_file: Path) -> Optional[Dict]:
-    logger.debug(f"reading {pyproject_file}")
+    logger.debug(f"Reading {pyproject_file}")
     try:
         import tomli
 
         pyproject_dict = tomli.loads(pyproject_file.read_text())
-        logger.debug(f"pyproject_dict: {pyproject_dict}")
+        # logger.debug(f"pyproject_dict: {pyproject_dict}")
         phidata_conf = pyproject_dict.get("tool", {}).get("phidata", None)
         if phidata_conf is not None and isinstance(phidata_conf, dict):
             return phidata_conf
     except Exception as e:
         logger.error(f"Could not read {pyproject_file}")
         logger.error(e)
     return None
```

### Comparing `phiterm-1.5.9/phiterm/utils/ws_filter.py` & `phiterm-1.6.0/phiterm/utils/ws_filter.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/workflow/wf_operator.py` & `phiterm-1.6.0/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/workflow/wf_utils.py` & `phiterm-1.6.0/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/workspace/phi_ws_data.py` & `phiterm-1.6.0/phiterm/workspace/phi_ws_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from phidata.workspace import WorkspaceConfig
 
 from phiterm.schemas.workspace import WorkspaceSchema
 from phiterm.utils.common import is_empty
 from phiterm.utils.dttm import current_datetime_utc
 from phiterm.utils.log import logger
 from phiterm.workspace.ws_enums import WorkspaceSetupActions
-from phiterm.workspace.exceptions import WorkspaceConfigException
+from phiterm.workspace.exceptions import WorkspaceException
 
 
 class PhiWsData(BaseModel):
     """The PhiWsData model stores data for a phidata workspace."""
 
     # Name of the workspace
     ws_name: str
     # WorkspaceSchema: If exists then indicates that this ws has been authenticated
     # with the backend
     ws_schema: Optional[WorkspaceSchema] = None
     # The root directory for the workspace.
     # This field indicates that this ws has been downloaded on this machine
     ws_root_path: Optional[Path] = None
-    # Path for the WorkspaceConfig file
+    # DEPRECATED: Path for the WorkspaceConfig file
     ws_config_file_path: Optional[Path] = None
     # A Set of WorkspaceSetupActions which this workspace must satisfy to become valid.
     # if len(ws_data.required_actions.intersection(ws_data.pending_actions)) > 0:
     # the workspace is invalid
     required_actions: Set[WorkspaceSetupActions] = {
         WorkspaceSetupActions.WS_CONFIG_IS_AVL
     }
@@ -55,48 +55,36 @@
         """
         Returns the WorkspaceConfig for this workspace
         """
 
         if self.cached_ws_config is not None:
             return self.cached_ws_config
 
-        if self.ws_config_file_path is None or self.ws_root_path is None:
-            raise WorkspaceConfigException("WorkspaceConfig invalid")
+        if self.ws_root_path is None:
+            raise WorkspaceException("Workspace root not set")
 
         from phiterm.workspace.ws_loader import add_ws_dir_to_path, load_workspace
 
         # NOTE: When loading a workspace, relative imports or package imports dont work.
         # This is a known problem in python :(
         #     eg: https://stackoverflow.com/questions/6323860/sibling-package-imports/50193944#50193944
         # To make them work, we need to install the workspace as a python module
         #   But when we run `phi ws setup`, the ws module is not yet installed
         # So we add workspace_root to sys.path so is treated as a module
         add_ws_dir_to_path(self.ws_root_path)
 
         logger.debug(f"**--> Loading WorkspaceConfig")
-        ws_configs: List[WorkspaceConfig]
-        ws_configs = load_workspace(self.ws_config_file_path)
-
-        if is_empty(ws_configs):
-            logger.debug(f"No WorkspaceConfig found")
-            raise WorkspaceConfigException("No WorkspaceConfig found")
-
-        if len(ws_configs) > 1:
-            logger.warning(
-                "Found {} WorkspaceConfigs, first one will be selected".format(
-                    len(ws_configs)
-                )
-            )
+        loaded_config: WorkspaceConfig = load_workspace(ws_root_path=self.ws_root_path)
 
         # Update cached_ws_config
-        self.cached_ws_config = ws_configs[0]
+        self.cached_ws_config = loaded_config
         self.cached_ws_config.workspace_root_path = self.ws_root_path
         self.cached_ws_config.workspace_config_file_path = self.ws_config_file_path
 
-        # logger.debug("WorkspaceConfig:\n{}".format(self.cached_ws_config.args))
+        logger.debug("WorkspaceConfig:\n{}".format(self.cached_ws_config.args))
         return self.cached_ws_config
 
     ######################################################
     ## Print functions
     ######################################################
 
     def print_to_cli(self):
```

### Comparing `phiterm-1.5.9/phiterm/workspace/ws_enums.py` & `phiterm-1.6.0/phiterm/workspace/ws_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm/workspace/ws_operator.py` & `phiterm-1.6.0/phiterm/workspace/ws_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     print_subheading,
 )
 from phiterm.utils.log import logger
 from phiterm.workspace.ws_enums import (
     WorkspaceConfigType,
     WorkspaceStarterTemplate,
 )
-from phiterm.workspace.exceptions import WorkspaceConfigException
+from phiterm.workspace.exceptions import WorkspaceException
 
 # List of reserved workspace names
 RESERVED_WS_NAMES = ["root", "bedi", "ashpreet", "ashpreetbedi"]
 TEMPLATE_TO_NAME_MAP: Dict[WorkspaceStarterTemplate, str] = {
     WorkspaceStarterTemplate.ml_app: "ml-app",
     WorkspaceStarterTemplate.ai_app: "ai-app",
     WorkspaceStarterTemplate.duck_gpt: "duck-gpt",
@@ -56,18 +56,15 @@
     4. Provide the user with steps to add a remote origin for this workspace
 
     NOTE: till the user runs `phi ws setup` the workspace is not registered with phidata
         and can only be used locally
     """
     from shutil import copytree
     from phiterm.utils.filesystem import rmdir_recursive
-    from phiterm.workspace.ws_utils import (
-        get_ws_config_file_path,
-        get_ws_config_dir_path,
-    )
+    from phiterm.workspace.ws_utils import get_ws_config_dir_path
     from phiterm.utils.git import GitCloneProgress
 
     current_dir: Path = Path(".").resolve()
 
     # Phidata should be initialized before creating a workspace
     phi_conf: Optional[PhiConf] = PhiConf.get_saved_conf()
     if not phi_conf:
@@ -119,24 +116,17 @@
         try:
             _dot_git_exists = not rmdir_recursive(_dot_git_folder)
         except Exception as e:
             logger.warning(f"Failed to delete {_dot_git_folder}: {e}")
             logger.info("Please delete the .git folder manually")
             pass
 
-    # validate that a workspace config file exists
-    ws_config_file_path: Path = get_ws_config_file_path(ws_root_path)
-    if not (ws_config_file_path.exists() and ws_config_file_path.is_file()):
-        logger.error(f"Could not find workspace config at: {ws_config_file_path}")
-        return False
-
     phi_conf.add_new_ws_to_config(
         ws_name=ws_name,
         ws_root_path=ws_root_path,
-        ws_config_file_path=ws_config_file_path,
     )
 
     try:
         ws_config_dir_path: Path = get_ws_config_dir_path(ws_root_path)
         ws_config_secrets_dir = ws_config_dir_path.joinpath("secrets").resolve()
         ws_config_example_secrets_dir = ws_config_dir_path.joinpath(
             "example_secrets"
@@ -145,15 +135,17 @@
         print_info(f"Creating {str(ws_config_secrets_dir)}")
         copytree(
             str(ws_config_example_secrets_dir),
             str(ws_config_secrets_dir),
         )
     except Exception as e:
         logger.warning(f"Could not create workspace/secrets: {e}")
-        logger.warning("Please create the folder manually")
+        logger.warning(
+            "Please manually copy workspace/example_secrets to workspace/secrets"
+        )
 
     print_info(f"Your new workspace is available at {str(ws_root_path)}\n")
     return setup_workspace(ws_root_path=ws_root_path)
 
 
 def create_workspace_using_input():
     """Takes input from the user and calls create_new_workspace()"""
@@ -242,19 +234,15 @@
         Reaching here implies a all ws_data is available and updated.
         Validate the ws_data and print any pending setup actions.
 
     `phi ws setup` is a generic catch-all function. It should handle errors graciously
     and provide "how to fix" messages and "next steps" to get the user running.
     """
     from phiterm.utils.git import get_remote_origin_for_dir
-    from phiterm.workspace.ws_utils import (
-        get_ws_config_file_path,
-        is_valid_ws_config_file_path,
-        print_howtofix_pending_actions,
-    )
+    from phiterm.workspace.ws_utils import print_howtofix_pending_actions
 
     print_heading("Running workspace setup\n")
 
     ######################################################
     ## 1. Validate Pre-requisites
     ######################################################
     ######################################################
@@ -281,31 +269,25 @@
     logger.debug(f"Checking for a workspace at {ws_root_path}")
     ws_data: Optional[PhiWsData] = phi_conf.get_ws_data_by_path(ws_root_path)
     if ws_data is None:
         # This happens if
         # - The user is setting up an existing workspace
         # - the user ran `phi init -r` which erases the self._path_to_ws_data_map
         logger.debug(f"Could not find an existing workspace at path: {ws_root_path}")
-        # We'll try to parse this workspace using the workspace config
-        # validate that a workspace config file exists
-        __ws_config_file_path: Path = get_ws_config_file_path(ws_root_path)
 
         # In this case, the local workspace directory exists but PhiConf does not have a record
         print_info(f"Adding {ws_root_path} as a workspace")
         phi_conf.add_new_ws_to_config(
             ws_name=ws_root_path.stem,
             ws_root_path=ws_root_path,
-            ws_config_file_path=__ws_config_file_path,
         )
         ws_data = phi_conf.get_ws_data_by_path(ws_root_path)
         # If the ws_data is still none it means the workspace has bad data in it
         if ws_data is None:
-            logger.error(f"Could not create workspace")
-            print_info(f"Workspace Dir     : {ws_root_path}")
-            print_info(f"Workspace Config   : {__ws_config_file_path}")
+            logger.error(f"Could not add workspace from: {ws_root_path}")
             logger.error("Please try again")
             return False
     else:
         logger.debug(f"Found workspace {ws_data.ws_name}")
         phi_conf.refresh_ws_config(ws_data.ws_name)
 
     ######################################################
@@ -377,36 +359,25 @@
     ws_data = cast(PhiWsData, phi_conf.get_ws_data_by_name(ws_data.ws_name))
 
     ######################################################
     ## 3. Complete Workspace setup
     ######################################################
 
     ######################################################
-    # 3.1 Validate ws_config_file_path
-    ######################################################
-    _ws_config_file_path: Optional[Path] = ws_data.ws_config_file_path
-    if not is_valid_ws_config_file_path(_ws_config_file_path):
-        logger.error("Could not validate workspace config")
-        return False
-    logger.debug("--> Workspace config is valid")
-
-    ######################################################
-    # 3.2 Validate PhiWsData
+    # 3.1 Validate PhiWsData
     ######################################################
     ws_is_valid, pending_actions = phi_conf.validate_workspace(ws_name=ws_data.ws_name)
 
     if ws_is_valid and ws_data.ws_config is not None:
         scripts_dir = ws_data.ws_config.scripts_dir
         install_deps_file = f"sh {ws_root_path}/{scripts_dir}/install.sh"
         print_subheading(f"Setup complete! Next steps:\n")
         print_info("1. Deploy workspace:")
         print_info("\tphi ws up")
-        print_info("2. Update workspace config:")
-        print_info(f"\t{str(_ws_config_file_path)}")
-        print_info("3. Install workspace dependencies:")
+        print_info("2. Install workspace dependencies:")
         print_info(f"\t{install_deps_file}")
         # if pending_actions and len(pending_actions) > 0:
         #     print_info("3. Complete pending actions:")
         #     print_howtofix_pending_actions(pending_actions)
         return True
     else:
         print_info(f"Workspace setup pending.")
@@ -510,15 +481,15 @@
     auto_confirm: Optional[bool] = False,
 ) -> None:
     """Deploy a Phidata Workspace. This is called from `phi ws up`"""
     from phidata.docker.config import DockerConfig
     from phidata.k8s.config import K8sConfig
     from phidata.aws.config import AwsConfig
 
-    if ws_data is None or ws_data.ws_config is None:
+    if ws_data is None is None:
         logger.error("WorkspaceConfig invalid")
         return
 
     ws_config: WorkspaceConfig = ws_data.ws_config
     # Set the local environment variables before processing configs
     ws_config.set_local_env()
 
@@ -591,15 +562,15 @@
     auto_confirm: Optional[bool] = False,
 ) -> None:
     """Shutdown the Phidata Workspace. This is called from `phi ws down`"""
     from phidata.docker.config import DockerConfig
     from phidata.k8s.config import K8sConfig
     from phidata.aws.config import AwsConfig
 
-    if ws_data is None or ws_data.ws_config is None:
+    if ws_data is None is None:
         logger.error("WorkspaceConfig invalid")
         return
 
     ws_config: WorkspaceConfig = ws_data.ws_config
     # Set the local environment variables before processing configs
     ws_config.set_local_env()
 
@@ -674,15 +645,15 @@
     auto_confirm: Optional[bool] = False,
 ) -> None:
     """Patch the Phidata Workspace. This is called from `phi ws patch`"""
     from phidata.docker.config import DockerConfig
     from phidata.k8s.config import K8sConfig
     from phidata.aws.config import AwsConfig
 
-    if ws_data is None or ws_data.ws_config is None:
+    if ws_data is None is None:
         logger.error("WorkspaceConfig invalid")
         return
 
     ws_config: WorkspaceConfig = ws_data.ws_config
     # Set the local environment variables before processing configs
     ws_config.set_local_env()
 
@@ -795,15 +766,15 @@
         return False
 
     new_active_ws_name: str = active_ws_data.ws_name
     print_heading(f"Setting workspace {new_active_ws_name} as active")
     if refresh:
         try:
             phi_conf.refresh_ws_config(new_active_ws_name)
-        except WorkspaceConfigException as e:
+        except WorkspaceException as e:
             logger.error(
                 "Could not refresh workspace config, please fix errors and try again"
             )
             logger.error(e)
             return False
 
     ######################################################
@@ -863,15 +834,15 @@
     auto_confirm: Optional[bool] = False,
 ) -> None:
     """Print the Workspace status. This is called from `phi ws status`"""
     from phidata.docker.config import DockerConfig
     from phidata.k8s.config import K8sConfig
     from phidata.aws.config import AwsConfig
 
-    if ws_data is None or ws_data.ws_config is None:
+    if ws_data is None is None:
         logger.error("WorkspaceConfig invalid")
         return
 
     ws_config: WorkspaceConfig = ws_data.ws_config
     # Set the local environment variables before processing configs
     ws_config.set_local_env()
```

### Comparing `phiterm-1.5.9/phiterm/workspace/ws_schemas.py` & `phiterm-1.6.0/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/phiterm.egg-info/SOURCES.txt` & `phiterm-1.6.0/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.5.9/pyproject.toml` & `phiterm-1.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.5.9"
+version = "1.6.0"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

