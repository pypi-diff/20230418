# Comparing `tmp/prelude-cli-0.9.97.tar.gz` & `tmp/prelude-cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-0.9.97.tar", last modified: Thu Apr 13 13:54:34 2023, max compression
+gzip compressed data, was "prelude-cli-1.0.0.tar", last modified: Tue Apr 18 19:09:56 2023, max compression
```

## Comparing `prelude-cli-0.9.97.tar` & `prelude-cli-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:54:34.145863 prelude-cli-0.9.97/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      833 2023-04-13 13:54:34.145909 prelude-cli-0.9.97/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-0.9.97/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:54:34.142739 prelude-cli-0.9.97/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1078 2023-04-11 22:16:02.000000 prelude-cli-0.9.97/prelude_cli/cli.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:54:34.143715 prelude-cli-0.9.97/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-0.9.97/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:54:34.145648 prelude-cli-0.9.97/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-0.9.97/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-0.9.97/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     5966 2023-04-13 13:44:46.000000 prelude-cli-0.9.97/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3714 2023-04-13 13:44:46.000000 prelude-cli-0.9.97/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)    31169 2023-04-11 22:16:02.000000 prelude-cli-0.9.97/prelude_cli/views/interactive.py
--rw-r--r--   0 pack       (501) staff       (20)     1508 2023-04-11 22:16:02.000000 prelude-cli-0.9.97/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-0.9.97/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-13 13:54:34.143526 prelude-cli-0.9.97/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      833 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      608 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-04-13 13:54:34.000000 prelude-cli-0.9.97/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-0.9.97/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      679 2023-04-13 13:54:34.146135 prelude-cli-0.9.97/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:56.637009 prelude-cli-1.0.0/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-18 19:09:56.637062 prelude-cli-1.0.0/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.0.0/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:56.633476 prelude-cli-1.0.0/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1243 2023-04-18 14:03:55.000000 prelude-cli-1.0.0/prelude_cli/cli.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:56.634751 prelude-cli-1.0.0/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-1.0.0/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:56.636792 prelude-cli-1.0.0/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-1.0.0/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.0.0/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     6089 2023-04-18 17:04:09.000000 prelude-cli-1.0.0/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3763 2023-04-18 14:03:55.000000 prelude-cli-1.0.0/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)    29181 2023-04-18 17:04:09.000000 prelude-cli-1.0.0/prelude_cli/views/interactive.py
+-rw-r--r--   0 pack       (501) staff       (20)     1508 2023-04-11 22:16:02.000000 prelude-cli-1.0.0/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-1.0.0/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-18 19:09:56.634528 prelude-cli-1.0.0/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      608 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       59 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-04-18 19:09:56.000000 prelude-cli-1.0.0/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.0.0/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      690 2023-04-18 19:09:56.637282 prelude-cli-1.0.0/setup.cfg
```

### Comparing `prelude-cli-0.9.97/LICENSE` & `prelude-cli-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.97/PKG-INFO` & `prelude-cli-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 0.9.97
+Version: 1.0.0
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-0.9.97/prelude_cli/cli.py` & `prelude-cli-1.0.0/prelude_cli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 from prelude_cli.views.detect import detect
 from prelude_cli.views.partner import partner
 from prelude_sdk.models.account import Account
 from prelude_cli.views.configure import configure
 from prelude_cli.views.interactive import interactive as interactive_command
 
 
+def complete_profile(ctx, param, incomplete):
+    return [x for x in Account().read_keychain_config() if x.startswith(incomplete)]
+
 @click.group(invoke_without_command=True)
 @click.version_option()
 @click.pass_context
-@click.option('--profile', default='default', help='The prelude keychain profile to use', show_default=True)
+@click.option('--profile', default='default', help='The prelude keychain profile to use', show_default=True, shell_complete=complete_profile)
 @click.option('--interactive', help='Open interactive wizard (cannot be used with a subcommand)', default=False, is_flag=True)
 def cli(ctx, profile, interactive):
     ctx.obj = Account(profile=profile)
     if ctx.invoked_subcommand is None:
         if interactive:
             ctx.invoke(interactive_command)
         else:
