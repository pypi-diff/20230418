# Comparing `tmp/nua-0.5.11.tar.gz` & `tmp/nua-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua-0.5.11.tar", max compression
+gzip compressed data, was "nua-0.5.8.tar", max compression
```

## Comparing `nua-0.5.11.tar` & `nua-0.5.8.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     1280 2023-04-18 16:54:57.863021 nua-0.5.11/pyproject.toml
--rw-r--r--   0        0        0     1994 2023-04-12 10:06:30.438962 nua-0.5.11/readme.md
--rw-r--r--   0        0        0        0 2023-01-02 15:45:01.827907 nua-0.5.11/src/nua_cli/__init__.py
--rw-r--r--   0        0        0     2029 2023-04-17 10:11:29.772670 nua-0.5.11/src/nua_cli/client.py
--rw-r--r--   0        0        0        0 2023-02-08 20:21:55.685155 nua-0.5.11/src/nua_cli/commands/__init__.py
--rw-r--r--   0        0        0     1010 2023-04-17 10:06:21.226164 nua-0.5.11/src/nua_cli/commands/apps.py
--rw-r--r--   0        0        0      464 2023-04-17 10:06:36.592612 nua-0.5.11/src/nua_cli/commands/backup.py
--rw-r--r--   0        0        0     3373 2023-04-17 10:12:01.970928 nua-0.5.11/src/nua_cli/commands/build.py
--rw-r--r--   0        0        0      963 2023-04-17 18:21:32.441064 nua-0.5.11/src/nua_cli/commands/config.py
--rw-r--r--   0        0        0     1490 2023-04-17 18:21:32.441043 nua-0.5.11/src/nua_cli/commands/env.py
--rw-r--r--   0        0        0      490 2023-04-17 10:09:42.111936 nua-0.5.11/src/nua_cli/commands/help.py
--rw-r--r--   0        0        0     1799 2023-04-17 10:11:29.781769 nua-0.5.11/src/nua_cli/commands/lifecycle.py
--rw-r--r--   0        0        0      823 2023-04-17 10:10:22.613380 nua-0.5.11/src/nua_cli/commands/logs.py
--rw-r--r--   0        0        0      172 2023-04-17 10:10:35.298837 nua-0.5.11/src/nua_cli/commands/main.py
--rw-r--r--   0        0        0     2520 2023-04-17 18:21:32.441152 nua-0.5.11/src/nua_cli/commands/server.py
--rw-r--r--   0        0        0     1345 2023-04-11 21:17:25.337231 nua-0.5.11/src/nua_cli/common.py
--rw-r--r--   0        0        0     1622 2023-04-17 20:52:17.865921 nua-0.5.11/src/nua_cli/main.py
--rw-r--r--   0        0        0      103 2023-01-06 22:10:31.942417 nua-0.5.11/src/nua_cli/version.py
--rw-r--r--   0        0        0     2490 1970-01-01 00:00:00.000000 nua-0.5.11/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-04-13 09:53:05.626200 nua-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     1994 2023-04-12 10:06:30.438962 nua-0.5.8/readme.md
+-rw-r--r--   0        0        0        0 2023-01-02 15:45:01.827907 nua-0.5.8/src/nua_cli/__init__.py
+-rw-r--r--   0        0        0     6506 2023-04-13 06:22:42.919805 nua-0.5.8/src/nua_cli/base.py
+-rw-r--r--   0        0        0     2032 2023-04-12 14:30:30.888082 nua-0.5.8/src/nua_cli/client.py
+-rw-r--r--   0        0        0      313 2023-04-11 21:17:25.332899 nua-0.5.8/src/nua_cli/colors.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:21:55.685155 nua-0.5.8/src/nua_cli/commands/__init__.py
+-rw-r--r--   0        0        0     1024 2023-04-12 12:47:44.478176 nua-0.5.8/src/nua_cli/commands/apps.py
+-rw-r--r--   0        0        0      478 2023-04-12 10:07:34.002570 nua-0.5.8/src/nua_cli/commands/backup.py
+-rw-r--r--   0        0        0      849 2023-04-11 21:17:25.332143 nua-0.5.8/src/nua_cli/commands/build.py
+-rw-r--r--   0        0        0      960 2023-04-13 07:58:37.131820 nua-0.5.8/src/nua_cli/commands/config.py
+-rw-r--r--   0        0        0     1476 2023-04-13 08:14:53.074209 nua-0.5.8/src/nua_cli/commands/env.py
+-rw-r--r--   0        0        0      496 2023-04-11 21:17:25.334547 nua-0.5.8/src/nua_cli/commands/help.py
+-rw-r--r--   0        0        0     1805 2023-04-12 12:48:11.107863 nua-0.5.8/src/nua_cli/commands/lifecycle.py
+-rw-r--r--   0        0        0      821 2023-04-13 07:58:37.131453 nua-0.5.8/src/nua_cli/commands/logs.py
+-rw-r--r--   0        0        0      171 2023-04-11 21:17:25.335842 nua-0.5.8/src/nua_cli/commands/main.py
+-rw-r--r--   0        0        0     2463 2023-04-12 12:33:13.257321 nua-0.5.8/src/nua_cli/commands/server.py
+-rw-r--r--   0        0        0     1345 2023-04-11 21:17:25.337231 nua-0.5.8/src/nua_cli/common.py
+-rw-r--r--   0        0        0      168 2023-04-11 21:17:25.337653 nua-0.5.8/src/nua_cli/exceptions.py
+-rw-r--r--   0        0        0     1363 2023-04-12 08:38:41.344743 nua-0.5.8/src/nua_cli/main.py
+-rw-r--r--   0        0        0      103 2023-01-06 22:10:31.942417 nua-0.5.8/src/nua_cli/version.py
+-rw-r--r--   0        0        0     2468 1970-01-01 00:00:00.000000 nua-0.5.8/PKG-INFO
```

### Comparing `nua-0.5.11/pyproject.toml` & `nua-0.5.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "nua"
-version = "0.5.11"
+version = "0.5.8"
 description = ""
 authors = ["Stefane Fermigier <sf@abilian.com>"]
 readme = "readme.md"
 packages = [
   { include = "nua_cli", from = "src" }
 ]
 
 [tool.poetry.scripts]
