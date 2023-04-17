# Comparing `tmp/sqlalchemy_sqlite_session-1.8.420.tar.gz` & `tmp/sqlalchemy_sqlite_session-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_sqlite_session-1.8.420.tar", last modified: Wed Apr 20 14:58:22 2022, max compression
+gzip compressed data, was "sqlalchemy_sqlite_session-1.9.0.tar", last modified: Mon Apr 17 23:13:14 2023, max compression
```

## Comparing `sqlalchemy_sqlite_session-1.8.420.tar` & `sqlalchemy_sqlite_session-1.9.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-04-20 14:58:22.371135 sqlalchemy_sqlite_session-1.8.420/
--rw-rw-rw-   0        0        0     1091 2021-09-18 02:20:09.000000 sqlalchemy_sqlite_session-1.8.420/LICENSE
--rw-rw-rw-   0        0        0     1296 2022-04-20 14:58:22.369137 sqlalchemy_sqlite_session-1.8.420/PKG-INFO
--rw-rw-rw-   0        0        0      685 2022-03-11 06:19:16.000000 sqlalchemy_sqlite_session-1.8.420/README.md
--rw-rw-rw-   0        0        0      108 2021-09-18 02:20:09.000000 sqlalchemy_sqlite_session-1.8.420/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-04-20 14:58:22.372134 sqlalchemy_sqlite_session-1.8.420/setup.cfg
--rw-rw-rw-   0        0        0      879 2022-04-20 14:57:36.000000 sqlalchemy_sqlite_session-1.8.420/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-20 14:58:22.241214 sqlalchemy_sqlite_session-1.8.420/src/
-drwxrwxrwx   0        0        0        0 2022-04-20 14:58:22.329161 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/
--rw-rw-rw-   0        0        0        0 2021-09-18 02:20:09.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/__init__.py
--rw-rw-rw-   0        0        0      949 2022-04-13 06:08:09.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/adapters.py
--rw-rw-rw-   0        0        0     5179 2022-04-13 06:08:09.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/bin2.py
--rw-rw-rw-   0        0        0     4611 2022-04-13 06:08:09.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/cjcp.py
--rw-rw-rw-   0        0        0    28039 2022-04-18 03:23:41.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/kl8.py
--rw-rw-rw-   0        0        0     2253 2022-04-13 06:08:09.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/qlc.py
--rw-rw-rw-   0        0        0     2181 2022-04-13 06:08:09.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/qxc.py
--rw-rw-rw-   0        0        0    51506 2022-04-13 06:08:09.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/sport.py
--rw-rw-rw-   0        0        0     8647 2022-04-13 06:08:09.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/ssq.py
--rw-rw-rw-   0        0        0       85 2022-04-13 06:08:09.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/test.py
--rw-rw-rw-   0        0        0      463 2022-04-13 06:08:09.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/tools.py
--rw-rw-rw-   0        0        0    54657 2022-04-16 16:02:49.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/welfare.py
-drwxrwxrwx   0        0        0        0 2022-04-20 14:58:22.357144 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session.egg-info/
--rw-rw-rw-   0        0        0     1296 2022-04-20 14:58:20.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      731 2022-04-20 14:58:22.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-20 14:58:21.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2022-04-20 14:58:22.000000 sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-20 14:58:22.363141 sqlalchemy_sqlite_session-1.8.420/test/
--rw-rw-rw-   0        0        0      103 2021-09-18 02:20:09.000000 sqlalchemy_sqlite_session-1.8.420/test/test.py
+drwxrwxrwx   0        0        0        0 2023-04-17 23:13:14.117781 sqlalchemy_sqlite_session-1.9.0/
+-rw-rw-rw-   0        0        0     1091 2023-04-17 23:10:49.000000 sqlalchemy_sqlite_session-1.9.0/LICENSE
+-rw-rw-rw-   0        0        0     1255 2023-04-17 23:13:14.116782 sqlalchemy_sqlite_session-1.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-04-17 23:10:49.000000 sqlalchemy_sqlite_session-1.9.0/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-17 23:10:49.000000 sqlalchemy_sqlite_session-1.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-17 23:13:14.117781 sqlalchemy_sqlite_session-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      877 2023-04-17 23:12:05.000000 sqlalchemy_sqlite_session-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 23:13:14.026840 sqlalchemy_sqlite_session-1.9.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-17 23:13:14.091800 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/
+-rw-rw-rw-   0        0        0        0 2023-04-17 23:10:49.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/__init__.py
+-rw-rw-rw-   0        0        0     1290 2023-04-17 21:57:23.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/abcs.py
+-rw-rw-rw-   0        0        0      949 2023-04-17 13:48:15.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/adapters.py
+-rw-rw-rw-   0        0        0     5179 2023-04-17 13:48:15.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/bin2.py
+-rw-rw-rw-   0        0        0     4611 2023-04-17 13:48:15.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/cjcp.py
+-rw-rw-rw-   0        0        0    28039 2023-04-17 13:48:15.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/kl8.py
+-rw-rw-rw-   0        0        0     2253 2023-04-17 13:48:15.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/qlc.py
+-rw-rw-rw-   0        0        0     2181 2023-04-17 13:48:15.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/qxc.py
+-rw-rw-rw-   0        0        0    52096 2023-04-17 14:05:19.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/sport.py
+-rw-rw-rw-   0        0        0     8647 2023-04-17 13:48:15.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/ssq.py
+-rw-rw-rw-   0        0        0       85 2023-04-17 13:48:15.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/test.py
+-rw-rw-rw-   0        0        0      463 2023-04-17 13:48:15.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/tools.py
+-rw-rw-rw-   0        0        0    54657 2023-04-17 13:48:15.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/welfare.py
+drwxrwxrwx   0        0        0        0 2023-04-17 23:13:14.108790 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session.egg-info/
+-rw-rw-rw-   0        0        0     1255 2023-04-17 23:13:13.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      769 2023-04-17 23:13:14.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 23:13:13.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-17 23:13:13.000000 sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-17 23:13:14.112786 sqlalchemy_sqlite_session-1.9.0/test/
+-rw-rw-rw-   0        0        0      103 2023-04-17 23:10:49.000000 sqlalchemy_sqlite_session-1.9.0/test/test.py
```

### Comparing `sqlalchemy_sqlite_session-1.8.420/LICENSE` & `sqlalchemy_sqlite_session-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_sqlite_session-1.8.420/PKG-INFO` & `sqlalchemy_sqlite_session-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_sqlite_session
-Version: 1.8.420
+Version: 1.9.0
 Summary: get sqlite session or engine for sqlalchemy
 Home-page: https://gitee.com/tensorflows/sqlalchemy-sqlite-session
 Author: WangJulong
 Author-email: 496349619@qq.com
