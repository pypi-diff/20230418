# Comparing `tmp/hcs-cli-0.1.29.tar.gz` & `tmp/hcs-cli-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-cli-0.1.29.tar", last modified: Mon Apr 17 21:14:58 2023, max compression
+gzip compressed data, was "hcs-cli-0.1.30.tar", last modified: Tue Apr 18 00:06:34 2023, max compression
```

## Comparing `hcs-cli-0.1.29.tar` & `hcs-cli-0.1.30.tar`

### file list

```diff
@@ -1,129 +1,131 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.214221 hcs-cli-0.1.29/
--rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.29/.gitignore
--rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-07 18:36:38.000000 hcs-cli-0.1.29/CHANGELOG.md
--rw-r--r--   0 nanw       (501) staff       (20)      729 2023-04-17 20:42:14.000000 hcs-cli-0.1.29/Makefile
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-17 21:14:58.213666 hcs-cli-0.1.29/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-11 01:01:20.000000 hcs-cli-0.1.29/README.md
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.104380 hcs-cli-0.1.29/hcs_cli.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-17 21:14:57.000000 hcs-cli-0.1.29/hcs_cli.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     2804 2023-04-17 21:14:58.000000 hcs-cli-0.1.29/hcs_cli.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-17 21:14:57.000000 hcs-cli-0.1.29/hcs_cli.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-17 21:14:57.000000 hcs-cli-0.1.29/hcs_cli.egg-info/entry_points.txt
--rw-r--r--   0 nanw       (501) staff       (20)      168 2023-04-17 21:14:57.000000 hcs-cli-0.1.29/hcs_cli.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-17 21:14:57.000000 hcs-cli-0.1.29/hcs_cli.egg-info/top_level.txt
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.076564 hcs-cli-0.1.29/payload/
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.105369 hcs-cli-0.1.29/payload/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-11 00:40:07.000000 hcs-cli-0.1.29/payload/lcm/zero.json
--rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.29/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      168 2023-04-17 20:59:09.000000 hcs-cli-0.1.29/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-17 21:14:58.214354 hcs-cli-0.1.29/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      545 2023-04-17 21:14:53.000000 hcs-cli-0.1.29/setup.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.107544 hcs-cli-0.1.29/tests/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:50.000000 hcs-cli-0.1.29/tests/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:42.000000 hcs-cli-0.1.29/tests/conftest.py
--rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-08 01:06:36.000000 hcs-cli-0.1.29/tests/test_utils.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.108685 hcs-cli-0.1.29/tests/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:35.000000 hcs-cli-0.1.29/tests/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.109779 hcs-cli-0.1.29/tests/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:38.000000 hcs-cli-0.1.29/tests/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.114317 hcs-cli-0.1.29/tests/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:39.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.116570 hcs-cli-0.1.29/tests/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:41.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 21:57:30.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-08 01:06:36.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/test_auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-08 01:06:36.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/test_context.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-08 01:16:54.000000 hcs-cli-0.1.29/tests/vhcs/cli/cmds/test_profile.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.117448 hcs-cli-0.1.29/vhcs/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.29/vhcs/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.119222 hcs-cli-0.1.29/vhcs/cli/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/cli/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.123858 hcs-cli-0.1.29/vhcs/cli/cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/cli/cmds/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.124966 hcs-cli-0.1.29/vhcs/cli/cmds/admin/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-10 16:58:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.129598 hcs-cli-0.1.29/vhcs/cli/cmds/admin/edge/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:21:00.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/edge/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      341 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/edge/get.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-10 16:21:00.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/edge/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.135816 hcs-cli-0.1.29/vhcs/cli/cmds/admin/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:20:13.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      349 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)     1235 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/admin/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.29/vhcs/cli/cmds/auth.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.140051 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.144993 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/provider/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/provider/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/provider/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/provider/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      382 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/provider/list.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.153213 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/
--rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1257 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/create.py
--rw-r--r--   0 nanw       (501) staff       (20)      474 2023-04-11 00:46:01.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/delete.py
--rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-11 23:21:14.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/get.py
--rw-r--r--   0 nanw       (501) staff       (20)      957 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/list.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/wait.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.29/vhcs/cli/cmds/lcm/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.160779 hcs-cli-0.1.29/vhcs/cli/cmds/pki/
--rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/delete_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/get_org_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/get_root_ca.py
--rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/sign_resource_cert.py
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.29/vhcs/cli/cmds/pki/test.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.163422 hcs-cli-0.1.29/vhcs/cli/cmds/profile/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/cli/cmds/profile/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3840 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/cli/cmds/profile/init.py
--rw-r--r--   0 nanw       (501) staff       (20)      171 2023-04-17 21:14:07.000000 hcs-cli-0.1.29/vhcs/cli/cmds/test.py
--rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.29/vhcs/cli/cmds/upgrade.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.170119 hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/
--rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/redeem-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/request-otp.py
--rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/test.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2413 2023-04-17 21:01:02.000000 hcs-cli-0.1.29/vhcs/cli/main.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.172582 hcs-cli-0.1.29/vhcs/common/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.186532 hcs-cli-0.1.29/vhcs/common/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/ctxp/README.md
--rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-10 18:35:40.000000 hcs-cli-0.1.29/vhcs/common/ctxp/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.190881 hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-07 23:54:52.000000 hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     1819 2023-04-17 21:08:13.000000 hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     4139 2023-04-11 23:07:45.000000 hcs-cli-0.1.29/vhcs/common/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/ctxp/cli_state.py
--rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.29/vhcs/common/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.29/vhcs/common/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-07 00:18:58.000000 hcs-cli-0.1.29/vhcs/common/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)      548 2023-04-07 16:49:23.000000 hcs-cli-0.1.29/vhcs/common/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     3954 2023-04-17 21:10:37.000000 hcs-cli-0.1.29/vhcs/common/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     2157 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/common/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.29/vhcs/common/ctxp/var_template.py
--rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.29/vhcs/common/logger.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.198389 hcs-cli-0.1.29/vhcs/common/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/common/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.29/vhcs/common/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.29/vhcs/common/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     3853 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/common/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-07 19:17:10.000000 hcs-cli-0.1.29/vhcs/common/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-10 18:29:50.000000 hcs-cli-0.1.29/vhcs/common/sglib/util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.201035 hcs-cli-0.1.29/vhcs/config/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/config/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.29/vhcs/config/hcs-deployments.yaml
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.207460 hcs-cli-0.1.29/vhcs/service/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/service/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      985 2023-04-17 21:09:33.000000 hcs-cli-0.1.29/vhcs/service/_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      823 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/service/admin.py
--rw-r--r--   0 nanw       (501) staff       (20)     3194 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/service/lcm.py
--rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-07 21:33:14.000000 hcs-cli-0.1.29/vhcs/service/pki.py
--rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-07 19:31:02.000000 hcs-cli-0.1.29/vhcs/service/vmhub.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-17 21:14:58.212862 hcs-cli-0.1.29/vhcs/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/util/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     2159 2023-04-17 20:32:30.000000 hcs-cli-0.1.29/vhcs/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.29/vhcs/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-04-10 19:16:42.000000 hcs-cli-0.1.29/vhcs/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)      832 2023-04-07 19:01:08.000000 hcs-cli-0.1.29/vhcs/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.961171 hcs-cli-0.1.30/
+-rw-r--r--   0 nanw       (501) staff       (20)     2820 2023-01-11 22:10:27.000000 hcs-cli-0.1.30/.gitignore
+-rw-r--r--   0 nanw       (501) staff       (20)       82 2023-04-07 18:36:38.000000 hcs-cli-0.1.30/CHANGELOG.md
+-rw-r--r--   0 nanw       (501) staff       (20)      825 2023-04-18 00:06:30.000000 hcs-cli-0.1.30/Makefile
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-18 00:06:34.960642 hcs-cli-0.1.30/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1486 2023-04-11 01:01:20.000000 hcs-cli-0.1.30/README.md
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.865810 hcs-cli-0.1.30/hcs_cli.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     2256 2023-04-18 00:06:34.000000 hcs-cli-0.1.30/hcs_cli.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     2856 2023-04-18 00:06:34.000000 hcs-cli-0.1.30/hcs_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2023-04-18 00:06:34.000000 hcs-cli-0.1.30/hcs_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       43 2023-04-18 00:06:34.000000 hcs-cli-0.1.30/hcs_cli.egg-info/entry_points.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-18 00:06:34.000000 hcs-cli-0.1.30/hcs_cli.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       11 2023-04-18 00:06:34.000000 hcs-cli-0.1.30/hcs_cli.egg-info/top_level.txt
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.842285 hcs-cli-0.1.30/payload/
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.867138 hcs-cli-0.1.30/payload/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)      752 2023-04-11 00:40:07.000000 hcs-cli-0.1.30/payload/lcm/zero.json
+-rw-r--r--   0 nanw       (501) staff       (20)     1125 2023-04-07 16:11:06.000000 hcs-cli-0.1.30/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      127 2023-04-17 23:56:43.000000 hcs-cli-0.1.30/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2023-04-18 00:06:34.961369 hcs-cli-0.1.30/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      545 2023-04-17 22:59:55.000000 hcs-cli-0.1.30/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.869720 hcs-cli-0.1.30/tests/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:50.000000 hcs-cli-0.1.30/tests/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:01:42.000000 hcs-cli-0.1.30/tests/conftest.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2425 2023-04-08 01:06:36.000000 hcs-cli-0.1.30/tests/test_utils.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.871280 hcs-cli-0.1.30/tests/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:35.000000 hcs-cli-0.1.30/tests/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.872208 hcs-cli-0.1.30/tests/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:38.000000 hcs-cli-0.1.30/tests/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.876412 hcs-cli-0.1.30/tests/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:39.000000 hcs-cli-0.1.30/tests/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.878699 hcs-cli-0.1.30/tests/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 22:02:41.000000 hcs-cli-0.1.30/tests/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-07 21:57:30.000000 hcs-cli-0.1.30/tests/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)      290 2023-04-08 01:06:36.000000 hcs-cli-0.1.30/tests/vhcs/cli/cmds/test_auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1343 2023-04-08 01:06:36.000000 hcs-cli-0.1.30/tests/vhcs/cli/cmds/test_context.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-08 01:16:54.000000 hcs-cli-0.1.30/tests/vhcs/cli/cmds/test_profile.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.879652 hcs-cli-0.1.30/vhcs/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 21:25:27.000000 hcs-cli-0.1.30/vhcs/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.881313 hcs-cli-0.1.30/vhcs/cli/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/cli/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.886431 hcs-cli-0.1.30/vhcs/cli/cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/cli/cmds/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.887997 hcs-cli-0.1.30/vhcs/cli/cmds/admin/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-10 16:58:33.000000 hcs-cli-0.1.30/vhcs/cli/cmds/admin/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.891908 hcs-cli-0.1.30/vhcs/cli/cmds/admin/edge/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:21:00.000000 hcs-cli-0.1.30/vhcs/cli/cmds/admin/edge/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      341 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/cli/cmds/admin/edge/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-10 16:21:00.000000 hcs-cli-0.1.30/vhcs/cli/cmds/admin/edge/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.894989 hcs-cli-0.1.30/vhcs/cli/cmds/admin/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-10 16:20:13.000000 hcs-cli-0.1.30/vhcs/cli/cmds/admin/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      349 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/cli/cmds/admin/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1235 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/cli/cmds/admin/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)      375 2023-04-07 18:22:47.000000 hcs-cli-0.1.30/vhcs/cli/cmds/auth.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.897282 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.902233 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/provider/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      196 2023-04-07 18:26:01.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/provider/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      187 2023-04-07 18:26:21.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/provider/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      382 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/provider/list.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.908471 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/template/
+-rw-r--r--   0 nanw       (501) staff       (20)       28 2023-04-06 17:42:33.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/template/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1257 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/template/create.py
+-rw-r--r--   0 nanw       (501) staff       (20)      474 2023-04-11 00:46:01.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/template/delete.py
+-rw-r--r--   0 nanw       (501) staff       (20)      235 2023-04-11 23:21:14.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/template/get.py
+-rw-r--r--   0 nanw       (501) staff       (20)      957 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/template/list.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/template/wait.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:18:56.000000 hcs-cli-0.1.30/vhcs/cli/cmds/lcm/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.914484 hcs-cli-0.1.30/vhcs/cli/cmds/pki/
+-rw-r--r--   0 nanw       (501) staff       (20)       31 2023-04-06 17:42:33.000000 hcs-cli-0.1.30/vhcs/cli/cmds/pki/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      551 2023-04-07 18:26:57.000000 hcs-cli-0.1.30/vhcs/cli/cmds/pki/delete_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      297 2023-04-07 18:27:02.000000 hcs-cli-0.1.30/vhcs/cli/cmds/pki/get_org_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      163 2023-04-07 18:27:20.000000 hcs-cli-0.1.30/vhcs/cli/cmds/pki/get_root_ca.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1220 2023-04-06 22:12:04.000000 hcs-cli-0.1.30/vhcs/cli/cmds/pki/sign_resource_cert.py
+-rw-r--r--   0 nanw       (501) staff       (20)      106 2023-04-07 18:21:03.000000 hcs-cli-0.1.30/vhcs/cli/cmds/pki/test.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.916393 hcs-cli-0.1.30/vhcs/cli/cmds/profile/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/cli/cmds/profile/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3840 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/cli/cmds/profile/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)      171 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/cli/cmds/test.py
+-rw-r--r--   0 nanw       (501) staff       (20)      332 2023-04-07 18:23:32.000000 hcs-cli-0.1.30/vhcs/cli/cmds/upgrade.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.921471 hcs-cli-0.1.30/vhcs/cli/cmds/vmhub/
+-rw-r--r--   0 nanw       (501) staff       (20)       33 2023-04-06 17:42:33.000000 hcs-cli-0.1.30/vhcs/cli/cmds/vmhub/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      662 2023-04-07 18:27:15.000000 hcs-cli-0.1.30/vhcs/cli/cmds/vmhub/redeem-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      567 2023-04-07 18:27:38.000000 hcs-cli-0.1.30/vhcs/cli/cmds/vmhub/request-otp.py
+-rw-r--r--   0 nanw       (501) staff       (20)      110 2023-04-07 18:22:14.000000 hcs-cli-0.1.30/vhcs/cli/cmds/vmhub/test.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2264 2023-04-17 23:56:08.000000 hcs-cli-0.1.30/vhcs/cli/main.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.923534 hcs-cli-0.1.30/vhcs/common/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/common/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.937622 hcs-cli-0.1.30/vhcs/common/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)     1839 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/common/ctxp/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)      107 2023-04-17 22:17:15.000000 hcs-cli-0.1.30/vhcs/common/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      611 2023-04-17 22:48:15.000000 hcs-cli-0.1.30/vhcs/common/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.939867 hcs-cli-0.1.30/vhcs/common/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/common/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1419 2023-04-07 23:54:52.000000 hcs-cli-0.1.30/vhcs/common/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1819 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/common/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4141 2023-04-17 23:56:31.000000 hcs-cli-0.1.30/vhcs/common/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-17 22:10:00.000000 hcs-cli-0.1.30/vhcs/common/ctxp/cli_state.py
+-rw-r--r--   0 nanw       (501) staff       (20)      337 2023-04-07 00:28:47.000000 hcs-cli-0.1.30/vhcs/common/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1656 2023-04-07 00:28:55.000000 hcs-cli-0.1.30/vhcs/common/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5680 2023-04-17 22:58:19.000000 hcs-cli-0.1.30/vhcs/common/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)      600 2023-04-17 22:29:42.000000 hcs-cli-0.1.30/vhcs/common/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2128 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/common/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3951 2023-04-17 22:58:19.000000 hcs-cli-0.1.30/vhcs/common/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)      876 2023-04-17 22:58:19.000000 hcs-cli-0.1.30/vhcs/common/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2157 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/common/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2633 2023-04-07 00:29:18.000000 hcs-cli-0.1.30/vhcs/common/ctxp/var_template.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4246 2023-04-07 00:37:01.000000 hcs-cli-0.1.30/vhcs/common/logger.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.944453 hcs-cli-0.1.30/vhcs/common/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)       54 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/common/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2504 2023-04-07 00:18:58.000000 hcs-cli-0.1.30/vhcs/common/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3601 2023-04-07 00:18:58.000000 hcs-cli-0.1.30/vhcs/common/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3853 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/common/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      549 2023-04-07 19:17:10.000000 hcs-cli-0.1.30/vhcs/common/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      370 2023-04-10 18:29:50.000000 hcs-cli-0.1.30/vhcs/common/sglib/util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.946518 hcs-cli-0.1.30/vhcs/config/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/config/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7327 2023-04-06 17:22:27.000000 hcs-cli-0.1.30/vhcs/config/hcs-deployments.yaml
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.952321 hcs-cli-0.1.30/vhcs/service/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/service/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      986 2023-04-17 22:58:19.000000 hcs-cli-0.1.30/vhcs/service/_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)      823 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/service/admin.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3194 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/service/lcm.py
+-rw-r--r--   0 nanw       (501) staff       (20)      610 2023-04-07 21:33:14.000000 hcs-cli-0.1.30/vhcs/service/pki.py
+-rw-r--r--   0 nanw       (501) staff       (20)      929 2023-04-07 19:31:02.000000 hcs-cli-0.1.30/vhcs/service/vmhub.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2023-04-18 00:06:34.959228 hcs-cli-0.1.30/vhcs/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/util/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2159 2023-04-17 22:12:13.000000 hcs-cli-0.1.30/vhcs/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4699 2023-04-06 02:05:21.000000 hcs-cli-0.1.30/vhcs/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1127 2023-04-10 19:16:42.000000 hcs-cli-0.1.30/vhcs/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1126 2023-04-17 23:57:58.000000 hcs-cli-0.1.30/vhcs/util/versions.py
```

### Comparing `hcs-cli-0.1.29/.gitignore` & `hcs-cli-0.1.30/.gitignore`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/Makefile` & `hcs-cli-0.1.30/Makefile`

 * *Files 23% similar despite different names*

