# Comparing `tmp/pros-cli-3.4.1.tar.gz` & `tmp/pros-cli-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pros-cli-3.4.1.tar", last modified: Tue Nov 15 16:15:33 2022, max compression
+gzip compressed data, was "pros-cli-3.4.2.tar", last modified: Tue Apr 18 01:19:57 2023, max compression
```

## Comparing `pros-cli-3.4.1.tar` & `pros-cli-3.4.2.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.396540 pros-cli-3.4.1/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)    16725 2021-12-20 01:03:11.000000 pros-cli-3.4.1/LICENSE
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      275 2022-11-15 16:15:33.396396 pros-cli-3.4.1/PKG-INFO
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1862 2021-12-20 01:03:11.000000 pros-cli-3.4.1/README.md
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.376202 pros-cli-3.4.1/pros/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)        0 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/__init__.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.379258 pros-cli-3.4.1/pros/cli/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)        0 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/cli/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     2873 2022-10-06 14:25:08.000000 pros-cli-3.4.1/pros/cli/build.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     5972 2022-11-14 09:50:52.000000 pros-cli-3.4.1/pros/cli/click_classes.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)    12809 2022-02-21 23:09:29.000000 pros-cli-3.4.1/pros/cli/common.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)    15181 2022-11-14 09:50:52.000000 pros-cli-3.4.1/pros/cli/conductor.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     8302 2022-02-21 23:09:29.000000 pros-cli-3.4.1/pros/cli/conductor_utils.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1454 2022-02-21 23:09:29.000000 pros-cli-3.4.1/pros/cli/interactive.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     3332 2022-11-14 09:50:52.000000 pros-cli-3.4.1/pros/cli/main.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1398 2022-06-14 17:33:46.000000 pros-cli-3.4.1/pros/cli/misc_commands.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     4485 2022-10-06 14:37:11.000000 pros-cli-3.4.1/pros/cli/terminal.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      369 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/cli/test.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     9685 2022-05-18 21:12:53.000000 pros-cli-3.4.1/pros/cli/upload.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      754 2022-02-21 23:09:29.000000 pros-cli-3.4.1/pros/cli/user_script.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)    10692 2022-10-06 14:37:11.000000 pros-cli-3.4.1/pros/cli/v5_utils.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.379755 pros-cli-3.4.1/pros/common/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      109 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     5218 2022-02-21 23:09:29.000000 pros-cli-3.4.1/pros/common/sentry.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.380056 pros-cli-3.4.1/pros/common/ui/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     6987 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/__init__.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.380714 pros-cli-3.4.1/pros/common/ui/interactive/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      859 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/ConfirmModal.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)        0 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     5007 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/application.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.381834 pros-cli-3.4.1/pros/common/ui/interactive/components/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      472 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/components/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      591 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/components/button.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      229 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/components/checkbox.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     2612 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/components/component.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1157 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/components/container.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      805 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/components/input.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      400 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/components/input_groups.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      599 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/components/label.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     3113 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/observable.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.382400 pros-cli-3.4.1/pros/common/ui/interactive/parameters/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      335 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/parameters/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1262 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/parameters/misc_parameters.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      702 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/parameters/parameter.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     2205 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/parameters/validatable_parameter.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.383176 pros-cli-3.4.1/pros/common/ui/interactive/renderers/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     3520 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/renderers/MachineOutputRenderer.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      691 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/renderers/Renderer.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)       57 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/interactive/renderers/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1781 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/common/ui/log.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     4701 2022-11-14 09:50:52.000000 pros-cli-3.4.1/pros/common/utils.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.383796 pros-cli-3.4.1/pros/conductor/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      265 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)    11642 2022-05-23 20:27:26.000000 pros-cli-3.4.1/pros/conductor/conductor.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.384515 pros-cli-3.4.1/pros/conductor/depots/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)       95 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/depots/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1946 2022-05-23 20:27:26.000000 pros-cli-3.4.1/pros/conductor/depots/depot.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1585 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/depots/http_depot.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     2366 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/depots/local_depot.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.385428 pros-cli-3.4.1/pros/conductor/interactive/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     2998 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/interactive/NewProjectModal.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     6239 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/interactive/UpdateProjectModal.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      175 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/interactive/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1846 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/interactive/components.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     5466 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/interactive/parameters.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.386138 pros-cli-3.4.1/pros/conductor/project/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      905 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/project/ProjectReport.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     7498 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/project/ProjectTransaction.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)    20072 2022-02-21 23:09:29.000000 pros-cli-3.4.1/pros/conductor/project/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      515 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/project/template_resolution.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.386915 pros-cli-3.4.1/pros/conductor/templates/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      161 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/templates/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     3963 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/templates/base_template.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      850 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/templates/external_template.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      635 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/templates/local_template.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      475 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/templates/template.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     3392 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/conductor/transaction.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.387375 pros-cli-3.4.1/pros/config/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)       63 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/config/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     2836 2022-02-21 23:09:29.000000 pros-cli-3.4.1/pros/config/cli_config.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     4764 2022-05-23 20:27:26.000000 pros-cli-3.4.1/pros/config/config.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.387748 pros-cli-3.4.1/pros/ga/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)        0 2022-05-18 23:08:37.000000 pros-cli-3.4.1/pros/ga/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     2364 2022-05-18 21:12:53.000000 pros-cli-3.4.1/pros/ga/analytics.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.388141 pros-cli-3.4.1/pros/jinx/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)        0 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/jinx/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      148 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/jinx/server.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.388307 pros-cli-3.4.1/pros/serial/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      471 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/__init__.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.389001 pros-cli-3.4.1/pros/serial/devices/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)       99 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      242 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/generic_device.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1034 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/stream_device.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      285 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/system_device.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.390948 pros-cli-3.4.1/pros/serial/devices/vex/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      218 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/vex/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      202 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/vex/comm_error.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     5989 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/vex/cortex_device.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      831 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/vex/crc.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1386 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/vex/message.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     7686 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/vex/stm32_device.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)    50297 2022-11-14 09:50:52.000000 pros-cli-3.4.1/pros/serial/devices/vex/v5_device.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1564 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/vex/v5_user_device.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     5294 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/devices/vex/vex_device.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.391276 pros-cli-3.4.1/pros/serial/interactive/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     7328 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/interactive/UploadProjectModal.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)       85 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/interactive/__init__.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.392858 pros-cli-3.4.1/pros/serial/ports/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      456 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/ports/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      689 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/ports/base_port.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     2497 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/ports/direct_port.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      560 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/ports/exceptions.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     8208 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/ports/serial_share_bridge.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     3389 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/ports/serial_share_port.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1222 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/ports/v5_wireless_port.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.393212 pros-cli-3.4.1/pros/serial/terminal/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)       31 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/terminal/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)    10518 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/serial/terminal/terminal.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.393554 pros-cli-3.4.1/pros/upgrade/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      176 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/upgrade/__init__.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.394644 pros-cli-3.4.1/pros/upgrade/instructions/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      347 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/upgrade/instructions/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      573 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/upgrade/instructions/base_instructions.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1336 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/upgrade/instructions/download_instructions.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      504 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/upgrade/instructions/explorer_instructions.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      321 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/upgrade/instructions/nothing_instructions.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.395207 pros-cli-3.4.1/pros/upgrade/manifests/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      307 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/upgrade/manifests/__init__.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     1419 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/upgrade/manifests/upgrade_manifest_v1.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     2614 2022-11-14 09:50:52.000000 pros-cli-3.4.1/pros/upgrade/manifests/upgrade_manifest_v2.py
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     3575 2021-12-20 01:03:11.000000 pros-cli-3.4.1/pros/upgrade/upgrade_manager.py
-drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2022-11-15 16:15:33.396163 pros-cli-3.4.1/pros_cli.egg-info/
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      275 2022-11-15 16:15:33.000000 pros-cli-3.4.1/pros_cli.egg-info/PKG-INFO
--rw-r--r--   0 kunwarsahni   (501) staff       (20)     3884 2022-11-15 16:15:33.000000 pros-cli-3.4.1/pros_cli.egg-info/SOURCES.txt
--rw-r--r--   0 kunwarsahni   (501) staff       (20)        1 2022-11-15 16:15:33.000000 pros-cli-3.4.1/pros_cli.egg-info/dependency_links.txt
--rw-r--r--   0 kunwarsahni   (501) staff       (20)       72 2022-11-15 16:15:33.000000 pros-cli-3.4.1/pros_cli.egg-info/entry_points.txt
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      165 2022-11-15 16:15:33.000000 pros-cli-3.4.1/pros_cli.egg-info/requires.txt
--rw-r--r--   0 kunwarsahni   (501) staff       (20)        5 2022-11-15 16:15:33.000000 pros-cli-3.4.1/pros_cli.egg-info/top_level.txt
--rw-r--r--   0 kunwarsahni   (501) staff       (20)       38 2022-11-15 16:15:33.396580 pros-cli-3.4.1/setup.cfg
--rw-r--r--   0 kunwarsahni   (501) staff       (20)      656 2021-12-20 01:03:11.000000 pros-cli-3.4.1/setup.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.954854 pros-cli-3.4.2/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)    16725 2021-12-20 01:03:11.000000 pros-cli-3.4.2/LICENSE
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      275 2023-04-18 01:19:57.954723 pros-cli-3.4.2/PKG-INFO
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1862 2021-12-20 01:03:11.000000 pros-cli-3.4.2/README.md
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.933464 pros-cli-3.4.2/pros/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)        0 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/__init__.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.935691 pros-cli-3.4.2/pros/cli/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)        0 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/cli/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     2873 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/cli/build.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     5972 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/cli/click_classes.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)    12809 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/cli/common.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)    16074 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/cli/conductor.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     8573 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/cli/conductor_utils.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1454 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/cli/interactive.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     3447 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/cli/main.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1398 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/cli/misc_commands.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     4566 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/cli/terminal.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      369 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/cli/test.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     9685 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/cli/upload.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      754 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/cli/user_script.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)    10832 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/cli/v5_utils.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.936156 pros-cli-3.4.2/pros/common/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      109 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     5218 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/common/sentry.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.936423 pros-cli-3.4.2/pros/common/ui/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     6987 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/__init__.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.937072 pros-cli-3.4.2/pros/common/ui/interactive/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      859 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/ConfirmModal.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)        0 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     5007 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/application.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.942101 pros-cli-3.4.2/pros/common/ui/interactive/components/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      472 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/components/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      591 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/components/button.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      229 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/components/checkbox.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     2612 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/components/component.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1157 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/components/container.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      805 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/components/input.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      400 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/components/input_groups.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      599 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/components/label.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     3113 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/observable.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.942646 pros-cli-3.4.2/pros/common/ui/interactive/parameters/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      335 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/parameters/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1262 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/parameters/misc_parameters.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      702 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/parameters/parameter.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     2205 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/parameters/validatable_parameter.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.943123 pros-cli-3.4.2/pros/common/ui/interactive/renderers/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     3520 2022-12-21 19:38:48.000000 pros-cli-3.4.2/pros/common/ui/interactive/renderers/MachineOutputRenderer.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      691 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/renderers/Renderer.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)       57 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/common/ui/interactive/renderers/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1781 2022-12-21 19:38:48.000000 pros-cli-3.4.2/pros/common/ui/log.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     4701 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/common/utils.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.943535 pros-cli-3.4.2/pros/conductor/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      265 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)    16329 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/conductor/conductor.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.944269 pros-cli-3.4.2/pros/conductor/depots/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)       95 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/depots/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1946 2023-04-11 18:47:45.000000 pros-cli-3.4.2/pros/conductor/depots/depot.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1795 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/conductor/depots/http_depot.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     2366 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/depots/local_depot.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.945001 pros-cli-3.4.2/pros/conductor/interactive/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     2998 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/interactive/NewProjectModal.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     6239 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/interactive/UpdateProjectModal.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      175 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/interactive/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1846 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/interactive/components.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     5466 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/interactive/parameters.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.945993 pros-cli-3.4.2/pros/conductor/project/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      905 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/project/ProjectReport.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     7498 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/project/ProjectTransaction.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)    20182 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/conductor/project/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      515 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/project/template_resolution.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.946716 pros-cli-3.4.2/pros/conductor/templates/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      161 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/templates/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     3963 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/templates/base_template.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      850 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/templates/external_template.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      635 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/templates/local_template.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      475 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/templates/template.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     3392 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/conductor/transaction.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.947116 pros-cli-3.4.2/pros/config/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)       63 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/config/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     2836 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/config/cli_config.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     4764 2022-05-23 20:27:26.000000 pros-cli-3.4.2/pros/config/config.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.947433 pros-cli-3.4.2/pros/ga/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)        0 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/ga/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     2971 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/ga/analytics.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.947660 pros-cli-3.4.2/pros/jinx/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)        0 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/jinx/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      148 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/jinx/server.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.947810 pros-cli-3.4.2/pros/serial/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      471 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/__init__.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.948373 pros-cli-3.4.2/pros/serial/devices/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)       99 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      242 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/generic_device.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1034 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/stream_device.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      285 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/system_device.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.950610 pros-cli-3.4.2/pros/serial/devices/vex/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      218 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/vex/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      202 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/vex/comm_error.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     5989 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/vex/cortex_device.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      831 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/vex/crc.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1386 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/vex/message.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     7686 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/vex/stm32_device.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)    50297 2023-04-11 18:47:45.000000 pros-cli-3.4.2/pros/serial/devices/vex/v5_device.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1564 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/vex/v5_user_device.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     5294 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/devices/vex/vex_device.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.950909 pros-cli-3.4.2/pros/serial/interactive/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     7328 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/interactive/UploadProjectModal.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)       85 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/interactive/__init__.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.951859 pros-cli-3.4.2/pros/serial/ports/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      456 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/ports/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      689 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/ports/base_port.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     2566 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/serial/ports/direct_port.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1150 2023-04-18 01:11:20.000000 pros-cli-3.4.2/pros/serial/ports/exceptions.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     8208 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/ports/serial_share_bridge.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     3389 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/ports/serial_share_port.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1222 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/ports/v5_wireless_port.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.952174 pros-cli-3.4.2/pros/serial/terminal/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)       31 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/terminal/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)    10518 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/serial/terminal/terminal.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.952482 pros-cli-3.4.2/pros/upgrade/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      176 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/upgrade/__init__.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.953167 pros-cli-3.4.2/pros/upgrade/instructions/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      347 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/upgrade/instructions/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      573 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/upgrade/instructions/base_instructions.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1336 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/upgrade/instructions/download_instructions.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      504 2022-12-21 19:38:48.000000 pros-cli-3.4.2/pros/upgrade/instructions/explorer_instructions.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      321 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/upgrade/instructions/nothing_instructions.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.953651 pros-cli-3.4.2/pros/upgrade/manifests/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      307 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/upgrade/manifests/__init__.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     1419 2023-04-17 22:41:15.000000 pros-cli-3.4.2/pros/upgrade/manifests/upgrade_manifest_v1.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     2614 2023-02-23 00:33:36.000000 pros-cli-3.4.2/pros/upgrade/manifests/upgrade_manifest_v2.py
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     3575 2021-12-20 01:03:11.000000 pros-cli-3.4.2/pros/upgrade/upgrade_manager.py
+drwxr-xr-x   0 kunwarsahni   (501) staff       (20)        0 2023-04-18 01:19:57.954548 pros-cli-3.4.2/pros_cli.egg-info/
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      275 2023-04-18 01:19:57.000000 pros-cli-3.4.2/pros_cli.egg-info/PKG-INFO
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)     3884 2023-04-18 01:19:57.000000 pros-cli-3.4.2/pros_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)        1 2023-04-18 01:19:57.000000 pros-cli-3.4.2/pros_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)       72 2023-04-18 01:19:57.000000 pros-cli-3.4.2/pros_cli.egg-info/entry_points.txt
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      182 2023-04-18 01:19:57.000000 pros-cli-3.4.2/pros_cli.egg-info/requires.txt
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)        5 2023-04-18 01:19:57.000000 pros-cli-3.4.2/pros_cli.egg-info/top_level.txt
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)       38 2023-04-18 01:19:57.954890 pros-cli-3.4.2/setup.cfg
+-rw-r--r--   0 kunwarsahni   (501) staff       (20)      656 2021-12-20 01:03:11.000000 pros-cli-3.4.2/setup.py
```

### Comparing `pros-cli-3.4.1/LICENSE` & `pros-cli-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/README.md` & `pros-cli-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/cli/build.py` & `pros-cli-3.4.2/pros/cli/build.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/cli/click_classes.py` & `pros-cli-3.4.2/pros/cli/click_classes.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/cli/common.py` & `pros-cli-3.4.2/pros/cli/common.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/cli/conductor.py` & `pros-cli-3.4.2/pros/cli/conductor.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,25 +74,28 @@
     # whether the arguments are for the template or for the depot, so they share them
     logger(__name__).debug(f'Additional depot and template args: {query.metadata}')
     c.Conductor().fetch_template(depot, template, **query.metadata)
 
 
 @conductor.command(context_settings={'ignore_unknown_options': True})
 @click.option('--upgrade/--no-upgrade', 'upgrade_ok', default=True, help='Allow upgrading templates in a project')
