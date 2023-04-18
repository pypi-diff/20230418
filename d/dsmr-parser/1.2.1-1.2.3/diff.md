# Comparing `tmp/dsmr-parser-1.2.1.tar.gz` & `tmp/dsmr-parser-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsmr-parser-1.2.1.tar", last modified: Wed Apr  5 09:22:16 2023, max compression
+gzip compressed data, was "dsmr-parser-1.2.3.tar", last modified: Tue Apr 18 18:50:01 2023, max compression
```

## Comparing `dsmr-parser-1.2.1.tar` & `dsmr-parser-1.2.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-05 09:22:16.761757 dsmr-parser-1.2.1/
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     1089 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/LICENSE
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      297 2023-04-05 09:22:16.761757 dsmr-parser-1.2.1/PKG-INFO
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    10844 2023-02-19 11:25:41.000000 dsmr-parser-1.2.1/README.rst
-drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-05 09:22:16.761757 dsmr-parser-1.2.1/dsmr_parser/
--rw-rw-r--   0 nigel     (1000) nigel     (1000)        0 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/dsmr_parser/__init__.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     2406 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/dsmr_parser/__main__.py
-drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-05 09:22:16.761757 dsmr-parser-1.2.1/dsmr_parser/clients/
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      345 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/dsmr_parser/clients/__init__.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     6147 2023-02-19 11:25:41.000000 dsmr-parser-1.2.1/dsmr_parser/clients/filereader.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     6287 2023-02-12 17:32:14.000000 dsmr-parser-1.2.1/dsmr_parser/clients/protocol.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     2168 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/dsmr_parser/clients/rfxtrx_protocol.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     4520 2023-02-19 11:25:41.000000 dsmr-parser-1.2.1/dsmr_parser/clients/serial_.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      639 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/dsmr_parser/clients/settings.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     2738 2023-02-19 11:25:41.000000 dsmr-parser-1.2.1/dsmr_parser/clients/socket_.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     1801 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/dsmr_parser/clients/telegram_buffer.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)       89 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/dsmr_parser/exceptions.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     6268 2023-02-19 11:25:41.000000 dsmr-parser-1.2.1/dsmr_parser/obis_name_mapping.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     6114 2023-02-19 11:25:41.000000 dsmr-parser-1.2.1/dsmr_parser/obis_references.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    11887 2023-02-19 11:25:41.000000 dsmr-parser-1.2.1/dsmr_parser/objects.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    13627 2023-04-05 09:09:04.000000 dsmr-parser-1.2.1/dsmr_parser/parsers.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      340 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/dsmr_parser/profile_generic_specifications.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    19026 2023-02-12 17:32:14.000000 dsmr-parser-1.2.1/dsmr_parser/telegram_specifications.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      755 2023-02-12 17:32:14.000000 dsmr-parser-1.2.1/dsmr_parser/value_types.py
-drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-05 09:22:16.761757 dsmr-parser-1.2.1/dsmr_parser.egg-info/
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      297 2023-04-05 09:22:16.000000 dsmr-parser-1.2.1/dsmr_parser.egg-info/PKG-INFO
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     1093 2023-04-05 09:22:16.000000 dsmr-parser-1.2.1/dsmr_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 nigel     (1000) nigel     (1000)        1 2023-04-05 09:22:16.000000 dsmr-parser-1.2.1/dsmr_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 nigel     (1000) nigel     (1000)       63 2023-04-05 09:22:16.000000 dsmr-parser-1.2.1/dsmr_parser.egg-info/entry_points.txt
--rw-rw-r--   0 nigel     (1000) nigel     (1000)       72 2023-04-05 09:22:16.000000 dsmr-parser-1.2.1/dsmr_parser.egg-info/requires.txt
--rw-rw-r--   0 nigel     (1000) nigel     (1000)       12 2023-04-05 09:22:16.000000 dsmr-parser-1.2.1/dsmr_parser.egg-info/top_level.txt
--rw-rw-r--   0 nigel     (1000) nigel     (1000)       38 2023-04-05 09:22:16.761757 dsmr-parser-1.2.1/setup.cfg
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      630 2023-04-05 09:18:56.000000 dsmr-parser-1.2.1/setup.py
-drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-05 09:22:16.761757 dsmr-parser-1.2.1/test/
--rw-rw-r--   0 nigel     (1000) nigel     (1000)      663 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/test/test_filereader.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    17591 2023-04-05 09:09:04.000000 dsmr-parser-1.2.1/test/test_parse_fluvius.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     9700 2023-02-12 17:32:14.000000 dsmr-parser-1.2.1/test/test_parse_iskra_ie.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     4788 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/test/test_parse_sagemcom_t210_d_r.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     4720 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/test/test_parse_v2_2.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     5180 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/test/test_parse_v3.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    12898 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/test/test_parse_v4_2.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)    14306 2023-02-19 11:25:41.000000 dsmr-parser-1.2.1/test/test_parse_v5.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     2327 2023-02-19 11:25:41.000000 dsmr-parser-1.2.1/test/test_protocol.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     2436 2023-02-19 11:25:41.000000 dsmr-parser-1.2.1/test/test_rfxtrx_protocol.py
--rw-rw-r--   0 nigel     (1000) nigel     (1000)     3535 2023-01-28 10:18:52.000000 dsmr-parser-1.2.1/test/test_telegram_buffer.py
+drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     1089 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/LICENSE
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)      297 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/PKG-INFO
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)    10844 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/README.rst
+drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/dsmr_parser/
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)        0 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/__init__.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     2406 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/__main__.py
+drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/dsmr_parser/clients/
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)      345 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/clients/__init__.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     6147 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/dsmr_parser/clients/filereader.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     6287 2023-02-12 17:32:14.000000 dsmr-parser-1.2.3/dsmr_parser/clients/protocol.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     2168 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/clients/rfxtrx_protocol.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     4520 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/dsmr_parser/clients/serial_.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)      639 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/clients/settings.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     2738 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/dsmr_parser/clients/socket_.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     1543 2023-04-12 08:58:40.000000 dsmr-parser-1.2.3/dsmr_parser/clients/telegram_buffer.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)       89 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/exceptions.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     6268 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/dsmr_parser/obis_name_mapping.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     6201 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/dsmr_parser/obis_references.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)    11887 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/dsmr_parser/objects.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)    14128 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/dsmr_parser/parsers.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)      340 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/dsmr_parser/profile_generic_specifications.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)    19026 2023-02-12 17:32:14.000000 dsmr-parser-1.2.3/dsmr_parser/telegram_specifications.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)      755 2023-02-12 17:32:14.000000 dsmr-parser-1.2.3/dsmr_parser/value_types.py
+drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/dsmr_parser.egg-info/
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)      297 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     1093 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)        1 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)       63 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/entry_points.txt
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)       72 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/requires.txt
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)       12 2023-04-18 18:50:01.000000 dsmr-parser-1.2.3/dsmr_parser.egg-info/top_level.txt
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)       38 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/setup.cfg
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)      630 2023-04-18 18:46:29.000000 dsmr-parser-1.2.3/setup.py
+drwxrwxr-x   0 nigel     (1000) nigel     (1000)        0 2023-04-18 18:50:01.561324 dsmr-parser-1.2.3/test/
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)      663 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/test/test_filereader.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)    17716 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_fluvius.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     9825 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_iskra_ie.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     4788 2023-01-28 10:18:52.000000 dsmr-parser-1.2.3/test/test_parse_sagemcom_t210_d_r.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     4845 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_v2_2.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     5305 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_v3.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)    13023 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_v4_2.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)    14431 2023-04-18 18:46:02.000000 dsmr-parser-1.2.3/test/test_parse_v5.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     2327 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/test/test_protocol.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     2436 2023-02-19 11:25:41.000000 dsmr-parser-1.2.3/test/test_rfxtrx_protocol.py
+-rw-rw-r--   0 nigel     (1000) nigel     (1000)     3535 2023-04-12 08:39:00.000000 dsmr-parser-1.2.3/test/test_telegram_buffer.py
```

### Comparing `dsmr-parser-1.2.1/LICENSE` & `dsmr-parser-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/README.rst` & `dsmr-parser-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/__main__.py` & `dsmr-parser-1.2.3/dsmr_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/clients/filereader.py` & `dsmr-parser-1.2.3/dsmr_parser/clients/filereader.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/clients/protocol.py` & `dsmr-parser-1.2.3/dsmr_parser/clients/protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/clients/rfxtrx_protocol.py` & `dsmr-parser-1.2.3/dsmr_parser/clients/rfxtrx_protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/clients/serial_.py` & `dsmr-parser-1.2.3/dsmr_parser/clients/serial_.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/clients/settings.py` & `dsmr-parser-1.2.3/dsmr_parser/clients/settings.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/clients/socket_.py` & `dsmr-parser-1.2.3/dsmr_parser/clients/socket_.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/clients/telegram_buffer.py` & `dsmr-parser-1.2.3/dsmr_parser/clients/telegram_buffer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import re
 
