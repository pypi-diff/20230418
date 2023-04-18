# Comparing `tmp/ji-coursesel-0.1.3.tar.gz` & `tmp/ji-coursesel-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ji-coursesel-0.1.3.tar", last modified: Tue Jan 10 09:34:03 2023, max compression
+gzip compressed data, was "ji-coursesel-0.1.4.tar", last modified: Tue Apr 18 14:38:59 2023, max compression
```

## Comparing `ji-coursesel-0.1.3.tar` & `ji-coursesel-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-01-10 09:34:03.609455 ji-coursesel-0.1.3/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2022-12-30 03:18:49.000000 ji-coursesel-0.1.3/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      760 2023-01-10 09:34:03.609455 ji-coursesel-0.1.3/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      503 2022-12-30 04:55:07.000000 ji-coursesel-0.1.3/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-01-10 09:34:03.606120 ji-coursesel-0.1.3/courseselcli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2022-12-30 03:18:49.000000 ji-coursesel-0.1.3/courseselcli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      114 2022-12-30 03:18:49.000000 ji-coursesel-0.1.3/courseselcli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      357 2022-12-30 03:18:49.000000 ji-coursesel-0.1.3/courseselcli/coursesel.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)     9607 2023-01-10 09:32:40.000000 ji-coursesel-0.1.3/courseselcli/elector.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      820 2022-12-30 03:18:49.000000 ji-coursesel-0.1.3/courseselcli/login.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)     6322 2023-01-10 08:47:41.000000 ji-coursesel-0.1.3/courseselcli/main.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)     5082 2022-12-30 07:08:19.000000 ji-coursesel-0.1.3/courseselcli/single.py
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-01-10 09:34:03.609455 ji-coursesel-0.1.3/ji_coursesel.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      760 2023-01-10 09:34:03.000000 ji-coursesel-0.1.3/ji_coursesel.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      428 2023-01-10 09:34:03.000000 ji-coursesel-0.1.3/ji_coursesel.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-01-10 09:34:03.000000 ji-coursesel-0.1.3/ji_coursesel.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       64 2023-01-10 09:34:03.000000 ji-coursesel-0.1.3/ji_coursesel.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       36 2023-01-10 09:34:03.000000 ji-coursesel-0.1.3/ji_coursesel.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-01-10 09:34:03.000000 ji-coursesel-0.1.3/ji_coursesel.egg-info/top_level.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)      433 2023-01-10 09:34:03.609455 ji-coursesel-0.1.3/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      164 2022-12-30 03:18:49.000000 ji-coursesel-0.1.3/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-04-18 14:38:59.923922 ji-coursesel-0.1.4/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2022-12-30 03:18:49.000000 ji-coursesel-0.1.4/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      760 2023-04-18 14:38:59.923922 ji-coursesel-0.1.4/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      503 2022-12-30 04:55:07.000000 ji-coursesel-0.1.4/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-04-18 14:38:59.923922 ji-coursesel-0.1.4/courseselcli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2022-12-30 03:18:49.000000 ji-coursesel-0.1.4/courseselcli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      114 2022-12-30 03:18:49.000000 ji-coursesel-0.1.4/courseselcli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      357 2022-12-30 03:18:49.000000 ji-coursesel-0.1.4/courseselcli/coursesel.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     9525 2023-04-18 14:37:23.000000 ji-coursesel-0.1.4/courseselcli/elector.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      820 2022-12-30 03:18:49.000000 ji-coursesel-0.1.4/courseselcli/login.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)     6322 2023-04-18 14:37:38.000000 ji-coursesel-0.1.4/courseselcli/main.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)     5104 2023-04-18 14:37:59.000000 ji-coursesel-0.1.4/courseselcli/single.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-04-18 14:38:59.923922 ji-coursesel-0.1.4/ji_coursesel.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      760 2023-04-18 14:38:59.000000 ji-coursesel-0.1.4/ji_coursesel.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      428 2023-04-18 14:38:59.000000 ji-coursesel-0.1.4/ji_coursesel.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-04-18 14:38:59.000000 ji-coursesel-0.1.4/ji_coursesel.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       64 2023-04-18 14:38:59.000000 ji-coursesel-0.1.4/ji_coursesel.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       36 2023-04-18 14:38:59.000000 ji-coursesel-0.1.4/ji_coursesel.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-04-18 14:38:59.000000 ji-coursesel-0.1.4/ji_coursesel.egg-info/top_level.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      433 2023-04-18 14:38:59.927255 ji-coursesel-0.1.4/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      164 2022-12-30 03:18:49.000000 ji-coursesel-0.1.4/setup.py
```

### Comparing `ji-coursesel-0.1.3/PKG-INFO` & `ji-coursesel-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ji-coursesel
-Version: 0.1.3
+Version: 0.1.4
 Summary: CLI Interface for JI Coursesel
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli,course
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ji-coursesel-0.1.3/courseselcli/elector.py` & `ji-coursesel-0.1.4/courseselcli/elector.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,17 @@
             'JSESSIONID': jsessionid
         }
 
         self.headers = {
             'Connection': 'keep-alive',
             'sec-ch-ua': '^\\^Chromium^\\^;v=^\\^92^\\^, ^\\^',
             'Accept': 'application/json, text/javascript, */*; q=0.01',
-            'X-CSRF-TOKEN': 'ab3849d5-4aa0-471c-86eb-adfc0916af73',
             'X-Requested-With': 'XMLHttpRequest',
             'sec-ch-ua-mobile': '?0',
-            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.159 Safari/537.36',
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36',
             'Content-Type': 'application/x-www-form-urlencoded',
             'Origin': 'https://coursesel.umji.sjtu.edu.cn',
             'Sec-Fetch-Site': 'same-origin',
             'Sec-Fetch-Mode': 'cors',
             'Sec-Fetch-Dest': 'empty',
             'Referer': 'https://coursesel.umji.sjtu.edu.cn/welcome.action',
             'Accept-Language': 'zh-CN,zh;q=0.9',
```

### Comparing `ji-coursesel-0.1.3/courseselcli/login.py` & `ji-coursesel-0.1.4/courseselcli/login.py`

 * *Files identical despite different names*

### Comparing `ji-coursesel-0.1.3/courseselcli/main.py` & `ji-coursesel-0.1.4/courseselcli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 @app.command()
 def elect(jsessionID: str = typer.Option(None, "--jsessionID", "-j", help="Your JSESSIONID"),
           electTurnID: str = typer.Option(None, "--electTurnID", "-e"),
           ElectTurnLessonTaskID: str = typer.Option(None, "--electTurnLessonTaskID", "-l",
                                                     help="List of all courses you want to select, separated by comma (,)."),
           CoursesDesc: str = typer.Option(None, "--coursesDesc",
                                           help="List of all course description you want to select, separated by comma (,)."),
-          thread_number: int = typer.Option(3, "--thread", "-x",
+          thread_number: int = typer.Option(1, "--thread", "-x",
                                             help="Number of threads to use for each course."),
           max_try: int = typer.Option(None, "--max-try", "-m",
                                       help="Maximum number of requests to send for all course. If not set, will try forever."),
           demo: bool = typer.Option(
               False, "--demo", help="Do a demonstration.")
           ):
     """
```

### Comparing `ji-coursesel-0.1.3/courseselcli/single.py` & `ji-coursesel-0.1.4/courseselcli/single.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import requests
 import time
 import threading
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
 
 class ElectSingle:
-    def __init__(self, JSESSIONID, TURNID, COURSEID: list, thread_number=3, max_try=None, course_desc: list = None) -> None:
+    def __init__(self, JSESSIONID, TURNID, COURSEID: list, thread_number=1, max_try=None, course_desc: list = None) -> None:
         '''
         COURSEID: list of the ElectTurnLessonTaskID of courses
         thread_number: thred number for each course
         max_try: max try times
         course_desc: list of course description
         '''
         self.ELECTTURNID = TURNID
@@ -67,15 +67,16 @@
                 ('_t', realtime),
             )
             response = requests.post('https://coursesel.umji.sjtu.edu.cn/tpm/doElect_ElectTurn.action',
                                      headers=self.headers, params=params, cookies=self.cookies, data=data)
             ret = response.content.decode(encoding='utf-8', errors='ignore')
             if(len(ret) > 1000):
                 # print("error")
-                self.progress.log("Got error response. It's very likely that you are using expired JSESSIONID.")
+                self.progress.log(
+                    "Got error response. It's very likely that you are using expired JSESSIONID.")
                 self.progress.update(
                     self.tasks[taskid], advance=1, description="[white]" + self.course_desc[taskid] + ": [red]Failed")
                 return
             if(str(ret).find("false") == -1):
                 # print("success, congrats")
                 self.progress.update(
                     self.tasks[taskid], advance=1, description="[white]" + self.course_desc[taskid] + ": [green]Success")
```

### Comparing `ji-coursesel-0.1.3/ji_coursesel.egg-info/PKG-INFO` & `ji-coursesel-0.1.4/ji_coursesel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ji-coursesel
-Version: 0.1.3
+Version: 0.1.4
 Summary: CLI Interface for JI Coursesel
 Author: linsyking
 Author-email: linsy_king@sjtu.edu.cn
 License: MIT License
 Keywords: cli,course
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