+
 @click.option('--install/--no-install', 'install_ok', default=True, help='Allow installing templates in a project')
 @click.option('--download/--no-download', 'download_ok', default=True,
               help='Allow downloading templates or only allow local templates')
 @click.option('--upgrade-user-files/--no-upgrade-user-files', 'force_user', default=False,
               help='Replace all user files in a template')
 @click.option('--force', 'force_system', default=False, is_flag=True,
               help="Force all system files to be inserted into the project")
 @click.option('--force-apply', 'force_apply', default=False, is_flag=True,
               help="Force apply the template, disregarding if the template is already installed.")
 @click.option('--remove-empty-dirs/--no-remove-empty-dirs', 'remove_empty_directories', is_flag=True, default=True,
               help='Remove empty directories when removing files')
+@click.option('--beta', is_flag=True, default=False, show_default=True,
+              help='Allow applying beta templates')
 @project_option()
 @template_query(required=True)
 @default_options
 def apply(project: c.Project, query: c.BaseTemplate, **kwargs):
     """
     Upgrade or install a template to a PROS project
 
@@ -109,14 +112,16 @@
               help='Replace all user files in a template')
 @click.option('--force-system', '-f', 'force_system', default=False, is_flag=True,
               help="Force all system files to be inserted into the project")
 @click.option('--force-apply', 'force_apply', default=False, is_flag=True,
               help="Force apply the template, disregarding if the template is already installed.")
 @click.option('--remove-empty-dirs/--no-remove-empty-dirs', 'remove_empty_directories', is_flag=True, default=True,
               help='Remove empty directories when removing files')
+@click.option('--beta', is_flag=True, default=False, show_default=True,
+              help='Allow applying beta templates')
 @project_option()
 @template_query(required=True)
 @default_options
 @click.pass_context
 def install(ctx: click.Context, **kwargs):
     """
     Install a library into a PROS project
