# Comparing `tmp/mysql-cli-1.0.0.tar.gz` & `tmp/mysql-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-cli-1.0.0.tar", last modified: Sun Dec 11 15:48:02 2022, max compression
+gzip compressed data, was "mysql-cli-1.1.0.tar", last modified: Tue Apr 18 08:25:29 2023, max compression
```

## Comparing `mysql-cli-1.0.0.tar` & `mysql-cli-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 william    (501) staff       (20)        0 2022-12-11 15:48:02.427571 mysql-cli-1.0.0/
--rw-r--r--   0 william    (501) staff       (20)     1070 2022-12-04 06:15:33.000000 mysql-cli-1.0.0/LICENSE
--rw-r--r--   0 william    (501) staff       (20)     6985 2022-12-11 15:48:02.427074 mysql-cli-1.0.0/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)     6453 2022-12-11 15:46:55.000000 mysql-cli-1.0.0/README.md
-drwxr-xr-x   0 william    (501) staff       (20)        0 2022-12-11 15:48:02.422925 mysql-cli-1.0.0/mysql_cli/
--rw-r--r--   0 william    (501) staff       (20)      235 2022-12-11 11:07:30.000000 mysql-cli-1.0.0/mysql_cli/__init__.py
--rw-r--r--   0 william    (501) staff       (20)     1190 2022-12-08 12:57:07.000000 mysql-cli-1.0.0/mysql_cli/client.py
--rw-r--r--   0 william    (501) staff       (20)     6701 2022-12-11 12:13:17.000000 mysql-cli-1.0.0/mysql_cli/query.py
--rw-r--r--   0 william    (501) staff       (20)      397 2022-12-10 02:55:17.000000 mysql-cli-1.0.0/mysql_cli/utils.py
-drwxr-xr-x   0 william    (501) staff       (20)        0 2022-12-11 15:48:02.426323 mysql-cli-1.0.0/mysql_cli.egg-info/
--rw-r--r--   0 william    (501) staff       (20)     6985 2022-12-11 15:48:02.000000 mysql-cli-1.0.0/mysql_cli.egg-info/PKG-INFO
--rw-r--r--   0 william    (501) staff       (20)      285 2022-12-11 15:48:02.000000 mysql-cli-1.0.0/mysql_cli.egg-info/SOURCES.txt
--rw-r--r--   0 william    (501) staff       (20)        1 2022-12-11 15:48:02.000000 mysql-cli-1.0.0/mysql_cli.egg-info/dependency_links.txt
--rw-r--r--   0 william    (501) staff       (20)       45 2022-12-11 15:48:02.000000 mysql-cli-1.0.0/mysql_cli.egg-info/requires.txt
--rw-r--r--   0 william    (501) staff       (20)       10 2022-12-11 15:48:02.000000 mysql-cli-1.0.0/mysql_cli.egg-info/top_level.txt
--rw-r--r--   0 william    (501) staff       (20)      780 2022-12-11 15:45:52.000000 mysql-cli-1.0.0/pyproject.toml
--rw-r--r--   0 william    (501) staff       (20)       38 2022-12-11 15:48:02.427733 mysql-cli-1.0.0/setup.cfg
--rw-r--r--   0 william    (501) staff       (20)      184 2022-12-11 15:43:06.000000 mysql-cli-1.0.0/setup.py
+drwxr-xr-x   0 will4j    (1000) will4j    (1000)        0 2023-04-18 08:25:29.807120 mysql-cli-1.1.0/
+-rw-r--r--   0 will4j    (1000) will4j    (1000)     1090 2022-12-22 06:38:46.000000 mysql-cli-1.1.0/LICENSE
+-rw-r--r--   0 will4j    (1000) will4j    (1000)     9220 2023-04-18 08:25:29.807120 mysql-cli-1.1.0/PKG-INFO
+-rw-r--r--   0 will4j    (1000) will4j    (1000)     8961 2023-04-18 08:16:54.000000 mysql-cli-1.1.0/README.md
+drwxr-xr-x   0 will4j    (1000) will4j    (1000)        0 2023-04-18 08:25:29.807120 mysql-cli-1.1.0/mysql_cli/
+-rw-r--r--   0 will4j    (1000) will4j    (1000)      250 2023-04-17 04:33:33.000000 mysql-cli-1.1.0/mysql_cli/__init__.py
+-rw-r--r--   0 will4j    (1000) will4j    (1000)     1229 2022-12-23 02:00:00.000000 mysql-cli-1.1.0/mysql_cli/client.py
+-rw-r--r--   0 will4j    (1000) will4j    (1000)    11908 2023-04-18 08:16:54.000000 mysql-cli-1.1.0/mysql_cli/query.py
+-rw-r--r--   0 will4j    (1000) will4j    (1000)      412 2022-12-23 02:00:00.000000 mysql-cli-1.1.0/mysql_cli/utils.py
+drwxr-xr-x   0 will4j    (1000) will4j    (1000)        0 2023-04-18 08:25:29.807120 mysql-cli-1.1.0/mysql_cli.egg-info/
+-rw-r--r--   0 will4j    (1000) will4j    (1000)     9220 2023-04-18 08:25:29.000000 mysql-cli-1.1.0/mysql_cli.egg-info/PKG-INFO
+-rw-r--r--   0 will4j    (1000) will4j    (1000)      326 2023-04-18 08:25:29.000000 mysql-cli-1.1.0/mysql_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 will4j    (1000) will4j    (1000)        1 2023-04-18 08:25:29.000000 mysql-cli-1.1.0/mysql_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 will4j    (1000) will4j    (1000)       45 2023-04-18 08:25:29.000000 mysql-cli-1.1.0/mysql_cli.egg-info/requires.txt
+-rw-r--r--   0 will4j    (1000) will4j    (1000)       10 2023-04-18 08:25:29.000000 mysql-cli-1.1.0/mysql_cli.egg-info/top_level.txt
+-rw-r--r--   0 will4j    (1000) will4j    (1000)      810 2023-04-18 08:22:55.000000 mysql-cli-1.1.0/pyproject.toml
+-rw-r--r--   0 will4j    (1000) will4j    (1000)       38 2023-04-18 08:25:29.807120 mysql-cli-1.1.0/setup.cfg
+-rw-r--r--   0 will4j    (1000) will4j    (1000)      194 2022-12-22 06:38:46.000000 mysql-cli-1.1.0/setup.py
+drwxr-xr-x   0 will4j    (1000) will4j    (1000)        0 2023-04-18 08:25:29.807120 mysql-cli-1.1.0/tests/
+-rw-r--r--   0 will4j    (1000) will4j    (1000)      891 2022-12-22 11:03:41.000000 mysql-cli-1.1.0/tests/test_client.py
+-rw-r--r--   0 will4j    (1000) will4j    (1000)     9663 2023-04-18 08:16:54.000000 mysql-cli-1.1.0/tests/test_query.py
```

### Comparing `mysql-cli-1.0.0/PKG-INFO` & `mysql-cli-1.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql-cli
-Version: 1.0.0
+Version: 1.1.0
 Summary: A MySQL Python Client
 Author-email: William Wang <williamw0825@gmail.com>
 Project-URL: Homepage, https://github.com/will4j/mysql-cli-py
 Project-URL: Bug Tracker, https://github.com/will4j/mysql-cli-py/issues
 Keywords: MySQL,Python,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -133,14 +133,17 @@
 assert insert({"name": "hello", "cnt": 2}) == 1 # lastrowid
 params = [{"name": "world", "cnt": 1}, {"name": "world", "cnt": 2}]
 assert batch_insert(params) == 2 # affected_rows
 ```
 ### Select
 `Select` execute select SQL and return one row.  
 `SelectMany` execute select SQL and return list of rows.
+
+support use ":word" or ? as a placeholder, but when the use of ":word" placeholder does not allow to use "?" as a placeholder
+
 Returned row is dictionary by default, you can set `dictionary=False` to return row as tuple.
 ```python
 from mysql_cli import Select, SelectMany
 
 
 @Select("select id, name, cnt from my_test where name = ? limit 1;", dictionary=False)
 def select_one_return_tuple(name):