```diff
@@ -29,18 +29,21 @@
 
 dev: clean uninstall lint build devinstall
 
 SHELL := /bin/bash
 test:
 	python3 -m unittest discover ./tests
 
+testinstall:
+	docker run python /bin/bash -c "pip3 install hcs-cli && hcs profile"
+
 publish:
 	twine upload dist/*
 
 install:
 	pip3 install hcs-cli
 
 wait:
 	sleep 30
 
-release: clean buildrelease publish uninstall wait install
+release: clean buildrelease publish uninstall testinstall wait install
```

### Comparing `hcs-cli-0.1.29/PKG-INFO` & `hcs-cli-0.1.30/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.29
+Version: 0.1.30
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.29/README.md` & `hcs-cli-0.1.30/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/hcs_cli.egg-info/PKG-INFO` & `hcs-cli-0.1.30/hcs_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-cli
-Version: 0.1.29
+Version: 0.1.30
 Summary: Horizon Cloud Service CLI
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/nanw1103/hcs-cli
 Project-URL: Bug Tracker, https://github.com/nanw1103/hcs-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/nanw1103/hcs-cli
 Project-URL: changelog, https://github.com/nanw1103/hcs-cli/blob/master/CHANGELOG.md
```

### Comparing `hcs-cli-0.1.29/hcs_cli.egg-info/SOURCES.txt` & `hcs-cli-0.1.30/hcs_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -61,22 +61,24 @@
 vhcs/cli/cmds/vmhub/redeem-otp.py
 vhcs/cli/cmds/vmhub/request-otp.py
 vhcs/cli/cmds/vmhub/test.py
 vhcs/common/__init__.py
 vhcs/common/logger.py
 vhcs/common/ctxp/README.md
 vhcs/common/ctxp/__init__.py