@@ -134,14 +139,16 @@
               help='Replace all user files in a template')
 @click.option('--force-system', '-f', 'force_system', default=False, is_flag=True,
               help="Force all system files to be inserted into the project")
 @click.option('--force-apply', 'force_apply', default=False, is_flag=True,
               help="Force apply the template, disregarding if the template is already installed.")
 @click.option('--remove-empty-dirs/--no-remove-empty-dirs', 'remove_empty_directories', is_flag=True, default=True,
               help='Remove empty directories when removing files')
+@click.option('--beta', is_flag=True, default=False, show_default=True,
+              help='Allow upgrading to beta templates')
 @project_option()
 @template_query(required=False)
 @default_options
 @click.pass_context
 def upgrade(ctx: click.Context, project: c.Project, query: c.BaseTemplate, **kwargs):
     """
     Upgrade a PROS project or one of its libraries
@@ -194,14 +201,16 @@
               help='Force update all remote depots, ignoring automatic update checks')
 @click.option('--no-default-libs', 'no_default_libs', default=False, is_flag=True,
               help='Do not install any default libraries after creating the project.')
 @click.option('--compile-after', is_flag=True, default=True, show_default=True,
               help='Compile the project after creation')
 @click.option('--build-cache', is_flag=True, default=None, show_default=False,
               help='Build compile commands cache after creation. Overrides --compile-after if both are specified.')
+@click.option('--beta', is_flag=True, default=False, show_default=True,
+              help='Create a project with a beta template')
 @click.pass_context
 @default_options
 def new_project(ctx: click.Context, path: str, target: str, version: str,
                 force_user: bool = False, force_system: bool = False,
                 no_default_libs: bool = False, compile_after: bool = True, build_cache: bool = None, **kwargs):
     """
     Create a new PROS project
