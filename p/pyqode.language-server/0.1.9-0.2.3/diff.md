# Comparing `tmp/pyqode.language_server-0.1.9.tar.gz` & `tmp/pyqode.language-server-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqode.language_server-0.1.9.tar", last modified: Thu Jan 21 15:23:50 2021, max compression
+gzip compressed data, was "pyqode.language-server-0.2.3.tar", last modified: Tue Apr 18 14:34:50 2023, max compression
```

## Comparing `pyqode.language_server-0.1.9.tar` & `pyqode.language-server-0.2.3.tar`

### file list

```diff
@@ -1,32 +1,13 @@
-drwxrwxr-x   0 sebastiaan  (1000) sebastiaan  (1000)        0 2021-01-21 15:23:50.383225 pyqode.language_server-0.1.9/
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      144 2020-12-22 12:40:05.000000 pyqode.language_server-0.1.9/AUTHORS.rst
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)     1089 2020-12-22 12:40:28.000000 pyqode.language_server-0.1.9/LICENSE
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      186 2021-01-06 18:40:29.000000 pyqode.language_server-0.1.9/MANIFEST.in
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)     1415 2021-01-21 15:23:50.383225 pyqode.language_server-0.1.9/PKG-INFO
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      989 2020-12-22 12:38:33.000000 pyqode.language_server-0.1.9/README.rst
-drwxrwxr-x   0 sebastiaan  (1000) sebastiaan  (1000)        0 2021-01-21 15:23:50.379225 pyqode.language_server-0.1.9/pyqode/
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      204 2020-12-13 10:37:04.000000 pyqode.language_server-0.1.9/pyqode/__init__.py
-drwxrwxr-x   0 sebastiaan  (1000) sebastiaan  (1000)        0 2021-01-21 15:23:50.379225 pyqode.language_server-0.1.9/pyqode/language_server/
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      151 2021-01-21 15:22:13.000000 pyqode.language_server-0.1.9/pyqode/language_server/__init__.py
-drwxrwxr-x   0 sebastiaan  (1000) sebastiaan  (1000)        0 2021-01-21 15:23:50.383225 pyqode.language_server-0.1.9/pyqode/language_server/backend/
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      256 2020-12-13 10:39:40.000000 pyqode.language_server-0.1.9/pyqode/language_server/backend/__init__.py
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)     1232 2021-01-15 09:29:09.000000 pyqode.language_server-0.1.9/pyqode/language_server/backend/server.py
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)    14941 2021-01-21 15:21:54.000000 pyqode.language_server-0.1.9/pyqode/language_server/backend/workers.py
-drwxrwxr-x   0 sebastiaan  (1000) sebastiaan  (1000)        0 2021-01-21 15:23:50.383225 pyqode.language_server-0.1.9/pyqode/language_server/modes/
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      395 2020-12-25 12:32:54.000000 pyqode.language_server-0.1.9/pyqode/language_server/modes/__init__.py
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)     2770 2020-12-27 15:15:05.000000 pyqode.language_server-0.1.9/pyqode/language_server/modes/calltips.py
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)     2471 2020-12-31 15:40:43.000000 pyqode.language_server-0.1.9/pyqode/language_server/modes/diagnostics.py
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      793 2020-12-25 12:28:05.000000 pyqode.language_server-0.1.9/pyqode/language_server/modes/language_server_mode.py
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      674 2021-01-06 18:52:24.000000 pyqode.language_server-0.1.9/pyqode/language_server/modes/symbols.py
-drwxrwxr-x   0 sebastiaan  (1000) sebastiaan  (1000)        0 2021-01-21 15:23:50.379225 pyqode.language_server-0.1.9/pyqode.language_server.egg-info/
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)     1415 2021-01-21 15:23:50.000000 pyqode.language_server-0.1.9/pyqode.language_server.egg-info/PKG-INFO
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      808 2021-01-21 15:23:50.000000 pyqode.language_server-0.1.9/pyqode.language_server.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)        1 2021-01-21 15:23:50.000000 pyqode.language_server-0.1.9/pyqode.language_server.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)        7 2021-01-21 15:23:50.000000 pyqode.language_server-0.1.9/pyqode.language_server.egg-info/namespace_packages.txt
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)        1 2020-12-13 11:16:58.000000 pyqode.language_server-0.1.9/pyqode.language_server.egg-info/not-zip-safe
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)       14 2021-01-21 15:23:50.000000 pyqode.language_server-0.1.9/pyqode.language_server.egg-info/requires.txt
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)        7 2021-01-21 15:23:50.000000 pyqode.language_server-0.1.9/pyqode.language_server.egg-info/top_level.txt
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)      121 2021-01-21 15:23:50.383225 pyqode.language_server-0.1.9/setup.cfg
--rw-rw-r--   0 sebastiaan  (1000) sebastiaan  (1000)     2174 2020-12-29 11:34:20.000000 pyqode.language_server-0.1.9/setup.py
-drwxrwxr-x   0 sebastiaan  (1000) sebastiaan  (1000)        0 2021-01-21 15:23:50.383225 pyqode.language_server-0.1.9/test/
--rw-r--r--   0 sebastiaan  (1000) sebastiaan  (1000)       28 2020-12-29 11:33:00.000000 pyqode.language_server-0.1.9/test/test_dummy.py
+-rw-r--r--   0        0        0     1089 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/LICENSE
+-rw-r--r--   0        0        0      989 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/README.rst
+-rw-r--r--   0        0        0      585 2023-04-18 14:34:43.731439 pyqode.language-server-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      151 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/pyqode/language_server/__init__.py
+-rw-r--r--   0        0        0      256 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/pyqode/language_server/backend/__init__.py
+-rw-r--r--   0        0        0     1232 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/pyqode/language_server/backend/server.py
+-rw-r--r--   0        0        0    15744 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/pyqode/language_server/backend/workers.py
+-rw-r--r--   0        0        0      395 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/pyqode/language_server/modes/__init__.py
+-rw-r--r--   0        0        0     1400 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/pyqode/language_server/modes/calltips.py
+-rw-r--r--   0        0        0     2587 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/pyqode/language_server/modes/diagnostics.py
+-rw-r--r--   0        0        0      787 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/pyqode/language_server/modes/language_server_mode.py
+-rw-r--r--   0        0        0      674 2023-04-18 14:34:35.998959 pyqode.language-server-0.2.3/pyqode/language_server/modes/symbols.py
+-rw-r--r--   0        0        0     1459 1970-01-01 00:00:00.000000 pyqode.language-server-0.2.3/PKG-INFO
```

### Comparing `pyqode.language_server-0.1.9/LICENSE` & `pyqode.language-server-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqode.language_server-0.1.9/README.rst` & `pyqode.language-server-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyqode.language_server-0.1.9/pyqode/language_server/backend/server.py` & `pyqode.language-server-0.2.3/pyqode/language_server/backend/server.py`

 * *Files identical despite different names*

### Comparing `pyqode.language_server-0.1.9/pyqode/language_server/backend/workers.py` & `pyqode.language-server-0.2.3/pyqode/language_server/backend/workers.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,19 @@
     CompletionTriggerKind,
     CompletionItemKind,
     DiagnosticSeverity,
     VersionedTextDocumentIdentifier,
     TextDocumentContentChangeEvent,
 )
 