```

### Comparing `prelude-cli-0.9.97/prelude_cli/views/build.py` & `prelude-cli-1.0.0/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.97/prelude_cli/views/configure.py` & `prelude-cli-1.0.0/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.97/prelude_cli/views/detect.py` & `prelude-cli-1.0.0/prelude_cli/views/detect.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,27 +42,28 @@
 @click.option('-t', '--tags', help='only enable for these tags (comma-separated list)', type=str, default='')
 @click.option('-r', '--run_code',
               help='provide a run_code',
               default=RunCode.DAILY.name, show_default=True,
               type=click.Choice([r.name for r in RunCode], case_sensitive=False))
 @click.pass_obj
 @handle_api_error
-def activate_test(controller, test, run_code, tags):
+def enable_test(controller, test, run_code, tags):
     """ Add test to your queue """
     controller.enable_test(ident=test, run_code=RunCode[run_code.upper()].value, tags=tags)
 
 
 @detect.command('disable-test')
 @click.argument('test')
+@click.option('-t', '--tags', help='only disable for these tags (comma-separated list)', type=str, default='')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
-def deactivate_test(controller, test):
+def disable_test(controller, test, tags):
     """ Remove test from your queue """
-    controller.disable_test(ident=test)
+    controller.disable_test(ident=test, tags=tags)
 
 
 @detect.command('social-stats')
 @click.argument('test')
 @click.option('-d', '--days', help='days to look back', default=30, type=int, show_default=True)
 @click.pass_obj
 @handle_api_error
```

### Comparing `prelude-cli-0.9.97/prelude_cli/views/iam.py` & `prelude-cli-1.0.0/prelude_cli/views/iam.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,16 @@
     expires = datetime.utcnow() + timedelta(days=days)
     resp = controller.create_user(
         handle=handle, 
         permission=Permission[permission.upper()].value, 
         expires=expires
     )
     print_json(data=resp)
-    print("\nCheck your email to verifiy your account.\n")
+    if permission != Permission.SERVICE.name:
+        print("\nCheck your email to verify your account.\n")
 
 @iam.command('delete-user')
 @click.confirmation_option(prompt='Are you sure?')
 @click.argument('handle')
 @click.pass_obj
 @handle_api_error
 def delete_user(controller, handle):
```

### Comparing `prelude-cli-0.9.97/prelude_cli/views/interactive.py` & `prelude-cli-1.0.0/prelude_cli/views/interactive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import os
 import uuid
 import click
 import shutil
 import socket
+import readline
 import webbrowser
 import prelude_cli.templates as templates
 import importlib.resources as pkg_resources
 
 from rich import print
+from rich.rule import Rule
 from rich.console import Console
 from rich.padding import Padding
 from rich.markdown import Markdown
 from pathlib import Path, PurePath
 from collections import OrderedDict
 from rich.prompt import Prompt, Confirm
 from simple_term_menu import TerminalMenu
 from datetime import datetime, timedelta, time
 
 from prelude_cli.views.shared import handle_api_error
 from prelude_sdk.controllers.iam_controller import IAMController
-from prelude_sdk.models.codes import RunCode, ExitCode, Permission
 from prelude_sdk.controllers.build_controller import BuildController
 from prelude_sdk.controllers.probe_controller import ProbeController
 from prelude_sdk.controllers.detect_controller import DetectController
