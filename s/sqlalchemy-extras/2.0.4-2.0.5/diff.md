# Comparing `tmp/sqlalchemy_extras-2.0.4.tar.gz` & `tmp/sqlalchemy_extras-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_extras-2.0.4.tar", max compression
+gzip compressed data, was "sqlalchemy_extras-2.0.5.tar", max compression
```

## Comparing `sqlalchemy_extras-2.0.4.tar` & `sqlalchemy_extras-2.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.4/README.md
--rw-r--r--   0        0        0      790 2023-04-17 23:01:29.435274 sqlalchemy_extras-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      183 2023-03-09 19:01:38.717890 sqlalchemy_extras-2.0.4/sqlalchemy_extras/__init__.py
--rw-r--r--   0        0        0     5753 2023-04-17 23:01:49.106054 sqlalchemy_extras-2.0.4/sqlalchemy_extras/fastapi.py
--rw-r--r--   0        0        0     5402 2023-04-11 18:37:10.574642 sqlalchemy_extras-2.0.4/sqlalchemy_extras/models.py
--rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.4/sqlalchemy_extras/py.typed
--rw-r--r--   0        0        0     2092 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.4/sqlalchemy_extras/utils.py
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 sqlalchemy_extras-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.5/README.md
+-rw-r--r--   0        0        0      790 2023-04-17 23:36:02.330137 sqlalchemy_extras-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-03-09 19:01:38.717890 sqlalchemy_extras-2.0.5/sqlalchemy_extras/__init__.py
+-rw-r--r--   0        0        0     5599 2023-04-17 23:36:12.250308 sqlalchemy_extras-2.0.5/sqlalchemy_extras/fastapi.py
+-rw-r--r--   0        0        0     5402 2023-04-11 18:37:10.574642 sqlalchemy_extras-2.0.5/sqlalchemy_extras/models.py
+-rw-r--r--   0        0        0        0 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.5/sqlalchemy_extras/py.typed
+-rw-r--r--   0        0        0     2092 2023-03-09 18:34:58.457012 sqlalchemy_extras-2.0.5/sqlalchemy_extras/utils.py
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 sqlalchemy_extras-2.0.5/PKG-INFO
```

### Comparing `sqlalchemy_extras-2.0.4/pyproject.toml` & `sqlalchemy_extras-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Francisco Del Roio <francipvb@hotmail.com>"]
 description = ""
 name = "sqlalchemy-extras"
 readme = "README.md"
-version = "2.0.4"
+version = "2.0.5"
 
 [tool.poetry.dependencies]
 sqlalchemy = "^2.0.9"
 fastapi = { version = ">=0.60.0,<1.0.0", optional = true }
 python = ">=3.10.0, <4"
 
 [tool.poetry.extras]
```

### Comparing `sqlalchemy_extras-2.0.4/sqlalchemy_extras/fastapi.py` & `sqlalchemy_extras-2.0.5/sqlalchemy_extras/fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,21 +144,15 @@
         try:
             if in_transaction:
                 async with session.begin():
                     yield session
             else:
                 yield session
         finally:
-            while True:
-                try:
-                    await session.close()
-                except:
-                    continue
-                else:
-                    break
+            await session.close()
 
     @asynccontextmanager
     async def connection(
         self, *, in_transaction: bool = False
     ) -> AsyncGenerator[AsyncConnection, None]:
         connection_contextmanager: Optional[AsyncContextManager[AsyncConnection]] = None
         if in_transaction:
```

### Comparing `sqlalchemy_extras-2.0.4/sqlalchemy_extras/models.py` & `sqlalchemy_extras-2.0.5/sqlalchemy_extras/models.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_extras-2.0.4/sqlalchemy_extras/utils.py` & `sqlalchemy_extras-2.0.5/sqlalchemy_extras/utils.py`

 * *Files identical despite different names*