+vhcs/common/ctxp/_init.py
 vhcs/common/ctxp/cli_processor.py
 vhcs/common/ctxp/cli_state.py
 vhcs/common/ctxp/config.py
 vhcs/common/ctxp/context.py
 vhcs/common/ctxp/fstore.py
 vhcs/common/ctxp/init.py
 vhcs/common/ctxp/jsondot.py
 vhcs/common/ctxp/profile.py
+vhcs/common/ctxp/state.py
 vhcs/common/ctxp/util.py
 vhcs/common/ctxp/var_template.py
 vhcs/common/ctxp/built_in_cmds/__init__.py
 vhcs/common/ctxp/built_in_cmds/context.py
 vhcs/common/ctxp/built_in_cmds/profile.py
 vhcs/common/sglib/__init__.py
 vhcs/common/sglib/auth.py
```

### Comparing `hcs-cli-0.1.29/payload/lcm/zero.json` & `hcs-cli-0.1.30/payload/lcm/zero.json`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/pyproject.toml` & `hcs-cli-0.1.30/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/setup.py` & `hcs-cli-0.1.30/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools_scm import get_version
 import os
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-VERSION = "0.1.29"
+VERSION = "0.1.30"
 
 
 def get_version():
     version = VERSION
     local_version = os.environ.get("SCM_REV")
     if local_version:
         version += "+" + local_version
```

