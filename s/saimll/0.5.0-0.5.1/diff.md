# Comparing `tmp/saimll-0.5.0.tar.gz` & `tmp/saimll-0.5.1.tar.gz`

## Comparing `saimll-0.5.0.tar` & `saimll-0.5.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 saimll-0.5.0/examples/basics.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 saimll-0.5.0/playground/sample.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/__init__.py
--rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/pprint.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/logger/LogLevel.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/logger/__init__.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/logger/encoding.py
--rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/logger/log.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/saiml/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/saiml/color/__init__.py
--rw-r--r--   0        0        0    14911 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/saiml/color/colors.py
--rw-r--r--   0        0        0    10285 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/saiml/color/xterm_colors.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/saiml/markup/__init__.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/saiml/markup/formatting.py
--rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/saiml/markup/markup.py
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 saimll-0.5.0/saimll/saiml/markup/tokens.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 saimll-0.5.0/LICENSE
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 saimll-0.5.0/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 saimll-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 saimll-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 saimll-0.5.1/Makefile
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 saimll-0.5.1/examples/basics.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 saimll-0.5.1/playground/sample.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/__init__.py
+-rw-r--r--   0        0        0    13664 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/pprint.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/logger/LogLevel.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/logger/__init__.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/logger/encoding.py
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/logger/log.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/saiml/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/saiml/color/__init__.py
+-rw-r--r--   0        0        0    14911 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/saiml/color/colors.py
+-rw-r--r--   0        0        0    10285 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/saiml/color/xterm_colors.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/saiml/markup/__init__.py
+-rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/saiml/markup/formatting.py
+-rw-r--r--   0        0        0    11758 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/saiml/markup/markup.py
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 saimll-0.5.1/saimll/saiml/markup/tokens.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 saimll-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 saimll-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 saimll-0.5.1/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 saimll-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 saimll-0.5.1/PKG-INFO
```

### Comparing `saimll-0.5.0/examples/basics.py` & `saimll-0.5.1/examples/basics.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/saimll/pprint.py` & `saimll-0.5.1/saimll/pprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,31 @@
 class Missing:
     def __repr__(self) -> str:
         return f"MISSING"
 
 
 MISSING = Missing()
 
-def ppath(*args: str, clr: str = "yellow", spr: str = " > ") -> str:
+def _type(val: Any) -> type:
+    if isinstance(val, type):
+        return val
+    return type(val)
+
+def ppath(*args: str, clr: str = "\x1b[33m", spr: str = " > ") -> str:
     """Takes all the arguments, segments of path, and combines them with the given seperator and color.
 
     Args:
         clr (int): The color to apply to each segment of the path
         spr (str): The seperator between each segement of the path
 
     Returns:
         str: The formatted string
     """
