# Comparing `tmp/skyagi-0.0.2.tar.gz` & `tmp/skyagi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyagi-0.0.2.tar", last modified: Mon Apr 17 02:58:08 2023, max compression
+gzip compressed data, was "skyagi-0.0.3.tar", last modified: Mon Apr 17 22:47:57 2023, max compression
```

## Comparing `skyagi-0.0.2.tar` & `skyagi-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 02:58:08.695374 skyagi-0.0.2/
--rw-r--r--   0 tanl       (501) staff       (20)       54 2023-04-17 02:48:47.000000 skyagi-0.0.2/.gitignore
--rw-r--r--   0 tanl       (501) staff       (20)      303 2023-04-17 00:22:26.000000 skyagi-0.0.2/Makefile
--rw-r--r--   0 tanl       (501) staff       (20)      540 2023-04-17 02:58:08.695516 skyagi-0.0.2/PKG-INFO
--rw-r--r--   0 tanl       (501) staff       (20)       10 2023-04-17 00:11:44.000000 skyagi-0.0.2/README.md
--rw-r--r--   0 tanl       (501) staff       (20)      137 2023-04-17 02:55:54.000000 skyagi-0.0.2/pyproject.toml
-drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 02:58:08.692375 skyagi-0.0.2/scripts/
--rw-r--r--   0 tanl       (501) staff       (20)     2239 2023-04-17 00:17:41.000000 skyagi-0.0.2/scripts/format-staged-files.sh
--rwxr-xr-x   0 tanl       (501) staff       (20)      703 2023-04-17 00:21:20.000000 skyagi-0.0.2/scripts/pre-commit
--rwxr-xr-x   0 tanl       (501) staff       (20)      378 2023-04-17 00:22:38.000000 skyagi-0.0.2/scripts/pre-push
--rw-r--r--   0 tanl       (501) staff       (20)     1043 2023-04-17 02:58:08.695905 skyagi-0.0.2/setup.cfg
-drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 02:58:08.690752 skyagi-0.0.2/src/
-drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 02:58:08.693901 skyagi-0.0.2/src/skyagi/
--rw-r--r--   0 tanl       (501) staff       (20)       38 2023-04-17 01:04:20.000000 skyagi-0.0.2/src/skyagi/__init__.py
-drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 02:58:08.695271 skyagi-0.0.2/src/skyagi/agent/
--rw-r--r--   0 tanl       (501) staff       (20)       15 2023-04-17 01:11:47.000000 skyagi-0.0.2/src/skyagi/agent/README.md
--rw-r--r--   0 tanl       (501) staff       (20)        0 2023-04-17 01:11:47.000000 skyagi-0.0.2/src/skyagi/agent/__init__.py
--rw-r--r--   0 tanl       (501) staff       (20)        0 2023-04-17 01:11:47.000000 skyagi-0.0.2/src/skyagi/agent/agent.py
--rw-r--r--   0 tanl       (501) staff       (20)     2535 2023-04-17 02:40:04.000000 skyagi-0.0.2/src/skyagi/cli.py
--rw-r--r--   0 tanl       (501) staff       (20)     1094 2023-04-17 02:40:04.000000 skyagi-0.0.2/src/skyagi/config.py
--rw-r--r--   0 tanl       (501) staff       (20)        0 2023-04-17 01:04:20.000000 skyagi-0.0.2/src/skyagi/skyagi.py
--rw-r--r--   0 tanl       (501) staff       (20)        0 2023-04-17 02:40:04.000000 skyagi-0.0.2/src/skyagi/tui.py
--rw-r--r--   0 tanl       (501) staff       (20)     1535 2023-04-17 02:40:04.000000 skyagi-0.0.2/src/skyagi/util.py
-drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 02:58:08.694773 skyagi-0.0.2/src/skyagi.egg-info/
--rw-r--r--   0 tanl       (501) staff       (20)      540 2023-04-17 02:58:08.000000 skyagi-0.0.2/src/skyagi.egg-info/PKG-INFO
--rw-r--r--   0 tanl       (501) staff       (20)      529 2023-04-17 02:58:08.000000 skyagi-0.0.2/src/skyagi.egg-info/SOURCES.txt
--rw-r--r--   0 tanl       (501) staff       (20)        1 2023-04-17 02:58:08.000000 skyagi-0.0.2/src/skyagi.egg-info/dependency_links.txt
--rw-r--r--   0 tanl       (501) staff       (20)       38 2023-04-17 02:58:08.000000 skyagi-0.0.2/src/skyagi.egg-info/entry_points.txt
--rw-r--r--   0 tanl       (501) staff       (20)      260 2023-04-17 02:58:08.000000 skyagi-0.0.2/src/skyagi.egg-info/requires.txt
--rw-r--r--   0 tanl       (501) staff       (20)        7 2023-04-17 02:58:08.000000 skyagi-0.0.2/src/skyagi.egg-info/top_level.txt
+drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 22:47:57.902488 skyagi-0.0.3/
+drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 22:47:57.896663 skyagi-0.0.3/.github/
+drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 22:47:57.898422 skyagi-0.0.3/.github/scripts/
+-rw-r--r--   0 tanl       (501) staff       (20)     1398 2023-04-17 04:33:53.000000 skyagi-0.0.3/.github/scripts/release.py
+drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 22:47:57.899034 skyagi-0.0.3/.github/workflows/
+-rw-r--r--   0 tanl       (501) staff       (20)      581 2023-04-17 04:33:53.000000 skyagi-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 tanl       (501) staff       (20)      341 2023-04-17 04:33:53.000000 skyagi-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0 tanl       (501) staff       (20)       54 2023-04-17 04:33:53.000000 skyagi-0.0.3/.gitignore
+-rw-r--r--   0 tanl       (501) staff       (20)       16 2023-04-17 08:23:06.000000 skyagi-0.0.3/CODEOWNERS
+-rw-r--r--   0 tanl       (501) staff       (20)      303 2023-04-17 00:22:26.000000 skyagi-0.0.3/Makefile
+-rw-r--r--   0 tanl       (501) staff       (20)      557 2023-04-17 22:47:57.902593 skyagi-0.0.3/PKG-INFO
+-rw-r--r--   0 tanl       (501) staff       (20)       27 2023-04-17 17:27:24.000000 skyagi-0.0.3/README.md
+-rw-r--r--   0 tanl       (501) staff       (20)      137 2023-04-17 22:46:04.000000 skyagi-0.0.3/pyproject.toml
+drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 22:47:57.900064 skyagi-0.0.3/scripts/
+-rw-r--r--   0 tanl       (501) staff       (20)     2239 2023-04-17 00:17:41.000000 skyagi-0.0.3/scripts/format-staged-files.sh
+-rwxr-xr-x   0 tanl       (501) staff       (20)      703 2023-04-17 00:21:20.000000 skyagi-0.0.3/scripts/pre-commit
+-rwxr-xr-x   0 tanl       (501) staff       (20)      378 2023-04-17 00:22:38.000000 skyagi-0.0.3/scripts/pre-push
+-rw-r--r--   0 tanl       (501) staff       (20)     1033 2023-04-17 22:47:57.902931 skyagi-0.0.3/setup.cfg
+drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 22:47:57.896920 skyagi-0.0.3/src/
+drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 22:47:57.901275 skyagi-0.0.3/src/skyagi/
+-rw-r--r--   0 tanl       (501) staff       (20)       38 2023-04-17 01:04:20.000000 skyagi-0.0.3/src/skyagi/__init__.py
+-rw-r--r--   0 tanl       (501) staff       (20)     3984 2023-04-17 17:32:30.000000 skyagi-0.0.3/src/skyagi/cli.py
+-rw-r--r--   0 tanl       (501) staff       (20)     1094 2023-04-17 02:40:04.000000 skyagi-0.0.3/src/skyagi/config.py
+-rw-r--r--   0 tanl       (501) staff       (20)     2041 2023-04-17 22:45:39.000000 skyagi-0.0.3/src/skyagi/skyagi.py
+-rw-r--r--   0 tanl       (501) staff       (20)        0 2023-04-17 02:40:04.000000 skyagi-0.0.3/src/skyagi/tui.py
+-rw-r--r--   0 tanl       (501) staff       (20)     1535 2023-04-17 15:32:51.000000 skyagi-0.0.3/src/skyagi/util.py
+drwxr-xr-x   0 tanl       (501) staff       (20)        0 2023-04-17 22:47:57.902345 skyagi-0.0.3/src/skyagi.egg-info/
+-rw-r--r--   0 tanl       (501) staff       (20)      557 2023-04-17 22:47:57.000000 skyagi-0.0.3/src/skyagi.egg-info/PKG-INFO
+-rw-r--r--   0 tanl       (501) staff       (20)      545 2023-04-17 22:47:57.000000 skyagi-0.0.3/src/skyagi.egg-info/SOURCES.txt
+-rw-r--r--   0 tanl       (501) staff       (20)        1 2023-04-17 22:47:57.000000 skyagi-0.0.3/src/skyagi.egg-info/dependency_links.txt
+-rw-r--r--   0 tanl       (501) staff       (20)       38 2023-04-17 22:47:57.000000 skyagi-0.0.3/src/skyagi.egg-info/entry_points.txt
+-rw-r--r--   0 tanl       (501) staff       (20)      251 2023-04-17 22:47:57.000000 skyagi-0.0.3/src/skyagi.egg-info/requires.txt
+-rw-r--r--   0 tanl       (501) staff       (20)        7 2023-04-17 22:47:57.000000 skyagi-0.0.3/src/skyagi.egg-info/top_level.txt
```

### Comparing `skyagi-0.0.2/PKG-INFO` & `skyagi-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: skyagi
-Version: 0.0.2
+Version: 0.0.3
 Summary: AGI
 Home-page: https://github.com/litanlitudan/skyagi
 Author: Tan Li
 Author-email: tan@tanli.dev
 Project-URL: Bug Tracker, https://github.com/litanlitudan/skyagi/issues
 Project-URL: Changelog, https://github.com/litanlitudan/skyagi/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-# sky-agi