### Comparing `hcs-cli-0.1.29/tests/test_utils.py` & `hcs-cli-0.1.30/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/tests/vhcs/cli/cmds/test_context.py` & `hcs-cli-0.1.30/tests/vhcs/cli/cmds/test_context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/tests/vhcs/cli/cmds/test_profile.py` & `hcs-cli-0.1.30/tests/vhcs/cli/cmds/test_profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/cli/cmds/admin/template/list.py` & `hcs-cli-0.1.30/vhcs/cli/cmds/admin/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/create.py` & `hcs-cli-0.1.30/vhcs/cli/cmds/lcm/template/create.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/list.py` & `hcs-cli-0.1.30/vhcs/cli/cmds/lcm/template/list.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/cli/cmds/lcm/template/wait.py` & `hcs-cli-0.1.30/vhcs/cli/cmds/lcm/template/wait.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/cli/cmds/pki/delete_org_cert.py` & `hcs-cli-0.1.30/vhcs/cli/cmds/pki/delete_org_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/cli/cmds/pki/sign_resource_cert.py` & `hcs-cli-0.1.30/vhcs/cli/cmds/pki/sign_resource_cert.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/cli/cmds/profile/init.py` & `hcs-cli-0.1.30/vhcs/cli/cmds/profile/init.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/redeem-otp.py` & `hcs-cli-0.1.30/vhcs/cli/cmds/vmhub/redeem-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/cli/cmds/vmhub/request-otp.py` & `hcs-cli-0.1.30/vhcs/cli/cmds/vmhub/request-otp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/cli/main.py` & `hcs-cli-0.1.30/vhcs/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 _script_dir = path.abspath(path.join(path.dirname(path.realpath(__file__)), "."))
 _module_dir = path.dirname(_script_dir)
 if __name__ == "__main__":
     _cli_dir = path.dirname(_module_dir)
     sys.path.append(_cli_dir)
 
 import vhcs.common.ctxp as ctxp
