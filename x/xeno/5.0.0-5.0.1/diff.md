# Comparing `tmp/xeno-5.0.0.tar.gz` & `tmp/xeno-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeno-5.0.0.tar", last modified: Fri Apr 14 23:10:26 2023, max compression
+gzip compressed data, was "xeno-5.0.1.tar", last modified: Tue Apr 18 01:19:15 2023, max compression
```

## Comparing `xeno-5.0.0.tar` & `xeno-5.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-14 23:10:26.244811 xeno-5.0.0/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-04-03 20:39:53.000000 xeno-5.0.0/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-04-03 20:39:53.000000 xeno-5.0.0/MANIFEST.in
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-14 23:10:26.244811 xeno-5.0.0/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-04-03 20:39:53.000000 xeno-5.0.0/README.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-04-14 23:10:26.244811 xeno-5.0.0/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-04-14 23:10:04.000000 xeno-5.0.0/setup.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-14 23:10:26.244811 xeno-5.0.0/xeno/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/abstract.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/async_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/attributes.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    14309 2023-04-14 23:07:26.000000 xeno-5.0.0/xeno/build.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2956 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/color.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9804 2023-04-14 22:17:15.000000 xeno-5.0.0/xeno/cookbook.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/decorators.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/errors.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5436 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/events.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/namespaces.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/pkg_config.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19116 2023-04-14 22:53:16.000000 xeno-5.0.0/xeno/recipe.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6738 2023-04-14 22:25:58.000000 xeno-5.0.0/xeno/shell.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1559 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/spinner.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/sync_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/testing.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2965 2023-04-14 18:38:05.000000 xeno-5.0.0/xeno/utils.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-14 23:10:26.244811 xeno-5.0.0/xeno.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-14 23:10:26.000000 xeno-5.0.0/xeno.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-04-14 23:10:26.000000 xeno-5.0.0/xeno.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-04-14 23:10:26.000000 xeno-5.0.0/xeno.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-04-14 23:10:26.000000 xeno-5.0.0/xeno.egg-info/top_level.txt
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-18 01:19:15.848342 xeno-5.0.1/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-04-03 20:39:53.000000 xeno-5.0.1/LICENSE
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-04-03 20:39:53.000000 xeno-5.0.1/MANIFEST.in
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-18 01:19:15.848342 xeno-5.0.1/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-04-03 20:39:53.000000 xeno-5.0.1/README.md
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-04-18 01:19:15.848342 xeno-5.0.1/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-04-18 01:18:36.000000 xeno-5.0.1/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-18 01:19:15.848342 xeno-5.0.1/xeno/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/abstract.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/async_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/attributes.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    14967 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/build.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2956 2023-04-14 18:38:05.000000 xeno-5.0.1/xeno/color.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9807 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/cookbook.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/decorators.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-04-14 18:38:05.000000 xeno-5.0.1/xeno/errors.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5325 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/events.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-04-14 18:38:05.000000 xeno-5.0.1/xeno/namespaces.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-04-14 18:38:05.000000 xeno-5.0.1/xeno/pkg_config.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    20127 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/recipe.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6738 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/shell.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1543 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/spinner.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/sync_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/testing.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2965 2023-04-18 01:18:36.000000 xeno-5.0.1/xeno/utils.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-18 01:19:15.848342 xeno-5.0.1/xeno.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-18 01:19:15.000000 xeno-5.0.1/xeno.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-04-18 01:19:15.000000 xeno-5.0.1/xeno.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-04-18 01:19:15.000000 xeno-5.0.1/xeno.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-04-18 01:19:15.000000 xeno-5.0.1/xeno.egg-info/top_level.txt
```

### Comparing `xeno-5.0.0/LICENSE` & `xeno-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/PKG-INFO` & `xeno-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 5.0.0
+Version: 5.0.1
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xeno-5.0.0/README.md` & `xeno-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/setup.py` & `xeno-5.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="xeno",
-    version="5.0.0",
+    version="5.0.1",
     description="The Python dependency injector from outer space.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/xeno",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

