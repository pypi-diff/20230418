# Comparing `tmp/coolmysql-1.4.tar.gz` & `tmp/coolmysql-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolmysql-1.4.tar", last modified: Wed Apr 12 15:22:07 2023, max compression
+gzip compressed data, was "coolmysql-1.4.2.tar", last modified: Tue Apr 18 11:13:09 2023, max compression
```

## Comparing `coolmysql-1.4.tar` & `coolmysql-1.4.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4/LICENSE
--rw-r--r--   0        0        0     4351 2023-04-09 11:16:42.051321 coolmysql-1.4/README.md
--rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4/coolmysql.py
--rw-r--r--   0        0        0      562 2023-04-12 15:16:36.716121 coolmysql-1.4/pyproject.toml
--rw-r--r--   0        0        0     4603 1970-01-01 00:00:00.000000 coolmysql-1.4/PKG-INFO
+-rw-r--r--   0        0        0    10953 2023-02-13 16:22:52.569575 coolmysql-1.4.2/LICENSE
+-rw-r--r--   0        0        0     4343 2023-04-16 20:01:06.306928 coolmysql-1.4.2/README.md
+-rw-r--r--   0        0        0       29 2023-04-10 03:59:45.387315 coolmysql-1.4.2/coolmysql.py
+-rw-r--r--   0        0        0      566 2023-04-18 11:13:01.590911 coolmysql-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 coolmysql-1.4.2/PKG-INFO
```

### Comparing `coolmysql-1.4/LICENSE` & `coolmysql-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coolmysql-1.4/README.md` & `coolmysql-1.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     return connect(
         host = 'localhost',
         port = 3306,
         user = 'root',
         password = '123456789'
     )
 
-orm = ORM(mkconn=mkconn)  # 账户ORM
+orm = ORM(mkconn)  # 账户ORM
 db = orm['泉州市']  # 库ORM
 sheet = db['希望小学']  # 表ORM
 ```
 
 新增数据：
 
 ```python
@@ -110,25 +110,25 @@
 | **代码**               | **解释**                   |
 | ---------------------------- | -------------------------------- |
 | mc.年级.isin('初三', '高二') | 若字段值是传入值的成员，则符合   |
 | mc.年龄.notin(10, 30, 45)    | 若字段值不是传入值的成员，则符合 |
 
 过滤器的集合运算：
 
-| **代码**                                                        | **解释** |
-| --------------------------------------------------------------------- | -------------- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                          | 交集           |
-| [ (mc.年龄==30) \| (mc.年龄>30) \| (mc.年龄<30) \| (mc.年龄==None) ] | 并集           |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                       | 差集           |
-| [ ~(mc.年龄>100) ]                                                    | 补集           |
+| **代码**                                                         | **解释** |
+| ---------------------------------------------------------------------- | -------------- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集           |
+| [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集           |
+| [ ~(mc.年龄>100) ]                                                     | 补集           |
 
 只返回姓名、年龄这2个字段：
 
 ```python
-sheet[mc.年龄>11][mc.年龄<30]['姓名','年龄'][:]
+sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
 执行原生SQL语句：
 
 ```python
 data, cursor = sheet.execute('select 姓名 from 希望小学 limit 1')
 data
```

### Comparing `coolmysql-1.4/pyproject.toml` & `coolmysql-1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "coolmysql"
-version = "1.4"
+version = "1.4.2"
 description = "史上最优雅的 mysql ORM"
-dependencies = ["lccpy >=1.4"]
+dependencies = ["lccpy >=1.4.4"]
 keywords = ["coolmysql", "pymysql", "mysql"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 requires-python = ">=3.7"
```

### Comparing `coolmysql-1.4/PKG-INFO` & `coolmysql-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: coolmysql
-Version: 1.4
+Version: 1.4.2
 Summary: 史上最优雅的 mysql ORM
 Keywords: coolmysql,pymysql,mysql
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: lccpy >=1.4
+Requires-Dist: lccpy >=1.4.4
 Project-URL: HomePage, https://github.com/lcctoor/lccpy/tree/main/coolmysql
 
 # 项目描述
 
 史上最优雅的 mysql ORM 。
 
 # 安装与教程
@@ -52,15 +52,15 @@
     return connect(
         host = 'localhost',
         port = 3306,
         user = 'root',
         password = '123456789'
     )
 
-orm = ORM(mkconn=mkconn)  # 账户ORM
+orm = ORM(mkconn)  # 账户ORM
 db = orm['泉州市']  # 库ORM
 sheet = db['希望小学']  # 表ORM
 ```
 
 新增数据：
 
 ```python
@@ -122,25 +122,25 @@
 | **代码**               | **解释**                   |
 | ---------------------------- | -------------------------------- |
 | mc.年级.isin('初三', '高二') | 若字段值是传入值的成员，则符合   |
 | mc.年龄.notin(10, 30, 45)    | 若字段值不是传入值的成员，则符合 |
 
 过滤器的集合运算：
 
-| **代码**                                                        | **解释** |
-| --------------------------------------------------------------------- | -------------- |
-| [ mc.年龄>3 ][ mc.年龄<100 ]                                          | 交集           |
-| [ (mc.年龄==30) \| (mc.年龄>30) \| (mc.年龄<30) \| (mc.年龄==None) ] | 并集           |
-| [ (mc.年龄>3) - (mc.年龄>100) ]                                       | 差集           |
-| [ ~(mc.年龄>100) ]                                                    | 补集           |
+| **代码**                                                         | **解释** |
+| ---------------------------------------------------------------------- | -------------- |
+| [ mc.年龄>3 ][ mc.年龄<100 ]                                           | 交集           |
+| [ (mc.年龄<30) \| (mc.年龄>30) \| (mc.年龄==30) \| (mc.年龄==None) ] | 并集           |
+| [ (mc.年龄>3) - (mc.年龄>100) ]                                        | 差集           |
+| [ ~(mc.年龄>100) ]                                                     | 补集           |
 
 只返回姓名、年龄这2个字段：
 
 ```python
-sheet[mc.年龄>11][mc.年龄<30]['姓名','年龄'][:]
+sheet[mc.年级=='高一']['姓名','年龄'][:]
 ```
 
 执行原生SQL语句：
 
 ```python
 data, cursor = sheet.execute('select 姓名 from 希望小学 limit 1')
 data
```

