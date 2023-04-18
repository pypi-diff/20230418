# Comparing `tmp/PyOfficeRobot-0.1.3.tar.gz` & `tmp/PyOfficeRobot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOfficeRobot-0.1.3.tar", last modified: Mon Apr 17 13:43:48 2023, max compression
+gzip compressed data, was "PyOfficeRobot-0.1.4.tar", last modified: Tue Apr 18 13:25:54 2023, max compression
```

## Comparing `PyOfficeRobot-0.1.3.tar` & `PyOfficeRobot-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.079286 PyOfficeRobot-0.1.3/
--rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     7869 2023-04-17 13:43:48.080301 PyOfficeRobot-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.002703 PyOfficeRobot-0.1.3/PyOfficeRobot/
--rw-rw-rw-   0        0        0      120 2023-04-16 15:36:09.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.049697 PyOfficeRobot-0.1.3/PyOfficeRobot/api/
--rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/api/__init__.py
--rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/api/chat.py
--rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/api/file.py
--rw-rw-rw-   0        0        0     1625 2023-04-16 15:41:21.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/api/test.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.057208 PyOfficeRobot-0.1.3/PyOfficeRobot/core/
--rw-rw-rw-   0        0        0    13388 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/core/WeChatType.py
--rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.061229 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/
--rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/CONST.py
--rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.067229 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/dec/
--rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/dec/__init__.py
--rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/dec/act_dec.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.071747 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/decorator_utils/
--rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/decorator_utils/__init__.py
--rw-rw-rw-   0        0        0     2323 2023-03-19 12:08:23.000000 PyOfficeRobot-0.1.3/PyOfficeRobot/lib/decorator_utils/instruction_url.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.040158 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/
--rw-rw-rw-   0        0        0     7869 2023-04-17 13:43:47.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      728 2023-04-17 13:43:47.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 13:43:47.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-17 13:36:22.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-17 13:43:47.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-17 13:43:47.000000 PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7289 2023-04-02 05:09:27.000000 PyOfficeRobot-0.1.3/README.md
--rw-rw-rw-   0        0        0      785 2023-04-17 13:43:48.088315 PyOfficeRobot-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:43:48.077746 PyOfficeRobot-0.1.3/tests/
--rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.3/tests/chat.py
--rw-rw-rw-   0        0        0     1229 2023-04-17 13:43:31.000000 PyOfficeRobot-0.1.3/tests/test_file.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.735327 PyOfficeRobot-0.1.4/
+-rw-rw-rw-   0        0        0     1093 2022-09-09 17:29:26.000000 PyOfficeRobot-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     7869 2023-04-18 13:25:54.736329 PyOfficeRobot-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.648998 PyOfficeRobot-0.1.4/PyOfficeRobot/
+-rw-rw-rw-   0        0        0      120 2023-04-16 15:36:09.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.697810 PyOfficeRobot-0.1.4/PyOfficeRobot/api/
+-rw-rw-rw-   0        0        0        0 2022-09-09 17:57:22.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/api/__init__.py
+-rw-rw-rw-   0        0        0     3834 2023-03-19 10:39:04.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/api/chat.py
+-rw-rw-rw-   0        0        0     6984 2023-04-17 13:43:21.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/api/file.py
+-rw-rw-rw-   0        0        0     1625 2023-04-16 15:41:21.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/api/test.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.703805 PyOfficeRobot-0.1.4/PyOfficeRobot/core/
+-rw-rw-rw-   0        0        0    13543 2023-04-18 13:17:17.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/core/WeChatType.py
+-rw-rw-rw-   0        0        0        0 2022-09-01 13:34:44.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.708804 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/
+-rw-rw-rw-   0        0        0      117 2023-03-19 07:06:10.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/CONST.py
+-rw-rw-rw-   0        0        0        0 2022-09-12 08:16:33.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.719827 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/dec/
+-rw-rw-rw-   0        0        0        0 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/dec/__init__.py
+-rw-rw-rw-   0        0        0      385 2022-09-14 15:03:44.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/dec/act_dec.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.723812 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/decorator_utils/
+-rw-rw-rw-   0        0        0        0 2023-01-31 14:24:33.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/decorator_utils/__init__.py
+-rw-rw-rw-   0        0        0     2323 2023-03-19 12:08:23.000000 PyOfficeRobot-0.1.4/PyOfficeRobot/lib/decorator_utils/instruction_url.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.681773 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/
+-rw-rw-rw-   0        0        0     7869 2023-04-18 13:25:54.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      728 2023-04-18 13:25:54.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 13:25:54.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-17 13:36:22.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-04-18 13:25:54.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-18 13:25:54.000000 PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7289 2023-04-02 05:09:27.000000 PyOfficeRobot-0.1.4/README.md
+-rw-rw-rw-   0        0        0      785 2023-04-18 13:25:54.738327 PyOfficeRobot-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 PyOfficeRobot-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:25:54.734341 PyOfficeRobot-0.1.4/tests/
+-rw-rw-rw-   0        0        0      193 2023-02-13 13:41:39.000000 PyOfficeRobot-0.1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0       13 2023-04-17 13:43:22.000000 PyOfficeRobot-0.1.4/tests/chat.py
+-rw-rw-rw-   0        0        0     1230 2023-04-18 13:15:33.000000 PyOfficeRobot-0.1.4/tests/test_file.py
```

### Comparing `PyOfficeRobot-0.1.3/LICENSE` & `PyOfficeRobot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.3/PKG-INFO` & `PyOfficeRobot-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.3
+Version: 0.1.4
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.3 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.4 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `PyOfficeRobot-0.1.3/PyOfficeRobot/api/chat.py` & `PyOfficeRobot-0.1.4/PyOfficeRobot/api/chat.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.3/PyOfficeRobot/api/file.py` & `PyOfficeRobot-0.1.4/PyOfficeRobot/api/file.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.3/PyOfficeRobot/api/test.py` & `PyOfficeRobot-0.1.4/PyOfficeRobot/api/test.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.3/PyOfficeRobot/core/WeChatType.py` & `PyOfficeRobot-0.1.4/PyOfficeRobot/core/WeChatType.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,15 +306,16 @@
 
     ################################微信发文件崩溃 https://blog.csdn.net/weixin_45081575/article/details/126810748
 
     def test_SendFiles(self, filepath, not_exists='ignore'):
         """向当前聊天窗口发送文件
         not_exists: 如果未找到指定文件，继续或终止程序
         filepath: 要复制文件的绝对路径"""
-
+        if not Path(filepath).exists():
+            raise BaseException(f'你指定的文件不存在，请检查filepath后，重新运行：{filepath}')
         class DROPFILES(Structure):
             _fields_ = [
                 ("pFiles", c_uint),
                 ("x", c_long),
                 ("y", c_long),
                 ("fNC", c_int),
                 ("fWide", c_bool),
```

