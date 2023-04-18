# Comparing `tmp/ospd_openvas-22.4.6.tar.gz` & `tmp/ospd_openvas-22.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ospd_openvas-22.4.6.tar", max compression
+gzip compressed data, was "ospd_openvas-22.5.0.tar", max compression
```

## Comparing `ospd_openvas-22.4.6.tar` & `ospd_openvas-22.5.0.tar`

### file list

```diff
@@ -1,89 +1,88 @@
--rw-r--r--   0        0        0    12468 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/CHANGELOG.md
--rw-r--r--   0        0        0    34008 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/COPYING
--rw-r--r--   0        0        0     5031 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/README.md
--rw-r--r--   0        0        0      175 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/config/ospd-openvas.conf
--rw-r--r--   0        0        0      636 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/config/ospd-openvas.service
--rw-r--r--   0        0        0     4983 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/docs/ospd-openvas.8
--rw-r--r--   0        0        0      854 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/__init__.py
--rw-r--r--   0        0        0      855 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/command/__init__.py
--rw-r--r--   0        0        0    23236 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/command/command.py
--rw-r--r--   0        0        0     1697 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/command/initsubclass.py
--rw-r--r--   0        0        0     1141 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/command/registry.py
--rw-r--r--   0        0        0     1639 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/config.py
--rw-r--r--   0        0        0     5255 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/cvss.py
--rw-r--r--   0        0        0     4900 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/datapickler.py
--rw-r--r--   0        0        0     1846 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/errors.py
--rw-r--r--   0        0        0     3320 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/logger.py
--rw-r--r--   0        0        0     4502 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/main.py
--rw-r--r--   0        0        0     4522 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/misc.py
--rw-r--r--   0        0        0    16225 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/network.py
--rw-r--r--   0        0        0    49515 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/ospd.py
--rw-r--r--   0        0        0     9674 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/parser.py
--rw-r--r--   0        0        0    11404 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/protocol.py
--rw-r--r--   0        0        0     3945 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/resultlist.py
--rw-r--r--   0        0        0    21119 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/scan.py
--rw-r--r--   0        0        0     9199 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/server.py
--rw-r--r--   0        0        0     1878 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/timer.py
--rw-r--r--   0        0        0     4757 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/vtfilter.py
--rw-r--r--   0        0        0     6375 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/vts.py
--rw-r--r--   0        0        0     9277 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/xml.py
--rw-r--r--   0        0        0    12715 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd/xmlvt.py
--rw-r--r--   0        0        0      815 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd_openvas/__init__.py
--rw-r--r--   0        0        0      103 2023-02-08 09:39:23.891769 ospd_openvas-22.4.6/ospd_openvas/__version__.py
--rw-r--r--   0        0        0    44060 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/daemon.py
--rw-r--r--   0        0        0    22426 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/db.py
--rw-r--r--   0        0        0     7115 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/dryrun.py
--rw-r--r--   0        0        0      995 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/errors.py
--rw-r--r--   0        0        0     1327 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/feed.py
--rw-r--r--   0        0        0     4500 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/gpg_sha_verifier.py
--rw-r--r--   0        0        0     3950 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/lock.py
--rw-r--r--   0        0        0      748 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/messages/__init__.py
--rw-r--r--   0        0        0     2922 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/messages/message.py
--rw-r--r--   0        0        0     2899 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/messages/result.py
--rw-r--r--   0        0        0      748 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/messaging/__init__.py
--rw-r--r--   0        0        0     6000 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/messaging/mqtt.py
--rw-r--r--   0        0        0     1110 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/messaging/publisher.py
--rw-r--r--   0        0        0     1214 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/messaging/subscriber.py
--rw-r--r--   0        0        0     9130 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/notus.py
--rw-r--r--   0        0        0     9781 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/nvticache.py
--rw-r--r--   0        0        0     5724 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/openvas.py
--rw-r--r--   0        0        0    29271 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/preferencehandler.py
--rw-r--r--   0        0        0     9019 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/ospd_openvas/vthelper.py
--rw-r--r--   0        0        0    68299 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/poetry.lock
--rw-r--r--   0        0        0       32 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/poetry.toml
--rw-r--r--   0        0        0     2386 2023-02-08 09:39:23.895769 ospd_openvas-22.4.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/__init__.py
--rw-r--r--   0        0        0      753 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/command/__init__.py
--rw-r--r--   0        0        0     2659 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/command/test_command.py
--rw-r--r--   0        0        0    17656 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/command/test_commands.py
--rw-r--r--   0        0        0     2056 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/command/test_registry.py
--rw-r--r--   0        0        0     6184 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/dummydaemon.py
--rw-r--r--   0        0        0     7077 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/helper.py
--rw-r--r--   0        0        0      748 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/messages/__init__.py
--rw-r--r--   0        0        0     4835 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/messages/test_message.py
--rw-r--r--   0        0        0     6506 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/messages/test_result.py
--rw-r--r--   0        0        0      748 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/messaging/__init__.py
--rw-r--r--   0        0        0     3354 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/messaging/test_mqtt.py
--rw-r--r--   0        0        0     5394 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_argument_parser.py
--rw-r--r--   0        0        0     1640 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_cvss.py
--rw-r--r--   0        0        0    23643 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_daemon.py
--rw-r--r--   0        0        0     4266 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_datapickler.py
--rw-r--r--   0        0        0    23560 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_db.py
--rw-r--r--   0        0        0     2414 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_errors.py
--rw-r--r--   0        0        0     1574 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_feed.py
--rw-r--r--   0        0        0     3492 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_gpg.py
--rw-r--r--   0        0        0     3643 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_lock.py
--rw-r--r--   0        0        0     7472 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_notus.py
--rw-r--r--   0        0        0    11381 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_nvti_cache.py
--rw-r--r--   0        0        0    10923 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_openvas.py
--rw-r--r--   0        0        0    56922 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_port_convert.py
--rw-r--r--   0        0        0    50670 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_preferencehandler.py
--rw-r--r--   0        0        0     1085 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_protocol.py
--rw-r--r--   0        0        0    55047 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_scan_and_result.py
--rw-r--r--   0        0        0     3886 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_target_convert.py
--rw-r--r--   0        0        0    10295 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_vthelper.py
--rw-r--r--   0        0        0     5529 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_vts.py
--rw-r--r--   0        0        0    15029 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/test_xml.py
--rw-r--r--   0        0        0      373 2023-02-08 09:39:23.899769 ospd_openvas-22.4.6/tests/testing.conf
--rw-r--r--   0        0        0     6465 1970-01-01 00:00:00.000000 ospd_openvas-22.4.6/setup.py
--rw-r--r--   0        0        0     6606 1970-01-01 00:00:00.000000 ospd_openvas-22.4.6/PKG-INFO
+-rw-r--r--   0        0        0    12468 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34008 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/COPYING
+-rw-r--r--   0        0        0     4883 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/README.md
+-rw-r--r--   0        0        0      175 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/config/ospd-openvas.conf
+-rw-r--r--   0        0        0      636 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/config/ospd-openvas.service
+-rw-r--r--   0        0        0     4972 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/docs/ospd-openvas.8
+-rw-r--r--   0        0        0      843 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/__init__.py
+-rw-r--r--   0        0        0      844 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/command/__init__.py
+-rw-r--r--   0        0        0    23225 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/command/command.py
+-rw-r--r--   0        0        0     1686 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/command/initsubclass.py
+-rw-r--r--   0        0        0     1130 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/command/registry.py
+-rw-r--r--   0        0        0     1628 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/config.py
+-rw-r--r--   0        0        0     5244 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/cvss.py
+-rw-r--r--   0        0        0     4889 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/datapickler.py
+-rw-r--r--   0        0        0     1835 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/errors.py
+-rw-r--r--   0        0        0     3309 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/logger.py
+-rw-r--r--   0        0        0     4480 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/main.py
+-rw-r--r--   0        0        0     4511 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/misc.py
+-rw-r--r--   0        0        0    16214 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/network.py
+-rw-r--r--   0        0        0    49500 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/ospd.py
+-rw-r--r--   0        0        0    10001 2023-04-18 13:26:24.924457 ospd_openvas-22.5.0/ospd/parser.py
+-rw-r--r--   0        0        0    11393 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/protocol.py
+-rw-r--r--   0        0        0     3934 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/resultlist.py
+-rw-r--r--   0        0        0    21108 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/scan.py
+-rw-r--r--   0        0        0     9188 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/server.py
+-rw-r--r--   0        0        0     1867 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/timer.py
+-rw-r--r--   0        0        0     4746 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/vtfilter.py
+-rw-r--r--   0        0        0     6364 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/vts.py
+-rw-r--r--   0        0        0     9266 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/xml.py
+-rw-r--r--   0        0        0    12704 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd/xmlvt.py
+-rw-r--r--   0        0        0      804 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/__version__.py
+-rw-r--r--   0        0        0    44291 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/daemon.py
+-rw-r--r--   0        0        0    22646 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/db.py
+-rw-r--r--   0        0        0     7104 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/dryrun.py
+-rw-r--r--   0        0        0      984 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/errors.py
+-rw-r--r--   0        0        0     1316 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/feed.py
+-rw-r--r--   0        0        0     4500 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/gpg_sha_verifier.py
+-rw-r--r--   0        0        0     3939 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/lock.py
+-rw-r--r--   0        0        0      737 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messages/__init__.py
+-rw-r--r--   0        0        0     2911 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messages/message.py
+-rw-r--r--   0        0        0     2888 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messages/result.py
+-rw-r--r--   0        0        0      737 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messaging/__init__.py
+-rw-r--r--   0        0        0     5989 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messaging/mqtt.py
+-rw-r--r--   0        0        0     1099 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messaging/publisher.py
+-rw-r--r--   0        0        0     1203 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/messaging/subscriber.py
+-rw-r--r--   0        0        0     9119 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/notus.py
+-rw-r--r--   0        0        0     9770 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/nvticache.py
+-rw-r--r--   0        0        0     6199 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/openvas.py
+-rw-r--r--   0        0        0    29260 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/preferencehandler.py
+-rw-r--r--   0        0        0     9008 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/ospd_openvas/vthelper.py
+-rw-r--r--   0        0        0    71367 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/poetry.lock
+-rw-r--r--   0        0        0       32 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/poetry.toml
+-rw-r--r--   0        0        0     2390 2023-04-18 13:26:24.928457 ospd_openvas-22.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      742 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/command/__init__.py
+-rw-r--r--   0        0        0     2648 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/command/test_command.py
+-rw-r--r--   0        0        0    17645 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/command/test_commands.py
+-rw-r--r--   0        0        0     2045 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/command/test_registry.py
+-rw-r--r--   0        0        0     6173 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/dummydaemon.py
+-rw-r--r--   0        0        0     7066 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/helper.py
+-rw-r--r--   0        0        0      737 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/messages/__init__.py
+-rw-r--r--   0        0        0     4824 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/messages/test_message.py
+-rw-r--r--   0        0        0     6495 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/messages/test_result.py
+-rw-r--r--   0        0        0      737 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/messaging/__init__.py
+-rw-r--r--   0        0        0     3343 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/messaging/test_mqtt.py
+-rw-r--r--   0        0        0     5383 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_argument_parser.py
+-rw-r--r--   0        0        0     1629 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_cvss.py
+-rw-r--r--   0        0        0    23632 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_daemon.py
+-rw-r--r--   0        0        0     4255 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_datapickler.py
+-rw-r--r--   0        0        0    25291 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_db.py
+-rw-r--r--   0        0        0     2403 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_errors.py
+-rw-r--r--   0        0        0     1563 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_feed.py
+-rw-r--r--   0        0        0     3481 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_gpg.py
+-rw-r--r--   0        0        0     3632 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_lock.py
+-rw-r--r--   0        0        0     7461 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_notus.py
+-rw-r--r--   0        0        0    11370 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_nvti_cache.py
+-rw-r--r--   0        0        0    10912 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_openvas.py
+-rw-r--r--   0        0        0    56911 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_port_convert.py
+-rw-r--r--   0        0        0    50659 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_preferencehandler.py
+-rw-r--r--   0        0        0     1074 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_protocol.py
+-rw-r--r--   0        0        0    55036 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_scan_and_result.py
+-rw-r--r--   0        0        0     3875 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_target_convert.py
+-rw-r--r--   0        0        0    10284 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_vthelper.py
+-rw-r--r--   0        0        0     5518 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_vts.py
+-rw-r--r--   0        0        0    15018 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/test_xml.py
+-rw-r--r--   0        0        0      373 2023-04-18 13:26:24.932457 ospd_openvas-22.5.0/tests/testing.conf
+-rw-r--r--   0        0        0     6447 1970-01-01 00:00:00.000000 ospd_openvas-22.5.0/PKG-INFO
```

### Comparing `ospd_openvas-22.4.6/CHANGELOG.md` & `ospd_openvas-22.5.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.4.6/COPYING` & `ospd_openvas-22.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.4.6/README.md` & `ospd_openvas-22.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 ![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
 
 # ospd-openvas
 
 [![GitHub releases](https://img.shields.io/github/release/greenbone/ospd-openvas.svg)](https://github.com/greenbone/ospd-openvas/releases)
 [![PyPI](https://img.shields.io/pypi/v/ospd-openvas.svg)](https://pypi.org/project/ospd-openvas/)
-[![code test coverage](https://codecov.io/gh/greenbone/ospd/branch/main/graphs/badge.svg)](https://codecov.io/gh/greenbone/ospd-openvas)
 [![Build and test](https://github.com/greenbone/ospd-openvas/actions/workflows/ci-python.yml/badge.svg?branch=main)](https://github.com/greenbone/ospd-openvas/actions/workflows/ci-python.yml?query=branch%3Amain++)
 
 ospd-openvas is an OSP server implementation to remotely control
 [OpenVAS Scanner](https://github.com/greenbone/openvas-scanner) and [Notus Scanner](https://github.com/greenbone/notus-scanner).
 
 Once running, you need to configure OpenVAS Scanner and Notus Scanner for the Greenbone Vulnerability
 Manager, for example via the web interface Greenbone Security Assistant. Then
@@ -116,10 +115,10 @@
 are active.
 
     poetry install
     poetry run autohooks activate --force
 
 ## License
 
-Copyright (C) 2018-2022 [Greenbone Networks GmbH](https://www.greenbone.net/)
+Copyright (C) 2018-2022 [Greenbone AG](https://www.greenbone.net/)
 
 Licensed under the [GNU Affero General Public License v3.0 or later](COPYING).
```

### Comparing `ospd_openvas-22.4.6/config/ospd-openvas.service` & `ospd_openvas-22.5.0/config/ospd-openvas.service`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.4.6/docs/ospd-openvas.8` & `ospd_openvas-22.5.0/docs/ospd-openvas.8`

 * *Files 1% similar despite different names*

```diff
@@ -186,8 +186,8 @@
 .UR https://www.openvas.org
 Traditional home site
 .UE
 .RE
 
 .SH AUTHORS
 
-ospd-openvas code is developed by Greenbone Networks GmbH.
+ospd-openvas code is developed by Greenbone AG.
```

### Comparing `ospd_openvas-22.4.6/ospd/__init__.py` & `ospd_openvas-22.5.0/ospd/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/command/__init__.py` & `ospd_openvas-22.5.0/ospd/command/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/command/command.py` & `ospd_openvas-22.5.0/ospd/command/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/command/initsubclass.py` & `ospd_openvas-22.5.0/ospd/command/initsubclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/command/registry.py` & `ospd_openvas-22.5.0/ospd/command/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/config.py` & `ospd_openvas-22.5.0/ospd/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/cvss.py` & `ospd_openvas-22.5.0/ospd/cvss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/datapickler.py` & `ospd_openvas-22.5.0/ospd/datapickler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/errors.py` & `ospd_openvas-22.5.0/ospd/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/logger.py` & `ospd_openvas-22.5.0/ospd/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/main.py` & `ospd_openvas-22.5.0/ospd/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -30,15 +30,15 @@
 from ospd.misc import go_to_background, create_pid
 from ospd.ospd import OSPDaemon
 from ospd.parser import create_parser, ParserType
 from ospd.server import TlsServer, UnixSocketServer, BaseServer
 from ospd.logger import init_logging
 
 
-COPYRIGHT = """Copyright (C) 2014-2021 Greenbone Networks GmbH
+COPYRIGHT = """Copyright (C) 2014-2021 Greenbone AG
 License GPLv2+: GNU GPL version 2 or later
 This is free software: you are free to change and redistribute it.
 There is NO WARRANTY, to the extent permitted by law."""
 
 logger = logging.getLogger(__name__)
```

### Comparing `ospd_openvas-22.4.6/ospd/misc.py` & `ospd_openvas-22.5.0/ospd/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/network.py` & `ospd_openvas-22.5.0/ospd/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/ospd.py` & `ospd_openvas-22.5.0/ospd/ospd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -120,15 +120,15 @@
     def __init__(
         self,
         *,
         customvtfilter=None,
         storage=None,
         max_scans=0,
         min_free_mem_scan_queue=0,
-        file_storage_dir='/var/run/ospd',
+        file_storage_dir='/run/ospd',
         max_queued_scans=0,
         **kwargs,
     ):  # pylint: disable=unused-argument
         """Initializes the daemon's internal data."""
 
         def remove_previous_data_pickler_files():
             logger.debug("removing uuid files in %s", file_storage_dir)
```

### Comparing `ospd_openvas-22.4.6/ospd/parser.py` & `ospd_openvas-22.5.0/ospd/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -28,15 +28,15 @@
 
 DEFAULT_PORT = 0
 DEFAULT_ADDRESS = "0.0.0.0"
 DEFAULT_NICENESS = 10
 DEFAULT_UNIX_SOCKET_MODE = "0o770"
 DEFAULT_CONFIG_PATH = "~/.config/ospd.conf"
 DEFAULT_LOG_CONFIG_PATH = "~/.config/ospd-logging.conf"
-DEFAULT_UNIX_SOCKET_PATH = "/run/ospd/ospd.sock"
+DEFAULT_UNIX_SOCKET_PATH = "/run/ospd/ospd-openvas.sock"
 DEFAULT_PID_PATH = "/run/ospd/ospd.pid"
 DEFAULT_LOCKFILE_DIR_PATH = "/run/ospd"
 DEFAULT_STREAM_TIMEOUT = 10  # ten seconds
 DEFAULT_SCANINFO_STORE_TIME = 0  # in hours
 DEFAULT_MAX_SCAN = 0  # 0 = disable
 DEFAULT_MIN_FREE_MEM_SCAN_QUEUE = 0  # 0 = Disable
 DEFAULT_MAX_QUEUED_SCANS = 0  # 0 = Disable
@@ -215,14 +215,24 @@
             type=self.network_port,
             help=(
                 'Broker port to connect to for MQTT communication.'
                 ' Neccessary to get results from Notus-Scanner.Default'
                 'Default %(default)s'
             ),
         )
+        parser.add_argument(
+            '--feed-updater',
+            default="openvas",
+            choices=['openvas', 'nasl-cli'],
+            help=(
+                'Sets the method of updating the feed.'
+                ' Can either be openvas or nasl-cli.'
+                ' Default: %(default)s.'
+            ),
+        )
 
         self.parser = parser
 
     def network_port(self, string: str) -> int:
         """Check if provided string is a valid network port."""
 
         value = int(string)
```

### Comparing `ospd_openvas-22.4.6/ospd/protocol.py` & `ospd_openvas-22.5.0/ospd/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/resultlist.py` & `ospd_openvas-22.5.0/ospd/resultlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/scan.py` & `ospd_openvas-22.5.0/ospd/scan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/server.py` & `ospd_openvas-22.5.0/ospd/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/timer.py` & `ospd_openvas-22.5.0/ospd/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/vtfilter.py` & `ospd_openvas-22.5.0/ospd/vtfilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/vts.py` & `ospd_openvas-22.5.0/ospd/vts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/xml.py` & `ospd_openvas-22.5.0/ospd/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd/xmlvt.py` & `ospd_openvas-22.5.0/ospd/xmlvt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/__init__.py` & `ospd_openvas-22.5.0/ospd_openvas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/daemon.py` & `ospd_openvas-22.5.0/ospd_openvas/daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -46,15 +46,15 @@
 from ospd_openvas.notus import Cache, Notus, NotusParser, NotusResultHandler
 from ospd_openvas.dryrun import DryRun
 from ospd_openvas.messages.result import ResultMessage
 from ospd_openvas.nvticache import NVTICache
 from ospd_openvas.db import MainDB, BaseDB
 from ospd_openvas.lock import LockFile
 from ospd_openvas.preferencehandler import PreferenceHandler
-from ospd_openvas.openvas import Openvas
+from ospd_openvas.openvas import NASLCli, Openvas
 from ospd_openvas.vthelper import VtHelper
 from ospd_openvas.messaging.mqtt import MQTTClient, MQTTDaemon, MQTTSubscriber
 from ospd_openvas.feed import Feed
 
 SENTRY_DSN_OSPD_OPENVAS = environ.get("SENTRY_DSN_OSPD_OPENVAS")
 if SENTRY_DSN_OSPD_OPENVAS:
     # pylint: disable=import-error
@@ -468,14 +468,15 @@
     def __init__(
         self,
         *,
         niceness=None,
         lock_file_dir='/var/lib/openvas',
         mqtt_broker_address="localhost",
         mqtt_broker_port=1883,
+        feed_updater="openvas",
         disable_notus_hashsum_verification=False,
         **kwargs,
     ):
         """Initializes the ospd-openvas daemon's internal data."""
 
         self.main_db = MainDB()
         notus_dir = kwargs.get('notus_feed_dir')
@@ -484,14 +485,15 @@
             ndir = Path(notus_dir)
             self.notus = Notus(
                 ndir,
                 Cache(self.main_db),
                 disable_notus_hashsum_verification,
             )
 
+        self.feed_updater = feed_updater
         self.nvti = NVTICache(self.main_db)
 
         super().__init__(
             customvtfilter=OpenVasVtsFilter(self.nvti, self.notus),
             storage=dict,
             file_storage_dir=lock_file_dir,
             **kwargs,
@@ -666,16 +668,21 @@
             "Loading VTs. Scans will be [requested|queued] until VTs are"
             " loaded. This may take a few minutes, please wait..."
         )
         old = self.nvti.get_feed_version() or 0
         # reload notus cache
         if self.notus:
             self.notus.reload_cache()
+        loaded = False
+        if self.feed_updater == "nasl-cli":
+            loaded = NASLCli.load_vts_into_redis()
+        else:
+            loaded = Openvas.load_vts_into_redis()
 
-        if Openvas.load_vts_into_redis():
+        if loaded:
             new = self.nvti.get_feed_version()
             if new != old:
                 logger.info(
                     "Finished loading VTs. The VT cache has been updated from"
                     " version %s to %s.",
                     old,
                     new,
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/db.py` & `ospd_openvas-22.5.0/ospd_openvas/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -68,14 +68,21 @@
     from a KB to another."""
 
     _db_address = None
 
     @classmethod
     def get_database_address(cls) -> Optional[str]:
         if not cls._db_address:
+            if not Openvas.check():
+                logger.error(
+                    'openvas executable not available. Please install openvas'
+                    ' into your PATH.'
+                )
+                sys.exit(1)
+
             settings = Openvas.get_settings()
 
             cls._db_address = settings.get('db_address')
             if cls._db_address:
                 # translate openvas tcp:// configuration to redis://
                 cls._db_address = cls._db_address.replace("tcp://", "redis://")
                 # translate non scheme to unix://
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/dryrun.py` & `ospd_openvas-22.5.0/ospd_openvas/dryrun.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/errors.py` & `ospd_openvas-22.5.0/ospd_openvas/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/feed.py` & `ospd_openvas-22.5.0/ospd_openvas/feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/gpg_sha_verifier.py` & `ospd_openvas-22.5.0/ospd_openvas/gpg_sha_verifier.py`

 * *Files identical despite different names*

### Comparing `ospd_openvas-22.4.6/ospd_openvas/lock.py` & `ospd_openvas-22.5.0/ospd_openvas/lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/messages/__init__.py` & `ospd_openvas-22.5.0/ospd_openvas/messages/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/messages/message.py` & `ospd_openvas-22.5.0/ospd_openvas/messages/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/messages/result.py` & `ospd_openvas-22.5.0/ospd_openvas/messages/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/messaging/__init__.py` & `ospd_openvas-22.5.0/ospd_openvas/messaging/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/messaging/mqtt.py` & `ospd_openvas-22.5.0/ospd_openvas/messaging/mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/messaging/publisher.py` & `ospd_openvas-22.5.0/ospd_openvas/messaging/publisher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/messaging/subscriber.py` & `ospd_openvas-22.5.0/ospd_openvas/messaging/subscriber.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/notus.py` & `ospd_openvas-22.5.0/ospd_openvas/notus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/nvticache.py` & `ospd_openvas-22.5.0/ospd_openvas/nvticache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/openvas.py` & `ospd_openvas-22.5.0/ospd_openvas/openvas.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -24,14 +24,30 @@
 
 
 logger = logging.getLogger(__name__)
 
 _BOOL_DICT = {'no': 0, 'yes': 1}
 
 
+class NASLCli:
+    """Class for calling nasl-cli executable"""
+
+    @staticmethod
+    def load_vts_into_redis() -> bool:
+        """Loads all VTs into the redis database"""
+        try:
+            subprocess.check_call(
+                ['nasl-cli', 'feed', 'update'], stdout=subprocess.DEVNULL
+            )
+            return True
+        except (subprocess.SubprocessError, OSError) as err:
+            logger.error('nasl-cli failed to load VTs. %s', err)
+            return False
+
+
 class Openvas:
     """Class for calling the openvas executable"""
 
     @staticmethod
     def _get_version_output() -> Optional[str]:
         try:
             result = subprocess.check_output(
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/preferencehandler.py` & `ospd_openvas-22.5.0/ospd_openvas/preferencehandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/ospd_openvas/vthelper.py` & `ospd_openvas-22.5.0/ospd_openvas/vthelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/poetry.lock` & `ospd_openvas-22.5.0/poetry.lock`

 * *Files 3% similar despite different names*

```diff
@@ -103,40 +103,54 @@
 
 [package.dependencies]
 autohooks = ">=2.2.0"
 pylint = ">=2.8.3,<3.0.0"
 
 [[package]]
 name = "black"
-version = "22.12.0"
+version = "23.3.0"
 description = "The uncompromising code formatter."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "black-22.12.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9eedd20838bd5d75b80c9f5487dbcb06836a43833a37846cf1d8c1cc01cef59d"},
-    {file = "black-22.12.0-cp310-cp310-win_amd64.whl", hash = "sha256:159a46a4947f73387b4d83e87ea006dbb2337eab6c879620a3ba52699b1f4351"},
-    {file = "black-22.12.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:d30b212bffeb1e252b31dd269dfae69dd17e06d92b87ad26e23890f3efea366f"},
-    {file = "black-22.12.0-cp311-cp311-win_amd64.whl", hash = "sha256:7412e75863aa5c5411886804678b7d083c7c28421210180d67dfd8cf1221e1f4"},
-    {file = "black-22.12.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:c116eed0efb9ff870ded8b62fe9f28dd61ef6e9ddd28d83d7d264a38417dcee2"},
-    {file = "black-22.12.0-cp37-cp37m-win_amd64.whl", hash = "sha256:1f58cbe16dfe8c12b7434e50ff889fa479072096d79f0a7f25e4ab8e94cd8350"},
-    {file = "black-22.12.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:77d86c9f3db9b1bf6761244bc0b3572a546f5fe37917a044e02f3166d5aafa7d"},
-    {file = "black-22.12.0-cp38-cp38-win_amd64.whl", hash = "sha256:82d9fe8fee3401e02e79767016b4907820a7dc28d70d137eb397b92ef3cc5bfc"},
-    {file = "black-22.12.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:101c69b23df9b44247bd88e1d7e90154336ac4992502d4197bdac35dd7ee3320"},
-    {file = "black-22.12.0-cp39-cp39-win_amd64.whl", hash = "sha256:559c7a1ba9a006226f09e4916060982fd27334ae1998e7a38b3f33a37f7a2148"},
-    {file = "black-22.12.0-py3-none-any.whl", hash = "sha256:436cc9167dd28040ad90d3b404aec22cedf24a6e4d7de221bec2730ec0c97bcf"},
-    {file = "black-22.12.0.tar.gz", hash = "sha256:229351e5a18ca30f447bf724d007f890f97e13af070bb6ad4c0a441cd7596a2f"},
+    {file = "black-23.3.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915"},
+    {file = "black-23.3.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9"},
+    {file = "black-23.3.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2"},
+    {file = "black-23.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c"},
+    {file = "black-23.3.0-cp310-cp310-win_amd64.whl", hash = "sha256:35d1381d7a22cc5b2be2f72c7dfdae4072a3336060635718cc7e1ede24221d6c"},
+    {file = "black-23.3.0-cp311-cp311-macosx_10_16_arm64.whl", hash = "sha256:a8a968125d0a6a404842fa1bf0b349a568634f856aa08ffaff40ae0dfa52e7c6"},
+    {file = "black-23.3.0-cp311-cp311-macosx_10_16_universal2.whl", hash = "sha256:c7ab5790333c448903c4b721b59c0d80b11fe5e9803d8703e84dcb8da56fec1b"},
+    {file = "black-23.3.0-cp311-cp311-macosx_10_16_x86_64.whl", hash = "sha256:a6f6886c9869d4daae2d1715ce34a19bbc4b95006d20ed785ca00fa03cba312d"},
+    {file = "black-23.3.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6f3c333ea1dd6771b2d3777482429864f8e258899f6ff05826c3a4fcc5ce3f70"},
+    {file = "black-23.3.0-cp311-cp311-win_amd64.whl", hash = "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326"},
+    {file = "black-23.3.0-cp37-cp37m-macosx_10_16_x86_64.whl", hash = "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b"},
+    {file = "black-23.3.0-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:50cb33cac881766a5cd9913e10ff75b1e8eb71babf4c7104f2e9c52da1fb7de2"},
+    {file = "black-23.3.0-cp37-cp37m-win_amd64.whl", hash = "sha256:e114420bf26b90d4b9daa597351337762b63039752bdf72bf361364c1aa05925"},
+    {file = "black-23.3.0-cp38-cp38-macosx_10_16_arm64.whl", hash = "sha256:48f9d345675bb7fbc3dd85821b12487e1b9a75242028adad0333ce36ed2a6d27"},
+    {file = "black-23.3.0-cp38-cp38-macosx_10_16_universal2.whl", hash = "sha256:714290490c18fb0126baa0fca0a54ee795f7502b44177e1ce7624ba1c00f2331"},
+    {file = "black-23.3.0-cp38-cp38-macosx_10_16_x86_64.whl", hash = "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5"},
+    {file = "black-23.3.0-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:562bd3a70495facf56814293149e51aa1be9931567474993c7942ff7d3533961"},
+    {file = "black-23.3.0-cp38-cp38-win_amd64.whl", hash = "sha256:e198cf27888ad6f4ff331ca1c48ffc038848ea9f031a3b40ba36aced7e22f2c8"},
+    {file = "black-23.3.0-cp39-cp39-macosx_10_16_arm64.whl", hash = "sha256:3238f2aacf827d18d26db07524e44741233ae09a584273aa059066d644ca7b30"},
+    {file = "black-23.3.0-cp39-cp39-macosx_10_16_universal2.whl", hash = "sha256:f0bd2f4a58d6666500542b26354978218a9babcdc972722f4bf90779524515f3"},
+    {file = "black-23.3.0-cp39-cp39-macosx_10_16_x86_64.whl", hash = "sha256:92c543f6854c28a3c7f39f4d9b7694f9a6eb9d3c5e2ece488c327b6e7ea9b266"},
+    {file = "black-23.3.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3a150542a204124ed00683f0db1f5cf1c2aaaa9cc3495b7a3b5976fb136090ab"},
+    {file = "black-23.3.0-cp39-cp39-win_amd64.whl", hash = "sha256:6b39abdfb402002b8a7d030ccc85cf5afff64ee90fa4c5aebc531e3ad0175ddb"},
+    {file = "black-23.3.0-py3-none-any.whl", hash = "sha256:ec751418022185b0c1bb7d7736e6933d40bbb14c14a0abcf9123d1b159f98dd4"},
+    {file = "black-23.3.0.tar.gz", hash = "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940"},
 ]
 
 [package.dependencies]
 click = ">=8.0.0"
 mypy-extensions = ">=0.4.3"
+packaging = ">=22.0"
 pathspec = ">=0.9.0"
 platformdirs = ">=2"
-tomli = {version = ">=1.1.0", markers = "python_full_version < \"3.11.0a7\""}
+tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
 typed-ast = {version = ">=1.4.2", markers = "python_version < \"3.8\" and implementation_name == \"cpython\""}
 typing-extensions = {version = ">=3.10.0.0", markers = "python_version < \"3.10\""}
 
 [package.extras]
 colorama = ["colorama (>=0.4.3)"]
 d = ["aiohttp (>=3.7.4)"]
 jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
@@ -532,33 +546,33 @@
 cssselect = ["cssselect (>=0.7)"]
 html5 = ["html5lib"]
 htmlsoup = ["BeautifulSoup4"]
 source = ["Cython (>=0.29.7)"]
 
 [[package]]
 name = "markdown-it-py"
-version = "2.1.0"
+version = "2.2.0"
 description = "Python port of markdown-it. Markdown parsing, done right!"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "markdown-it-py-2.1.0.tar.gz", hash = "sha256:cf7e59fed14b5ae17c0006eff14a2d9a00ed5f3a846148153899a0224e2c07da"},
-    {file = "markdown_it_py-2.1.0-py3-none-any.whl", hash = "sha256:93de681e5c021a432c63147656fe21790bc01231e0cd2da73626f1aa3ac0fe27"},
+    {file = "markdown-it-py-2.2.0.tar.gz", hash = "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"},
+    {file = "markdown_it_py-2.2.0-py3-none-any.whl", hash = "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30"},
 ]
 
 [package.dependencies]
 mdurl = ">=0.1,<1.0"
 typing_extensions = {version = ">=3.7.4", markers = "python_version < \"3.8\""}
 
 [package.extras]
-benchmarking = ["psutil", "pytest", "pytest-benchmark (>=3.2,<4.0)"]
-code-style = ["pre-commit (==2.6)"]
-compare = ["commonmark (>=0.9.1,<0.10.0)", "markdown (>=3.3.6,<3.4.0)", "mistletoe (>=0.8.1,<0.9.0)", "mistune (>=2.0.2,<2.1.0)", "panflute (>=2.1.3,<2.2.0)"]
-linkify = ["linkify-it-py (>=1.0,<2.0)"]
+benchmarking = ["psutil", "pytest", "pytest-benchmark"]
+code-style = ["pre-commit (>=3.0,<4.0)"]
+compare = ["commonmark (>=0.9,<1.0)", "markdown (>=3.4,<4.0)", "mistletoe (>=1.0,<2.0)", "mistune (>=2.0,<3.0)", "panflute (>=2.3,<3.0)"]
+linkify = ["linkify-it-py (>=1,<3)"]
 plugins = ["mdit-py-plugins"]
 profiling = ["gprof2dot"]
 rtd = ["attrs", "myst-parser", "pyyaml", "sphinx", "sphinx-copybutton", "sphinx-design", "sphinx_book_theme"]
 testing = ["coverage", "pytest", "pytest-cov", "pytest-regressions"]
 
 [[package]]
 name = "mccabe"
@@ -582,39 +596,36 @@
 files = [
     {file = "mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
     {file = "mdurl-0.1.2.tar.gz", hash = "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"},
 ]
 
 [[package]]
 name = "mypy-extensions"
-version = "1.0.0"
-description = "Type system extensions for programs checked with the mypy type checker."
+version = "0.4.3"
+description = "Experimental type system extensions for programs checked with the mypy typechecker."
 category = "dev"
 optional = false
-python-versions = ">=3.5"
+python-versions = "*"
 files = [
-    {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
-    {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
+    {file = "mypy_extensions-0.4.3-py2.py3-none-any.whl", hash = "sha256:090fedd75945a69ae91ce1303b5824f428daf5a028d2f6ab8a299250a846f15d"},
+    {file = "mypy_extensions-0.4.3.tar.gz", hash = "sha256:2d82818f5bb3e369420cb3c4060a7970edba416647068eb4c5343488a6c604a8"},
 ]
 
 [[package]]
 name = "packaging"
-version = "20.9"
+version = "23.0"
 description = "Core utilities for Python packages"
 category = "main"
 optional = false
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
+python-versions = ">=3.7"
 files = [
-    {file = "packaging-20.9-py2.py3-none-any.whl", hash = "sha256:67714da7f7bc052e064859c05c595155bd1ee9f69f76557e21f051443c20947a"},
-    {file = "packaging-20.9.tar.gz", hash = "sha256:5b327ac1320dc863dca72f4514ecc086f31186744b84a230374cc1fd776feae5"},
+    {file = "packaging-23.0-py3-none-any.whl", hash = "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2"},
+    {file = "packaging-23.0.tar.gz", hash = "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"},
 ]
 
-[package.dependencies]
-pyparsing = ">=2.0.2"
-
 [[package]]
 name = "paho-mqtt"
 version = "1.6.1"
 description = "MQTT version 5.0/3.1.1 client class"
 category = "main"
 optional = false
 python-versions = "*"
@@ -635,49 +646,50 @@
 files = [
     {file = "pathspec-0.11.0-py3-none-any.whl", hash = "sha256:3a66eb970cbac598f9e5ccb5b2cf58930cd8e3ed86d393d541eaf2d8b1705229"},
     {file = "pathspec-0.11.0.tar.gz", hash = "sha256:64d338d4e0914e91c1792321e6907b5a593f1ab1851de7fc269557a21b30ebbc"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "3.0.0"
+version = "2.6.2"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-3.0.0-py3-none-any.whl", hash = "sha256:b1d5eb14f221506f50d6604a561f4c5786d9e80355219694a1b244bcd96f4567"},
-    {file = "platformdirs-3.0.0.tar.gz", hash = "sha256:8a1228abb1ef82d788f74139988b137e78692984ec7b08eaa6c65f1723af28f9"},
+    {file = "platformdirs-2.6.2-py3-none-any.whl", hash = "sha256:83c8f6d04389165de7c9b6f0c682439697887bca0aa2f1c87ef1826be3584490"},
+    {file = "platformdirs-2.6.2.tar.gz", hash = "sha256:e1fea1fe471b9ff8332e229df3cb7de4f53eeea4998d3b6bfff542115e998bd2"},
 ]
 
 [package.dependencies]
 typing-extensions = {version = ">=4.4", markers = "python_version < \"3.8\""}
 
 [package.extras]
-docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=6.1.3)", "sphinx-autodoc-typehints (>=1.22,!=1.23.4)"]
-test = ["appdirs (==1.4.4)", "covdefaults (>=2.2.2)", "pytest (>=7.2.1)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
+docs = ["furo (>=2022.12.7)", "proselint (>=0.13)", "sphinx (>=5.3)", "sphinx-autodoc-typehints (>=1.19.5)"]
+test = ["appdirs (==1.4.4)", "covdefaults (>=2.2.2)", "pytest (>=7.2)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pontos"
-version = "23.2.4"
+version = "23.3.5"
 description = "Common utilities and tools maintained by Greenbone Networks"
 category = "dev"
 optional = false
 python-versions = ">=3.7,<4.0"
 files = [
-    {file = "pontos-23.2.4-py3-none-any.whl", hash = "sha256:e899da775724de7c72b0865f5fffd907cd77f0ac3c670723654a9e8a9a9ced18"},
-    {file = "pontos-23.2.4.tar.gz", hash = "sha256:92517badeab9f8c9dfb6bc60946854a9e7880d233047ce7c7157237c7d5aca1f"},
+    {file = "pontos-23.3.5-py3-none-any.whl", hash = "sha256:b82c6165c8d73ce66e234945ed52104b1895215e3dedac0fecee5326035a0df8"},
+    {file = "pontos-23.3.5.tar.gz", hash = "sha256:f19f42718faa20af54096fe88a9210f285e89b7586ffeca665ad49c9e3c7ae69"},
 ]
 
 [package.dependencies]
 colorful = ">=0.5.4,<0.6.0"
 httpx = {version = ">=0.23.0,<0.24.0", extras = ["http2"]}
 packaging = ">=20.3"
 python-dateutil = ">=2.8.2,<3.0.0"
 rich = ">=12.4.4"
+semver = ">=2.13.0,<3.0.0"
 tomlkit = ">=0.5.11"
 typing-extensions = {version = ">=4.4.0,<5.0.0", markers = "python_version < \"3.8\""}
 
 [[package]]
 name = "psutil"
 version = "5.9.4"
 description = "Cross-platform lib for process and system monitoring in Python."
@@ -741,29 +753,14 @@
 tomli = {version = ">=1.1.0", markers = "python_version < \"3.11\""}
 typing-extensions = {version = ">=3.10.0", markers = "python_version < \"3.10\""}
 
 [package.extras]
 testutil = ["gitpython (>3)"]
 
 [[package]]
-name = "pyparsing"
-version = "3.0.9"
-description = "pyparsing module - Classes and methods to define and execute parsing grammars"
-category = "main"
-optional = false
-python-versions = ">=3.6.8"
-files = [
-    {file = "pyparsing-3.0.9-py3-none-any.whl", hash = "sha256:5026bae9a10eeaefb61dab2f09052b9f4307d44aee4eda64b309723d8d206bbc"},
-    {file = "pyparsing-3.0.9.tar.gz", hash = "sha256:2b020ecf7d21b687f219b71ecad3631f644a47f01403fa1d1036b0c6416d70fb"},
-]
-
-[package.extras]
-diagrams = ["jinja2", "railroad-diagrams"]
-
-[[package]]
 name = "python-dateutil"
 version = "2.8.2"
 description = "Extensions to the standard Python datetime module"
 category = "dev"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,>=2.7"
 files = [
@@ -772,38 +769,62 @@
 ]
 
 [package.dependencies]
 six = ">=1.5"
 
 [[package]]
 name = "python-gnupg"
-version = "0.4.9"
+version = "0.5.0"
 description = "A wrapper for the Gnu Privacy Guard (GPG or GnuPG)"
 category = "main"
 optional = false
 python-versions = "*"
 files = [
-    {file = "python-gnupg-0.4.9.tar.gz", hash = "sha256:aaa748795572591aaf127b4ac8985684f3673ff82b39f370c836b006e68fc537"},
-    {file = "python_gnupg-0.4.9-py2.py3-none-any.whl", hash = "sha256:012960bde4d25dad631bb7650f563dda5e7271248a73f3584240063a293d99d8"},
+    {file = "python-gnupg-0.5.0.tar.gz", hash = "sha256:70758e387fc0e0c4badbcb394f61acbe68b34970a8fed7e0f7c89469fe17912a"},
+    {file = "python_gnupg-0.5.0-py2.py3-none-any.whl", hash = "sha256:345723a03e67b82aba0ea8ae2328b2e4a3906fbe2c18c4082285c3b01068f270"},
+]
+
+[[package]]
+name = "pytoolconfig"
+version = "1.2.5"
+description = "Python tool configuration"
+category = "dev"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "pytoolconfig-1.2.5-py3-none-any.whl", hash = "sha256:239ba9d3e537b91d0243275a497700ea39a5e259ddb80421c366e3b288bf30fe"},
+    {file = "pytoolconfig-1.2.5.tar.gz", hash = "sha256:a50f9dfe23b03a9d40414c1fdf902fefbeae12f2ac75a3c8f915944d6ffac279"},
 ]
 
+[package.dependencies]
+packaging = ">=22.0"
+platformdirs = {version = ">=1.4.4", optional = true, markers = "extra == \"global\""}
+tomli = {version = ">=2.0.1", markers = "python_version < \"3.11\""}
+typing-extensions = {version = ">=4.4.0", markers = "python_version < \"3.8\""}
+
+[package.extras]
+doc = ["sphinx (>=4.5.0)", "tabulate (>=0.8.9)"]
+gendocs = ["pytoolconfig[doc]", "sphinx (>=4.5.0)", "sphinx-autodoc-typehints (>=1.18.1)", "sphinx-rtd-theme (>=1.0.0)"]
+global = ["platformdirs (>=1.4.4)"]
+validation = ["pydantic (>=1.7.4)"]
+
 [[package]]
 name = "redis"
-version = "4.5.0"
+version = "4.5.4"
 description = "Python client for Redis database and key-value store"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "redis-4.5.0-py3-none-any.whl", hash = "sha256:98d265eea4d2255f4d0ea98c53326adf30c0a581b6cfba9d77eefb341ed8145c"},
-    {file = "redis-4.5.0.tar.gz", hash = "sha256:16135483fd35fb6c3927e4bb056780a0ad11234f61e0aa81f1db89292129c714"},
+    {file = "redis-4.5.4-py3-none-any.whl", hash = "sha256:2c19e6767c474f2e85167909061d525ed65bea9301c0770bb151e041b7ac89a2"},
+    {file = "redis-4.5.4.tar.gz", hash = "sha256:73ec35da4da267d6847e47f68730fdd5f62e2ca69e3ef5885c6a78a9374c3893"},
 ]
 
 [package.dependencies]
-async-timeout = ">=4.0.2"
+async-timeout = {version = ">=4.0.2", markers = "python_version <= \"3.11.2\""}
 importlib-metadata = {version = ">=1.0", markers = "python_version < \"3.8\""}
 typing-extensions = {version = "*", markers = "python_version < \"3.8\""}
 
 [package.extras]
 hiredis = ["hiredis (>=1.0.0)"]
 ocsp = ["cryptography (>=36.0.1)", "pyopenssl (==20.0.1)", "requests (>=2.26.0)"]
 
@@ -843,45 +864,62 @@
 typing-extensions = {version = ">=4.0.0,<5.0", markers = "python_version < \"3.9\""}
 
 [package.extras]
 jupyter = ["ipywidgets (>=7.5.1,<9)"]
 
 [[package]]
 name = "rope"
-version = "1.1.1"
+version = "1.7.0"
 description = "a python refactoring library..."
 category = "dev"
 optional = false
-python-versions = ">=3"
+python-versions = ">=3.7"
 files = [
-    {file = "rope-1.1.1-py3-none-any.whl", hash = "sha256:216390b6342bde8ef1f27a6663554de0ea0b1fdad7c421deb3d5a3f6c5fc01e7"},
-    {file = "rope-1.1.1.tar.gz", hash = "sha256:13048ff0245a0fa187f282697a55add46e4ccf083e7670f868bdf54ee9e47f2e"},
+    {file = "rope-1.7.0-py3-none-any.whl", hash = "sha256:893dd80ba7077fc9f6f42b0a849372076b70f1d6e405b9f0cc52781ffa0e6890"},
+    {file = "rope-1.7.0.tar.gz", hash = "sha256:ba39581d0f8dee4ae8b5b5e82e35d03cebad965ccb127b7eaab9755cdc85e85a"},
 ]
 
+[package.dependencies]
+pytoolconfig = {version = ">=1.2.2", extras = ["global"]}
+
 [package.extras]
-dev = ["build", "pytest", "pytest-timeout"]
+dev = ["build (>=0.7.0)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)"]
+doc = ["pytoolconfig[doc]", "sphinx (>=4.5.0)", "sphinx-autodoc-typehints (>=1.18.1)", "sphinx-rtd-theme (>=1.0.0)"]
+
+[[package]]
+name = "semver"
+version = "2.13.0"
+description = "Python helper for Semantic Versioning (http://semver.org/)"
+category = "dev"
+optional = false
+python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
+files = [
+    {file = "semver-2.13.0-py2.py3-none-any.whl", hash = "sha256:ced8b23dceb22134307c1b8abfa523da14198793d9787ac838e70e29e77458d4"},
+    {file = "semver-2.13.0.tar.gz", hash = "sha256:fa0fe2722ee1c3f57eac478820c3a5ae2f624af8264cbdf9000c980ff7f75e3f"},
+]
 
 [[package]]
 name = "sentry-sdk"
-version = "1.15.0"
+version = "1.18.0"
 description = "Python client for Sentry (https://sentry.io)"
 category = "main"
 optional = true
 python-versions = "*"
 files = [
-    {file = "sentry-sdk-1.15.0.tar.gz", hash = "sha256:69ecbb2e1ff4db02a06c4f20f6f69cb5dfe3ebfbc06d023e40d77cf78e9c37e7"},
-    {file = "sentry_sdk-1.15.0-py2.py3-none-any.whl", hash = "sha256:7ad4d37dd093f4a7cb5ad804c6efe9e8fab8873f7ffc06042dc3f3fd700a93ec"},
+    {file = "sentry-sdk-1.18.0.tar.gz", hash = "sha256:d07b9569a151033b462f7a7113ada94cc41ecf49daa83d35f5f852a0b9cf3b44"},
+    {file = "sentry_sdk-1.18.0-py2.py3-none-any.whl", hash = "sha256:714203a9adcac4a4a35e348dc9d3e294ad0200a66cdca26c068967d728f34fcb"},
 ]
 
 [package.dependencies]
 certifi = "*"
 urllib3 = {version = ">=1.26.11", markers = "python_version >= \"3.6\""}
 
 [package.extras]
 aiohttp = ["aiohttp (>=3.5)"]
+arq = ["arq (>=0.23)"]
 beam = ["apache-beam (>=2.12)"]
 bottle = ["bottle (>=0.12.13)"]
 celery = ["celery (>=3)"]
 chalice = ["chalice (>=1.16.0)"]
 django = ["django (>=1.8)"]
 falcon = ["falcon (>=1.4)"]
 fastapi = ["fastapi (>=0.79.0)"]
@@ -898,22 +936,22 @@
 sqlalchemy = ["sqlalchemy (>=1.2)"]
 starlette = ["starlette (>=0.19.1)"]
 starlite = ["starlite (>=1.48)"]
 tornado = ["tornado (>=5)"]
 
 [[package]]
 name = "setuptools"
-version = "67.2.0"
+version = "67.1.0"
 description = "Easily download, build, install, upgrade, and uninstall Python packages"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "setuptools-67.2.0-py3-none-any.whl", hash = "sha256:16ccf598aab3b506593c17378473978908a2734d7336755a8769b480906bec1c"},
-    {file = "setuptools-67.2.0.tar.gz", hash = "sha256:b440ee5f7e607bb8c9de15259dba2583dd41a38879a7abc1d43a71c59524da48"},
+    {file = "setuptools-67.1.0-py3-none-any.whl", hash = "sha256:a7687c12b444eaac951ea87a9627c4f904ac757e7abdc5aac32833234af90378"},
+    {file = "setuptools-67.1.0.tar.gz", hash = "sha256:e261cdf010c11a41cb5cb5f1bf3338a7433832029f559a6a7614bd42a967c300"},
 ]
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "pygments-github-lexers (==0.0.5)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-favicon", "sphinx-hoverxref (<2)", "sphinx-inline-tabs", "sphinx-lint", "sphinx-notfound-page (==0.8.3)", "sphinx-reredirects", "sphinxcontrib-towncrier"]
 testing = ["build[virtualenv]", "filelock (>=3.4.0)", "flake8 (<5)", "flake8-2020", "ini2toml[lite] (>=0.9)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pip (>=19.1)", "pip-run (>=8.8)", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf", "pytest-timeout", "pytest-xdist", "tomli-w (>=1.0.0)", "virtualenv (>=13.0.0)", "wheel"]
 testing-integration = ["build[virtualenv]", "filelock (>=3.4.0)", "jaraco.envs (>=2.2)", "jaraco.path (>=3.2.0)", "pytest", "pytest-enabler", "pytest-xdist", "tomli", "virtualenv (>=13.0.0)", "wheel"]
 
@@ -1100,28 +1138,28 @@
     {file = "wrapt-1.14.1-cp39-cp39-win32.whl", hash = "sha256:dee0ce50c6a2dd9056c20db781e9c1cfd33e77d2d569f5d1d9321c641bb903d5"},
     {file = "wrapt-1.14.1-cp39-cp39-win_amd64.whl", hash = "sha256:dee60e1de1898bde3b238f18340eec6148986da0455d8ba7848d50470a7a32fb"},
     {file = "wrapt-1.14.1.tar.gz", hash = "sha256:380a85cf89e0e69b7cfbe2ea9f765f004ff419f34194018a6827ac0e3edfed4d"},
 ]
 
 [[package]]
 name = "zipp"
-version = "3.12.1"
+version = "3.12.0"
 description = "Backport of pathlib-compatible object wrapper for zip files"
 category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "zipp-3.12.1-py3-none-any.whl", hash = "sha256:6c4fe274b8f85ec73c37a8e4e3fa00df9fb9335da96fb789e3b96b318e5097b3"},
-    {file = "zipp-3.12.1.tar.gz", hash = "sha256:a3cac813d40993596b39ea9e93a18e8a2076d5c378b8bc88ec32ab264e04ad02"},
+    {file = "zipp-3.12.0-py3-none-any.whl", hash = "sha256:9eb0a4c5feab9b08871db0d672745b53450d7f26992fd1e4653aa43345e97b86"},
+    {file = "zipp-3.12.0.tar.gz", hash = "sha256:73efd63936398aac78fd92b6f4865190119d6c91b531532e798977ea8dd402eb"},
 ]
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
 testing = ["flake8 (<5)", "func-timeout", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
 
 [extras]
 tracking = ["sentry-sdk"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = "^3.7"
-content-hash = "d9b97904da119746deb7964df2825363f791f6a1bcdb832b0772607fd21449fa"
+content-hash = "94d9d5f179101967644d48a72b8ab3cbad09561a4d6522808bbd6fb8e681caea"
```

### Comparing `ospd_openvas-22.4.6/pyproject.toml` & `ospd_openvas-22.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ospd-openvas"
-version = "22.4.6"
+version = "22.5.0"
 description = "ospd based scanner for openvas"
-authors = ["Greenbone Networks GmbH <info@greenbone.net>"]
+authors = ["Greenbone AG <info@greenbone.net>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/ospd-openvas"
 repository = "https://github.com/greenbone/ospd-openvas"
 # Full list: https://pypi.org/pypi?%3Aaction=list_classifiers
 classifiers=[
   "Development Status :: 4 - Beta",
@@ -42,25 +42,25 @@
   { include = "poetry.toml", format = "sdist"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 redis = ">=3.5.3,<5.0.0"
 psutil = "^5.5.1"
-packaging = "^20.4"
+packaging = ">=20.4,<24.0"
 sentry-sdk = {version="^1.1.0", optional=true}
 lxml = "^4.5.2"
 defusedxml = ">=0.6,<0.8"
 deprecated = "^1.2.10"
 paho-mqtt = ">=1.5.1"
-python-gnupg = "^0.4.8"
+python-gnupg = ">=0.4.8,<0.6.0"
 
 [tool.poetry.dev-dependencies]
 pylint = "^2.13.9"
-rope = "^1.1.1"
+rope = "^1.7.0"
 autohooks-plugin-pylint = ">=21.6.0"
 autohooks-plugin-black = ">=22.7.0"
 pontos = ">=22.7.2"
 black = ">=22.6.0"
 
 [tool.poetry.extras]
 tracking = ["sentry-sdk"]
```

### Comparing `ospd_openvas-22.4.6/tests/command/__init__.py` & `ospd_openvas-22.5.0/tests/command/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/command/test_command.py` & `ospd_openvas-22.5.0/tests/command/test_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/command/test_commands.py` & `ospd_openvas-22.5.0/tests/command/test_commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/command/test_registry.py` & `ospd_openvas-22.5.0/tests/command/test_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/dummydaemon.py` & `ospd_openvas-22.5.0/tests/dummydaemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/helper.py` & `ospd_openvas-22.5.0/tests/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/messages/__init__.py` & `ospd_openvas-22.5.0/tests/messages/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/messages/test_message.py` & `ospd_openvas-22.5.0/tests/messages/test_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/messages/test_result.py` & `ospd_openvas-22.5.0/tests/messages/test_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/messaging/__init__.py` & `ospd_openvas-22.5.0/tests/messaging/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/messaging/test_mqtt.py` & `ospd_openvas-22.5.0/tests/messaging/test_mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_argument_parser.py` & `ospd_openvas-22.5.0/tests/test_argument_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_cvss.py` & `ospd_openvas-22.5.0/tests/test_cvss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_daemon.py` & `ospd_openvas-22.5.0/tests/test_daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_datapickler.py` & `ospd_openvas-22.5.0/tests/test_datapickler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_db.py` & `ospd_openvas-22.5.0/tests/test_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
@@ -54,29 +54,44 @@
 
         self.assertEqual(mock_openvas.get_settings.call_count, 2)
 
         # should cache address
         self.assertEqual(OpenvasDB.get_database_address(), "unix:///foo/bar")
         self.assertEqual(mock_openvas.get_settings.call_count, 2)
 
-    def test_create_context_fail(self, mock_redis):
+    @patch('ospd_openvas.db.Openvas')
+    def test_create_context_fail(self, mock_openvas: MagicMock, mock_redis):
         mock_redis.from_url.side_effect = RCE
+        mock_check = mock_openvas.check.return_value
+        mock_check.get.return_value = True
+
+        OpenvasDB._db_address = None  # pylint: disable=protected-access
+        mock_settings = mock_openvas.get_settings.return_value
+        mock_settings.get.return_value = None
 
         logging.Logger.error = MagicMock()
 
         with patch.object(time, 'sleep', return_value=None):
             with self.assertRaises(SystemExit):
                 OpenvasDB.create_context()
 
         logging.Logger.error.assert_called_with(  # pylint: disable=no-member
             'Redis Error: Not possible to connect to the kb.'
         )
 
-    def test_create_context_success(self, mock_redis):
+    @patch('ospd_openvas.db.Openvas')
+    def test_create_context_success(self, mock_openvas: MagicMock, mock_redis):
         ctx = mock_redis.from_url.return_value
+        mock_check = mock_openvas.check.return_value
+        mock_check.get.return_value = True
+
+        OpenvasDB._db_address = None  # pylint: disable=protected-access
+        mock_settings = mock_openvas.get_settings.return_value
+        mock_settings.get.return_value = None
+
         ret = OpenvasDB.create_context()
         self.assertIs(ret, ctx)
 
     def test_select_database_error(self, mock_redis):
         with self.assertRaises(RequiredArgument):
             OpenvasDB.select_database(None, 1)
 
@@ -324,26 +339,46 @@
         self.assertEqual(ret, 2)
         ctx.keys.assert_called_with('*')
 
     def test_get_key_count_error(self, mock_redis):
         with self.assertRaises(RequiredArgument):
             OpenvasDB.get_key_count(None)
 
-    def test_find_database_by_pattern_none(self, mock_redis):
+    @patch('ospd_openvas.db.Openvas')
+    def test_find_database_by_pattern_none(
+        self, mock_openvas: MagicMock, mock_redis
+    ):
         ctx = mock_redis.from_url.return_value
         ctx.keys.return_value = None
 
+        mock_check = mock_openvas.check.return_value
+        mock_check.get.return_value = True
+
+        OpenvasDB._db_address = None  # pylint: disable=protected-access
+        mock_settings = mock_openvas.get_settings.return_value
+        mock_settings.get.return_value = None
+
         new_ctx, index = OpenvasDB.find_database_by_pattern('foo*', 123)
 
         self.assertIsNone(new_ctx)
         self.assertIsNone(index)
 
-    def test_find_database_by_pattern(self, mock_redis):
+    @patch('ospd_openvas.db.Openvas')
+    def test_find_database_by_pattern(
+        self, mock_openvas: MagicMock, mock_redis
+    ):
         ctx = mock_redis.from_url.return_value
 
+        mock_check = mock_openvas.check.return_value
+        mock_check.get.return_value = True
+
+        OpenvasDB._db_address = None  # pylint: disable=protected-access
+        mock_settings = mock_openvas.get_settings.return_value
+        mock_settings.get.return_value = None
+
         # keys is called twice per iteration
         ctx.keys.side_effect = [None, None, None, None, True, True]
 
         new_ctx, index = OpenvasDB.find_database_by_pattern('foo*', 123)
 
         self.assertEqual(new_ctx, ctx)
         self.assertEqual(index, 2)
@@ -685,17 +720,25 @@
 
         maindb = MainDB(ctx)
         maindb.release()
 
         ctx.hdel.assert_called_with(DBINDEX_NAME, maindb.index)
         ctx.flushdb.assert_called_with()
 
-    def test_get_new_kb_database(self, mock_redis):
+    @patch('ospd_openvas.db.Openvas')
+    def test_get_new_kb_database(self, mock_openvas: MagicMock, mock_redis):
         ctx = mock_redis.from_url.return_value
 
+        mock_check = mock_openvas.check.return_value
+        mock_check.get.return_value = True
+
+        OpenvasDB._db_address = None  # pylint: disable=protected-access
+        mock_settings = mock_openvas.get_settings.return_value
+        mock_settings.get.return_value = None
+
         maindb = MainDB(ctx)
         maindb._max_dbindex = 123  # pylint: disable=protected-access
 
         ctx.hsetnx.side_effect = [0, 0, 1]
 
         kbdb = maindb.get_new_kb_database()
```

### Comparing `ospd_openvas-22.4.6/tests/test_errors.py` & `ospd_openvas-22.5.0/tests/test_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_feed.py` & `ospd_openvas-22.5.0/tests/test_feed.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_gpg.py` & `ospd_openvas-22.5.0/tests/test_gpg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 Greenbone Networks GmbH
+# Copyright (C) 2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_lock.py` & `ospd_openvas-22.5.0/tests/test_lock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_notus.py` & `ospd_openvas-22.5.0/tests/test_notus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_nvti_cache.py` & `ospd_openvas-22.5.0/tests/test_nvti_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_openvas.py` & `ospd_openvas-22.5.0/tests/test_openvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_port_convert.py` & `ospd_openvas-22.5.0/tests/test_port_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_preferencehandler.py` & `ospd_openvas-22.5.0/tests/test_preferencehandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_protocol.py` & `ospd_openvas-22.5.0/tests/test_protocol.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_scan_and_result.py` & `ospd_openvas-22.5.0/tests/test_scan_and_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_target_convert.py` & `ospd_openvas-22.5.0/tests/test_target_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_vthelper.py` & `ospd_openvas-22.5.0/tests/test_vthelper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_vts.py` & `ospd_openvas-22.5.0/tests/test_vts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/tests/test_xml.py` & `ospd_openvas-22.5.0/tests/test_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2014-2021 Greenbone Networks GmbH
+# Copyright (C) 2014-2021 Greenbone AG
 #
 # SPDX-License-Identifier: AGPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
 # published by the Free Software Foundation, either version 3 of the
 # License, or (at your option) any later version.
```

### Comparing `ospd_openvas-22.4.6/setup.py` & `ospd_openvas-22.5.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,161 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ospd-openvas
+Version: 22.5.0
+Summary: ospd based scanner for openvas
+Home-page: https://github.com/greenbone/ospd-openvas
+License: AGPL-3.0-or-later
+Keywords: openvas,Greenbone Vulnerability Management,Vulnerability Scanning,OSP,Open Scanner Protocol
+Author: Greenbone AG
+Author-email: info@greenbone.net
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: tracking
+Requires-Dist: defusedxml (>=0.6,<0.8)
+Requires-Dist: deprecated (>=1.2.10,<2.0.0)
+Requires-Dist: lxml (>=4.5.2,<5.0.0)
+Requires-Dist: packaging (>=20.4,<24.0)
+Requires-Dist: paho-mqtt (>=1.5.1)
+Requires-Dist: psutil (>=5.5.1,<6.0.0)
+Requires-Dist: python-gnupg (>=0.4.8,<0.6.0)
+Requires-Dist: redis (>=3.5.3,<5.0.0)
+Requires-Dist: sentry-sdk (>=1.1.0,<2.0.0) ; extra == "tracking"
+Project-URL: Repository, https://github.com/greenbone/ospd-openvas
+Description-Content-Type: text/markdown
 
-packages = \
-['ospd',
- 'ospd.command',
- 'ospd_openvas',
- 'ospd_openvas.messages',
- 'ospd_openvas.messaging',
- 'tests',
- 'tests.command',
- 'tests.messages',
- 'tests.messaging']
-
-package_data = \
-{'': ['*']}
-
-modules = \
-['ospd-openvas', 'CHANGELOG', 'COPYING', 'poetry']
-install_requires = \
-['defusedxml>=0.6,<0.8',
- 'deprecated>=1.2.10,<2.0.0',
- 'lxml>=4.5.2,<5.0.0',
- 'packaging>=20.4,<21.0',
- 'paho-mqtt>=1.5.1',
- 'psutil>=5.5.1,<6.0.0',
- 'python-gnupg>=0.4.8,<0.5.0',
- 'redis>=3.5.3,<5.0.0']
-
-extras_require = \
-{'tracking': ['sentry-sdk>=1.1.0,<2.0.0']}
-
-entry_points = \
-{'console_scripts': ['ospd-openvas = ospd_openvas.daemon:main']}
-
-setup_kwargs = {
-    'name': 'ospd-openvas',
-    'version': '22.4.6',
-    'description': 'ospd based scanner for openvas',
-    'long_description': '![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)\n\n# ospd-openvas\n\n[![GitHub releases](https://img.shields.io/github/release/greenbone/ospd-openvas.svg)](https://github.com/greenbone/ospd-openvas/releases)\n[![PyPI](https://img.shields.io/pypi/v/ospd-openvas.svg)](https://pypi.org/project/ospd-openvas/)\n[![code test coverage](https://codecov.io/gh/greenbone/ospd/branch/main/graphs/badge.svg)](https://codecov.io/gh/greenbone/ospd-openvas)\n[![Build and test](https://github.com/greenbone/ospd-openvas/actions/workflows/ci-python.yml/badge.svg?branch=main)](https://github.com/greenbone/ospd-openvas/actions/workflows/ci-python.yml?query=branch%3Amain++)\n\nospd-openvas is an OSP server implementation to remotely control\n[OpenVAS Scanner](https://github.com/greenbone/openvas-scanner) and [Notus Scanner](https://github.com/greenbone/notus-scanner).\n\nOnce running, you need to configure OpenVAS Scanner and Notus Scanner for the Greenbone Vulnerability\nManager, for example via the web interface Greenbone Security Assistant. Then\nyou can create scan tasks to use both scanners.\n\n## Installation\n\n### Requirements\n\nPython 3.7 and later is supported.\n\n`ospd-openvas` has dependencies on the following Python packages:\n\n- `defusedxml`\n- `depreacted`\n- `lxml`\n- `packaging`\n- `paho-mqtt`\n- `psutil`\n- `python-gnupg`\n- `redis`\n\n### Mandatory configuration\n\nThe `ospd-openvas` startup parameter `--lock-file-dir` or the `lock_file_dir` config\nparameter of the `ospd.conf` config file needs to point to the same location / path of\nthe `gvmd` daemon and the `openvas` command line tool (Default: `<install-prefix>/var/run`).\nExamples for both are shipped within the `config` sub-folder of this project.\n\nAlso in order to be able to use Notus ospd-openvas must connect to a MQTT broker, such as [Mosquitto](https://mosquitto.org/) in order to communicate. With the parameter `--mqtt-broker-address` (Default: localhost) the correct address must be given as well as the corresponding port with `--mqtt-broker-port` (Default: 1883).\n\nPlease see the `Details` section of the [GVM release notes](https://community.greenbone.net/t/gvm-20-08-stable-initial-release-2020-08-12/6312)\nfor more details.\n\n### Optional configuration\n\nPlease note that although you can run `openvas` (launched from an `ospd-openvas`\nprocess) as a user without elevated privileges, it is recommended that you start\n`openvas` as `root` since a number of Network Vulnerability Tests (NVTs) require\nroot privileges to perform certain operations like packet forgery. If you run\n`openvas` as a user without permission to perform these operations, your scan\nresults are likely to be incomplete.\n\nAs `openvas` will be launched from an `ospd-openvas` process with sudo,\nthe next configuration is required in the sudoers file:\n\n    sudo visudo\n\nadd this line to allow the user running `ospd-openvas`, to launch `openvas`\nwith root permissions\n\n    <user> ALL = NOPASSWD: <install prefix>/sbin/openvas\n\nIf you set an install prefix, you have to update the path in the sudoers\nfile too:\n\n    Defaults        secure_path=<existing paths...>:<install prefix>/sbin\n\n## Usage\n\nThere are no special usage aspects for this module beyond the generic usage\nguide.\n\nPlease follow the general usage guide for ospd-based scanners:\n\n  <https://github.com/greenbone/ospd-openvas/blob/main/docs/USAGE-ospd-scanner.md>\n\n## Support\n\nFor any question on the usage of ospd-openvas please use the [Greenbone\nCommunity Portal](https://community.greenbone.net/). If you found a problem\nwith the software, please [create an\nissue](https://github.com/greenbone/ospd-openvas/issues) on GitHub. If you are a\nGreenbone customer you may alternatively or additionally forward your issue to\nthe Greenbone Support Portal.\n\n## Maintainer\n\nThis project is maintained by [Greenbone Networks\nGmbH](https://www.greenbone.net/).\n\n## Contributing\n\nYour contributions are highly appreciated. Please [create a pull\nrequest](https://github.com/greenbone/ospd-openvas/pulls) on GitHub. Bigger\nchanges need to be discussed with the development team via the [issues section\nat GitHub](https://github.com/greenbone/ospd-openvas/issues) first.\n\nFor development you should use [poetry](https://python-poetry.org)\nto keep your python packages separated in different environments. First install\npoetry via pip\n\n    python3 -m pip install --user poetry\n\nAfterwards run\n\n    poetry install\n\nin the checkout directory of ospd-openvas (the directory containing the\n`pyproject.toml` file) to install all dependencies including the packages only\nrequired for development.\n\nThe ospd-openvas repository uses [autohooks](https://github.com/greenbone/autohooks)\nto apply linting and auto formatting via git hooks. Please ensure the git hooks\nare active.\n\n    poetry install\n    poetry run autohooks activate --force\n\n## License\n\nCopyright (C) 2018-2022 [Greenbone Networks GmbH](https://www.greenbone.net/)\n\nLicensed under the [GNU Affero General Public License v3.0 or later](COPYING).\n',
-    'author': 'Greenbone Networks GmbH',
-    'author_email': 'info@greenbone.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/greenbone/ospd-openvas',
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+![Greenbone Logo](https://www.greenbone.net/wp-content/uploads/gb_new-logo_horizontal_rgb_small.png)
 
+# ospd-openvas
+
+[![GitHub releases](https://img.shields.io/github/release/greenbone/ospd-openvas.svg)](https://github.com/greenbone/ospd-openvas/releases)
+[![PyPI](https://img.shields.io/pypi/v/ospd-openvas.svg)](https://pypi.org/project/ospd-openvas/)
+[![Build and test](https://github.com/greenbone/ospd-openvas/actions/workflows/ci-python.yml/badge.svg?branch=main)](https://github.com/greenbone/ospd-openvas/actions/workflows/ci-python.yml?query=branch%3Amain++)
+
+ospd-openvas is an OSP server implementation to remotely control
+[OpenVAS Scanner](https://github.com/greenbone/openvas-scanner) and [Notus Scanner](https://github.com/greenbone/notus-scanner).
+
+Once running, you need to configure OpenVAS Scanner and Notus Scanner for the Greenbone Vulnerability
+Manager, for example via the web interface Greenbone Security Assistant. Then
+you can create scan tasks to use both scanners.
+
+## Installation
+
+### Requirements
+
+Python 3.7 and later is supported.
+
+`ospd-openvas` has dependencies on the following Python packages:
+
+- `defusedxml`
+- `depreacted`
+- `lxml`
+- `packaging`
+- `paho-mqtt`
+- `psutil`
+- `python-gnupg`
+- `redis`
+
+### Mandatory configuration
+
+The `ospd-openvas` startup parameter `--lock-file-dir` or the `lock_file_dir` config
+parameter of the `ospd.conf` config file needs to point to the same location / path of
+the `gvmd` daemon and the `openvas` command line tool (Default: `<install-prefix>/var/run`).
+Examples for both are shipped within the `config` sub-folder of this project.
+
+Also in order to be able to use Notus ospd-openvas must connect to a MQTT broker, such as [Mosquitto](https://mosquitto.org/) in order to communicate. With the parameter `--mqtt-broker-address` (Default: localhost) the correct address must be given as well as the corresponding port with `--mqtt-broker-port` (Default: 1883).
+
+Please see the `Details` section of the [GVM release notes](https://community.greenbone.net/t/gvm-20-08-stable-initial-release-2020-08-12/6312)
+for more details.
+
+### Optional configuration
+
+Please note that although you can run `openvas` (launched from an `ospd-openvas`
+process) as a user without elevated privileges, it is recommended that you start
+`openvas` as `root` since a number of Network Vulnerability Tests (NVTs) require
+root privileges to perform certain operations like packet forgery. If you run
+`openvas` as a user without permission to perform these operations, your scan
+results are likely to be incomplete.
+
+As `openvas` will be launched from an `ospd-openvas` process with sudo,
+the next configuration is required in the sudoers file:
+
+    sudo visudo
+
+add this line to allow the user running `ospd-openvas`, to launch `openvas`
+with root permissions
+
+    <user> ALL = NOPASSWD: <install prefix>/sbin/openvas
+
+If you set an install prefix, you have to update the path in the sudoers
+file too:
+
+    Defaults        secure_path=<existing paths...>:<install prefix>/sbin
+
+## Usage
+
+There are no special usage aspects for this module beyond the generic usage
+guide.
+
+Please follow the general usage guide for ospd-based scanners:
+
+  <https://github.com/greenbone/ospd-openvas/blob/main/docs/USAGE-ospd-scanner.md>
+
+## Support
+
+For any question on the usage of ospd-openvas please use the [Greenbone
+Community Portal](https://community.greenbone.net/). If you found a problem
+with the software, please [create an
+issue](https://github.com/greenbone/ospd-openvas/issues) on GitHub. If you are a
+Greenbone customer you may alternatively or additionally forward your issue to
+the Greenbone Support Portal.
+
+## Maintainer
+
+This project is maintained by [Greenbone Networks
+GmbH](https://www.greenbone.net/).
+
+## Contributing
+
+Your contributions are highly appreciated. Please [create a pull
+request](https://github.com/greenbone/ospd-openvas/pulls) on GitHub. Bigger
+changes need to be discussed with the development team via the [issues section
+at GitHub](https://github.com/greenbone/ospd-openvas/issues) first.
+
+For development you should use [poetry](https://python-poetry.org)
+to keep your python packages separated in different environments. First install
+poetry via pip
+
+    python3 -m pip install --user poetry
+
+Afterwards run
+
+    poetry install
+
+in the checkout directory of ospd-openvas (the directory containing the
+`pyproject.toml` file) to install all dependencies including the packages only
+required for development.
+
+The ospd-openvas repository uses [autohooks](https://github.com/greenbone/autohooks)
+to apply linting and auto formatting via git hooks. Please ensure the git hooks
+are active.
+
+    poetry install
+    poetry run autohooks activate --force
+
+## License
+
+Copyright (C) 2018-2022 [Greenbone AG](https://www.greenbone.net/)
+
+Licensed under the [GNU Affero General Public License v3.0 or later](COPYING).
 
-setup(**setup_kwargs)
```

