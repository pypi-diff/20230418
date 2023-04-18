# Comparing `tmp/mechanical_bull-0.0.4.tar.gz` & `tmp/mechanical_bull-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanical_bull-0.0.4.tar", max compression
+gzip compressed data, was "mechanical_bull-0.0.5.tar", max compression
```

## Comparing `mechanical_bull-0.0.4.tar` & `mechanical_bull-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1062 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/LICENSE
--rw-r--r--   0        0        0     1798 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-04-16 16:46:42.697227 mechanical_bull-0.0.4/mechanical_bull/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 16:46:42.697227 mechanical_bull-0.0.4/mechanical_bull/actions/__init__.py
--rw-r--r--   0        0        0      196 2023-04-16 16:47:06.613418 mechanical_bull-0.0.4/mechanical_bull/actions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1206 2023-04-16 16:47:06.617418 mechanical_bull-0.0.4/mechanical_bull/actions/__pycache__/handle_follow_request.cpython-311.pyc
--rw-r--r--   0        0        0      930 2023-04-16 16:47:06.625418 mechanical_bull-0.0.4/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc
--rw-r--r--   0        0        0     1648 2023-04-16 16:47:06.613418 mechanical_bull-0.0.4/mechanical_bull/actions/__pycache__/test_handle_follow_request.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      491 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/mechanical_bull/actions/handle_follow_request.py
--rw-r--r--   0        0        0      225 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/mechanical_bull/actions/log_to_file.py
--rw-r--r--   0        0        0      611 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/mechanical_bull/actions/test_handle_follow_request.py
--rw-r--r--   0        0        0     1357 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/mechanical_bull/add_user.py
--rw-r--r--   0        0        0      787 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/mechanical_bull/event_loop.py
--rw-r--r--   0        0        0      335 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/mechanical_bull/handlers.py
--rw-r--r--   0        0        0      685 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/mechanical_bull/run.py
--rw-r--r--   0        0        0      542 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/mechanical_bull/test_event_loop.py
--rw-r--r--   0        0        0      484 2023-04-16 16:46:42.601226 mechanical_bull-0.0.4/mechanical_bull/test_handlers.py
--rw-r--r--   0        0        0      706 2023-04-16 16:46:42.605226 mechanical_bull-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 mechanical_bull-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3161 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 13:15:41.978646 mechanical_bull-0.0.5/mechanical_bull/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 13:15:41.978646 mechanical_bull-0.0.5/mechanical_bull/actions/__init__.py
+-rw-r--r--   0        0        0      196 2023-04-18 13:16:06.350846 mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1206 2023-04-18 13:16:06.350846 mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc
+-rw-r--r--   0        0        0      930 2023-04-18 13:16:06.362846 mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc
+-rw-r--r--   0        0        0     1236 2023-04-18 13:16:06.350846 mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/reject_follow_request.cpython-311.pyc
+-rw-r--r--   0        0        0     1985 2023-04-18 13:16:06.350846 mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/test_accept_reject_follow_request.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      491 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/actions/accept_follow_request.py
+-rw-r--r--   0        0        0      225 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/actions/log_to_file.py
+-rw-r--r--   0        0        0      521 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/actions/reject_follow_request.py
+-rw-r--r--   0        0        0      847 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/actions/test_accept_reject_follow_request.py
+-rw-r--r--   0        0        0     1362 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/add_user.py
+-rw-r--r--   0        0        0      787 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/event_loop.py
+-rw-r--r--   0        0        0      335 2023-04-18 13:15:41.910645 mechanical_bull-0.0.5/mechanical_bull/handlers.py
+-rw-r--r--   0        0        0      685 2023-04-18 13:15:41.914645 mechanical_bull-0.0.5/mechanical_bull/run.py
+-rw-r--r--   0        0        0      542 2023-04-18 13:15:41.914645 mechanical_bull-0.0.5/mechanical_bull/test_event_loop.py
+-rw-r--r--   0        0        0      484 2023-04-18 13:15:41.914645 mechanical_bull-0.0.5/mechanical_bull/test_handlers.py
+-rw-r--r--   0        0        0      683 2023-04-18 13:15:41.914645 mechanical_bull-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 mechanical_bull-0.0.5/PKG-INFO
```

### Comparing `mechanical_bull-0.0.4/LICENSE` & `mechanical_bull-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.4/mechanical_bull/actions/__pycache__/handle_follow_request.cpython-311.pyc` & `mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/accept_follow_request.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x72263c64 (Sun Apr 16 16:46:42 2023 UTC)
+moddate:  0xfd973e64 (Tue Apr 18 13:15:41 2023 UTC)
 files sz: 491
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -33,15 +33,15 @@
                 52 STORE_NAME               5 (logger)
    
      8          54 LOAD_CONST               3 ('actor')
                 56 LOAD_NAME                2 (BovineActor)
                 58 LOAD_CONST               4 ('data')
                 60 LOAD_NAME                6 (dict)
                 62 BUILD_TUPLE              4