@@ -152,48 +155,106 @@
     return name
 
 
 @SelectMany("select name, cnt from my_test where name = ? order by cnt asc;")
 def select_many_by_name(name):
     return name
 
+@Select("select id, name, cnt from my_test where name = ? and cnt in (?) limit 1;", dictionary=False)
+def select_one_by_in(name,cnt):
+    return name,cnt
+
+@Select("select id, name, cnt from my_test where name = ? and cnt in (?) limit ? offset ?;", dictionary=False)
+def select_one_by_in_more_condition(name,cnt,limit,offset):
+    return name,cnt,limit,offset
+
+@Select("select id, name, cnt from my_test where name = :name and cnt in (:cnt) limit :limit offset :offset;", dictionary=False)
+def select_one_by_word_placeholders(params: dict):
+    return params
+
 
 row = select_one_return_tuple("hello")
 assert row == (1, 'hello', 2)
 row = select_one_return_dict("hello")
 assert row == {'id': 1, 'name': 'hello', 'cnt': 2}
 rows = select_many_by_name("hello")
 assert len(rows) == 2
 assert rows[0] == {'id': 1, 'name': 'hello', 'cnt': 2}
+row = select_one_by_in("world",[2,3])
+assert row == (4, 'world', 2)
+row = select_one_by_in_more_condition("world", [2, 3],1,1)
+assert row == (5, 'world', 3)
+params = {
+    "cnt":[2,3],
+    "name":"world",
+    "limit":1,
+    "offset":1,
+}
+row1 = select_one_by_word_placeholders(params=params)
+assert row == row1
 ```
 ### Update
 `Update` execute update SQL and return affected row number.
+
+support use ":word" or ? as a placeholder, but when the use of ":word" placeholder does not allow to use "?" as a placeholder
+
 ```python
 from mysql_cli import Update
 
 
 @Update("update my_test set cnt = ? where name = ? limit ?;")
 def update_cnt_by_name(name, cnt, limit=10):
     return cnt, name, limit
 