+try:
+    BrokenPipeError
+except NameError:
+    BrokenPipeError = Exception  # For Python 2
+
 WARNING = 1
 ERROR = 2
 ICON_PATH = ('path', ':/pyqode_python_icons/rc/path.png')
 ICON_CLASS = ('code-class', ':/pyqode_python_icons/rc/class.png')
 ICON_FUNC = ('code-function', ':/pyqode_python_icons/rc/func.png')
 ICON_VAR = ('code-variable', ':/pyqode_python_icons/rc/var.png')
 ICON_KEYWORD = ('quickopen', ':/pyqode_python_icons/rc/keyword.png')
@@ -54,31 +59,38 @@
 diagnostics = {}  # Set by on_publish_diagnostics
 # Maintains opened documents as path => version mappings. The empty string is
 # used as the path for new (unsaved) documents.
 open_documents = {'': 0}
 _, tmp_path = tempfile.mkstemp('pyqode.language_server')
 
 
-def start_language_server(cmd, folders):
+def start_language_server(cmd, folders, shell=False):
     """Starts the language server and waits for initialization to complete."""
     
     global client, server_process, server_cmd, server_status, project_folders
     global server_capabilities
 
     print('starting language server: "{}"'.format(cmd))
     try:
         server_process = subprocess.Popen(
             shlex.split(cmd),
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
-            shell=False  # Otherwise the binary may not be found on Windows
+            shell=shell
         )
     except FileNotFoundError as e:
         print('failed to start language server: {}"'.format(e))
