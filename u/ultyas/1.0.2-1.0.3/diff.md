# Comparing `tmp/ultyas-1.0.2.tar.gz` & `tmp/ultyas-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultyas-1.0.2.tar", last modified: Wed Apr  5 02:16:14 2023, max compression
+gzip compressed data, was "ultyas-1.0.3.tar", last modified: Tue Apr 18 15:48:07 2023, max compression
```

## Comparing `ultyas-1.0.2.tar` & `ultyas-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-04-05 02:16:14.591855 ultyas-1.0.2/
--rw-r--r--   0 work      (1000) work      (1000)     1969 2023-04-05 02:16:14.591855 ultyas-1.0.2/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)      713 2023-04-05 02:02:16.000000 ultyas-1.0.2/README.md
--rw-r--r--   0 work      (1000) work      (1000)       38 2023-04-05 02:16:14.591855 ultyas-1.0.2/setup.cfg
--rwxr-xr-x   0 work      (1000) work      (1000)     1558 2023-04-05 02:13:24.000000 ultyas-1.0.2/setup.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-04-05 02:16:14.591855 ultyas-1.0.2/ultyas/
--rw-r--r--   0 work      (1000) work      (1000)     3564 2023-04-05 01:58:59.000000 ultyas-1.0.2/ultyas/__init__.py
--rw-r--r--   0 work      (1000) work      (1000)     4517 2023-04-05 01:33:33.000000 ultyas-1.0.2/ultyas/ultisnips.py
-drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-04-05 02:16:14.591855 ultyas-1.0.2/ultyas.egg-info/
--rw-r--r--   0 work      (1000) work      (1000)     1969 2023-04-05 02:16:14.000000 ultyas-1.0.2/ultyas.egg-info/PKG-INFO
--rw-r--r--   0 work      (1000) work      (1000)      210 2023-04-05 02:16:14.000000 ultyas-1.0.2/ultyas.egg-info/SOURCES.txt
--rw-r--r--   0 work      (1000) work      (1000)        1 2023-04-05 02:16:14.000000 ultyas-1.0.2/ultyas.egg-info/dependency_links.txt
--rw-r--r--   0 work      (1000) work      (1000)       67 2023-04-05 02:16:14.000000 ultyas-1.0.2/ultyas.egg-info/entry_points.txt
--rw-r--r--   0 work      (1000) work      (1000)        7 2023-04-05 02:16:14.000000 ultyas-1.0.2/ultyas.egg-info/top_level.txt
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-04-18 15:48:07.642502 ultyas-1.0.3/
+-rw-r--r--   0 work      (1000) work      (1000)       26 2023-04-18 14:41:15.000000 ultyas-1.0.3/.gitignore
+-rw-r--r--   0 work      (1000) work      (1000)    35149 2023-04-04 03:13:38.000000 ultyas-1.0.3/LICENSE
+-rw-r--r--   0 work      (1000) work      (1000)     1735 2023-04-18 15:48:07.642502 ultyas-1.0.3/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)      713 2023-04-18 14:41:15.000000 ultyas-1.0.3/README.md
+-rw-r--r--   0 work      (1000) work      (1000)       38 2023-04-18 15:48:07.642502 ultyas-1.0.3/setup.cfg
+-rwxr-xr-x   0 work      (1000) work      (1000)     1558 2023-04-18 15:46:36.000000 ultyas-1.0.3/setup.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-04-18 15:48:07.642502 ultyas-1.0.3/ultyas/
+-rw-r--r--   0 work      (1000) work      (1000)     4574 2023-04-18 15:43:19.000000 ultyas-1.0.3/ultyas/__init__.py
+-rw-r--r--   0 work      (1000) work      (1000)     4730 2023-04-18 15:42:26.000000 ultyas-1.0.3/ultyas/ultisnips.py
+drwxr-xr-x   0 work      (1000) work      (1000)        0 2023-04-18 15:48:07.642502 ultyas-1.0.3/ultyas.egg-info/
+-rw-r--r--   0 work      (1000) work      (1000)     1735 2023-04-18 15:48:07.000000 ultyas-1.0.3/ultyas.egg-info/PKG-INFO
+-rw-r--r--   0 work      (1000) work      (1000)      229 2023-04-18 15:48:07.000000 ultyas-1.0.3/ultyas.egg-info/SOURCES.txt
+-rw-r--r--   0 work      (1000) work      (1000)        1 2023-04-18 15:48:07.000000 ultyas-1.0.3/ultyas.egg-info/dependency_links.txt
+-rw-r--r--   0 work      (1000) work      (1000)       66 2023-04-18 15:48:07.000000 ultyas-1.0.3/ultyas.egg-info/entry_points.txt
+-rw-r--r--   0 work      (1000) work      (1000)        7 2023-04-18 15:48:07.000000 ultyas-1.0.3/ultyas.egg-info/top_level.txt
```

### Comparing `ultyas-1.0.2/README.md` & `ultyas-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ultyas-1.0.2/setup.py` & `ultyas-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 CURRENT_DIRECTORY = Path(__file__).parent.resolve()
 LONG_DESCRIPTION = \
     (CURRENT_DIRECTORY / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ultyas",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
     description=("A tool for converting code snippets from "
                  "Ultisnips to YASnippet format"),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/ultyas",
     author="James Cherti",
```

### Comparing `ultyas-1.0.2/ultyas/__init__.py` & `ultyas-1.0.3/ultyas/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 import argparse
 from pathlib import Path
 
 from .ultisnips import UltisnipsSnippetsFile, UltisnipsParseError
 
 
 def parse_args():
-    usage = ("%(prog)s <ultisnips-file> -o <yasnippet-major-mode-dir>")
+    usage = ("%(prog)s <file.snippets> "
+             "-o <yasnippet-major-mode-dir>")
     parser = argparse.ArgumentParser(
         description=("A command-line tool for converting code snippets "
                      "from Ultisnips to YASnippet format."),
         usage=usage,
     )
 
     parser.add_argument(
@@ -45,19 +46,44 @@
         "'~/.vim/UltiSnips/python.snippets')",
     )
 
     parser.add_argument(
         "-o",
         "--yasnippet-dir",
         required=True,
-        help="The directory of the major mode YASnippet snippets (e.g. "
+        help="The YASnippet snippets major mode directory (e.g. "
         "'~/.emacs.d/snippets/python-mode/')"
     )
 
     parser.add_argument(
+        "-i",
+        "--yas-indent-line",
+        default="nothing",
+        choices=["auto", "fixed", "nothing"],
+        required=False,
+        help=("Add one of the following comments to the "
+              "YASnippet snippets that will be generated: "
+              "\"# expand-env: ((yas-indent-line 'fixed))\" or "
+              "\"# expand-env: ((yas-indent-line 'auto))\". "
+              "For information on 'yas-indent-line', visit: "
+              "https://joaotavora.github.io/yasnippet/snippet-reference.html"
+              "#yas-indent-line"),
+    )
+
+    parser.add_argument(
+        "-t",
+        "--convert-tabs-to",
+        default="$>",
+        required=False,
+        help=("Convert the tabs that are in the generated snippets to "
+              "the string passed to this option "
+              "(Default: The indentation marker '$>')"),
+    )
+
+    parser.add_argument(
         "-m",
         "--mkdir",
         default=False,
         action="store_true",
         required=False,
         help="Ensure that the directory passed to "
         "the --yasnippet-dir flag exists",
@@ -99,15 +125,17 @@
 
         if not os.path.isdir(yasnippet_dir):
             print(f"Error: The directory does not exist: {yasnippet_dir}",
                   file=sys.stderr)
             sys.exit(1)
 
         list_yasnippet_files = ultisnips_snippet.convert_to_yasnippet(
-            yasnippet_dir,
+            directory=yasnippet_dir,
+            convert_tabs_to=args.convert_tabs_to,
+            yas_indent_line=args.yas_indent_line,
         )
 
         if not args.quiet:
             if args.verbose:
                 for yasnippet_file in list_yasnippet_files:
                     print(yasnippet_file)
```

### Comparing `ultyas-1.0.2/ultyas/ultisnips.py` & `ultyas-1.0.3/ultyas/ultisnips.py`

 * *Files 10% similar despite different names*

```diff
@@ -94,30 +94,37 @@
                 if line_strip != "":
                     line = line.rstrip("\n")
                     err = f"{snippet_file}: {line_num}: '{line}'"
                     raise UltisnipsParseError(err)
 
     def convert_to_yasnippet(self,
                              directory: os.PathLike,
-                             convert_tab_to: str = "$>") -> List[str]:
-        header_expand_fixed = "# expand-env: ((yas-indent-line 'fixed))\n" \
-            if convert_tab_to == "$>" else ""
+                             convert_tabs_to: str = "$>",
+                             yas_indent_line: str = "") -> List[str]:
+        if yas_indent_line and yas_indent_line not in ("auto", "fixed"):
+            yas_indent_line = ""
+
+        comment_yas_indent_line = (
+            f"# expand-env: ((yas-indent-line '{yas_indent_line}))\n"
+            if yas_indent_line
+            else ""
+        )
 
         result = []
         for snippet_name, snippet_data in self.snippets.items():
             snippet_path = Path(directory).joinpath(snippet_name)
             result.append(str(snippet_path))
 
             header = ("# -*- mode: snippet -*-\n"
                       f"# name: {snippet_name}\n"
                       f"# key: {snippet_name}\n"  # Used to expand
-                      f"{header_expand_fixed}"
+                      f"{comment_yas_indent_line}"
                       "# --\n")
             content = ((header + snippet_data.content.rstrip("\n"))
-                       .replace("\t", convert_tab_to))
+                       .replace("\t", convert_tabs_to))
             if snippet_path.is_file():
                 content_md5sum = hashlib.md5(content.encode()).hexdigest()
                 if content_md5sum == md5sum_file(snippet_path):
                     continue
 
             with open(snippet_path, "w", encoding="utf-8") as fhandler:
                 fhandler.write(content)
```