-    return f"{spr}".join([SAIML.parse(f"[@F {clr}$]{arg.strip()}[@F]") for arg in args])
+    path = f"{spr}".join([f"{clr}{arg.strip()}\x1b[39m" for arg in args])
+    return path
 
 def pprint(
     *values: Any,
     depth: int = 2,
     end: str = "\n",
     seperator: str = " ",
     handler: Optional[Callable] = None,
@@ -63,15 +69,15 @@
         return p_collection(
             value, depth=depth, indent=indent, decode=decode, leading=leading
         )
 
     if isinstance(value, dict):
         return p_dict(value, depth=depth, indent=indent, decode=decode, leading=leading)
 
-    if isinstance(value, Callable) and not isinstance(value, type):
+    if callable(value) and value.__module__ not in ["builtins", "_sitebuiltins"] and not isinstance(value, type):
         if handler is not None:
             return handler(value, depth, indent, decode, leading)
         return p_def(value, indent=indent, decode=decode)
 
     if handler is not None:
         return handler(value, depth, indent, decode, leading)
     return p_type(value, indent=indent, decode=decode)
@@ -100,62 +106,66 @@
             styled_args.reverse()
             if annotations is not None:
                 for i, arg in enumerate(styled_args):
                     if arg[0] in annotations:
                         styled_args[i][1] = annotations[arg[0]]
 
         return styled_args
-
-    (
-        args,
-        varargs,
-        varkw,
-        defaults,
-        kwonlyargs,
-        kwonlydefaults,
-        annotations,
-    ) = getfullargspec(value)
-    styled_args = build_arg_data(args, defaults, annotations)
-    styled_args.extend(build_arg_data(kwonlyargs, kwonlydefaults, annotations))
-
-    if varargs is not None:
-        styled_args.append(
-            [
-                f"*{varargs}",
-                annotations[varargs] if varargs in annotations else MISSING,
-                MISSING,
-            ]
-        )
-
-    if varkw is not None:
-        styled_args.append(
-            [
-                f"**{varkw}",
-                annotations[varkw] if varkw in annotations else MISSING,
-                MISSING,
-            ]
-        )
-
-    args = []
-    for arg in styled_args:
-        args.append(p_arg(arg, decode=False))
-
-    return_annotation = signature(value).return_annotation
-    if return_annotation == _empty:
-        return_annotation = f" -> {p_none(decode=False)}"
-    else:
-        return_annotation = f" -> {p_value(return_annotation, decode=False)}"
-
-    val = f"[@F #8aadf4$]{value.__name__}[$@F]({', '.join(args)}){return_annotation}"
+    try:
+        (
+            args,
+            varargs,
+            varkw,
+            defaults,
+            kwonlyargs,
+            kwonlydefaults,
+            annotations,
+        ) = getfullargspec(value)
+
+        styled_args = build_arg_data(args, defaults, annotations)
+        styled_args.extend(build_arg_data(kwonlyargs, kwonlydefaults, annotations))
+
+        if varargs is not None:
+            styled_args.append(
+                [
+                    f"*{varargs}",
+                    annotations[varargs] if varargs in annotations else MISSING,
+                    MISSING,
+                ]
+            )
+
+        if varkw is not None:
+            styled_args.append(
+                [
+                    f"**{varkw}",
+                    annotations[varkw] if varkw in annotations else MISSING,
+                    MISSING,
+                ]
+            )
+
+        args = []
+        for arg in styled_args:
+            args.append(p_arg(arg, decode=False))
+
+        return_annotation = signature(value).return_annotation
+        if return_annotation == _empty:
+            return_annotation = f" -> {p_none(decode=False)}"
+        else:
+            return_annotation = f" -> {p_value(return_annotation, decode=False)}"
+
+        val = f"[@F #8aadf4$]{value.__name__}[$@F]({', '.join(args)}){return_annotation}"
+    except:
+        val = f"[@F red]{_type(value).__name__}()[@F]"
     if decode:
         return SAIML.parse(val)
     return val
 
 
 def p_arg(value: tuple[str, Any, Any], indent: int = 0, decode: bool = True):
+    _type = ""
     if isinstance(value[1], (GenericAlias, UnionType, str)):
         _type = (
             f": [@F#f5a97f]{SAIML.escape(str(value[1]))}[@F]" if not isinstance(value[1], Missing) else ""
         )
     elif isinstance(value[1], type):
         _type = f": [$]{p_value(value[1], decode=False)}[$]"
 
@@ -174,30 +184,35 @@
     val = f"{' '*indent}[@F#f5bde6$]{value[0]}[$@F]{_type}{_default}"
     
     if decode:
         return SAIML.parse(val)
     return val
 
 
-def p_type(value: bool, indent: int = 0, decode: bool = True) -> str:
+def p_type(value: type, indent: int = 0, decode: bool = True) -> str:
     """Construct an ansi encoded colored bool str.
 
     Args:
         value (bool): The bool to encode.
         indent (int): The amount of spaces added to the prefix of the value.
         decode (bool): Whether to decode SAIML markup string to ansi.
 
     Returns:
         `[@F #f5a97f]{value}` == `\\x1b[38;5;147m{value}\\x1b[0m`
     """
 
-    if isinstance(type(value), type):
-        val = f"[@F #f5a97f]{SAIML.escape(value.__name__)}[@F]"
+    if isinstance(value, type):
+        val = f"[@F #f5a97f $]{SAIML.escape(_type(value).__name__)}[@F $]"
     else:
-        val = f"[@F #f5a97f]{SAIML.escape(type(value).__name__)}[@F]"
+        if hasattr(value, "__repr__"):
+            val = f"[$]{value!r}[$]"
+        elif hasattr(value, "__str__"):
+            val = f"[$]{value}[$]"
+        else:
+            val = f"[@F #f5a97f $]{SAIML.escape(type(value).__name__)}[@F $]"
 
     if decode:
         return SAIML.parse(val)
     return val
 
 
 def p_dict(
```

### Comparing `saimll-0.5.0/saimll/logger/LogLevel.py` & `saimll-0.5.1/saimll/logger/LogLevel.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/saimll/logger/encoding.py` & `saimll-0.5.1/saimll/logger/encoding.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/saimll/logger/log.py` & `saimll-0.5.1/saimll/logger/log.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/saimll/saiml/__init__.py` & `saimll-0.5.1/saimll/saiml/__init__.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/saimll/saiml/color/__init__.py` & `saimll-0.5.1/saimll/saiml/color/__init__.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/saimll/saiml/color/colors.py` & `saimll-0.5.1/saimll/saiml/color/colors.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/saimll/saiml/color/xterm_colors.py` & `saimll-0.5.1/saimll/saiml/color/xterm_colors.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/saimll/saiml/markup/formatting.py` & `saimll-0.5.1/saimll/saiml/markup/formatting.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/saimll/saiml/markup/markup.py` & `saimll-0.5.1/saimll/saiml/markup/markup.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/saimll/saiml/markup/tokens.py` & `saimll-0.5.1/saimll/saiml/markup/tokens.py`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/LICENSE` & `saimll-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/README.md` & `saimll-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `saimll-0.5.0/pyproject.toml` & `saimll-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "saimll"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
     { name="Tired Fox", email="zboehm104@gmail.com"}
 ]
 description="Simple Inline Markup Language and Logging"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
```

### Comparing `saimll-0.5.0/PKG-INFO` & `saimll-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saimll
-Version: 0.5.0
+Version: 0.5.1
 Summary: Simple Inline Markup Language and Logging
 Project-URL: Homepage, https://github.com/Tired-Fox/saimll
 Project-URL: Documentation, https://tired-fox.github.io/saimll
 Author-email: Tired Fox <zboehm104@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

