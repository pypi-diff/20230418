# Comparing `tmp/PrSpiders-0.3.2.tar.gz` & `tmp/PrSpiders-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.3.2.tar", last modified: Tue Apr 18 02:50:26 2023, max compression
+gzip compressed data, was "PrSpiders-0.3.3.tar", last modified: Tue Apr 18 06:08:51 2023, max compression
```

## Comparing `PrSpiders-0.3.2.tar` & `PrSpiders-0.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:50:26.601161 PrSpiders-0.3.2/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.2/LICENSE.txt
--rw-rw-rw-   0        0        0     4583 2023-04-18 02:50:26.566156 PrSpiders-0.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 02:50:25.974155 PrSpiders-0.3.2/PrSpider/
--rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.2/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.2/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11166 2023-04-17 02:59:19.000000 PrSpiders-0.3.2/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     4073 2023-04-18 02:20:24.000000 PrSpiders-0.3.2/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.2/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:50:26.189157 PrSpiders-0.3.2/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4583 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 02:50:26.276159 PrSpiders-0.3.2/pkg/
--rw-rw-rw-   0        0        0        0 2023-03-31 05:23:03.000000 PrSpiders-0.3.2/pkg/__init.py
--rw-rw-rw-   0        0        0        0 2023-04-17 12:21:36.000000 PrSpiders-0.3.2/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:50:26.504165 PrSpiders-0.3.2/pkg/prspider/
--rw-rw-rw-   0        0        0     1166 2023-04-18 02:49:55.000000 PrSpiders-0.3.2/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.3.2/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.3.2/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      494 2023-04-18 01:45:59.000000 PrSpiders-0.3.2/pkg/prspider/start.py
--rw-rw-rw-   0        0        0       42 2023-04-18 02:50:26.602157 PrSpiders-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-04-18 02:49:58.000000 PrSpiders-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:08:51.331638 PrSpiders-0.3.3/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     4583 2023-04-18 06:08:51.299629 PrSpiders-0.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 06:08:51.155634 PrSpiders-0.3.3/PrSpider/
+-rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.3/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.3/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11191 2023-04-18 06:06:03.000000 PrSpiders-0.3.3/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     4073 2023-04-18 02:20:24.000000 PrSpiders-0.3.3/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.3/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:08:51.224635 PrSpiders-0.3.3/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4583 2023-04-18 06:08:50.000000 PrSpiders-0.3.3/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-04-18 06:08:50.000000 PrSpiders-0.3.3/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:08:50.000000 PrSpiders-0.3.3/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 06:08:50.000000 PrSpiders-0.3.3/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-18 06:08:50.000000 PrSpiders-0.3.3/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 06:08:50.000000 PrSpiders-0.3.3/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 06:08:51.248633 PrSpiders-0.3.3/pkg/
+-rw-rw-rw-   0        0        0        0 2023-03-31 05:23:03.000000 PrSpiders-0.3.3/pkg/__init.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:21:36.000000 PrSpiders-0.3.3/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:08:51.292635 PrSpiders-0.3.3/pkg/prspider/
+-rw-rw-rw-   0        0        0     1173 2023-04-18 06:07:28.000000 PrSpiders-0.3.3/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.3.3/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.3.3/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-04-18 01:45:59.000000 PrSpiders-0.3.3/pkg/prspider/start.py
+-rw-rw-rw-   0        0        0       42 2023-04-18 06:08:51.333635 PrSpiders-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-04-18 06:08:42.000000 PrSpiders-0.3.3/setup.py
```

### Comparing `PrSpiders-0.3.2/LICENSE.txt` & `PrSpiders-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.2/PKG-INFO` & `PrSpiders-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.3.2
+Version: 0.3.3
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.3.2/PrSpider/PrSpiders.py` & `PrSpiders-0.3.3/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.2/PrSpider/pxpath.py` & `PrSpiders-0.3.3/PrSpider/pxpath.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from urllib.parse import urljoin
 import re, time, copy
 from lxml import etree
 from datetime import timedelta, datetime
-from table_parse import tb_parse
 import unicodedata
 from .PrSpiders import logging
 
 
 class Xpath(object):