+# - Match all characters after start of telegram except for the start
+# itself again '^\/]+', which eliminates incomplete preceding telegrams.
+# - Do non greedy match using '?' so start is matched up to the first
+# checksum that's found.
+# - The checksum is optional '{0,4}' because not all telegram versions
+# support it.
+_FIND_TELEGRAMS_REGEX = re.compile(r"\/[^\/]+?\![A-F0-9]{0,4}\0?\r\n", re.DOTALL)
+
 
 class TelegramBuffer(object):
     """
     Used as a buffer for a stream of telegram data. Constructs full telegram
     strings from the buffered data and returns it.
     """
 
     def __init__(self):
-        self._buffer = ''
+        self._buffer = ""
 
     def get_all(self):
         """
         Remove complete telegrams from buffer and yield them.
         :rtype generator:
         """
-        for telegram in self._find_telegrams():
+        for telegram in _FIND_TELEGRAMS_REGEX.findall(self._buffer):
             self._remove(telegram)
             yield telegram
 
     def append(self, data):
         """
         Add telegram data to buffer.
         :param str data: chars, lines or full telegram strings of telegram data
@@ -33,25 +41,7 @@
         :param str telegram:
         :return:
         """
         # Remove data leading up to the telegram and the telegram itself.
         index = self._buffer.index(telegram) + len(telegram)
 
         self._buffer = self._buffer[index:]
