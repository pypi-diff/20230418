# Comparing `tmp/pipen_board-0.0.5.tar.gz` & `tmp/pipen_board-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_board-0.0.5.tar", max compression
+gzip compressed data, was "pipen_board-0.0.6.tar", max compression
```

## Comparing `pipen_board-0.0.5.tar` & `pipen_board-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1780 2023-04-18 03:46:49.609347 pipen_board-0.0.5/README.md
--rw-r--r--   0        0        0      348 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/__init__.py
--rw-r--r--   0        0        0     7170 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/apis.py
--rw-r--r--   0        0        0     4081 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/cli.py
--rw-r--r--   0        0        0    21706 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/data_manager.py
--rw-r--r--   0        0        0     5895 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/defaults.py
--rw-r--r--   0        0        0    23628 2023-04-18 03:46:49.609347 pipen_board-0.0.5/pipen_board/frontend/build/assets/favicon.png
--rw-r--r--   0        0        0   621271 2023-04-18 03:46:49.613347 pipen_board-0.0.5/pipen_board/frontend/build/assets/index.css
--rw-r--r--   0        0        0   723656 2023-04-18 03:46:49.617347 pipen_board-0.0.5/pipen_board/frontend/build/assets/index.js
--rw-r--r--   0        0        0     4128 2023-04-18 03:46:49.617347 pipen_board-0.0.5/pipen_board/frontend/build/assets/schema.json
--rw-r--r--   0        0        0      406 2023-04-18 03:46:49.617347 pipen_board-0.0.5/pipen_board/frontend/build/index.html
--rw-r--r--   0        0        0     7488 2023-04-18 03:46:49.621347 pipen_board-0.0.5/pipen_board/plugin.py
--rw-r--r--   0        0        0     3341 2023-04-18 03:46:49.621347 pipen_board-0.0.5/pipen_board/quart_app.py
--rw-r--r--   0        0        0      766 2023-04-18 03:46:49.621347 pipen_board-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 pipen_board-0.0.5/setup.py
--rw-r--r--   0        0        0     2628 1970-01-01 00:00:00.000000 pipen_board-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1780 2023-04-18 06:52:37.703848 pipen_board-0.0.6/README.md
+-rw-r--r--   0        0        0      348 2023-04-18 06:52:37.703848 pipen_board-0.0.6/pipen_board/__init__.py
+-rw-r--r--   0        0        0     7513 2023-04-18 06:52:37.703848 pipen_board-0.0.6/pipen_board/apis.py
+-rw-r--r--   0        0        0     4134 2023-04-18 06:52:37.703848 pipen_board-0.0.6/pipen_board/cli.py
+-rw-r--r--   0        0        0    22001 2023-04-18 06:52:37.707848 pipen_board-0.0.6/pipen_board/data_manager.py
+-rw-r--r--   0        0        0     5895 2023-04-18 06:52:37.707848 pipen_board-0.0.6/pipen_board/defaults.py
+-rw-r--r--   0        0        0    23628 2023-04-18 06:52:37.707848 pipen_board-0.0.6/pipen_board/frontend/build/assets/favicon.png
+-rw-r--r--   0        0        0   621271 2023-04-18 06:52:37.707848 pipen_board-0.0.6/pipen_board/frontend/build/assets/index.css
+-rw-r--r--   0        0        0   723656 2023-04-18 06:52:37.711848 pipen_board-0.0.6/pipen_board/frontend/build/assets/index.js
+-rw-r--r--   0        0        0     4128 2023-04-18 06:52:37.711848 pipen_board-0.0.6/pipen_board/frontend/build/assets/schema.json
+-rw-r--r--   0        0        0      406 2023-04-18 06:52:37.711848 pipen_board-0.0.6/pipen_board/frontend/build/index.html
+-rw-r--r--   0        0        0     7488 2023-04-18 06:52:37.715848 pipen_board-0.0.6/pipen_board/plugin.py
+-rw-r--r--   0        0        0     3393 2023-04-18 06:52:37.715848 pipen_board-0.0.6/pipen_board/quart_app.py
+-rw-r--r--   0        0        0      727 2023-04-18 06:52:37.715848 pipen_board-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pipen_board-0.0.6/setup.py
+-rw-r--r--   0        0        0     2550 1970-01-01 00:00:00.000000 pipen_board-0.0.6/PKG-INFO
```

### Comparing `pipen_board-0.0.5/README.md` & `pipen_board-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.5/pipen_board/apis.py` & `pipen_board-0.0.6/pipen_board/apis.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     """Redirect to the index.html"""
     if request.cli_args.dev:
         return redirect('index.html?dev=1')
     return redirect('index.html')
 
 
 async def history():