-from vhcs.common.ctxp.util import option_output, option_verbose, option_field
+from vhcs.common.ctxp.util import option_output, option_verbose, option_field, panic, CtxpException
 
 # -----------------------------------------------------------
 import vhcs.common.logger as logger
 
 logger.setup()
 logging.getLogger("charset_normalizer").setLevel(logging.WARN)
 logging.getLogger("csp").setLevel(logging.INFO)
@@ -34,46 +34,40 @@
 @option_verbose
 @option_output
 @option_field
 @click.option("--profile", "-p", type=str, required=False, help="Specify the profile to use. Optional.")
 @click.option("--upgrade-check/--no-upgrade-check", default=True, help="Check new version of HCS CLI.")
 @click.option("--telemetry/--no-telemetry", default=True, help="Send telemetry")
 def cli(**kwargs):
-
     upgrade_check = kwargs.get("upgrade_check")
     if upgrade_check:
         from vhcs.util.versions import check_upgrade
 
         check_upgrade()
 
     profile = kwargs.get("profile")
     if profile:
         ctxp.profile._active_profile_name = profile
 
 
-# @cli.result_callback()
-# def _process_result(result, **kwargs):
-#     print("_process_result", result, kwargs)
-#     pass
-
-
 def main():
     try:
         commands_dir = path.join(_module_dir, "cli/cmds")
         config_path = path.join(_module_dir, "config")
         ctxp.init(cli_name="hcs", main_cli=cli, commands_dir=commands_dir, config_path=config_path)