+from prelude_sdk.models.codes import RunCode, ExitCode, Permission, Decision
 
 
 HELLO="""
 ```go
 package main
 
 // This is a Verified Security Test
@@ -63,27 +65,27 @@
         self.tests = dict()
         self.console = Console()
         self.filters = dict(
             start=datetime.combine(datetime.utcnow() - timedelta(days=30), time.min),
             finish=datetime.combine(datetime.utcnow(), time.max)
         )
 
-    def splash(self, markdown: str, helper: str = None):
+    def splash(self, markdown: str, short: str, helper: str = None):
+        print(Rule(short))
         identifier = hash(markdown)
-        if identifier not in self.cached_splashes:
+        if not os.getenv('PRELUDE_NOSPLASH') and identifier not in self.cached_splashes:
             self.console.print(Markdown(markdown))
             self.cached_splashes.append(identifier)
             if helper:
                 print(Padding(helper, 1))
+            return
 
+    @handle_api_error
     def load_tests(self):
-        try:
-            self.tests = {row['id']: row['name'] for row in self.detect.list_tests()}
-        except Exception:
-            pass
+        self.tests = {row['id']: row['name'] for row in self.detect.list_tests()}
 
     def my_tests(self):
         account_id = self.build.account.headers['account']
         return {te['id']: te['name'] for te in self.detect.list_tests() if te['account_id'] == account_id}
     
     def convert(self, i: str, reverse=False):
         if reverse:
@@ -96,79 +98,28 @@
 
     @staticmethod
     def normalize(element: str, chars: int):
         element = '' if element is None else element
         return f'{element[:chars - 2]}..' if len(element) > chars else (element or '').ljust(chars, " ")
 
 
-class ViewLogs:
-
-    def __init__(self, wiz: Wizard):
-        self.wiz = wiz
-
-
-    @handle_api_error
-    def enter(self, e: str):
-        while True:
-            try:
-                endpoint_id = e.split(' ')[0]
-                filters = self.wiz.filters.copy()
-                filters['endpoints'] = endpoint_id
-                logs = self.wiz.detect.describe_activity(view='logs', filters=filters)
-                print(f'> {endpoint_id} has {len(logs)} results over the last 30 days')
-
-                menu = OrderedDict()
-                for log in logs:
-                    entry = f'{self.wiz.normalize(log["date"], 30)} {self.wiz.normalize(ExitCode(log["status"]).name, 15)} {self.wiz.convert(log["test"])}'
-                    menu[entry] = None
-                TerminalMenu(menu.keys()).show()
-                break
-            except Exception:
-                break
-
-
-class ListProbes:
-
-    def __init__(self, wiz: Wizard):
-        self.wiz = wiz
-
-    @handle_api_error
-    def enter(self):
-        my_probes = self.wiz.detect.describe_activity(view='probes', filters=self.wiz.filters)
-        states = {x['state'] for x in my_probes}
-        dos = {x['dos'] for x in my_probes}
-        tags = {tag for x in my_probes for tag in x['tags']}
-        print(f'Last 30 days: {len(my_probes)} probes in {len(states)} states, across {len(dos)} operating systems, with {len(tags)} tags')
-
-        menu = OrderedDict()
-        legend = f'{self.wiz.normalize("endpoint_id", 20)} {self.wiz.normalize("os", 15)} {self.wiz.normalize("state", 15)} tags'
-        menu[legend] = None
-        for probe in my_probes:
-            entry = f'{self.wiz.normalize(probe["endpoint_id"], 20)} {self.wiz.normalize(probe["dos"], 15)} {self.wiz.normalize(probe["state"], 15)} {",".join(probe["tags"])}'
-            menu[entry] = ViewLogs
-
-        while True:
-            try:
-                index = TerminalMenu(menu.keys()).show()
-                answer = list(menu.items())
-                answer[index][1](self.wiz).enter(e=answer[index][0])
-            except Exception:
-                break
-
-
 class DeployProbe:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         # register endpoint
-        host = Prompt.ask("Enter hostname of your probe:", default=socket.gethostname())
-        serial = Prompt.ask("Enter serial number of your probe:", default='1-2-3-4')
-        edr = Prompt.ask("[Optional] Enter edr_id of your endpoint:", default='')
+        default = socket.gethostname()
+        host = input(f'Enter hostname of your probe [{default}]: ') or default
+
+        default = '1-2-3-4'
+        serial = input(f'Enter serial number of your probe [{default}]: ') or default
+
+        edr = input(f'[Optional] Enter edr_id of your endpoint: ')
 
         print(f'Optionally, select a host type tag')
         systems = ['workstation', 'server', 'container', 'cloud']
         menu = TerminalMenu(
             systems,
             multi_select=True,
             show_multi_select_hint=True,
@@ -219,22 +170,32 @@
 
 class DeleteProbe:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
-        my_probes = [entry['endpoint_id'] for entry in self.wiz.detect.list_endpoints()]
-        print(f'You have {len(my_probes)} registered probes')
-        menu = TerminalMenu(my_probes, multi_select=True, show_multi_select_hint=True)
-        menu.show()
+        probes = self.wiz.detect.list_endpoints()
+        print(f'You have {len(probes)} registered probes')
+
+        menu = OrderedDict()
+        for p in probes:
+            entry = f'{self.wiz.normalize(p["host"], 50)} {self.wiz.normalize(p["endpoint_id"], 36)}'
+            menu[entry] = None
+        indexes = TerminalMenu(
+            menu,
+            multi_select=True,
+            show_multi_select_hint=True,
+            multi_select_select_on_accept=False,
+            multi_select_empty_ok=True
+        ).show()
 
-        for ep in menu.chosen_menu_entries:
-            print(f'Deleting "{ep}"')
-            self.wiz.detect.delete_endpoint(ident=ep)
+        for i in indexes:
+            self.wiz.detect.delete_endpoint(ident=probes[i]['endpoint_id'])
+            print(f'Deleted "{probes[i]["host"]}" ({probes[i]["endpoint_id"]})')
 
 
 class Probes:
 
     SPLASH="""
 ```bash
 # My name is Nocturnal and I am the Detect probe for Linux and MacOS
@@ -250,19 +211,18 @@
 
     def __init__(self, wiz: Wizard, title: str):
         self.wiz = wiz
         self.title = title
 
     @handle_api_error
     def enter(self):
-        self.wiz.splash(self.SPLASH, helper='Probes are 1 KB processes that run on endpoints and execute security tests')
+        self.wiz.splash(self.SPLASH, "PROBES", helper='Probes are 1 KB processes that run on endpoints and execute security tests')
 
         menu = OrderedDict()
         menu['Register new probe'] = DeployProbe
-        menu['View probe results'] = ListProbes
         menu['Delete existing probe'] = DeleteProbe
 
         while True:
             try:
                 index = TerminalMenu(menu.keys(), title=self.title).show()
                 answer = list(menu.items())
                 answer[index][1](self.wiz).enter()
@@ -274,24 +234,24 @@
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         menu = OrderedDict()
         queue = self.wiz.detect.list_queue()
-        print(f'You have {len(queue)} schedules')
+        print(f'You have {len(queue)} tests scheduled')
         legend = f'{self.wiz.normalize("schedule", 10)} {self.wiz.normalize("tag", 10)} {self.wiz.normalize("started", 15)} {"test"}'
         menu[legend] = None
         for item in queue:
             entry = f'{self.wiz.normalize(RunCode(item["run_code"]).name, 10)} {self.wiz.normalize(item.get("tag"), 10)} {self.wiz.normalize(item["started"], 15)} {self.wiz.convert(item["test"])}'
             menu[entry] = None
         TerminalMenu(menu.keys()).show()
 
 
-class AddSchedule:
+class ScheduleTest:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         print('Select tests to schedule')
         menu = TerminalMenu(
@@ -301,15 +261,15 @@
             multi_select_select_on_accept=False,
             multi_select_empty_ok=True
         )
         menu.show()
         tests = {self.wiz.convert(i, reverse=True): i for i in list(menu.chosen_menu_entries)}
 
         print('How often do you want to run these tests?')
-        menu = [RunCode.DAILY.name, RunCode.WEEKLY.name, RunCode.MONTHLY.name]
+        menu = [r.name for r in RunCode if r != RunCode.INVALID]
         index = TerminalMenu(menu, multi_select=False).show()
         run_code = RunCode[menu[index]].value
 
         menu = TerminalMenu(
             {tag for probe in self.wiz.detect.list_endpoints() for tag in probe['tags']},
             skip_empty_entries=True,
             multi_select=True,
@@ -318,36 +278,38 @@
             multi_select_empty_ok=True
         )
         print('Apply this schedule to specific probe tags?')
         menu.show()
         tags = ",".join(menu.chosen_menu_entries or [])
 
         for test_id in tests:
-            print(f'Adding schedule for {tests[test_id]}')
+            print(f'Test [{tests[test_id]}] has been scheduled')
             self.wiz.detect.enable_test(ident=test_id, run_code=run_code, tags=tags)
         print('Probes check in every few hours to retrieve their scheduled tests')
 
 
-class DeleteSchedule:
+class DescheduleTest:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
-        menu = TerminalMenu(
-            [self.wiz.convert(entry['test']) for entry in self.wiz.detect.list_queue()],
+        queue = self.wiz.detect.list_queue()
+        menu = [f'{self.wiz.normalize(self.wiz.convert(q["test"]), 50)} tag: {self.wiz.normalize(q["tag"], 20)}' for q in queue]
+        indexes = TerminalMenu(
+            menu,
             multi_select=True,
             show_multi_select_hint=True,
-        )
-        menu.show()
+            multi_select_select_on_accept=False,
+            multi_select_empty_ok=True
+        ).show()
 
-        tests = {self.wiz.convert(i, reverse=True): i for i in list(menu.chosen_menu_entries)}
-        for test_id in tests:
-            print(f'Removing schedule for {tests[test_id]}')
-            self.wiz.detect.disable_test(ident=test_id)
+        for i in indexes:
+            self.wiz.detect.disable_test(ident=queue[i]['test'], tags=queue[i]['tag'])
+            print(f'Test has been descheduled: [{menu[i]}]')
 
 
 class Schedule:
 
     SPLASH="""
 ```python
 class RunCode(Enum):