-License: UNKNOWN
 Project-URL: project url, https://gitee.com/tensorflows/sqlalchemy-sqlite-session
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -49,8 +47,7 @@
 ```
 
 ### Uploading Project to PyPI
 ```
 twine check dist/*
 twine upload dist/*
 ```
-
```

### Comparing `sqlalchemy_sqlite_session-1.8.420/README.md` & `sqlalchemy_sqlite_session-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_sqlite_session-1.8.420/setup.py` & `sqlalchemy_sqlite_session-1.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sqlalchemy_sqlite_session",
-    version="1.8.420",
+    version="1.9.0",
     author="WangJulong",
     author_email="496349619@qq.com",
     description="get sqlite session or engine for sqlalchemy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/tensorflows/sqlalchemy-sqlite-session",
     project_urls={
```

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/adapters.py` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/adapters.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/bin2.py` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/bin2.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/cjcp.py` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/cjcp.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/kl8.py` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/kl8.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/qlc.py` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/qlc.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/qxc.py` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/qxc.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/sport.py` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/sport.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,25 @@
     num2 = Column(Integer, nullable=False)
     num3 = Column(Integer, nullable=False)
 
     def __init__(self, data_list: list):
         self.issue, self.num1, self.num2, self.num3 = data_list
 
     @classmethod
+    def get_issue_future(cls):
+        """get issue"""
+        session = get_session_sport()
+        i = session.query(cls).all()
+        session.close()
+        last = [x.issue for x in i]
+        last.sort()
+        result = last[-1] + 1
+        return result
+    
+    @classmethod
     def get_num1(cls, issue_number: int):
         """获取对应 issue 的号码 num1"""
         session = get_session_sport()
         data = session.query(cls).get(issue_number)
         session.close()
         return data.num1
 
@@ -811,14 +822,25 @@
     num4 = Column(Integer, nullable=False)
     num5 = Column(Integer, nullable=False)
 
     def __init__(self, data_list: list):
         self.issue, self.num1, self.num2, self.num3, self.num4, self.num5 = data_list
 
     @classmethod
+    def get_issue_future(cls):
+        """get issue"""
+        session = get_session_sport()
+        i = session.query(cls).all()
+        session.close()
+        last = [x.issue for x in i]
+        last.sort()
+        result = last[-1] + 1
+        return result
+    
+    @classmethod
     def get_issues(cls):
         """get issues[list]"""
         session = get_session_sport()
         i = session.query(cls).all()
         result = [x.issue for x in i]
         result.sort()
         session.close()
```

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/ssq.py` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/ssq.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session/welfare.py` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session/welfare.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session.egg-info/PKG-INFO` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-sqlite-session
-Version: 1.8.420
+Version: 1.9.0
 Summary: get sqlite session or engine for sqlalchemy
 Home-page: https://gitee.com/tensorflows/sqlalchemy-sqlite-session
 Author: WangJulong
 Author-email: 496349619@qq.com
-License: UNKNOWN
 Project-URL: project url, https://gitee.com/tensorflows/sqlalchemy-sqlite-session
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -49,8 +47,7 @@
 ```
 
 ### Uploading Project to PyPI
 ```
 twine check dist/*
 twine upload dist/*
 ```
-
```

### Comparing `sqlalchemy_sqlite_session-1.8.420/src/sqlalchemy_sqlite_session.egg-info/SOURCES.txt` & `sqlalchemy_sqlite_session-1.9.0/src/sqlalchemy_sqlite_session.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/sqlalchemy_sqlite_session/__init__.py
+src/sqlalchemy_sqlite_session/abcs.py
 src/sqlalchemy_sqlite_session/adapters.py
 src/sqlalchemy_sqlite_session/bin2.py
 src/sqlalchemy_sqlite_session/cjcp.py
 src/sqlalchemy_sqlite_session/kl8.py
 src/sqlalchemy_sqlite_session/qlc.py
 src/sqlalchemy_sqlite_session/qxc.py
 src/sqlalchemy_sqlite_session/sport.py
```