-
-    def _find_telegrams(self):
-        """
-        Find complete telegrams in buffer from  start ('/') till ending
-        checksum ('!AB12\r\n').
-        :rtype: list
-        """
-        # - Match all characters after start of telegram except for the start
-        # itself again '^\/]+', which eliminates incomplete preceding telegrams.
-        # - Do non greedy match using '?' so start is matched up to the first
-        # checksum that's found.
-        # - The checksum is optional '{0,4}' because not all telegram versions
-        # support it.
-        return re.findall(
-            r'\/[^\/]+?\![A-F0-9]{0,4}\0?\r\n',
-            self._buffer,
-            re.DOTALL
-        )
```

### Comparing `dsmr-parser-1.2.1/dsmr_parser/obis_name_mapping.py` & `dsmr-parser-1.2.3/dsmr_parser/obis_name_mapping.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/obis_references.py` & `dsmr-parser-1.2.3/dsmr_parser/obis_references.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,123 +2,123 @@
 Contains the signatures of each telegram line.
 
 Previously contained the channel + obis reference signatures, but has been
 refactored to full line signatures to maintain backwards compatibility.
 Might be refactored in a backwards incompatible way as soon as proper telegram
 objects are introduced.
 """
-P1_MESSAGE_HEADER = r'\d-\d:0\.2\.8.+?\r\n'
-P1_MESSAGE_TIMESTAMP = r'\d-\d:1\.0\.0.+?\r\n'
-ELECTRICITY_USED_TARIFF_1 = r'\d-\d:1\.8\.1.+?\r\n'
-ELECTRICITY_USED_TARIFF_2 = r'\d-\d:1\.8\.2.+?\r\n'
-ELECTRICITY_DELIVERED_TARIFF_1 = r'\d-\d:2\.8\.1.+?\r\n'
-ELECTRICITY_DELIVERED_TARIFF_2 = r'\d-\d:2\.8\.2.+?\r\n'
-CURRENT_REACTIVE_IMPORTED = r'\d-\d:3\.7\.0.+?\r\n'
-ELECTRICITY_REACTIVE_IMPORTED_TOTAL = r'\d-\d:3\.8\.0.+?\r\n'
-ELECTRICITY_REACTIVE_IMPORTED_TARIFF_1 = r'\d-\d:3\.8\.1.+?\r\n'
-ELECTRICITY_REACTIVE_IMPORTED_TARIFF_2 = r'\d-\d:3\.8\.2.+?\r\n'
-CURRENT_REACTIVE_EXPORTED = r'\d-\d:4\.7\.0.+?\r\n'
-ELECTRICITY_REACTIVE_EXPORTED_TOTAL = r'\d-\d:4\.8\.0.+?\r\n'
-ELECTRICITY_REACTIVE_EXPORTED_TARIFF_1 = r'\d-\d:4\.8\.1.+?\r\n'
-ELECTRICITY_REACTIVE_EXPORTED_TARIFF_2 = r'\d-\d:4\.8\.2.+?\r\n'
-ELECTRICITY_ACTIVE_TARIFF = r'\d-\d:96\.14\.0.+?\r\n'
-EQUIPMENT_IDENTIFIER = r'\d-\d:96\.1\.1.+?\r\n'
-CURRENT_ELECTRICITY_USAGE = r'\d-\d:1\.7\.0.+?\r\n'
-CURRENT_ELECTRICITY_DELIVERY = r'\d-\d:2\.7\.0.+?\r\n'
-LONG_POWER_FAILURE_COUNT = r'\d-\d:96\.7\.9.+?\r\n'
-SHORT_POWER_FAILURE_COUNT = r'\d-\d:96\.7\.21.+?\r\n'
-POWER_EVENT_FAILURE_LOG = r'\d-\d:99\.97\.0.+?\r\n'
-VOLTAGE_SAG_L1_COUNT = r'\d-\d:32\.32\.0.+?\r\n'
-VOLTAGE_SAG_L2_COUNT = r'\d-\d:52\.32\.0.+?\r\n'
-VOLTAGE_SAG_L3_COUNT = r'\d-\d:72\.32\.0.+?\r\n'
-VOLTAGE_SWELL_L1_COUNT = r'\d-\d:32\.36\.0.+?\r\n'
-VOLTAGE_SWELL_L2_COUNT = r'\d-\d:52\.36\.0.+?\r\n'
-VOLTAGE_SWELL_L3_COUNT = r'\d-\d:72\.36\.0.+?\r\n'
-INSTANTANEOUS_VOLTAGE_L1 = r'\d-\d:32\.7\.0.+?\r\n'
-INSTANTANEOUS_VOLTAGE_L2 = r'\d-\d:52\.7\.0.+?\r\n'
-INSTANTANEOUS_VOLTAGE_L3 = r'\d-\d:72\.7\.0.+?\r\n'
-INSTANTANEOUS_CURRENT_L1 = r'\d-\d:31\.7\.0.+?\r\n'
-INSTANTANEOUS_CURRENT_L2 = r'\d-\d:51\.7\.0.+?\r\n'
-INSTANTANEOUS_CURRENT_L3 = r'\d-\d:71\.7\.0.+?\r\n'
-TEXT_MESSAGE_CODE = r'\d-\d:96\.13\.1.+?\r\n'
-TEXT_MESSAGE = r'\d-\d:96\.13\.0.+?\r\n'
-DEVICE_TYPE = r'\d-\d:24\.1\.0.+?\r\n'
-INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE = r'\d-\d:21\.7\.0.+?\r\n'
-INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE = r'\d-\d:41\.7\.0.+?\r\n'
-INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE = r'\d-\d:61\.7\.0.+?\r\n'
-INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE = r'\d-\d:22\.7\.0.+?\r\n'
-INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE = r'\d-\d:42\.7\.0.+?\r\n'
-INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE = r'\d-\d:62\.7\.0.+?\r\n'
-INSTANTANEOUS_REACTIVE_POWER_L1_POSITIVE = r'\d-\d:23\.7\.0.+?\r\n'
-INSTANTANEOUS_REACTIVE_POWER_L1_NEGATIVE = r'\d-\d:24\.7\.0.+?\r\n'
-INSTANTANEOUS_REACTIVE_POWER_L2_POSITIVE = r'\d-\d:43\.7\.0.+?\r\n'
-INSTANTANEOUS_REACTIVE_POWER_L2_NEGATIVE = r'\d-\d:44\.7\.0.+?\r\n'
-INSTANTANEOUS_REACTIVE_POWER_L3_POSITIVE = r'\d-\d:63\.7\.0.+?\r\n'
-INSTANTANEOUS_REACTIVE_POWER_L3_NEGATIVE = r'\d-\d:64\.7\.0.+?\r\n'
-EQUIPMENT_IDENTIFIER_GAS = r'\d-\d:96\.1\.0.+?\r\n'
+P1_MESSAGE_HEADER = r'^\d-\d:0\.2\.8.+?\r\n'
+P1_MESSAGE_TIMESTAMP = r'^\d-\d:1\.0\.0.+?\r\n'
+ELECTRICITY_USED_TARIFF_1 = r'^\d-\d:1\.8\.1.+?\r\n'
+ELECTRICITY_USED_TARIFF_2 = r'^\d-\d:1\.8\.2.+?\r\n'
+ELECTRICITY_DELIVERED_TARIFF_1 = r'^\d-\d:2\.8\.1.+?\r\n'
+ELECTRICITY_DELIVERED_TARIFF_2 = r'^\d-\d:2\.8\.2.+?\r\n'
+CURRENT_REACTIVE_IMPORTED = r'^\d-\d:3\.7\.0.+?\r\n'
+ELECTRICITY_REACTIVE_IMPORTED_TOTAL = r'^\d-\d:3\.8\.0.+?\r\n'
+ELECTRICITY_REACTIVE_IMPORTED_TARIFF_1 = r'^\d-\d:3\.8\.1.+?\r\n'
+ELECTRICITY_REACTIVE_IMPORTED_TARIFF_2 = r'^\d-\d:3\.8\.2.+?\r\n'
+CURRENT_REACTIVE_EXPORTED = r'^\d-\d:4\.7\.0.+?\r\n'
+ELECTRICITY_REACTIVE_EXPORTED_TOTAL = r'^\d-\d:4\.8\.0.+?\r\n'
+ELECTRICITY_REACTIVE_EXPORTED_TARIFF_1 = r'^\d-\d:4\.8\.1.+?\r\n'
+ELECTRICITY_REACTIVE_EXPORTED_TARIFF_2 = r'^\d-\d:4\.8\.2.+?\r\n'
+ELECTRICITY_ACTIVE_TARIFF = r'^\d-\d:96\.14\.0.+?\r\n'
+EQUIPMENT_IDENTIFIER = r'^\d-\d:96\.1\.1.+?\r\n'
+CURRENT_ELECTRICITY_USAGE = r'^\d-\d:1\.7\.0.+?\r\n'
+CURRENT_ELECTRICITY_DELIVERY = r'^\d-\d:2\.7\.0.+?\r\n'
+LONG_POWER_FAILURE_COUNT = r'^\d-\d:96\.7\.9.+?\r\n'
+SHORT_POWER_FAILURE_COUNT = r'^\d-\d:96\.7\.21.+?\r\n'
+POWER_EVENT_FAILURE_LOG = r'^\d-\d:99\.97\.0.+?\r\n'
+VOLTAGE_SAG_L1_COUNT = r'^\d-\d:32\.32\.0.+?\r\n'
+VOLTAGE_SAG_L2_COUNT = r'^\d-\d:52\.32\.0.+?\r\n'
+VOLTAGE_SAG_L3_COUNT = r'^\d-\d:72\.32\.0.+?\r\n'
+VOLTAGE_SWELL_L1_COUNT = r'^\d-\d:32\.36\.0.+?\r\n'
+VOLTAGE_SWELL_L2_COUNT = r'^\d-\d:52\.36\.0.+?\r\n'
+VOLTAGE_SWELL_L3_COUNT = r'^\d-\d:72\.36\.0.+?\r\n'
+INSTANTANEOUS_VOLTAGE_L1 = r'^\d-\d:32\.7\.0.+?\r\n'
+INSTANTANEOUS_VOLTAGE_L2 = r'^\d-\d:52\.7\.0.+?\r\n'
+INSTANTANEOUS_VOLTAGE_L3 = r'^\d-\d:72\.7\.0.+?\r\n'
+INSTANTANEOUS_CURRENT_L1 = r'^\d-\d:31\.7\.0.+?\r\n'
+INSTANTANEOUS_CURRENT_L2 = r'^\d-\d:51\.7\.0.+?\r\n'
+INSTANTANEOUS_CURRENT_L3 = r'^\d-\d:71\.7\.0.+?\r\n'
+TEXT_MESSAGE_CODE = r'^\d-\d:96\.13\.1.+?\r\n'
+TEXT_MESSAGE = r'^\d-\d:96\.13\.0.+?\r\n'
+DEVICE_TYPE = r'^\d-\d:24\.1\.0.+?\r\n'
+INSTANTANEOUS_ACTIVE_POWER_L1_POSITIVE = r'^\d-\d:21\.7\.0.+?\r\n'
+INSTANTANEOUS_ACTIVE_POWER_L2_POSITIVE = r'^\d-\d:41\.7\.0.+?\r\n'
+INSTANTANEOUS_ACTIVE_POWER_L3_POSITIVE = r'^\d-\d:61\.7\.0.+?\r\n'
+INSTANTANEOUS_ACTIVE_POWER_L1_NEGATIVE = r'^\d-\d:22\.7\.0.+?\r\n'
+INSTANTANEOUS_ACTIVE_POWER_L2_NEGATIVE = r'^\d-\d:42\.7\.0.+?\r\n'
+INSTANTANEOUS_ACTIVE_POWER_L3_NEGATIVE = r'^\d-\d:62\.7\.0.+?\r\n'
+INSTANTANEOUS_REACTIVE_POWER_L1_POSITIVE = r'^\d-\d:23\.7\.0.+?\r\n'
+INSTANTANEOUS_REACTIVE_POWER_L1_NEGATIVE = r'^\d-\d:24\.7\.0.+?\r\n'
+INSTANTANEOUS_REACTIVE_POWER_L2_POSITIVE = r'^\d-\d:43\.7\.0.+?\r\n'
+INSTANTANEOUS_REACTIVE_POWER_L2_NEGATIVE = r'^\d-\d:44\.7\.0.+?\r\n'
+INSTANTANEOUS_REACTIVE_POWER_L3_POSITIVE = r'^\d-\d:63\.7\.0.+?\r\n'
+INSTANTANEOUS_REACTIVE_POWER_L3_NEGATIVE = r'^\d-\d:64\.7\.0.+?\r\n'
+EQUIPMENT_IDENTIFIER_GAS = r'^\d-\d:96\.1\.0.+?\r\n'
 # TODO differences between gas meter readings in v3 and lower and v4 and up
-HOURLY_GAS_METER_READING = r'\d-\d:24\.2\.1.+?\r\n'
-GAS_METER_READING = r'\d-\d:24\.3\.0.+?\r\n.+?\r\n'
-ACTUAL_TRESHOLD_ELECTRICITY = r'\d-\d:17\.0\.0.+?\r\n'
-ACTUAL_SWITCH_POSITION = r'\d-\d:96\.3\.10.+?\r\n'
-VALVE_POSITION_GAS = r'\d-\d:24\.4\.0.+?\r\n'
+HOURLY_GAS_METER_READING = r'^\d-\d:24\.2\.1.+?\r\n'
+GAS_METER_READING = r'^\d-\d:24\.3\.0.+?\r\n.+?\r\n'
+ACTUAL_TRESHOLD_ELECTRICITY = r'^\d-\d:17\.0\.0.+?\r\n'
+ACTUAL_SWITCH_POSITION = r'^\d-\d:96\.3\.10.+?\r\n'
+VALVE_POSITION_GAS = r'^\d-\d:24\.4\.0.+?\r\n'
 
 # TODO 17.0.0
 # TODO 96.3.10
 
 ELECTRICITY_USED_TARIFF_ALL = (
     ELECTRICITY_USED_TARIFF_1,
     ELECTRICITY_USED_TARIFF_2
 )
 ELECTRICITY_DELIVERED_TARIFF_ALL = (
     ELECTRICITY_DELIVERED_TARIFF_1,
     ELECTRICITY_DELIVERED_TARIFF_2
 )
 
 # International generalized additions
-ELECTRICITY_IMPORTED_TOTAL = r'\d-\d:1\.8\.0.+?\r\n'  # Total imported energy register (P+)
-ELECTRICITY_EXPORTED_TOTAL = r'\d-\d:2\.8\.0.+?\r\n'  # Total exported energy register (P-)
+ELECTRICITY_IMPORTED_TOTAL = r'^\d-\d:1\.8\.0.+?\r\n'  # Total imported energy register (P+)
+ELECTRICITY_EXPORTED_TOTAL = r'^\d-\d:2\.8\.0.+?\r\n'  # Total exported energy register (P-)
 
 # International non generalized additions (country specific) / risk for necessary refactoring
-BELGIUM_VERSION_INFORMATION = r'\d-\d:96\.1\.4.+?\r\n'
-BELGIUM_EQUIPMENT_IDENTIFIER = r'\d-0:96\.1\.1.+?\r\n'
-BELGIUM_CURRENT_AVERAGE_DEMAND = r'\d-\d:1\.4\.0.+?\r\n'
-BELGIUM_MAXIMUM_DEMAND_MONTH = r'\d-\d:1\.6\.0.+?\r\n'
-BELGIUM_MAXIMUM_DEMAND_13_MONTHS = r'\d-\d:98\.1\.0.+?\r\n'
-BELGIUM_MAX_POWER_PER_PHASE = r'\d-\d:17\.0\.0.+?\r\n'  # Applicable when power limitation is active
-BELGIUM_MAX_CURRENT_PER_PHASE = r'\d-\d:31\.4\.0.+?\r\n'  # Applicable when current limitation is active
+BELGIUM_VERSION_INFORMATION = r'^\d-\d:96\.1\.4.+?\r\n'
+BELGIUM_EQUIPMENT_IDENTIFIER = r'^\d-0:96\.1\.1.+?\r\n'
+BELGIUM_CURRENT_AVERAGE_DEMAND = r'^\d-\d:1\.4\.0.+?\r\n'
+BELGIUM_MAXIMUM_DEMAND_MONTH = r'^\d-\d:1\.6\.0.+?\r\n'
+BELGIUM_MAXIMUM_DEMAND_13_MONTHS = r'^\d-\d:98\.1\.0.+?\r\n'
+BELGIUM_MAX_POWER_PER_PHASE = r'^\d-\d:17\.0\.0.+?\r\n'  # Applicable when power limitation is active
+BELGIUM_MAX_CURRENT_PER_PHASE = r'^\d-\d:31\.4\.0.+?\r\n'  # Applicable when current limitation is active
 
 # Multiple 'slaves' can be linked to the main device.
 # Mostly MBUS1 = GAS METER with values on 24.2.3
 # While WATER METER reports it's values on 24.2.1
 # The GAS METER also reports its valve state on 24.4.0
 # Dev type for gas = 7 and water = 8
-BELGIUM_MBUS1_DEVICE_TYPE = r'\d-1:24\.1\.0.+?\r\n'
-BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER = r'\d-1:96\.1\.1.+?\r\n'
-BELGIUM_MBUS1_VALVE_POSITION = r'\d-1:24\.4\.0.+?\r\n'
-BELGIUM_MBUS1_METER_READING1 = r'\d-1:24\.2\.1.+?\r\n'
-BELGIUM_MBUS1_METER_READING2 = r'\d-1:24\.2\.3.+?\r\n'
-
-BELGIUM_MBUS2_DEVICE_TYPE = r'\d-2:24\.1\.0.+?\r\n'
-BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER = r'\d-2:96\.1\.1.+?\r\n'
-BELGIUM_MBUS2_VALVE_POSITION = r'\d-2:24\.4\.0.+?\r\n'
-BELGIUM_MBUS2_METER_READING1 = r'\d-2:24\.2\.1.+?\r\n'
-BELGIUM_MBUS2_METER_READING2 = r'\d-2:24\.2\.3.+?\r\n'
-
-BELGIUM_MBUS3_DEVICE_TYPE = r'\d-3:24\.1\.0.+?\r\n'
-BELGIUM_MBUS3_EQUIPMENT_IDENTIFIER = r'\d-3:96\.1\.1.+?\r\n'
-BELGIUM_MBUS3_VALVE_POSITION = r'\d-3:24\.4\.0.+?\r\n'
-BELGIUM_MBUS3_METER_READING1 = r'\d-3:24\.2\.1.+?\r\n'
-BELGIUM_MBUS3_METER_READING2 = r'\d-3:24\.2\.3.+?\r\n'
-
-BELGIUM_MBUS4_DEVICE_TYPE = r'\d-4:24\.1\.0.+?\r\n'
-BELGIUM_MBUS4_EQUIPMENT_IDENTIFIER = r'\d-4:96\.1\.1.+?\r\n'
-BELGIUM_MBUS4_VALVE_POSITION = r'\d-4:24\.4\.0.+?\r\n'
-BELGIUM_MBUS4_METER_READING1 = r'\d-4:24\.2\.1.+?\r\n'
-BELGIUM_MBUS4_METER_READING2 = r'\d-4:24\.2\.3.+?\r\n'
-
-
-LUXEMBOURG_EQUIPMENT_IDENTIFIER = r'\d-\d:42\.0\.0.+?\r\n'  # Logical device name
-
-Q3D_EQUIPMENT_IDENTIFIER = r'\d-\d:0\.0\.0.+?\r\n'  # Logical device name
-Q3D_EQUIPMENT_STATE = r'\d-\d:96\.5\.5.+?\r\n'  # Device state (hexadecimal)
-Q3D_EQUIPMENT_SERIALNUMBER = r'\d-\d:96\.1\.255.+?\r\n'  # Device Serialnumber
+BELGIUM_MBUS1_DEVICE_TYPE = r'^\d-1:24\.1\.0.+?\r\n'
+BELGIUM_MBUS1_EQUIPMENT_IDENTIFIER = r'^\d-1:96\.1\.1.+?\r\n'
+BELGIUM_MBUS1_VALVE_POSITION = r'^\d-1:24\.4\.0.+?\r\n'
+BELGIUM_MBUS1_METER_READING1 = r'^\d-1:24\.2\.1.+?\r\n'
+BELGIUM_MBUS1_METER_READING2 = r'^\d-1:24\.2\.3.+?\r\n'
+
+BELGIUM_MBUS2_DEVICE_TYPE = r'^\d-2:24\.1\.0.+?\r\n'
+BELGIUM_MBUS2_EQUIPMENT_IDENTIFIER = r'^\d-2:96\.1\.1.+?\r\n'
+BELGIUM_MBUS2_VALVE_POSITION = r'^\d-2:24\.4\.0.+?\r\n'
+BELGIUM_MBUS2_METER_READING1 = r'^\d-2:24\.2\.1.+?\r\n'
+BELGIUM_MBUS2_METER_READING2 = r'^\d-2:24\.2\.3.+?\r\n'
+
+BELGIUM_MBUS3_DEVICE_TYPE = r'^\d-3:24\.1\.0.+?\r\n'
+BELGIUM_MBUS3_EQUIPMENT_IDENTIFIER = r'^\d-3:96\.1\.1.+?\r\n'
+BELGIUM_MBUS3_VALVE_POSITION = r'^\d-3:24\.4\.0.+?\r\n'
+BELGIUM_MBUS3_METER_READING1 = r'^\d-3:24\.2\.1.+?\r\n'
+BELGIUM_MBUS3_METER_READING2 = r'^\d-3:24\.2\.3.+?\r\n'
+
+BELGIUM_MBUS4_DEVICE_TYPE = r'^\d-4:24\.1\.0.+?\r\n'
+BELGIUM_MBUS4_EQUIPMENT_IDENTIFIER = r'^\d-4:96\.1\.1.+?\r\n'
+BELGIUM_MBUS4_VALVE_POSITION = r'^\d-4:24\.4\.0.+?\r\n'
+BELGIUM_MBUS4_METER_READING1 = r'^\d-4:24\.2\.1.+?\r\n'
+BELGIUM_MBUS4_METER_READING2 = r'^\d-4:24\.2\.3.+?\r\n'
+
+
+LUXEMBOURG_EQUIPMENT_IDENTIFIER = r'^\d-\d:42\.0\.0.+?\r\n'  # Logical device name
+
+Q3D_EQUIPMENT_IDENTIFIER = r'^\d-\d:0\.0\.0.+?\r\n'  # Logical device name
+Q3D_EQUIPMENT_STATE = r'^\d-\d:96\.5\.5.+?\r\n'  # Device state (hexadecimal)
+Q3D_EQUIPMENT_SERIALNUMBER = r'^\d-\d:96\.1\.255.+?\r\n'  # Device Serialnumber
```

### Comparing `dsmr-parser-1.2.1/dsmr_parser/objects.py` & `dsmr-parser-1.2.3/dsmr_parser/objects.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/parsers.py` & `dsmr-parser-1.2.3/dsmr_parser/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,23 @@
     def __init__(self, telegram_specification, apply_checksum_validation=True):
         """
         :param telegram_specification: determines how the telegram is parsed
         :param apply_checksum_validation: validate checksum if applicable for
             telegram DSMR version (v4 and up).
         :type telegram_specification: dict
         """
-        self.telegram_specification = telegram_specification
         self.apply_checksum_validation = apply_checksum_validation
+        self.telegram_specification = telegram_specification
+        # Regexes are compiled once to improve performance
+        self.telegram_specification_regexes = {
+            signature: re.compile(signature, re.DOTALL | re.MULTILINE)
+            for signature in self.telegram_specification['objects'].keys()
+        }
 
-    def parse(self, telegram_data, encryption_key="", authentication_key=""):  # noqa: C901
+    def parse(self, telegram_data, encryption_key="", authentication_key="", throw_ex=False):  # noqa: C901
         """
         Parse telegram from string to dict.
         The telegram str type makes python 2.x integration easier.
 
         :param str telegram_data: full telegram from start ('/') to checksum
             ('!ABCD') including line endings in between the telegram's lines
         :param str encryption_key: encryption key