@@ -359,83 +321,38 @@
 
     def __init__(self, wiz: Wizard, title: str):
         self.wiz = wiz
         self.title = title
 
     @handle_api_error
     def enter(self):
-        self.wiz.splash(self.SPLASH, helper='Verified Security Tests are designed to run continuously')
+        self.wiz.splash(self.SPLASH, "SCHEDULING", helper='Verified Security Tests are designed to run continuously')
 
         menu = OrderedDict()
         menu['View schedule'] = ViewSchedule
-        menu['Add schedule'] = AddSchedule
-        menu['Remove schedule'] = DeleteSchedule
+        menu['Schedule test'] = ScheduleTest
+        menu['Deschedule test'] = DescheduleTest
 
         while True:
             try:
                 index = TerminalMenu(menu.keys(), title=self.title).show()
                 answer = list(menu.items())
                 answer[index][1](self.wiz).enter()
             except Exception:
                 break
 
 
-class FiltersView:
-
-    def __init__(self, wiz: Wizard):
-        self.wiz = wiz
-
-    def process(self, filters):
-        my_endpoints = self.wiz.detect.describe_activity(view='probes', filters=self.wiz.filters)
-
-        print('Filter results by probe tags?')
-        menu = TerminalMenu(
-            {tag for probe in my_endpoints for tag in probe['tags']},
-            multi_select=True,
-            show_multi_select_hint=True,
-            multi_select_select_on_accept=False,
-            multi_select_empty_ok=True
-        )
-        menu.show()
-        if menu.chosen_menu_entries:
-            filters['tags'] = ",".join(menu.chosen_menu_entries)
-
-        print('Filter results by operating system?')
-        menu = TerminalMenu(
-            {probe['dos'] for probe in my_endpoints},
-            multi_select=True,
-            show_multi_select_hint=True,
-            multi_select_select_on_accept=False,
-            multi_select_empty_ok=True
-        )
-        menu.show()
-        if menu.chosen_menu_entries:
-            filters['dos'] = ",".join(menu.chosen_menu_entries)
-
-        print('Filter results by tests?')
-        menu = TerminalMenu(
-            self.wiz.tests.values(),
-            multi_select=True,
-            show_multi_select_hint=True,
-            multi_select_select_on_accept=False,
-            multi_select_empty_ok=True
-        )
-        menu.show()
-        if menu.chosen_menu_entries:
-            filters['tests'] = ",".join([self.wiz.convert(i, reverse=True) for i in menu.chosen_menu_entries])
-
-
 class ViewDays:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         filters = self.wiz.filters.copy()
