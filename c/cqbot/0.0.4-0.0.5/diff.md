# Comparing `tmp/cqbot-0.0.4.tar.gz` & `tmp/cqbot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqbot-0.0.4.tar", last modified: Tue Feb 21 01:05:35 2023, max compression
+gzip compressed data, was "cqbot-0.0.5.tar", last modified: Mon Apr 17 22:47:44 2023, max compression
```

## Comparing `cqbot-0.0.4.tar` & `cqbot-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-02-21 01:05:35.595782 cqbot-0.0.4/
--rw-r--r--   0 yu         (501) staff       (20)     1063 2023-02-16 14:05:37.000000 cqbot-0.0.4/LICENSE
--rw-r--r--   0 yu         (501) staff       (20)     7950 2023-02-21 01:05:35.595375 cqbot-0.0.4/PKG-INFO
--rw-r--r--   0 yu         (501) staff       (20)     7571 2023-02-19 08:09:32.000000 cqbot-0.0.4/README.md
-drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-02-21 01:05:35.591911 cqbot-0.0.4/cqbot/
--rw-r--r--   0 yu         (501) staff       (20)      119 2023-02-19 07:23:57.000000 cqbot-0.0.4/cqbot/__init__.py
--rw-r--r--   0 yu         (501) staff       (20)    37544 2023-02-19 07:23:57.000000 cqbot-0.0.4/cqbot/action.py
--rw-r--r--   0 yu         (501) staff       (20)     9200 2023-02-20 15:27:59.000000 cqbot-0.0.4/cqbot/bot.py
--rw-r--r--   0 yu         (501) staff       (20)     2460 2023-02-19 07:53:39.000000 cqbot-0.0.4/cqbot/cmd.py
--rw-r--r--   0 yu         (501) staff       (20)    11209 2023-02-19 07:23:57.000000 cqbot-0.0.4/cqbot/cq.py
--rw-r--r--   0 yu         (501) staff       (20)     4323 2023-02-19 07:23:57.000000 cqbot-0.0.4/cqbot/enum.py
--rw-r--r--   0 yu         (501) staff       (20)    19764 2023-02-19 07:23:57.000000 cqbot-0.0.4/cqbot/event.py
-drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-02-21 01:05:35.594779 cqbot-0.0.4/cqbot.egg-info/
--rw-r--r--   0 yu         (501) staff       (20)     7950 2023-02-21 01:05:35.000000 cqbot-0.0.4/cqbot.egg-info/PKG-INFO
--rw-r--r--   0 yu         (501) staff       (20)      271 2023-02-21 01:05:35.000000 cqbot-0.0.4/cqbot.egg-info/SOURCES.txt
--rw-r--r--   0 yu         (501) staff       (20)        1 2023-02-21 01:05:35.000000 cqbot-0.0.4/cqbot.egg-info/dependency_links.txt
--rw-r--r--   0 yu         (501) staff       (20)       33 2023-02-21 01:05:35.000000 cqbot-0.0.4/cqbot.egg-info/requires.txt
--rw-r--r--   0 yu         (501) staff       (20)        6 2023-02-21 01:05:35.000000 cqbot-0.0.4/cqbot.egg-info/top_level.txt
--rw-r--r--   0 yu         (501) staff       (20)       38 2023-02-21 01:05:35.595914 cqbot-0.0.4/setup.cfg
--rw-r--r--   0 yu         (501) staff       (20)      847 2023-02-20 15:27:59.000000 cqbot-0.0.4/setup.py
+drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-04-17 22:47:44.267672 cqbot-0.0.5/
+-rw-r--r--   0 yu         (501) staff       (20)     1063 2023-02-16 14:05:37.000000 cqbot-0.0.5/LICENSE
+-rw-r--r--   0 yu         (501) staff       (20)     7950 2023-04-17 22:47:44.267403 cqbot-0.0.5/PKG-INFO
+-rw-r--r--   0 yu         (501) staff       (20)     7571 2023-02-19 08:09:32.000000 cqbot-0.0.5/README.md
+drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-04-17 22:47:44.264576 cqbot-0.0.5/cqbot/
+-rw-r--r--   0 yu         (501) staff       (20)      119 2023-02-19 07:23:57.000000 cqbot-0.0.5/cqbot/__init__.py
+-rw-r--r--   0 yu         (501) staff       (20)    37544 2023-02-19 07:23:57.000000 cqbot-0.0.5/cqbot/action.py
+-rw-r--r--   0 yu         (501) staff       (20)     9200 2023-02-20 15:27:59.000000 cqbot-0.0.5/cqbot/bot.py
+-rw-r--r--   0 yu         (501) staff       (20)     2451 2023-04-17 22:45:36.000000 cqbot-0.0.5/cqbot/cmd.py
+-rw-r--r--   0 yu         (501) staff       (20)    12592 2023-04-17 22:47:40.000000 cqbot-0.0.5/cqbot/cq.py
+-rw-r--r--   0 yu         (501) staff       (20)     4323 2023-02-19 07:23:57.000000 cqbot-0.0.5/cqbot/enum.py
+-rw-r--r--   0 yu         (501) staff       (20)    19764 2023-02-19 07:23:57.000000 cqbot-0.0.5/cqbot/event.py
+drwxr-xr-x   0 yu         (501) staff       (20)        0 2023-04-17 22:47:44.267041 cqbot-0.0.5/cqbot.egg-info/
+-rw-r--r--   0 yu         (501) staff       (20)     7950 2023-04-17 22:47:44.000000 cqbot-0.0.5/cqbot.egg-info/PKG-INFO
+-rw-r--r--   0 yu         (501) staff       (20)      271 2023-04-17 22:47:44.000000 cqbot-0.0.5/cqbot.egg-info/SOURCES.txt
+-rw-r--r--   0 yu         (501) staff       (20)        1 2023-04-17 22:47:44.000000 cqbot-0.0.5/cqbot.egg-info/dependency_links.txt
+-rw-r--r--   0 yu         (501) staff       (20)       33 2023-04-17 22:47:44.000000 cqbot-0.0.5/cqbot.egg-info/requires.txt
+-rw-r--r--   0 yu         (501) staff       (20)        6 2023-04-17 22:47:44.000000 cqbot-0.0.5/cqbot.egg-info/top_level.txt
+-rw-r--r--   0 yu         (501) staff       (20)       38 2023-04-17 22:47:44.267762 cqbot-0.0.5/setup.cfg
+-rw-r--r--   0 yu         (501) staff       (20)      847 2023-04-17 21:03:45.000000 cqbot-0.0.5/setup.py
```

### Comparing `cqbot-0.0.4/LICENSE` & `cqbot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.4/PKG-INFO` & `cqbot-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqbot
-Version: 0.0.4
+Version: 0.0.5
 Summary: go-cqhttp python 框架，可以用于快速塔建 bot
 Home-page: https://github.com/lhlyu/cqbot
 Author: lhlyu
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `cqbot-0.0.4/README.md` & `cqbot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.4/cqbot/action.py` & `cqbot-0.0.5/cqbot/action.py`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.4/cqbot/bot.py` & `cqbot-0.0.5/cqbot/bot.py`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.4/cqbot/cmd.py` & `cqbot-0.0.5/cqbot/cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import re
 from typing import Callable, List, Any
 from .action import Action
 from .event import EventMessage
+from .cq import CQ
 
 # def handler(act: Action, msg: EventMessage, args: List[Any]) -> bool
 CmdHandler = Callable[[Action, EventMessage, List[Any]], bool] | None
 
-rule = r'\[CQ:[\S ]+?\]'
-
 
 class Cmd:
     __cmds: dict[str, CmdHandler]
     __helps: dict[str, str]
     __commanders: dict[str, List[int]]
 
     def __init__(self, admins: List[int] = None):
@@ -60,15 +59,15 @@
         """
         # 机器人的消息过滤
         if msg.self_id == msg.user_id:
             return False
         if self.admins is not None and msg.user_id not in self.admins:
             return False
         # 将CQ码替换成空
-        prompt = re.sub(rule, ' ', msg.message).strip()
+        prompt = CQ.replace(msg.message, ' ').strip()
         # 根据空格切割参数
         args = re.split(r'\s+', prompt)
         if len(args) == 0:
             return False
         handler = self.__cmds.get(args[0], None)
         if handler is None:
             return False
```