+@Update("update my_test set cnt = ? where name in (?) limit ?;")
+def update_cnt_by_name_and_in(name, cnt, limit=10):
+    return cnt, name, limit
+
+@Update("update my_test set cnt = :cnt where name in (:name) limit :limit;")
+def update_cnt_by_word_placeholders(params:dict):
+    return params
+
 
 assert update_cnt_by_name("update_many", 0) == 3 # affected_rows
+assert update_cnt_by_name_and_in(["update_one", "update_many"], 4, 2) == 2
+params = {
+    "name":["update_one", "update_many"],
+    "cnt":5,
+    "limit":2,
+}
+assert update_cnt_by_word_placeholders(params=params) == 2
 ```
 ### Delete
 `Delete` execute delete SQL and return affected row number.
+
+support use ":word" or ? as a placeholder, but when the use of ":word" placeholder does not allow to use "?" as a placeholder
 ```python
 from mysql_cli import Delete
 
 
 @Delete("delete from my_test where name = ? limit ?;")
 def delete_by_name(name, limit=10):
     return name, limit
 
+@Delete("delete from my_test where name in (?) and cnt in (?) limit ?;")
+def delete_by_in(name, cnt, limit=10):
+    return name, cnt, limit
+
+@Delete("delete from my_test where name in (:name) and cnt = :cnt limit :limit;")
+def delete_by_word_placeholders(params:dict):
+    return params
 
 assert delete_by_name("delete_many") == 2 # affected_rows
+assert delete_by_in(["delete_one"], [1,2]) == 2
+params = {
+    "cnt":2,
+    "name":["delete_one","delete_two"],
+    "limit": 1,
+}
+assert delete_by_word_placeholders(params=params) == 1
 ```
 
 ### Transactional
 `Transactional` will start a SQL transaction and control commit or rollback based on decorated method's return. Connection and cursor will be shared in thread local among query decorators. If `Transactional` appears multiple times, they will be merged into one transaction, the very first `Transactional` decides whether to commit or rollback transaction.
 
 ```python
 from mysql_cli import BatchInsert, Select, Transactional
@@ -218,9 +279,10 @@
     raise RuntimeError("rollback")
 
 
 transaction_rollback()
 assert select_one_return_dict("tx_rollback") is None
 ```
 
+
 ## References
 1. https://dev.mysql.com/doc/connector-python/en/connector-python-api-mysqlcursorprepared.html
```