-        FiltersView(self.wiz).process(filters)
+        filters['start'] = datetime.combine(datetime.utcnow() - timedelta(days=14), time.min),
 
         days = self.wiz.detect.describe_activity(view='days', filters=filters)
         days.reverse()
 
         menu = OrderedDict()
         legend = f'{self.wiz.normalize("date", 15)} {self.wiz.normalize("failed", 15)} {self.wiz.normalize("endpoints", 15)}'
         menu[legend] = None
@@ -448,24 +365,25 @@
 class ViewRules:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         print(Padding('Detect classifies tests under rules, which analyze the surface area of operating systems', 1))
-        rules = self.wiz.detect.describe_activity(view='rules', filters=self.wiz.filters)
+        rules = self.wiz.detect.describe_activity(view='rules', filters=self.wiz.filters.copy())
 
         menu = OrderedDict()
         legend = f'{self.wiz.normalize("rule", 35)} {self.wiz.normalize("failed", 15)} {self.wiz.normalize("endpoints", 15)}'
         menu[legend] = None
         for item in rules:
             rule = item.get('rule')
             usage = item.get('usage')
-            entry = f'{self.wiz.normalize(rule["label"], 35)} {self.wiz.normalize(str(usage["failed"]), 15)} {self.wiz.normalize(str(usage["count"]), 15)}'
-            menu[entry] = None
+            if usage:
+                entry = f'{self.wiz.normalize(rule["label"], 35)} {self.wiz.normalize(str(usage["failed"]), 15)} {self.wiz.normalize(str(usage["count"]), 15)}'
+                menu[entry] = None
         TerminalMenu(menu.keys()).show()
 
 
 class ViewInsights:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
