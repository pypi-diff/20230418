# Comparing `tmp/lccpy-1.4.3.tar.gz` & `tmp/lccpy-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lccpy-1.4.3.tar", last modified: Wed Apr 12 18:15:45 2023, max compression
+gzip compressed data, was "lccpy-1.4.4.tar", last modified: Tue Apr 18 11:10:38 2023, max compression
```

## Comparing `lccpy-1.4.3.tar` & `lccpy-1.4.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4.3/LICENSE
--rw-r--r--   0        0        0      119 2023-04-10 04:12:12.772589 lccpy-1.4.3/README.md
--rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4.3/lccpy/__init__.py
--rw-r--r--   0        0        0      143 2023-04-11 02:41:01.880058 lccpy-1.4.3/lccpy/_mtype.py
--rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4.3/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
--rw-r--r--   0        0        0      168 2023-04-10 03:51:03.558895 lccpy-1.4.3/lccpy/asymongo/__init__.py
--rw-r--r--   0        0        0    20512 2023-04-11 02:42:19.557384 lccpy-1.4.3/lccpy/asymongo/_asymongo.py
--rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4.3/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
--rw-r--r--   0        0        0       89 2023-04-10 03:50:24.852505 lccpy-1.4.3/lccpy/asymysql/__init__.py
--rw-r--r--   0        0        0    20191 2023-04-12 16:47:55.128042 lccpy-1.4.3/lccpy/asymysql/_asymysql.py
--rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4.3/lccpy/coolfunc/__init__.py
--rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4.3/lccpy/coolfunc/_coolfunc.py
--rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4.3/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
--rw-r--r--   0        0        0      169 2023-04-10 03:53:42.961556 lccpy-1.4.3/lccpy/coolmongo/__init__.py
--rw-r--r--   0        0        0    20930 2023-04-11 02:42:37.661736 lccpy-1.4.3/lccpy/coolmongo/_coolmongo.py
--rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4.3/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
--rw-r--r--   0        0        0       90 2023-04-10 03:53:46.616102 lccpy-1.4.3/lccpy/coolmysql/__init__.py
--rw-r--r--   0        0        0    21592 2023-04-12 18:14:45.697852 lccpy-1.4.3/lccpy/coolmysql/_coolmysql.py
--rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4.3/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
--rw-r--r--   0        0        0       35 2022-11-15 14:17:28.000000 lccpy-1.4.3/lccpy/encrypt256/__init__.py
--rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4.3/lccpy/encrypt256/_encrypt256.py
--rw-r--r--   0        0        0       35 2023-04-07 08:40:27.218236 lccpy-1.4.3/lccpy/increment/__init__.py
--rw-r--r--   0        0        0     1544 2023-04-12 06:50:22.634385 lccpy-1.4.3/lccpy/increment/_increment.py
--rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4.3/lccpy/rstyleslice/__init__.py
--rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4.3/lccpy/rstyleslice/_rstyleslice.py
--rw-r--r--   0        0        0      175 2023-04-09 15:53:54.291702 lccpy-1.4.3/lccpy/vtype/__init__.py
--rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.4.3/lccpy/vtype/_cooltime.py
--rw-r--r--   0        0        0    11771 2023-04-12 12:56:02.300717 lccpy-1.4.3/lccpy/vtype/_vtype.py
--rw-r--r--   0        0        0      573 2023-04-12 18:14:18.978381 lccpy-1.4.3/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 lccpy-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0    10951 2023-02-13 16:30:40.665398 lccpy-1.4.4/LICENSE
+-rw-r--r--   0        0        0      119 2023-04-10 04:12:12.772589 lccpy-1.4.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 03:05:49.119798 lccpy-1.4.4/lccpy/__init__.py
+-rw-r--r--   0        0        0      143 2023-04-11 02:41:01.880058 lccpy-1.4.4/lccpy/_mtype.py
+-rw-r--r--   0        0        0    11357 2022-10-25 20:46:40.000000 lccpy-1.4.4/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE
+-rw-r--r--   0        0        0      168 2023-04-10 03:51:03.558895 lccpy-1.4.4/lccpy/asymongo/__init__.py
+-rw-r--r--   0        0        0    20512 2023-04-11 02:42:19.557384 lccpy-1.4.4/lccpy/asymongo/_asymongo.py
+-rw-r--r--   0        0        0     1070 2022-05-08 19:03:55.000000 lccpy-1.4.4/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE
+-rw-r--r--   0        0        0       89 2023-04-10 03:50:24.852505 lccpy-1.4.4/lccpy/asymysql/__init__.py
+-rw-r--r--   0        0        0    20277 2023-04-18 11:07:49.320573 lccpy-1.4.4/lccpy/asymysql/_asymysql.py
+-rw-r--r--   0        0        0      273 2023-04-09 17:36:47.380717 lccpy-1.4.4/lccpy/coolfunc/__init__.py
+-rw-r--r--   0        0        0     2787 2023-04-10 03:18:54.132549 lccpy-1.4.4/lccpy/coolfunc/_coolfunc.py
+-rw-r--r--   0        0        0    11357 2022-11-17 21:35:25.000000 lccpy-1.4.4/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE
+-rw-r--r--   0        0        0      169 2023-04-10 03:53:42.961556 lccpy-1.4.4/lccpy/coolmongo/__init__.py
+-rw-r--r--   0        0        0    20930 2023-04-11 02:42:37.661736 lccpy-1.4.4/lccpy/coolmongo/_coolmongo.py
+-rw-r--r--   0        0        0     1070 2013-11-27 14:43:24.000000 lccpy-1.4.4/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE
+-rw-r--r--   0        0        0       90 2023-04-10 03:53:46.616102 lccpy-1.4.4/lccpy/coolmysql/__init__.py
+-rw-r--r--   0        0        0    21686 2023-04-18 11:07:58.985529 lccpy-1.4.4/lccpy/coolmysql/_coolmysql.py
+-rw-r--r--   0        0        0     2926 2023-01-27 23:35:02.000000 lccpy-1.4.4/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE
+-rw-r--r--   0        0        0       35 2022-11-15 14:17:28.000000 lccpy-1.4.4/lccpy/encrypt256/__init__.py
+-rw-r--r--   0        0        0     5141 2023-03-09 14:58:17.055833 lccpy-1.4.4/lccpy/encrypt256/_encrypt256.py
+-rw-r--r--   0        0        0       35 2023-04-07 08:40:27.218236 lccpy-1.4.4/lccpy/increment/__init__.py
+-rw-r--r--   0        0        0     1544 2023-04-12 06:50:22.634385 lccpy-1.4.4/lccpy/increment/_increment.py
+-rw-r--r--   0        0        0       32 2023-02-19 09:41:05.530766 lccpy-1.4.4/lccpy/rstyleslice/__init__.py
+-rw-r--r--   0        0        0     2903 2023-03-09 15:08:02.859531 lccpy-1.4.4/lccpy/rstyleslice/_rstyleslice.py
+-rw-r--r--   0        0        0      175 2023-04-09 15:53:54.291702 lccpy-1.4.4/lccpy/vtype/__init__.py
+-rw-r--r--   0        0        0     3546 2023-04-09 15:28:10.501541 lccpy-1.4.4/lccpy/vtype/_cooltime.py
+-rw-r--r--   0        0        0    11771 2023-04-12 12:56:02.300717 lccpy-1.4.4/lccpy/vtype/_vtype.py
+-rw-r--r--   0        0        0      573 2023-04-18 11:09:10.992464 lccpy-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 lccpy-1.4.4/PKG-INFO
```

### Comparing `lccpy-1.4.3/LICENSE` & `lccpy-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE` & `lccpy-1.4.4/lccpy/asymongo/Licenses of dependent packages/motor/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/asymongo/_asymongo.py` & `lccpy-1.4.4/lccpy/asymongo/_asymongo.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE` & `lccpy-1.4.4/lccpy/asymysql/Licenses of dependent packages/aiomysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/asymysql/_asymysql.py` & `lccpy-1.4.4/lccpy/asymysql/_asymysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,18 @@
             await conn.rollback()
             raise
     
     async def getPK(self):
         if not self._pk:
             sql = f"select column_name from information_schema.columns where table_schema = '{self.dbName}' and table_name = '{self.sheetName}' and column_key='PRI' "
             rdata, cursor = await self.execute(sql, commit=False)