### Comparing `xeno-5.0.0/xeno/__init__.py` & `xeno-5.0.1/xeno/__init__.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/abstract.py` & `xeno-5.0.1/xeno/abstract.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/async_injector.py` & `xeno-5.0.1/xeno/async_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/attributes.py` & `xeno-5.0.1/xeno/attributes.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/build.py` & `xeno-5.0.1/xeno/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 # Date: Friday March 17, 2023
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
 import asyncio
 import io
+import sys
 from argparse import ArgumentParser
 from functools import partial
 from typing import Any, Callable, Optional, cast
 
 from xeno.async_injector import AsyncInjector
 from xeno.attributes import MethodAttributes
 from xeno.color import color
 from xeno.cookbook import recipe as base_recipe
 from xeno.decorators import named
 from xeno.events import Event, EventBus
-from xeno.recipe import Events, Recipe, FormatF
+from xeno.recipe import Events, FormatF, Recipe
 from xeno.shell import Environment
+from xeno.spinner import Spinner
 from xeno.utils import async_map
 
 # --------------------------------------------------------------------
-BusHook = Callable[[EventBus], None]
+EngineHook = Callable[["Engine", EventBus], None]
 
 
 # --------------------------------------------------------------------
 class Config:
     class Mode:
         BUILD = "build"
         REBUILD = "rebuild"
@@ -136,19 +138,20 @@
 
     class Attributes:
         TARGET = "xeno.build.target"
         DEFAULT = "xeno.build.default"
 
     def __init__(self, name="Xeno v5 Build Engine"):
         self.name = name
-        self.bus_hooks: list[BusHook] = list()
+        self.bus_hooks: list[EngineHook] = list()
         self.env = Environment.context()
         self.injector = AsyncInjector()
+        self.scan = Recipe.Scanner()
 