-                64 LOAD_CONST               5 (<code object handle, file "/woodpecker/src/codeberg.org/bovine/mechanical_bull/mechanical_bull/actions/handle_follow_request.py", line 8>)
+                64 LOAD_CONST               5 (<code object handle, file "/woodpecker/src/codeberg.org/bovine/mechanical_bull/mechanical_bull/actions/accept_follow_request.py", line 8>)
                 66 MAKE_FUNCTION            4 (annotations)
                 68 STORE_NAME               7 (handle)
                 70 LOAD_CONST               1 (None)
                 72 RETURN_VALUE
    consts
       0
       None
@@ -145,19 +145,19 @@
             'id'
             'Accepting follow request from %s'
             ('to',)
          names      ('isinstance', 'dict', 'logger', 'info', 'activity_factory', 'accept', 'build', 'send_to_outbox')
          varnames   ('actor', 'data', 'follow_actor', 'accept')
          freevars   ()
          cellvars   ()
-         filename   '/woodpecker/src/codeberg.org/bovine/mechanical_bull/mechanical_bull/actions/handle_follow_request.py'
+         filename   '/woodpecker/src/codeberg.org/bovine/mechanical_bull/mechanical_bull/actions/accept_follow_request.py'
          name       'handle'
          firstlineno 8
          lnotab 0x06011801040210012a01100236027602
    names      ('logging', 'bovine', 'BovineActor', 'getLogger', '__name__', 'logger', 'dict', 'handle')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/woodpecker/src/codeberg.org/bovine/mechanical_bull/mechanical_bull/actions/handle_follow_request.py'
+   filename   '/woodpecker/src/codeberg.org/bovine/mechanical_bull/mechanical_bull/actions/accept_follow_request.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020108020c022003
```

### Comparing `mechanical_bull-0.0.4/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc` & `mechanical_bull-0.0.5/mechanical_bull/actions/__pycache__/log_to_file.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x72263c64 (Sun Apr 16 16:46:42 2023 UTC)
+moddate:  0xfd973e64 (Tue Apr 18 13:15:41 2023 UTC)
 files sz: 225
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `mechanical_bull-0.0.4/mechanical_bull/actions/test_handle_follow_request.py` & `mechanical_bull-0.0.5/mechanical_bull/actions/test_accept_reject_follow_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import pytest
 from unittest.mock import AsyncMock, MagicMock
 
 from bovine.activitystreams.activity_factory import Activity
-from .handle_follow_request import handle
+from .accept_follow_request import handle as handle_accept
+from .reject_follow_request import handle as handle_reject
 
 
-async def test_does_nothing_on_random_activity():
+@pytest.mark.parametrize("handle", [handle_accept, handle_reject])
+async def test_does_nothing_on_random_activity(handle):
     data = {"type": "Note"}
 
     client = AsyncMock()
 
     await handle(client, data)
 
     client.send_to_outbox.assert_not_awaited()
 
 
-async def test_replies_to_follow_with_accept():
+@pytest.mark.parametrize("handle", [handle_accept, handle_reject])
+async def test_replies_to_follow_with_accept(handle):
     data = Activity(id="uuid", type="Follow", actor="actor").build()
     client = AsyncMock()
     client.activity_factory.accept = MagicMock()
 
     await handle(client, data)
 
     client.send_to_outbox.assert_awaited_once()
```

### Comparing `mechanical_bull-0.0.4/mechanical_bull/add_user.py` & `mechanical_bull-0.0.5/mechanical_bull/add_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,23 +29,26 @@
     host = input("Please enter your host name: ")
     print()
     private_key = generate_ed25519_private_key()
     did_key = private_key_to_did_key(private_key)
 
     print(f"Please add {did_key} to the access list of your ActivityPub actor")
 