@@ -240,30 +249,36 @@
                    context_settings={'ignore_unknown_options': True})
 @click.option('--allow-offline/--no-offline', 'allow_offline', default=True, show_default=True,
               help='(Dis)allow offline templates in the listing')
 @click.option('--allow-online/--no-online', 'allow_online', default=True, show_default=True,
               help='(Dis)allow online templates in the listing')
 @click.option('--force-refresh', is_flag=True, default=False, show_default=True,
               help='Force update all remote depots, ignoring automatic update checks')
-@click.option('--limit', type=int, default=15, help='The maximum number of displayed results for each library')
+@click.option('--limit', type=int, default=15,
+              help='The maximum number of displayed results for each library')
+@click.option('--beta', is_flag=True, default=False, show_default=True,
+              help='View beta templates in the listing')
 @template_query(required=False)
 @click.pass_context
 @default_options
 def query_templates(ctx, query: c.BaseTemplate, allow_offline: bool, allow_online: bool, force_refresh: bool,
-                    limit: int):
+                    limit: int, beta: bool):
     """
     Query local and remote templates based on a spec
 
     Visit https://pros.cs.purdue.edu/v5/cli/conductor.html to learn more
     """
     analytics.send("query-templates")
     if limit < 0:
         limit = 15
     templates = c.Conductor().resolve_templates(query, allow_offline=allow_offline, allow_online=allow_online,
-                                                force_refresh=force_refresh)
+                                                force_refresh=force_refresh, beta=beta)
+    if beta:
+        templates += c.Conductor().resolve_templates(query, allow_offline=allow_offline, allow_online=allow_online,
+                                                force_refresh=force_refresh, beta=False)
 
     render_templates = {}
     for template in templates:
         key = (template.identifier, template.origin)
         if key in render_templates:
             if isinstance(template, c.LocalTemplate):
                 render_templates[key]['local'] = True
```

### Comparing `pros-cli-3.4.1/pros/cli/conductor_utils.py` & `pros-cli-3.4.2/pros/cli/conductor_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,16 +154,21 @@
 def purge_template(query: c.BaseTemplate, force):
     analytics.send("purge-template")
     if not query:
         force = click.confirm('Are you sure you want to remove all cached templates? This action is non-reversable!',
                               abort=True)
     cond = c.Conductor()
     templates = cond.resolve_templates(query, allow_online=False)
+    beta_templates = cond.resolve_templates(query, allow_online=False, beta=True)
     if len(templates) == 0:
         click.echo('No matching templates were found matching the spec.')
         return 0
-    click.echo(f'The following template(s) will be removed {[t.identifier for t in templates]}')
+    t_list = [t.identifier for t in templates] + [t.identifier for t in beta_templates]
+    click.echo(f'The following template(s) will be removed {t_list}')
     if len(templates) > 1 and not force:
         click.confirm(f'Are you sure you want to remove multiple templates?', abort=True)
     for template in templates:
         if isinstance(template, c.LocalTemplate):
             cond.purge_template(template)
+    for template in beta_templates:
+        if isinstance(template, c.LocalTemplate):
+            cond.purge_template(template)
```

### Comparing `pros-cli-3.4.1/pros/cli/interactive.py` & `pros-cli-3.4.2/pros/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/cli/main.py` & `pros-cli-3.4.2/pros/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,18 +97,23 @@
     ui.echo('Analytics set to : {}'.format(analytics.useAnalytics))
     ctx.exit(0)
 
 
 @click.command('pros',
                cls=PROSCommandCollection,
                sources=root_commands)
+@click.pass_context
 @default_options
 @click.option('--version', help='Displays version and exits.', is_flag=True, expose_value=False, is_eager=True,
               callback=version)
 @click.option('--use-analytics', help='Set analytics usage (True/False).', type=str, expose_value=False,
               is_eager=True, default=None, callback=use_analytics)
-def cli():
+def cli(ctx):
     pros.common.sentry.register()
+    ctx.call_on_close(after_command)
+
+def after_command():
+    analytics.process_requests()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pros-cli-3.4.1/pros/cli/misc_commands.py` & `pros-cli-3.4.2/pros/cli/misc_commands.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/cli/terminal.py` & `pros-cli-3.4.2/pros/cli/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,16 @@
         sys.stdout = output
         logger(__name__).info(f'Redirecting Terminal Output to File: {output_file}')
     else:
         sys.stdout = sys.__stdout__
 
     signal.signal(signal.SIGINT, term.stop)
     term.start()
+    sys.stdout.write("Established terminal connection\n")
+    sys.stdout.flush()
     while not term.alive.is_set():
         time.sleep(0.005)
     sys.stdout = sys.__stdout__
     if output:
         output.end()
     term.join()
     logger(__name__).info('CLI Main Thread Dying')