-    except ctxp.CtxpException as e:
-        ctxp.panic(e)
+    except CtxpException as e:
+        panic(e)
     except httpx.HTTPStatusError as e:
-        import traceback
+        _on_http_error(e)
 
-        traceback.print_exc()
-        try:
-            err = json.loads(e.response.text)
-        except:
-            err = {"message": str(e), "response": e.response.text, "resource": str(e.request.url)}
-        text = json.dumps(err, indent=4)
-        ctxp.panic(text)
+
+def _on_http_error(e):
+    try:
+        err = json.loads(e.response.text)
+    except:
+        err = {"message": str(e), "response": e.response.text, "resource": str(e.request.url)}
+    text = json.dumps(err, indent=4)
+    panic(text)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/README.md` & `hcs-cli-0.1.30/vhcs/common/ctxp/README.md`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/context.py` & `hcs-cli-0.1.30/vhcs/common/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/built_in_cmds/profile.py` & `hcs-cli-0.1.30/vhcs/common/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/cli_processor.py` & `hcs-cli-0.1.30/vhcs/common/ctxp/cli_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import yaml
 from click.core import Group
 import os.path as path
 import os
 import importlib
 import importlib.util
 from pathlib import Path
-from . import util
+from .util import print_output
 
 _eager_loading = os.environ.get("_CTXP_EAGER_LOAD")
 if _eager_loading:
     print("_CTXP_EAGER_LOAD:", _eager_loading, file=sys.stderr)
 
 
 class LazyGroup(click.Group):
@@ -108,22 +108,22 @@
 
 
 def _process_result(result, **kwargs):
     if result is not None:
         if isinstance(result, tuple):
             data, return_code = result
             if data is not None:
-                util.print_output(data, kwargs.get("output"), kwargs.get("field"))
+                print_output(data, kwargs.get("output"), kwargs.get("field"))
             if isinstance(return_code, int):
                 ctx = click.get_current_context()
                 ctx.exit(return_code)
             else:
                 raise Exception("Invalid command return code. Expect int, actual=" + str(type(return_code)))
         else:
-            util.print_output(result, kwargs.get("output"), kwargs.get("field"))
+            print_output(result, kwargs.get("output"), kwargs.get("field"))
 
 
 def init(main_cli: click.Group, commands_dir: str):
     _add_built_in_commands(main_cli)
     _add_subcommands(commands_dir, main_cli)
     main_cli.result_callback()(_process_result)
     return main_cli(obj={})
```

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/context.py` & `hcs-cli-0.1.30/vhcs/common/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/fstore.py` & `hcs-cli-0.1.30/vhcs/common/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/init.py` & `hcs-cli-0.1.30/vhcs/common/ctxp/init.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 from os import path
 from pathlib import Path
 from . import profile