@@ -473,15 +391,15 @@
     def enter(self):
         print(Padding('A computer generated insight exposes the most vulnerable combinations of test and OS', 1))
         insights = self.wiz.detect.describe_activity(view='insights', filters=self.wiz.filters)
 
         menu = OrderedDict()
         legend = f'{self.wiz.normalize("unprotected", 15)} {self.wiz.normalize("protected", 15)} {self.wiz.normalize("dos", 15)} {"test"}'
         menu[legend] = None
-        for item in insights:
+        for item in insights[:10]:
             vol = item['volume']
             if vol['unprotected']:
                 entry = f'{self.wiz.normalize(str(vol["unprotected"]), 15)} {self.wiz.normalize(str(vol["protected"]), 15)} {self.wiz.normalize(item["dos"], 15)} {self.wiz.convert(item["test"])}'
                 menu[entry] = None
         TerminalMenu(menu.keys()).show()
 
 
@@ -492,22 +410,43 @@
 
     def enter(self):
         print(Padding('The Prelude team provides manual security recommendations for licensed accounts', 1))
         menu = OrderedDict()
         recommendations = self.wiz.detect.recommendations()
 
         if recommendations:
+            legend = f'{self.wiz.normalize("created", 15)} {self.wiz.normalize("user", 20)} {self.wiz.normalize("title", 40)} {"description"}'
+            menu[legend] = None
             for item in recommendations:
-                entry = f'{self.wiz.normalize(item["created"], 15)} {self.wiz.normalize(item["handle"], 20)} {self.wiz.normalize(item["title"], 50)} {item["description"]}'
-                menu[entry] = None
-            TerminalMenu(menu.keys()).show()
+                entry = f'{self.wiz.normalize(item["created"], 15)} {self.wiz.normalize(item["handle"], 20)} {self.wiz.normalize(item["title"], 40)} {item["description"]}'
+                menu[entry] = item
+            index = TerminalMenu(menu.keys()).show()
+
+            answer = list(menu.items())
+            AddDecision(self.wiz, answer[index][1]).enter()
+
         else:
             print('No recommendations are available')
 
 