### Comparing `PyOfficeRobot-0.1.3/PyOfficeRobot/lib/decorator_utils/instruction_url.py` & `PyOfficeRobot-0.1.4/PyOfficeRobot/lib/decorator_utils/instruction_url.py`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/PKG-INFO` & `PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyOfficeRobot
-Version: 0.1.3
+Version: 0.1.4
 Summary: pip install PyOfficeRobot
 Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/README.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.3 Summary: pip install
+Metadata-Version: 2.1 Name: PyOfficeRobot Version: 0.1.4 Summary: pip install
 PyOfficeRobot Home-page: https://www.python-office.com/office/robot.html
 Author: CoderWanFeng Author-email: 1957875073@qq.com License: MIT Project-URL:
 Bug Tracker, https://github.com/CoderWanFeng/PyOfficeRobot/issues Project-URL:
 Documentation, https://github.com/CoderWanFeng/PyOfficeRobot/blob/main/
 README.md Project-URL: Source Code, https://github.com/CoderWanFeng/
 PyOfficeRobot Platform: any Requires-Python: >=3.6 Description-Content-Type:
 text/markdown License-File: LICENSE
```

### Comparing `PyOfficeRobot-0.1.3/PyOfficeRobot.egg-info/SOURCES.txt` & `PyOfficeRobot-0.1.4/PyOfficeRobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.3/README.md` & `PyOfficeRobot-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `PyOfficeRobot-0.1.3/setup.cfg` & `PyOfficeRobot-0.1.4/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 794f 6666 6963 6552 6f62 6f74   = PyOfficeRobot
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 312e  ..version = 0.1.
-00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
+00000030: 340d 0a64 6573 6372 6970 7469 6f6e 203d  4..description =
 00000040: 2070 6970 2069 6e73 7461 6c6c 2050 794f   pip install PyO
 00000050: 6666 6963 6552 6f62 6f74 0d0a 6c6f 6e67  fficeRobot..long
 00000060: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000070: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000080: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000090: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 000000a0: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
```

### Comparing `PyOfficeRobot-0.1.3/tests/test_file.py` & `PyOfficeRobot-0.1.4/tests/test_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,12 +24,12 @@
         send_message_by_time(who='每天进步一点点', message='你好', time='17:38')
 
     def test_chat_by_gpt(self):
         chat_by_gpt(who='每天进步一点点')
 
     def test_weixin_file(self):
         who = '每天进步一点点'
-        file_path = r'./chat.py'
+        file_path = r'./dfasd.py'
         # file_path = r'D:\workplace\code\github\PyOfficeRobot\tests\chat.py'
         # PyOfficeRobot.file.send_file(who, file)
         file.send_file(who, file_path)
         # file.send_file(who='每天进步一点点', file=r'D:\workplace\code\github\PyOfficeRobot\dev\contributor\gen\自动加好友\Excel_File\【企查查】查企业-高级搜索“涂料”(202302030683).xls')
```