+from . import state
 from . import config
 from . import cli_processor
 
 user_home = str(Path.home())
 
 
 def init(
@@ -15,9 +16,10 @@
     store_path: str = user_home,
     config_path="./config",
 ):
     real_store_path = path.join(store_path, "." + cli_name)
     profile_path = path.join(real_store_path, "profile")
     profile.init(profile_path)
     config._init(config_path)
+    state.init(real_store_path)
 
     return cli_processor.init(main_cli, commands_dir)
```

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/jsondot.py` & `hcs-cli-0.1.30/vhcs/common/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/profile.py` & `hcs-cli-0.1.30/vhcs/common/ctxp/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from .util import CtxpException, panic
 from .jsondot import dotdict
 from .fstore import fstore
 
-
 _store: fstore = None
 _active_profile_name: str = None
 _plain: dotdict = None
 
 _active_profile_store_item = ".active"
 
 
@@ -26,15 +25,15 @@
 
 
 def create(name: str, data: dict) -> None:
     _store.save(name, data)
     use(name)
 
 
-def current(reload: bool = False, exit_on_failure = True) -> dict:
+def current(reload: bool = False, exit_on_failure=True) -> dict:
     """Get content of the current active profile"""
     profile_name = name()
     if not profile_name:
         raise CtxpException("Profile not specified")
     data = get(profile_name, reload)
     global _plain
     _plain = None
```

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/util.py` & `hcs-cli-0.1.30/vhcs/common/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/ctxp/var_template.py` & `hcs-cli-0.1.30/vhcs/common/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/logger.py` & `hcs-cli-0.1.30/vhcs/common/logger.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/sglib/auth.py` & `hcs-cli-0.1.30/vhcs/common/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/sglib/csp.py` & `hcs-cli-0.1.30/vhcs/common/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/sglib/ez_client.py` & `hcs-cli-0.1.30/vhcs/common/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/common/sglib/hcs_client.py` & `hcs-cli-0.1.30/vhcs/common/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/config/hcs-deployments.yaml` & `hcs-cli-0.1.30/vhcs/config/hcs-deployments.yaml`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/service/_util.py` & `hcs-cli-0.1.30/vhcs/service/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from vhcs.common.ctxp import profile, panic
 from vhcs.common.sglib import hcs_client
 
+
 def hdc_service_client(service_name: str):
     url = profile.current().hcs.url
     if not url.endswith("/"):
         url += "/"
     url += service_name
     return hcs_client(url)
```