+        if not shell:
+            # If the language server cannot be found, then perhaps trying 
+            # through the shell works, because that way it can make use of
+            # paths etc.
+            print('retrying through shell')
+            start_language_server(cmd, folders, shell=True)
+            return
         server_status = SERVER_ERROR
         return
     server_status = SERVER_RUNNING
     json_rpc_endpoint = JsonRpcEndpoint(
         server_process.stdin,
         server_process.stdout
     )
@@ -97,15 +109,15 @@
             rootPath=None,
             rootUri=None if not project_folders else project_folders[0],
             initializationOptions=None,
             capabilities=CLIENT_CAPABILITIES,
             trace='off',
             workspaceFolders=None if not project_folders else project_folders
         )
-    except (lsp_structs.ResponseError, TimeoutError) as e:
+    except (lsp_structs.ResponseError, TimeoutError, BrokenPipeError) as e:
         print('failed to initialize language server: {}'.format(e))
         server_status = SERVER_ERROR
         return
     client.initialized()
     server_cmd = cmd
     print(server_capabilities)
     print('project_folders {}'.format(project_folders))
@@ -310,16 +322,18 @@
         print('completions gave {} suggestions'.format(len(matches)))
         return [match.to_dict() for match in matches]
     
     
 def on_publish_diagnostics(d):
     """Is called by the server when diagnostic info is available."""
     
-    global diagnostics
-    diagnostics = d
+    msg = d.get('diagnostics', [])
+    uri = d.get('uri', None)
+    print('publishing diagnostic {} messages for {}'.format(len(msg), uri))
+    diagnostics[uri] = d
 
 
 def run_diagnostics(request_data):
     """Sends a didOpen or didChange to the server to start a diagnostic check.
     Immediately returns information about the server status, but the actual
     diagnostics messages are returned by poll_diagnostics() to avoid
     diagnostics from blocking the server.
@@ -328,17 +342,18 @@
     global diagnostics
     if server_status != SERVER_RUNNING:
         return {
             'server_status': server_status,
             'server_pid': None,
             'server_capabilities': {}
         }
-    diagnostics = {}
     path = request_data['path']
-    if path in open_documents and False:
+    print('opening  {}'.format(path))
+    diagnostics[_path_to_uri(path)] = {}  # reset diagnostics for this file
+    if path in open_documents:
         client.didChange(
             _text_identifier(**request_data),
             [_everything_changed(**request_data)]
         )
     else:
         open_documents[path] = 0
         client.didOpen(_text_document(**request_data))
@@ -348,32 +363,36 @@
         'server_capabilities': server_capabilities
     }
 
 
 def poll_diagnostics(request_data):
     """Returns diagnostic messages if they are available."""
     
-    if not diagnostics:
+    uri = _path_to_uri(request_data['path'])
+    d = diagnostics.get(uri)
+    if not d:
         return [None]
     ignore_rules = request_data['ignore_rules']
-    d = diagnostics.get('diagnostics', [])
     ret_val = []
-    for msg in d:
+    for msg in d.get('diagnostics', []):
         if any(msg['message'].startswith(ir) for ir in ignore_rules):
             continue
         ret_val.append((
             msg['message'],
             ERROR if msg['severity'] <= DiagnosticSeverity.Error else WARNING,
             msg['range']['start']['line'],
             (
                 msg['range']['start']['character'],
                 msg['range']['end']['character']
             )
         ))
-    print('{} diagnostic messages'.format(len(ret_val)))
+    print('polling {} diagnostic messages for {}'.format(
+        len(ret_val),
+        format(uri))
+    )
     return ret_val
 
 
 def close_document(request_data):
     """Sends a didClose to the server to indicate that the document was closed
     in the client.
     """
@@ -436,14 +455,16 @@
 
 def _run_command(name, fnc, args):
     """Sends a command to the server and returns the response. If a
     ResponseError occurs, None is returned. If a TimeoutError occurs, None is
     also returned, and the server is restarted (because it may be hanging).
     """
     
+    if server_status != SERVER_RUNNING:
+        print('{} not performed because server not running'.format(name))
     with _timer(name):
         try:
             ret_val = fnc(*args)
         except lsp_structs.ResponseError as e:
             print('{}() gave ResponseError'.format(name))
             print(str(e))
             ret_val = None
```

### Comparing `pyqode.language_server-0.1.9/pyqode/language_server/modes/diagnostics.py` & `pyqode.language-server-0.2.3/pyqode/language_server/modes/diagnostics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 This module contains the LSP diagnostics checker mode
 """
 from pyqode.core.modes import CheckerMode
