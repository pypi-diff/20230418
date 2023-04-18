# Comparing `tmp/hello_robot_stretch_factory-0.4.1.tar.gz` & `tmp/hello_robot_stretch_factory-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_factory-0.4.1.tar", last modified: Wed Apr 12 23:17:11 2023, max compression
+gzip compressed data, was "hello_robot_stretch_factory-0.4.2.tar", last modified: Tue Apr 18 19:47:03 2023, max compression
```

## Comparing `hello_robot_stretch_factory-0.4.1.tar` & `hello_robot_stretch_factory-0.4.2.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-12 23:17:11.756573 hello_robot_stretch_factory-0.4.1/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      929 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/LICENSE.md
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-04-12 23:17:11.756573 hello_robot_stretch_factory-0.4.1/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      355 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/README.md
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-12 23:17:11.752573 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      816 2023-04-12 23:17:11.000000 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1796 2023-04-12 23:17:11.000000 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-04-12 23:17:11.000000 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       74 2023-04-12 23:17:11.000000 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2023-04-12 23:17:11.000000 hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-04-12 23:17:11.756573 hello_robot_stretch_factory-0.4.1/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      995 2023-04-12 23:14:54.000000 hello_robot_stretch_factory-0.4.1/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-12 23:17:11.756573 hello_robot_stretch_factory-0.4.1/stretch_factory/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/device_mgmt.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4425 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_available.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5248 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_installed.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3861 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_recommended.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    37370 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5254 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2726 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_version.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20922 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/hello_device_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/stretch_factory/param_mgmt.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-12 23:17:11.756573 hello_robot_stretch_factory-0.4.1/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/test/test_firmware_updater.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/test/test_usb_reset.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-12 23:17:11.752573 hello_robot_stretch_factory-0.4.1/tools/
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/RE1_migrate_contacts.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/RE1_migrate_params.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    22012 2023-02-03 03:51:49.000000 hello_robot_stretch_factory-0.4.1/tools/REx_D435i_check.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_imu_collect.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_imu_process.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_wheel_separation.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4771 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_gravity_comp.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7456 2023-04-12 23:11:21.000000 hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_guarded_contact.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_range.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_cliff_sensor_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18552 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_discover_hello_devices.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_id_change.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1354 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_id_scan.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5045 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1374 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_reboot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_set_baud.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4410 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/tools/REx_firmware_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5804 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/tools/REx_firmware_updater.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_gamepad_configure.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_gripper_calibrate.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_hello_dynamixel_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_YAML_to_flash.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      685 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_flash_to_YAML.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_run.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_ctrl_tuning.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_gains.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4064 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_jog.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_stepper_mechaduino_menu.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    10577 2023-04-03 20:35:08.000000 hello_robot_stretch_factory-0.4.1/tools/REx_trace_firmware.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7819 2023-04-12 22:15:57.000000 hello_robot_stretch_factory-0.4.1/tools/REx_trace_robot.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_usb_reset.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2023-01-26 20:33:11.000000 hello_robot_stretch_factory-0.4.1/tools/REx_wacc_calibrate.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      935 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      355 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/README.md
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      935 2023-04-18 19:47:03.000000 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1785 2023-04-18 19:47:03.000000 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2023-04-18 19:47:03.000000 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       74 2023-04-18 19:47:03.000000 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       16 2023-04-18 19:47:03.000000 hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2023-04-18 19:47:03.657871 hello_robot_stretch_factory-0.4.2/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      995 2023-04-18 19:28:09.000000 hello_robot_stretch_factory-0.4.2/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/stretch_factory/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6326 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/device_mgmt.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4425 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_available.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5248 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_installed.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3861 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_recommended.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    37747 2023-04-18 19:39:17.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_updater.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5254 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2726 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_version.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    20922 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/hello_device_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12828 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/stretch_factory/param_mgmt.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/test/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      685 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/test/test_firmware_updater.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      668 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/test/test_usb_reset.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2023-04-18 19:47:03.653871 hello_robot_stretch_factory-0.4.2/tools/
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2456 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/RE1_migrate_contacts.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     6621 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/RE1_migrate_params.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    22012 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_D435i_check.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5418 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_imu_collect.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    32027 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_imu_process.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5950 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_wheel_separation.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4771 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_gravity_comp.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7456 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_guarded_contact.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     3578 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_range.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1728 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_cliff_sensor_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18552 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_discover_hello_devices.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1442 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_id_change.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1354 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_id_scan.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5045 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1374 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_reboot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1188 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_set_baud.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4397 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_firmware_flash.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     5804 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_firmware_updater.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1583 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_gamepad_configure.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2338 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_gripper_calibrate.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1947 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_hello_dynamixel_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      870 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_YAML_to_flash.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      685 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_flash_to_YAML.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1168 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_run.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    18644 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_ctrl_tuning.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1163 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_gains.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     4064 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_jog.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)      852 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_stepper_mechaduino_menu.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    10577 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_trace_firmware.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     7819 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_trace_robot.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     2347 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_usb_reset.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     1379 2023-04-18 17:53:03.000000 hello_robot_stretch_factory-0.4.2/tools/REx_wacc_calibrate.py
```

### Comparing `hello_robot_stretch_factory-0.4.1/PKG-INFO` & `hello_robot_stretch_factory-0.4.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: hello_robot_stretch_factory
-Version: 0.4.1
+Version: 0.4.2
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
+License: UNKNOWN
+Description: # Overview
+        
+        The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
+        
+        **These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
+        
+        This package can be installed by:
+        
+        ```
+        python -m pip install  -U hello-robot-stretch-factory
+        ```
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Overview
-
-The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
-
-**These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
-
-This package can be installed by:
-
-```
-python -m pip install  -U hello-robot-stretch-factory
-```
-
```

### Comparing `hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/PKG-INFO` & `hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: hello-robot-stretch-factory
-Version: 0.4.1
+Version: 0.4.2
 Summary: Stretch Factory Tools
 Home-page: https://github.com/hello-robot/stretch_factory
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
+License: UNKNOWN
+Description: # Overview
+        
+        The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
+        
+        **These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
+        
+        This package can be installed by:
+        
+        ```
+        python -m pip install  -U hello-robot-stretch-factory
+        ```
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Overview
-
-The Stretch Factory package provides Python tools for testing and calibration of the Hello Robot Stretch RE1 and RE2. 
-
-**These tools are provided for reference only and are intended to be used by qualified Hello Robot production engineers.** 
-
-This package can be installed by:
-
-```
-python -m pip install  -U hello-robot-stretch-factory
-```
-
```

### Comparing `hello_robot_stretch_factory-0.4.1/hello_robot_stretch_factory.egg-info/SOURCES.txt` & `hello_robot_stretch_factory-0.4.2/hello_robot_stretch_factory.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.md
 README.md
 setup.py
 ./tools/RE1_migrate_contacts.py
 ./tools/RE1_migrate_params.py
 ./tools/REx_D435i_check.py
 ./tools/REx_base_calibrate_imu_collect.py
 ./tools/REx_base_calibrate_imu_process.py