+# SkyAGI: Sky is the Limit
```

### Comparing `skyagi-0.0.2/scripts/format-staged-files.sh` & `skyagi-0.0.3/scripts/format-staged-files.sh`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.2/scripts/pre-commit` & `skyagi-0.0.3/scripts/pre-commit`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.2/setup.cfg` & `skyagi-0.0.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = skyagi
-version = 0.0.2
+version = 0.0.3
 author = Tan Li
 author_email = tan@tanli.dev
 description = AGI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/litanlitudan/skyagi
 project_urls = 
@@ -21,21 +21,20 @@
 packages = find:
 python_requires = >=3.8
 install_requires = 
 	beautifulsoup4
 	fastapi
 	html2text
 	markdown
+	networkx
 	psutil
 	rich
-	sentry-sdk
 	textual
 	typer
 	uvicorn[standard]
-	whoosh
 	datasets
 	faiss-cpu
 	openai
 	pinecone-client
 	sacremoses
 	sentence-transformers
 	transformers
```

### Comparing `skyagi-0.0.2/src/skyagi/cli.py` & `skyagi-0.0.3/src/skyagi/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import typer
+import time
 from rich.console import Console
-from rich.prompt import Prompt, Confirm, IntPrompt
+from rich.prompt import Prompt, IntPrompt
 