-    logger.info("API Getting histories")
+    logger.info("[bold][yellow]API[/yellow][/bold] Getting histories")
     args = request.cli_args
     out = {}
     out["pipeline"] = args.pipeline
     out["histories"] = []
 
     for histfile in PIPEN_BOARD_DIR.glob(
         f"{slugify(args.pipeline)}.{args.name}.*.json"
@@ -87,21 +87,24 @@
         })
 
     return out
 
 
 async def history_del():
     configfile = (await request.get_json())["configfile"]
-    logger.info("API Deleting history: %s", configfile)
+    logger.info(
+        "[bold][yellow]API[/yellow][/bold] Deleting history: %s",
+        configfile,
+    )
     PIPEN_BOARD_DIR.joinpath(configfile).unlink()
     return {"ok": True}
 
 
 async def pipeline_data():
-    logger.info("API Getting pipeline data")
+    logger.info("[bold][yellow]API[/yellow][/bold] Getting pipeline data")
     configfile = (await request.get_json()).get("configfile")
     return data_manager.get_data(request.cli_args, configfile)
 
 
 async def config_save():
     args = request.cli_args
     data = await request.get_json()
@@ -112,28 +115,36 @@
     out = {"name": args.name, "mtime": now}
     if not configfile:
         configfile = PIPEN_BOARD_DIR.joinpath(
             f"{slugify(args.pipeline)}.{args.name}."
             f"{now.replace(' ', '_').replace(':', '-')}.json"
         )
         out["ctime"] = now
-        logger.info(f"API Saving config to a new file: {configfile}")
+        logger.info(
+            "[bold][yellow]API[/yellow][/bold] Saving config to a new file: "
+            f"{configfile}"
+        )
     else:
         configfile = PIPEN_BOARD_DIR.joinpath(configfile)
-        logger.info(f"API Saving config to: {configfile}")
+        logger.info(
+            f"[bold][yellow]API[/yellow][/bold] Saving config to: {configfile}"
+        )
 
     out["configfile"] = configfile.name
     configfile.write_text(configdata)
     return out
 
 
 async def job_get_tree():
     args = request.cli_args
     data = await request.get_json()
-    logger.info(f"API Fetching tree for: {data['proc']}/{data['job']}")
+    logger.info(
+        "[bold][yellow]API[/yellow][/bold] Fetching tree for: "
+        f"{data['proc']}/{data['job']}"
+    )
     jobdir = Path(args.root).joinpath(
         ".pipen",
         args.name,
         data["proc"],
         str(data["job"]),
     )
     if not jobdir.is_dir():
@@ -147,21 +158,21 @@
 async def job_get_file():
     """Get file details"""
     data = await request.get_json()
     how = data.get("how", "full")
     path = Path(data["path"])
     if how != "full":
         logger.info(
-            "API Fetching file for "
+            "[bold][yellow]API[/yellow][/bold] Fetching file for "
             f"{data['proc']}/{data['job']}: {path} ({how})"
         )
         return {"type": "bigtext-part", "content": _get_file_content(path, how)}
 
     logger.info(
-        "API Fetching file for "
+        "[bold][yellow]API[/yellow][/bold] Fetching file for "
         f"{data['proc']}/{data['job']}: {path}"
     )
     if (
         path.name.startswith("job.wrapped.")
         or path.name in ("job.script", "job.signature.toml", "job.rc")
     ):
         return {"type": "text", "content": path.read_text()}