+class AddDecision:
+
+    def __init__(self, wiz: Wizard, rec: dict):
+        self.wiz = wiz
+        self.rec = rec
+
+    def enter(self):
+        decision = Decision(self.rec['events'][0]['decision']).name if self.rec['events'] else "None"
+        print(f'Title: {self.rec["title"]}\nDecision: {decision}\nDescription: {self.rec["description"]}')
+
+        menu = ['cancel', 'approve', 'deny']
+        index = TerminalMenu(menu).show()
+        if index:
+            self.wiz.detect.make_decision(id=self.rec['id'], decision=Decision[menu[index].upper()].value)
+
 class Results:
 
     SPLASH="""
 ```python
 PROTECTED = 100
 UNPROTECTED = 101
 TIMEOUT = 102
@@ -521,19 +460,20 @@
 
     def __init__(self, wiz: Wizard, title: str):
         self.wiz = wiz
         self.title = title
 
     @handle_api_error
     def enter(self):
-        self.wiz.splash(self.SPLASH, helper='Detect records a code for each executed test to explain what happened')
+        self.wiz.splash(self.SPLASH, "RESULTS", helper='Detect records a code for each executed test to explain what happened')
 
         menu = OrderedDict()
-        menu['Results by day'] = ViewDays
-        menu['Results by rule'] = ViewRules
+        menu['Full results: open executive dashboard'] = ExecutiveDashboard
+        menu['Summary: results by day'] = ViewDays
+        menu['Summary: results by rule'] = ViewRules
         menu['Computer insights'] = ViewInsights
         menu['Human recommendations'] = ViewRecommendations
 
         while True:
             try:
                 index = TerminalMenu(menu.keys(), title=self.title).show()
                 answer = list(menu.items())
@@ -575,21 +515,23 @@
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         print('Tests should be in the form of a question')
         # save test
-        name = Prompt.ask('Enter a test name', default='Does my defense work?')
+        default = 'Does my defense work?'
+        name = input(f'Enter a test name [{default}]: ') or default
         test_id = str(uuid.uuid4())
         self.wiz.build.create_test(test_id=test_id, name=name)
 
         mapping = Confirm.ask('Add a classification, such as a rule, CVE or ATT&CK technique?')
         if mapping:
-            value = Prompt.ask('Enter a classification ID', default='VSR-2023-0')
+            default = 'VSR-2023-0'
+            value = input(f'Enter a classification ID [{default}]: ') or default
             self.wiz.build.map(test_id=test_id, x=value.replace(' ', ''))
 
         # construct test file
         basename = f'{test_id}.go'
         template = pkg_resources.read_text(templates, 'template.go')
         template = template.replace('$ID', test_id)
         template = template.replace('$NAME', name)
@@ -677,15 +619,15 @@
 
     def __init__(self, wiz: Wizard, title: str):
         self.wiz = wiz
         self.title = title
 
     @handle_api_error
     def enter(self):
-        self.wiz.splash(self.SPLASH, helper='Verified Security Tests (VST) are production-ready TTPs written in Go')
+        self.wiz.splash(self.SPLASH, "BUILD", helper='Verified Security Tests (VST) are production-ready TTPs written in Go')
 
         menu = OrderedDict()
         menu['Create new test'] = CreateTest
         menu['Upload test'] = UploadTest
         menu['Download test'] = DownloadTests
         menu['Delete test'] = DeleteTest
 
@@ -720,21 +662,22 @@
 class CreateUser:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         print('All users share an account ID but have unique access tokens')
-        handle = Prompt.ask('Enter a user handle', default=os.getlogin())
+        default = 'test@email.com'
+        handle = input(f'Enter a user handle. All handles, except for those with SERVICE permissions, must be valid email addresses [{default}]: ') or default
         menu = [p.name for p in Permission if p != Permission.INVALID]
         answer = TerminalMenu(menu).show()
         expires = datetime.utcnow() + timedelta(days=365)
 
         creds = self.wiz.iam.create_user(handle=handle, permission=answer, expires=expires)
-        print(f'Created "{handle}" with token "{creds["token"]}"')
+        print(f'Created "{handle}" with token "{creds["token"]}". New users will receive an email to complete verification.')
 
 
 class DeleteUser:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
@@ -748,66 +691,68 @@
         menu.show()
 
         for handle in menu.chosen_menu_entries:
             print(f'Deleting "{handle}"')
             self.wiz.iam.delete_user(handle=handle)
 
 
-class ListControls:
+class ListPartners:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         account = self.wiz.iam.get_account()
         menu = OrderedDict()
-        legend = f'{self.wiz.normalize("name", 20)} {self.wiz.normalize("apî", 40)} {self.wiz.normalize("username", 10)} {self.wiz.normalize("secret", 10)}'
+        legend = f'{self.wiz.normalize("name", 20)}'
         menu[legend] = None
-        for control in account['controls']:
-            name = control['name']
-            api = control['api']
-            username = control['username']
-            secret = control['secret']
-            entry = f'{self.wiz.normalize(name, 20)} {self.wiz.normalize(api, 40)} {self.wiz.normalize(username, 10)} {self.wiz.normalize(secret, 10)} '
+        for name in account['controls']:
+            entry = f'{self.wiz.normalize(name, 20)}'
             menu[entry] = None
         TerminalMenu(menu.keys()).show()
 
 
 class AttachPartner:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         print('Learn about integrations: https://docs.preludesecurity.com/docs/defensive-integrations')
         menu = ['crowdstrike']
         answer = TerminalMenu(menu).show()
-
         name = menu[answer]
-        api = Prompt.ask('API FQDN', default='https://api.us-2.crowdstrike.com')
-        user = Prompt.ask('User or client ID', default=os.getlogin())
-        secret = Prompt.ask('API token', default='password123')
+
+        default = 'https://api.us-2.crowdstrike.com'
+        api = input(f'API FQDN [{default}]: ') or default
+
+        default = os.getlogin()
+        user = input(f'User or client ID [{default}]: ') or default
+
+        default = 'password123'
+        secret = input(f'API token [{default}]: ') or default
+
         print(f'Attaching "{name}" to your account')
         self.wiz.iam.attach_partner(name=name, api=api, user=user, secret=secret)
 
 
 class DetachPartner:
 
     def __init__(self, wiz: Wizard):
         self.wiz = wiz
 
     def enter(self):
         account = self.wiz.iam.get_account()
-        controls = [ctrl['name'] for ctrl in account['controls']]
+        partners = account['controls']
 
-        if not controls:
-            print('No controls exist for this account')
+        if not partners:
+            print('No partners exist for this account')
             return
 
-        menu = TerminalMenu(controls, multi_select=True, show_multi_select_hint=True)
+        menu = TerminalMenu(partners, multi_select=True, show_multi_select_hint=True)
         menu.show()
 
         for name in menu.chosen_menu_entries:
             print(f'Detaching "{name}" from your account')
             self.wiz.iam.detach_partner(name=name)
 
 
@@ -842,80 +787,81 @@
 
     def __init__(self, wiz: Wizard, title: str):
         self.wiz = wiz
         self.title = title
 
     @handle_api_error
     def enter(self):
-        self.wiz.splash(self.SPLASH, helper='Prelude accounts can contain multiple users with different permissions')
+        self.wiz.splash(self.SPLASH, "IAM", helper='Prelude accounts can contain multiple users with different permissions')
 
         menu = OrderedDict()
         menu['List users'] = ListUser
         menu['Create user'] = CreateUser
         menu['Delete user'] = DeleteUser
-        menu['List integrations'] = ListControls
-        menu['Attach integration'] = AttachPartner
-        menu['Detach integration'] = DetachPartner
+        menu['List partners'] = ListPartners
+        menu['Attach partner'] = AttachPartner
+        menu['Detach partner'] = DetachPartner
         menu['Delete account'] = DeleteAccount
 
         while True:
             try:
                 index = TerminalMenu(menu.keys(), title=self.title).show()
                 answer = list(menu.items())
                 answer[index][1](self.wiz).enter()
             except Exception:
                 break
 
 
 class ExecutiveDashboard:
 
-    def __init__(self, wiz: Wizard, title: str):
+    def __init__(self, wiz: Wizard, title: str = ''):
         self.wiz = wiz
         self.title = title
 
     def enter(self):
         account = self.wiz.detect.account.headers['account']
         token = self.wiz.detect.account.headers['token']
         webbrowser.open(f'{self.wiz.detect.account.hq}/iam/user?account={account}&token={token}', new=2)
 
 
 @click.command()
 @click.pass_obj
 def interactive(account):
     """ Interactive shell for Prelude Detect """
     wizard = Wizard(account=account)
-    wizard.splash(HELLO)
+    wizard.splash(HELLO, "WELCOME")
     wizard.load_tests()
     print(Padding(f'Your account has access to {len(wizard.tests)} Verified Security Tests', 1))
 
     menu = OrderedDict()
     wizard.add_menu(menu, 'Deploy probes', Probes)
     wizard.add_menu(menu, 'Schedule tests', Schedule)
     wizard.add_menu(menu, 'View results', Results)
     wizard.add_menu(menu, 'Developer hub', Build)
     wizard.add_menu(menu, 'Manage account', IAM)
     wizard.add_menu(menu, 'Open executive dashboard', ExecutiveDashboard)
 
     while True:
         try:
             if not wizard.tests:
-                raise PermissionError('No local keychain found. Would you like to create a Prelude account?')
+                raise PermissionError('Account not found. Would you like to create a Prelude account?')
             
             index = TerminalMenu(menu.keys()).show()
             answer = list(menu.items())
             answer[index][1].enter()
         except TypeError:
             print(Padding('Goodbye. May Verified Security Tests be with you.', 1))
             break
         except PermissionError as pe:
             yes = Confirm.ask(str(pe))
             if not yes:
                 break
 
-            email = Prompt.ask('Enter your email handle')
+            default = 'test@email.com'
+            email = input(f'Enter your email handle [{default}]: ') or default
             wizard.iam.new_account(handle=email)
             keychain = PurePath(Path.home(), '.prelude', 'keychain.ini')
             print(f'Account created! Credentials are stored in your keychain: {keychain}')
             print('Check your email to verify your account, then restart the wizard to continue.')
             break
         except Exception as ex:
             wizard.console.print(str(ex), style='red')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prelude-cli-0.9.97/prelude_cli/views/partner.py` & `prelude-cli-1.0.0/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.97/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.0.0/prelude_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 0.9.97
+Version: 1.0.0
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-0.9.97/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.0.0/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-0.9.97/setup.cfg` & `prelude-cli-1.0.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 0.9.97
+version = 1.0.0
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,18 +13,19 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 0.9.97
+	prelude-sdk == 1.0.0
 	click
 	rich
 	simple-term-menu
+	gnureadline
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
 
 [egg_info]
 tag_build =
```