-nua = "nua_cli.main:main"
+nua = "nua_cli.main:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
+
 tomli = "^2.0.1"
 fabric = "^3.0.0"
+# Temp: use snoop in prod code
 snoop = "*"
+
+# typer = "^0.7.0"
 termcolor = "^2.2.0"
-cleez = "*"
 
 [tool.poetry.group.dev.dependencies]
 abilian-devtools = "*"
 devtools = "*"
 types-setuptools = "*"
 
 # To please poetry
```

### Comparing `nua-0.5.11/readme.md` & `nua-0.5.8/readme.md`

 * *Files identical despite different names*

### Comparing `nua-0.5.11/src/nua_cli/client.py` & `nua-0.5.8/src/nua_cli/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import os
 import sys
 from io import StringIO
 
-from cleez.colors import red
 from fabric import Connection
 
+from nua_cli.colors import red
+
 # Hardcoded for now
 NUA_CMD = "./env/bin/nua-orchestrator"
 
 
 class Client:
     connection: Connection
```

### Comparing `nua-0.5.11/src/nua_cli/commands/apps.py` & `nua-0.5.8/src/nua_cli/commands/apps.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from cleez import Command
-from cleez.colors import green, red, yellow
-
-from ..client import get_client
+from nua_cli.base import Command
+from nua_cli.client import get_client
+from nua_cli.colors import green, red, yellow
 
 client = get_client()
 
 
 class AppsCommand(Command):
     """List applications."""
```

### Comparing `nua-0.5.11/src/nua_cli/commands/config.py` & `nua-0.5.8/src/nua_cli/commands/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 from pprint import pp
 