-            object.__setattr__(self, '_pk', rdata[0]['COLUMN_NAME'])
+            data = rdata[0]
+            assert len(data) == 1
+            _pk = list(data.values())[0]
+            object.__setattr__(self, '_pk', _pk)
         return self._pk
     
     async def getColumns(self, comment=True, type=True):
         need = ['column_name as name']
         if comment: need.append('column_comment as comment')
         if type: need.append('column_type as type')
         need = ', '.join(need)
```

### Comparing `lccpy-1.4.3/lccpy/coolfunc/_coolfunc.py` & `lccpy-1.4.4/lccpy/coolfunc/_coolfunc.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE` & `lccpy-1.4.4/lccpy/coolmongo/Licenses of dependent packages/pymongo/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/coolmongo/_coolmongo.py` & `lccpy-1.4.4/lccpy/coolmongo/_coolmongo.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE` & `lccpy-1.4.4/lccpy/coolmysql/Licenses of dependent packages/pymysql/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/coolmysql/_coolmysql.py` & `lccpy-1.4.4/lccpy/coolmysql/_coolmysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
                 for k, v in kvs.items():
                     s.append(f"        when {pk} = {jsonChinese(k)} then {jsonChinese(v)}")
                 s.append(f"else {field}")
                 s.append('end')
                 blocks.append('\n'.join(s))
             blocks = ' ,\n'.join(blocks)
             sql = f"update {self.sheetName} set \n{blocks}"