### Comparing `mysql-cli-1.0.0/README.md` & `mysql-cli-1.1.0/mysql_cli.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: mysql-cli
+Version: 1.1.0
+Summary: A MySQL Python Client
+Author-email: William Wang <williamw0825@gmail.com>
+Project-URL: Homepage, https://github.com/will4j/mysql-cli-py
+Project-URL: Bug Tracker, https://github.com/will4j/mysql-cli-py/issues
+Keywords: MySQL,Python,client
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MySQL Python Client
 A MySQL python client based on [mysql-connector-python](https://github.com/mysql/mysql-connector-python), with friendly interface and full-featured client configuration.  
 Compare with the way which only takes table names and SQL parameters as input and assembles SQL statement internally, I personally prefer developer taking complete control of SQL, making it flexible which means you can use whatever SQL feature as you need, clear which means the final statement is obviously what you see in code and also no redundant part like '1=1' ever appear, also it's easier to debug and optimize as long as you can see the whole picture.
 
 ## Installation
 ### use pip
 ```bash
@@ -118,14 +133,17 @@
 assert insert({"name": "hello", "cnt": 2}) == 1 # lastrowid
 params = [{"name": "world", "cnt": 1}, {"name": "world", "cnt": 2}]
 assert batch_insert(params) == 2 # affected_rows
 ```
 ### Select
 `Select` execute select SQL and return one row.  
 `SelectMany` execute select SQL and return list of rows.
+
+support use ":word" or ? as a placeholder, but when the use of ":word" placeholder does not allow to use "?" as a placeholder
+
 Returned row is dictionary by default, you can set `dictionary=False` to return row as tuple.
 ```python
 from mysql_cli import Select, SelectMany
 
 
 @Select("select id, name, cnt from my_test where name = ? limit 1;", dictionary=False)
 def select_one_return_tuple(name):
@@ -137,48 +155,106 @@
     return name
 
 
 @SelectMany("select name, cnt from my_test where name = ? order by cnt asc;")
 def select_many_by_name(name):
     return name
 
+@Select("select id, name, cnt from my_test where name = ? and cnt in (?) limit 1;", dictionary=False)
+def select_one_by_in(name,cnt):
+    return name,cnt
+
+@Select("select id, name, cnt from my_test where name = ? and cnt in (?) limit ? offset ?;", dictionary=False)
+def select_one_by_in_more_condition(name,cnt,limit,offset):
+    return name,cnt,limit,offset
+
+@Select("select id, name, cnt from my_test where name = :name and cnt in (:cnt) limit :limit offset :offset;", dictionary=False)
+def select_one_by_word_placeholders(params: dict):
+    return params
+
 
 row = select_one_return_tuple("hello")
 assert row == (1, 'hello', 2)
 row = select_one_return_dict("hello")
 assert row == {'id': 1, 'name': 'hello', 'cnt': 2}
 rows = select_many_by_name("hello")
 assert len(rows) == 2
 assert rows[0] == {'id': 1, 'name': 'hello', 'cnt': 2}
+row = select_one_by_in("world",[2,3])
+assert row == (4, 'world', 2)
+row = select_one_by_in_more_condition("world", [2, 3],1,1)
+assert row == (5, 'world', 3)
+params = {
+    "cnt":[2,3],
+    "name":"world",
+    "limit":1,
+    "offset":1,
+}
+row1 = select_one_by_word_placeholders(params=params)
+assert row == row1
 ```
 ### Update
 `Update` execute update SQL and return affected row number.
+
+support use ":word" or ? as a placeholder, but when the use of ":word" placeholder does not allow to use "?" as a placeholder
+
 ```python
 from mysql_cli import Update
 
 
 @Update("update my_test set cnt = ? where name = ? limit ?;")
 def update_cnt_by_name(name, cnt, limit=10):
     return cnt, name, limit
 
+@Update("update my_test set cnt = ? where name in (?) limit ?;")
+def update_cnt_by_name_and_in(name, cnt, limit=10):
+    return cnt, name, limit
+
+@Update("update my_test set cnt = :cnt where name in (:name) limit :limit;")
+def update_cnt_by_word_placeholders(params:dict):
+    return params
+
 
 assert update_cnt_by_name("update_many", 0) == 3 # affected_rows
+assert update_cnt_by_name_and_in(["update_one", "update_many"], 4, 2) == 2
+params = {
+    "name":["update_one", "update_many"],
+    "cnt":5,
+    "limit":2,
+}
+assert update_cnt_by_word_placeholders(params=params) == 2
 ```
 ### Delete
 `Delete` execute delete SQL and return affected row number.
+
+support use ":word" or ? as a placeholder, but when the use of ":word" placeholder does not allow to use "?" as a placeholder
 ```python
 from mysql_cli import Delete
 
 
 @Delete("delete from my_test where name = ? limit ?;")
 def delete_by_name(name, limit=10):
     return name, limit
 
+@Delete("delete from my_test where name in (?) and cnt in (?) limit ?;")
+def delete_by_in(name, cnt, limit=10):
+    return name, cnt, limit
+
+@Delete("delete from my_test where name in (:name) and cnt = :cnt limit :limit;")
+def delete_by_word_placeholders(params:dict):
+    return params
 
 assert delete_by_name("delete_many") == 2 # affected_rows
+assert delete_by_in(["delete_one"], [1,2]) == 2
+params = {
+    "cnt":2,
+    "name":["delete_one","delete_two"],
+    "limit": 1,
+}
+assert delete_by_word_placeholders(params=params) == 1
 ```
 
 ### Transactional
 `Transactional` will start a SQL transaction and control commit or rollback based on decorated method's return. Connection and cursor will be shared in thread local among query decorators. If `Transactional` appears multiple times, they will be merged into one transaction, the very first `Transactional` decides whether to commit or rollback transaction.
 
 ```python
 from mysql_cli import BatchInsert, Select, Transactional
@@ -203,9 +279,10 @@
     raise RuntimeError("rollback")
 
 
 transaction_rollback()
 assert select_one_return_dict("tx_rollback") is None
 ```
 
+
 ## References
 1. https://dev.mysql.com/doc/connector-python/en/connector-python-api-mysqlcursorprepared.html
```

### Comparing `mysql-cli-1.0.0/mysql_cli/client.py` & `mysql-cli-1.1.0/mysql_cli/client.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import tomli
-
-from mysql.connector.pooling import MySQLConnectionPool, PooledMySQLConnection
-
-
-class MySQLWrapper:
-    # borg pattern
-    _shared_state = {}
-
-    def __init__(self, pool: MySQLConnectionPool = None):
-        self.__dict__ = self._shared_state
-        if pool is not None:
-            self.mysql_connection_pool = pool
-
-    @classmethod
-    def get_connection(cls) -> PooledMySQLConnection:
-        new_instance = cls()
-        if not hasattr(new_instance, "mysql_connection_pool"):
-            raise RuntimeError("MySQL not inited, see mysql_cli.init_from_* method.")
-        return new_instance.mysql_connection_pool.get_connection()
-
-    @classmethod
-    def init_from_conf_dict(cls, mysql_conf: dict):
-        return cls(MySQLConnectionPool(**mysql_conf))
-
-    @classmethod
-    def init_from_conf_file(cls, mysql_conf_file):
-        """
-        mysql conf from toml file
-        :param mysql_conf_file: toml file path
-        :return:
-        """
-        mysql_conf = parse_mysql_conf(mysql_conf_file)
-        return cls(MySQLConnectionPool(**mysql_conf))
-
-
-def parse_mysql_conf(mysql_conf_file):
-    with open(mysql_conf_file) as f:
-        return tomli.loads(f.read())
+import tomli
+
+from mysql.connector.pooling import MySQLConnectionPool, PooledMySQLConnection
+
+
+class MySQLWrapper:
+    # borg pattern
+    _shared_state = {}
+
+    def __init__(self, pool: MySQLConnectionPool = None):
+        self.__dict__ = self._shared_state
+        if pool is not None:
+            self.mysql_connection_pool = pool
+
+    @classmethod
+    def get_connection(cls) -> PooledMySQLConnection:
+        new_instance = cls()
+        if not hasattr(new_instance, "mysql_connection_pool"):
+            raise RuntimeError("MySQL not inited, see mysql_cli.init_from_* method.")
+        return new_instance.mysql_connection_pool.get_connection()
+
+    @classmethod
+    def init_from_conf_dict(cls, mysql_conf: dict):
+        return cls(MySQLConnectionPool(**mysql_conf))
+
+    @classmethod
+    def init_from_conf_file(cls, mysql_conf_file):
+        """
+        mysql conf from toml file
+        :param mysql_conf_file: toml file path
+        :return:
+        """
+        mysql_conf = parse_mysql_conf(mysql_conf_file)
+        return cls(MySQLConnectionPool(**mysql_conf))
+
+
+def parse_mysql_conf(mysql_conf_file):
+    with open(mysql_conf_file) as f:
+        return tomli.loads(f.read())
```