-from cleez import Command, CommandError
-from cleez.command import Argument
-
-from ..client import get_client
-from ..common import get_current_app_id
+from nua_cli.base import Argument, Command
+from nua_cli.client import get_client
+from nua_cli.common import get_current_app_id
+from nua_cli.exceptions import CommandError
 
 client = get_client()
 
 
-class ConfigCommand(Command):
-    """Show/edit application config."""
-
-    name = "config"
-    hide_from_help = True
-
-    def run(self):
-        self.cli.print_help()
-
-
 class ShowCommand(Command):
     """Show application config."""
 
     name = "config show"
 
     arguments = [
         Argument("app_id", nargs="?", help="Id of the application."),
@@ -38,7 +27,16 @@
 
         for instance in result:
             if instance["app_id"] == app_id:
                 pp(instance)
                 break
         else:
             raise CommandError(f"App {app_id} not found")
+
+
+class ConfigCommand(Command):
+    """Show/edit application config."""
+
+    name = "config"
+
+    def run(self):
+        self.cli.print_help()
```

### Comparing `nua-0.5.11/src/nua_cli/commands/env.py` & `nua-0.5.8/src/nua_cli/commands/env.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,15 @@
-from cleez.colors import bold, red
-from cleez.command import Argument, Command
-
-from ..client import get_client
-from ..common import get_current_app_id
+from nua_cli.base import Argument, Command
+from nua_cli.client import get_client
+from nua_cli.colors import bold, red
+from nua_cli.common import get_current_app_id
 
 client = get_client()
 
 
-class EnvCommand(Command):
-    """Manage an app's env variables."""
-
-    name = "env"
-    hide_from_help = True
-
-    def run(self):
-        self.cli.print_help()
-
-
 class EnvShowCommand(Command):
     """Show application env variables."""
 
     name = "env show"
 
     arguments = [
         Argument("app_id", nargs="?", help="Application ID"),
@@ -52,7 +41,16 @@
 class EnvSetCommand(Command):
     """Show application env variables."""
 
     name = "env set"
 
     def run(self, app_id: str = ""):
         print(red("Not implemented yet"))
+
+
+class EnvCommand(Command):
+    """Manage an app's env variables."""
+
+    name = "env"
+
+    def run(self):
+        self.cli.print_help()
```

### Comparing `nua-0.5.11/src/nua_cli/commands/lifecycle.py` & `nua-0.5.8/src/nua_cli/commands/lifecycle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from cleez.colors import red
-from cleez.command import Argument, Command
-
-from ..client import get_client
+from nua_cli.base import Argument, Command
+from nua_cli.client import get_client
+from nua_cli.colors import red
 
 client = get_client()
 
 # Hardcoded for now
 ORCH_PATH = "/home/nua/env/bin/nua-orchestrator"
```

### Comparing `nua-0.5.11/src/nua_cli/commands/logs.py` & `nua-0.5.8/src/nua_cli/commands/logs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from cleez.command import Argument, Command
-
+from nua_cli.base import Argument, Command
 from nua_cli.client import get_client
 from nua_cli.common import get_current_app_id
 
 client = get_client()
 
 
 class LogsCommand(Command):
```

### Comparing `nua-0.5.11/src/nua_cli/commands/server.py` & `nua-0.5.8/src/nua_cli/commands/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 from operator import itemgetter
 from pprint import pp
 
-from cleez import BadArgumentError
-from cleez.command import Argument, Command
-
-from ..client import get_client
+from nua_cli.base import Argument, Command
+from nua_cli.client import get_client
+from nua_cli.exceptions import BadArgument
 
 client = get_client()
 
 
-class ServerCommand(Command):
-    """Manage the Nua server."""
-
-    name = "server"
-    hide_from_help = True
-
-    def run(self):
-        self.cli.print_help()
-
-
 class LogsCommand(Command):
     """Show server logs."""
 
     name = "server logs"
 
     arguments = [
         Argument("service", help="Service to show logs for"),
@@ -37,17 +26,15 @@
                 print("Showing Nua logs [TODO]")
             case "letsencrypt":
                 result = client.ssh("cat log/letsencrypt/letsencrypt.log")
                 print(result.stdout)
             case "nginx":
                 print("Showing Nginx logs [TODO]")
             case _:
-                raise BadArgumentError(
-                    "Service must be one of: nua, letsencrypt, nginx"
-                )
+                raise BadArgument("Service must be one of: nua, letsencrypt, nginx")
 
 
 class StatusCommand(Command):
     """Show Nua status."""
 
     name = "server status"
 
@@ -104,7 +91,16 @@
 
     # TODO: ask for confirmation
 
     def run(self):
         result = client.ssh("docker system prune -af")
         result = client.ssh("docker volume prune -f")
         print(result.stdout)
+
+
+class ServerCommand(Command):
+    """Manage the Nua server."""
+
+    name = "server"
+
+    def run(self):
+        self.cli.print_help()
```

### Comparing `nua-0.5.11/src/nua_cli/common.py` & `nua-0.5.8/src/nua_cli/common.py`

 * *Files identical despite different names*

### Comparing `nua-0.5.11/src/nua_cli/main.py` & `nua-0.5.8/src/nua_cli/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,62 +4,49 @@
 [x] = done
 [ ] = not done
 
 [x] apps              List apps
 [x] build             Build app but don't deploy it
 [x] backup            Backup/restore app data
 [x] config            Show/manage config for current app
-[x] deploy            Deploy app
-[x] destroy           Destroy app
-[x] help              Display help
+[ ] deploy            Deploy app
+[ ] destroy           Destroy app
+[ ] help              Display help
 [ ] init              Create a new app
 [x] logs              Tail running logs
-[x] restart           Restart an app
+[ ] restart           Restart an app
 [ ] run               Run a command in the app's environment
 [ ] scale             Scale processes
-[x] server            Manage the Nua server
-[x] start             Start an app
-[x] status            Show app status
-[x] stop              Stop an app
+[ ] server            Manage the Nua server
+[ ] start             Start an app
+[ ] status            Show app status
+[ ] stop              Stop an app
 [ ] update            Update an app
 [x] version           Show Nua version
 """
 from __future__ import annotations
 
-import importlib.metadata
-
 import snoop
-from cleez import CLI
+
+from nua_cli.base import CLI
 
 snoop.install()
 
 
-# Quick hack for now
-class MyCli(CLI):
-    def get_version(self):
-        return importlib.metadata.version("nua.cli")
-
-
-def main():
-    cli = MyCli("nua")
-    cli.add_option(
-        "-h", "--help", default=False, action="store_true", help="Show help and exit"
-    )
-    cli.add_option(
-        "-V",
-        "--version",
-        default=False,
-        action="store_true",
-        help="Show version and exit",
-    )
-    cli.add_option(
-        "-d", "--debug", default=False, action="store_true", help="Enable debug mode"
-    )
-    cli.add_option(
-        "-v", "--verbose", default=False, action="store_true", help="Increase verbosity"
-    )
-    cli.scan("nua_cli.commands")
-    cli.run()
+cli = CLI()
+cli.add_option(
+    "-h", "--help", default=False, action="store_true", help="Show help and exit"
+)
+cli.add_option(
+    "-V", "--version", default=False, action="store_true", help="Show version and exit"
+)
+cli.add_option(
+    "-d", "--debug", default=False, action="store_true", help="Enable debug mode"
+)
+cli.add_option(
+    "-v", "--verbose", default=False, action="store_true", help="Increase verbosity"
+)
+cli.scan("nua_cli.commands")
 
 
 if __name__ == "__main__":
-    main()
+    cli.run()
```

### Comparing `nua-0.5.11/PKG-INFO` & `nua-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: nua
-Version: 0.5.11
+Version: 0.5.8
 Summary: 
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cleez
 Requires-Dist: fabric (>=3.0.0,<4.0.0)
 Requires-Dist: snoop
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # nua-cli: CLI for NUA (for users)
```