-            r, cursor = self.execute(sql=sql)
+            self.execute(sql=sql)
             return dict(data=lines)
         else:
             return dict(data=lines)
 
     def order(self, **rule): return self._copy(_sort={**rule})
 
     def __add__(self, data):
@@ -452,14 +452,17 @@
             conn.rollback()
             raise
     
     def getPK(self):
         if not self._pk:
             sql = f"select column_name from information_schema.columns where table_schema = '{self.dbName}' and table_name = '{self.sheetName}' and column_key='PRI' "
             rdata, cursor = self.execute(sql, commit=False)
+            data = rdata[0]
+            assert len(data) == 1
+            _pk = list(data.values())[0]
             object.__setattr__(self, '_pk', rdata[0]['COLUMN_NAME'])
         return self._pk
     
     def getColumns(self, comment=True, type=True):
         need = ['column_name as name']
         if comment: need.append('column_comment as comment')
         if type: need.append('column_type as type')
```

### Comparing `lccpy-1.4.3/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE` & `lccpy-1.4.4/lccpy/encrypt256/Licenses of dependent packages/pycryptodome/LICENSE`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/encrypt256/_encrypt256.py` & `lccpy-1.4.4/lccpy/encrypt256/_encrypt256.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/increment/_increment.py` & `lccpy-1.4.4/lccpy/increment/_increment.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/rstyleslice/_rstyleslice.py` & `lccpy-1.4.4/lccpy/rstyleslice/_rstyleslice.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/vtype/_cooltime.py` & `lccpy-1.4.4/lccpy/vtype/_cooltime.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/lccpy/vtype/_vtype.py` & `lccpy-1.4.4/lccpy/vtype/_vtype.py`

 * *Files identical despite different names*

### Comparing `lccpy-1.4.3/pyproject.toml` & `lccpy-1.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "lccpy"
-version = "1.4.3"
+version = "1.4.4"
 description = "The dependent package of project <Make Python simpler> ."
 dependencies = ["motor", "aiomysql", "pymongo", "pymysql", "pycryptodome"]
 
 readme = "README.md"
 authors = [{name = "许灿标", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `lccpy-1.4.3/PKG-INFO` & `lccpy-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lccpy
-Version: 1.4.3
+Version: 1.4.4
 Summary: The dependent package of project <Make Python simpler> .
 Author-email: 许灿标 <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: motor
 Requires-Dist: aiomysql
```