-    config[user] = {"private_key": private_key, "host": host, "handlers": {}}
+    config[user] = {
+        "private_key": private_key,
+        "host": host,
+    }
 
     with open(config_file, "wb") as fp:
         tomli_w.dump(config, fp)
 
     print()
     print("Please note the handlers for this user are currently empty.")
     print("To automatically accept follow requests include the block")
     print(
-        f"""[{user.handlers}]
-"mechanical_bull.actions.handle_follow_request"]] = true"""
+        f"""[{user}.handlers]
+"mechanical_bull.actions.handle_follow_request" = true"""
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mechanical_bull-0.0.4/mechanical_bull/event_loop.py` & `mechanical_bull-0.0.5/mechanical_bull/event_loop.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.4/mechanical_bull/run.py` & `mechanical_bull-0.0.5/mechanical_bull/run.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.4/mechanical_bull/test_event_loop.py` & `mechanical_bull-0.0.5/mechanical_bull/test_event_loop.py`

 * *Files identical despite different names*

### Comparing `mechanical_bull-0.0.4/pyproject.toml` & `mechanical_bull-0.0.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "mechanical-bull"
-version = "0.0.4"
+version = "0.0.5"
 description = "A framework to automate reacting to ActivityStreams events."
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "mechanical_bull"}]
-repository = "https://codeberg.org/helge/mechanical_bull"
+repository = "https://codeberg.org/bovine/mechanical_bull"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 tomli-w = "^1.0.0"
 bovine = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
-flake8 = "^6.0.0"
 black = "^23.1.0"
-flake8-black = "^0.3.6"
+ruff = "^0.0.261"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.pytest.ini_options]
```

### Comparing `mechanical_bull-0.0.4/PKG-INFO` & `mechanical_bull-0.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,10 @@
-Metadata-Version: 2.1
-Name: mechanical-bull
-Version: 0.0.4
-Summary: A framework to automate reacting to ActivityStreams events.
-Home-page: https://codeberg.org/helge/mechanical_bull
-License: MIT
-Author: Helge
-Author-email: helge.krueger@gmail.com
-Requires-Python: >=3.11,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bovine (>=0.1.1,<0.2.0)
-Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
-Project-URL: Repository, https://codeberg.org/helge/mechanical_bull
-Description-Content-Type: text/markdown
-
 # Mechanical Bull
 
-Mechanical Bull is an ActivityPub Client application build based on [bovine](https://codeberg.org/helge/bovine/). It's main goal is to provide a platform for automating activities undertaking in the FediVerse. Furthermore, it serves as a demonstration how ActivityPub Clients can be build with bovine.
+Mechanical Bull is an ActivityPub Client application build based on [bovine](https://codeberg.org/bovine/bovine/). It's main goal is to provide a platform for automating activities undertaking in the FediVerse. Furthermore, it serves as a demonstration how ActivityPub Clients can be build with bovine.
 
 ## Installation
 
 One can simply install mechanical_bull with pip via
 
 ```bash
 pip install mechanical-bull
@@ -39,23 +22,47 @@
 
 Then you should be able to run mechanical bull via
 
 ```bash
 python -m mechanical_bull.run
 ```
 
+## Configuration
+
+First by adding `log_file = "mechanical_bull.log"` to your `config.toml` you can make mechanical_bull write log entries to a file. Second, the config file has the following format
+
+```toml
+logfile = "mechanical_bull.log"
+
+[cow]
+private_key = "z3u2Yxcowsarethebestcowsarethebestcowsarethebest"
+host = "cows.rocks"
+
+[cow.handlers]
+"mechanical_bull.actions.reject_follow_request" = true
+# "mechanical_bull.actions.accept_follow_request" = true
+"mechanical_bull.actions.log_to_file" = { filename = "cow.txt" }
+```
+
+The listed handlers are provided by mechanical_bull. They allow to accept / reject follow requests automatically, and the final one logs all traffic on the event source to "cow.txt".
+
 ## Writing automations
 
-The examples of `mechanical_bull.actions.handle_follow_request` and `mechanical_bull.actions.log_to_file` should show how to write a new automation. The basic idea is that each file contains a function handle with signature
+The examples of `mechanical_bull.actions.accept_follow_request` and `mechanical_bull.actions.log_to_file` should show how to write a new automation. The basic idea is that each file contains a function handle with signature
 
 ```python
 async def handle(client: BovineClient, data: dict, **kwargs):
     return
 ```
 
 here the kwargs are the dict given by the definiton in the handler block, i.e.
 
 ```toml
 [user.handlers]
 "my.package" = { arg1 = "value1", arg2 = "value2 }
 ```
 
+## Contibuting
+
+Please report bugs, etc. to the [issue tracker](https://codeberg.org/bovine/mechanical_bull/issues). Contributings in the form of pull requests are welcome. You can also contact me on the FediVerse at `@helge@mymath.rocks`.
+
+Finally, I plan a multi-user "server" version of this project called __mechanical_herd__. The functionality should be similar, but updating the configuration should not require a restart. One might also think hooking into the redis from [bovine_pubsub](https://codeberg.org/bovine/bovine/src/branch/dev/bovine_pubsub) for this. mechanical_herd will probably be part of the bovine user management interface.
```