```

### Comparing `pros-cli-3.4.1/pros/cli/upload.py` & `pros-cli-3.4.2/pros/cli/upload.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/cli/user_script.py` & `pros-cli-3.4.2/pros/cli/user_script.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/cli/v5_utils.py` & `pros-cli-3.4.2/pros/cli/v5_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,34 +290,36 @@
         w.write(file_, i_data)
 
     print(f'Saved screen capture to {file_name}')
 
 @v5.command(aliases=['sv', 'set'], short_help='Set a kernel variable on a connected V5 device')
 @click.argument('variable', type=click.Choice(['teamnumber', 'robotname']), required=True)
 @click.argument('value', required=True, type=click.STRING, nargs=1)
+@click.argument('port', type=str, default=None, required=False)
 @default_options
-def set_variable(variable, value):
+def set_variable(variable, value, port):
     import pros.serial.devices.vex as vex
     from pros.serial.ports import DirectPort
 
     # Get the connected v5 device
-    port = resolve_v5_port(None, 'system')[0]
+    port = resolve_v5_port(port, 'system')[0]
     if port == None:
         return
     device = vex.V5Device(DirectPort(port))
     actual_value = device.kv_write(variable, value).decode()
     print(f'Value of \'{variable}\' set to : {actual_value}')
 
 @v5.command(aliases=['rv', 'get'], short_help='Read a kernel variable from a connected V5 device')
 @click.argument('variable', type=click.Choice(['teamnumber', 'robotname']), required=True)
+@click.argument('port', type=str, default=None, required=False)
 @default_options
-def read_variable(variable):
+def read_variable(variable, port):
     import pros.serial.devices.vex as vex
     from pros.serial.ports import DirectPort
 
     # Get the connected v5 device
-    port = resolve_v5_port(None, 'system')[0]
+    port = resolve_v5_port(port, 'system')[0]
     if port == None:
         return
     device = vex.V5Device(DirectPort(port))
     value = device.kv_read(variable).decode()
     print(f'Value of \'{variable}\' is : {value}')
```

### Comparing `pros-cli-3.4.1/pros/common/sentry.py` & `pros-cli-3.4.2/pros/common/sentry.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/__init__.py` & `pros-cli-3.4.2/pros/common/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/ConfirmModal.py` & `pros-cli-3.4.2/pros/common/ui/interactive/ConfirmModal.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/application.py` & `pros-cli-3.4.2/pros/common/ui/interactive/application.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/components/button.py` & `pros-cli-3.4.2/pros/common/ui/interactive/components/button.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/components/component.py` & `pros-cli-3.4.2/pros/common/ui/interactive/components/component.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/components/container.py` & `pros-cli-3.4.2/pros/common/ui/interactive/components/container.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/components/input.py` & `pros-cli-3.4.2/pros/common/ui/interactive/components/input.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/components/label.py` & `pros-cli-3.4.2/pros/common/ui/interactive/components/label.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/observable.py` & `pros-cli-3.4.2/pros/common/ui/interactive/observable.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/parameters/misc_parameters.py` & `pros-cli-3.4.2/pros/common/ui/interactive/parameters/misc_parameters.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/parameters/parameter.py` & `pros-cli-3.4.2/pros/common/ui/interactive/parameters/parameter.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/parameters/validatable_parameter.py` & `pros-cli-3.4.2/pros/common/ui/interactive/parameters/validatable_parameter.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/renderers/MachineOutputRenderer.py` & `pros-cli-3.4.2/pros/common/ui/interactive/renderers/MachineOutputRenderer.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/interactive/renderers/Renderer.py` & `pros-cli-3.4.2/pros/common/ui/interactive/renderers/Renderer.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/ui/log.py` & `pros-cli-3.4.2/pros/common/ui/log.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/common/utils.py` & `pros-cli-3.4.2/pros/common/utils.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/conductor.py` & `pros-cli-3.4.2/pros/conductor/conductor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os.path
 import shutil
+from enum import Enum
 from pathlib import Path
 from typing import *
 
 import click
 from semantic_version import Spec, Version
 
 from pros.common import *
@@ -12,53 +13,80 @@
 from pros.config import Config
 from .depots import Depot, HttpDepot
 from .project import Project
 from .templates import BaseTemplate, ExternalTemplate, LocalTemplate, Template
 
 MAINLINE_NAME = 'pros-mainline'
 MAINLINE_URL = 'https://purduesigbots.github.io/pros-mainline/pros-mainline.json'
+BETA_NAME = 'kernel-beta-mainline'
+BETA_URL = 'https://raw.githubusercontent.com/purduesigbots/pros-mainline/master/beta/kernel-beta-mainline.json'
 
+"""
+# TBD? Currently, beta value is stored in config file
+class ReleaseChannel(Enum):
+    Stable = 'stable'
+    Beta = 'beta'
+"""
 
 class Conductor(Config):
     """
     Provides entrances for all conductor-related tasks (fetching, applying, creating new projects)
     """
-
     def __init__(self, file=None):
         if not file:
             file = os.path.join(click.get_app_dir('PROS'), 'conductor.pros')
         self.local_templates: Set[LocalTemplate] = set()
+        self.beta_local_templates: Set[LocalTemplate] = set()
         self.depots: Dict[str, Depot] = {}
         self.default_target: str = 'v5'
         self.default_libraries: Dict[str, List[str]] = None
+        self.beta_libraries: Dict[str, List[str]] = None
+        self.is_beta = False
         super(Conductor, self).__init__(file)
         needs_saving = False
         if MAINLINE_NAME not in self.depots or \
                 not isinstance(self.depots[MAINLINE_NAME], HttpDepot) or \
                 self.depots[MAINLINE_NAME].location != MAINLINE_URL:
             self.depots[MAINLINE_NAME] = HttpDepot(MAINLINE_NAME, MAINLINE_URL)
             needs_saving = True
+        # add beta depot as another remote depot
+        if BETA_NAME not in self.depots or \
+                not isinstance(self.depots[BETA_NAME], HttpDepot) or \
+                self.depots[BETA_NAME].location != BETA_URL:
+            self.depots[BETA_NAME] = HttpDepot(BETA_NAME, BETA_URL)
+            needs_saving = True
         if self.default_target is None:
             self.default_target = 'v5'
             needs_saving = True
         if self.default_libraries is None:
             self.default_libraries = {
                 'v5': ['okapilib'],
                 'cortex': []
             }
             needs_saving = True