-    def add_hook(self, hook: BusHook):
+    def add_hook(self, hook: EngineHook):
         self.bus_hooks.append(hook)
 
     async def root_targets(self) -> list[tuple[str, Recipe]]:
         root_names = [
             k
             for k, _ in self.injector.scan_resources(
                 lambda _, v: v.check(self.Attributes.TARGET)
@@ -275,20 +278,21 @@
             assert isinstance(
                 target, Recipe
             ), f"Target `{name}` did not yield a recipe."
 
         return targets
 
     async def _make_targets(self, config, targets):
-        scan = Recipe.Scanner()
-        scan.scan_params(*[v for _, v in targets])
-        while scan.has_recipes():
-            await scan.gather_all()
-
-        return scan.args(Recipe.PassMode.RESULTS)
+        self.scan.scan_params(*[v for _, v in targets])
+        while self.scan.has_recipes():
+            await self.scan.gather_all()
+
+        args = self.scan.args(Recipe.PassMode.RESULTS)
+        self.scan.clear()
+        return args
 
     async def _clean_targets(self, config, targets):
         match config.cleanup_mode:
             case Config.CleanupMode.SHALLOW:
                 return await asyncio.gather(*[t.clean() for _, t in targets])
             case Config.CleanupMode.RECURSIVE:
                 return await asyncio.gather(
@@ -339,86 +343,102 @@
         result, _ = await asyncio.gather(self.build_async(*argv), bus.run())
         return result
 
     def build(self, *argv):
         with EventBus.session():
             bus = EventBus.get()
             for hook in self.bus_hooks:
-                hook(bus)
+                hook(self, bus)
             return asyncio.run(self._build_loop(bus, *argv))
 
 
 # --------------------------------------------------------------------
 class DefaultEngineHook:
+    def __init__(self):
+        self.spinner = Spinner("resolving")
+        self._clear_chars = 0
+
+    def print(self, s):
+        sys.stdout.write("\r")
+        sys.stdout.write(" " * self._clear_chars)
+        sys.stdout.write("\r")
+        return print(s)
+
     def sigil(self, event, **kwargs):
-        bkt = partial(color, fg='white', render='bold')
+        bkt = partial(color, fg="white", render="bold")
         sb = io.StringIO()
-        sb.write(bkt('['))
+        sb.write(bkt("["))
         sb.write(color(event.context.sigil(event.context), **kwargs))
-        sb.write(bkt(']'))
-        sb.write(' ')
+        sb.write(bkt("]"))
+        sb.write(" ")
         return sb.getvalue()
 
+    async def on_frame(self, event):
+        self.spinner.message = f"resolving [{Recipe.count}]"
+        self._clear_chars = await self.spinner.spin()
+
     def on_clean(self, event):
-        clr = partial(color, fg='white')
+        clr = partial(color, fg="white")
         sb = io.StringIO()
-        sb.write(self.sigil(event, fg='green', render='bold'))
+        sb.write(self.sigil(event, fg="green", render="bold"))
         sb.write(clr(event.context.clean_f(event.context)))
-        print(sb.getvalue())
+        self.print(sb.getvalue())
 
     def on_error(self, event):
-        clr = partial(color, fg='red')
+        clr = partial(color, fg="red")
         sb = io.StringIO()
-        sb.write(self.sigil(event, fg='red', render='bold'))
+        sb.write(self.sigil(event, fg="red", render="bold"))
         sb.write(clr(event.data))
-        print(sb.getvalue())
+        self.print(sb.getvalue())
 
     def on_fail(self, event):
-        clr = partial(color, fg='white')
+        clr = partial(color, fg="white")
         sb = io.StringIO()
-        sb.write(self.sigil(event, fg='red', render='bold'))
+        sb.write(self.sigil(event, fg="red", render="bold"))
         sb.write(clr(event.context.fail_f(event.context)))
-        print(sb.getvalue())
+        self.print(sb.getvalue())
 
     def on_info(self, event: Event):
-        clr = partial(color, fg='white', render='dim')
+        clr = partial(color, fg="white", render="dim")
         sb = io.StringIO()
-        sb.write(self.sigil(event, fg='white', render='dim'))
+        sb.write(self.sigil(event, fg="white", render="dim"))
         sb.write(clr(event.data))
-        print(sb.getvalue())
+        self.print(sb.getvalue())
 
     def on_start(self, event: Event):
-        clr = partial(color, fg='white')
+        clr = partial(color, fg="white")
         sb = io.StringIO()
-        sb.write(self.sigil(event, fg='cyan', render='bold'))
+        sb.write(self.sigil(event, fg="cyan", render="bold"))
         sb.write(clr(event.context.start_f(event.context)))
-        print(sb.getvalue())
+        self.print(sb.getvalue())
 
     def on_success(self, event: Event):
-        clr = partial(color, fg='white')
+        clr = partial(color, fg="white")
         sb = io.StringIO()
-        sb.write(self.sigil(event, fg='green', render='bold'))
+        sb.write(self.sigil(event, fg="green", render="bold"))
         sb.write(clr(event.context.ok_f(event.context)))
-        print(sb.getvalue())
+        self.print(sb.getvalue())
 
     def on_warning(self, event: Event):
-        clr = partial(color, fg='white')
+        clr = partial(color, fg="white")
         sb = io.StringIO()
-        sb.write(self.sigil(event, fg='yellow', render='bold'))
+        sb.write(self.sigil(event, fg="yellow", render="bold"))
         sb.write(clr(event.data))
-        print(sb.getvalue())
+        self.print(sb.getvalue())
 
-    def __call__(self, bus: EventBus):
+    def __call__(self, engine: Engine, bus: EventBus):
         bus.subscribe(Events.CLEAN, self.on_clean)
         bus.subscribe(Events.ERROR, self.on_error)
         bus.subscribe(Events.FAIL, self.on_fail)
         bus.subscribe(Events.INFO, self.on_info)
         bus.subscribe(Events.START, self.on_start)
         bus.subscribe(Events.SUCCESS, self.on_success)
         bus.subscribe(Events.WARNING, self.on_warning)
+        bus.subscribe(EventBus.FRAME, self.on_frame)
+
 
 # --------------------------------------------------------------------
 engine = Engine()
 engine.add_hook(DefaultEngineHook())
 provide = engine.provide
 recipe = engine.recipe
 target = engine.target
```

### Comparing `xeno-5.0.0/xeno/color.py` & `xeno-5.0.1/xeno/color.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/cookbook.py` & `xeno-5.0.1/xeno/cookbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,17 +150,17 @@
     ResultSpec = Iterable[Result] | Result
 
     @staticmethod
     def sigil_format(recipe: Recipe) -> str:
         assert isinstance(recipe, ShellRecipe)
         recipe = cast(ShellRecipe, recipe)
         if recipe.target is not None:
-            return f'{recipe.program_name()}{recipe.SIGIL_TARGET_SEPARATOR}{recipe.target.name}'
+            return f'>_{recipe.program_name()}{recipe.symbols().target}{recipe.target.name}'
         else:
-            return recipe.program_name()
+            return f'>_{recipe.program_name()}'
 
     def __init__(
         self,
         cmd: Union[str, Iterable[str]],
         *,
         as_user: Optional[str] = None,
         code=0,
```

### Comparing `xeno-5.0.0/xeno/decorators.py` & `xeno-5.0.1/xeno/decorators.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/errors.py` & `xeno-5.0.1/xeno/errors.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/events.py` & `xeno-5.0.1/xeno/events.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,24 @@
 # --------------------------------------------------------------------
 
 """
 Asynchronous event dispatch and broadcast.
 """
 
 import asyncio
+import inspect
 from collections import defaultdict
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
-from enum import Enum
 from typing import Any, Callable, Generator, Optional
 
 from xeno.utils import async_wrap
 
 
 # --------------------------------------------------------------------
-class DispatchMode(Enum):
-    IMMEDIATE = 0
-    ASYNC = 1
-
-
-# --------------------------------------------------------------------
 @dataclass
 class Event:
     name: str
     context: Any = None
     data: Any = None
     when: datetime = field(default_factory=datetime.now)
 
@@ -41,14 +35,16 @@
 
 # --------------------------------------------------------------------
 EventListener = Callable[[Event], Any]
 
 
 # --------------------------------------------------------------------
 class EventBus:
+    FRAME = "EventBus.FRAME"
+
     _current_bus: Optional["EventBus"] = None
 
     class _Session:
         def __init__(self):
             self.bus = EventBus()
 
         def __enter__(self):
@@ -78,52 +74,44 @@
 
     def send(self, event: Event):
         if self._has_async_listeners_for_event(event):
             self.queue.put_nowait(event)
         self._dispatch_sync(event)
 
     def shutdown(self):
-        self.shutdown_flag = True
+        self.shutdown_flag.set()
         self.sync_listeners.clear()
         self.sync_subs.clear()
         self.async_listeners.clear()
         self.async_subs.clear()
         while not self.queue.empty():
             self.queue.get_nowait()
 
-    def listen(
-        self,
-        listener: EventListener,
-        dispatch_mode=DispatchMode.IMMEDIATE,
-    ):
-        match dispatch_mode:
-            case DispatchMode.IMMEDIATE:
-                self.sync_listeners.add(listener)
-            case DispatchMode.ASYNC:
-                self.async_listeners.add(listener)
+    def listen(self, listener: EventListener):
+        if inspect.iscoroutinefunction(listener):
+            self.async_listeners.add(listener)
+        else:
+            self.sync_listeners.add(listener)
 
     def unlisten(self, listener: EventListener):
         try:
             self.sync_listeners.remove(listener)
         except KeyError:
             pass
 
         try:
             self.async_listeners.remove(listener)
         except KeyError:
             pass
 
-    def subscribe(
-        self, event: str, listener: EventListener, dispatch_mode=DispatchMode.IMMEDIATE
-    ):
-        match dispatch_mode:
-            case DispatchMode.IMMEDIATE:
-                self.sync_subs[event].add(listener)
-            case DispatchMode.ASYNC:
-                self.async_subs[event].add(listener)
+    def subscribe(self, event: str, listener: EventListener):
+        if inspect.iscoroutinefunction(listener):
+            self.async_subs[event].add(listener)
+        else:
+            self.sync_subs[event].add(listener)
 
     def unsubscribe(self, event: str, listener: EventListener):
         subs = self.sync_subs[event]
         try:
             subs.remove(listener)
         except KeyError:
             pass
@@ -135,22 +123,23 @@
             subs.remove(listener)
         except KeyError:
             pass
         if not subs:
             del self.async_subs[event]
 
     async def run(self):
-        while not self.shutdown_flag:
+        while not self.shutdown_flag.is_set():
             try:
                 event = self.queue.get_nowait()
                 await self._dispatch_async(event)
 
             except asyncio.QueueEmpty:
                 pass
 
+            await self._dispatch_frame_event()
             await asyncio.sleep(0)
 
     def _has_async_listeners_for_event(self, event: Event) -> bool:
         try:
             next(self._async_listeners_for_event(event))
             return True
         except StopIteration:
@@ -166,14 +155,19 @@
     def _sync_listeners_for_event(
         self, event: Event
     ) -> Generator[EventListener, None, None]:
         yield from self.sync_listeners
         if event.name in self.sync_subs:
             yield from self.sync_subs[event.name]
 
+    async def _dispatch_frame_event(self):
+        event = Event(EventBus.FRAME, self)
+        await self._dispatch_async(event)
+        self._dispatch_sync(event)
+
     def _dispatch_sync(self, event: Event):
         for listener in self._sync_listeners_for_event(event):
             listener(event)
 
     async def _dispatch_async(self, event: Event):
         await asyncio.gather(
             *(
```

### Comparing `xeno-5.0.0/xeno/namespaces.py` & `xeno-5.0.1/xeno/namespaces.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/pkg_config.py` & `xeno-5.0.1/xeno/pkg_config.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/recipe.py` & `xeno-5.0.1/xeno/recipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,34 +6,40 @@
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
 import asyncio
 import inspect
 import shutil
+import sys
+from dataclasses import dataclass
 from datetime import datetime, timedelta
 from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, Generator, Iterable, Optional
 
 from xeno.events import Event, EventBus
 from xeno.shell import PathSpec, Shell
 from xeno.utils import async_map, async_vwrap, async_wrap, is_iterable
 
+# --------------------------------------------------------------------
+UNICODE_SUPPORT = sys.stdout.encoding.lower().startswith("utf")
+
 
 # --------------------------------------------------------------------
 class Events:
     CLEAN = "clean"
     DEBUG = "debug"
     ERROR = "error"
     FAIL = "fail"
     INFO = "info"
     START = "start"
     SUCCESS = "success"
     WARNING = "warning"
+    END = "end"
 
 
 # --------------------------------------------------------------------
 class BuildError(Exception):
     pass
 
 
@@ -60,19 +66,36 @@
 MappedComponents = dict[str, "Recipe" | Iterable["Recipe"]]
 FormatF = Callable[["Recipe"], str]
 
 
 # --------------------------------------------------------------------
 class Recipe:
     DEFAULT_TARGET_PARAM = "out"
-    SIGIL_TARGET_SEPARATOR = "→ "
-    START_SYMBOL = "⚙"
-    OK_SYMBOL = "✓"
-    FAIL_SYMBOL = "✗"
-    WARNING_SYMBOL = "⚠"
+    UNICODE_SUPPORT = UNICODE_SUPPORT
+
+    @dataclass
+    class Symbols:
+        target: str
+        start: str
+        ok: str
+        fail: str
+        warning: str
+
+    SYMBOLS: Optional[Symbols] = None
+
+    @classmethod
+    def symbols(cls) -> "Recipe.Symbols":
+        if cls.SYMBOLS is None:
+            if Recipe.UNICODE_SUPPORT:
+                cls.SYMBOLS = Recipe.Symbols(target="→ ", start="⚙", ok="✓", fail="✗", warning="⚠")
+            else:
+                cls.SYMBOLS = Recipe.Symbols(target="->", start="@", ok=":)", fail=":(", warning="/!\\")
+        return cls.SYMBOLS
+
+    count = 0
 
     class PassMode(Enum):
         NORMAL = 0
         RESULTS = 1
         TARGETS = 2
 
     class ParamType(Enum):
@@ -84,14 +107,21 @@
         def __init__(self):
             self._args: list[Any] = []
             self._kwargs: dict[str, Any] = {}
             self._arg_offsets: list[int] = []
             self._kwarg_keys: list[str] = []
             self._paths: list[Path] = []
 
+        def clear(self):
+            self._args.clear()
+            self._kwargs.clear()
+            self._arg_offsets.clear()
+            self._kwarg_keys.clear()
+            self._paths.clear()
+
         def _scan_one(self, arg) -> tuple[Any, "Recipe.ParamType"]:
             if isinstance(arg, Recipe):
                 return arg, Recipe.ParamType.RECIPE
 
             if is_iterable(arg):
                 arg = [*arg]
                 if all(isinstance(x, Recipe) for x in arg):
@@ -103,14 +133,17 @@
                 return arg, Recipe.ParamType.PATH
 
             return arg, Recipe.ParamType.NORMAL
 
         def has_recipes(self):
             return self._arg_offsets or self._kwarg_keys
 
+        def num_recipes(self):
+            return len(self._arg_offsets) + len(self._kwarg_keys)
+
         async def gather_args(self):
             """
             Await resolution of recipes in args and update args with their results.
             """
             results = await asyncio.gather(
                 *[v() if isinstance(v, Recipe) else async_vwrap(v) for v in self._args]
             )
@@ -140,19 +173,15 @@
             Await resolution of recipes in args and kwargs and update both with
             their results.
             """
 
             return asyncio.gather(self.gather_args(), self.gather_kwargs())
 
         def scan_params(self, *args, **kwargs):
-            self._args.clear()
-            self._arg_offsets.clear()
-            self._kwargs.clear()
-            self._kwarg_keys.clear()
-            self._paths.clear()
+            self.clear()
 
             for i, arg in enumerate(args):
                 self.scan(arg, offset=i)
 
             for k, arg in kwargs.items():
                 self.scan(arg, key=k)
 
@@ -260,18 +289,18 @@
             scanner.scan(arg, offset=i)
 
         for k, arg in kwargs.items():
             scanner.scan(arg, key=k)
 
         return scanner
 
-    @staticmethod
-    def sigil_format(recipe: "Recipe") -> str:
+    @classmethod
+    def sigil_format(cls, recipe: "Recipe") -> str:
         if recipe.target is not None:
-            return f"{recipe.name}{recipe.SIGIL_TARGET_SEPARATOR}{recipe.target.name}"
+            return f"{recipe.name}{cls.symbols().target}{recipe.target.name}"
         return recipe.name
 
     def __init__(
         self,
         component_list: ListedComponents = [],
         component_map: MappedComponents = {},
         *,
@@ -292,22 +321,22 @@
         self.component_list = component_list
         self.component_map = component_map
 
         self.as_user = as_user
         self.clean_f: FormatF = clean_f or (
             lambda r: f'cleaned {r.target.name if r.target else ""}'
         )
-        self.fail_f: FormatF = fail_f or (lambda _: f"{Recipe.FAIL_SYMBOL} fail")
+        self.fail_f: FormatF = fail_f or (lambda _: f"{self.symbols().fail} fail")
         self.keep = keep
         self.memoize = memoize
         self.name = name
         self.setup = setup
         self.sigil: FormatF = sigil or Recipe.sigil_format
-        self.start_f: FormatF = start_f or (lambda _: f"{Recipe.START_SYMBOL} start")
-        self.ok_f: FormatF = ok_f or (lambda _: f"{Recipe.OK_SYMBOL} ok")
+        self.start_f: FormatF = start_f or (lambda _: f"{self.symbols().start} start")
+        self.ok_f: FormatF = ok_f or (lambda _: f"{self.symbols().ok} ok")
         self.static_files = [Path(s) for s in static_files if s != target]
         self.sync = sync
         self.target = None if target is None else Path(target)
 
         self.lock = asyncio.Lock()
         self.saved_result = None
         self.parent_path: list[str] = []
@@ -518,26 +547,31 @@
 
     async def __call__(self):
         async with self.lock:
             if self.memoize and self.done() and not self.outdated(datetime.now()):
                 return self.saved_result
 
             try:
+                Recipe.count += 1
+
                 if self.setup is not None:
                     await self.setup()
 
                 self.log(Events.START)
                 result = await self._resolve()
                 self.log(Events.SUCCESS)
                 return result
 
             except Exception as e:
                 self.log(Events.FAIL, e)
                 raise BuildError() from e
 
+            finally:
+                Recipe.count -= 1
+
 
 # --------------------------------------------------------------------
 class Lambda(Recipe):
     def __init__(
         self,
         f: Callable,
         lambda_args: list[Any],
@@ -547,27 +581,30 @@
         **kwargs,
     ):
         if "name" not in kwargs:
             kwargs = {**kwargs, "name": f.__name__}
 
         scanner = Recipe.scan(lambda_args, lambda_kwargs)
         sig = inspect.signature(f)
-        bound_args = sig.bind(*lambda_args, **lambda_kwargs)
-        target = bound_args.arguments.get(target_param, None)
+        self.bound_args = sig.bind(*lambda_args, **lambda_kwargs)
+        target = self.bound_args.arguments.get(target_param, None)
 
         super().__init__(
             scanner.component_list(),
             scanner.component_map(),
             static_files=scanner.paths(),
             target=target,
             **kwargs,
         )
         self.f = f
         self.pass_mode = pass_mode
         self.scanner = scanner
 
+    def arg(self, name: str):
+        return self.bound_args.arguments.get(name, None)
+
     async def make(self):
         return await async_wrap(
             self.f,
             *self.scanner.args(self.pass_mode),
             **self.scanner.kwargs(self.pass_mode),
         )
```

### Comparing `xeno-5.0.0/xeno/shell.py` & `xeno-5.0.1/xeno/shell.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/spinner.py` & `xeno-5.0.1/xeno/spinner.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #
 # Distributed under terms of the MIT license.
 # --------------------------------------------------------------------
 
 import sys
 import asyncio
 import itertools
-from typing import Callable
 from datetime import datetime, timedelta
+from xeno.events import EventBus
 
 from xeno.color import color
 
 DEFAULT_SHAPE = [
     "[=   ]",
     "[==  ]",
     "[=== ]",
@@ -25,25 +25,25 @@
     "[   =]",
     "[    ]",
 ]
 
 
 class Spinner:
     def __init__(self, message: str, interval: float = 0.05, delay: float = 0.25):
-        ansi_spinner_shape = []
+        shape_array = []
 
         for shape in DEFAULT_SHAPE:
-            ansi_spinner_shape.append(
+            shape_array.append(
                 "".join(
                     [shape[0], color(shape[1:-1], fg="red", render="dim"), shape[-1]]
                 )
             )
 
         self.message = message
-        self.cycle = itertools.cycle(ansi_spinner_shape)
+        self.cycle = itertools.cycle(shape_array)
         self.interval = interval
         self.delay = delay
         self.start = datetime.now()
 
     async def spin(self) -> int:
         if not sys.stdout.isatty():
             return 0
```

### Comparing `xeno-5.0.0/xeno/sync_injector.py` & `xeno-5.0.1/xeno/sync_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/testing.py` & `xeno-5.0.1/xeno/testing.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno/utils.py` & `xeno-5.0.1/xeno/utils.py`

 * *Files identical despite different names*

### Comparing `xeno-5.0.0/xeno.egg-info/PKG-INFO` & `xeno-5.0.1/xeno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 5.0.0
+Version: 5.0.1
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
```