-from pyqode.qt.QtCore import Signal, QTimer
+from qtpy.QtCore import Signal, QTimer
 from pyqode.language_server.backend.workers import (
     run_diagnostics,
     poll_diagnostics
 )
 
 
 class DiagnosticsMode(CheckerMode):
@@ -31,23 +31,27 @@
             return
         super()._on_work_finished(results)
         
     def _poll_messages(self):
 
         self.editor.backend.send_request(
             poll_diagnostics,
-            {'ignore_rules': self.ignore_rules},
+            {
+                'path': self.editor.file.path,
+                'ignore_rules': self.ignore_rules
+            },
             on_receive=self._on_poll_result
         )
         
     def _on_work_finished(self, results):
         
         # Check if the result is valid
         if not isinstance(results, dict) or 'server_status' not in results:
             return
+        # Check if the server status changed
         if results['server_status'] != self._last_server_status:
             self.server_status_changed.emit(
                 results['server_status'],
                 results['server_pid'],
                 results['server_capabilities']
             )
             self._set_completion_triggers(results['server_capabilities'])
@@ -63,8 +67,8 @@
         if 'CodeCompletionMode' not in self.editor.modes.keys():
             return
         trigger_symbols = capabilities.get('capabilities', {}) \
             .get('completionProvider', {}) \
             .get('triggerCharacters', [])
         self.editor.modes.get(
             'CodeCompletionMode'
-        ).trigger_symbols = trigger_symbols
+        ).trigger_symbols = trigger_symbols
```

### Comparing `pyqode.language_server-0.1.9/pyqode/language_server/modes/language_server_mode.py` & `pyqode.language-server-0.2.3/pyqode/language_server/modes/language_server_mode.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding=utf-8
 """
 A base class for language-server modes.
 """
 import time
 from pyqode.core.api import Mode
-from pyqode.qt import QtCore
+from qtpy import QtCore
 
 
 REQUEST_TIMEOUT = 5
 
 
 class LanguageServerMode(Mode):
 
@@ -27,8 +27,8 @@
             QtCore.QCoreApplication.processEvents()
         else:
             return []
         return self._results
         
     def _on_results_available(self, results):
         
-        self._results = results
+        self._results = results
```

### Comparing `pyqode.language_server-0.1.9/pyqode/language_server/modes/symbols.py` & `pyqode.language-server-0.2.3/pyqode/language_server/modes/symbols.py`

 * *Files identical despite different names*