### Comparing `hcs-cli-0.1.29/vhcs/service/admin.py` & `hcs-cli-0.1.30/vhcs/service/admin.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/service/lcm.py` & `hcs-cli-0.1.30/vhcs/service/lcm.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/service/pki.py` & `hcs-cli-0.1.30/vhcs/service/pki.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/service/vmhub.py` & `hcs-cli-0.1.30/vhcs/service/vmhub.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/util/duration.py` & `hcs-cli-0.1.30/vhcs/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/util/pki_util.py` & `hcs-cli-0.1.30/vhcs/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/util/query_util.py` & `hcs-cli-0.1.30/vhcs/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-cli-0.1.29/vhcs/util/versions.py` & `hcs-cli-0.1.30/vhcs/util/versions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import logging
 import httpx
+import time
+import vhcs.common.ctxp as ctxp
 
 import pkg_resources
 from packaging.version import Version
 
 log = logging.getLogger(__name__)
 
+def check_upgrade():
+    last_upgrade_check_at = "last_upgrade_check_at"
+    checked_at = ctxp.state.get(last_upgrade_check_at, 0)
+
+    now = time.time()
+    if now - checked_at > 24 * 60 * 60:
+        try:
+            latest = get_latest_version()
+            current = Version(get_version())
+            if current < latest:
+                log.warning(f"New version available: {latest}. Execute 'hcs upgrade' to upgrade.")
+        except Exception as e:
+            logging.debug(e)
+    
+    ctxp.state.set(last_upgrade_check_at, now)
 
 def get_version():
     return pkg_resources.require("hcs-cli")[0].version
 
-
-def check_upgrade():
-    try:
-        latest = get_latest_version()
-        current = Version(get_version())
-        if current < latest:
-            log.warning(f"New version available: {latest}. Execute 'hcs upgrade' to upgrade.")
-    except Exception as e:
-        logging.debug(e)
-
-
 def get_latest_version() -> Version:
     res = httpx.get("https://pypi.org/pypi/hcs-cli/json")
     names = res.json().get("releases").keys()
     versions = [Version(n) for n in names]
     versions.sort(reverse=True)
     return versions[0]
```