+        if self.beta_libraries is None or len(self.beta_libraries['v5']) != 2:
+            self.beta_libraries = {
+                'v5': ['liblvgl', 'okapilib'],
+                'cortex': []
+            }
+            needs_saving = True
         if 'v5' not in self.default_libraries:
             self.default_libraries['v5'] = []
             needs_saving = True
         if 'cortex' not in self.default_libraries:
             self.default_libraries['cortex'] = []
             needs_saving = True
+        if 'v5' not in self.beta_libraries:
+            self.beta_libraries['v5'] = []
+            needs_saving = True
+        if 'cortex' not in self.beta_libraries:
+            self.beta_libraries['cortex'] = []
+            needs_saving = True
         if needs_saving:
             self.save()
-
         from pros.common.sentry import add_context
         add_context(self)
 
     def get_depot(self, name: str) -> Optional[Depot]:
         return self.depots.get(name)
 
     def fetch_template(self, depot: Depot, template: BaseTemplate, **kwargs) -> LocalTemplate:
@@ -74,58 +102,74 @@
                 shutil.rmtree(destination)
 
         template: Template = depot.fetch_template(template, destination, **kwargs)
         click.secho(f'Fetched {template.identifier} from {depot.name} depot', dim=True)
         local_template = LocalTemplate(orig=template, location=destination)
         local_template.metadata['origin'] = depot.name
         click.echo(f'Adding {local_template.identifier} to registry...', nl=False)
-        self.local_templates.add(local_template)
+        if depot.name == BETA_NAME: # check for beta
+            self.beta_local_templates.add(local_template)
+        else:
+            self.local_templates.add(local_template)
         self.save()
         if isinstance(template, ExternalTemplate) and template.directory == destination:
             template.delete()
         click.secho('Done', fg='green')
         return local_template
 
     def purge_template(self, template: LocalTemplate):
-        if template not in self.local_templates:
-            logger(__name__).info(f"{template.identifier} was not in the Conductor's local templates cache.")
+        if template.metadata['origin'] == BETA_NAME:
+            if template not in self.beta_local_templates:
+                logger(__name__).info(f"{template.identifier} was not in the Conductor's local beta templates cache.")
+            else:
+                self.beta_local_templates.remove(template)
         else:
-            self.local_templates.remove(template)
+            if template not in self.local_templates:
+                logger(__name__).info(f"{template.identifier} was not in the Conductor's local templates cache.")
+            else:
+                self.local_templates.remove(template)
 
         if os.path.abspath(template.location).startswith(
                 os.path.abspath(os.path.join(self.directory, 'templates'))) \
                 and os.path.isdir(template.location):
             shutil.rmtree(template.location)
         self.save()
 
     def resolve_templates(self, identifier: Union[str, BaseTemplate], allow_online: bool = True,
                           allow_offline: bool = True, force_refresh: bool = False,
                           unique: bool = True, **kwargs) -> List[BaseTemplate]:
         results = list() if not unique else set()
         kernel_version = kwargs.get('kernel_version', None)
+        self.is_beta = kwargs.get('beta', False)
         if isinstance(identifier, str):
             query = BaseTemplate.create_query(name=identifier, **kwargs)
         else:
             query = identifier
         if allow_offline:
-            offline_results = filter(lambda t: t.satisfies(query, kernel_version=kernel_version), self.local_templates)
+            if self.is_beta:
+                offline_results = filter(lambda t: t.satisfies(query, kernel_version=kernel_version), self.beta_local_templates)
+            else:
+                offline_results = filter(lambda t: t.satisfies(query, kernel_version=kernel_version), self.local_templates)
             if unique:
                 results.update(offline_results)
             else:
                 results.extend(offline_results)
         if allow_online:
             for depot in self.depots.values():
-                online_results = filter(lambda t: t.satisfies(query, kernel_version=kernel_version),
+                # beta depot will only be accessed when the --beta flag is true
+                if depot.name != BETA_NAME or (depot.name == BETA_NAME and self.is_beta):
+                    online_results = filter(lambda t: t.satisfies(query, kernel_version=kernel_version),
                                         depot.get_remote_templates(force_check=force_refresh, **kwargs))
-                if unique:
-                    results.update(online_results)
-                else:
-                    results.extend(online_results)
+                    if unique:
+                        results.update(online_results)
+                    else:
+                        results.extend(online_results)
             logger(__name__).debug('Saving Conductor config after checking for remote updates')
             self.save()  # Save self since there may have been some updates from the depots
+            
         return list(results)
 
     def resolve_template(self, identifier: Union[str, BaseTemplate], **kwargs) -> Optional[BaseTemplate]:
         if isinstance(identifier, str):
             kwargs['name'] = identifier
         elif isinstance(identifier, BaseTemplate):
             kwargs['orig'] = identifier
@@ -174,14 +218,34 @@
             # support_kernels for backwards compatibility, but kernel_version should be getting most of the exposure
             kwargs['kernel_version'] = kwargs['supported_kernels'] = project.templates['kernel'].version
         template = self.resolve_template(identifier=identifier, allow_online=download_ok, **kwargs)
         if template is None:
             raise dont_send(
                 InvalidTemplateException(f'Could not find a template satisfying {identifier} for {project.target}'))
 
+        # warn and prompt user if upgrading to PROS 4 or downgrading to PROS 3
+        if template.name == 'kernel':
+            isProject = Project.find_project("")
+            if isProject:
+                curr_proj = Project()
+                if curr_proj.kernel:
+                    if template.version[0] == '4' and curr_proj.kernel[0] == '3':
+                        confirm = ui.confirm(f'Warning! Upgrading project to PROS 4 will cause breaking changes. '
+                                             f'For PROS 4 LLEMU/LVGL to function, the library liblvgl is required. '
+                                             f'Run \'pros conductor apply liblvgl --beta\' in the project directory. '
+                                             f'Do you still want to upgrade?')
+                        if not confirm:
+                            raise dont_send(
+                                InvalidTemplateException(f'Not upgrading'))
+                    if template.version[0] == '3' and curr_proj.kernel[0] == '4':
+                        confirm = ui.confirm(f'Warning! Downgrading project to PROS 3 will cause breaking changes. '
+                                             f'Do you still want to downgrade?')
+                        if not confirm:
+                            raise dont_send(
+                                InvalidTemplateException(f'Not downgrading'))
         if not isinstance(template, LocalTemplate):
             with ui.Notification():
                 template = self.fetch_template(self.get_depot(template.metadata['origin']), template, **kwargs)
         assert isinstance(template, LocalTemplate)
 
         logger(__name__).info(str(project))
         valid_action = project.get_template_actions(template)
@@ -203,38 +267,56 @@
                                          f' and that is not allowed.', reason=valid_action)
             )
 
     @staticmethod
     def remove_template(project: Project, identifier: Union[str, BaseTemplate], remove_user: bool = True,
                         remove_empty_directories: bool = True):
         ui.logger(__name__).debug(f'Uninstalling templates matching {identifier}')