-from skyagi import config, tui, util
+from skyagi import config, util
+from skyagi.skyagi import Agent, Context, step
 
 cli = typer.Typer()
 console = Console()
 
 #######################################################################################
 # Config CLI
 
@@ -21,28 +23,30 @@
     token = Prompt.ask("Enter your OpenAI API token").strip()
     verify_resp = util.verify_openai_token(token)
     if verify_resp != "OK":
         console.print("[Error] OpenAI Token is invalid", style="red")
         console.print(verify_resp)
         return
     config.set_openai_token(token)
+    console.print("OpenAI Key is Configured Successfully!", style="green")
 
 
 @config_cli.command("pinecone")
 def config_pinecone():
     """
     Configure Pinecone API token
     """
     token = Prompt.ask("Enter your Pinecone API token").strip()
     verify_resp = util.verify_pinecone_token(token)
     if verify_resp != "OK":
         console.print("[Error] Pinecone Token is invalid", style="red")
         console.print(verify_resp)
         return
     config.set_pinecone_token(token)
+    console.print("Pinecone Key is Configured Successfully!", style="green")
 
 
 @config_cli.callback(invoke_without_command=True)
 def config_main(ctx: typer.Context):
     """
     Configure SkyAGI
     """
@@ -73,14 +77,43 @@
 def status():
     """
     Status of the SkyAGI
     """
     console.print("SkyAGI status")
 
 
+@cli.command("run")
+def run():
+    """
+    Run SkyAGI
+    """
+    agent_count = IntPrompt.ask("Number of characters to create?", default=3)
+    agents = []
+    for idx in range(agent_count):
+        console.print(f"Creating character {idx+1}")
+        name = Prompt.ask("What is the character's name?").strip()
+        personality = Prompt.ask("Please use 3~5 words describe the character's personality, [yellow]e.g. confident, creative...[/yellow]")
+        intro = Prompt.ask(f"A brief intro, [yellow]e.g. {name} is a famous singer...[/yellow]")
+        agent = Agent(name, personality, intro, idx==0)
+        agents.append(agent)
+        console.print(f"Successfully created character {name}", style="green")
+        time.sleep(0.5)
+    console.print("SkyAGI starting...")
+    console.print(f"Now, you are going to behave as {agents[0].name}", style="yellow")
+    ctx = Context(console, config.load_openai_token())
+    instruction = ""
+    while True:
+        step(agents, ctx, instruction)
+        console.print("What's your action? Q for quit, Enter for continue", style="yellow")
+        instruction = Prompt.ask().strip()
+        if (instruction == "Q" or instruction == "q"):
+            console.print("Quitting SkyAGI...")
+            break
+
+
 @cli.callback(invoke_without_command=True)
 def main(
     ctx: typer.Context,
 ):
     """
     Default behavior
     """
```

### Comparing `skyagi-0.0.2/src/skyagi/config.py` & `skyagi-0.0.3/src/skyagi/config.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.2/src/skyagi/util.py` & `skyagi-0.0.3/src/skyagi/util.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.2/src/skyagi.egg-info/PKG-INFO` & `skyagi-0.0.3/src/skyagi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: skyagi
-Version: 0.0.2
+Version: 0.0.3
 Summary: AGI
 Home-page: https://github.com/litanlitudan/skyagi
 Author: Tan Li
 Author-email: tan@tanli.dev
 Project-URL: Bug Tracker, https://github.com/litanlitudan/skyagi/issues
 Project-URL: Changelog, https://github.com/litanlitudan/skyagi/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
-# sky-agi
+# SkyAGI: Sky is the Limit
```

