# Comparing `tmp/ats_case-0.4.4.tar.gz` & `tmp/ats_case-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.4.4.tar", last modified: Sat Apr 15 06:07:03 2023, max compression
+gzip compressed data, was "ats_case-0.4.5.tar", last modified: Tue Apr 18 06:40:23 2023, max compression
```

## Comparing `ats_case-0.4.4.tar` & `ats_case-0.4.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.789340 ats_case-0.4.4/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.4/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-15 06:07:03.786341 ats_case-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.415243 ats_case-0.4.4/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.4/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.618074 ats_case-0.4.4/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.4/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17491 2023-04-15 06:06:14.000000 ats_case-0.4.4/ats_case/case/command.py
--rw-rw-rw-   0        0        0    10103 2023-04-07 01:41:51.000000 ats_case-0.4.4/ats_case/case/context.py
--rw-rw-rw-   0        0        0     5317 2023-04-15 05:22:12.000000 ats_case-0.4.4/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5437 2023-04-12 01:16:48.000000 ats_case-0.4.4/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.682517 ats_case-0.4.4/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.4/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.4/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      646 2023-04-15 05:21:08.000000 ats_case-0.4.4/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.743947 ats_case-0.4.4/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.4/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.4/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2586 2023-04-12 01:16:48.000000 ats_case-0.4.4/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.777185 ats_case-0.4.4/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.4/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2089 2023-04-12 01:03:34.000000 ats_case-0.4.4/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-15 06:07:03.502130 ats_case-0.4.4/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-15 06:07:02.000000 ats_case-0.4.4/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-15 06:07:03.000000 ats_case-0.4.4/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 06:07:02.000000 ats_case-0.4.4/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-15 06:07:02.000000 ats_case-0.4.4/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 06:07:02.000000 ats_case-0.4.4/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 06:07:03.789340 ats_case-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-15 06:06:40.000000 ats_case-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.976412 ats_case-0.4.5/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-18 06:40:23.973419 ats_case-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.577253 ats_case-0.4.5/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.4.5/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.793589 ats_case-0.4.5/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.4.5/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    16904 2023-04-18 06:39:42.000000 ats_case-0.4.5/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    10337 2023-04-18 06:38:27.000000 ats_case-0.4.5/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     5317 2023-04-15 05:22:12.000000 ats_case-0.4.5/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5437 2023-04-12 01:16:48.000000 ats_case-0.4.5/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.862718 ats_case-0.4.5/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.4.5/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      381 2023-04-10 07:20:19.000000 ats_case-0.4.5/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      646 2023-04-15 05:21:08.000000 ats_case-0.4.5/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.921559 ats_case-0.4.5/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.5/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.4.5/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2586 2023-04-12 01:16:48.000000 ats_case-0.4.5/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.963447 ats_case-0.4.5/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.4.5/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2089 2023-04-12 01:03:34.000000 ats_case-0.4.5/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-18 06:40:23.668719 ats_case-0.4.5/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-18 06:40:23.000000 ats_case-0.4.5/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-18 06:40:23.000000 ats_case-0.4.5/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:40:23.000000 ats_case-0.4.5/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-18 06:40:23.000000 ats_case-0.4.5/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-18 06:40:23.000000 ats_case-0.4.5/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 06:40:23.976412 ats_case-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-18 06:39:42.000000 ats_case-0.4.5/setup.py
```

### Comparing `ats_case-0.4.4/PKG-INFO` & `ats_case-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.4.4
+Version: 0.4.5
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.4/README.md` & `ats_case-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.4/ats_case/case/command.py` & `ats_case-0.4.5/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,37 +238,23 @@
         next_frame = data.get('next_frame', None)
         if next_frame is not None:
             result = send(context,
                           todo={
                               'meter:comm': {'channel': {'type': 'RS485', 'baudrate': 9600}, 'frame': next_frame}})
             self._frame = result.get('result')
             self.decode(context, index+1)
+        else:
+            context.runtime.final_result = data.get('result')
         # 分帧处理结束
 
         if index == 0:
-            self._parse = data.get('result')
+            self._parse = context.runtime.final_result
             self._flush(context)
             return self._parse
 
-    def _handle_framing(self, context: Context, data: dict, index=0):
-        try:
-            next_frame = data.get('next_frame', None)
-        except:
-            next_frame = None
-
-        if next_frame is not None:
-            result = send(context,
-                          todo={
-                              'meter:comm': {'channel': {'type': 'RS485', 'baudrate': 9600}, 'frame': next_frame}})
-            self._frame = result.get('result')
-            data = pro.decode(
-                func.to_dict(protocol=self._protocol.name, frame=self._frame, session_key=context.session.basename))
-
-            self._handle_framing(context, data, index + 1)
-
     def _flush(self, context: Context):
         context.runtime.steps.update({context.runtime.step: func.to_dict(obj='meter', op=self._operation
                                                                          , element=self._element
                                                                          , parameter=self._parameter,
                                                                          result=self._parse)})
 
     def acv(self, context: Context):
```

### Comparing `ats_case-0.4.4/ats_case/case/context.py` & `ats_case-0.4.5/ats_case/case/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,14 +290,15 @@
             self._step = -1
             self._loop_sn = 0
             self._loop_start_step = 0
             self._loop_end_step = 0
             self._loop_count = 0
             self._loop_index = 0
             self._steps = {}
+            self._final_result = None
 
         @property
         def step(self):
             return self._step
 
         @step.setter
         def step(self, value):
@@ -343,25 +344,29 @@
         def loop_index(self, value):
             self._loop_index = value
 
         @property
         def steps(self):
             return self._steps
 
+        @property
+        def final_result(self):
+            return self._final_result
+
+        @final_result.setter
+        def final_result(self, value):
+            self._final_result = value
 
     class Session(object):
         def __init__(self, parent):
             self._basename = '{}:{}:{}'.format(parent.test_sn
-                                                 , parent.case.id, parent.meter.pos)
+                                               , parent.case.id, parent.meter.pos)
 
         def get(self, name: str, key: str):
             return mm.Dict.get('{}:{}'.format(self._basename, name), key)
 
         def set(self, name: str, key: str, data):
             return mm.Dict.put('{}:{}'.format(self._basename, name), key, data)
 
         @property
         def basename(self):
             return self._basename
-
-
-
```

### Comparing `ats_case-0.4.4/ats_case/case/executor.py` & `ats_case-0.4.5/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.4/ats_case/case/translator.py` & `ats_case-0.4.5/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.4/ats_case/common/error.py` & `ats_case-0.4.5/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.4/ats_case/manage/core.py` & `ats_case-0.4.5/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.4/ats_case/manage/start.py` & `ats_case-0.4.5/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.4/ats_case/template/testcase_v1.tmp` & `ats_case-0.4.5/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.4/ats_case.egg-info/PKG-INFO` & `ats_case-0.4.5/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.4.4
+Version: 0.4.5
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.4.4/ats_case.egg-info/SOURCES.txt` & `ats_case-0.4.5/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.4.4/setup.py` & `ats_case-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.4.4",
+    version="0.4.5",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