+        if not project.resolve_template(identifier):
+            ui.echo(f"{identifier} is not an applicable template")
         for template in project.resolve_template(identifier):
             ui.echo(f'Uninstalling {template.identifier}')
             project.remove_template(template, remove_user=remove_user,
                                     remove_empty_directories=remove_empty_directories)
 
     def new_project(self, path: str, no_default_libs: bool = False, **kwargs) -> Project:
+        self.is_beta = kwargs.get('beta', False)
         if Path(path).exists() and Path(path).samefile(os.path.expanduser('~')):
             raise dont_send(ValueError('Will not create a project in user home directory'))
+        for char in str(Path(path)):
+            if char in ['/', '?', '<', '>', '\\', ':', '*', '|', '^', '#', '%', '&', '$', '+', '!', '`', '\'', '=',
+                        '@', '\'', '{', '}', '[', ']', '(', ')', '~'] or ord(char) > 127:
+                raise dont_send(ValueError(f'Invalid character found in directory name: \'{char}\''))
         proj = Project(path=path, create=True)
         if 'target' in kwargs:
             proj.target = kwargs['target']
         if 'project_name' in kwargs and kwargs['project_name'] and not kwargs['project_name'].isspace():
             proj.project_name = kwargs['project_name']
         else:
             proj.project_name = os.path.basename(os.path.normpath(os.path.abspath(path)))
         if 'version' in kwargs:
             if kwargs['version'] == 'latest':
                 kwargs['version'] = '>=0'
             self.apply_template(proj, identifier='kernel', **kwargs)
         proj.save()
 
         if not no_default_libs:
-            for library in self.default_libraries[proj.target]:
-                try:
-                    # remove kernel version so that latest template satisfying query is correctly selected
-                    if 'version' in kwargs:
-                        kwargs.pop('version')
-                    self.apply_template(proj, library, **kwargs)
-                except Exception as e:
-                    logger(__name__).exception(e)
+            if self.is_beta:
+                #libraries = self.beta_libraries if self.is_beta else self.default_libraries
+                for library in self.beta_libraries[proj.target]:
+                    try:
+                        # remove kernel version so that latest template satisfying query is correctly selected
+                        if 'version' in kwargs:
+                            kwargs.pop('version')
+                        self.apply_template(proj, library, **kwargs)
+                    except Exception as e:
+                        logger(__name__).exception(e)
+            else:
+                for library in self.default_libraries[proj.target]:
+                    try:
+                        # remove kernel version so that latest template satisfying query is correctly selected
+                        if 'version' in kwargs:
+                            kwargs.pop('version')
+                        self.apply_template(proj, library, **kwargs)
+                    except Exception as e:
+                        logger(__name__).exception(e)
         return proj
```

### Comparing `pros-cli-3.4.1/pros/conductor/depots/depot.py` & `pros-cli-3.4.2/pros/conductor/depots/depot.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/depots/http_depot.py` & `pros-cli-3.4.2/pros/conductor/depots/http_depot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import os
 import zipfile
-from datetime import datetime
+from datetime import datetime, timedelta
 
 import jsonpickle
 
 import pros.common.ui as ui
 from pros.common import logger
 from pros.common.utils import download_file
 from .depot import Depot
 from ..templates import BaseTemplate, ExternalTemplate
 
 
 class HttpDepot(Depot):
     def __init__(self, name: str, location: str):
-        super().__init__(name, location, config_schema={})
+        # Note: If update_frequency = timedelta(minutes=1) isn't included as a parameter,
+        # the beta depot won't be saved in conductor.json correctly
+        super().__init__(name, location, config_schema={}, update_frequency = timedelta(minutes=1))
 
     def fetch_template(self, template: BaseTemplate, destination: str, **kwargs):
         import requests
         assert 'location' in template.metadata
         url = template.metadata['location']
         tf = download_file(url, ext='zip', desc=f'Downloading {template.identifier}')
         if tf is None:
```

### Comparing `pros-cli-3.4.1/pros/conductor/depots/local_depot.py` & `pros-cli-3.4.2/pros/conductor/depots/local_depot.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/interactive/NewProjectModal.py` & `pros-cli-3.4.2/pros/conductor/interactive/NewProjectModal.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/interactive/UpdateProjectModal.py` & `pros-cli-3.4.2/pros/conductor/interactive/UpdateProjectModal.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/interactive/components.py` & `pros-cli-3.4.2/pros/conductor/interactive/components.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/interactive/parameters.py` & `pros-cli-3.4.2/pros/conductor/interactive/parameters.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/project/ProjectReport.py` & `pros-cli-3.4.2/pros/conductor/project/ProjectReport.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/project/ProjectTransaction.py` & `pros-cli-3.4.2/pros/conductor/project/ProjectTransaction.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/project/__init__.py` & `pros-cli-3.4.2/pros/conductor/project/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 
     def get_template_actions(self, template: BaseTemplate) -> TemplateAction:
         ui.logger(__name__).debug(template)
         if template.target != self.target:
             return TemplateAction.NotApplicable
         from semantic_version import Spec, Version
         if template.name != 'kernel' and Version(self.kernel) not in Spec(template.supported_kernels or '>0'):
+            if template.name in self.templates.keys():
+                return TemplateAction.AlreadyInstalled
             return TemplateAction.NotApplicable
         for current in self.templates.values():
             if template.name != current.name:
                 continue
             if template > current:
                 return TemplateAction.Upgradable
             if template == current:
```

### Comparing `pros-cli-3.4.1/pros/conductor/project/template_resolution.py` & `pros-cli-3.4.2/pros/conductor/project/template_resolution.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/templates/base_template.py` & `pros-cli-3.4.2/pros/conductor/templates/base_template.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/templates/external_template.py` & `pros-cli-3.4.2/pros/conductor/templates/external_template.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/templates/local_template.py` & `pros-cli-3.4.2/pros/conductor/templates/local_template.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/conductor/transaction.py` & `pros-cli-3.4.2/pros/conductor/transaction.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/config/cli_config.py` & `pros-cli-3.4.2/pros/config/cli_config.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/config/config.py` & `pros-cli-3.4.2/pros/config/config.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/ga/analytics.py` & `pros-cli-3.4.2/pros/ga/analytics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import json
 from os import path
 import uuid
 import requests