### Comparing `cqbot-0.0.4/cqbot/cq.py` & `cqbot-0.0.5/cqbot/cq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,40 @@
-from typing import List, Callable, Any
+from typing import List, Callable, Any, Dict, Union
+import re
 
+rule = r'(\[CQ:\w+(?:,\w+\=\S+?)+\])'
 
-def escape(s, quote=True):
+
+def escape(s):
     """
     转义
     :param s:
     :param quote:
     :return:
     """
-    s = s.replace("&", "&amp;")  # Must be done first!
-    s = s.replace("<", "&lt;")
-    s = s.replace(">", "&gt;")
+
+    s = s.replace("&", "&amp;")
     s = s.replace("[", "&#91;")
     s = s.replace("]", "&#93;")
     s = s.replace(",", "&#44;")
-    if quote:
-        s = s.replace('"', "&quot;")
-        s = s.replace('\'', "&#x27;")
+    return s
+
+
+def unescape(s):
+    """
+    反转义
+    :param s:
+    :param quote:
+    :return:
+    """
+
+    s = s.replace("&amp;", "&")
+    s = s.replace("&#91;", "[")
+    s = s.replace("&#93;", "]")
+    s = s.replace("&#44;", ",")
     return s
 
 
 def g(key: str, value: Any, cond: Callable[[Any], bool], escape: bool = False, fail_break: bool = False):
     """
     :param key:
     :param value:
@@ -355,9 +369,51 @@
         :return: str
         """
         if text == '':
             return ''
 
         return f'[CQ:tts,text={text}]'
 