-    def __init__(self, response, encoding='utf-8'):
+    def __init__(self, response, encoding="utf-8"):
         if isinstance(response, str):
             self.res = etree.HTML(response)
         else:
             response.encoding = encoding
             self.res = etree.HTML(response.text)
 
-    def xpath(self, x=None, filter='style|script', character=True, is_list=False, easy=False, rule=None):
+    def xpath(
+        self,
+        x=None,
+        filter="style|script",
+        character=True,
+        is_list=False,
+        easy=False,
+        rule=None,
+    ):
         """
         x: xpath 语法
         filter: 过滤器
         character: join方法带换行
         is_list: 是否为列表 True 列表,
         easy: xpath默认子集关系
         rule: 正则提取
@@ -27,101 +34,91 @@
         try:
             self.treeres = xpath_filter(self.res, filter)
             self.treeres = self.treeres.xpath(x)
             return prxpath(xp=self.treeres, xp_rule=x)
         except Exception as e:
             logging.error(e)
 
-    def xxpath(self, x=None):
-        return self.res.xpath(x)
-
-    def dpath(self, x=None, rule=None):
-        x = x.split('|')
-        x = [i + '//text()' if '/@' not in i else i for i in x]
-        x = '|'.join(x)
-        obj = self.res.xpath(x)
-        obj = [i.replace('\n', '').strip() for i in obj]
-        obj = ' '.join(obj)
-        obj = self.process_date(data=obj, rule=rule)
-        return obj
-
-    def tbxpath(self, tb_xpath=None, p='S', text=None, lable='th'):
-        if text is None:
-            text = self.res
-        return tb_parse.tbxpath(tb_xpath=tb_xpath, p=p, text=text, lable=lable)
-
-    def fxpath(self, x=None, p='', h='', rule=None):
-        le = x.split('|')
+    def fxpath(self, x=None, p="", h="", rule=None):
+        le = x.split("|")
         if len(le) > 1:
-            x = x.split('|')
+            x = x.split("|")
             for item in x:
-                p += item + '//text()|'
-                h += item + '//@href|'
+                p += item + "//text()|"
+                h += item + "//@href|"
             p = p[:-1]
             h = h[:-1]
         else:
-            p = x + '//text()'
-            h = x + '//@href'
+            p = x + "//text()"
+            h = x + "//@href"
 
         filename = self.res.xpath(p) or None
         filelink = self.res.xpath(h) or None
         fn = []
         fk = []
         try:
             if filename is not None and filelink is not None:
                 for i in range(len(filelink)):
                     is_file = bool(
-                        re.search(r'(\.tar|\.shtml|\.zip|\.pdf|\.png|\.doc|\.txt|\.ppt|\.html|\.xls|\.rar|\.jpg)',
-                                  str(filename[i])))
+                        re.search(
+                            r"(\.tar|\.shtml|\.zip|\.pdf|\.png|\.doc|\.txt|\.ppt|\.html|\.xls|\.rar|\.jpg)",
+                            str(filename[i]),
+                        )
+                    )
                     is_link = bool(
-                        re.search(r'(\.tar|\.shtml|\.zip|\.pdf|\.png|\.doc|\.txt|\.ppt|\.html|\.xls|\.rar|\.jpg)',
-                                  str(filelink[i])))
+                        re.search(
+                            r"(\.tar|\.shtml|\.zip|\.pdf|\.png|\.doc|\.txt|\.ppt|\.html|\.xls|\.rar|\.jpg)",
+                            str(filelink[i]),
+                        )
+                    )
                     if is_file or is_link:
                         fn.append(filename[i])
                         fk.append(filelink[i])
                     else:
                         pass
                 if fn is not None and fk is not None:
-                    filename = '|'.join(fn)
-                    filename = self.replace(filename).replace('\n', '')
+                    filename = "|".join(fn)
+                    filename = self.replace(filename).replace("\n", "")
                     filelink = [urljoin(rule, i) for i in fk]
-                    filelink = '|'.join(filelink)
+                    filelink = "|".join(filelink)
 
                 if len(filelink) == 0 or len(filename) == 0:
                     return None, None
                 else:
                     return filename, filelink
             else:
                 return None, None
         except:
             return None, None
 
     def replace(self, str):
-        result = re.sub(r'(\\u[a-zA-Z0-9]{4})', lambda x: x.group(
-            1).encode("utf-8").decode("unicode-escape"), str)
-        result = re.sub(r'(\\r|\\n|\\t|\xa0|\\u[0-9]{4})', lambda x: '', result)
-        result = unicodedata.normalize('NFKC', result)
+        result = re.sub(
+            r"(\\u[a-zA-Z0-9]{4})",
+            lambda x: x.group(1).encode("utf-8").decode("unicode-escape"),
+            str,
+        )
+        result = re.sub(r"(\\r|\\n|\\t|\xa0|\\u[0-9]{4})", lambda x: "", result)
+        result = unicodedata.normalize("NFKC", result)
         return result.strip()
 
     def process_text(self, obj, character=True, is_list=False):
         try:
             obj = [self.replace(i) for i in obj]
             obj = [i for i in obj if len(i) > 0]
             if is_list:
                 return obj
-            character = '\n' if character else ''
+            character = "\n" if character else ""
             result = character.join(obj)
             return result
         except Exception as e:
             print(e)
             return None
 
 
-class prxpath():
-
+class prxpath:
     def __init__(self, xp=None, xp_rule=None):
         self.xp = xp
 
         self._expr = xp_rule
 
     def getall(self):
         if isinstance(self.xp, list):
@@ -140,35 +137,42 @@
     def text(self, lists=False, warps=0, repl=True):
         """
         :param lists: 是否返回列表,True返回列表
         :param warps: 换行符合 0*\n
         :param repl: 文本进行格式化
         :return:  返回解析文本的字符串或者列表
         """
-        text_xpath = './/text()'
-        if 'text()' in self._expr:
+        text_xpath = ".//text()"
+        if "text()" in self._expr:
             return self.xp
-        warps = '\n' * warps
+        warps = "\n" * warps
         if isinstance(self.xp, list):
             self.result = [_.xpath(text_xpath) for _ in self.xp]
             if lists is False:
-                self.result = [f'{warps}'.join([replace(i) for i in _]) for _ in self.result] if repl is True else [
-                    f'{warps}'.join(_) for _ in self.result]
+                self.result = (
+                    [f"{warps}".join([replace(i) for i in _]) for _ in self.result]
+                    if repl is True
+                    else [f"{warps}".join(_) for _ in self.result]
+                )
                 self.result = [replace(_) for _ in self.result]
-                self.result = [_ for _ in self.result if _ != '']
-                self.result = f'{warps}'.join(self.result) if len(self.result) == 1 else self.result
+                self.result = [_ for _ in self.result if _ != ""]
+                self.result = (
+                    f"{warps}".join(self.result)
+                    if len(self.result) == 1
+                    else self.result
+                )
             else:
-                self.result = [f'{warps}'.join(_) for _ in self.result]
+                self.result = [f"{warps}".join(_) for _ in self.result]
                 self.result = [replace(_) for _ in self.result] if repl else self.result
 
         else:
             self.result = self.xp.xpath(text_xpath)
             if lists is False:
                 self.result = [replace(_) for _ in self.result] if repl else self.result
-                self.result = f'{warps}'.join(self.result)
+                self.result = f"{warps}".join(self.result)
 
         return self.result
 
     def date(self):
         text = self.text()
         if isinstance(text, str):
             return Process_Date.process_date(text)
@@ -177,15 +181,15 @@
 
     def __str__(self) -> str:
         data = self.xp
         return f"<{type(self).__name__} xpath={self._expr!r} data={data}>"
 
 
 def replace(str):
-    result = re.sub('([\r]|[\n]|[\t]|[\xa0])', lambda x: '', str)
+    result = re.sub("([\r]|[\n]|[\t]|[\xa0])", lambda x: "", str)
     return result.strip()
 
 
 class Process_Date:
     """处理时间类"""
 
     @classmethod
@@ -199,101 +203,123 @@
         except Exception as e:
             logging.error(e)
             return None
 
     @classmethod
     def repl_date(self, l: list):
         if len(l) > 1:
-            raise ValueError('匹配时间数量超过一个')
-        res = ''.join(l).strip()
-        res = re.sub('年|月|/', '-', res)
-        res = re.sub('日|秒', '', res)
-        res = re.sub('时|分|：', ':', res)
+            raise ValueError("匹配时间数量超过一个")
+        res = "".join(l).strip()
+        res = re.sub("年|月|/", "-", res)
+        res = re.sub("日|秒", "", res)
+        res = re.sub("时|分|：", ":", res)
         return self.timechange(res)
 
     @classmethod
     def timechange(self, start_date):
-        daterule = '%Y-%m-%d' if ':' not in start_date else '%Y-%m-%d %H:%M:%S'
+        daterule = "%Y-%m-%d" if ":" not in start_date else "%Y-%m-%d %H:%M:%S"
         dateres = datetime.strptime(start_date, daterule)
         return dateres
 
     @classmethod
     def parse_time(self, s_time):
-        result_time = ''
-        start_rule = '(\d{4}\S\d{1,2}\S\d{1,2}\S? \d{1,2}时\d{1,2}分\d{1,2}秒' \
-                     '|\d{4}\S\d{1,2}\S\d{1,2}\S? \d{1,2}时\d{1,2}分\d{1,2}' \
-                     '|\d{4}\S\d{1,2}\S\d{1,2}\S? \d{1,2}:\d{1,2}:\d{1,2}' \
-                     '|\d{4}\S\d{1,2}\S\d{1,2}\S? \d{1,2}：\d{1,2}：\d{1,2}' \
-                     '|\d{4}\S\d{1,2}\S\d{1,2}\S?)'
+        result_time = ""
+        start_rule = (
+            "(\d{4}\S\d{1,2}\S\d{1,2}\S? \d{1,2}时\d{1,2}分\d{1,2}秒"
+            "|\d{4}\S\d{1,2}\S\d{1,2}\S? \d{1,2}时\d{1,2}分\d{1,2}"
+            "|\d{4}\S\d{1,2}\S\d{1,2}\S? \d{1,2}:\d{1,2}:\d{1,2}"
+            "|\d{4}\S\d{1,2}\S\d{1,2}\S? \d{1,2}：\d{1,2}：\d{1,2}"
+            "|\d{4}\S\d{1,2}\S\d{1,2}\S?)"
+        )
         # 1、2017-06-15
         res = re.findall(start_rule, s_time)
         if res:
             result_time = self.repl_date(res)
         # 6天前
-        elif u'天前' in s_time:
-            days = re.findall(u'(\d+)天前', s_time)[0]
-            result_time = (datetime.now() - timedelta(days=int(days))).strftime("%Y-%m-%d %H:%M:%S")
+        elif "天前" in s_time:
+            days = re.findall("(\d+)天前", s_time)[0]
+            result_time = (datetime.now() - timedelta(days=int(days))).strftime(
+                "%Y-%m-%d %H:%M:%S"
+            )
 
         # 昨天 18:03
-        elif u'昨天' in s_time:
-            last_time = re.findall(r'.*?(\d{1,2}:\d{1,2})', s_time)[0]
+        elif "昨天" in s_time:
+            last_time = re.findall(r".*?(\d{1,2}:\d{1,2})", s_time)[0]
             days_ago = datetime.now() - timedelta(days=int(1))
-            y_m_d = str(days_ago.year) + '-' + str(days_ago.month) + '-' + str(days_ago.day)
-            _time = y_m_d + ' ' + last_time
-            result_time = time.strftime("%Y-%m-%d %H:%M:%S", time.strptime(_time, "%Y-%m-%d %H:%M"))
+            y_m_d = (
+                str(days_ago.year) + "-" + str(days_ago.month) + "-" + str(days_ago.day)
+            )
+            _time = y_m_d + " " + last_time
+            result_time = time.strftime(
+                "%Y-%m-%d %H:%M:%S", time.strptime(_time, "%Y-%m-%d %H:%M")
+            )
 
-        elif u'前天' in s_time:
-            last_time = re.findall(r'.*?(\d{1,2}:\d{1,2})', s_time)[0]
+        elif "前天" in s_time:
+            last_time = re.findall(r".*?(\d{1,2}:\d{1,2})", s_time)[0]
             days_ago = datetime.now() - timedelta(days=int(2))
-            y_m_d = str(days_ago.year) + '-' + str(days_ago.month) + '-' + str(days_ago.day)
-            _time = y_m_d + ' ' + last_time
-            result_time = time.strftime("%Y-%m-%d %H:%M:%S", time.strptime(_time, "%Y-%m-%d %H:%M"))
+            y_m_d = (
+                str(days_ago.year) + "-" + str(days_ago.month) + "-" + str(days_ago.day)
+            )
+            _time = y_m_d + " " + last_time
+            result_time = time.strftime(
+                "%Y-%m-%d %H:%M:%S", time.strptime(_time, "%Y-%m-%d %H:%M")
+            )
 
         # 28分钟前
-        elif u'分钟前' in s_time:
-            minutes = re.findall(u'(\d+)分钟', s_time)[0]
-            minutes_ago = (datetime.now() - timedelta(minutes=int(minutes))).strftime("%Y-%m-%d %H:%M:%S")
+        elif "分钟前" in s_time:
+            minutes = re.findall("(\d+)分钟", s_time)[0]
+            minutes_ago = (datetime.now() - timedelta(minutes=int(minutes))).strftime(
+                "%Y-%m-%d %H:%M:%S"
+            )
             result_time = minutes_ago
 
-        elif u'秒前' in s_time:
-            second = re.findall(u'(\d+)秒前', s_time)[0]
-            second_ago = (datetime.now() - timedelta(seconds=int(second))).strftime("%Y-%m-%d %H:%M:%S")
+        elif "秒前" in s_time:
+            second = re.findall("(\d+)秒前", s_time)[0]
+            second_ago = (datetime.now() - timedelta(seconds=int(second))).strftime(
+                "%Y-%m-%d %H:%M:%S"
+            )
             result_time = second_ago
 
         # 06-29 1月12日
-        elif re.findall(r'\d{1,2}-\d{1,2}|\d{1,2}月\d{1,2}日', s_time) and len(s_time) <= 5:
-            s_time = s_time.replace('月', '-').replace('日', '')
+        elif (
+            re.findall(r"\d{1,2}-\d{1,2}|\d{1,2}月\d{1,2}日", s_time) and len(s_time) <= 5
+        ):
+            s_time = s_time.replace("月", "-").replace("日", "")
             now_year = str(datetime.now().year)
-            _time = now_year + '-' + s_time
-            result_time = time.strftime("%Y-%m-%d %H:%M:%S", time.strptime(_time, "%Y-%m-%d"))
+            _time = now_year + "-" + s_time
+            result_time = time.strftime(
+                "%Y-%m-%d %H:%M:%S", time.strptime(_time, "%Y-%m-%d")
+            )
 
         # 1小时前
-        elif u'小时前' in s_time:
-            hours = re.findall(u'(\d+|半)小时前', s_time)[0]
-            hours = 0.5 if hours == '半' else hours
-            hours_ago = (datetime.now() - timedelta(hours=float(hours))).strftime("%Y-%m-%d %H:%M:%S")
+        elif "小时前" in s_time:
+            hours = re.findall("(\d+|半)小时前", s_time)[0]
+            hours = 0.5 if hours == "半" else hours
+            hours_ago = (datetime.now() - timedelta(hours=float(hours))).strftime(
+                "%Y-%m-%d %H:%M:%S"
+            )
             result_time = hours_ago
 
         return result_time
 
     @classmethod
     def parse_txt(self, data):
-        while '  ' in data:
-            data = data.replace('  ', ' ')
+        while "  " in data:
+            data = data.replace("  ", " ")
         return data
 
 
 def xpath_filter(response=None, filter=None):
-    if filter is None or filter == '':
+    if filter is None or filter == "":
         return response
     else:
         response = copy.deepcopy(response)
-        filter_num = filter.split('|')
+        filter_num = filter.split("|")
         if len(filter_num) > 1:
-            filter = filter.split('|')
-            filter = '//' + '|//'.join(filter)
+            filter = filter.split("|")
+            filter = "//" + "|//".join(filter)
         else:
-            filter = '//' + filter
+            filter = "//" + filter
         ele = response.xpath(filter)
         for e in ele:
             e.getparent().remove(e)
         return response
```

### Comparing `PrSpiders-0.3.2/PrSpider/requestXpath.py` & `PrSpiders-0.3.3/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.2/PrSpider/useragent.py` & `PrSpiders-0.3.3/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.2/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.3.3/PrSpiders.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.3.2
+Version: 0.3.3
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.3.2/README.md` & `PrSpiders-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.2/setup.py` & `PrSpiders-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