+from requests_futures.sessions import FuturesSession
 import random
+from concurrent.futures import as_completed
 
 url = 'https://www.google-analytics.com/collect'
 agent = 'pros-cli'
 
 """
 PROS ANALYTICS CLASS
 """
@@ -25,14 +27,15 @@
             }
         self.cli_config.save()
         self.sent = False
         #Variables that the class will use
         self.gaID = self.cli_config.ga['ga_id']
         self.useAnalytics = self.cli_config.ga['enabled']
         self.uID = self.cli_config.ga['u_id']
+        self.pendingRequests = []
 
     def send(self,action):
         if not self.useAnalytics or self.sent:
             return
         self.sent=True # Prevent Send from being called multiple times
         try:
             #Payload to be sent to GA, idk what some of them are but it works
@@ -44,29 +47,49 @@
                 'cid': self.uID,
                 't': 'event',
                 'ec': 'action',
                 'ea': action,
                 'el': 'CLI',
                 'ev': '1',
                 'ni': 0
-            }          
+            }
+
+            session = FuturesSession()          
 
             #Send payload to GA servers 
-            response = requests.post(url=url,
+            future = session.post(url=url,
                              data=payload,
                              headers={'User-Agent': agent},
                              timeout=5.0)
-            if not response.status_code==200:
-                print("Something went wrong while sending analytics!")
-                print(response)
-            return response
+            self.pendingRequests.append(future)
+
         except Exception as e:
             from pros.cli.common import logger
             logger(__name__).warning("Unable to send analytics. Do you have a stable internet connection?", extra={'sentry': False})
 
     def set_use(self, value: bool):
         #Sets if GA is being used or not
         self.useAnalytics = value
         self.cli_config.ga['enabled'] = self.useAnalytics
         self.cli_config.save()
+    
+    def process_requests(self):
+        responses = []
+        for future in as_completed(self.pendingRequests):
+            try:
+                response = future.result()
+                
+                if not response.status_code==200:
+                    print("Something went wrong while sending analytics!")
+                    print(response)
+
+                responses.append(response)
+
+            except Exception:
+                print("Something went wrong while sending analytics!")
+
+
+        self.pendingRequests.clear()
+        return responses
+
 
 analytics = Analytics()
```

### Comparing `pros-cli-3.4.1/pros/serial/devices/stream_device.py` & `pros-cli-3.4.2/pros/serial/devices/stream_device.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/devices/vex/cortex_device.py` & `pros-cli-3.4.2/pros/serial/devices/vex/cortex_device.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/devices/vex/crc.py` & `pros-cli-3.4.2/pros/serial/devices/vex/crc.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/devices/vex/message.py` & `pros-cli-3.4.2/pros/serial/devices/vex/message.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/devices/vex/stm32_device.py` & `pros-cli-3.4.2/pros/serial/devices/vex/stm32_device.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/devices/vex/v5_device.py` & `pros-cli-3.4.2/pros/serial/devices/vex/v5_device.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/devices/vex/v5_user_device.py` & `pros-cli-3.4.2/pros/serial/devices/vex/v5_user_device.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/devices/vex/vex_device.py` & `pros-cli-3.4.2/pros/serial/devices/vex/vex_device.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/interactive/UploadProjectModal.py` & `pros-cli-3.4.2/pros/serial/interactive/UploadProjectModal.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/ports/base_port.py` & `pros-cli-3.4.2/pros/serial/ports/base_port.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/ports/direct_port.py` & `pros-cli-3.4.2/pros/serial/ports/direct_port.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from typing import *
 
 import serial
 
 from pros.common import logger, dont_send
-from pros.serial.ports.exceptions import ConnectionRefusedException
+from pros.serial.ports.exceptions import ConnectionRefusedException, PortNotFoundException
 from .base_port import BasePort, PortConnectionException
 
 
 def create_serial_port(port_name: str, timeout: Optional[float] = 1.0) -> serial.Serial:
     try:
         logger(__name__).debug(f'Opening serial port {port_name}')
         port = serial.Serial(port_name, baudrate=115200, bytesize=serial.EIGHTBITS,
@@ -19,15 +19,16 @@
     except serial.SerialException as e:
         if any(msg in str(e) for msg in [
             'Access is denied', 'Errno 16', 'Errno 13'
         ]):
             tb = sys.exc_info()[2]
             raise dont_send(ConnectionRefusedException(port_name, e).with_traceback(tb))
         else:
-            raise e
+            raise dont_send(PortNotFoundException(port_name, e))
+
 
 
 class DirectPort(BasePort):
 
     def __init__(self, port_name: str, **kwargs):
         self.serial: serial.Serial = create_serial_port(port_name=port_name, timeout=kwargs.pop('timeout', 1.0))
         self.buffer: bytearray = bytearray()
```

### Comparing `pros-cli-3.4.1/pros/serial/ports/serial_share_bridge.py` & `pros-cli-3.4.2/pros/serial/ports/serial_share_bridge.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/ports/serial_share_port.py` & `pros-cli-3.4.2/pros/serial/ports/serial_share_port.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/ports/v5_wireless_port.py` & `pros-cli-3.4.2/pros/serial/ports/v5_wireless_port.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/serial/terminal/terminal.py` & `pros-cli-3.4.2/pros/serial/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/upgrade/instructions/base_instructions.py` & `pros-cli-3.4.2/pros/upgrade/instructions/base_instructions.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/upgrade/instructions/download_instructions.py` & `pros-cli-3.4.2/pros/upgrade/instructions/download_instructions.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/upgrade/manifests/upgrade_manifest_v1.py` & `pros-cli-3.4.2/pros/upgrade/manifests/upgrade_manifest_v1.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/upgrade/manifests/upgrade_manifest_v2.py` & `pros-cli-3.4.2/pros/upgrade/manifests/upgrade_manifest_v2.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros/upgrade/upgrade_manager.py` & `pros-cli-3.4.2/pros/upgrade/upgrade_manager.py`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/pros_cli.egg-info/SOURCES.txt` & `pros-cli-3.4.2/pros_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pros-cli-3.4.1/setup.py` & `pros-cli-3.4.2/setup.py`

 * *Files identical despite different names*