@@ -76,25 +81,30 @@
 
         if self.apply_checksum_validation and self.telegram_specification['checksum_support']:
             self.validate_checksum(telegram_data)
 
         telegram = Telegram()
 
         for signature, parser in self.telegram_specification['objects'].items():
-            pattern = re.compile(signature, re.DOTALL)
+            pattern = self.telegram_specification_regexes[signature]
             matches = pattern.findall(telegram_data)
 
             # Some signatures are optional and may not be present,
             # so only parse lines that match
             for match in matches:
                 try:
                     dsmr_object = parser.parse(match)
-                except Exception:
+                except ParseError:
                     logger.error("ignore line with signature {}, because parsing failed.".format(signature),
                                  exc_info=True)
+                    if throw_ex:
+                        raise
+                except Exception as err:
+                    logger.error("Unexpected {}: {}".format(type(err), err))
+                    raise
                 else:
                     telegram.add(obis_reference=signature, dsmr_object=dsmr_object)
 
         return telegram
 
     @staticmethod
     def validate_checksum(telegram):
```

### Comparing `dsmr-parser-1.2.1/dsmr_parser/telegram_specifications.py` & `dsmr-parser-1.2.3/dsmr_parser/telegram_specifications.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser/value_types.py` & `dsmr-parser-1.2.3/dsmr_parser/value_types.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/dsmr_parser.egg-info/SOURCES.txt` & `dsmr-parser-1.2.3/dsmr_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/setup.py` & `dsmr-parser-1.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 setup(
     name='dsmr-parser',
     description='Library to parse Dutch Smart Meter Requirements (DSMR)',
     author='Nigel Dokter and many others',
     author_email='mail@nldr.net',
     license='MIT',
     url='https://github.com/ndokter/dsmr_parser',
-    version='1.2.1',
+    version='1.2.3',
     packages=find_packages(exclude=('test', 'test.*')),
     install_requires=[
         'pyserial>=3,<4',
         'pyserial-asyncio<1',
         'pytz',
         'Tailer==0.4.1',
         'dlms_cosem==21.3.2'
```

### Comparing `dsmr-parser-1.2.1/test/test_filereader.py` & `dsmr-parser-1.2.3/test/test_filereader.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/test/test_parse_fluvius.py` & `dsmr-parser-1.2.3/test/test_parse_fluvius.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,18 @@
 
 
 class TelegramParserFluviusTest(unittest.TestCase):
     """ Test parsing of a DSMR Fluvius telegram. """
 
     def test_parse(self):
         parser = TelegramParser(telegram_specifications.BELGIUM_FLUVIUS)
-        result = parser.parse(TELEGRAM_FLUVIUS_V171)
+        try:
+            result = parser.parse(TELEGRAM_FLUVIUS_V171, throw_ex=True)
+        except Exception as ex:
+            assert False, f"parse trigged an exception {ex}"
 
         # BELGIUM_VERSION_INFORMATION (0-0:96.1.4)
         assert isinstance(result[obis.BELGIUM_VERSION_INFORMATION], CosemObject)
         assert result[obis.BELGIUM_VERSION_INFORMATION].unit is None
         assert isinstance(result[obis.BELGIUM_VERSION_INFORMATION].value, str)
         assert result[obis.BELGIUM_VERSION_INFORMATION].value == '50217'
```

### Comparing `dsmr-parser-1.2.1/test/test_parse_iskra_ie.py` & `dsmr-parser-1.2.3/test/test_parse_iskra_ie.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 
 
 class TelegramParserIskraIETest(unittest.TestCase):
     """ Test parsing of a Iskra IE5 telegram. """
 
     def test_parse(self):
         parser = TelegramParser(telegram_specifications.ISKRA_IE)
-        result = parser.parse(TELEGRAM_ISKRA_IE)
+        try:
+            result = parser.parse(TELEGRAM_ISKRA_IE, throw_ex=True)
+        except Exception as ex:
+            assert False, f"parse trigged an exception {ex}"
 
         # EQUIPMENT_IDENTIFIER_GAS (0-0:96.1.0)
         assert isinstance(result[obis.EQUIPMENT_IDENTIFIER_GAS], CosemObject)
         assert result[obis.EQUIPMENT_IDENTIFIER_GAS].unit is None
         assert isinstance(result[obis.EQUIPMENT_IDENTIFIER_GAS].value, str)
         assert result[obis.EQUIPMENT_IDENTIFIER_GAS].value == '09610'
```

### Comparing `dsmr-parser-1.2.1/test/test_parse_sagemcom_t210_d_r.py` & `dsmr-parser-1.2.3/test/test_parse_sagemcom_t210_d_r.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/test/test_parse_v2_2.py` & `dsmr-parser-1.2.3/test/test_parse_v2_2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
 
 class TelegramParserV2_2Test(unittest.TestCase):
     """ Test parsing of a DSMR v2.2 telegram. """
 
     def test_parse(self):
         parser = TelegramParser(telegram_specifications.V2_2)
-        result = parser.parse(TELEGRAM_V2_2)
+        try:
+            result = parser.parse(TELEGRAM_V2_2, throw_ex=True)
+        except Exception as ex:
+            assert False, f"parse trigged an exception {ex}"
 
         # ELECTRICITY_USED_TARIFF_1 (1-0:1.8.1)
         assert isinstance(result[obis.ELECTRICITY_USED_TARIFF_1], CosemObject)
         assert result[obis.ELECTRICITY_USED_TARIFF_1].unit == 'kWh'
         assert isinstance(result[obis.ELECTRICITY_USED_TARIFF_1].value, Decimal)
         assert result[obis.ELECTRICITY_USED_TARIFF_1].value == Decimal('1.001')
```

### Comparing `dsmr-parser-1.2.1/test/test_parse_v3.py` & `dsmr-parser-1.2.3/test/test_parse_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
 
 class TelegramParserV3Test(unittest.TestCase):
     """ Test parsing of a DSMR v3 telegram. """
 
     def test_parse(self):
         parser = TelegramParser(telegram_specifications.V3)
-        result = parser.parse(TELEGRAM_V3)
+        try:
+            result = parser.parse(TELEGRAM_V3, throw_ex=True)
+        except Exception as ex:
+            assert False, f"parse trigged an exception {ex}"
 
         # ELECTRICITY_USED_TARIFF_1 (1-0:1.8.1)
         assert isinstance(result[obis.ELECTRICITY_USED_TARIFF_1], CosemObject)
         assert result[obis.ELECTRICITY_USED_TARIFF_1].unit == 'kWh'
         assert isinstance(result[obis.ELECTRICITY_USED_TARIFF_1].value, Decimal)
         assert result[obis.ELECTRICITY_USED_TARIFF_1].value == Decimal('12345.678')
```

### Comparing `dsmr-parser-1.2.1/test/test_parse_v4_2.py` & `dsmr-parser-1.2.3/test/test_parse_v4_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 
 
 class TelegramParserV4_2Test(unittest.TestCase):
     """ Test parsing of a DSMR v4.2 telegram. """
 
     def test_parse(self):
         parser = TelegramParser(telegram_specifications.V4)
-        result = parser.parse(TELEGRAM_V4_2)
+        try:
+            result = parser.parse(TELEGRAM_V4_2, throw_ex=True)
+        except Exception as ex:
+            assert False, f"parse trigged an exception {ex}"
 
         # P1_MESSAGE_HEADER (1-3:0.2.8)
         assert isinstance(result[obis.P1_MESSAGE_HEADER], CosemObject)
         assert result[obis.P1_MESSAGE_HEADER].unit is None
         assert isinstance(result[obis.P1_MESSAGE_HEADER].value, str)
         assert result[obis.P1_MESSAGE_HEADER].value == '42'
```

### Comparing `dsmr-parser-1.2.1/test/test_parse_v5.py` & `dsmr-parser-1.2.3/test/test_parse_v5.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 
 
 class TelegramParserV5Test(unittest.TestCase):
     """ Test parsing of a DSMR v5.x telegram. """
 
     def test_parse(self):
         parser = TelegramParser(telegram_specifications.V5)
-        telegram = parser.parse(TELEGRAM_V5)
+        try:
+            telegram = parser.parse(TELEGRAM_V5, throw_ex=True)
+        except Exception as ex:
+            assert False, f"parse trigged an exception {ex}"
 
         # P1_MESSAGE_HEADER (1-3:0.2.8)
         assert isinstance(telegram.P1_MESSAGE_HEADER, CosemObject)
         assert telegram.P1_MESSAGE_HEADER.unit is None
         assert isinstance(telegram.P1_MESSAGE_HEADER.value, str)
         assert telegram.P1_MESSAGE_HEADER.value == '50'
```

### Comparing `dsmr-parser-1.2.1/test/test_protocol.py` & `dsmr-parser-1.2.3/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/test/test_rfxtrx_protocol.py` & `dsmr-parser-1.2.3/test/test_rfxtrx_protocol.py`

 * *Files identical despite different names*

### Comparing `dsmr-parser-1.2.1/test/test_telegram_buffer.py` & `dsmr-parser-1.2.3/test/test_telegram_buffer.py`

 * *Files identical despite different names*