@@ -215,29 +226,29 @@
         and type.startswith("on_")
         and callable(getattr(data_manager, type, None))
     ):
         await getattr(data_manager, type)(data["data"], clients.get("web"))
 
 
 async def ws_web_conn(clients):
-    logger.info(f"WS/WEB Client 'web' connected.")
+    logger.info("WS/WEB Client 'web' connected.")
     # send the current run data, to let UI know the current status
     await data_manager.send_run_data(clients["web"], True)
 
 
 async def ws_pipeline_conn(clients):
-    logger.info(f"WS/PIPELINE Client 'pipeline' connected.")
+    logger.info("WS/PIPELINE Client 'pipeline' connected.")
 
 
 async def ws_web_disconn(clients):
-    logger.info(f"WS/WEB Client 'web' disconnected.")
+    logger.info("WS/WEB Client 'web' disconnected.")
 
 
 async def ws_pipeline_disconn(clients):
-    logger.info(f"WS/PIPELINE Client 'pipeline' disconnected.")
+    logger.info("WS/PIPELINE Client 'pipeline' disconnected.")
     data_manager.running = False
 
 
 GETS = {
     "/": index,
     "/api/history": history,
 }
```

### Comparing `pipen_board-0.0.5/pipen_board/cli.py` & `pipen_board-0.0.6/pipen_board/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,28 +22,31 @@
         self,
         parser: ArgumentParser,
         subparser: ArgumentParser,
     ) -> None:
         super().__init__(parser, subparser)
         subparser.usage = "%(prog)s [options] <pipeline> -- [pipeline options]"
         subparser.add_argument(
+            "-p",
             "--port",
             type=int,
             default=18521,
             help="Port to serve the UI wizard",
         )
         subparser.add_argument(
+            "-n",
             "--name",
             help=(
                 "The name of the pipeline. Default to the pipeline class name. "
                 "You can use a different name to associate with a different "
                 "set of configurations."
             )
         )
         subparser.add_argument(
+            "-a",
             "--additional",
             metavar="FILE",
             help=(
                 "Additional arguments for the pipeline, "
                 "in YAML, INI, JSON or TOML format. "
                 "Can have sections `ADDITIONAL_OPTIONS` and `RUNNING_OPTIONS`"
             ),
@@ -86,15 +89,15 @@
     def parse_args(self) -> Namespace:
         """Parse the arguments"""
         # split the args into two parts, separated by `--`
         # the first part is the args for pipen_cli_config
         # the second part is the args for the pipeline
         args = sys.argv[1:]
         idx = args.index("--") if "--" in args else len(args)
-        args, rest = args[:idx], args[idx + 1 :]
+        args, rest = args[:idx], args[idx + 1:]
         parsed = self.parser.parse_args(args=args)
         parsed.name = parsed.name or parsed.pipeline.rpartition(":")[-1]
         parsed.pipeline_args = rest
         return parsed
 
     def exec_command(self, args: Namespace) -> None:
         """Execute the command"""
```

### Comparing `pipen_board-0.0.5/pipen_board/data_manager.py` & `pipen_board-0.0.6/pipen_board/data_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,26 +107,25 @@
     for arg, arginfo in anno.items():
         argspec[arg] = arginfo.attrs.copy()
         # type - bool/text/choice/mchoice(s)/json/auto/list(array)/ns(namespace)
         # required
         # choices
         # itype
         if "ctype" not in argspec[arg]:
-            if (argspec[arg].get("action") in ("store_true", "store_false")):
+            if argspec[arg].get("action") in ("store_true", "store_false"):
                 argspec[arg]["type"] = "bool"
             elif (
                 argspec[arg].get("action") in ("ns", "namespace")
                 or argspec[arg].get("ns")
                 or argspec[arg].get("namespace")
             ):
                 argspec[arg]["type"] = "ns"
             elif (
-                argspec[arg].get("action") in (
-                    "append", "extend", "clear_append", "clear_extend"
-                )
+                argspec[arg].get("action")
+                in ("append", "extend", "clear_append", "clear_extend")
                 or argspec[arg].get("array")
                 or argspec[arg].get("list")
             ):
                 argspec[arg]["type"] = "list"
             elif argspec[arg].get("choices") or argspec[arg].get("choice"):
                 argspec[arg]["type"] = "choice"
             elif argspec[arg].get("mchoice") or argspec[arg].get("mchoices"):
@@ -143,18 +142,17 @@
             argspec[arg]["choices_desc"] = [
                 term.help for term in arginfo.terms.values()
             ]
         else:
             argspec[arg]["value"] = argspec[arg].pop("default", None)
 
         # determine the itype for list elements
-        if t == 'list':
-            if (
-                argspec[arg]["value"] is not None
-                and not isinstance(argspec[arg]["value"], list)
+        if t == "list":
+            if argspec[arg]["value"] is not None and not isinstance(
+                argspec[arg]["value"], list
             ):
                 argspec[arg]["value"] = [argspec[arg]["value"]]
             if (
                 argspec[arg]["value"] is not None
                 and argspec[arg]["value"]
                 and "itype" not in argspec[arg]
                 and not isinstance(argspec[arg]["value"][0], str)
@@ -219,36 +217,36 @@
 
 def _load_additional(additional: str, **kwargs) -> Mapping[str, Any]:
     """Load additional config files"""
     if not additional:
         return {}
 
     parsed = urlparse(additional)
-    cache_dir = Path(gettempdir()) / 'pipen-cli-config-additional-configs'
+    cache_dir = Path(gettempdir()) / "pipen-cli-config-additional-configs"
     cache_dir.mkdir(parents=True, exist_ok=True)
-    if parsed.scheme in ('http', 'https', 'ftp', 'ftps', 'gh'):
+    if parsed.scheme in ("http", "https", "ftp", "ftps", "gh"):
         from hashlib import sha256
         from urllib.error import URLError
         from urllib.request import urlretrieve
 
-        if parsed.scheme == 'gh':
+        if parsed.scheme == "gh":
             try:
-                user, repo, file_path = parsed.path.split('/', 2)
+                user, repo, file_path = parsed.path.split("/", 2)
             except ValueError:
                 raise ValueError(f"Invalid gh:// URL: {additional}")
-            branch = 'master'
-            if '@' in file_path:
-                file_path, branch = file_path.split('@')
+            branch = "master"
+            if "@" in file_path:
+                file_path, branch = file_path.split("@")
             parsed = urlparse(
                 "https://raw.githubusercontent.com/"
                 f"{user}/{repo}/{branch}/{file_path}"
             )
 
         url = parsed.geturl()
-        cache_key = sha256(url.encode('utf-8')).hexdigest()
+        cache_key = sha256(url.encode("utf-8")).hexdigest()
         additional = cache_dir / f"{cache_key}-{parsed.path.split('/')[-1]}"
         if not additional.exists():
             try:
                 urlretrieve(url, additional)
             except URLError:
                 raise ValueError(
                     f"Could not retrieve remote path: {additional}"
@@ -267,26 +265,33 @@
     return Config.load(configfile)
 
 
 async def _get_config_data(args: Namespace) -> Mapping[str, Any]:
     """Get the pipeline data"""
     old_argv = sys.argv
     sys.argv = ["@pipen-board"] + args.pipeline_args
-    logger.debug("DBG Fetching pipeline data ...")
+    logger.debug(
+        "[bold][yellow]DBG[/yellow][/bold] Fetching pipeline data ..."
+    )
     try:
         pipeline = parse_pipeline(args.pipeline)
         # Initialize the pipeline so that the arguments definied by
         # other plugins (i.e. pipen-args) to take in place.
+        pipeline.workdir = Path(pipeline.config.workdir) / args.name
         await pipeline._init()
+        pipeline.workdir.mkdir(parents=True, exist_ok=True)
         pipeline.build_proc_relationships()
     finally:
         sys.argv = old_argv
 
     if args.additional:
-        logger.debug("DBG Loading additional configuration items ...")
+        logger.debug(
+            "[bold][yellow]DBG[/yellow][/bold] "
+            "Loading additional configuration items ..."
+        )
         data = _load_additional(
             args.additional,
             name=args.name,
             pipeline=args.pipeline,
             pipeline_args=args.pipeline_args,
         )
     else:
@@ -304,36 +309,36 @@
             "the result directory"
         ),
     }
     data[SECTION_PIPELINE_OPTIONS]["desc"] = {
         "type": "str",
         "value": pipeline.desc,
         "desc": (
-            "The description of the pipeline, "
-            "shows in the log and report."
+            "The description of the pipeline, " "shows in the log and report."
         ),
     }
     data[SECTION_PIPELINE_OPTIONS]["outdir"] = {
         "desc": "The output directory of your pipeline",
-        "placeholder": "./<name>_results",
+        "placeholder": "./<name>-output",
         "type": "str",
         "value": None,
     }
     data[SECTION_PROCESSES] = {}
     pg_sec = {}
     for proc in pipeline.procs:
-        logger.debug("DBG Parsing process %s ...", proc.name)
+        logger.debug(
+            "[bold][yellow]DBG[/yellow][/bold] Parsing process %s ...",
+            proc.name,
+        )
 
         pg = proc.__meta__["procgroup"]
         if pg:
             if pg.name not in pg_sec:
                 pg_sec[pg.name] = {"PROCESSES": {}}
-                pg_args = _anno_to_argspec(
-                    annotate(pg.__class__).get("Args")
-                )
+                pg_args = _anno_to_argspec(annotate(pg.__class__).get("Args"))
                 if pg_args:
                     for arg, arginfo in pg_args.items():
                         arginfo["value"] = pg.DEFAULTS.get(arg)
                     pg_sec[pg.name]["ARGUMENTS"] = pg_args
 
             pg_sec[pg.name][SECTION_PROCESSES][proc.name] = _proc_to_argspec(
                 proc,
@@ -381,25 +386,22 @@
         """
         if configfile:
             with PIPEN_BOARD_DIR.joinpath(configfile).open() as f:
                 self._config_data = json.load(f)
                 return
 
         if (
-            (use_cached is True or (use_cached == "auto" and args.dev))
-            and self._config_data
-        ):
+            use_cached is True or (use_cached == "auto" and args.dev)
+        ) and self._config_data:
             return
 
         # Use multiprocessing to get a clean environment
         # to load the pipeline to avoid conflicts
         def target(conn):
-            conn.send(
-                json.dumps(asyncio.run(_get_config_data(args))).encode()
-            )
+            conn.send(json.dumps(asyncio.run(_get_config_data(args))).encode())
             conn.close()
 
         parent_conn, child_conn = Pipe()
         p = Process(target=target, args=(child_conn,))
         p.start()
         data = parent_conn.recv()
         p.join()
@@ -428,15 +430,15 @@
             out[SECTION_LOG] = logfile.read_text()
 
         config_data = self._config_data
         outdir = config_data[SECTION_PIPELINE_OPTIONS].get(
             "outdir",
             {"value": None},
         )["value"]
-        outdir = outdir or Path(args.root).joinpath(f"{args.name}_results")
+        outdir = outdir or Path(args.root).joinpath(f"{args.name}-output")
         reports_dir = outdir.joinpath("REPORTS")
         if reports_dir.joinpath("index.html").is_file():
             out[SECTION_REPORTS] = str(reports_dir)
 
         diagram = outdir.joinpath("diagram.svg")
         if diagram.is_file():
             out[SECTION_DIAGRAM] = diagram.read_text()
@@ -508,15 +510,17 @@
     async def send_run_data(self, ws, force: bool = False):
         if ws is None:
             return
         if not force and time.time() - self._timer < self.INTERVAL:
             return
 
         # Send data
-        logger.debug("DBG Sending run data to the frontend")
+        logger.debug(
+            "[bold][yellow]DBG[/yellow][/bold] Sending run data to the frontend"
+        )
         try:
             await ws.send(json.dumps(self._run_data))
         except BrokenPipeError:
             pass
 
         # Reset timer
         self._timer = time.time()
@@ -528,23 +532,25 @@
 
         if SECTION_DIAGRAM in data:
             self._run_data[SECTION_DIAGRAM] = data[SECTION_DIAGRAM]
 
         if SECTION_PROCESSES in data:
             for proc in data[SECTION_PROCESSES]:
                 self._run_data[SECTION_PROCESSES][proc] = {
-                    "status": "init", "jobs": []
+                    "status": "init",
+                    "jobs": [],
                 }
 
         if SECTION_PROCGROUPS in data:
             for pg in data[SECTION_PROCGROUPS]:
                 self._run_data[SECTION_PROCGROUPS][pg] = {}
                 for proc in data[SECTION_PROCGROUPS][pg]:
                     self._run_data[SECTION_PROCGROUPS][pg][proc] = {
-                        "status": "init", "jobs": []
+                        "status": "init",
+                        "jobs": [],
                     }
 
         self.timer = time.time()
         await self.send_run_data(ws, force=True)
 
     async def on_complete(self, data, ws):
         if isinstance(data, str):
@@ -562,15 +568,17 @@
 
         proc, group, njobs = data["proc"], data["procgroup"], data["njobs"]
 
         if not group:
             self._run_data[SECTION_PROCESSES][proc]["status"] = "running"
             self._run_data[SECTION_PROCESSES][proc]["jobs"] = ["init"] * njobs
         else:
-            self._run_data[SECTION_PROCGROUPS][group][proc]["status"] = "running"
+            self._run_data[SECTION_PROCGROUPS][group][proc][
+                "status"
+            ] = "running"
             self._run_data[SECTION_PROCGROUPS][group][proc]["jobs"] = [
                 "init"
             ] * njobs
 
         await self.send_run_data(ws, force=True)
 
     async def on_proc_done(self, data, ws):
@@ -597,17 +605,17 @@
             data = json.loads(data)
 
         proc, group, job = data["proc"], data["procgroup"], data["job"]
 
         if not group:
             self._run_data[SECTION_PROCESSES][proc]["jobs"][job] = status
         else:
-            self._run_data[
-                SECTION_PROCGROUPS
-            ][group][proc]["jobs"][job] = status
+            self._run_data[SECTION_PROCGROUPS][group][proc]["jobs"][
+                job
+            ] = status
         await self.send_run_data(ws)
 
     async def on_job_queued(self, data, ws):
         await self._on_job(data, "queued", ws)
 
     async def on_job_submitted(self, data, ws):
         await self._on_job(data, "submitted", ws)
```

### Comparing `pipen_board-0.0.5/pipen_board/defaults.py` & `pipen_board-0.0.6/pipen_board/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.5/pipen_board/frontend/build/assets/favicon.png` & `pipen_board-0.0.6/pipen_board/frontend/build/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.5/pipen_board/frontend/build/assets/index.css` & `pipen_board-0.0.6/pipen_board/frontend/build/assets/index.css`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.5/pipen_board/frontend/build/assets/index.js` & `pipen_board-0.0.6/pipen_board/frontend/build/assets/index.js`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.5/pipen_board/frontend/build/assets/schema.json` & `pipen_board-0.0.6/pipen_board/frontend/build/assets/schema.json`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.5/pipen_board/plugin.py` & `pipen_board-0.0.6/pipen_board/plugin.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.0.5/pipen_board/quart_app.py` & `pipen_board-0.0.6/pipen_board/quart_app.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,15 +102,17 @@
         if not overwriteConfig and tomlfile.exists():
             return {}, 409
         try:
             tomlfile.write_text(config)
         except Exception:
             return {}, 410
 
-        logger.info(f"API Running pipeline: {command}")
+        logger.info(
+            f"[bold][yellow]API[/yellow][/bold] Running pipeline: {command}"
+        )
         # Run command at background
         app.add_background_task(
             data_manager.run_pipeline,
             command,
             clients.get("web"),
         )
         return {"ok": True}
```

### Comparing `pipen_board-0.0.5/pyproject.toml` & `pipen_board-0.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 [tool.poetry]
 name = "pipen-board"
-version = "0.0.5"
+version = "0.0.6"
 description = "Visualization configuration and running of pipen pipelines on the web"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 exclude = ["pipen_board/frontend/[!build]*", "pipen_board/frontend/index.html"]
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pipen = "^0.9"
 quart = "^0.18"
-pipen-annotate = "^0.7"
-pipen-args = "^0.9.5"
+pipen-args = "^0.9.7"
 websocket-client = "^1.5"
 cmdy = "^0.5"
 pipen-log2file = "^0.2.1"
 
 [tool.poetry.plugins.pipen]
 board = "pipen_board:pipen_board_plugin"
```

### Comparing `pipen_board-0.0.5/setup.py` & `pipen_board-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 ['pipen_board']
 
 package_data = \
 {'': ['*'], 'pipen_board': ['frontend/build/*', 'frontend/build/assets/*']}
 
 install_requires = \
 ['cmdy>=0.5,<0.6',
- 'pipen-annotate>=0.7,<0.8',
- 'pipen-args>=0.9.5,<0.10.0',
+ 'pipen-args>=0.9.7,<0.10.0',
  'pipen-log2file>=0.2.1,<0.3.0',
- 'pipen>=0.9,<0.10',
  'quart>=0.18,<0.19',
  'websocket-client>=1.5,<2.0']
 
 entry_points = \
 {'pipen': ['board = pipen_board:pipen_board_plugin'],
  'pipen_cli': ['cli-board = pipen_board:PipenCliBoardPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-board',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'Visualization configuration and running of pipen pipelines on the web',
     'long_description': "# pipen-board\n\nVisualize configuration and running of [pipen][1] pipelines on the web.\n\n## Installation\n\n```bash\npip install pipen-board\n```\n\n## Usage\n\n```bash\n$ pipen board --help\nUsage: pipen board [options] <pipeline> -- [pipeline options]\n\nVisualize configuration and running of pipen pipelines on the web\n\nRequired Arguments:\n  pipeline              The pipeline and the CLI arguments to run the pipeline. For the\n                        pipeline either `/path/to/pipeline.py:<pipeline>` or\n                        `<module.submodule>:<pipeline>` `<pipeline>` must be an instance of\n                        `Pipen` and running the pipeline should be called under `__name__ ==\n                        '__main__'.\n\nOptions:\n  -h, --help            show help message and exit\n  --port PORT           Port to serve the UI wizard [default: 18521]\n  --name NAME           The name of the pipeline. Default to the pipeline class name. You\n                        can use a different name to associate with a different set of\n                        configurations.\n  --additional FILE     Additional arguments for the pipeline, in YAML, INI, JSON or TOML\n                        format. Can have sections `ADDITIONAL_OPTIONS` and `RUNNING_OPTIONS`\n  --dev                 Run the pipeline in development mode. This will print verbosal\n                        logging information and reload the pipeline if a new instantce\n                        starts when page reloads.\n  --root ROOT           The root directory of the pipeline. [default: .]\n  --loglevel {auto,debug,info,warning,error,critical}\n                        Logging level. If `auto`, set to `debug` if `--dev` is set,\n                        otherwise `info` [default: auto]\n```\n\n[1]: https://github.com/pwwang/pipen\n",
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_board-0.0.5/PKG-INFO` & `pipen_board-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: pipen-board
-Version: 0.0.5
+Version: 0.0.6
 Summary: Visualization configuration and running of pipen pipelines on the web
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cmdy (>=0.5,<0.6)
-Requires-Dist: pipen (>=0.9,<0.10)
-Requires-Dist: pipen-annotate (>=0.7,<0.8)
-Requires-Dist: pipen-args (>=0.9.5,<0.10.0)
+Requires-Dist: pipen-args (>=0.9.7,<0.10.0)
 Requires-Dist: pipen-log2file (>=0.2.1,<0.3.0)
 Requires-Dist: quart (>=0.18,<0.19)
 Requires-Dist: websocket-client (>=1.5,<2.0)
 Description-Content-Type: text/markdown
 
 # pipen-board
```