```

### Comparing `hello_robot_stretch_factory-0.4.1/setup.py` & `hello_robot_stretch_factory-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 script_path='./tools'
 ex_scripts = glob.glob(script_path+'/*.py') + glob.glob(script_path+'/*.sh')
 stretch_scripts=[f for f in ex_scripts if isfile(f)]
 
 setuptools.setup(
     name="hello_robot_stretch_factory",
-    version="0.4.1",
+    version="0.4.2",
     author="Hello Robot Inc.",
     author_email="support@hello-robot.com",
     description="Stretch Factory Tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hello-robot/stretch_factory",
     scripts = stretch_scripts,
```

### Comparing `hello_robot_stretch_factory-0.4.1/stretch_factory/device_mgmt.py` & `hello_robot_stretch_factory-0.4.2/stretch_factory/device_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_available.py` & `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_available.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_installed.py` & `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_installed.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_recommended.py` & `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_recommended.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_updater.py` & `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,24 +221,29 @@
             for d in self.target:
                 click.secho(' %s  '.center(110, '#') % d.upper(), fg="yellow", bold=True)
                 click.secho(' %s |  COMPILE AND FLASH FIRMWARE... '.center(110, '#')%d.upper(), fg="cyan", bold=True)
                 if not self.state['completed'][d]['flash']:
                     if self.fw_installed.is_device_valid(d):
                         nretry=3
                         for i in range(nretry):
-                            self.state['completed'][d]['flash']=self.do_device_flash(d,self.target[d].to_string(),self.state['repo_path'],self.state['verbose'])
-                            if not self.state['completed'][d]['flash']:
+                            compile_fail, upload_success=self.do_device_flash(d,self.target[d].to_string(),self.state['repo_path'],self.state['verbose'])
+                            self.state['completed'][d]['flash'] = not compile_fail and upload_success
+                            if self.state['completed'][d]['flash']:
+                                break
+                            if compile_fail:
+                                click.secho('WARNING: Firmware failed to compile. Fix source then try again', fg="red",bold=True)
+                                break
+                            if not upload_success: #Dont retry if compile failure
                                 #It may get here if the usb bus connectoin fails during flash
                                 #Attempt to reset the device and then try again
                                 print('Retrying firmware flash for %s'%d)
                                 port=fwu.get_port_name(d)
                                 if port is not None:
                                     hdu.place_arduino_in_bootloader('/dev/'+port)
-                            else:
-                                break
+                           
                     else:
                         click.secho('WARNING: Unable to flash %s as device not valid'%d, fg="yellow", bold=True)
                         self.state['completed'][d]['flash'] =False
 
                     if not self.state['completed'][d]['flash']:
                         click.secho('WARNING: Device %s did not flash firmware successfully'%d, fg="red", bold=True)
                         click.secho('WARNING: Power cycle robot.', fg="red", bold=True)
@@ -319,31 +324,33 @@
         all_completed=True
         for d in self.target:
             all_completed=all_completed and self.state['completed'][d][state_name]
         return all_completed
 
 # ########################################################################################################################
     def do_device_flash(self, device_name, tag, repo_path=None, verbose=False, port_name=None):
-        #click.secho('-------- FIRMWARE FLASH %s | %s ------------' % (device_name, tag), fg="cyan", bold=True)
+        """
+        Return compile_fail, upload_success
+        """
         config_file = self.fw_available.repo_path + '/arduino-cli.yaml'
 
         fwu.user_msg_log('Config: ' + str(config_file), user_display=verbose)
         fwu.user_msg_log('Repo: ' + str(repo_path), user_display=verbose)
 
         sketch_name=fwu.get_sketch_name(device_name)
 
         if sketch_name == 'hello_stepper' and not fwu.does_stepper_have_encoder_calibration_YAML(device_name):
             print('Encoder data has not been stored for %s and may be lost. Aborting firmware flash.' % device_name)
-            return False
+            return False, False
 
         if port_name is None:
             print('Looking for device %s on bus' % device_name)
             if not fwu.wait_on_device(device_name, timeout=5.0):
                 print('Failure: Device not on bus.')
-                return False
+                return False, False
             port_name = fwu.get_port_name(device_name)
 
         fwu.user_msg_log('Device: %s Port: %s' % (device_name, port_name), user_display=verbose)
 
         if port_name is not None and sketch_name is not None:
             print('Starting programming. This will take about 5s...')
             if repo_path is None:
@@ -368,15 +375,15 @@
 
             # In version 0.18.x the last line after compile is: Sketch uses xxx bytes (58%) of program storage space. Maximum is yyy bytes.
             # In version 0.24.x +this is now on line 0.
             # Need a more robust way to determine successful compile. Works for now.
             success = (str(cc[0]).find('Sketch uses') != -1)
             if not success:
                 print('Firmware failed to compile %s at %s' % (sketch_name, src_path))
-                return False
+                return True, False
             else:
                 print('Success in firmware compile')
 
             upload_command = 'arduino-cli upload  --config-file %s -p /dev/%s --fqbn hello-robot:samd:%s %s/arduino/%s' % (
             config_file, port_name, sketch_name, src_path, sketch_name)
 
             fwu.user_msg_log(upload_command, user_display=verbose)
@@ -397,21 +404,21 @@
                     else:
                         for m in k:
                             print(m)
             success = uu[-1] == 'CPU reset.'
 
             if not success:
                 print('Firmware flash. Failed to upload to %s' % (port_name))
-                return False
+                return False, False
             else:
                 click.secho('Success in firmware flash' , fg="green")
-                return True
+                return False, True
         else:
             print('Firmware update %s. Failed to find device %s' % (tag, device_name))
-            return False
+            return False, False
 
 # ########################################################################################################3
     def wait_on_return_to_bus(self,device_name):
         click.secho('Checking that device %s returned to bus '%device_name)
         print('It may take several minutes to appear on the USB bus.' )
         ts = time.time()
         found = False
```

### Comparing `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_utils.py` & `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/stretch_factory/firmware_version.py` & `hello_robot_stretch_factory-0.4.2/stretch_factory/firmware_version.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/stretch_factory/hello_device_utils.py` & `hello_robot_stretch_factory-0.4.2/stretch_factory/hello_device_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/stretch_factory/param_mgmt.py` & `hello_robot_stretch_factory-0.4.2/stretch_factory/param_mgmt.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/test/test_firmware_updater.py` & `hello_robot_stretch_factory-0.4.2/test/test_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/test/test_usb_reset.py` & `hello_robot_stretch_factory-0.4.2/test/test_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/RE1_migrate_contacts.py` & `hello_robot_stretch_factory-0.4.2/tools/RE1_migrate_contacts.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/RE1_migrate_params.py` & `hello_robot_stretch_factory-0.4.2/tools/RE1_migrate_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_D435i_check.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_D435i_check.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_imu_collect.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_imu_collect.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_imu_process.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_imu_process.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_base_calibrate_wheel_separation.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_base_calibrate_wheel_separation.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_gravity_comp.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_gravity_comp.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_guarded_contact.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_guarded_contact.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_calibrate_range.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_calibrate_range.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_cliff_sensor_calibrate.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_cliff_sensor_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_discover_hello_devices.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_discover_hello_devices.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_id_change.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_id_change.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_id_scan.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_id_scan.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_reboot.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_reboot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_dynamixel_set_baud.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_dynamixel_set_baud.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_firmware_flash.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_firmware_flash.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 #Note: This is a simple alternative to REx_firmware_updater.py
 parser = argparse.ArgumentParser(description='Tool to directly flash Stretch firmware to a ttyACM device', )
 
 group = parser.add_mutually_exclusive_group()
 group.add_argument("--map", help="Print mapping from ttyACMx to Hello devices", action="store_true")
 group.add_argument('--flash', nargs=2, type=str, help='Flash firmware. E.g, --flash /dev/ttyACM0 hello-motor-arm')
-group.add_argument('--boot', nargs=1, type=str, help='Place board in bootloader mode. E.g, --reset /dev/ttyACM0')
+group.add_argument('--boot', nargs=1, type=str, help='Place board in bootloader mode. E.g, --boot /dev/ttyACM0')
 
 
 args = parser.parse_args()
 
 
 def does_stepper_have_encoder_calibration_YAML(device_name):
     d = stretch_body.device.Device(req_params=False)
@@ -68,18 +68,18 @@
         sketch_name = 'hello_pimu'
     elif "hello-wacc" in device:
         sketch_name = 'hello_wacc'
     else:
         print(Fore.RED + 'Invalid Device name')
         sys.exit()
 
-    repo_path = os.path.expanduser('~/repos/stretch_firmware')
+    repo_path = os.path.expanduser('~/stretch_firmware')
     if not os.path.exists(repo_path):
         print('Firmware not present')
-        print('Clone https://github.com/hello-robot/stretch_firmware to ~/repos/stretch_firmware first')
+        print('Clone https://github.com/hello-robot/stretch_firmware to ~/stretch_firmware first')
         sys.exit()
     t = 'Choose a Firmware Version'
     print(Style.BRIGHT + t)
     print('=' * len(t))
     i = 0
     for v in a.versions[device]:
         v_s = v.to_string()
```

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_firmware_updater.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_firmware_updater.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_gamepad_configure.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_gamepad_configure.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_gripper_calibrate.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_gripper_calibrate.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_hello_dynamixel_jog.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_hello_dynamixel_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_YAML_to_flash.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_YAML_to_flash.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_flash_to_YAML.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_flash_to_YAML.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_calibration_run.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_calibration_run.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_ctrl_tuning.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_ctrl_tuning.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_gains.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_gains.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_jog.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_jog.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_stepper_mechaduino_menu.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_stepper_mechaduino_menu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_trace_firmware.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_trace_firmware.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_trace_robot.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_trace_robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_usb_reset.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_usb_reset.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_factory-0.4.1/tools/REx_wacc_calibrate.py` & `hello_robot_stretch_factory-0.4.2/tools/REx_wacc_calibrate.py`

 * *Files identical despite different names*