+    @classmethod
+    def parse(cls, message: str, code: str = '') -> Dict[str, Dict[str, Union[int, str]]]:
+        """
+        解析消息里的CQ码
+
+        例子: [CQ:tts,text=message]xy[CQ:at,qq=123,name=jack]
+
+        返回: {'tts': {'text': 'message'}, 'at': {'qq': 123, 'name': 'jack'}}
+
+        :param code: 仅解析特定的cq码， 如: face
+        :param message:
+        :return:
+        """
+        cqs: Dict[str, Dict[str, Union[int, str]]] = {}
+        for item in re.findall(rule,  message):
+            group = str(item).lstrip('[').rstrip(']').split(',')
+            if len(group) == 0:
+                continue
+            name = group[0][3:]
+            if len(code) > 0 and name != code:
+                continue
+
+            fields: Dict[str, Union[int, str]] = {}
+            for v in group[1:]:
+                cols = v.split('=', 1)
+                if len(cols) != 2:
+                    continue
+                fields[cols[0]] = unescape(cols[1])
+            cqs[name] = fields
+
+        return cqs
+
+    @classmethod
+    def replace(cls, message: str, repl: str = '') -> str:
+        """
+        替换消息里的cq码
+        :param message:
+        :param repl:
+        :return:
+        """
+        return re.sub(rule, repl, message)
+
 
 __all__ = ['CQ']
```

### Comparing `cqbot-0.0.4/cqbot/enum.py` & `cqbot-0.0.5/cqbot/enum.py`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.4/cqbot/event.py` & `cqbot-0.0.5/cqbot/event.py`

 * *Files identical despite different names*

### Comparing `cqbot-0.0.4/cqbot.egg-info/PKG-INFO` & `cqbot-0.0.5/cqbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cqbot
-Version: 0.0.4
+Version: 0.0.5
 Summary: go-cqhttp python 框架，可以用于快速塔建 bot
 Home-page: https://github.com/lhlyu/cqbot
 Author: lhlyu
 License: MIT
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `cqbot-0.0.4/setup.py` & `cqbot-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="cqbot",
-    version="0.0.4",
+    version="0.0.5",
     description="go-cqhttp python 框架，可以用于快速塔建 bot",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
```

