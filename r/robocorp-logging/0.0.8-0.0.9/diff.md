# Comparing `tmp/robocorp_logging-0.0.8.tar.gz` & `tmp/robocorp_logging-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_logging-0.0.8.tar", max compression
+gzip compressed data, was "robocorp_logging-0.0.9.tar", max compression
```

## Comparing `robocorp_logging-0.0.8.tar` & `robocorp_logging-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0    10142 2023-04-16 13:45:02.062870 robocorp_logging-0.0.8/LICENSE
--rw-r--r--   0        0        0     1021 2023-04-16 13:45:02.062870 robocorp_logging-0.0.8/README.md
--rw-r--r--   0        0        0      985 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    13205 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/__init__.py
--rw-r--r--   0        0        0     8413 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_ast_utils.py
--rw-r--r--   0        0        0     4215 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_auto_logging_setup.py
--rw-r--r--   0        0        0     2697 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_config.py
--rw-r--r--   0        0        0      572 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_convert_units.py
--rw-r--r--   0        0        0     6272 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_decoder.py
--rw-r--r--   0        0        0     1863 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_lifecycle_hooks.py
--rw-r--r--   0        0        0      493 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_logger_instances.py
--rw-r--r--   0        0        0    11599 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_rewrite_ast_add_callbacks.py
--rw-r--r--   0        0        0    10726 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_rewrite_filtering.py
--rw-r--r--   0        0        0    12211 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_rewrite_importhook.py
--rw-r--r--   0        0        0     8346 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_robo_logger.py
--rw-r--r--   0        0        0    48506 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/_robo_output_impl.py
--rw-r--r--   0        0        0    41588 2023-04-16 13:45:50.456683 robocorp_logging-0.0.8/src/robo_log/index.py
--rw-r--r--   0        0        0    46346 2023-04-16 13:45:53.320789 robocorp_logging-0.0.8/src/robo_log/index_v2.py
--rw-r--r--   0        0        0      511 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/protocols.py
--rw-r--r--   0        0        0        0 2023-04-16 13:45:02.070870 robocorp_logging-0.0.8/src/robo_log/py.typed
--rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 robocorp_logging-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-04-18 19:05:04.200318 robocorp_logging-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1021 2023-04-18 19:05:04.200318 robocorp_logging-0.0.9/README.md
+-rw-r--r--   0        0        0      987 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    15806 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/__init__.py
+-rw-r--r--   0        0        0     8413 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_ast_utils.py
+-rw-r--r--   0        0        0     5624 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_auto_logging_setup.py
+-rw-r--r--   0        0        0     4909 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_config.py
+-rw-r--r--   0        0        0      572 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_convert_units.py
+-rw-r--r--   0        0        0     6284 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_decoder.py
+-rw-r--r--   0        0        0    41877 2023-04-18 19:06:01.454442 robocorp_logging-0.0.9/src/robo_log/_index.py
+-rw-r--r--   0        0        0    51888 2023-04-18 19:06:04.630558 robocorp_logging-0.0.9/src/robo_log/_index_v2.py
+-rw-r--r--   0        0        0     1977 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0      493 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_logger_instances.py
+-rw-r--r--   0        0        0      385 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_obj_info_repr.py
+-rw-r--r--   0        0        0    13226 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0     8900 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12246 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_rewrite_importhook.py
+-rw-r--r--   0        0        0     8732 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_robo_logger.py
+-rw-r--r--   0        0        0    48935 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/_robo_output_impl.py
+-rw-r--r--   0        0        0      511 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/protocols.py
+-rw-r--r--   0        0        0        0 2023-04-18 19:05:04.208319 robocorp_logging-0.0.9/src/robo_log/py.typed
+-rw-r--r--   0        0        0     1509 1970-01-01 00:00:00.000000 robocorp_logging-0.0.9/PKG-INFO
```

### Comparing `robocorp_logging-0.0.8/LICENSE` & `robocorp_logging-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.8/README.md` & `robocorp_logging-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.8/pyproject.toml` & `robocorp_logging-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "robocorp-logging"
-version = "0.0.8"
+version = "0.0.9"
 description = "Automatic trace logging for Python"
 authors = [
     "Fabio Z. <fabio@robocorp.com>",
     "Ossi R. <ossi@robocorp.com>",
     "Kerkko P. <kerkko@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robo_log", from = "src"}]
-include = ["**/index.py", "**/index_v2.py"]
+include = ["**/_index.py", "**/_index_v2.py"]
 
 [tool.mypy]
 mypy_path = "logging/src:logging/tests"
 
 [[tool.mypy.overrides]]
 module = "setuptools.*"
 ignore_missing_imports = true
```

### Comparing `robocorp_logging-0.0.8/src/robo_log/__init__.py` & `robocorp_logging-0.0.9/src/robo_log/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,26 +17,27 @@
     List,
     Sequence,
     Dict,
     Union,
     Iterable,
     Literal,
 )
-from ._config import Filter, FilterKind
 from ._logger_instances import _get_logger_instances
-from .protocols import OptExcInfo, LogHTMLStyle, Status
-from robo_log.protocols import IReadLines
+from .protocols import OptExcInfo, LogHTMLStyle, Status, IReadLines
+
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
-    from ._rewrite_filtering import FilesFiltering
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 version_info = [int(x) for x in __version__.split(".")]
 
+# --- Make these a part of the public API.
+from ._config import Filter, FilterKind, BaseConfig, ConfigFilesFiltering
+
 
 # --- Logging methods for custom messaging.
 
 
 def _log(level, message: str, html: bool = False) -> None:
     back_frame = sys._getframe(2)
     source = back_frame.f_code.co_filename
@@ -98,14 +99,18 @@
 # --- Methods related to hiding logging information.
 
 
 @contextmanager
 def stop_logging_methods():
     """
     Can be used so that method calls are no longer logged.
+
+    i.e.:
+        with stop_logging_methods():
+            ...
     """
     for robo_logger in _get_logger_instances():
         robo_logger.stop_logging_methods()
     try:
         yield
     finally:
         start_logging_methods()
@@ -122,15 +127,19 @@
     for robo_logger in _get_logger_instances():
         robo_logger.start_logging_methods()
 
 
 @contextmanager
 def stop_logging_variables():
     """
-    Can be used so that variables are no longer logged.
+    Can be used (as a context manager) so that variables are no longer logged.
+
+    i.e.:
+        with stop_logging_variables():
+            ...
     """
     for robo_logger in _get_logger_instances():
         robo_logger.stop_logging_variables()
 
     try:
         yield
     finally:
@@ -149,16 +158,16 @@
         robo_logger.start_logging_variables()
 
 
 def hide_from_output(string_to_hide: str) -> None:
     """
     Should be called to hide sensitive information from appearing in the output.
 
-    :param string_to_hide:
-        The string that should be hidden from the output.
+    Args:
+        string_to_hide: The string that should be hidden from the output.
     """
     for robo_logger in _get_logger_instances():
         robo_logger.hide_from_output(string_to_hide)
 
 
 # --- Logging methods usually called automatically from the framework.
 
@@ -183,18 +192,19 @@
 def end_task(name: str, libname: str, status: str, message: str) -> None:
     for robo_logger in _get_logger_instances():
         robo_logger.end_task(name, libname, status, message)
 
 
 def iter_decoded_log_format_from_stream(stream: IReadLines) -> Iterator[dict]:
     """
-    :param stream:
-        The stream which should be iterated in (anything with a `readlines()` method).
+    Args:
+        stream: The stream which should be iterated in (anything with a
+            `readlines()` method).
 
-    :returns:
+    Returns:
         An iterator which will decode the messages and provides a dictionary for
         each message found.
 
         Example of messages provided:
 
         {'message_type': 'V', 'version': '1'}
         {'message_type': 'T', 'initial_time': '2022-10-31T07:45:57.116'}
@@ -208,15 +218,15 @@
 
 
 def iter_decoded_log_format_from_log_html(log_html: Path) -> Iterator[dict]:
     """
     This function will read the chunks saved in the log html and provide
     an iterator which will provide the messages which were encoded into it.
 
-    :returns:
+    Returns:
         An iterator which will decode the messages and provides a dictionary for
         each message found.
 
         Example of messages provided:
 
         {'message_type': 'V', 'version': '1'}
         {'message_type': 'T', 'initial_time': '2022-10-31T07:45:57.116'}
@@ -263,19 +273,40 @@
     messages_iterator: Iterator[dict], expected: Sequence[dict]
 ) -> List[dict]:
     """
     A helper for checking that the expected messages are found in the
     given messages iterator.
 
     Args:
-        messages_iterator: An
-        expected:
+        messages_iterator: An iterator over the messages found.
+        expected: The messages wich are expected to be found. If some message
+            expected to be found is not found an AssertionError will be raised.
 
     Example:
+        verify_log_messages_from_messages_iterator(
+        messages_iterator,
+        [
+            {'message_type': 'V', 'version': '1'}
+            {'message_type': 'T', 'initial_time': '2022-10-31T07:45:57.116'}
+        ]
+
+    Note: if one of the key entries is `__check__` the value will be considered
+    a callable which should return `True` or `False` to determine if a match was
+    made.
 
+    Example:
+        verify_log_messages_from_messages_iterator(
+        messages_iterator,
+        [
+            {
+                "message_type": "T",
+                # i.e.: check for the utc timezone (+00:00) in the time.
+                "__check__": lambda msg: msg["initial_time"].endswith("+00:00"),
+            },
+        ]
     """
     expected_lst: List[dict] = list(expected)
     log_messages = list(messages_iterator)
     log_msg: dict
     for log_msg in log_messages:
         for expected_dct in expected_lst:
             for key, val in expected_dct.items():
@@ -296,100 +327,126 @@
         )
     return log_messages
 
 
 def verify_log_messages_from_decoded_str(
     s: str, expected: Sequence[dict]
 ) -> List[dict]:
+    """
+    Args:
+        s: A string with the messages already decoded (where messages are
+        separated by lines and each message is a json string to be decoded).
+        expected: The messages expected.
+
+    See: `verify_log_messages_from_messages_iterator` for more details on the
+        matching of messages.
+    """
     log_messages: List[dict] = []
     for log_msg in s.splitlines():
         log_msg_dict: dict = json.loads(log_msg.strip())
         log_messages.append(log_msg_dict)
 
     return verify_log_messages_from_messages_iterator(iter(log_messages), expected)
 
 
 def verify_log_messages_from_log_html(
     log_html: Path, expected: Sequence[dict]
 ) -> List[dict]:
+    """
+    Args:
+        log_html: The path to the log_html where messages were embedded.
+        expected: The messages expected.
+
+    See: `verify_log_messages_from_messages_iterator` for more details on the
+        matching of messages.
+    """
     iter_in = iter_decoded_log_format_from_log_html(log_html)
     return verify_log_messages_from_messages_iterator(iter_in, expected)
 
 
 def verify_log_messages_from_stream(
     stream: IReadLines, expected: Sequence[dict]
 ) -> Sequence[dict]:
+    """
+    Args:
+        stream: A stream from where the encoded messages are expected to be read
+            from.
+        expected: The messages expected.
+
+    See: `verify_log_messages_from_messages_iterator` for more details on the
+        matching of messages.
+    """
     return verify_log_messages_from_messages_iterator(
         iter_decoded_log_format_from_stream(stream), expected
     )
 
 
-def setup_auto_logging(
-    tracked_folders: Optional[Sequence[Union[Path, str]]] = None,
-    untracked_folders: Optional[Sequence[Union[Path, str]]] = None,
-    filters: Sequence[Filter] = (),
-):
+def setup_auto_logging(config: Optional[BaseConfig] = None):
     """
-    :param tracked_folders:
-        The folders which must be tracked (by default any folder in the
-        pythonpath which is not in a python-library folder).
-
-    :param untracked_folders:
-        The folders which must not be tracked (by default any folder which is a
-        python-library folder).
+    Sets up automatic logging.
 
-    :param filters:
-        Additional filters to add folders/modules to be tracked.
+    This must be called prior to actually importing the modules which should
+    be automatically logged.
 
-        i.e.:
+    Args:
+        config: The configuration specifying how modules should be automatically
+            logged.
 
-        [
-            Filter("mymodule.ignore", exclude=True, is_path=False),
-            Filter("mymodule.rpa", exclude=False, is_path=False),
-            Filter("**/check/**", exclude=True, is_path=True),
-        ]
+            If not passed, by default all files which are library files (i.e.:
+            in the python `Lib` or `site-packages`) won't be logged and all files
+            which are not library files will be fully logged.
+
+    Returns a context manager which will stop applying the auto-logging to new
+    loaded modules. Note that modules which are already being tracked won't
+    stop being tracked.
     """
-    from ._config import ConfigFilesFiltering
     from ._auto_logging_setup import register_auto_logging_callbacks
 
-    project_roots: Optional[Sequence[str]]
-    if tracked_folders:
-        project_roots = [
-            (f if isinstance(f, str) else str(f.absolute())) for f in tracked_folders
-        ]
+    use_config: BaseConfig
+    if config is None:
+        # If not passed, use default.
+        use_config = ConfigFilesFiltering()
     else:
-        project_roots = None
+        use_config = config
 
-    library_roots: Optional[Sequence[str]]
-    if untracked_folders:
-        library_roots = [
-            (f if isinstance(f, str) else str(f.absolute())) for f in untracked_folders
-        ]
-    else:
-        library_roots = None
-
-    return register_auto_logging_callbacks(
-        ConfigFilesFiltering(project_roots, library_roots, filters, set_as_global=True)
-    )
+    return register_auto_logging_callbacks(use_config)
 
 
 def add_log_output(
-    output_dir: Optional[Union[str, Path]] = None,
+    output_dir: Union[str, Path],
     max_file_size: str = "1MB",
     max_files: int = 5,
     log_html: Optional[Union[str, Path]] = None,
     log_html_style: LogHTMLStyle = "standalone",
 ):
+    """
+    Adds a log output which will write the contents to the given output
+    directory. Optionally it's possible to collect all the output when the run
+    is finished and put it into a log.html file.
+
+    Args:
+        output_dir: The output directory where the log contents should be saved.
+        max_file_size: The maximum file size for one log file.
+        max_files: The maximum amount of files which can be added (if more would
+            be needed the oldest one is erased).
+        log_html: If given this is the path (file) where the log.html contents
+            should be written (the log.html will include all the logs from the
+            run along with a viewer for such logs).
+        log_html_style: The style to be used for the log.html.
+
+    Note:
+        It's Ok to add more than one log output, but if 2 log outputs point
+        to the same directory there will be conflicts (in the future this should
+        generate an error).
+    """
     from ._robo_logger import _RoboLogger  # @Reimport
     from robo_log._auto_logging_setup import OnExitContextManager
 
-    if log_html and not output_dir:
-        raise RuntimeError(
-            "When log_html is specified, the output_dir must also be specified."
-        )
+    if not output_dir:
+        raise RuntimeError("The output directory must be specified.")
 
     logger = _RoboLogger(
         output_dir, max_file_size, max_files, log_html, log_html_style=log_html_style
     )
     _get_logger_instances()[logger] = 1
 
     def _exit():
@@ -407,14 +464,25 @@
     while _get_logger_instances():
         logger = next(iter(_get_logger_instances()))
         _get_logger_instances().pop(logger, None)
         logger.close()
 
 
 def add_in_memory_log_output(write):
+    """
+    Adds a log output which is in-memory.
+
+    Args:
+        write: A callable which will be called as `write(msg)` whenever
+        a message is sent from the logging.
+
+    Returns:
+        A context manager which can be used to automatically remove and
+        close the related logger.
+    """
     from ._robo_logger import _RoboLogger  # @Reimport
     from robo_log._auto_logging_setup import OnExitContextManager
 
     logger = _RoboLogger(__write__=write)
     _get_logger_instances()[logger] = 1
 
     def _exit():
@@ -422,17 +490,18 @@
         logger.close()
 
     return OnExitContextManager(_exit)
 
 
 # Not part of the API, used to determine whether a file is a project file
 # or a library file when running with the FilterKind.log_on_project_call kind.
-# Only set/used when setting up auto-logging (changed at runtime).
-def _in_project_roots(filename: str) -> bool:
-    return False
+from robo_log._rewrite_filtering import FilesFiltering
+
+_files_filtering = FilesFiltering()
+_in_project_roots = _files_filtering.in_project_roots
 
 
 def _caller_in_project_roots() -> bool:
     try:
         return _in_project_roots(sys._getframe(2).f_code.co_filename)
     except ValueError:  # call stack is not deep enough
         return False
```

### Comparing `robocorp_logging-0.0.8/src/robo_log/_ast_utils.py` & `robocorp_logging-0.0.9/src/robo_log/_ast_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.8/src/robo_log/_convert_units.py` & `robocorp_logging-0.0.9/src/robo_log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.8/src/robo_log/_decoder.py` & `robocorp_logging-0.0.9/src/robo_log/_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import json
 from typing import Optional, List, Callable, Any, Dict, Iterator
 from robo_log.protocols import IReadLines
 
 
 class Decoder:
-    def __init__(self):
+    def __init__(self) -> None:
         self.memo: Dict[str, str] = {}
 
     def decode_message_type(self, message_type: str, message: str) -> Optional[dict]:
         handler = _MESSAGE_TYPE_INFO[message_type]
         ret = {"message_type": message_type}
         try:
             r = handler(self, message)
@@ -139,19 +139,20 @@
     "ET": _decode("status:oid, message:oid, time_delta_in_seconds:float"),
     # Start Element (some element we're tracking such as method, for, while, etc).
     "SE": _decode(
         "name:oid, libname:oid, type:oid, doc:oid, source:oid, lineno:int, time_delta_in_seconds:float",
     ),
     # End Element
     "EE": _decode("status:oid, time_delta_in_seconds:float"),
+    # Assign
+    "AS": _decode(
+        "source:oid, lineno:int, target:oid, type:oid, value:oid, time_delta_in_seconds:float"
+    ),
     # Element/method argument (name and value of the argument).
-    "EA": _decode("name:oid, value:oid"),
-    # Can appear before element (method) to note that the result will
-    # be assigned to the given name.
-    "AS": _decode("assign:oid"),
+    "EA": _decode("name:oid, type:oid, value:oid"),
     # Tag the current scope with some value.
     "TG": _decode("tag:oid"),
     # Set some time for the current scope.
     "S": _decode("start_time_delta:float"),
     # --------------------------------------------------------------- Tracebacks
     # Start traceback with the exception error message.
     # Note: it should be possible to start a traceback inside another traceback
```

### Comparing `robocorp_logging-0.0.8/src/robo_log/_lifecycle_hooks.py` & `robocorp_logging-0.0.9/src/robo_log/_lifecycle_hooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,13 +56,16 @@
 # Called as: method_return(__name__, filename, name, lineno, return_value)
 method_return = Callback()
 
 # Called as: method_except(__name__, filename, name, lineno, exc_info)
 # tp, e, tb = exc_info
 method_except = Callback()
 
+# Called as: after_assign(__name__, filename, name, lineno, assign_name, assign_value)
+after_assign = Callback()
+
 
 def iter_all_callbacks():
     yield before_method
     yield after_method
     yield method_return
     yield method_except
```

### Comparing `robocorp_logging-0.0.8/src/robo_log/_rewrite_ast_add_callbacks.py` & `robocorp_logging-0.0.9/src/robo_log/_rewrite_ast_add_callbacks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import ast
-from typing import Any, Union, List, Optional, Tuple
+from typing import Any, Union, List, Optional, Tuple, Dict, Callable
 from . import _ast_utils
 from ._config import BaseConfig, FilterKind
 
 DEBUG = False
 
 
 def is_rewrite_disabled(docstring: str) -> bool:
@@ -45,21 +45,21 @@
             class_name = parent.name + "."
     except StopIteration:
         pass
 
     return function, class_name
 
 
-def _rewrite_return(function, class_name, node) -> Optional[list]:
+def _rewrite_return(function, class_name, node: ast.Return) -> Optional[list]:
     if function.name.startswith("_"):
         return None
 
     factory = _ast_utils.NodeFactory(node.lineno, node.col_offset)
 
-    result: list = []
+    result: List[ast.stmt] = []
 
     call = factory.Call()
     call.func = factory.NameLoadRewriteCallback("method_return")
     call.args.append(factory.NameLoad("__name__"))
     call.args.append(factory.NameLoad("__file__"))
     call.args.append(factory.Str(f"{class_name}{function.name}"))
     call.args.append(factory.LineConstant())
@@ -78,14 +78,35 @@
         call.args.append(factory.NoneConstant())
 
     result.append(factory.Expr(call))
     result.append(node)
     return result
 
 
+def _rewrite_assign(function, class_name, node: ast.Assign) -> Optional[list]:
+    factory = _ast_utils.NodeFactory(node.lineno, node.col_offset)
+
+    result: List[ast.stmt] = []
+
+    for target in node.targets:
+        if isinstance(target, ast.Name):
+            call = factory.Call()
+            call.func = factory.NameLoadRewriteCallback("after_assign")
+            call.args.append(factory.NameLoad("__name__"))
+            call.args.append(factory.NameLoad("__file__"))
+            call.args.append(factory.Str(f"{class_name}{function.name}"))
+            call.args.append(factory.LineConstant())
+            call.args.append(factory.Str(target.id))
+            call.args.append(factory.NameLoad(target.id))
+
+    result.append(node)
+    result.append(factory.Expr(call))
+    return result
+
+
 _EMPTY_LIST: list = []
 
 
 def _create_before_method_ast(factory, class_name, function, filter_kind) -> list:
     # Target code:
     # def method(a, b):
     #     before_method(__name, __file__, "method_name", 11, {'a': a, 'b': b})
@@ -139,15 +160,15 @@
 
 def _create_except_handler_ast(
     factory,
     class_name: str,
     function: ast.FunctionDef,
     last_body_lineno,
     filter_kind: FilterKind,
-):
+) -> ast.ExceptHandler:
     # Target code:
     #     import sys as @py_sys
     #     method_except(@py_sys.exc_info())
     #     raise
     #
     # ExceptHandler
     #   Import
@@ -195,29 +216,29 @@
     add_to_body.extend(imports)
     add_to_body.append(factory.Expr(call_method_except))
 
     except_handler.body.append(factory.Raise())
     return except_handler
 
 
-def _create_after_method_ast(factory, class_name, function, filter_kind):
+def _create_after_method_ast(factory, class_name, function, filter_kind) -> ast.Expr:
     call = factory.Call()
     call.func = factory.NameLoadRewriteCallback("after_method")
     call.args.append(factory.NameLoad("__name__"))
     call.args.append(factory.NameLoad("__file__"))
     call.args.append(factory.Str(f"{class_name}{function.name}"))
     call.args.append(factory.LineConstant())
 
     if filter_kind == FilterKind.log_on_project_call:
         return factory.AndExpr(factory.NameLoad("@caller_in_proj"), call)
     else:
         return factory.Expr(call)
 
 
-def _rewrite_funcdef(stack, node, filter_kind):
+def _rewrite_funcdef(stack, node, filter_kind) -> None:
     parent: Any
     function: ast.FunctionDef = node
     if function.name.startswith("_") and function.name != "__init__":
         return
 
     if not function.body:
         return
@@ -226,25 +247,23 @@
     class_name = ""
     if stack:
         parent = stack[-1]
         if parent.__class__.__name__ == "ClassDef":
             class_name = parent.name + "."
 
     first_non_constant_stmt_index = 0
+    stmt: ast.stmt
     for stmt in function.body:
-        if (
-            stmt.__class__.__name__ == "Expr"
-            and stmt.value.__class__.__name__ == "Constant"
-        ):
+        if isinstance(stmt, ast.Expr) and isinstance(stmt.value, ast.Constant):
             first_non_constant_stmt_index += 1
             continue
         break
 
     function_body = function.body
-    function.body = None  # Proper value will be set later.
+    function.body = []  # Proper value will be set later.
 
     # Separate the docstring.
     if first_non_constant_stmt_index > 0:
         function_body_prefix = function_body[0:first_non_constant_stmt_index]
         function_body = function_body[first_non_constant_stmt_index:]
     else:
         function_body_prefix = _EMPTY_LIST
@@ -341,36 +360,67 @@
 
     while True:
         try:
             stack, node = next(it)
         except StopIteration:
             break
 
-        if node.__class__.__name__ == "Return":
-            func_and_class_name = _get_function_and_class_name(stack)
-            if not func_and_class_name:
-                continue
-            function, class_name = func_and_class_name
-
-            try:
-                result = _rewrite_return(function, class_name, node)
-            except Exception:
-                raise RuntimeError(
-                    f"Error when rewriting function return: {function.name} line: {node.lineno} at: {module_path}"
-                )
-
-            if result is None:
-                continue
-            it.send(result)
-
-        elif node.__class__.__name__ == "FunctionDef":
-            try:
-                _rewrite_funcdef(stack, node, filter_kind)
-            except Exception:
-                raise RuntimeError(
-                    f"Error when rewriting function: {node.name} line: {node.lineno} at: {module_path}"
-                )
+        handler = _dispatch.get(node.__class__)
+        if handler:
+            result = handler(config, module_path, stack, filter_kind, node)
+            if result is not None:
+                it.send(result)
 
     if DEBUG:
         print("\n============ New AST (with hooks in place) ==============\n")
         # Note: only python 3.9 onwards.
         print(ast.unparse(mod))  # type: ignore
+
+
+def _handle_funcdef(config, module_path, stack, filter_kind, node):
+    try:
+        _rewrite_funcdef(stack, node, filter_kind)
+    except Exception:
+        raise RuntimeError(
+            f"Error when rewriting function: {node.name} line: {node.lineno} at: {module_path}"
+        )
+
+
+def _handle_return(config, module_path, stack, filter_kind, node):
+    func_and_class_name = _get_function_and_class_name(stack)
+    if not func_and_class_name:
+        return None
+
+    function, class_name = func_and_class_name
+
+    try:
+        return _rewrite_return(function, class_name, node)
+    except Exception:
+        raise RuntimeError(
+            f"Error when rewriting function return: {function.name} line: {node.lineno} at: {module_path}"
+        )
+
+
+def _handle_assign(config, module_path, stack, filter_kind, node):
+    if filter_kind != FilterKind.full_log:
+        return None
+
+    func_and_class_name = _get_function_and_class_name(stack)
+    if not func_and_class_name:
+        return None
+
+    function, class_name = func_and_class_name
+
+    try:
+        return _rewrite_assign(function, class_name, node)
+    except Exception:
+        raise RuntimeError(
+            f"Error when rewriting assign: {function.name} line: {node.lineno} at: {module_path}"
+        )
+
+
+_dispatch: Dict[
+    type, Callable[[BaseConfig, str, list, FilterKind, Any], Optional[list]]
+] = {}
+_dispatch[ast.Return] = _handle_return
+_dispatch[ast.Assign] = _handle_assign
+_dispatch[ast.FunctionDef] = _handle_funcdef
```

### Comparing `robocorp_logging-0.0.8/src/robo_log/_rewrite_filtering.py` & `robocorp_logging-0.0.9/src/robo_log/_rewrite_filtering.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os.path
 import sys
 
 import platform
 import logging
 from typing import Sequence, Optional, List, Dict
 import threading
-from ._config import Filter, FilterKind
 
 log = logging.getLogger(__name__)
 
 
 def normcase(s, NORMCASE_CACHE={}):
     try:
         return NORMCASE_CACHE[s]
@@ -37,29 +36,25 @@
 
 class FilesFiltering(object):
     """
     Usage is something as:
 
     files_filtering = FilesFiltering(...)
 
-    if files_filtering.accept(mod.__file__, mod.__name__):
-        ...
+    # Detects if a given file is user-code.
+    files_filtering.in_project_roots(mod.__file__)
     """
 
     def __init__(
         self,
         project_roots: Optional[Sequence[str]] = None,
         library_roots: Optional[Sequence[str]] = None,
-        filters: Sequence[Filter] = (),
     ):
-        self._filters = filters
         self._project_roots: List[str] = []
         self._library_roots: List[str] = []
-        self._cache_modname_to_kind: Dict[str, Optional[FilterKind]] = {}
-        self._cache_filename_to_kind: Dict[str, FilterKind] = {}
         self._cache_in_project_roots: Dict[str, bool] = {}
 
         if project_roots is not None:
             self._set_project_roots(project_roots)
 
         if library_roots is None:
             library_roots = self._get_default_library_roots()
@@ -259,54 +254,7 @@
             return self._cache_in_project_roots[filename]
         except KeyError:
             pass
 
         in_project_roots = self._in_project_roots(filename)
         self._cache_in_project_roots[filename] = in_project_roots
         return in_project_roots
-
-    def _compute_filter_kind(self, module_name: str) -> Optional[FilterKind]:
-        """
-        :return: True if it should be excluded, False if it should be included and None
-            if no rule matched the given file.
-        """
-        for exclude_filter in self._filters:
-            if exclude_filter.name == module_name or module_name.startswith(
-                exclude_filter.name + "."
-            ):
-                return exclude_filter.kind
-        return None
-
-    def get_modname_filter_kind(self, module_name: str) -> Optional[FilterKind]:
-        cache_key = module_name
-        try:
-            return self._cache_modname_to_kind[cache_key]
-        except KeyError:
-            pass
-
-        filter_kind = self._compute_filter_kind(module_name)
-        self._cache_modname_to_kind[cache_key] = filter_kind
-        return filter_kind
-
-    def get_modname_or_file_filter_kind(
-        self, filename: str, module_name: str
-    ) -> FilterKind:
-        filter_kind = self.get_modname_filter_kind(module_name)
-        if filter_kind is not None:
-            return filter_kind
-
-        absolute_filename = self._absolute_normalized_path(filename)
-
-        cache_key = absolute_filename
-        try:
-            return self._cache_filename_to_kind[cache_key]
-        except KeyError:
-            pass
-
-        exclude = not self.in_project_roots(absolute_filename)
-        if exclude:
-            filter_kind = FilterKind.exclude
-        else:
-            filter_kind = FilterKind.full_log
-
-        self._cache_filename_to_kind[cache_key] = filter_kind
-        return filter_kind
```

### Comparing `robocorp_logging-0.0.8/src/robo_log/_rewrite_importhook.py` & `robocorp_logging-0.0.9/src/robo_log/_rewrite_importhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 # 0.0.1: Initial version
 # 0.0.2: Bugfix: docstrings must be kept as the first statement
 # 0.0.3: Support for exception handlers
 # 0.0.4: Add __name__
 # 0.0.5: Renames of internal modules.
 # 0.0.6: Option to log just 1 level deep into library modules.
 # 0.0.7: Just include __name__, note __package__.
-version = "0.0.7"
+# 0.0.9: Rewrite assign statements
+version = "0.0.9"
 PYTEST_TAG = f"{sys.implementation.cache_tag}-robo_log-{version}"
 PYC_EXT = ".py" + (__debug__ and "c" or "o")
 PYC_TAIL = "." + PYTEST_TAG + PYC_EXT
 
 FORCE_CODE_GENERATION = False
 DEBUG = False
```

### Comparing `robocorp_logging-0.0.8/src/robo_log/_robo_logger.py` & `robocorp_logging-0.0.9/src/robo_log/_robo_logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         # Note: expected to be used just when used in-memory (not part of the public API).
         config.write = kwargs.get("__write__")
         config.initial_time = kwargs.get("__initial_time__")
         config.additional_info = kwargs.get("__additional_info__")
 
         self._robot_output_impl = _RoboOutputImpl(config)
         self._skip_log_methods = 0
-        self._skip_log_arguments = 0
+        self._skip_log_variables = 0
 
     def hide_from_output(self, string_to_hide: str) -> None:
         self._robot_output_impl.hide_from_output(string_to_hide)
 
     @property
     def robot_output_impl(self):
         return self._robot_output_impl
@@ -109,29 +109,29 @@
 
         self._skip_log_methods -= 1
 
     def stop_logging_methods(self):
         self._skip_log_methods += 1
 
     def start_logging_variables(self):
-        if self._skip_log_arguments <= 0:
+        if self._skip_log_variables <= 0:
             self._robot_output_impl.log_message(
                 "ERROR",
                 f"_RoboLogger error: start_logging_variables() called before stop_logging_variables() (call is ignored as logging is already on).",
                 False,
                 __file__,
                 sys._getframe().f_lineno,
                 self._robot_output_impl.get_time_delta(),
             )
             return
 
-        self._skip_log_arguments -= 1
+        self._skip_log_variables -= 1
 
     def stop_logging_variables(self):
-        self._skip_log_arguments += 1
+        self._skip_log_variables += 1
 
     @_log_error
     def start_run(self, name: str) -> None:
         return self._robot_output_impl.start_run(
             name,
             self._get_time_delta(),
         )
@@ -186,76 +186,94 @@
         self,
         name: str,
         libname: str,
         source: str,
         lineno: int,
         element_type: str,  # METHOD/IF/WHILE,etc.
         doc: str,
-        args: Sequence[Tuple[str, str]],
-        assign_targets: Sequence[str],
+        args: Sequence[Tuple[str, str, str]],
         tags: Sequence[str],
     ):
         """
         Example:
 
         start_element(
             "close_browser",
             "RPA.Browser",
             "c:/my/browser.py",
             lineno=1,
             element_type="METHOD",
             doc="Closes Browser",
-            args=["force=True"],
-            assign_targets=[],
+            args=[("force", "boolean", "True")],
             tags=["some-tag"],
         )
         """
         hide_from_logs = False
         if tags:
             if "log:ignore-methods" in tags:
                 self._skip_log_methods += 1
             if "log:ignore-variables" in tags:
-                self._skip_log_arguments += 1
+                self._skip_log_variables += 1
 
         if self._skip_log_methods:
             if name not in (
                 "stop_logging_methods",
                 "start_logging_methods",
             ):
                 hide_from_logs = True
 
         if args:
-            if self._skip_log_arguments or name == "hide_from_output":
-                args = [(name, "<redacted>") for name, _value in args]
+            if self._skip_log_variables or name == "hide_from_output":
+                args = [(name, tp, "<redacted>") for name, tp, _value in args]
 
         return self._robot_output_impl.start_element(
             name,
             libname,
             element_type,
             doc,
             source,
             lineno,
             self._get_time_delta(),
             args,
-            assign_targets,
             hide_from_logs=hide_from_logs,
         )
 
     @_log_error
+    def after_assign(
+        self,
+        filename: str,
+        lineno: int,
+        assign_name: str,
+        assign_type: str,
+        assign_repr: str,
+    ):
+        if self._skip_log_variables:
+            return
+
+        return self._robot_output_impl.after_assign(
+            filename,
+            lineno,
+            assign_name,
+            assign_type,
+            assign_repr,
+            self._get_time_delta(),
+        )
+
+    @_log_error
     def end_method(self, name: str, libname: str, status: str, tags: Sequence[str]):
         try:
             return self._robot_output_impl.end_method(
                 name, libname, status, self._get_time_delta()
             )
         finally:
             if tags:
                 if "log:ignore-methods" in tags:
                     self._skip_log_methods -= 1
                 if "log:ignore-variables" in tags:
-                    self._skip_log_arguments -= 1
+                    self._skip_log_variables -= 1
 
     @_log_error
     def log_message(
         self, level: str, message: str, html: bool, source: str, lineno: int
     ):
         return self._robot_output_impl.log_message(
             level, message, html, source, lineno, self._get_time_delta()
```

### Comparing `robocorp_logging-0.0.8/src/robo_log/_robo_output_impl.py` & `robocorp_logging-0.0.9/src/robo_log/_robo_output_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from pathlib import Path
-from typing import Dict, Iterator, List, Sequence, Set, Pattern
-import json
-import itertools
-import string
-import datetime
+from contextlib import contextmanager
+from datetime import timezone
+from functools import partial
+from robo_log.protocols import OptExcInfo
+from typing import Dict, Iterator, List, Sequence, Set, Pattern, Tuple
 from typing import Optional, Callable
+import datetime
+import itertools
+import json
 import os
-import traceback
-from contextlib import contextmanager
+import string
 import sys
-import weakref
-from robo_log.protocols import OptExcInfo
-from functools import partial
 import time
-from datetime import timezone
+import traceback
+import weakref
+
+WRITE_CONTENTS_TO_STDERR: bool = False
 
 
 _valid_chars = tuple(string.ascii_letters + string.digits)
 
 
 def _gen_id(level: int = 1) -> Iterator[str]:
     iter_in = tuple(_valid_chars for _ in range(level))
@@ -81,15 +83,17 @@
                 traceback.print_exc()
 
     def iter_found_files(self):
         yield from iter(self._found_files)
 
 
 class _StackEntry:
-    def __init__(self, entry_type, entry_id, msg_type, new_msg_type, hide_from_logs):
+    def __init__(
+        self, entry_type, entry_id, msg_type, new_msg_type, hide_from_logs
+    ) -> None:
         self.entry_type = entry_type
         self.entry_id = entry_id
         self.msg_type = msg_type
         self.new_msg_type = new_msg_type
         self.hide_from_logs = hide_from_logs
         self._messages: List[str] = []
 
@@ -114,15 +118,20 @@
         self._queue = []
         self.recording_writes = False
         self._record_to = None
         self._robot_output_impl = weakref.ref(robot_output_impl)
 
     @contextmanager
     def push_record(
-        self, entry_type, entry_id, msg_type, new_msg_type, hide_from_logs=False
+        self,
+        entry_type: str,
+        entry_id: str,
+        msg_type: str,
+        new_msg_type: str,
+        hide_from_logs: bool = False,
     ):
         self.recording_writes = True
         self._record_to = _StackEntry(
             entry_type, entry_id, msg_type, new_msg_type, hide_from_logs
         )
         try:
             yield
@@ -481,14 +490,16 @@
 
         :returns:
             Whether the exception was added to the log or not -- this may be
             because the exc_info is not complete or cases where the exception
             was already previously logged (see the `unhandled` parameter for
             details on the use-cases where it may be skipped).
         """
+        from robo_log._obj_info_repr import get_obj_type_and_repr
+
         tp, e, tb = exc_info
         if e is None or tb is None or tp is None:
             return False
 
         f = tb.tb_frame.f_back
         stack: List[tuple] = []
         while f is not None:
@@ -546,48 +557,44 @@
                     ],
                 )
 
                 for key, val in tuple(frame.f_locals.items()):
                     if key.startswith("@"):
                         # Skip our own variables.
                         continue
-                    try:
-                        val_type = val.__class__.__name__
-                    except:
-                        val_type = str(type(val))
 
+                    obj_type, obj_repr = get_obj_type_and_repr(val)
                     self._write_with_separator(
                         "TBV ",
                         [
                             oid(str(key)),
-                            oid(val_type),
-                            oid(repr(val)),
+                            oid(obj_type),
+                            oid(obj_repr),
                         ],
                     )
 
         stack_entry = self._stack_handler.pop("traceback", entry_id)
         assert stack_entry
 
         self._write_with_separator("ETB ", [self._number(self.get_time_delta())])
 
         return True
 
     def start_element(
         self,
-        name,
-        libname,
-        element_type,
-        doc,
-        source,
-        lineno,
-        start_time_delta,
-        args,
-        assigns,
-        hide_from_logs=False,
-    ):
+        name: str,
+        libname: str,
+        element_type: str,
+        doc: str,
+        source: str,
+        lineno: int,
+        start_time_delta: float,
+        args: Sequence[Tuple[str, str, str]],
+        hide_from_logs: bool = False,
+    ) -> None:
         element_type = element_type.upper()
         oid = self._obtain_id
         element_id = f"{libname}.{name}"
         with self._stack_handler.push_record(
             "element", element_id, "SE", "RE", hide_from_logs
         ):
             if hide_from_logs:
@@ -603,40 +610,25 @@
                     oid(doc),
                     oid(source),
                     self._number(lineno),
                     self._number(start_time_delta),
                 ],
             )
 
-            if assigns:
-                for assign in assigns:
-                    lower_assign = assign.lower()
-                    for p in ("password", "passwd"):
-                        if p in lower_assign:
-                            if args:
-                                for _, arg in args:
-                                    self.hide_from_output(arg)
-                            break
-
-                    self._write_with_separator(
-                        "AS ",
-                        [
-                            oid(assign),
-                        ],
-                    )
             if args:
-                for name, arg in args:
+                for name, arg_type, arg in args:
                     hide_strings_re = self._hide_strings_re
                     if hide_strings_re:
                         arg = hide_strings_re.sub("<redacted>", arg)
 
                     self._write_with_separator(
                         "EA ",
                         [
                             oid(name),
+                            oid(arg_type),
                             oid(arg),
                         ],
                     )
 
     def end_method(self, name, libname, status, time_delta):
         element_id = f"{libname}.{name}"
         oid = self._obtain_id
@@ -650,14 +642,41 @@
             "EE ",
             [
                 oid(status),
                 self._number(time_delta),
             ],
         )
 
+    def after_assign(
+        self,
+        filename: str,
+        lineno: int,
+        assign_name: str,
+        assign_type: str,
+        assign_repr: str,
+        time_delta: float,
+    ):
+        oid = self._obtain_id
+
+        hide_strings_re = self._hide_strings_re
+        if hide_strings_re:
+            assign_repr = hide_strings_re.sub("<redacted>", assign_repr)
+
+        self._write_with_separator(
+            "AS ",
+            [
+                oid(filename),
+                self._number(lineno),
+                oid(assign_name),
+                oid(assign_type),
+                oid(assign_repr),
+                self._number(time_delta),
+            ],
+        )
+
     def log_message(self, level, message, html, source, lineno, time_delta):
         oid = self._obtain_id
 
         msg_type = "L "
         if html in ("true", "yes", 1, True):
             # From output.xml it's "true", from listener it's "yes".
             msg_type = "LH "
@@ -696,17 +715,17 @@
             target = os.path.abspath(log_html)
             dirname = os.path.dirname(target)
             if not os.path.exists(dirname):
                 os.makedirs(dirname, exist_ok=True)
             print(f"Robocorp Log (html): {target}")
 
             if self._config.log_html_style == 1:
-                from robo_log import index
+                from robo_log import _index as index
             elif self._config.log_html_style == 2:
-                from robo_log import index_v2 as index
+                from robo_log import _index_v2 as index
             else:
                 raise ValueError(
                     "Unexpected log html style: {self._config.log_html_style}"
                 )
 
             # from robo_log import index
 
@@ -742,15 +761,14 @@
             assert end_of_json_parse_index > 0
             self._write_updating_sample(
                 stream, contents, return_json_parse_index, end_of_json_parse_index
             )
 
     def _write_index_updating_sample(self, target, contents):
         with open(target, "wb") as stream:
-            # We want to replace the string so that we write
             sample_contents_index = contents.index("getSampleContents")
             assert sample_contents_index > 0
 
             return_json_parse_index = contents.index(
                 "return JSON.parse", sample_contents_index
             )
             assert return_json_parse_index > 0
@@ -766,29 +784,37 @@
     ):
         import base64
 
         stream.write(contents[:return_json_parse_index].encode("utf-8"))
 
         import zlib
 
-        stream.write(b"\nlet chunks = [")
+        write = stream.write
+        if WRITE_CONTENTS_TO_STDERR:
+            stream_write = write
+
+            def write(b):
+                stream_write(b)
+                sys.stderr.buffer.write(b)
+
+        write(b"\nlet chunks = [")
         for f in self._rotate_handler.iter_found_files():
             with open(f, "rb") as fsrc:
                 while True:
                     chunk = fsrc.read(1024 * 8)
                     if not chunk:
                         break
-                    stream.write(b'"')
+                    write(b'"')
                     chunk = zlib.compress(chunk)
-                    stream.write(base64.b64encode(chunk))
-                    stream.write(b'",\n')
-        stream.write(b"];\n")
+                    write(base64.b64encode(chunk))
+                    write(b'",\n')
+        write(b"];\n")
 
         # Add code to decompress the data we added.
-        stream.write(
+        write(
             b"""
 /*! pako 2.1.0 https://github.com/nodeca/pako @license (MIT AND Zlib) */
 !function(e,t){"object"==typeof exports&&"undefined"!=typeof module?t(exports):"function"==typeof define&&define.amd?define(["exports"],t):t((e="undefined"!=typeof globalThis?globalThis:e||self).pako={})}(this,(function(e){"use strict";var t=(e,t,i,n)=>{let a=65535&e|0,r=e>>>16&65535|0,o=0;for(;0!==i;){o=i>2e3?2e3:i,i-=o;do{a=a+t[n++]|0,r=r+a|0}while(--o);a%=65521,r%=65521}return a|r<<16|0};const i=new Uint32Array((()=>{let e,t=[];for(var i=0;i<256;i++){e=i;for(var n=0;n<8;n++)e=1&e?3988292384^e>>>1:e>>>1;t[i]=e}return t})());var n=(e,t,n,a)=>{const r=i,o=a+n;e^=-1;for(let i=a;i<o;i++)e=e>>>8^r[255&(e^t[i])];return-1^e};const a=16209;var r=function(e,t){let i,n,r,o,s,l,d,f,c,h,u,w,b,m,k,_,g,p,v,x,y,E,R,A;const Z=e.state;i=e.next_in,R=e.input,n=i+(e.avail_in-5),r=e.next_out,A=e.output,o=r-(t-e.avail_out),s=r+(e.avail_out-257),l=Z.dmax,d=Z.wsize,f=Z.whave,c=Z.wnext,h=Z.window,u=Z.hold,w=Z.bits,b=Z.lencode,m=Z.distcode,k=(1<<Z.lenbits)-1,_=(1<<Z.distbits)-1;e:do{w<15&&(u+=R[i++]<<w,w+=8,u+=R[i++]<<w,w+=8),g=b[u&k];t:for(;;){if(p=g>>>24,u>>>=p,w-=p,p=g>>>16&255,0===p)A[r++]=65535&g;else{if(!(16&p)){if(0==(64&p)){g=b[(65535&g)+(u&(1<<p)-1)];continue t}if(32&p){Z.mode=16191;break e}e.msg="invalid literal/length code",Z.mode=a;break e}v=65535&g,p&=15,p&&(w<p&&(u+=R[i++]<<w,w+=8),v+=u&(1<<p)-1,u>>>=p,w-=p),w<15&&(u+=R[i++]<<w,w+=8,u+=R[i++]<<w,w+=8),g=m[u&_];i:for(;;){if(p=g>>>24,u>>>=p,w-=p,p=g>>>16&255,!(16&p)){if(0==(64&p)){g=m[(65535&g)+(u&(1<<p)-1)];continue i}e.msg="invalid distance code",Z.mode=a;break e}if(x=65535&g,p&=15,w<p&&(u+=R[i++]<<w,w+=8,w<p&&(u+=R[i++]<<w,w+=8)),x+=u&(1<<p)-1,x>l){e.msg="invalid distance too far back",Z.mode=a;break e}if(u>>>=p,w-=p,p=r-o,x>p){if(p=x-p,p>f&&Z.sane){e.msg="invalid distance too far back",Z.mode=a;break e}if(y=0,E=h,0===c){if(y+=d-p,p<v){v-=p;do{A[r++]=h[y++]}while(--p);y=r-x,E=A}}else if(c<p){if(y+=d+c-p,p-=c,p<v){v-=p;do{A[r++]=h[y++]}while(--p);if(y=0,c<v){p=c,v-=p;do{A[r++]=h[y++]}while(--p);y=r-x,E=A}}}else if(y+=c-p,p<v){v-=p;do{A[r++]=h[y++]}while(--p);y=r-x,E=A}for(;v>2;)A[r++]=E[y++],A[r++]=E[y++],A[r++]=E[y++],v-=3;v&&(A[r++]=E[y++],v>1&&(A[r++]=E[y++]))}else{y=r-x;do{A[r++]=A[y++],A[r++]=A[y++],A[r++]=A[y++],v-=3}while(v>2);v&&(A[r++]=A[y++],v>1&&(A[r++]=A[y++]))}break}}break}}while(i<n&&r<s);v=w>>3,i-=v,w-=v<<3,u&=(1<<w)-1,e.next_in=i,e.next_out=r,e.avail_in=i<n?n-i+5:5-(i-n),e.avail_out=r<s?s-r+257:257-(r-s),Z.hold=u,Z.bits=w};const o=15,s=new Uint16Array([3,4,5,6,7,8,9,10,11,13,15,17,19,23,27,31,35,43,51,59,67,83,99,115,131,163,195,227,258,0,0]),l=new Uint8Array([16,16,16,16,16,16,16,16,17,17,17,17,18,18,18,18,19,19,19,19,20,20,20,20,21,21,21,21,16,72,78]),d=new Uint16Array([1,2,3,4,5,7,9,13,17,25,33,49,65,97,129,193,257,385,513,769,1025,1537,2049,3073,4097,6145,8193,12289,16385,24577,0,0]),f=new Uint8Array([16,16,16,16,17,17,18,18,19,19,20,20,21,21,22,22,23,23,24,24,25,25,26,26,27,27,28,28,29,29,64,64]);var c=(e,t,i,n,a,r,c,h)=>{const u=h.bits;let w,b,m,k,_,g,p=0,v=0,x=0,y=0,E=0,R=0,A=0,Z=0,S=0,T=0,O=null;const U=new Uint16Array(16),D=new Uint16Array(16);let I,B,N,C=null;for(p=0;p<=o;p++)U[p]=0;for(v=0;v<n;v++)U[t[i+v]]++;for(E=u,y=o;y>=1&&0===U[y];y--);if(E>y&&(E=y),0===y)return a[r++]=20971520,a[r++]=20971520,h.bits=1,0;for(x=1;x<y&&0===U[x];x++);for(E<x&&(E=x),Z=1,p=1;p<=o;p++)if(Z<<=1,Z-=U[p],Z<0)return-1;if(Z>0&&(0===e||1!==y))return-1;for(D[1]=0,p=1;p<o;p++)D[p+1]=D[p]+U[p];for(v=0;v<n;v++)0!==t[i+v]&&(c[D[t[i+v]]++]=v);if(0===e?(O=C=c,g=20):1===e?(O=s,C=l,g=257):(O=d,C=f,g=0),T=0,v=0,p=x,_=r,R=E,A=0,m=-1,S=1<<E,k=S-1,1===e&&S>852||2===e&&S>592)return 1;for(;;){I=p-A,c[v]+1<g?(B=0,N=c[v]):c[v]>=g?(B=C[c[v]-g],N=O[c[v]-g]):(B=96,N=0),w=1<<p-A,b=1<<R,x=b;do{b-=w,a[_+(T>>A)+b]=I<<24|B<<16|N|0}while(0!==b);for(w=1<<p-1;T&w;)w>>=1;if(0!==w?(T&=w-1,T+=w):T=0,v++,0==--U[p]){if(p===y)break;p=t[i+c[v]]}if(p>E&&(T&k)!==m){for(0===A&&(A=E),_+=x,R=p-A,Z=1<<R;R+A<y&&(Z-=U[R+A],!(Z<=0));)R++,Z<<=1;if(S+=1<<R,1===e&&S>852||2===e&&S>592)return 1;m=T&k,a[m]=E<<24|R<<16|_-r|0}}return 0!==T&&(a[_+T]=p-A<<24|64<<16|0),h.bits=E,0},h={Z_NO_FLUSH:0,Z_PARTIAL_FLUSH:1,Z_SYNC_FLUSH:2,Z_FULL_FLUSH:3,Z_FINISH:4,Z_BLOCK:5,Z_TREES:6,Z_OK:0,Z_STREAM_END:1,Z_NEED_DICT:2,Z_ERRNO:-1,Z_STREAM_ERROR:-2,Z_DATA_ERROR:-3,Z_MEM_ERROR:-4,Z_BUF_ERROR:-5,Z_NO_COMPRESSION:0,Z_BEST_SPEED:1,Z_BEST_COMPRESSION:9,Z_DEFAULT_COMPRESSION:-1,Z_FILTERED:1,Z_HUFFMAN_ONLY:2,Z_RLE:3,Z_FIXED:4,Z_DEFAULT_STRATEGY:0,Z_BINARY:0,Z_TEXT:1,Z_UNKNOWN:2,Z_DEFLATED:8};const{Z_FINISH:u,Z_BLOCK:w,Z_TREES:b,Z_OK:m,Z_STREAM_END:k,Z_NEED_DICT:_,Z_STREAM_ERROR:g,Z_DATA_ERROR:p,Z_MEM_ERROR:v,Z_BUF_ERROR:x,Z_DEFLATED:y}=h,E=16180,R=16190,A=16191,Z=16192,S=16194,T=16199,O=16200,U=16206,D=16209,I=e=>(e>>>24&255)+(e>>>8&65280)+((65280&e)<<8)+((255&e)<<24);function B(){this.strm=null,this.mode=0,this.last=!1,this.wrap=0,this.havedict=!1,this.flags=0,this.dmax=0,this.check=0,this.total=0,this.head=null,this.wbits=0,this.wsize=0,this.whave=0,this.wnext=0,this.window=null,this.hold=0,this.bits=0,this.length=0,this.offset=0,this.extra=0,this.lencode=null,this.distcode=null,this.lenbits=0,this.distbits=0,this.ncode=0,this.nlen=0,this.ndist=0,this.have=0,this.next=null,this.lens=new Uint16Array(320),this.work=new Uint16Array(288),this.lendyn=null,this.distdyn=null,this.sane=0,this.back=0,this.was=0}const N=e=>{if(!e)return 1;const t=e.state;return!t||t.strm!==e||t.mode<E||t.mode>16211?1:0},C=e=>{if(N(e))return g;const t=e.state;return e.total_in=e.total_out=t.total=0,e.msg="",t.wrap&&(e.adler=1&t.wrap),t.mode=E,t.last=0,t.havedict=0,t.flags=-1,t.dmax=32768,t.head=null,t.hold=0,t.bits=0,t.lencode=t.lendyn=new Int32Array(852),t.distcode=t.distdyn=new Int32Array(592),t.sane=1,t.back=-1,m},z=e=>{if(N(e))return g;const t=e.state;return t.wsize=0,t.whave=0,t.wnext=0,C(e)},F=(e,t)=>{let i;if(N(e))return g;const n=e.state;return t<0?(i=0,t=-t):(i=5+(t>>4),t<48&&(t&=15)),t&&(t<8||t>15)?g:(null!==n.window&&n.wbits!==t&&(n.window=null),n.wrap=i,n.wbits=t,z(e))},L=(e,t)=>{if(!e)return g;const i=new B;e.state=i,i.strm=e,i.window=null,i.mode=E;const n=F(e,t);return n!==m&&(e.state=null),n};let M,H,j=!0;const K=e=>{if(j){M=new Int32Array(512),H=new Int32Array(32);let t=0;for(;t<144;)e.lens[t++]=8;for(;t<256;)e.lens[t++]=9;for(;t<280;)e.lens[t++]=7;for(;t<288;)e.lens[t++]=8;for(c(1,e.lens,0,288,M,0,e.work,{bits:9}),t=0;t<32;)e.lens[t++]=5;c(2,e.lens,0,32,H,0,e.work,{bits:5}),j=!1}e.lencode=M,e.lenbits=9,e.distcode=H,e.distbits=5},P=(e,t,i,n)=>{let a;const r=e.state;return null===r.window&&(r.wsize=1<<r.wbits,r.wnext=0,r.whave=0,r.window=new Uint8Array(r.wsize)),n>=r.wsize?(r.window.set(t.subarray(i-r.wsize,i),0),r.wnext=0,r.whave=r.wsize):(a=r.wsize-r.wnext,a>n&&(a=n),r.window.set(t.subarray(i-n,i-n+a),r.wnext),(n-=a)?(r.window.set(t.subarray(i-n,i),0),r.wnext=n,r.whave=r.wsize):(r.wnext+=a,r.wnext===r.wsize&&(r.wnext=0),r.whave<r.wsize&&(r.whave+=a))),0};var Y={inflateReset:z,inflateReset2:F,inflateResetKeep:C,inflateInit:e=>L(e,15),inflateInit2:L,inflate:(e,i)=>{let a,o,s,l,d,f,h,B,C,z,F,L,M,H,j,Y,G,X,W,q,J,Q,V=0;const $=new Uint8Array(4);let ee,te;const ie=new Uint8Array([16,17,18,0,8,7,9,6,10,5,11,4,12,3,13,2,14,1,15]);if(N(e)||!e.output||!e.input&&0!==e.avail_in)return g;a=e.state,a.mode===A&&(a.mode=Z),d=e.next_out,s=e.output,h=e.avail_out,l=e.next_in,o=e.input,f=e.avail_in,B=a.hold,C=a.bits,z=f,F=h,Q=m;e:for(;;)switch(a.mode){case E:if(0===a.wrap){a.mode=Z;break}for(;C<16;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}if(2&a.wrap&&35615===B){0===a.wbits&&(a.wbits=15),a.check=0,$[0]=255&B,$[1]=B>>>8&255,a.check=n(a.check,$,2,0),B=0,C=0,a.mode=16181;break}if(a.head&&(a.head.done=!1),!(1&a.wrap)||(((255&B)<<8)+(B>>8))%31){e.msg="incorrect header check",a.mode=D;break}if((15&B)!==y){e.msg="unknown compression method",a.mode=D;break}if(B>>>=4,C-=4,J=8+(15&B),0===a.wbits&&(a.wbits=J),J>15||J>a.wbits){e.msg="invalid window size",a.mode=D;break}a.dmax=1<<a.wbits,a.flags=0,e.adler=a.check=1,a.mode=512&B?16189:A,B=0,C=0;break;case 16181:for(;C<16;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}if(a.flags=B,(255&a.flags)!==y){e.msg="unknown compression method",a.mode=D;break}if(57344&a.flags){e.msg="unknown header flags set",a.mode=D;break}a.head&&(a.head.text=B>>8&1),512&a.flags&&4&a.wrap&&($[0]=255&B,$[1]=B>>>8&255,a.check=n(a.check,$,2,0)),B=0,C=0,a.mode=16182;case 16182:for(;C<32;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}a.head&&(a.head.time=B),512&a.flags&&4&a.wrap&&($[0]=255&B,$[1]=B>>>8&255,$[2]=B>>>16&255,$[3]=B>>>24&255,a.check=n(a.check,$,4,0)),B=0,C=0,a.mode=16183;case 16183:for(;C<16;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}a.head&&(a.head.xflags=255&B,a.head.os=B>>8),512&a.flags&&4&a.wrap&&($[0]=255&B,$[1]=B>>>8&255,a.check=n(a.check,$,2,0)),B=0,C=0,a.mode=16184;case 16184:if(1024&a.flags){for(;C<16;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}a.length=B,a.head&&(a.head.extra_len=B),512&a.flags&&4&a.wrap&&($[0]=255&B,$[1]=B>>>8&255,a.check=n(a.check,$,2,0)),B=0,C=0}else a.head&&(a.head.extra=null);a.mode=16185;case 16185:if(1024&a.flags&&(L=a.length,L>f&&(L=f),L&&(a.head&&(J=a.head.extra_len-a.length,a.head.extra||(a.head.extra=new Uint8Array(a.head.extra_len)),a.head.extra.set(o.subarray(l,l+L),J)),512&a.flags&&4&a.wrap&&(a.check=n(a.check,o,L,l)),f-=L,l+=L,a.length-=L),a.length))break e;a.length=0,a.mode=16186;case 16186:if(2048&a.flags){if(0===f)break e;L=0;do{J=o[l+L++],a.head&&J&&a.length<65536&&(a.head.name+=String.fromCharCode(J))}while(J&&L<f);if(512&a.flags&&4&a.wrap&&(a.check=n(a.check,o,L,l)),f-=L,l+=L,J)break e}else a.head&&(a.head.name=null);a.length=0,a.mode=16187;case 16187:if(4096&a.flags){if(0===f)break e;L=0;do{J=o[l+L++],a.head&&J&&a.length<65536&&(a.head.comment+=String.fromCharCode(J))}while(J&&L<f);if(512&a.flags&&4&a.wrap&&(a.check=n(a.check,o,L,l)),f-=L,l+=L,J)break e}else a.head&&(a.head.comment=null);a.mode=16188;case 16188:if(512&a.flags){for(;C<16;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}if(4&a.wrap&&B!==(65535&a.check)){e.msg="header crc mismatch",a.mode=D;break}B=0,C=0}a.head&&(a.head.hcrc=a.flags>>9&1,a.head.done=!0),e.adler=a.check=0,a.mode=A;break;case 16189:for(;C<32;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}e.adler=a.check=I(B),B=0,C=0,a.mode=R;case R:if(0===a.havedict)return e.next_out=d,e.avail_out=h,e.next_in=l,e.avail_in=f,a.hold=B,a.bits=C,_;e.adler=a.check=1,a.mode=A;case A:if(i===w||i===b)break e;case Z:if(a.last){B>>>=7&C,C-=7&C,a.mode=U;break}for(;C<3;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}switch(a.last=1&B,B>>>=1,C-=1,3&B){case 0:a.mode=16193;break;case 1:if(K(a),a.mode=T,i===b){B>>>=2,C-=2;break e}break;case 2:a.mode=16196;break;case 3:e.msg="invalid block type",a.mode=D}B>>>=2,C-=2;break;case 16193:for(B>>>=7&C,C-=7&C;C<32;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}if((65535&B)!=(B>>>16^65535)){e.msg="invalid stored block lengths",a.mode=D;break}if(a.length=65535&B,B=0,C=0,a.mode=S,i===b)break e;case S:a.mode=16195;case 16195:if(L=a.length,L){if(L>f&&(L=f),L>h&&(L=h),0===L)break e;s.set(o.subarray(l,l+L),d),f-=L,l+=L,h-=L,d+=L,a.length-=L;break}a.mode=A;break;case 16196:for(;C<14;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}if(a.nlen=257+(31&B),B>>>=5,C-=5,a.ndist=1+(31&B),B>>>=5,C-=5,a.ncode=4+(15&B),B>>>=4,C-=4,a.nlen>286||a.ndist>30){e.msg="too many length or distance symbols",a.mode=D;break}a.have=0,a.mode=16197;case 16197:for(;a.have<a.ncode;){for(;C<3;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}a.lens[ie[a.have++]]=7&B,B>>>=3,C-=3}for(;a.have<19;)a.lens[ie[a.have++]]=0;if(a.lencode=a.lendyn,a.lenbits=7,ee={bits:a.lenbits},Q=c(0,a.lens,0,19,a.lencode,0,a.work,ee),a.lenbits=ee.bits,Q){e.msg="invalid code lengths set",a.mode=D;break}a.have=0,a.mode=16198;case 16198:for(;a.have<a.nlen+a.ndist;){for(;V=a.lencode[B&(1<<a.lenbits)-1],j=V>>>24,Y=V>>>16&255,G=65535&V,!(j<=C);){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}if(G<16)B>>>=j,C-=j,a.lens[a.have++]=G;else{if(16===G){for(te=j+2;C<te;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}if(B>>>=j,C-=j,0===a.have){e.msg="invalid bit length repeat",a.mode=D;break}J=a.lens[a.have-1],L=3+(3&B),B>>>=2,C-=2}else if(17===G){for(te=j+3;C<te;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}B>>>=j,C-=j,J=0,L=3+(7&B),B>>>=3,C-=3}else{for(te=j+7;C<te;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}B>>>=j,C-=j,J=0,L=11+(127&B),B>>>=7,C-=7}if(a.have+L>a.nlen+a.ndist){e.msg="invalid bit length repeat",a.mode=D;break}for(;L--;)a.lens[a.have++]=J}}if(a.mode===D)break;if(0===a.lens[256]){e.msg="invalid code -- missing end-of-block",a.mode=D;break}if(a.lenbits=9,ee={bits:a.lenbits},Q=c(1,a.lens,0,a.nlen,a.lencode,0,a.work,ee),a.lenbits=ee.bits,Q){e.msg="invalid literal/lengths set",a.mode=D;break}if(a.distbits=6,a.distcode=a.distdyn,ee={bits:a.distbits},Q=c(2,a.lens,a.nlen,a.ndist,a.distcode,0,a.work,ee),a.distbits=ee.bits,Q){e.msg="invalid distances set",a.mode=D;break}if(a.mode=T,i===b)break e;case T:a.mode=O;case O:if(f>=6&&h>=258){e.next_out=d,e.avail_out=h,e.next_in=l,e.avail_in=f,a.hold=B,a.bits=C,r(e,F),d=e.next_out,s=e.output,h=e.avail_out,l=e.next_in,o=e.input,f=e.avail_in,B=a.hold,C=a.bits,a.mode===A&&(a.back=-1);break}for(a.back=0;V=a.lencode[B&(1<<a.lenbits)-1],j=V>>>24,Y=V>>>16&255,G=65535&V,!(j<=C);){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}if(Y&&0==(240&Y)){for(X=j,W=Y,q=G;V=a.lencode[q+((B&(1<<X+W)-1)>>X)],j=V>>>24,Y=V>>>16&255,G=65535&V,!(X+j<=C);){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}B>>>=X,C-=X,a.back+=X}if(B>>>=j,C-=j,a.back+=j,a.length=G,0===Y){a.mode=16205;break}if(32&Y){a.back=-1,a.mode=A;break}if(64&Y){e.msg="invalid literal/length code",a.mode=D;break}a.extra=15&Y,a.mode=16201;case 16201:if(a.extra){for(te=a.extra;C<te;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}a.length+=B&(1<<a.extra)-1,B>>>=a.extra,C-=a.extra,a.back+=a.extra}a.was=a.length,a.mode=16202;case 16202:for(;V=a.distcode[B&(1<<a.distbits)-1],j=V>>>24,Y=V>>>16&255,G=65535&V,!(j<=C);){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}if(0==(240&Y)){for(X=j,W=Y,q=G;V=a.distcode[q+((B&(1<<X+W)-1)>>X)],j=V>>>24,Y=V>>>16&255,G=65535&V,!(X+j<=C);){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}B>>>=X,C-=X,a.back+=X}if(B>>>=j,C-=j,a.back+=j,64&Y){e.msg="invalid distance code",a.mode=D;break}a.offset=G,a.extra=15&Y,a.mode=16203;case 16203:if(a.extra){for(te=a.extra;C<te;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}a.offset+=B&(1<<a.extra)-1,B>>>=a.extra,C-=a.extra,a.back+=a.extra}if(a.offset>a.dmax){e.msg="invalid distance too far back",a.mode=D;break}a.mode=16204;case 16204:if(0===h)break e;if(L=F-h,a.offset>L){if(L=a.offset-L,L>a.whave&&a.sane){e.msg="invalid distance too far back",a.mode=D;break}L>a.wnext?(L-=a.wnext,M=a.wsize-L):M=a.wnext-L,L>a.length&&(L=a.length),H=a.window}else H=s,M=d-a.offset,L=a.length;L>h&&(L=h),h-=L,a.length-=L;do{s[d++]=H[M++]}while(--L);0===a.length&&(a.mode=O);break;case 16205:if(0===h)break e;s[d++]=a.length,h--,a.mode=O;break;case U:if(a.wrap){for(;C<32;){if(0===f)break e;f--,B|=o[l++]<<C,C+=8}if(F-=h,e.total_out+=F,a.total+=F,4&a.wrap&&F&&(e.adler=a.check=a.flags?n(a.check,s,F,d-F):t(a.check,s,F,d-F)),F=h,4&a.wrap&&(a.flags?B:I(B))!==a.check){e.msg="incorrect data check",a.mode=D;break}B=0,C=0}a.mode=16207;case 16207:if(a.wrap&&a.flags){for(;C<32;){if(0===f)break e;f--,B+=o[l++]<<C,C+=8}if(4&a.wrap&&B!==(4294967295&a.total)){e.msg="incorrect length check",a.mode=D;break}B=0,C=0}a.mode=16208;case 16208:Q=k;break e;case D:Q=p;break e;case 16210:return v;default:return g}return e.next_out=d,e.avail_out=h,e.next_in=l,e.avail_in=f,a.hold=B,a.bits=C,(a.wsize||F!==e.avail_out&&a.mode<D&&(a.mode<U||i!==u))&&P(e,e.output,e.next_out,F-e.avail_out),z-=e.avail_in,F-=e.avail_out,e.total_in+=z,e.total_out+=F,a.total+=F,4&a.wrap&&F&&(e.adler=a.check=a.flags?n(a.check,s,F,e.next_out-F):t(a.check,s,F,e.next_out-F)),e.data_type=a.bits+(a.last?64:0)+(a.mode===A?128:0)+(a.mode===T||a.mode===S?256:0),(0===z&&0===F||i===u)&&Q===m&&(Q=x),Q},inflateEnd:e=>{if(N(e))return g;let t=e.state;return t.window&&(t.window=null),e.state=null,m},inflateGetHeader:(e,t)=>{if(N(e))return g;const i=e.state;return 0==(2&i.wrap)?g:(i.head=t,t.done=!1,m)},inflateSetDictionary:(e,i)=>{const n=i.length;let a,r,o;return N(e)?g:(a=e.state,0!==a.wrap&&a.mode!==R?g:a.mode===R&&(r=1,r=t(r,i,n,0),r!==a.check)?p:(o=P(e,i,n,n),o?(a.mode=16210,v):(a.havedict=1,m)))},inflateInfo:"pako inflate (from Nodeca project)"};const G=(e,t)=>Object.prototype.hasOwnProperty.call(e,t);var X=function(e){const t=Array.prototype.slice.call(arguments,1);for(;t.length;){const i=t.shift();if(i){if("object"!=typeof i)throw new TypeError(i+"must be non-object");for(const t in i)G(i,t)&&(e[t]=i[t])}}return e},W=e=>{let t=0;for(let i=0,n=e.length;i<n;i++)t+=e[i].length;const i=new Uint8Array(t);for(let t=0,n=0,a=e.length;t<a;t++){let a=e[t];i.set(a,n),n+=a.length}return i};let q=!0;try{String.fromCharCode.apply(null,new Uint8Array(1))}catch(e){q=!1}const J=new Uint8Array(256);for(let e=0;e<256;e++)J[e]=e>=252?6:e>=248?5:e>=240?4:e>=224?3:e>=192?2:1;J[254]=J[254]=1;var Q=e=>{if("function"==typeof TextEncoder&&TextEncoder.prototype.encode)return(new TextEncoder).encode(e);let t,i,n,a,r,o=e.length,s=0;for(a=0;a<o;a++)i=e.charCodeAt(a),55296==(64512&i)&&a+1<o&&(n=e.charCodeAt(a+1),56320==(64512&n)&&(i=65536+(i-55296<<10)+(n-56320),a++)),s+=i<128?1:i<2048?2:i<65536?3:4;for(t=new Uint8Array(s),r=0,a=0;r<s;a++)i=e.charCodeAt(a),55296==(64512&i)&&a+1<o&&(n=e.charCodeAt(a+1),56320==(64512&n)&&(i=65536+(i-55296<<10)+(n-56320),a++)),i<128?t[r++]=i:i<2048?(t[r++]=192|i>>>6,t[r++]=128|63&i):i<65536?(t[r++]=224|i>>>12,t[r++]=128|i>>>6&63,t[r++]=128|63&i):(t[r++]=240|i>>>18,t[r++]=128|i>>>12&63,t[r++]=128|i>>>6&63,t[r++]=128|63&i);return t},V=(e,t)=>{const i=t||e.length;if("function"==typeof TextDecoder&&TextDecoder.prototype.decode)return(new TextDecoder).decode(e.subarray(0,t));let n,a;const r=new Array(2*i);for(a=0,n=0;n<i;){let t=e[n++];if(t<128){r[a++]=t;continue}let o=J[t];if(o>4)r[a++]=65533,n+=o-1;else{for(t&=2===o?31:3===o?15:7;o>1&&n<i;)t=t<<6|63&e[n++],o--;o>1?r[a++]=65533:t<65536?r[a++]=t:(t-=65536,r[a++]=55296|t>>10&1023,r[a++]=56320|1023&t)}}return((e,t)=>{if(t<65534&&e.subarray&&q)return String.fromCharCode.apply(null,e.length===t?e:e.subarray(0,t));let i="";for(let n=0;n<t;n++)i+=String.fromCharCode(e[n]);return i})(r,a)},$=(e,t)=>{(t=t||e.length)>e.length&&(t=e.length);let i=t-1;for(;i>=0&&128==(192&e[i]);)i--;return i<0||0===i?t:i+J[e[i]]>t?i:t},ee={2:"need dictionary",1:"stream end",0:"","-1":"file error","-2":"stream error","-3":"data error","-4":"insufficient memory","-5":"buffer error","-6":"incompatible version"};var te=function(){this.input=null,this.next_in=0,this.avail_in=0,this.total_in=0,this.output=null,this.next_out=0,this.avail_out=0,this.total_out=0,this.msg="",this.state=null,this.data_type=2,this.adler=0};var ie=function(){this.text=0,this.time=0,this.xflags=0,this.os=0,this.extra=null,this.extra_len=0,this.name="",this.comment="",this.hcrc=0,this.done=!1};const ne=Object.prototype.toString,{Z_NO_FLUSH:ae,Z_FINISH:re,Z_OK:oe,Z_STREAM_END:se,Z_NEED_DICT:le,Z_STREAM_ERROR:de,Z_DATA_ERROR:fe,Z_MEM_ERROR:ce}=h;function he(e){this.options=X({chunkSize:65536,windowBits:15,to:""},e||{});const t=this.options;t.raw&&t.windowBits>=0&&t.windowBits<16&&(t.windowBits=-t.windowBits,0===t.windowBits&&(t.windowBits=-15)),!(t.windowBits>=0&&t.windowBits<16)||e&&e.windowBits||(t.windowBits+=32),t.windowBits>15&&t.windowBits<48&&0==(15&t.windowBits)&&(t.windowBits|=15),this.err=0,this.msg="",this.ended=!1,this.chunks=[],this.strm=new te,this.strm.avail_out=0;let i=Y.inflateInit2(this.strm,t.windowBits);if(i!==oe)throw new Error(ee[i]);if(this.header=new ie,Y.inflateGetHeader(this.strm,this.header),t.dictionary&&("string"==typeof t.dictionary?t.dictionary=Q(t.dictionary):"[object ArrayBuffer]"===ne.call(t.dictionary)&&(t.dictionary=new Uint8Array(t.dictionary)),t.raw&&(i=Y.inflateSetDictionary(this.strm,t.dictionary),i!==oe)))throw new Error(ee[i])}function ue(e,t){const i=new he(t);if(i.push(e),i.err)throw i.msg||ee[i.err];return i.result}he.prototype.push=function(e,t){const i=this.strm,n=this.options.chunkSize,a=this.options.dictionary;let r,o,s;if(this.ended)return!1;for(o=t===~~t?t:!0===t?re:ae,"[object ArrayBuffer]"===ne.call(e)?i.input=new Uint8Array(e):i.input=e,i.next_in=0,i.avail_in=i.input.length;;){for(0===i.avail_out&&(i.output=new Uint8Array(n),i.next_out=0,i.avail_out=n),r=Y.inflate(i,o),r===le&&a&&(r=Y.inflateSetDictionary(i,a),r===oe?r=Y.inflate(i,o):r===fe&&(r=le));i.avail_in>0&&r===se&&i.state.wrap>0&&0!==e[i.next_in];)Y.inflateReset(i),r=Y.inflate(i,o);switch(r){case de:case fe:case le:case ce:return this.onEnd(r),this.ended=!0,!1}if(s=i.avail_out,i.next_out&&(0===i.avail_out||r===se))if("string"===this.options.to){let e=$(i.output,i.next_out),t=i.next_out-e,a=V(i.output,e);i.next_out=t,i.avail_out=n-t,t&&i.output.set(i.output.subarray(e,e+t),0),this.onData(a)}else this.onData(i.output.length===i.next_out?i.output:i.output.subarray(0,i.next_out));if(r!==oe||0!==s){if(r===se)return r=Y.inflateEnd(this.strm),this.onEnd(r),this.ended=!0,!0;if(0===i.avail_in)break}}return!0},he.prototype.onData=function(e){this.chunks.push(e)},he.prototype.onEnd=function(e){e===oe&&("string"===this.options.to?this.result=this.chunks.join(""):this.result=W(this.chunks)),this.chunks=[],this.err=e,this.msg=this.strm.msg};var we=he,be=ue,me=function(e,t){return(t=t||{}).raw=!0,ue(e,t)},ke=ue,_e=h,ge={Inflate:we,inflate:be,inflateRaw:me,ungzip:ke,constants:_e};e.Inflate=we,e.constants=_e,e.default=ge,e.inflate=be,e.inflateRaw=me,e.ungzip=ke,Object.defineProperty(e,"__esModule",{value:!0})}));
 
 function fromZippedBase64(s) {
     let binary = atob(s);
```

### Comparing `robocorp_logging-0.0.8/src/robo_log/index.py` & `robocorp_logging-0.0.9/src/robo_log/_index.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Note: autogenerated file.
 # To regenerate this file use: python -m dev build-output-view.
 
 # The FILE_CONTENTS contains the contents of the files with
 # html/javascript code which can be used to visualize the contents of the
 # output generated by robocorp-logging (i.e.: the .robolog files).
 
-FILE_CONTENTS = {'index.html': '<!doctype html><html style="padding: 0 0 0 0; margin: 0 0 0 0; height: 100%"><head><meta charset="utf-8"/><title>Robot Output</title><meta name="viewport" content="width=device-width,initial-scale=1"/></head><body class="vscode-dark" style="padding: 0 0 0 0; margin: 0 0 0 0; height: 100%; display: flex; flex-direction: column"><div style="display: flex"><div class="summaryField" style="flex-grow: 1; white-space: nowrap" id="summary" class="NOT_RUN">Total:&nbsp;&nbsp;&nbsp;&nbsp;Failures:&nbsp;&nbsp;&nbsp;&nbsp;</div><div class="summaryField" style="flex-grow: 1"><div style="display: flex"><span>Filter:&nbsp;</span> <select name="filterLevel" id="filterLevel" style="flex-grow: 1" onchange="window.onChangedFilterLevel()"><option value="FAIL">FAIL</option><option value="WARN">WARN</option><option value="PASS" selected="selected">PASS</option><option value="NOT RUN">NOT RUN</option></select></div></div><div class="summaryField" id="selectRunContainer" style="flex-grow: 2; display: none"><select name="selectedRun" id="selectedRun" onchange="window.onChangedRun()" style="width: 100%"><option value="NO_RUN" selected="selected">No runs available...</option></select></div></div><div id="mainTree" style="white-space: nowrap; overflow: auto; flex-grow: 1"></div><script>(()=>{"use strict";var e={426:(e,n,t)=>{t.d(n,{Z:()=>a});var o=t(645),r=t.n(o)()((function(e){return e[1]}));r.push([e.id,":root {\\n    --fg-color: var(--vscode-editor-foreground, black);\\n    --bg-color: var(--vscode-editor-background, white);\\n    --font-family: var(--vscode-editor-font-family, monospace, courier);\\n    --font-size: var(--vscode-editor-font-size, 14px);\\n    --font-weight: var(--vscode-font-weight);\\n    --menu-background: var(--vscode-menu-background, rgb(235, 235, 235));\\n    --menu-foreground: var(--vscode-menu-foreground, rgb(0, 0, 0));\\n\\n    /* background-color: var(--vscode-editorError-foreground); */\\n    /* background-color: var(--vscode-inputValidation-errorBorder);  high-contrast doesn\'t have a good color */\\n    /* background-color: var(--vscode-testing-iconErrored);  red and green always (not always ideal...) */\\n    --error-background-color: var(--vscode-terminalCommandDecoration-errorBackground, rgb(201, 28, 28));\\n    --error-color: var(--vscode-button-foreground, white);\\n\\n    --hidden-background-color: var(--vscode-foobarcolornotthere, rgb(243, 152, 16));\\n    --hidden-color: var(--vscode-button-foreground, white);\\n\\n    /* background-color: var(--vscode-inputValidation-infoBorder); */\\n    /* background-color: var(--vscode-testing-iconPassed); */\\n    --pass-background-color: var(--vscode-terminalCommandDecoration-successBackground, rgb(36, 47, 202));\\n    --pass-color: var(--vscode-button-foreground, white);\\n\\n    --warn-background-color: var(--vscode-debugConsole-warningForeground, rgb(190, 159, 20));\\n    --warn-color: var(--vscode-button-foreground, white);\\n\\n    --not-run-background-color: var(--vscode-editor-foreground, rgb(102, 102, 102));\\n    --not-run-color: var(--vscode-editor-background, white);\\n\\n    --summary-hover-background-color: var(--vscode-editor-hoverHighlightBackground, rgb(222, 222, 222));\\n\\n    /* \\n    --fg-color: white;\\n    --bg-color: #4b4a4a;\\n    --font-family: \\"Segoe UI\\", Tahoma, Geneva, Verdana, sans-serif; \\n    */\\n}\\n\\n.summaryField {\\n    margin-left: 3px;\\n    margin-right: 3px;\\n}\\n\\n.summaryFileName {\\n    opacity: 0.6;\\n    margin-left: 1rem;\\n}\\n\\n.timeLabel {\\n    opacity: 0.6;\\n}\\n\\n/* .summaryInput {\\n    opacity: 0.6;\\n} */\\n\\n.summaryInput::before {\\n    margin-left: 3px;\\n    content: \\"(\\";\\n}\\n.summaryInput::after {\\n    margin-right: 3px;\\n    content: \\")\\";\\n}\\n\\n/* nesting level vertical line */\\n.detailInfo {\\n    border-left: 1px solid var(--error-background-color);\\n\\n    /* centering the line with the icon */\\n    margin-left: 1.5rem;\\n\\n    /* nesting indentation */\\n    padding-left: 0.8rem;\\n}\\n\\nbody {\\n    font-family: var(--font-family);\\n    font-size: var(--font-size);\\n    font-weight: var(--font-weight);\\n    color: var(--fg-color);\\n    background-color: var(--bg-color);\\n}\\n\\n#mainTree {\\n    margin-top: 5px;\\n}\\n\\nul {\\n    list-style-type: none;\\n    padding-inline-start: 0px;\\n    margin-block-start: 0px;\\n}\\n\\ndiv ul:not(:first-child) {\\n    border-left: 1px dotted rgb(141, 141, 141);\\n}\\n\\n.tree li {\\n    display: block;\\n    position: relative;\\n    padding-left: 0px;\\n}\\n\\n.tree ul {\\n    margin-left: 10px;\\n    padding-left: 0;\\n}\\n\\n.toolbarButton {\\n    display: inline;\\n    border-radius: 5px;\\n    background: var(--bg-color);\\n    color: var(--fg-color);\\n    margin-left: 3px;\\n    width: 15px;\\n    height: 15px;\\n    border: 0;\\n    padding: 0;\\n    vertical-align: middle;\\n}\\n\\n.toolbarContainer {\\n    display: inline-block;\\n}\\n\\n.summaryDiv {\\n    display: inline;\\n}\\n\\ndetails > summary {\\n    /* Note: couldn\'t get proper color with the svg approach */\\n    /* list-style-image: url(\\"data:image/svg+xml;utf8,<svg width=\'12px\' height=\'12px\' viewBox=\'0 0 20 20\' xmlns=\'http://www.w3.org/2000/svg\'><g data-name=\'Layer 2\'><g data-name=\'arrow-ios-forward\'><rect width=\'24\' height=\'24\' transform=\'rotate(-90 12 12)\' opacity=\'0\'/><path fill=\'currentColor\' stroke=\'currentColor\' d=\'M10 19a1 1 0 0 1-.64-.23 1 1 0 0 1-.13-1.41L13.71 12 9.39 6.63a1 1 0 0 1 .15-1.41 1 1 0 0 1 1.46.15l4.83 6a1 1 0 0 1 0 1.27l-5 6A1 1 0 0 1 10 19z\'/></g></g></svg>\\"); */\\n    /* list-style-type: \\"⮞ \\"; */\\n    /* list-style-type: \\"⏵\\"; */\\n    list-style-type: \\"+ \\";\\n}\\n\\ndetails[open] > summary {\\n    /* list-style-image: url(\\"data:image/svg+xml;utf8,<svg width=\'12px\' height=\'12px\' viewBox=\'0 0 20 20\' xmlns=\'http://www.w3.org/2000/svg\'><g data-name=\'Layer 2\'><g data-name=\'arrow-ios-downward\'><rect width=\'24\' height=\'24\' opacity=\'0\'/><path fill=\'currentColor\' stroke=\'currentColor\' d=\'M12 16a1 1 0 0 1-.64-.23l-6-5a1 1 0 1 1 1.28-1.54L12 13.71l5.36-4.32a1 1 0 0 1 1.41.15 1 1 0 0 1-.14 1.46l-6 4.83A1 1 0 0 1 12 16z\'/></g></g></svg>\\"); */\\n    /* list-style-type: \\"⮟ \\"; */\\n    /* list-style-type: \\"⏷\\"; */\\n    list-style-type: \\"- \\";\\n}\\n\\n.NO_CHILDREN > summary {\\n    list-style-type: \\"\xa0\xa0\\" !important;\\n}\\n\\nselect {\\n    background-color: var(--menu-background);\\n    color: var(--menu-foreground);\\n}\\n\\nsummary {\\n    padding: 3px;\\n}\\n\\na:link {\\n    color: var(--fg-color);\\n}\\n\\na:visited {\\n    color: var(--fg-color);\\n}\\n\\na:hover {\\n    color: var(--fg-color);\\n}\\n\\na:active {\\n    color: var(--fg-color);\\n}\\n\\n.label {\\n    padding: 2px 2px;\\n    font-size: 0.65em;\\n    letter-spacing: 1px;\\n    white-space: nowrap;\\n    border-radius: 3px;\\n    margin-right: 5px;\\n    font-weight: bold;\\n}\\n\\n.timeLabel {\\n    padding: 2px 2px;\\n    font-size: 0.85em;\\n    letter-spacing: 1px;\\n    white-space: nowrap;\\n    border-radius: 3px;\\n    margin-right: 5px;\\n    font-weight: lighter;\\n}\\n\\n.label.F,\\n.label.E,\\n.label.FAIL,\\n.label.ERROR {\\n    border-radius: 3px;\\n    background-color: var(--error-background-color);\\n    color: var(--error-color);\\n    font-weight: bolder;\\n}\\n\\n.label.PASS,\\n.label.I,\\n.label.INFO {\\n    border-radius: 3px;\\n    background-color: var(--pass-background-color);\\n    color: var(--pass-color);\\n    font-weight: bolder;\\n}\\n\\n.label.W,\\n.label.WARN {\\n    border-radius: 3px;\\n    background-color: var(--warn-background-color);\\n    color: var(--warn-color);\\n    font-weight: bolder;\\n}\\n\\n.label.HIDDEN {\\n    border-radius: 3px;\\n    background-color: var(--hidden-background-color);\\n    color: var(--hidden-color);\\n    font-weight: bolder;\\n}\\n.label.HIDDEN.inline {\\n    margin-left: 5px;\\n}\\n\\nsummary.HIDDEN {\\n    margin-top: 10px;\\n    margin-bottom: 10px;\\n}\\n\\n.label.NOT_RUN {\\n    border-radius: 3px;\\n    background-color: var(--not-run-background-color);\\n    color: var(--not-run-color);\\n    font-weight: bolder;\\n}\\n\\n#summary.FAIL,\\n#summary.ERROR {\\n    border-bottom: 5px solid var(--error-background-color);\\n}\\n\\n#summary.PASS {\\n    border-bottom: 5px solid var(--pass-background-color);\\n}\\n\\n#summary.NOT_RUN {\\n    border-bottom: 5px solid var(--not-run-background-color);\\n}\\n\\n/* .span_link::after {\\n    content: \\" ⮳\\";\\n} */\\n.span_link {\\n    cursor: pointer;\\n    /* text-decoration: underline; */\\n}\\n\\nsummary:hover {\\n    background-color: var(--summary-hover-background-color);\\n}\\n",""]);const a=r},645:e=>{e.exports=function(e){var n=[];return n.toString=function(){return this.map((function(n){var t=e(n);return n[2]?"@media ".concat(n[2]," {").concat(t,"}"):t})).join("")},n.i=function(e,t,o){"string"==typeof e&&(e=[[null,e,""]]);var r={};if(o)for(var a=0;a<this.length;a++){var s=this[a][0];null!=s&&(r[s]=!0)}for(var i=0;i<e.length;i++){var d=[].concat(e[i]);o&&r[d[0]]||(t&&(d[2]?d[2]="".concat(t," and ").concat(d[2]):d[2]=t),n.push(d))}},n}},391:(e,n,t)=>{let o;window.setVSCodeAPI=function(e){o=e};let r={};function a(e){let n;try{n=o}catch(e){}n&&n.postMessage(e)}let s={output:void 0},i={setContents:void 0,appendContents:void 0,updateLabel:void 0};window.addEventListener("message",(e=>{let n=e.data;if(n)switch(n.type){case"response":let e=n,t=r[e.request_seq];t&&(delete r[e.request_seq],t(e));break;case"event":let o=s[n.event];o?o(n):console.log("Unhandled event: ",n);break;case"request":let a=i[n.command];a?a(n):console.log("Unhandled request: ",n)}}));let d=0;function l(){return d+=1,d}let c={filterLevel:"PASS",runIdToTreeState:{},runIdLRU:[]},u={initialContents:void 0,runId:void 0,state:void 0,onClickReference:void 0,appendedContents:[],allRunIdsToLabel:{},showTime:!0,showExpand:!0};function m(){return void 0===u.state&&(u.state=function(){let e;try{e=o}catch(e){}if(e){let n=e.getState();return n||(n=c),void 0===n.filterLevel&&(n.filterLevel="PASS"),void 0===n.runIdToTreeState&&(n.runIdToTreeState={}),void 0===!n.runIdLRU&&(n.runIdLRU=[]),n}return c}()),u}function h(e){return document.getElementById(e)}function p(e){return h(e)}function f(e){return h(e)}function g(e){const n=document.createElement("ul");return n.setAttribute("data-tree-id",e),n}function v(){return document.createElement("span")}function y(){return document.createElement("button")}function b(){return document.createElement("div")}function S(e){return e.getAttribute("data-tree-id")}function C(e,n=undefined){if(void 0===n)return"1"===e.getAttribute("data-hidden");n?e.setAttribute("data-hidden","1"):e.removeAttribute("data-hidden")}function E(e){var n=document.createElement("template");return e=e.trim(),n.innerHTML=e,n.content.firstChild}function T(e,n){for(let t of n.childNodes)if(t instanceof HTMLDetailsElement){for(let n of t.childNodes)n instanceof HTMLUListElement&&w(e,n);t.open?e.openNodes[S(n)]="open":delete e.openNodes[S(n)]}}function w(e,n){for(let t of n.childNodes)t instanceof HTMLLIElement&&T(e,t)}const L=((e,n)=>{let t;return function(...e){clearTimeout(t),t=setTimeout((()=>{clearTimeout(t),(()=>{N()})(...e)}),500)}})();function N(){const e=m();!function(e,n){const t=p("mainTree");let o={openNodes:{}};if(void 0===e.runIdLRU&&(e.runIdLRU=[]),void 0===e.runIdToTreeState)e.runIdToTreeState={};else{const t=e.runIdToTreeState[n];t&&(o=t)}for(let e of t.childNodes)e instanceof HTMLUListElement&&w(o,e);e.runIdToTreeState[n]=o;const r=e.runIdLRU.indexOf(n);for(r>-1&&e.runIdLRU.splice(r,1),e.runIdLRU.push(n);e.runIdLRU.length>15;){const n=e.runIdLRU.splice(0,1);delete e.runIdToTreeState[n[0]]}}(e.state,e.runId),function(e){let n;try{n=o}catch(e){}n?n.setState(e):c=e}(e.state)}function x(e,n){if(void 0===e)return;const t=f("selectedRun"),o=new Map;for(let r of t.childNodes)if(r instanceof HTMLOptionElement){const t=r,a=t.value,s=e[a];if(void 0===s)r.remove();else{t.text!==s&&(t.text=s),o.set(a,s);const e=n==a;t.selected=e}}for(const r of Object.keys(e)){if(void 0===r)continue;const a=n==r;if(!o.has(r)){const n=document.createElement("option"),s=e[r];n.value=r,t.appendChild(n),n.selected=a,n.text=s,o.set(r,s)}}}Math.pow(10,8);var I=36e5;function M(e,n){var t;!function(e,n){if(n.length<1)throw new TypeError("1 argument required, but only "+n.length+" present")}(0,arguments);var o=function(e){if(null===e||!0===e||!1===e)return NaN;var n=Number(e);return isNaN(n)?n:n<0?Math.ceil(n):Math.floor(n)}(null!==(t=null==n?void 0:n.additionalDigits)&&void 0!==t?t:2);if(2!==o&&1!==o&&0!==o)throw new RangeError("additionalDigits must be 0, 1 or 2");if("string"!=typeof e&&"[object String]"!==Object.prototype.toString.call(e))return new Date(NaN);var r,a=function(e){var n,t={},o=e.split(k.dateTimeDelimiter);if(o.length>2)return t;if(/:/.test(o[0])?n=o[0]:(t.date=o[0],n=o[1],k.timeZoneDelimiter.test(t.date)&&(t.date=e.split(k.timeZoneDelimiter)[0],n=e.substr(t.date.length,e.length))),n){var r=k.timezone.exec(n);r?(t.time=n.replace(r[1],""),t.timezone=r[1]):t.time=n}return t}(e);if(a.date){var s=function(e,n){var t=new RegExp("^(?:(\\\\d{4}|[+-]\\\\d{"+(4+n)+"})|(\\\\d{2}|[+-]\\\\d{"+(2+n)+"})$)"),o=e.match(t);if(!o)return{year:NaN,restDateString:""};var r=o[1]?parseInt(o[1]):null,a=o[2]?parseInt(o[2]):null;return{year:null===a?r:100*a,restDateString:e.slice((o[1]||o[2]).length)}}(a.date,o);r=function(e,n){if(null===n)return new Date(NaN);var t=e.match(K);if(!t)return new Date(NaN);var o=!!t[4],r=A(t[1]),a=A(t[2])-1,s=A(t[3]),i=A(t[4]),d=A(t[5])-1;if(o)return function(e,n,t){return n>=1&&n<=53&&t>=0&&t<=6}(0,i,d)?function(e,n,t){var o=new Date(0);o.setUTCFullYear(e,0,4);var r=7*(n-1)+t+1-(o.getUTCDay()||7);return o.setUTCDate(o.getUTCDate()+r),o}(n,i,d):new Date(NaN);var l=new Date(0);return function(e,n,t){return n>=0&&n<=11&&t>=1&&t<=(F[n]||(O(e)?29:28))}(n,a,s)&&function(e,n){return n>=1&&n<=(O(e)?366:365)}(n,r)?(l.setUTCFullYear(n,a,Math.max(r,s)),l):new Date(NaN)}(s.restDateString,s.year)}if(!r||isNaN(r.getTime()))return new Date(NaN);var i,d=r.getTime(),l=0;if(a.time&&(l=function(e){var n=e.match(R);if(!n)return NaN;var t=D(n[1]),o=D(n[2]),r=D(n[3]);return function(e,n,t){return 24===e?0===n&&0===t:t>=0&&t<60&&n>=0&&n<60&&e>=0&&e<25}(t,o,r)?t*I+6e4*o+1e3*r:NaN}(a.time),isNaN(l)))return new Date(NaN);if(!a.timezone){var c=new Date(d+l),u=new Date(0);return u.setFullYear(c.getUTCFullYear(),c.getUTCMonth(),c.getUTCDate()),u.setHours(c.getUTCHours(),c.getUTCMinutes(),c.getUTCSeconds(),c.getUTCMilliseconds()),u}return i=function(e){if("Z"===e)return 0;var n=e.match(_);if(!n)return 0;var t="+"===n[1]?-1:1,o=parseInt(n[2]),r=n[3]&&parseInt(n[3])||0;return function(e,n){return n>=0&&n<=59}(0,r)?t*(o*I+6e4*r):NaN}(a.timezone),isNaN(i)?new Date(NaN):new Date(d+l+i)}var k={dateTimeDelimiter:/[T ]/,timeZoneDelimiter:/[Z ]/i,timezone:/([Z+-].*)$/},K=/^-?(?:(\\d{3})|(\\d{2})(?:-?(\\d{2}))?|W(\\d{2})(?:-?(\\d{1}))?|)$/,R=/^(\\d{2}(?:[.,]\\d*)?)(?::?(\\d{2}(?:[.,]\\d*)?))?(?::?(\\d{2}(?:[.,]\\d*)?))?$/,_=/^([+-])(\\d{2})(?::?(\\d{2}))?$/;function A(e){return e?parseInt(e):1}function D(e){return e&&parseFloat(e.replace(",","."))||0}var F=[31,null,31,30,31,30,31,31,30,31,30,31];function O(e){return e%400==0||e%4==0&&e%100!=0}function H(e,n){const t=e.memo[n];return void 0===t?`<ref not found: ${n}>`:t}function U(e,n){return parseFloat(n)}function B(e,n){return parseInt(n)}function j(e,n){return n}function P(e){const n=[],t=new Map;for(let o of e.split(",")){o=o.trim();let e="oid";if(-1!=o.indexOf(":")&&([o,e]=o.split(":",2)),n.push(o),"oid"===e)t.set(o,H);else if("int"===e)t.set(o,B);else if("float"===e)t.set(o,U);else{if("str"!==e)throw new Error("Unexpected: "+e);t.set(o,j)}}return function(e,o){const r=o.split("|",n.length),a={};for(let o=0;o<r.length;o++){const s=r[o],i=n[o];a[i]=t.get(i)(e,s)}return a}}const $=P("name:oid, time_delta_in_seconds:float"),z=P("status:oid, time_delta_in_seconds:float"),V=P("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),q=P("status:oid, message:oid, time_delta_in_seconds:float"),W=P("name:oid, libname:oid, type:oid, doc:oid, source:oid, lineno:int, time_delta_in_seconds:float"),J=P("status:oid, time_delta_in_seconds:float"),Y=P("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),Z={V:function(e,n){return{message:n}},ID:P("part:int, id:str"),I:function(e,n){return JSON.parse(n)},T:function(e,n){return{time:M(n).toString()}},M:function(e,n){var t,o;const r=Q(n,":");if(r){[t,o]=r;try{o=JSON.parse(o)}catch(e){return console.log("Error parsing json: "+o),console.log(e),null}e.memo[t]=o}return null},SR:$,RR:$,ER:z,ST:V,RT:V,ET:q,SE:W,RE:W,EE:J,EA:P("name:oid, value:oid"),L:Y,LH:Y,AS:P("assign:oid"),TG:P("tag:oid"),S:P("start_time_delta:float"),STB:P("message:oid, time_delta_in_seconds:float"),RTB:P("message:oid, time_delta_in_seconds:float"),TBE:P("source:oid, lineno:int, method:oid, line_content:oid"),TBV:P("name:oid, type:oid, value:oid"),ETB:P("time_delta_in_seconds:float")};class G{constructor(){this.memo={}}decode_message_type(e,n){return(0,Z[e])(this,n)}}function Q(e,n){const t=e.indexOf(n);if(t>0)return[e.substring(0,t),e.substring(t+1)]}function*X(e,n){var t,o,r;for(let a of e.split(/\\r?\\n/))if(a=a.trim(),a){const e=Q(a," ");if(e&&([r,o]=e,t=n.decode_message_type(r,o))){const e={message_type:r,decoded:t};yield e}}}function ee(e,n){const t=document.createElement("span");t.textContent=n,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}function ne(e,n){switch(e.state.filterLevel){case"FAIL":return n>=2;case"WARN":return n>=1;case"PASS":return n>=0;case"NOT RUN":return!0}}function te(e){switch(e){case"FAIL":case"ERROR":return 2;case"WARN":return 1;case"NOT RUN":case"NOT_RUN":return-1;default:return 0}}class oe{constructor(e){this.stack=[],this.exceptionMsg=e}pushEntry(e,n,t,o){const r=new Map;this.stack.push({source:e,lineno:n,method:t,lineContent:o,variables:r})}pushVar(e,n,t){this.stack.at(-1).variables.set(`${e} (${n})`,`${t}`)}}class re{constructor(){this.totalTests=0,this.totalFailures=0}clear(){this.totalTests=0,this.totalFailures=0,this.updateSummary()}onTestEndUpdateSummary(e){const n=e.decoded.status;this.totalTests+=1,"FAIL"!=n&&"ERROR"!=n||(this.totalFailures+=1),this.updateSummary()}updateSummary(){const e=p("summary");if(!e)return;const n=(""+this.totalTests).padStart(4),t=(""+this.totalFailures).padStart(4);if(e.textContent=`Total: ${n} Failures: ${t}`,0==this.totalFailures&&0==this.totalTests){const e=p("summary");e.classList.add("NOT_RUN"),e.classList.remove("PASS"),e.classList.remove("FAIL")}else if(1==this.totalFailures){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("PASS"),e.classList.add("FAIL")}else if(0==this.totalFailures&&1==this.totalTests){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("FAIL")}}}function ae(e,n){const t=function(e){const n=document.createElement("li");return n.setAttribute("data-tree-id",e),n}(n),o=document.createElement("details");e&&(o.open=e),o.classList.add("NO_CHILDREN"),t.appendChild(o);const r=b();r.classList.add("detailContainer"),o.appendChild(r);const a=document.createElement("summary"),s=b();s.classList.add("summaryDiv"),a.appendChild(s);const i=v();i.className="summaryName",i.textContent="[summaryName]",s.appendChild(i);const d=v();return d.className="summaryInput emptySummaryInput",d.textContent="",s.appendChild(d),o.appendChild(a),{li:t,details:o,summary:a,summaryDiv:s,summaryName:i,summaryInput:d,detailContainer:r}}function se(e,n,t,o,r,a,s,i,d,l){const c=e.state.runIdToTreeState[e.runId],u="li_"+l;if(c){const e=c.openNodes;e&&(a=e[u])}const m=ae(a,u),h=m.li,p=m.details,f=m.detailContainer,v=m.summary,y=m.summaryDiv,b=m.summaryName,S=m.summaryInput;if("LH"===r.message_type){b.textContent="";const e=E(t);b.appendChild(e)}else b.textContent=t;o&&(b.title=o),e.onClickReference&&(b.classList.add("span_link"),b.onclick=n=>{const t=[];let o=d.parent;for(;void 0!==o&&void 0!==o.message;)t.push(o.message),o=o.parent;n.preventDefault(),e.onClickReference({source:s,lineno:i,message:r.decoded,messageType:r.message_type,scope:t})});const C=g("ul_"+l);p.appendChild(C);const T={ul:C,li:h,details:p,detailContainer:f,summary:v,summaryName:b,summaryInput:S,source:s,lineno:i,appendContentChild:void 0,decodedMessage:r,maxLevelFoundInHierarchy:-1,summaryDiv:y};return T.appendContentChild=ue.bind(T),n.appendContentChild(T),T}let ie,de;function*le(e){for(let n of e.childNodes)if(n instanceof HTMLDetailsElement){for(let e of n.childNodes)if(e instanceof HTMLUListElement)for(let n of ce(e))yield n;yield n}}function*ce(e){for(let n of e.childNodes)if(n instanceof HTMLLIElement)for(let e of le(n))yield e}function ue(e){const n=this;n.ul.appendChild(e.li),n.details.classList.contains("NO_CHILDREN")&&(n.details.classList.remove("NO_CHILDREN"),n.details.addEventListener("toggle",(function(){L()})),m().showExpand&&n.summary.addEventListener("mouseover",(e=>{!function(e){if(void 0===ie){ie=b(),ie.classList.add("toolbarContainer");const e=y();e.appendChild(E(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path d="M7 12V7H6v5h1z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),e.onclick=()=>{!function(){if(void 0!==de){de.details.open=!0;for(let e of ce(de.ul))e.classList.contains("NO_CHILDREN")||(e.open=!0)}}()},e.classList.add("toolbarButton");const n=y();return n.appendChild(E(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),n.classList.add("toolbarButton"),n.onclick=()=>{!function(){if(void 0!==de){de.details.open=!1;for(let e of ce(de.ul))e.open=!1}}()},ie.appendChild(n),void ie.appendChild(e)}de=e,e.summaryDiv.appendChild(ie)}(n)})))}var me=(e,n,t)=>new Promise(((o,r)=>{var a=e=>{try{i(t.next(e))}catch(e){r(e)}},s=e=>{try{i(t.throw(e))}catch(e){r(e)}},i=e=>e.done?o(e.value):Promise.resolve(e.value).then(a,s);i((t=t.apply(e,n)).next())}));let he=0,pe=-1;class fe{constructor(){this.stack=[]}handle(e){let n;switch(e.message_type){case"STB":return void this.stack.push(new oe(e.decoded.message));case"TBE":return n=this.stack.at(-1),void n.pushEntry(e.decoded.source,e.decoded.lineno,e.decoded.method,e.decoded.line_content);case"TBV":return n=this.stack.at(-1),void n.pushVar(e.decoded.name,e.decoded.type,e.decoded.value);case"ETB":return n=this.stack.pop(),n.stack.reverse(),n}}}class ge{constructor(){this.stack=[],this.messageNode={parent:void 0,message:void 0},this.id=0,this.finishedAddingInitialContents=!1,this.appendedMessagesIndex=-1,this.decoder=new G,this.seenSuiteTaskOrElement=!1,this.tbHandler=new fe,this.suiteErrored=!1,this.opts=m(),this.runId=this.opts.runId,this.summaryBuilder=new re,this.lease=(he+=1,pe=he,he),this.resetState()}resetState(){this.seenSuiteTaskOrElement=!1}isCurrentTreeBuilder(){return this.lease===pe&&this.runId==this.opts.runId}clearAndInitializeTree(){this.summaryBuilder.clear(),this.resetState();const e=f("filterLevel");e&&(e.value=this.opts.state.filterLevel);const n=p("mainTree");n.replaceChildren();const t=g("ul_root");t.classList.add("tree"),n.appendChild(t),this.parent={ul:void 0,li:void 0,details:void 0,detailContainer:void 0,summary:void 0,summaryName:void 0,summaryInput:void 0,source:void 0,lineno:void 0,decodedMessage:void 0,appendContentChild:function(e){t.appendChild(e.li)},maxLevelFoundInHierarchy:-1,summaryDiv:void 0},this.stack.push(this.parent)}addInitialContents(){return me(this,null,(function*(){for(const e of X(this.opts.initialContents,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}this.finishedAddingInitialContents=!0,yield this.onAppendedContents()}))}onAppendedContents(){return me(this,null,(function*(){if(!this.finishedAddingInitialContents)return;if(!this.isCurrentTreeBuilder())return;const e=m();for(;this.appendedMessagesIndex+1<e.appendedContents.length;){this.appendedMessagesIndex+=1;const n=e.appendedContents[this.appendedMessagesIndex];for(const e of X(n,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}}}))}addOneMessage(e){return me(this,null,(function*(){if(this.isCurrentTreeBuilder())try{this.addOneMessageSync(e)}catch(n){console.log("Error: handling message: "+JSON.stringify(e)+": "+n+" - "+JSON.stringify(n))}}))}addOneMessageSync(e){var n,t;let o,r=e.message_type;switch(r){case"SR":case"ST":case"SE":case"STB":this.seenSuiteTaskOrElement=!0;break;case"RR":if(this.seenSuiteTaskOrElement)return;r="SR";break;case"RT":if(this.seenSuiteTaskOrElement)return;r="ST";break;case"RE":if(this.seenSuiteTaskOrElement)return;r="SE";break;case"RTB":if(this.seenSuiteTaskOrElement)return;r="STB"}switch(this.id+=1,r){case"SR":this.messageNode={parent:this.messageNode,message:e};for(const n of document.querySelectorAll(".suiteHeader"))n.textContent=e.decoded.name;break;case"ST":this.messageNode={parent:this.messageNode,message:e},this.parent=se(this.opts,this.parent,`${e.decoded.libname}.${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"SE":this.messageNode={parent:this.messageNode,message:e},this.parent=se(this.opts,this.parent,e.decoded.name,e.decoded.libname,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"ER":this.messageNode=this.messageNode.parent;{const n=p("suiteResult");n.style.display="block",this.suiteErrored?(n.classList.add("ERROR"),n.textContent="Run Failed"):(n.classList.add("PASS"),n.textContent="Run Passed");const t=p("suiteRunStart");t&&(t.textContent+=` - Finished in: ${e.decoded.time_delta_in_seconds.toFixed(2)}s.`)}break;case"ET":this.messageNode=this.messageNode.parent;const r=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(r,this.parent,e),this.onEndSetStatusOrRemove(this.opts,r,e.decoded,this.parent,!1),this.summaryBuilder.onTestEndUpdateSummary(e),o=this.addDetailsCSSClasses(e.decoded.status,r),o&&(this.suiteErrored=!0,r.details.open=!0);break;case"EE":this.messageNode=this.messageNode.parent;let a=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(a,this.parent,e),this.onEndSetStatusOrRemove(this.opts,a,e.decoded,this.parent,!0),o=this.addDetailsCSSClasses(e.decoded.status,a),o&&(a.details.open=!0);break;case"S":const s=e.decoded.start_time_delta;(null==(t=null==(n=this.parent)?void 0:n.decodedMessage)?void 0:t.decoded)&&(this.parent.decodedMessage.decoded.time_delta_in_seconds=s);break;case"EA":const i=this.stack.at(-1);i.summaryInput.classList.contains("emptySummaryInput")?(i.summaryInput.textContent=`${e.decoded.name}=${e.decoded.value}`,i.summaryInput.classList.remove("emptySummaryInput")):i.summaryInput.textContent+=`, ${e.decoded.name}=${e.decoded.value}`;break;case"L":case"LH":const d=e.decoded.level,l=function(e){switch(e){case"E":case"F":return 2;case"W":return 1;default:return 0}}(d);if(l>this.parent.maxLevelFoundInHierarchy&&(this.parent.maxLevelFoundInHierarchy=l),ne(this.opts,l)){const n=se(this.opts,this.parent,e.decoded.message,"",e,!1,void 0,void 0,this.messageNode,this.id.toString());n.maxLevelFoundInHierarchy=l,function(e,n){const t=document.createElement("span");t.textContent=`LOG ${function(e){switch(e){case"E":return"ERROR";case"F":return"FAIL";case"W":return"WARN";case"I":return"INFO";default:return e}}(n)}`,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}(n,d),this.addDetailsCSSClasses(l,n)}break;case"STB":case"TBE":case"TBV":case"ETB":const c=this.tbHandler.handle(e);c&&function(e,n){const t=b();t.classList.add("detailInfo");const o=b();o.classList.add("errorHeader"),o.textContent=n.exceptionMsg,t.appendChild(o);const r=[];for(const e of n.stack){let n=e.source;n.length>31&&(n=`... ${n.substring(27)}`),r.push(`File "${n}", line ${e.lineno}, in ${e.method}\\n`),r.push(`    ${e.lineContent}\\n`);for(const[n,t]of e.variables.entries())r.push(`        💠 ${n} = ${t}\\n`)}const a=b();a.classList.add("errorDetails"),a.style.whiteSpace="pre",a.textContent=r.join(""),t.appendChild(a),e.detailContainer.appendChild(t);const s=b();s.classList.add("detailInputs"),s.textContent=" ",e.detailContainer.appendChild(s),e.details.classList.add("parentNode")}(this.parent,c);break;case"T":const u=p("suiteRunStart");u&&(u.textContent=e.decoded.time)}}addDetailsCSSClasses(e,n){let t,o=!1;return t="string"==typeof e?te(e):e,t>=2?(n.details.classList.add("errorParent"),o=!0):1==t?n.details.classList.add("warnParent"):n.details.classList.add("passParent"),n.details.classList.contains("parentNode")||n.details.classList.contains("leafNode")||(0===n.ul.children.length?n.details.classList.add("leafNode"):n.details.classList.add("parentNode")),o}onEndUpdateMaxLevelFoundInHierarchyFromStatus(e,n,t){const o=te(t.decoded.status);o>e.maxLevelFoundInHierarchy&&(e.maxLevelFoundInHierarchy=o),e.maxLevelFoundInHierarchy>n.maxLevelFoundInHierarchy&&(n.maxLevelFoundInHierarchy=e.maxLevelFoundInHierarchy)}onEndSetStatusOrRemove(e,n,t,o,r){const a=t.status;if(ne(e,n.maxLevelFoundInHierarchy)){if(r&&n.maxLevelFoundInHierarchy<=0){const e=50;if(o.ul.childElementCount>e){const e=n.summaryName.textContent;if(e&&e.toLowerCase().includes("iteration")){const e=n.li.previousSibling,t=S(n.li);if(n.li.remove(),C(e))e.getElementsByClassName("FINAL_SPAN")[0].textContent=n.summaryName.textContent;else{const e=ae(!1,t);e.summaryName.textContent=n.summaryName.textContent,e.summary.classList.add("HIDDEN");const r=v();r.setAttribute("role","button"),r.textContent="...",r.classList.add("label"),r.classList.add("HIDDEN"),r.classList.add("inline"),e.summaryDiv.appendChild(r);const a=v();a.setAttribute("role","button"),a.classList.add("FINAL_SPAN"),e.summaryDiv.appendChild(a),ee(e,"HIDDEN"),C(e.li,!0),o.ul.appendChild(e.li)}return}}}if(n.summary,ee(n,a),null!=n.source&&n.source.length>0){const e=function(e){let n=e,t=Math.max(e.lastIndexOf("/"),e.lastIndexOf("\\\\"));return t>0&&(n=e.substring(t+1)),n}(n.source),t=document.createElement("span");t.textContent=e,t.classList.add("summaryFileName"),t.title=n.source,n.summaryDiv.appendChild(t)}if(this.opts.showTime){const e=n.decodedMessage.decoded.time_delta_in_seconds;void 0!==e&&e>=0&&function(e,n){const t=document.createElement("span");t.textContent=` (${n.toFixed(2)}s)`,t.classList.add("timeLabel"),e.summaryDiv.appendChild(t)}(n,t.time_delta_in_seconds-e)}}else n.li.remove()}}var ve=(e,n,t)=>new Promise(((o,r)=>{var a=e=>{try{i(t.next(e))}catch(e){r(e)}},s=e=>{try{i(t.throw(e))}catch(e){r(e)}},i=e=>e.done?o(e.value):Promise.resolve(e.value).then(a,s);i((t=t.apply(e,n)).next())}));let ye;function be(){return ve(this,null,(function*(){ye=new ge,ye.clearAndInitializeTree(),yield ye.addInitialContents()}))}function Se(e){let n={type:"event",seq:l(),event:"onClickReference"};n.data=e,a(n)}function Ce(e){N();const n=m();n.runId=e.runId,n.initialContents=e.initialContents,void 0!==o&&(n.onClickReference=Se),n.appendedContents=[],n.allRunIdsToLabel=e.allRunIdsToLabel,x(n.allRunIdsToLabel,n.runId),be()}t(320),i.setContents=Ce,i.appendContents=function(e){const n=m();n.runId===e.runId&&(n.appendedContents.push(e.appendContents),void 0!==ye&&ye.onAppendedContents())},i.updateLabel=function(e){const n=m();n.allRunIdsToLabel[e.runId]=e.label,x(n.allRunIdsToLabel,n.runId)},window.onChangedRun=function(){const e=f("selectedRun").value;let n={type:"event",seq:l(),event:"onSetCurrentRunId"};n.data={runId:e},a(n)},window.onChangedFilterLevel=function(){!function(e){const n=m();n.state.filterLevel!==e&&(n.state.filterLevel=e,N(),be())}(f("filterLevel").value)},window.setContents=Ce,window.setShowTime=function(e){m().showTime=e},window.setShowExpand=function(e){m().showExpand=e},window.getSampleContents=function(){return JSON.parse(\'"V 1\\\\nI \\\\"sys.platform=win32\\\\"\\\\nI \\\\"python=3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)]\\\\"\\\\nI \\\\"robot=5.1a3.dev1\\\\"\\\\nT 2022-10-19T09:48:34.018\\\\nM a:\\\\"Robot1\\\\"\\\\nM b:\\\\"s1\\\\"\\\\nM c:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\robot1.robot\\\\"\\\\nSS a|b|c|0.035\\\\nM d:\\\\"Simple Task\\\\"\\\\nM e:\\\\"s1-t1\\\\"\\\\nST d|e|16|0.036\\\\nM f:\\\\"First keyword\\\\"\\\\nM g:\\\\"\\\\"\\\\nM h:\\\\"KEYWORD\\\\"\\\\nSK f|g|h|g|c|17|0.036\\\\nM i:\\\\"No Operation\\\\"\\\\nM j:\\\\"BuiltIn\\\\"\\\\nM k:\\\\"Does absolutely nothing.\\\\"\\\\nSK i|j|h|k|c|8|0.037\\\\nM l:\\\\"PASS\\\\"\\\\nEK l|0.037\\\\nM m:\\\\"Log\\\\"\\\\nM n:\\\\"Logs the given message with the given level.\\\\"\\\\nSK m|j|h|n|c|10|0.037\\\\nM o:\\\\"Some warning message\\\\"\\\\nKA o\\\\nM p:\\\\"level=WARN\\\\"\\\\nKA p\\\\nEK l|0.046\\\\nM q:\\\\"Another keyword\\\\"\\\\nM r:\\\\"another\\\\"\\\\nSK q|r|h|g|c|11|0.047\\\\nM s:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\another.robot\\\\"\\\\nSK i|j|h|k|s|3|0.047\\\\nEK l|0.047\\\\nEK l|0.047\\\\nM t:\\\\"Another in sub keyword\\\\"\\\\nM u:\\\\"another_sub\\\\"\\\\nSK t|u|h|g|c|12|0.047\\\\nM v:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\sub\\\\\\\\\\\\\\\\another_sub.robot\\\\"\\\\nSK i|j|h|k|v|6|0.048\\\\nEK l|0.048\\\\nSK m|j|h|n|v|7|0.048\\\\nM w:\\\\"Some error message\\\\"\\\\nKA w\\\\nM x:\\\\"level=ERROR\\\\"\\\\nKA x\\\\nEK l|0.049\\\\nEK l|0.049\\\\nEK l|0.049\\\\nSK m|j|h|n|c|18|0.049\\\\nM y:\\\\"Some <data &encode <\\/script>\\\\"\\\\nKA y\\\\nEK l|0.049\\\\nM z:\\\\"Create Dictionary\\\\"\\\\nM A:\\\\"Creates and returns a dictionary based on the given ``items``.\\\\"\\\\nSK z|j|h|A|c|19|0.049\\\\nM B:\\\\"a=1\\\\"\\\\nKA B\\\\nM C:\\\\"b=1\\\\"\\\\nKA C\\\\nEK l|0.05\\\\nSK m|j|h|n|c|20|0.05\\\\nM D:\\\\"${dct}\\\\"\\\\nKA D\\\\nEK l|0.051\\\\nET l|g|0.051\\\\nM E:\\\\"Check 1\\\\"\\\\nM F:\\\\"s1-t2\\\\"\\\\nST E|F|22|0.051\\\\nSK f|g|h|g|c|23|0.051\\\\nSK i|j|h|k|c|8|0.052\\\\nEK l|0.052\\\\nSK m|j|h|n|c|10|0.052\\\\nKA o\\\\nKA p\\\\nEK l|0.052\\\\nSK q|r|h|g|c|11|0.053\\\\nSK i|j|h|k|s|3|0.053\\\\nEK l|0.053\\\\nEK l|0.053\\\\nSK t|u|h|g|c|12|0.053\\\\nSK i|j|h|k|v|6|0.054\\\\nEK l|0.054\\\\nSK m|j|h|n|v|7|0.054\\\\nKA w\\\\nKA x\\\\nEK l|0.054\\\\nEK l|0.055\\\\nEK l|0.055\\\\nM G:\\\\"${counter} IN RANGE [ 0 | 3 ]\\\\"\\\\nM H:\\\\"FOR\\\\"\\\\nSK G|g|H|g|c|25|0.055\\\\nM I:\\\\"${counter} = 0\\\\"\\\\nM J:\\\\"ITERATION\\\\"\\\\nSK I|g|J|g|c|25|0.055\\\\nM K:\\\\"${counter} == 2\\\\"\\\\nM L:\\\\"IF\\\\"\\\\nSK K|g|L|g|c|26|0.055\\\\nM M:\\\\"Fail\\\\"\\\\nM N:\\\\"Fails the test with the given message and optionally alters its tags.\\\\"\\\\nSK M|j|h|N|c|27|0.056\\\\nM O:\\\\"Failed execution for some reason...\\\\"\\\\nKA O\\\\nM P:\\\\"NOT RUN\\\\"\\\\nEK P|0.056\\\\nEK P|0.056\\\\nSK m|j|h|n|c|29|0.056\\\\nM Q:\\\\"${counter}\\\\"\\\\nKA Q\\\\nEK l|0.056\\\\nEK l|0.057\\\\nM R:\\\\"${counter} = 1\\\\"\\\\nSK R|g|J|g|c|25|0.057\\\\nSK K|g|L|g|c|26|0.057\\\\nSK M|j|h|N|c|27|0.057\\\\nKA O\\\\nEK P|0.057\\\\nEK P|0.057\\\\nSK m|j|h|n|c|29|0.058\\\\nKA Q\\\\nEK l|0.058\\\\nEK l|0.058\\\\nM S:\\\\"${counter} = 2\\\\"\\\\nSK S|g|J|g|c|25|0.058\\\\nSK K|g|L|g|c|26|0.058\\\\nSK M|j|h|N|c|27|0.059\\\\nKA O\\\\nM T:\\\\"FAIL\\\\"\\\\nEK T|0.059\\\\nEK T|0.059\\\\nSK m|j|h|n|c|29|0.059\\\\nKA Q\\\\nEK P|0.059\\\\nEK T|0.06\\\\nEK T|0.06\\\\nET T|O|0.06\\\\nM U:\\\\"Check 2\\\\"\\\\nM V:\\\\"s1-t3\\\\"\\\\nST U|V|32|0.06\\\\nM W:\\\\"Set Variable\\\\"\\\\nM X:\\\\"Returns the given values which can then be assigned to a variables.\\\\"\\\\nSK W|j|h|X|c|33|0.061\\\\nM Y:\\\\"3\\\\"\\\\nKA Y\\\\nEK l|0.061\\\\nM Z:\\\\"${counter} <= 2\\\\"\\\\nM 0:\\\\"WHILE\\\\"\\\\nSK Z|g|0|g|c|34|0.061\\\\nSK g|g|J|g|c|34|0.062\\\\nM 1:\\\\"Evaluate\\\\"\\\\nM 2:\\\\"Evaluates the given expression in Python and returns the result.\\\\"\\\\nSK 1|j|h|2|c|35|0.062\\\\nM 4:\\\\"$counter-1\\\\"\\\\nKA 4\\\\nEK P|0.062\\\\nSK m|j|h|n|c|36|0.062\\\\nM 5:\\\\"Current counter: ${counter}\\\\"\\\\nKA 5\\\\nKA p\\\\nEK P|0.062\\\\nEK P|0.062\\\\nEK P|0.063\\\\nET l|g|0.063\\\\nM 6:\\\\"Check 3\\\\"\\\\nM 7:\\\\"s1-t4\\\\"\\\\nST 6|7|39|0.064\\\\nM 8:\\\\"TRY\\\\"\\\\nSK g|g|8|g|c|40|0.064\\\\nSK i|j|h|k|c|41|0.064\\\\nEK l|0.064\\\\nEK l|0.064\\\\nM 9:\\\\"message\\\\"\\\\nM aa:\\\\"EXCEPT\\\\"\\\\nSK 9|g|aa|g|c|42|0.064\\\\nSK i|j|h|k|c|43|0.065\\\\nEK P|0.065\\\\nEK P|0.065\\\\nM ab:\\\\"FINALLY\\\\"\\\\nSK g|g|ab|g|c|44|0.065\\\\nSK i|j|h|k|c|45|0.065\\\\nEK l|0.065\\\\nEK l|0.065\\\\nET l|g|0.066\\\\nES T|0.067\\\\n"\')}},320:(e,n,t)=>{var o=t(379),r=t.n(o),a=t(426),s={injectType:"singletonStyleTag",insert:"head",singleton:!0};r()(a.Z,s),a.Z.locals},379:(e,n,t)=>{var o,r=function(){var e={};return function(n){if(void 0===e[n]){var t=document.querySelector(n);if(window.HTMLIFrameElement&&t instanceof window.HTMLIFrameElement)try{t=t.contentDocument.head}catch(e){t=null}e[n]=t}return e[n]}}(),a=[];function s(e){for(var n=-1,t=0;t<a.length;t++)if(a[t].identifier===e){n=t;break}return n}function i(e,n){for(var t={},o=[],r=0;r<e.length;r++){var i=e[r],d=n.base?i[0]+n.base:i[0],l=t[d]||0,c="".concat(d," ").concat(l);t[d]=l+1;var u=s(c),m={css:i[1],media:i[2],sourceMap:i[3]};-1!==u?(a[u].references++,a[u].updater(m)):a.push({identifier:c,updater:f(m,n),references:1}),o.push(c)}return o}function d(e){var n=document.createElement("style"),o=e.attributes||{};if(void 0===o.nonce){var a=t.nc;a&&(o.nonce=a)}if(Object.keys(o).forEach((function(e){n.setAttribute(e,o[e])})),"function"==typeof e.insert)e.insert(n);else{var s=r(e.insert||"head");if(!s)throw new Error("Couldn\'t find a style target. This probably means that the value for the \'insert\' parameter is invalid.");s.appendChild(n)}return n}var l,c=(l=[],function(e,n){return l[e]=n,l.filter(Boolean).join("\\n")});function u(e,n,t,o){var r=t?"":o.media?"@media ".concat(o.media," {").concat(o.css,"}"):o.css;if(e.styleSheet)e.styleSheet.cssText=c(n,r);else{var a=document.createTextNode(r),s=e.childNodes;s[n]&&e.removeChild(s[n]),s.length?e.insertBefore(a,s[n]):e.appendChild(a)}}function m(e,n,t){var o=t.css,r=t.media,a=t.sourceMap;if(r?e.setAttribute("media",r):e.removeAttribute("media"),a&&"undefined"!=typeof btoa&&(o+="\\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a))))," */")),e.styleSheet)e.styleSheet.cssText=o;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(o))}}var h=null,p=0;function f(e,n){var t,o,r;if(n.singleton){var a=p++;t=h||(h=d(n)),o=u.bind(null,t,a,!1),r=u.bind(null,t,a,!0)}else t=d(n),o=m.bind(null,t,n),r=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(t)};return o(e),function(n){if(n){if(n.css===e.css&&n.media===e.media&&n.sourceMap===e.sourceMap)return;o(e=n)}else r()}}e.exports=function(e,n){(n=n||{}).singleton||"boolean"==typeof n.singleton||(n.singleton=(void 0===o&&(o=Boolean(window&&document&&document.all&&!window.atob)),o));var t=i(e=e||[],n);return function(e){if(e=e||[],"[object Array]"===Object.prototype.toString.call(e)){for(var o=0;o<t.length;o++){var r=s(t[o]);a[r].references--}for(var d=i(e,n),l=0;l<t.length;l++){var c=s(t[l]);0===a[c].references&&(a[c].updater(),a.splice(c,1))}t=d}}}}},n={};function t(o){var r=n[o];if(void 0!==r)return r.exports;var a=n[o]={id:o,exports:{}};return e[o](a,a.exports,t),a.exports}t.n=e=>{var n=e&&e.__esModule?()=>e.default:()=>e;return t.d(n,{a:n}),n},t.d=(e,n)=>{for(var o in n)t.o(n,o)&&!t.o(e,o)&&Object.defineProperty(e,o,{enumerable:!0,get:n[o]})},t.o=(e,n)=>Object.prototype.hasOwnProperty.call(e,n),t.nc=void 0,t(391),t(320)})();</script></body><script>window.setShowTime(true);\n    window.setShowExpand(true);\n    try {\n        const vscode = acquireVsCodeApi();\n        window.setVSCodeAPI(vscode);\n        document.getElementById("selectRunContainer").style.display = "block";\n    } catch (err) {\n        // That\'s ok (not running in VSCode).\n        window.setContents({\n            "initialContents": window.getSampleContents(),\n        });\n    }</script></html>'}
+FILE_CONTENTS = {'index.html': '<!doctype html><html style="padding: 0 0 0 0; margin: 0 0 0 0; height: 100%"><head><meta charset="utf-8"/><title>Robot Output</title><meta name="viewport" content="width=device-width,initial-scale=1"/></head><body class="vscode-dark" style="padding: 0 0 0 0; margin: 0 0 0 0; height: 100%; display: flex; flex-direction: column"><div style="display: flex"><div class="summaryField" style="flex-grow: 1; white-space: nowrap" id="summary" class="NOT_RUN">Total:&nbsp;&nbsp;&nbsp;&nbsp;Failures:&nbsp;&nbsp;&nbsp;&nbsp;</div><div class="summaryField" style="flex-grow: 1"><div style="display: flex"><span>Filter:&nbsp;</span> <select name="filterLevel" id="filterLevel" style="flex-grow: 1" onchange="window.onChangedFilterLevel()"><option value="FAIL">FAIL</option><option value="WARN">WARN</option><option value="PASS" selected="selected">PASS</option><option value="NOT RUN">NOT RUN</option></select></div></div><div class="summaryField" id="selectRunContainer" style="flex-grow: 2; display: none"><select name="selectedRun" id="selectedRun" onchange="window.onChangedRun()" style="width: 100%"><option value="NO_RUN" selected="selected">No runs available...</option></select></div></div><div id="mainTree" style="white-space: nowrap; overflow: auto; flex-grow: 1"></div><script>(()=>{"use strict";var e={426:(e,t,n)=>{n.d(t,{Z:()=>s});var o=n(645),r=n.n(o)()((function(e){return e[1]}));r.push([e.id,":root {\\n    --fg-color: var(--vscode-editor-foreground, black);\\n    --bg-color: var(--vscode-editor-background, white);\\n    --font-family: var(--vscode-editor-font-family, monospace, courier);\\n    --font-size: var(--vscode-editor-font-size, 14px);\\n    --font-weight: var(--vscode-font-weight);\\n    --menu-background: var(--vscode-menu-background, rgb(235, 235, 235));\\n    --menu-foreground: var(--vscode-menu-foreground, rgb(0, 0, 0));\\n\\n    /* background-color: var(--vscode-editorError-foreground); */\\n    /* background-color: var(--vscode-inputValidation-errorBorder);  high-contrast doesn\'t have a good color */\\n    /* background-color: var(--vscode-testing-iconErrored);  red and green always (not always ideal...) */\\n    --error-background-color: var(--vscode-terminalCommandDecoration-errorBackground, rgb(201, 28, 28));\\n    --error-color: var(--vscode-button-foreground, white);\\n\\n    --hidden-background-color: var(--vscode-foobarcolornotthere, rgb(243, 152, 16));\\n    --hidden-color: var(--vscode-button-foreground, white);\\n\\n    /* background-color: var(--vscode-inputValidation-infoBorder); */\\n    /* background-color: var(--vscode-testing-iconPassed); */\\n    --pass-background-color: var(--vscode-terminalCommandDecoration-successBackground, rgb(36, 47, 202));\\n    --pass-color: var(--vscode-button-foreground, white);\\n\\n    --warn-background-color: var(--vscode-debugConsole-warningForeground, rgb(190, 159, 20));\\n    --warn-color: var(--vscode-button-foreground, white);\\n\\n    --not-run-background-color: var(--vscode-editor-foreground, rgb(102, 102, 102));\\n    --not-run-color: var(--vscode-editor-background, white);\\n\\n    --summary-hover-background-color: var(--vscode-editor-hoverHighlightBackground, rgb(222, 222, 222));\\n\\n    /* \\n    --fg-color: white;\\n    --bg-color: #4b4a4a;\\n    --font-family: \\"Segoe UI\\", Tahoma, Geneva, Verdana, sans-serif; \\n    */\\n}\\n\\n.summaryField {\\n    margin-left: 3px;\\n    margin-right: 3px;\\n}\\n\\n.summaryFileName {\\n    opacity: 0.6;\\n    margin-left: 1rem;\\n}\\n\\n.timeLabel {\\n    opacity: 0.6;\\n}\\n\\n/* .summaryInput {\\n    opacity: 0.6;\\n} */\\n\\n.summaryInput::before {\\n    margin-left: 3px;\\n    content: \\"(\\";\\n}\\n.summaryInput::after {\\n    margin-right: 3px;\\n    content: \\")\\";\\n}\\n\\n/* nesting level vertical line */\\n.detailInfo {\\n    border-left: 1px solid var(--error-background-color);\\n\\n    /* centering the line with the icon */\\n    margin-left: 1.5rem;\\n\\n    /* nesting indentation */\\n    padding-left: 0.8rem;\\n}\\n\\nbody {\\n    font-family: var(--font-family);\\n    font-size: var(--font-size);\\n    font-weight: var(--font-weight);\\n    color: var(--fg-color);\\n    background-color: var(--bg-color);\\n}\\n\\n#mainTree {\\n    margin-top: 5px;\\n}\\n\\nul {\\n    list-style-type: none;\\n    padding-inline-start: 0px;\\n    margin-block-start: 0px;\\n}\\n\\ndiv ul:not(:first-child) {\\n    border-left: 1px dotted rgb(141, 141, 141);\\n}\\n\\n.tree li {\\n    display: block;\\n    position: relative;\\n    padding-left: 0px;\\n}\\n\\n.tree ul {\\n    margin-left: 10px;\\n    padding-left: 0;\\n}\\n\\n.toolbarButton {\\n    display: inline;\\n    border-radius: 5px;\\n    background: var(--bg-color);\\n    color: var(--fg-color);\\n    margin-left: 3px;\\n    width: 15px;\\n    height: 15px;\\n    border: 0;\\n    padding: 0;\\n    vertical-align: middle;\\n}\\n\\n.toolbarContainer {\\n    display: inline-block;\\n}\\n\\n.summaryDiv {\\n    display: inline;\\n}\\n\\ndetails > summary {\\n    /* Note: couldn\'t get proper color with the svg approach */\\n    /* list-style-image: url(\\"data:image/svg+xml;utf8,<svg width=\'12px\' height=\'12px\' viewBox=\'0 0 20 20\' xmlns=\'http://www.w3.org/2000/svg\'><g data-name=\'Layer 2\'><g data-name=\'arrow-ios-forward\'><rect width=\'24\' height=\'24\' transform=\'rotate(-90 12 12)\' opacity=\'0\'/><path fill=\'currentColor\' stroke=\'currentColor\' d=\'M10 19a1 1 0 0 1-.64-.23 1 1 0 0 1-.13-1.41L13.71 12 9.39 6.63a1 1 0 0 1 .15-1.41 1 1 0 0 1 1.46.15l4.83 6a1 1 0 0 1 0 1.27l-5 6A1 1 0 0 1 10 19z\'/></g></g></svg>\\"); */\\n    /* list-style-type: \\"⮞ \\"; */\\n    /* list-style-type: \\"⏵\\"; */\\n    list-style-type: \\"+ \\";\\n}\\n\\ndetails[open] > summary {\\n    /* list-style-image: url(\\"data:image/svg+xml;utf8,<svg width=\'12px\' height=\'12px\' viewBox=\'0 0 20 20\' xmlns=\'http://www.w3.org/2000/svg\'><g data-name=\'Layer 2\'><g data-name=\'arrow-ios-downward\'><rect width=\'24\' height=\'24\' opacity=\'0\'/><path fill=\'currentColor\' stroke=\'currentColor\' d=\'M12 16a1 1 0 0 1-.64-.23l-6-5a1 1 0 1 1 1.28-1.54L12 13.71l5.36-4.32a1 1 0 0 1 1.41.15 1 1 0 0 1-.14 1.46l-6 4.83A1 1 0 0 1 12 16z\'/></g></g></svg>\\"); */\\n    /* list-style-type: \\"⮟ \\"; */\\n    /* list-style-type: \\"⏷\\"; */\\n    list-style-type: \\"- \\";\\n}\\n\\n.NO_CHILDREN > summary {\\n    list-style-type: \\"\xa0\xa0\\" !important;\\n}\\n\\nselect {\\n    background-color: var(--menu-background);\\n    color: var(--menu-foreground);\\n}\\n\\nsummary {\\n    padding: 3px;\\n}\\n\\na:link {\\n    color: var(--fg-color);\\n}\\n\\na:visited {\\n    color: var(--fg-color);\\n}\\n\\na:hover {\\n    color: var(--fg-color);\\n}\\n\\na:active {\\n    color: var(--fg-color);\\n}\\n\\n.label {\\n    padding: 2px 2px;\\n    font-size: 0.65em;\\n    letter-spacing: 1px;\\n    white-space: nowrap;\\n    border-radius: 3px;\\n    margin-right: 5px;\\n    font-weight: bold;\\n}\\n\\n.timeLabel {\\n    padding: 2px 2px;\\n    font-size: 0.85em;\\n    letter-spacing: 1px;\\n    white-space: nowrap;\\n    border-radius: 3px;\\n    margin-right: 5px;\\n    font-weight: lighter;\\n}\\n\\n.label.F,\\n.label.E,\\n.label.FAIL,\\n.label.ERROR {\\n    border-radius: 3px;\\n    background-color: var(--error-background-color);\\n    color: var(--error-color);\\n    font-weight: bolder;\\n}\\n\\n.label.PASS,\\n.label.I,\\n.label.INFO {\\n    border-radius: 3px;\\n    background-color: var(--pass-background-color);\\n    color: var(--pass-color);\\n    font-weight: bolder;\\n}\\n\\n.label.W,\\n.label.WARN {\\n    border-radius: 3px;\\n    background-color: var(--warn-background-color);\\n    color: var(--warn-color);\\n    font-weight: bolder;\\n}\\n\\n.label.HIDDEN {\\n    border-radius: 3px;\\n    background-color: var(--hidden-background-color);\\n    color: var(--hidden-color);\\n    font-weight: bolder;\\n}\\n.label.HIDDEN.inline {\\n    margin-left: 5px;\\n}\\n\\nsummary.HIDDEN {\\n    margin-top: 10px;\\n    margin-bottom: 10px;\\n}\\n\\n.label.NOT_RUN {\\n    border-radius: 3px;\\n    background-color: var(--not-run-background-color);\\n    color: var(--not-run-color);\\n    font-weight: bolder;\\n}\\n\\n#summary.FAIL,\\n#summary.ERROR {\\n    border-bottom: 5px solid var(--error-background-color);\\n}\\n\\n#summary.PASS {\\n    border-bottom: 5px solid var(--pass-background-color);\\n}\\n\\n#summary.NOT_RUN {\\n    border-bottom: 5px solid var(--not-run-background-color);\\n}\\n\\n/* .span_link::after {\\n    content: \\" ⮳\\";\\n} */\\n.span_link {\\n    cursor: pointer;\\n    /* text-decoration: underline; */\\n}\\n\\nsummary:hover {\\n    background-color: var(--summary-hover-background-color);\\n}\\n",""]);const s=r},645:e=>{e.exports=function(e){var t=[];return t.toString=function(){return this.map((function(t){var n=e(t);return t[2]?"@media ".concat(t[2]," {").concat(n,"}"):n})).join("")},t.i=function(e,n,o){"string"==typeof e&&(e=[[null,e,""]]);var r={};if(o)for(var s=0;s<this.length;s++){var a=this[s][0];null!=a&&(r[a]=!0)}for(var i=0;i<e.length;i++){var d=[].concat(e[i]);o&&r[d[0]]||(n&&(d[2]?d[2]="".concat(n," and ").concat(d[2]):d[2]=n),t.push(d))}},t}},391:(e,t,n)=>{let o;window.setVSCodeAPI=function(e){o=e};let r={};function s(e){let t;try{t=o}catch(e){}t&&t.postMessage(e)}let a={output:void 0},i={setContents:void 0,appendContents:void 0,updateLabel:void 0};window.addEventListener("message",(e=>{let t=e.data;if(t)switch(t.type){case"response":let e=t,n=r[e.request_seq];n&&(delete r[e.request_seq],n(e));break;case"event":let o=a[t.event];o?o(t):console.log("Unhandled event: ",t);break;case"request":let s=i[t.command];s?s(t):console.log("Unhandled request: ",t)}}));let d=0;function l(){return d+=1,d}let c={filterLevel:"PASS",runIdToTreeState:{},runIdLRU:[]},u={initialContents:void 0,runId:void 0,state:void 0,onClickReference:void 0,appendedContents:[],allRunIdsToLabel:{},showTime:!0,showExpand:!0};function m(){return void 0===u.state&&(u.state=function(){let e;try{e=o}catch(e){}if(e){let t=e.getState();return t||(t=c),void 0===t.filterLevel&&(t.filterLevel="PASS"),void 0===t.runIdToTreeState&&(t.runIdToTreeState={}),void 0===!t.runIdLRU&&(t.runIdLRU=[]),t}return c}()),u}function h(e){return document.getElementById(e)}function p(e){return h(e)}function f(e){return h(e)}function g(e){const t=document.createElement("ul");return t.setAttribute("data-tree-id",e),t}function v(){return document.createElement("span")}function E(){return document.createElement("button")}function y(){return document.createElement("div")}function b(e){return e.getAttribute("data-tree-id")}function S(e,t=undefined){if(void 0===t)return"1"===e.getAttribute("data-hidden");t?e.setAttribute("data-hidden","1"):e.removeAttribute("data-hidden")}function C(e){var t=document.createElement("template");return e=e.trim(),t.innerHTML=e,t.content.firstChild}function T(e,t){for(let n of t.childNodes)if(n instanceof HTMLDetailsElement){for(let t of n.childNodes)t instanceof HTMLUListElement&&L(e,t);n.open?e.openNodes[b(t)]="open":delete e.openNodes[b(t)]}}function L(e,t){for(let n of t.childNodes)n instanceof HTMLLIElement&&T(e,n)}const w=((e,t)=>{let n;return function(...e){clearTimeout(n),n=setTimeout((()=>{clearTimeout(n),(()=>{N()})(...e)}),500)}})();function N(){const e=m();!function(e,t){const n=p("mainTree");let o={openNodes:{}};if(void 0===e.runIdLRU&&(e.runIdLRU=[]),void 0===e.runIdToTreeState)e.runIdToTreeState={};else{const n=e.runIdToTreeState[t];n&&(o=n)}for(let e of n.childNodes)e instanceof HTMLUListElement&&L(o,e);e.runIdToTreeState[t]=o;const r=e.runIdLRU.indexOf(t);for(r>-1&&e.runIdLRU.splice(r,1),e.runIdLRU.push(t);e.runIdLRU.length>15;){const t=e.runIdLRU.splice(0,1);delete e.runIdToTreeState[t[0]]}}(e.state,e.runId),function(e){let t;try{t=o}catch(e){}t?t.setState(e):c=e}(e.state)}function I(e,t){if(void 0===e)return;const n=f("selectedRun"),o=new Map;for(let r of n.childNodes)if(r instanceof HTMLOptionElement){const n=r,s=n.value,a=e[s];if(void 0===a)r.remove();else{n.text!==a&&(n.text=a),o.set(s,a);const e=t==s;n.selected=e}}for(const r of Object.keys(e)){if(void 0===r)continue;const s=t==r;if(!o.has(r)){const t=document.createElement("option"),a=e[r];t.value=r,n.appendChild(t),t.selected=s,t.text=a,o.set(r,a)}}}Math.pow(10,8);var x=36e5;function M(e,t){var n;!function(e,t){if(t.length<1)throw new TypeError("1 argument required, but only "+t.length+" present")}(0,arguments);var o=function(e){if(null===e||!0===e||!1===e)return NaN;var t=Number(e);return isNaN(t)?t:t<0?Math.ceil(t):Math.floor(t)}(null!==(n=null==t?void 0:t.additionalDigits)&&void 0!==n?n:2);if(2!==o&&1!==o&&0!==o)throw new RangeError("additionalDigits must be 0, 1 or 2");if("string"!=typeof e&&"[object String]"!==Object.prototype.toString.call(e))return new Date(NaN);var r,s=function(e){var t,n={},o=e.split(k.dateTimeDelimiter);if(o.length>2)return n;if(/:/.test(o[0])?t=o[0]:(n.date=o[0],t=o[1],k.timeZoneDelimiter.test(n.date)&&(n.date=e.split(k.timeZoneDelimiter)[0],t=e.substr(n.date.length,e.length))),t){var r=k.timezone.exec(t);r?(n.time=t.replace(r[1],""),n.timezone=r[1]):n.time=t}return n}(e);if(s.date){var a=function(e,t){var n=new RegExp("^(?:(\\\\d{4}|[+-]\\\\d{"+(4+t)+"})|(\\\\d{2}|[+-]\\\\d{"+(2+t)+"})$)"),o=e.match(n);if(!o)return{year:NaN,restDateString:""};var r=o[1]?parseInt(o[1]):null,s=o[2]?parseInt(o[2]):null;return{year:null===s?r:100*s,restDateString:e.slice((o[1]||o[2]).length)}}(s.date,o);r=function(e,t){if(null===t)return new Date(NaN);var n=e.match(R);if(!n)return new Date(NaN);var o=!!n[4],r=D(n[1]),s=D(n[2])-1,a=D(n[3]),i=D(n[4]),d=D(n[5])-1;if(o)return function(e,t,n){return t>=1&&t<=53&&n>=0&&n<=6}(0,i,d)?function(e,t,n){var o=new Date(0);o.setUTCFullYear(e,0,4);var r=7*(t-1)+n+1-(o.getUTCDay()||7);return o.setUTCDate(o.getUTCDate()+r),o}(t,i,d):new Date(NaN);var l=new Date(0);return function(e,t,n){return t>=0&&t<=11&&n>=1&&n<=(O[t]||(H(e)?29:28))}(t,s,a)&&function(e,t){return t>=1&&t<=(H(e)?366:365)}(t,r)?(l.setUTCFullYear(t,s,Math.max(r,a)),l):new Date(NaN)}(a.restDateString,a.year)}if(!r||isNaN(r.getTime()))return new Date(NaN);var i,d=r.getTime(),l=0;if(s.time&&(l=function(e){var t=e.match(_);if(!t)return NaN;var n=F(t[1]),o=F(t[2]),r=F(t[3]);return function(e,t,n){return 24===e?0===t&&0===n:n>=0&&n<60&&t>=0&&t<60&&e>=0&&e<25}(n,o,r)?n*x+6e4*o+1e3*r:NaN}(s.time),isNaN(l)))return new Date(NaN);if(!s.timezone){var c=new Date(d+l),u=new Date(0);return u.setFullYear(c.getUTCFullYear(),c.getUTCMonth(),c.getUTCDate()),u.setHours(c.getUTCHours(),c.getUTCMinutes(),c.getUTCSeconds(),c.getUTCMilliseconds()),u}return i=function(e){if("Z"===e)return 0;var t=e.match(A);if(!t)return 0;var n="+"===t[1]?-1:1,o=parseInt(t[2]),r=t[3]&&parseInt(t[3])||0;return function(e,t){return t>=0&&t<=59}(0,r)?n*(o*x+6e4*r):NaN}(s.timezone),isNaN(i)?new Date(NaN):new Date(d+l+i)}var k={dateTimeDelimiter:/[T ]/,timeZoneDelimiter:/[Z ]/i,timezone:/([Z+-].*)$/},R=/^-?(?:(\\d{3})|(\\d{2})(?:-?(\\d{2}))?|W(\\d{2})(?:-?(\\d{1}))?|)$/,_=/^(\\d{2}(?:[.,]\\d*)?)(?::?(\\d{2}(?:[.,]\\d*)?))?(?::?(\\d{2}(?:[.,]\\d*)?))?$/,A=/^([+-])(\\d{2})(?::?(\\d{2}))?$/;function D(e){return e?parseInt(e):1}function F(e){return e&&parseFloat(e.replace(",","."))||0}var O=[31,null,31,30,31,30,31,31,30,31,30,31];function H(e){return e%400==0||e%4==0&&e%100!=0}function U(e,t){const n=e.memo[t];return void 0===n?`<ref not found: ${t}>`:n}function B(e,t){return parseFloat(t)}function j(e,t){return parseInt(t)}function P(e,t){return t}function $(e){const t=[],n=new Map;for(let o of e.split(",")){o=o.trim();let e="oid";if(-1!=o.indexOf(":")&&([o,e]=o.split(":",2)),t.push(o),"oid"===e)n.set(o,U);else if("int"===e)n.set(o,j);else if("float"===e)n.set(o,B);else{if("str"!==e)throw new Error("Unexpected: "+e);n.set(o,P)}}return function(e,o){const r=o.split("|",t.length),s={};for(let o=0;o<r.length;o++){const a=r[o],i=t[o];s[i]=n.get(i)(e,a)}return s}}const z=$("name:oid, time_delta_in_seconds:float"),V=$("status:oid, time_delta_in_seconds:float"),q=$("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),W=$("status:oid, message:oid, time_delta_in_seconds:float"),J=$("name:oid, libname:oid, type:oid, doc:oid, source:oid, lineno:int, time_delta_in_seconds:float"),Y=$("status:oid, time_delta_in_seconds:float"),Z=$("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),G={V:function(e,t){return{message:t}},ID:$("part:int, id:str"),I:function(e,t){return JSON.parse(t)},T:function(e,t){return{time:M(t).toString()}},M:function(e,t){var n,o;const r=Q(t,":");if(r){[n,o]=r;try{o=JSON.parse(o)}catch(e){return console.log("Error parsing json: "+o),console.log(e),null}e.memo[n]=o}return null},SR:z,RR:z,ER:V,ST:q,RT:q,ET:W,SE:J,RE:J,EE:Y,EA:$("name:oid, type:oid, value:oid"),AS:$("source:oid, lineno:int, target:oid, type:oid, value:oid, time_delta_in_seconds:float"),L:Z,LH:Z,TG:$("tag:oid"),S:$("start_time_delta:float"),STB:$("message:oid, time_delta_in_seconds:float"),RTB:$("message:oid, time_delta_in_seconds:float"),TBE:$("source:oid, lineno:int, method:oid, line_content:oid"),TBV:$("name:oid, type:oid, value:oid"),ETB:$("time_delta_in_seconds:float")};class K{constructor(){this.memo={}}decode_message_type(e,t){return(0,G[e])(this,t)}}function Q(e,t){const n=e.indexOf(t);if(n>0)return[e.substring(0,n),e.substring(n+1)]}function*X(e,t){var n,o,r;for(let s of e.split(/\\r?\\n/))if(s=s.trim(),s)try{const e=Q(s," ");if(e&&([r,o]=e,n=t.decode_message_type(r,o))){const e={message_type:r,decoded:n};yield e}}catch(e){console.log("Unable to decode message: "+s),console.log(e)}}function ee(e,t){const n=document.createElement("span");n.textContent=t,n.classList.add("label"),n.classList.add(t.replace(" ","_")),e.summaryDiv.insertBefore(n,e.summaryDiv.firstChild)}function te(e,t){switch(e.state.filterLevel){case"FAIL":return t>=2;case"WARN":return t>=1;case"PASS":return t>=0;case"NOT RUN":return!0}}function ne(e){switch(e){case"FAIL":case"ERROR":return 2;case"WARN":return 1;case"NOT RUN":case"NOT_RUN":return-1;default:return 0}}class oe{constructor(e){this.stack=[],this.exceptionMsg=e}pushEntry(e,t,n,o){const r=new Map;this.stack.push({source:e,lineno:t,method:n,lineContent:o,variables:r})}pushVar(e,t,n){this.stack.at(-1).variables.set(e,[t,n])}}class re{constructor(){this.totalTests=0,this.totalFailures=0}clear(){this.totalTests=0,this.totalFailures=0,this.updateSummary()}onTestEndUpdateSummary(e){const t=e.decoded.status;this.totalTests+=1,"FAIL"!=t&&"ERROR"!=t||(this.totalFailures+=1),this.updateSummary()}updateSummary(){const e=p("summary");if(!e)return;const t=(""+this.totalTests).padStart(4),n=(""+this.totalFailures).padStart(4);if(e.textContent=`Total: ${t} Failures: ${n}`,0==this.totalFailures&&0==this.totalTests){const e=p("summary");e.classList.add("NOT_RUN"),e.classList.remove("PASS"),e.classList.remove("FAIL")}else if(1==this.totalFailures){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("PASS"),e.classList.add("FAIL")}else if(0==this.totalFailures&&1==this.totalTests){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("FAIL")}}}function se(e,t){const n=function(e){const t=document.createElement("li");return t.setAttribute("data-tree-id",e),t}(t),o=document.createElement("details");e&&(o.open=e),o.classList.add("NO_CHILDREN"),n.appendChild(o);const r=y();r.classList.add("detailContainer"),o.appendChild(r);const s=document.createElement("summary"),a=y();a.classList.add("summaryDiv"),s.appendChild(a);const i=v();i.className="summaryName",i.textContent="[summaryName]",a.appendChild(i);const d=v();return d.className="summaryInput emptySummaryInput",d.textContent="",a.appendChild(d),o.appendChild(s),{li:n,details:o,summary:s,summaryDiv:a,summaryName:i,summaryInput:d,detailContainer:r}}function ae(e,t,n,o,r,s,a,i,d,l){const c=e.state.runIdToTreeState[e.runId],u="li_"+l;if(c){const e=c.openNodes;e&&(s=e[u])}const m=se(s,u),h=m.li,p=m.details,f=m.detailContainer,v=m.summary,E=m.summaryDiv,y=m.summaryName,b=m.summaryInput;if("LH"===r.message_type){y.textContent="";const e=C(n);y.appendChild(e)}else y.textContent=n;o&&(y.title=o),e.onClickReference&&(y.classList.add("span_link"),y.onclick=t=>{const n=[];let o=d.parent;for(;void 0!==o&&void 0!==o.message;)n.push(o.message),o=o.parent;t.preventDefault(),e.onClickReference({source:a,lineno:i,message:r.decoded,messageType:r.message_type,scope:n})});const S=g("ul_"+l);p.appendChild(S);const T={ul:S,li:h,details:p,detailContainer:f,summary:v,summaryName:y,summaryInput:b,source:a,lineno:i,appendContentChild:void 0,decodedMessage:r,maxLevelFoundInHierarchy:-1,summaryDiv:E};return T.appendContentChild=ue.bind(T),t.appendContentChild(T),T}let ie,de;function*le(e){for(let t of e.childNodes)if(t instanceof HTMLDetailsElement){for(let e of t.childNodes)if(e instanceof HTMLUListElement)for(let t of ce(e))yield t;yield t}}function*ce(e){for(let t of e.childNodes)if(t instanceof HTMLLIElement)for(let e of le(t))yield e}function ue(e){const t=this;t.ul.appendChild(e.li),t.details.classList.contains("NO_CHILDREN")&&(t.details.classList.remove("NO_CHILDREN"),t.details.addEventListener("toggle",(function(){w()})),m().showExpand&&t.summary.addEventListener("mouseover",(e=>{!function(e){if(void 0===ie){ie=y(),ie.classList.add("toolbarContainer");const e=E();e.appendChild(C(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path d="M7 12V7H6v5h1z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),e.onclick=()=>{!function(){if(void 0!==de){de.details.open=!0;for(let e of ce(de.ul))e.classList.contains("NO_CHILDREN")||(e.open=!0)}}()},e.classList.add("toolbarButton");const t=E();return t.appendChild(C(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),t.classList.add("toolbarButton"),t.onclick=()=>{!function(){if(void 0!==de){de.details.open=!1;for(let e of ce(de.ul))e.open=!1}}()},ie.appendChild(t),void ie.appendChild(e)}de=e,e.summaryDiv.appendChild(ie)}(t)})))}var me=(e,t,n)=>new Promise(((o,r)=>{var s=e=>{try{i(n.next(e))}catch(e){r(e)}},a=e=>{try{i(n.throw(e))}catch(e){r(e)}},i=e=>e.done?o(e.value):Promise.resolve(e.value).then(s,a);i((n=n.apply(e,t)).next())}));let he=0,pe=-1;class fe{constructor(){this.stack=[]}handle(e){let t;switch(e.message_type){case"STB":return void this.stack.push(new oe(e.decoded.message));case"TBE":return t=this.stack.at(-1),void t.pushEntry(e.decoded.source,e.decoded.lineno,e.decoded.method,e.decoded.line_content);case"TBV":return;case"ETB":return t=this.stack.pop(),t.stack.reverse(),t}}}class ge{constructor(){this.stack=[],this.messageNode={parent:void 0,message:void 0},this.id=0,this.finishedAddingInitialContents=!1,this.appendedMessagesIndex=-1,this.decoder=new K,this.seenSuiteTaskOrElement=!1,this.tbHandler=new fe,this.suiteErrored=!1,this.opts=m(),this.runId=this.opts.runId,this.summaryBuilder=new re,this.lease=(he+=1,pe=he,he),this.resetState()}resetState(){this.seenSuiteTaskOrElement=!1}isCurrentTreeBuilder(){return this.lease===pe&&this.runId==this.opts.runId}clearAndInitializeTree(){this.summaryBuilder.clear(),this.resetState();const e=f("filterLevel");e&&(e.value=this.opts.state.filterLevel);const t=p("mainTree");t.replaceChildren();const n=g("ul_root");n.classList.add("tree"),t.appendChild(n),this.parent={ul:void 0,li:void 0,details:void 0,detailContainer:void 0,summary:void 0,summaryName:void 0,summaryInput:void 0,source:void 0,lineno:void 0,decodedMessage:void 0,appendContentChild:function(e){n.appendChild(e.li)},maxLevelFoundInHierarchy:-1,summaryDiv:void 0},this.stack.push(this.parent)}addInitialContents(){return me(this,null,(function*(){for(const e of X(this.opts.initialContents,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}this.finishedAddingInitialContents=!0,yield this.onAppendedContents()}))}onAppendedContents(){return me(this,null,(function*(){if(!this.finishedAddingInitialContents)return;if(!this.isCurrentTreeBuilder())return;const e=m();for(;this.appendedMessagesIndex+1<e.appendedContents.length;){this.appendedMessagesIndex+=1;const t=e.appendedContents[this.appendedMessagesIndex];for(const e of X(t,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}}}))}addOneMessage(e){return me(this,null,(function*(){if(this.isCurrentTreeBuilder())try{this.addOneMessageSync(e)}catch(t){console.log("Error: handling message: "+JSON.stringify(e)+": "+t+" - "+JSON.stringify(t))}}))}addOneMessageSync(e){var t,n;let o,r,s=e.message_type;switch(s){case"SR":case"ST":case"SE":case"STB":this.seenSuiteTaskOrElement=!0;break;case"RR":if(this.seenSuiteTaskOrElement)return;s="SR";break;case"RT":if(this.seenSuiteTaskOrElement)return;s="ST";break;case"RE":if(this.seenSuiteTaskOrElement)return;s="SE";break;case"RTB":if(this.seenSuiteTaskOrElement)return;s="STB"}switch(this.id+=1,s){case"SR":this.messageNode={parent:this.messageNode,message:e};for(const t of document.querySelectorAll(".suiteHeader"))t.textContent=e.decoded.name;break;case"AS":r=ae(this.opts,this.parent,`${e.decoded.target} = `,`Assign to name: ${e.decoded.target}\\nAn object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),function(e,t){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${t}`,e.summaryInput.classList.remove("emptySummaryInput")):e.summaryInput.textContent+=`, ${t}`}(r,e.decoded.value),this.addAssignCssClass(r);break;case"ST":this.messageNode={parent:this.messageNode,message:e},this.parent=ae(this.opts,this.parent,`${e.decoded.libname}.${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"SE":this.messageNode={parent:this.messageNode,message:e},this.parent=ae(this.opts,this.parent,e.decoded.name,e.decoded.libname,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"ER":this.messageNode=this.messageNode.parent;{const t=p("suiteResult");t.style.display="block",this.suiteErrored?(t.classList.add("ERROR"),t.textContent="Run Failed"):(t.classList.add("PASS"),t.textContent="Run Passed");const n=p("suiteRunStart");n&&(n.textContent+=` - Finished in: ${e.decoded.time_delta_in_seconds.toFixed(2)}s.`)}break;case"ET":this.messageNode=this.messageNode.parent;const s=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(s,this.parent,e),this.onEndSetStatusOrRemove(this.opts,s,e.decoded,this.parent,!1),this.summaryBuilder.onTestEndUpdateSummary(e),o=this.addDetailsCSSClasses(e.decoded.status,s),o&&(this.suiteErrored=!0,s.details.open=!0);break;case"EE":this.messageNode=this.messageNode.parent;let a=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(a,this.parent,e),this.onEndSetStatusOrRemove(this.opts,a,e.decoded,this.parent,!0),o=this.addDetailsCSSClasses(e.decoded.status,a),o&&(a.details.open=!0);break;case"S":const i=e.decoded.start_time_delta;(null==(n=null==(t=this.parent)?void 0:t.decodedMessage)?void 0:n.decoded)&&(this.parent.decodedMessage.decoded.time_delta_in_seconds=i);break;case"EA":r=this.stack.at(-1),function(e,t,n,o){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${t} (${n}) = ${o}`,e.summaryInput.classList.remove("emptySummaryInput")):e.summaryInput.textContent+=`, ${t} (${n}) = ${o}`}(r,e.decoded.name,e.decoded.type,e.decoded.value);break;case"L":case"LH":const d=e.decoded.level,l=function(e){switch(e){case"E":case"F":return 2;case"W":return 1;default:return 0}}(d);if(l>this.parent.maxLevelFoundInHierarchy&&(this.parent.maxLevelFoundInHierarchy=l),te(this.opts,l)){const t=ae(this.opts,this.parent,e.decoded.message,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());t.maxLevelFoundInHierarchy=l,function(e,t){const n=document.createElement("span");n.textContent=`LOG ${function(e){switch(e){case"E":return"ERROR";case"F":return"FAIL";case"W":return"WARN";case"I":return"INFO";default:return e}}(t)}`,n.classList.add("label"),n.classList.add(t.replace(" ","_")),e.summaryDiv.insertBefore(n,e.summaryDiv.firstChild)}(t,d),this.addDetailsCSSClasses(l,t)}break;case"STB":case"TBE":case"TBV":case"ETB":const c=this.tbHandler.handle(e);if(c&&c.stack.length>0){const t=c.stack[0];r=ae(this.opts,this.parent,c.exceptionMsg,"",e,!1,t.source,t.lineno,this.messageNode,this.id.toString()),this.addExceptionCssClass(r)}break;case"T":const u=p("suiteRunStart");u&&(u.textContent=e.decoded.time)}}addAssignCssClass(e){e.details.classList.add("variableParent"),e.details.classList.add("leafNode")}addExceptionCssClass(e){e.details.classList.add("exceptionParent"),e.details.classList.add("leafNode")}addDetailsCSSClasses(e,t){let n,o=!1;return n="string"==typeof e?ne(e):e,n>=2?(t.details.classList.add("errorParent"),o=!0):1==n?t.details.classList.add("warnParent"):t.details.classList.add("passParent"),t.details.classList.contains("parentNode")||t.details.classList.contains("leafNode")||(0===t.ul.children.length?t.details.classList.add("leafNode"):t.details.classList.add("parentNode")),o}onEndUpdateMaxLevelFoundInHierarchyFromStatus(e,t,n){const o=ne(n.decoded.status);o>e.maxLevelFoundInHierarchy&&(e.maxLevelFoundInHierarchy=o),e.maxLevelFoundInHierarchy>t.maxLevelFoundInHierarchy&&(t.maxLevelFoundInHierarchy=e.maxLevelFoundInHierarchy)}onEndSetStatusOrRemove(e,t,n,o,r){const s=n.status;if(te(e,t.maxLevelFoundInHierarchy)){if(r&&t.maxLevelFoundInHierarchy<=0){const e=50;if(o.ul.childElementCount>e){const e=t.summaryName.textContent;if(e&&e.toLowerCase().includes("iteration")){const e=t.li.previousSibling,n=b(t.li);if(t.li.remove(),S(e))e.getElementsByClassName("FINAL_SPAN")[0].textContent=t.summaryName.textContent;else{const e=se(!1,n);e.summaryName.textContent=t.summaryName.textContent,e.summary.classList.add("HIDDEN");const r=v();r.setAttribute("role","button"),r.textContent="...",r.classList.add("label"),r.classList.add("HIDDEN"),r.classList.add("inline"),e.summaryDiv.appendChild(r);const s=v();s.setAttribute("role","button"),s.classList.add("FINAL_SPAN"),e.summaryDiv.appendChild(s),ee(e,"HIDDEN"),S(e.li,!0),o.ul.appendChild(e.li)}return}}}if(t.summary,ee(t,s),null!=t.source&&t.source.length>0){const e=function(e){let t=e,n=Math.max(e.lastIndexOf("/"),e.lastIndexOf("\\\\"));return n>0&&(t=e.substring(n+1)),t}(t.source),n=document.createElement("span");n.textContent=e,n.classList.add("summaryFileName"),n.title=t.source,t.summaryDiv.appendChild(n)}if(this.opts.showTime){const e=t.decodedMessage.decoded.time_delta_in_seconds;void 0!==e&&e>=0&&function(e,t){const n=document.createElement("span");n.textContent=` (${t.toFixed(2)}s)`,n.classList.add("timeLabel"),e.summaryDiv.appendChild(n)}(t,n.time_delta_in_seconds-e)}}else t.li.remove()}}var ve=(e,t,n)=>new Promise(((o,r)=>{var s=e=>{try{i(n.next(e))}catch(e){r(e)}},a=e=>{try{i(n.throw(e))}catch(e){r(e)}},i=e=>e.done?o(e.value):Promise.resolve(e.value).then(s,a);i((n=n.apply(e,t)).next())}));let Ee;function ye(){return ve(this,null,(function*(){Ee=new ge,Ee.clearAndInitializeTree(),yield Ee.addInitialContents()}))}function be(e){let t={type:"event",seq:l(),event:"onClickReference"};t.data=e,s(t)}function Se(e){N();const t=m();t.runId=e.runId,t.initialContents=e.initialContents,void 0!==o&&(t.onClickReference=be),t.appendedContents=[],t.allRunIdsToLabel=e.allRunIdsToLabel,I(t.allRunIdsToLabel,t.runId),ye()}n(320),i.setContents=Se,i.appendContents=function(e){const t=m();t.runId===e.runId&&(t.appendedContents.push(e.appendContents),void 0!==Ee&&Ee.onAppendedContents())},i.updateLabel=function(e){const t=m();t.allRunIdsToLabel[e.runId]=e.label,I(t.allRunIdsToLabel,t.runId)},window.onChangedRun=function(){const e=f("selectedRun").value;let t={type:"event",seq:l(),event:"onSetCurrentRunId"};t.data={runId:e},s(t)},window.onChangedFilterLevel=function(){!function(e){const t=m();t.state.filterLevel!==e&&(t.state.filterLevel=e,N(),ye())}(f("filterLevel").value)},window.setContents=Se,window.setShowTime=function(e){m().showTime=e},window.setShowExpand=function(e){m().showExpand=e},window.getSampleContents=function(){return JSON.parse(\'"V 1\\\\nI \\\\"sys.platform=win32\\\\"\\\\nI \\\\"python=3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)]\\\\"\\\\nI \\\\"robot=5.1a3.dev1\\\\"\\\\nT 2022-10-19T09:48:34.018\\\\nM a:\\\\"Robot1\\\\"\\\\nM b:\\\\"s1\\\\"\\\\nM c:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\robot1.robot\\\\"\\\\nSR a|b|c|0.035\\\\nM d:\\\\"Simple Task\\\\"\\\\nM e:\\\\"s1-t1\\\\"\\\\nST d|e|16|0.036\\\\nM f:\\\\"First keyword\\\\"\\\\nM g:\\\\"\\\\"\\\\nM h:\\\\"KEYWORD\\\\"\\\\nSE f|g|h|g|c|17|0.036\\\\nM i:\\\\"No Operation\\\\"\\\\nM j:\\\\"BuiltIn\\\\"\\\\nM k:\\\\"Does absolutely nothing.\\\\"\\\\nSE i|j|h|k|c|8|0.037\\\\nM l:\\\\"PASS\\\\"\\\\nEE l|0.037\\\\nM m:\\\\"Log\\\\"\\\\nM n:\\\\"Logs the given message with the given level.\\\\"\\\\nSE m|j|h|n|c|10|0.037\\\\nM o:\\\\"Some warning message\\\\"\\\\nEA o\\\\nM p:\\\\"level=WARN\\\\"\\\\nEA p\\\\nEE l|0.046\\\\nM q:\\\\"Another keyword\\\\"\\\\nM r:\\\\"another\\\\"\\\\nSE q|r|h|g|c|11|0.047\\\\nM s:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\another.robot\\\\"\\\\nSE i|j|h|k|s|3|0.047\\\\nEE l|0.047\\\\nEE l|0.047\\\\nM t:\\\\"Another in sub keyword\\\\"\\\\nM u:\\\\"another_sub\\\\"\\\\nSE t|u|h|g|c|12|0.047\\\\nM v:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\sub\\\\\\\\\\\\\\\\another_sub.robot\\\\"\\\\nSE i|j|h|k|v|6|0.048\\\\nEE l|0.048\\\\nSE m|j|h|n|v|7|0.048\\\\nM w:\\\\"Some error message\\\\"\\\\nEA w\\\\nM x:\\\\"level=ERROR\\\\"\\\\nEA x\\\\nEE l|0.049\\\\nEE l|0.049\\\\nEE l|0.049\\\\nSE m|j|h|n|c|18|0.049\\\\nM y:\\\\"Some <data &encode <\\/script>\\\\"\\\\nEA y\\\\nEE l|0.049\\\\nM z:\\\\"Create Dictionary\\\\"\\\\nM A:\\\\"Creates and returns a dictionary based on the given ``items``.\\\\"\\\\nSE z|j|h|A|c|19|0.049\\\\nM B:\\\\"a=1\\\\"\\\\nEA B\\\\nM C:\\\\"b=1\\\\"\\\\nEA C\\\\nEE l|0.05\\\\nSE m|j|h|n|c|20|0.05\\\\nM D:\\\\"${dct}\\\\"\\\\nEA D\\\\nEE l|0.051\\\\nET l|g|0.051\\\\nM E:\\\\"Check 1\\\\"\\\\nM F:\\\\"s1-t2\\\\"\\\\nST E|F|22|0.051\\\\nSE f|g|h|g|c|23|0.051\\\\nSE i|j|h|k|c|8|0.052\\\\nEE l|0.052\\\\nSE m|j|h|n|c|10|0.052\\\\nEA o\\\\nEA p\\\\nEE l|0.052\\\\nSE q|r|h|g|c|11|0.053\\\\nSE i|j|h|k|s|3|0.053\\\\nEE l|0.053\\\\nEE l|0.053\\\\nSE t|u|h|g|c|12|0.053\\\\nSE i|j|h|k|v|6|0.054\\\\nEE l|0.054\\\\nSE m|j|h|n|v|7|0.054\\\\nEA w\\\\nEA x\\\\nEE l|0.054\\\\nEE l|0.055\\\\nEE l|0.055\\\\nM G:\\\\"${counter} IN RANGE [ 0 | 3 ]\\\\"\\\\nM H:\\\\"FOR\\\\"\\\\nSE G|g|H|g|c|25|0.055\\\\nM I:\\\\"${counter} = 0\\\\"\\\\nM J:\\\\"ITERATION\\\\"\\\\nSE I|g|J|g|c|25|0.055\\\\nM K:\\\\"${counter} == 2\\\\"\\\\nM L:\\\\"IF\\\\"\\\\nSE K|g|L|g|c|26|0.055\\\\nM M:\\\\"Fail\\\\"\\\\nM N:\\\\"Fails the test with the given message and optionally alters its tags.\\\\"\\\\nSE M|j|h|N|c|27|0.056\\\\nM O:\\\\"Failed execution for some reason...\\\\"\\\\nEA O\\\\nM P:\\\\"NOT RUN\\\\"\\\\nEE P|0.056\\\\nEE P|0.056\\\\nSE m|j|h|n|c|29|0.056\\\\nM Q:\\\\"${counter}\\\\"\\\\nEA Q\\\\nEE l|0.056\\\\nEE l|0.057\\\\nM R:\\\\"${counter} = 1\\\\"\\\\nSE R|g|J|g|c|25|0.057\\\\nSE K|g|L|g|c|26|0.057\\\\nSE M|j|h|N|c|27|0.057\\\\nEA O\\\\nEE P|0.057\\\\nEE P|0.057\\\\nSE m|j|h|n|c|29|0.058\\\\nEA Q\\\\nEE l|0.058\\\\nEE l|0.058\\\\nM S:\\\\"${counter} = 2\\\\"\\\\nSE S|g|J|g|c|25|0.058\\\\nSE K|g|L|g|c|26|0.058\\\\nSE M|j|h|N|c|27|0.059\\\\nEA O\\\\nM T:\\\\"FAIL\\\\"\\\\nEE T|0.059\\\\nEE T|0.059\\\\nSE m|j|h|n|c|29|0.059\\\\nEA Q\\\\nEE P|0.059\\\\nEE T|0.06\\\\nEE T|0.06\\\\nET T|O|0.06\\\\nM U:\\\\"Check 2\\\\"\\\\nM V:\\\\"s1-t3\\\\"\\\\nST U|V|32|0.06\\\\nM W:\\\\"Set Variable\\\\"\\\\nM X:\\\\"Returns the given values which can then be assigned to a variables.\\\\"\\\\nSE W|j|h|X|c|33|0.061\\\\nM Y:\\\\"3\\\\"\\\\nEA Y\\\\nEE l|0.061\\\\nM Z:\\\\"${counter} <= 2\\\\"\\\\nM 0:\\\\"WHILE\\\\"\\\\nSE Z|g|0|g|c|34|0.061\\\\nSE g|g|J|g|c|34|0.062\\\\nM 1:\\\\"Evaluate\\\\"\\\\nM 2:\\\\"Evaluates the given expression in Python and returns the result.\\\\"\\\\nSE 1|j|h|2|c|35|0.062\\\\nM 4:\\\\"$counter-1\\\\"\\\\nEA 4\\\\nEE P|0.062\\\\nSE m|j|h|n|c|36|0.062\\\\nM 5:\\\\"Current counter: ${counter}\\\\"\\\\nEA 5\\\\nEA p\\\\nEE P|0.062\\\\nEE P|0.062\\\\nEE P|0.063\\\\nET l|g|0.063\\\\nM 6:\\\\"Check 3\\\\"\\\\nM 7:\\\\"s1-t4\\\\"\\\\nST 6|7|39|0.064\\\\nM 8:\\\\"TRY\\\\"\\\\nSE g|g|8|g|c|40|0.064\\\\nSE i|j|h|k|c|41|0.064\\\\nEE l|0.064\\\\nEE l|0.064\\\\nM 9:\\\\"message\\\\"\\\\nM aa:\\\\"EXCEPT\\\\"\\\\nSE 9|g|aa|g|c|42|0.064\\\\nSE i|j|h|k|c|43|0.065\\\\nEE P|0.065\\\\nEE P|0.065\\\\nM ab:\\\\"FINALLY\\\\"\\\\nSE g|g|ab|g|c|44|0.065\\\\nSE i|j|h|k|c|45|0.065\\\\nEE l|0.065\\\\nEE l|0.065\\\\nET l|g|0.066\\\\nER T|0.067\\\\n"\')}},320:(e,t,n)=>{var o=n(379),r=n.n(o),s=n(426),a={injectType:"singletonStyleTag",insert:"head",singleton:!0};r()(s.Z,a),s.Z.locals},379:(e,t,n)=>{var o,r=function(){var e={};return function(t){if(void 0===e[t]){var n=document.querySelector(t);if(window.HTMLIFrameElement&&n instanceof window.HTMLIFrameElement)try{n=n.contentDocument.head}catch(e){n=null}e[t]=n}return e[t]}}(),s=[];function a(e){for(var t=-1,n=0;n<s.length;n++)if(s[n].identifier===e){t=n;break}return t}function i(e,t){for(var n={},o=[],r=0;r<e.length;r++){var i=e[r],d=t.base?i[0]+t.base:i[0],l=n[d]||0,c="".concat(d," ").concat(l);n[d]=l+1;var u=a(c),m={css:i[1],media:i[2],sourceMap:i[3]};-1!==u?(s[u].references++,s[u].updater(m)):s.push({identifier:c,updater:f(m,t),references:1}),o.push(c)}return o}function d(e){var t=document.createElement("style"),o=e.attributes||{};if(void 0===o.nonce){var s=n.nc;s&&(o.nonce=s)}if(Object.keys(o).forEach((function(e){t.setAttribute(e,o[e])})),"function"==typeof e.insert)e.insert(t);else{var a=r(e.insert||"head");if(!a)throw new Error("Couldn\'t find a style target. This probably means that the value for the \'insert\' parameter is invalid.");a.appendChild(t)}return t}var l,c=(l=[],function(e,t){return l[e]=t,l.filter(Boolean).join("\\n")});function u(e,t,n,o){var r=n?"":o.media?"@media ".concat(o.media," {").concat(o.css,"}"):o.css;if(e.styleSheet)e.styleSheet.cssText=c(t,r);else{var s=document.createTextNode(r),a=e.childNodes;a[t]&&e.removeChild(a[t]),a.length?e.insertBefore(s,a[t]):e.appendChild(s)}}function m(e,t,n){var o=n.css,r=n.media,s=n.sourceMap;if(r?e.setAttribute("media",r):e.removeAttribute("media"),s&&"undefined"!=typeof btoa&&(o+="\\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(s))))," */")),e.styleSheet)e.styleSheet.cssText=o;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(o))}}var h=null,p=0;function f(e,t){var n,o,r;if(t.singleton){var s=p++;n=h||(h=d(t)),o=u.bind(null,n,s,!1),r=u.bind(null,n,s,!0)}else n=d(t),o=m.bind(null,n,t),r=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(n)};return o(e),function(t){if(t){if(t.css===e.css&&t.media===e.media&&t.sourceMap===e.sourceMap)return;o(e=t)}else r()}}e.exports=function(e,t){(t=t||{}).singleton||"boolean"==typeof t.singleton||(t.singleton=(void 0===o&&(o=Boolean(window&&document&&document.all&&!window.atob)),o));var n=i(e=e||[],t);return function(e){if(e=e||[],"[object Array]"===Object.prototype.toString.call(e)){for(var o=0;o<n.length;o++){var r=a(n[o]);s[r].references--}for(var d=i(e,t),l=0;l<n.length;l++){var c=a(n[l]);0===s[c].references&&(s[c].updater(),s.splice(c,1))}n=d}}}}},t={};function n(o){var r=t[o];if(void 0!==r)return r.exports;var s=t[o]={id:o,exports:{}};return e[o](s,s.exports,n),s.exports}n.n=e=>{var t=e&&e.__esModule?()=>e.default:()=>e;return n.d(t,{a:t}),t},n.d=(e,t)=>{for(var o in t)n.o(t,o)&&!n.o(e,o)&&Object.defineProperty(e,o,{enumerable:!0,get:t[o]})},n.o=(e,t)=>Object.prototype.hasOwnProperty.call(e,t),n.nc=void 0,n(391),n(320)})();</script></body><script>window.setShowTime(true);\n    window.setShowExpand(true);\n    try {\n        const vscode = acquireVsCodeApi();\n        window.setVSCodeAPI(vscode);\n        document.getElementById("selectRunContainer").style.display = "block";\n    } catch (err) {\n        // That\'s ok (not running in VSCode).\n        window.setContents({\n            "initialContents": window.getSampleContents(),\n        });\n    }</script></html>'}
```

### Comparing `robocorp_logging-0.0.8/src/robo_log/index_v2.py` & `robocorp_logging-0.0.9/src/robo_log/_index_v2.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Note: autogenerated file.
 # To regenerate this file use: python -m dev build-output-view.
 
 # The FILE_CONTENTS contains the contents of the files with
 # html/javascript code which can be used to visualize the contents of the
 # output generated by robocorp-logging (i.e.: the .robolog files).
 
-FILE_CONTENTS = {'index.html': '<!doctype html><html><head><meta charset="utf-8"/><title class="suiteHeader">Robocorp Log</title><meta name="viewport" content="width=device-width,initial-scale=1"/></head><body><div class="headerTitleSection"><h3 class="suiteHeader">Robocorp Log</h3><span id="suiteResult" class="label" style="display: none;"></span></div><div id="suiteRunStart" class="headerRunDetails"></div><div class="headers"><span class="headerSource">Source</span> <span class="headerInputs">Input Arguments</span></div><div id="mainTree"></div><script>(()=>{"use strict";var e={599:(e,n,t)=>{t.d(n,{Z:()=>s});var a=t(645),r=t.n(a)()((function(e){return e[1]}));r.push([e.id,\'/* ******************************* */\\n/* CONTAINERS ETC */\\n\\n/* box model reset */\\n* {\\n    box-sizing: border-box;\\n}\\n\\nhtml,\\nbody {\\n    margin: 0;\\n    padding: 0;\\n    height: 100%;\\n}\\n\\n:root {\\n    --right-column-width-narrow: 40vw;\\n    --right-column-width-wide: 50vw;\\n    /* from here: https://qwtel.com/posts/software/the-monospaced-system-ui-css-font-stack/ */\\n    --sans-font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen", "Ubuntu",\\n        "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue", Arial, sans-serif;\\n    /* from here: https://qwtel.com/posts/software/the-monospaced-system-ui-css-font-stack/ */\\n    --fixed-font-family: ui-monospace, Menlo, Monaco, "Cascadia Mono", "Segoe UI Mono", "Roboto Mono", "Oxygen Mono",\\n        "Ubuntu Monospace", "Source Code Pro", "Fira Mono", "Droid Sans Mono", "Courier New", monospace;\\n}\\n\\n/* ******************************* */\\n/* THEMING SUPPORT */\\n\\n@media (prefers-color-scheme: light) {\\n    :root {\\n        --log-color-error: #e84f5c;\\n        --log-color-success: #219f7f;\\n\\n        --log-color-warn: #93801c;\\n        --log-color-disabled: #999999;\\n        --log-color-border: #dddddd;\\n\\n        --log-color-text: #000000;\\n        --log-color-text-weaker: #444444;\\n        --log-color-text-weakest: #666666;\\n\\n        --log-color-bg: #ffffff;\\n        --log-color-bg-raised: #f3f3f3;\\n    }\\n}\\n\\n@media (prefers-color-scheme: dark) {\\n    :root {\\n        --log-color-error: #e84f5c;\\n        --log-color-success: #219f7f;\\n        --log-color-warn: #fff565;\\n\\n        --log-color-disabled: #666666;\\n        --log-color-border: #444444;\\n\\n        --log-color-text: #eeeeee;\\n        --log-color-text-weaker: #bbbbbb;\\n        --log-color-text-weakest: #666666;\\n\\n        --log-color-bg: #222222;\\n        --log-color-bg-raised: #333333;\\n    }\\n}\\n\\nbody {\\n    display: flex;\\n    flex-direction: column;\\n    padding: 1rem;\\n    font-size: 0.8rem;\\n    font-family: var(--sans-font-family);\\n    color: var(--log-color-text);\\n    background-color: var(--log-color-bg);\\n}\\n\\nul {\\n    list-style-type: none;\\n    padding-inline-start: 0px;\\n    margin-block-start: 0px;\\n}\\n\\n#mainTree {\\n    white-space: nowrap;\\n    overflow: auto;\\n    flex-grow: 1;\\n}\\n\\n/* ******************************* */\\n/* TREE */\\n\\n.tree li {\\n    display: block;\\n    position: relative;\\n    padding-left: 0px;\\n}\\n\\n/* nesting level vertical line */\\n.tree ul:not(:first-child),\\n.detailContainer {\\n    border-left: 1px solid var(--log-color-border);\\n\\n    /* centering the line with the icon */\\n    margin-left: 0.65rem;\\n\\n    /* nesting indentation */\\n    padding-left: 0.8rem;\\n}\\n\\ndetails.errorParent .tree ul:not(:first-child),\\ndetails.errorParent .detailContainer {\\n    border-color: var(--log-color-error);\\n}\\n\\n/* ******************************* */\\n/* SUMMARY ROW FOR EACH CODE ROW */\\n\\ndetails.parentNode > summary,\\ndetails.errorParent.leafNode > summary {\\n    cursor: pointer;\\n}\\n\\ndetails > summary {\\n    padding-top: 0.25rem;\\n    padding-bottom: 0.25rem;\\n    padding-left: 0.25rem;\\n\\n    /* chrome needs this, safari doesn\\\'t */\\n    list-style: none;\\n}\\n\\ndetails > summary:hover {\\n    background-color: var(--log-color-bg-raised);\\n    border-radius: 2px;\\n}\\n\\ndetails > summary::-webkit-details-marker {\\n    display: none;\\n}\\n\\ndetails > summary::marker {\\n    display: none;\\n}\\n\\ndetails > summary::before {\\n    background-color: var(--log-color-success);\\n}\\n\\ndetails.errorParent > summary::before {\\n    background-color: var(--log-color-error);\\n}\\n\\ndetails.warnParent > summary::before {\\n    background-color: var(--log-color-warn);\\n}\\n\\n/* icon from: https://github.com/twbs/icons/blob/main/icons/caret-right-square-fill.svg */\\ndetails > summary::before {\\n    position: absolute;\\n    left: 0.25rem;\\n    top: 4px;\\n\\n    /* chrome seems to need the \\\'-webkit\\\' prefix here */\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="black" class="bi bi-caret-right-square-fill" viewBox="0 0 16 16"><path d="M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm5.5 10a.5.5 0 0 0 .832.374l4.5-4a.5.5 0 0 0 0-.748l-4.5-4A.5.5 0 0 0 5.5 4v8z"/></svg>\\\');\\n    width: 1rem;\\n    height: 1rem;\\n    display: inline-block;\\n    content: "";\\n}\\n\\n/* filled icon */\\n/*details.leafNode.passParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square-fill" viewBox="0 0 16 16"><path d="M2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2zm10.03 4.97a.75.75 0 0 1 .011 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.75.75 0 0 1 1.08-.022z"/></svg>\\\');\\n}*/\\n\\ndetails.leafNode.passParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M14 1a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1h12zM2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2z"/><path d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.235.235 0 0 1 .02-.022z"/></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (error) */\\ndetails.leafNode.errorParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M8.6 1c1.6.1 3.1.9 4.2 2 1.3 1.4 2 3.1 2 5.1 0 1.6-.6 3.1-1.6 4.4-1 1.2-2.4 2.1-4 2.4-1.6.3-3.2.1-4.6-.7-1.4-.8-2.5-2-3.1-3.5C.9 9.2.8 7.5 1.3 6c.5-1.6 1.4-2.9 2.8-3.8C5.4 1.3 7 .9 8.6 1zm.5 12.9c1.3-.3 2.5-1 3.4-2.1.8-1.1 1.3-2.4 1.2-3.8 0-1.6-.6-3.2-1.7-4.3-1-1-2.2-1.6-3.6-1.7-1.3-.1-2.7.2-3.8 1-1.1.8-1.9 1.9-2.3 3.3-.4 1.3-.4 2.7.2 4 .6 1.3 1.5 2.3 2.7 3 1.2.7 2.6.9 3.9.6zM7.9 7.5L10.3 5l.7.7-2.4 2.5 2.4 2.5-.7.7-2.4-2.5-2.4 2.5-.7-.7 2.4-2.5-2.4-2.5.7-.7 2.4 2.5z"/></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (warn) */\\ndetails.leafNode.warnParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M7.56 1h.88l6.54 12.26-.44.74H1.44L1 13.26 7.56 1zM8 2.28L2.28 13H13.7L8 2.28zM8.625 12v-1h-1.25v1h1.25zm-1.25-2V6h1.25v4h-1.25z"/></svg>\\\');\\n}\\n\\ndetails.parentNode > summary::before,\\ndetails.parentNode.errorParent > summary::before {\\n    transform-origin: 8px 8px;\\n    transform: rotate(0deg);\\n    transition: transform 0.2s ease-out !important;\\n}\\n\\ndetails[open].parentNode > summary::before,\\ndetails[open].parentNode.errorParent > summary::before {\\n    transform: rotate(90deg);\\n}\\n\\ndetails[open] > summary > .summaryDiv > .summaryInput {\\n    /* Display full input parameters when expanded by adjusting the\\n       white-space to wrap the contents. Even nodes that don\\\'t have\\n       children can be expanded in this way, but it is not obvious\\n       since there is no triangle icon next to them. */\\n    white-space: initial;\\n}\\n\\n.summaryDiv {\\n    /* aligns code line correctly with the icon */\\n    display: flex;\\n    margin-left: 1.2rem;\\n}\\n\\n.summaryDiv > .label {\\n    order: 2;\\n}\\n\\n.summaryDiv > .summaryName {\\n    order: 1;\\n\\n    margin-left: 0.5rem;\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n}\\n\\n.summaryDiv > .summaryName,\\n.detailContainer > .detailInfo {\\n    /* this forces the correct column size, see:\\n       https://makandracards.com/makandra/66994-css-flex-and-min-width */\\n    min-width: 0;\\n}\\n\\ndetails.errorParent > summary > .summaryDiv > .summaryName {\\n    font-weight: bold;\\n}\\n\\n.summaryDiv > .summaryInput {\\n    order: 4;\\n    margin-left: auto;\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n.summaryDiv > .summaryInput.emptySummaryInput {\\n    color: var(--log-color-text-weakest);\\n}\\n\\n.detailContainer {\\n    display: flex;\\n}\\n\\n.detailContainer > .detailInfo {\\n    margin-right: auto;\\n}\\n\\n.summaryDiv > .summaryInput,\\n.detailContainer > .detailInputs {\\n    flex: 0 0 var(--right-column-width-wide);\\n    padding-left: 0.5rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n}\\n\\n.summaryDiv .timeLabel,\\n.summaryDiv .summaryFileName {\\n    order: 3;\\n    color: var(--log-color-text-weakest);\\n    margin-left: 0.5rem;\\n}\\n\\ndetails > summary:hover .timeLabel,\\ndetails > summary:hover .summaryFileName {\\n    color: var(--log-color-text-weaker);\\n}\\n\\ndetails > summary:hover .summaryInput:not(.emptySummaryInput) {\\n    color: var(--log-color-text) !important;\\n}\\n\\n/* ******************************* */\\n/* RESPONSIVE SIZING */\\n\\n@media only screen and (max-width: 840px) {\\n    .summaryDiv > .summaryInput,\\n    .detailContainer > .detailInputs,\\n    .headerInputs {\\n        display: none;\\n    }\\n}\\n\\n@media only screen and (max-width: 960px) {\\n    .headerInputs {\\n        width: var(--right-column-width-narrow) !important;\\n    }\\n\\n    .summaryDiv > .summaryInput,\\n    .detailContainer > .detailInputs {\\n        flex: 0 0 var(--right-column-width-narrow) !important;\\n    }\\n}\\n\\n/* ******************************* */\\n/* ERROR OUTPUT */\\n\\n.detailInfo {\\n    margin: 0.25rem 0;\\n    padding: 0.25rem 0;\\n    border-radius: 3px;\\n    font-size: 0.8rem;\\n}\\n\\n.errorHeader {\\n    font-weight: bold;\\n    margin-bottom: 0.35rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n\\n    /* forces wrapping */\\n    white-space: initial;\\n}\\n\\n.errorDetails {\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n\\n    /* forces wrapping */\\n    white-space: initial;\\n\\n    color: var(--log-color-text-weaker);\\n}\\n\\n/* ******************************* */\\n/* HEADERS */\\n\\n.headers {\\n    display: flex;\\n    border-bottom: 1px solid var(--log-color-border);\\n    padding-bottom: 1rem;\\n    margin-bottom: 1rem;\\n}\\n\\n.headerSource,\\n.headerInputs {\\n    font-weight: 600;\\n    text-transform: uppercase;\\n    font-size: 0.75rem;\\n    letter-spacing: 0.3px;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n.headerInputs {\\n    margin-left: auto;\\n    width: var(--right-column-width-wide);\\n    padding-left: 0.5rem;\\n}\\n\\n.headerRunDetails {\\n    margin: 0;\\n    margin-bottom: 1.5rem;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n/* ******************************* */\\n/* LABEL IS THE PASS/ERROR BADGE */\\n\\n.label {\\n    display: inline-block;\\n    margin-left: 0.5rem;\\n    color: white;\\n    font-weight: 600;\\n    font-size: 10px;\\n    border-radius: 2px;\\n    padding: 0 4px;\\n    height: 1rem;\\n    line-height: 1rem;\\n    letter-spacing: 0;\\n    display: none;\\n}\\n\\n.errorParent.leafNode .label.F,\\n.errorParent.leafNode .label.E,\\n.errorParent.leafNode .label.FAIL,\\n.errorParent.leafNode .label.ERROR {\\n    display: block;\\n    background-color: var(--log-color-error);\\n}\\n\\n/* hide labels when everything was successful */\\n/*\\n.label.PASS,\\n.label.I,\\n.label.INFO {\\n}\\n*/\\n.errorParent.leafNode .label.W,\\n.errorParent.leafNode .label.WARN {\\n    background-color: var(--log-color-warn);\\n}\\n\\n.label.NOT_RUN {\\n    background-color: var(--log-color-disabled);\\n}\\n\\n/* ******************************* */\\n/* HEADER TITLE ROW */\\n\\n.headerTitleSection {\\n    display: flex;\\n    align-items: center;\\n    margin-top: 0.3rem;\\n    margin-bottom: 0.5rem;\\n}\\n\\n.headerTitleSection h3 {\\n    margin: 0;\\n    padding: 0;\\n    font-size: 1.5rem;\\n}\\n\\n#suiteResult {\\n    font-size: 0.82rem;\\n    padding: 0.1rem 0.3rem 0.15rem 0.3rem;\\n    height: auto;\\n    margin-left: 0.75rem;\\n    display: inline-block;\\n}\\n.headerTitleSection .ERROR {\\n    background-color: var(--log-color-error);\\n}\\n.headerTitleSection .PASS {\\n    background-color: var(--log-color-success);\\n}\\n\',""]);const s=r},645:e=>{e.exports=function(e){var n=[];return n.toString=function(){return this.map((function(n){var t=e(n);return n[2]?"@media ".concat(n[2]," {").concat(t,"}"):t})).join("")},n.i=function(e,t,a){"string"==typeof e&&(e=[[null,e,""]]);var r={};if(a)for(var s=0;s<this.length;s++){var o=this[s][0];null!=o&&(r[o]=!0)}for(var i=0;i<e.length;i++){var l=[].concat(e[i]);a&&r[l[0]]||(t&&(l[2]?l[2]="".concat(t," and ").concat(l[2]):l[2]=t),n.push(l))}},n}},457:(e,n,t)=>{let a;window.setVSCodeAPI=function(e){a=e};let r={};function s(e){let n;try{n=a}catch(e){}n&&n.postMessage(e)}let o={output:void 0},i={setContents:void 0,appendContents:void 0,updateLabel:void 0};window.addEventListener("message",(e=>{let n=e.data;if(n)switch(n.type){case"response":let e=n,t=r[e.request_seq];t&&(delete r[e.request_seq],t(e));break;case"event":let a=o[n.event];a?a(n):console.log("Unhandled event: ",n);break;case"request":let s=i[n.command];s?s(n):console.log("Unhandled request: ",n)}}));let l=0;function d(){return l+=1,l}let c={filterLevel:"PASS",runIdToTreeState:{},runIdLRU:[]},u={initialContents:void 0,runId:void 0,state:void 0,onClickReference:void 0,appendedContents:[],allRunIdsToLabel:{},showTime:!0,showExpand:!0};function m(){return void 0===u.state&&(u.state=function(){let e;try{e=a}catch(e){}if(e){let n=e.getState();return n||(n=c),void 0===n.filterLevel&&(n.filterLevel="PASS"),void 0===n.runIdToTreeState&&(n.runIdToTreeState={}),void 0===!n.runIdLRU&&(n.runIdLRU=[]),n}return c}()),u}function h(e){return document.getElementById(e)}function p(e){return h(e)}function f(e){return h(e)}function g(e){const n=document.createElement("ul");return n.setAttribute("data-tree-id",e),n}function v(){return document.createElement("span")}function y(){return document.createElement("button")}function b(){return document.createElement("div")}function w(e){return e.getAttribute("data-tree-id")}function S(e,n=undefined){if(void 0===n)return"1"===e.getAttribute("data-hidden");n?e.setAttribute("data-hidden","1"):e.removeAttribute("data-hidden")}function C(e){var n=document.createElement("template");return e=e.trim(),n.innerHTML=e,n.content.firstChild}function E(e,n){for(let t of n.childNodes)if(t instanceof HTMLDetailsElement){for(let n of t.childNodes)n instanceof HTMLUListElement&&T(e,n);t.open?e.openNodes[w(n)]="open":delete e.openNodes[w(n)]}}function T(e,n){for(let t of n.childNodes)t instanceof HTMLLIElement&&E(e,t)}const x=((e,n)=>{let t;return function(...e){clearTimeout(t),t=setTimeout((()=>{clearTimeout(t),(()=>{N()})(...e)}),500)}})();function N(){const e=m();!function(e,n){const t=p("mainTree");let a={openNodes:{}};if(void 0===e.runIdLRU&&(e.runIdLRU=[]),void 0===e.runIdToTreeState)e.runIdToTreeState={};else{const t=e.runIdToTreeState[n];t&&(a=t)}for(let e of t.childNodes)e instanceof HTMLUListElement&&T(a,e);e.runIdToTreeState[n]=a;const r=e.runIdLRU.indexOf(n);for(r>-1&&e.runIdLRU.splice(r,1),e.runIdLRU.push(n);e.runIdLRU.length>15;){const n=e.runIdLRU.splice(0,1);delete e.runIdToTreeState[n[0]]}}(e.state,e.runId),function(e){let n;try{n=a}catch(e){}n?n.setState(e):c=e}(e.state)}function I(e,n){if(void 0===e)return;const t=f("selectedRun"),a=new Map;for(let r of t.childNodes)if(r instanceof HTMLOptionElement){const t=r,s=t.value,o=e[s];if(void 0===o)r.remove();else{t.text!==o&&(t.text=o),a.set(s,o);const e=n==s;t.selected=e}}for(const r of Object.keys(e)){if(void 0===r)continue;const s=n==r;if(!a.has(r)){const n=document.createElement("option"),o=e[r];n.value=r,t.appendChild(n),n.selected=s,n.text=o,a.set(r,o)}}}Math.pow(10,8);var L=36e5;function M(e,n){var t;!function(e,n){if(n.length<1)throw new TypeError("1 argument required, but only "+n.length+" present")}(0,arguments);var a=function(e){if(null===e||!0===e||!1===e)return NaN;var n=Number(e);return isNaN(n)?n:n<0?Math.ceil(n):Math.floor(n)}(null!==(t=null==n?void 0:n.additionalDigits)&&void 0!==t?t:2);if(2!==a&&1!==a&&0!==a)throw new RangeError("additionalDigits must be 0, 1 or 2");if("string"!=typeof e&&"[object String]"!==Object.prototype.toString.call(e))return new Date(NaN);var r,s=function(e){var n,t={},a=e.split(k.dateTimeDelimiter);if(a.length>2)return t;if(/:/.test(a[0])?n=a[0]:(t.date=a[0],n=a[1],k.timeZoneDelimiter.test(t.date)&&(t.date=e.split(k.timeZoneDelimiter)[0],n=e.substr(t.date.length,e.length))),n){var r=k.timezone.exec(n);r?(t.time=n.replace(r[1],""),t.timezone=r[1]):t.time=n}return t}(e);if(s.date){var o=function(e,n){var t=new RegExp("^(?:(\\\\d{4}|[+-]\\\\d{"+(4+n)+"})|(\\\\d{2}|[+-]\\\\d{"+(2+n)+"})$)"),a=e.match(t);if(!a)return{year:NaN,restDateString:""};var r=a[1]?parseInt(a[1]):null,s=a[2]?parseInt(a[2]):null;return{year:null===s?r:100*s,restDateString:e.slice((a[1]||a[2]).length)}}(s.date,a);r=function(e,n){if(null===n)return new Date(NaN);var t=e.match(R);if(!t)return new Date(NaN);var a=!!t[4],r=A(t[1]),s=A(t[2])-1,o=A(t[3]),i=A(t[4]),l=A(t[5])-1;if(a)return function(e,n,t){return n>=1&&n<=53&&t>=0&&t<=6}(0,i,l)?function(e,n,t){var a=new Date(0);a.setUTCFullYear(e,0,4);var r=7*(n-1)+t+1-(a.getUTCDay()||7);return a.setUTCDate(a.getUTCDate()+r),a}(n,i,l):new Date(NaN);var d=new Date(0);return function(e,n,t){return n>=0&&n<=11&&t>=1&&t<=(F[n]||(O(e)?29:28))}(n,s,o)&&function(e,n){return n>=1&&n<=(O(e)?366:365)}(n,r)?(d.setUTCFullYear(n,s,Math.max(r,o)),d):new Date(NaN)}(o.restDateString,o.year)}if(!r||isNaN(r.getTime()))return new Date(NaN);var i,l=r.getTime(),d=0;if(s.time&&(d=function(e){var n=e.match(K);if(!n)return NaN;var t=D(n[1]),a=D(n[2]),r=D(n[3]);return function(e,n,t){return 24===e?0===n&&0===t:t>=0&&t<60&&n>=0&&n<60&&e>=0&&e<25}(t,a,r)?t*L+6e4*a+1e3*r:NaN}(s.time),isNaN(d)))return new Date(NaN);if(!s.timezone){var c=new Date(l+d),u=new Date(0);return u.setFullYear(c.getUTCFullYear(),c.getUTCMonth(),c.getUTCDate()),u.setHours(c.getUTCHours(),c.getUTCMinutes(),c.getUTCSeconds(),c.getUTCMilliseconds()),u}return i=function(e){if("Z"===e)return 0;var n=e.match(_);if(!n)return 0;var t="+"===n[1]?-1:1,a=parseInt(n[2]),r=n[3]&&parseInt(n[3])||0;return function(e,n){return n>=0&&n<=59}(0,r)?t*(a*L+6e4*r):NaN}(s.timezone),isNaN(i)?new Date(NaN):new Date(l+d+i)}var k={dateTimeDelimiter:/[T ]/,timeZoneDelimiter:/[Z ]/i,timezone:/([Z+-].*)$/},R=/^-?(?:(\\d{3})|(\\d{2})(?:-?(\\d{2}))?|W(\\d{2})(?:-?(\\d{1}))?|)$/,K=/^(\\d{2}(?:[.,]\\d*)?)(?::?(\\d{2}(?:[.,]\\d*)?))?(?::?(\\d{2}(?:[.,]\\d*)?))?$/,_=/^([+-])(\\d{2})(?::?(\\d{2}))?$/;function A(e){return e?parseInt(e):1}function D(e){return e&&parseFloat(e.replace(",","."))||0}var F=[31,null,31,30,31,30,31,31,30,31,30,31];function O(e){return e%400==0||e%4==0&&e%100!=0}function H(e,n){const t=e.memo[n];return void 0===t?`<ref not found: ${n}>`:t}function U(e,n){return parseFloat(n)}function P(e,n){return parseInt(n)}function B(e,n){return n}function z(e){const n=[],t=new Map;for(let a of e.split(",")){a=a.trim();let e="oid";if(-1!=a.indexOf(":")&&([a,e]=a.split(":",2)),n.push(a),"oid"===e)t.set(a,H);else if("int"===e)t.set(a,P);else if("float"===e)t.set(a,U);else{if("str"!==e)throw new Error("Unexpected: "+e);t.set(a,B)}}return function(e,a){const r=a.split("|",n.length),s={};for(let a=0;a<r.length;a++){const o=r[a],i=n[a];s[i]=t.get(i)(e,o)}return s}}const j=z("name:oid, time_delta_in_seconds:float"),$=z("status:oid, time_delta_in_seconds:float"),V=z("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),q=z("status:oid, message:oid, time_delta_in_seconds:float"),W=z("name:oid, libname:oid, type:oid, doc:oid, source:oid, lineno:int, time_delta_in_seconds:float"),J=z("status:oid, time_delta_in_seconds:float"),Y=z("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),Z={V:function(e,n){return{message:n}},ID:z("part:int, id:str"),I:function(e,n){return JSON.parse(n)},T:function(e,n){return{time:M(n).toString()}},M:function(e,n){var t,a;const r=Q(n,":");if(r){[t,a]=r;try{a=JSON.parse(a)}catch(e){return console.log("Error parsing json: "+a),console.log(e),null}e.memo[t]=a}return null},SR:j,RR:j,ER:$,ST:V,RT:V,ET:q,SE:W,RE:W,EE:J,EA:z("name:oid, value:oid"),L:Y,LH:Y,AS:z("assign:oid"),TG:z("tag:oid"),S:z("start_time_delta:float"),STB:z("message:oid, time_delta_in_seconds:float"),RTB:z("message:oid, time_delta_in_seconds:float"),TBE:z("source:oid, lineno:int, method:oid, line_content:oid"),TBV:z("name:oid, type:oid, value:oid"),ETB:z("time_delta_in_seconds:float")};class G{constructor(){this.memo={}}decode_message_type(e,n){return(0,Z[e])(this,n)}}function Q(e,n){const t=e.indexOf(n);if(t>0)return[e.substring(0,t),e.substring(t+1)]}function*X(e,n){var t,a,r;for(let s of e.split(/\\r?\\n/))if(s=s.trim(),s){const e=Q(s," ");if(e&&([r,a]=e,t=n.decode_message_type(r,a))){const e={message_type:r,decoded:t};yield e}}}function ee(e,n){const t=document.createElement("span");t.textContent=n,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}function ne(e,n){switch(e.state.filterLevel){case"FAIL":return n>=2;case"WARN":return n>=1;case"PASS":return n>=0;case"NOT RUN":return!0}}function te(e){switch(e){case"FAIL":case"ERROR":return 2;case"WARN":return 1;case"NOT RUN":case"NOT_RUN":return-1;default:return 0}}class ae{constructor(e){this.stack=[],this.exceptionMsg=e}pushEntry(e,n,t,a){const r=new Map;this.stack.push({source:e,lineno:n,method:t,lineContent:a,variables:r})}pushVar(e,n,t){this.stack.at(-1).variables.set(`${e} (${n})`,`${t}`)}}class re{constructor(){this.totalTests=0,this.totalFailures=0}clear(){this.totalTests=0,this.totalFailures=0,this.updateSummary()}onTestEndUpdateSummary(e){const n=e.decoded.status;this.totalTests+=1,"FAIL"!=n&&"ERROR"!=n||(this.totalFailures+=1),this.updateSummary()}updateSummary(){const e=p("summary");if(!e)return;const n=(""+this.totalTests).padStart(4),t=(""+this.totalFailures).padStart(4);if(e.textContent=`Total: ${n} Failures: ${t}`,0==this.totalFailures&&0==this.totalTests){const e=p("summary");e.classList.add("NOT_RUN"),e.classList.remove("PASS"),e.classList.remove("FAIL")}else if(1==this.totalFailures){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("PASS"),e.classList.add("FAIL")}else if(0==this.totalFailures&&1==this.totalTests){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("FAIL")}}}function se(e,n){const t=function(e){const n=document.createElement("li");return n.setAttribute("data-tree-id",e),n}(n),a=document.createElement("details");e&&(a.open=e),a.classList.add("NO_CHILDREN"),t.appendChild(a);const r=b();r.classList.add("detailContainer"),a.appendChild(r);const s=document.createElement("summary"),o=b();o.classList.add("summaryDiv"),s.appendChild(o);const i=v();i.className="summaryName",i.textContent="[summaryName]",o.appendChild(i);const l=v();return l.className="summaryInput emptySummaryInput",l.textContent="",o.appendChild(l),a.appendChild(s),{li:t,details:a,summary:s,summaryDiv:o,summaryName:i,summaryInput:l,detailContainer:r}}function oe(e,n,t,a,r,s,o,i,l,d){const c=e.state.runIdToTreeState[e.runId],u="li_"+d;if(c){const e=c.openNodes;e&&(s=e[u])}const m=se(s,u),h=m.li,p=m.details,f=m.detailContainer,v=m.summary,y=m.summaryDiv,b=m.summaryName,w=m.summaryInput;if("LH"===r.message_type){b.textContent="";const e=C(t);b.appendChild(e)}else b.textContent=t;a&&(b.title=a),e.onClickReference&&(b.classList.add("span_link"),b.onclick=n=>{const t=[];let a=l.parent;for(;void 0!==a&&void 0!==a.message;)t.push(a.message),a=a.parent;n.preventDefault(),e.onClickReference({source:o,lineno:i,message:r.decoded,messageType:r.message_type,scope:t})});const S=g("ul_"+d);p.appendChild(S);const E={ul:S,li:h,details:p,detailContainer:f,summary:v,summaryName:b,summaryInput:w,source:o,lineno:i,appendContentChild:void 0,decodedMessage:r,maxLevelFoundInHierarchy:-1,summaryDiv:y};return E.appendContentChild=ue.bind(E),n.appendContentChild(E),E}let ie,le;function*de(e){for(let n of e.childNodes)if(n instanceof HTMLDetailsElement){for(let e of n.childNodes)if(e instanceof HTMLUListElement)for(let n of ce(e))yield n;yield n}}function*ce(e){for(let n of e.childNodes)if(n instanceof HTMLLIElement)for(let e of de(n))yield e}function ue(e){const n=this;n.ul.appendChild(e.li),n.details.classList.contains("NO_CHILDREN")&&(n.details.classList.remove("NO_CHILDREN"),n.details.addEventListener("toggle",(function(){x()})),m().showExpand&&n.summary.addEventListener("mouseover",(e=>{!function(e){if(void 0===ie){ie=b(),ie.classList.add("toolbarContainer");const e=y();e.appendChild(C(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path d="M7 12V7H6v5h1z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),e.onclick=()=>{!function(){if(void 0!==le){le.details.open=!0;for(let e of ce(le.ul))e.classList.contains("NO_CHILDREN")||(e.open=!0)}}()},e.classList.add("toolbarButton");const n=y();return n.appendChild(C(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),n.classList.add("toolbarButton"),n.onclick=()=>{!function(){if(void 0!==le){le.details.open=!1;for(let e of ce(le.ul))e.open=!1}}()},ie.appendChild(n),void ie.appendChild(e)}le=e,e.summaryDiv.appendChild(ie)}(n)})))}var me=(e,n,t)=>new Promise(((a,r)=>{var s=e=>{try{i(t.next(e))}catch(e){r(e)}},o=e=>{try{i(t.throw(e))}catch(e){r(e)}},i=e=>e.done?a(e.value):Promise.resolve(e.value).then(s,o);i((t=t.apply(e,n)).next())}));let he=0,pe=-1;class fe{constructor(){this.stack=[]}handle(e){let n;switch(e.message_type){case"STB":return void this.stack.push(new ae(e.decoded.message));case"TBE":return n=this.stack.at(-1),void n.pushEntry(e.decoded.source,e.decoded.lineno,e.decoded.method,e.decoded.line_content);case"TBV":return n=this.stack.at(-1),void n.pushVar(e.decoded.name,e.decoded.type,e.decoded.value);case"ETB":return n=this.stack.pop(),n.stack.reverse(),n}}}class ge{constructor(){this.stack=[],this.messageNode={parent:void 0,message:void 0},this.id=0,this.finishedAddingInitialContents=!1,this.appendedMessagesIndex=-1,this.decoder=new G,this.seenSuiteTaskOrElement=!1,this.tbHandler=new fe,this.suiteErrored=!1,this.opts=m(),this.runId=this.opts.runId,this.summaryBuilder=new re,this.lease=(he+=1,pe=he,he),this.resetState()}resetState(){this.seenSuiteTaskOrElement=!1}isCurrentTreeBuilder(){return this.lease===pe&&this.runId==this.opts.runId}clearAndInitializeTree(){this.summaryBuilder.clear(),this.resetState();const e=f("filterLevel");e&&(e.value=this.opts.state.filterLevel);const n=p("mainTree");n.replaceChildren();const t=g("ul_root");t.classList.add("tree"),n.appendChild(t),this.parent={ul:void 0,li:void 0,details:void 0,detailContainer:void 0,summary:void 0,summaryName:void 0,summaryInput:void 0,source:void 0,lineno:void 0,decodedMessage:void 0,appendContentChild:function(e){t.appendChild(e.li)},maxLevelFoundInHierarchy:-1,summaryDiv:void 0},this.stack.push(this.parent)}addInitialContents(){return me(this,null,(function*(){for(const e of X(this.opts.initialContents,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}this.finishedAddingInitialContents=!0,yield this.onAppendedContents()}))}onAppendedContents(){return me(this,null,(function*(){if(!this.finishedAddingInitialContents)return;if(!this.isCurrentTreeBuilder())return;const e=m();for(;this.appendedMessagesIndex+1<e.appendedContents.length;){this.appendedMessagesIndex+=1;const n=e.appendedContents[this.appendedMessagesIndex];for(const e of X(n,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}}}))}addOneMessage(e){return me(this,null,(function*(){if(this.isCurrentTreeBuilder())try{this.addOneMessageSync(e)}catch(n){console.log("Error: handling message: "+JSON.stringify(e)+": "+n+" - "+JSON.stringify(n))}}))}addOneMessageSync(e){var n,t;let a,r=e.message_type;switch(r){case"SR":case"ST":case"SE":case"STB":this.seenSuiteTaskOrElement=!0;break;case"RR":if(this.seenSuiteTaskOrElement)return;r="SR";break;case"RT":if(this.seenSuiteTaskOrElement)return;r="ST";break;case"RE":if(this.seenSuiteTaskOrElement)return;r="SE";break;case"RTB":if(this.seenSuiteTaskOrElement)return;r="STB"}switch(this.id+=1,r){case"SR":this.messageNode={parent:this.messageNode,message:e};for(const n of document.querySelectorAll(".suiteHeader"))n.textContent=e.decoded.name;break;case"ST":this.messageNode={parent:this.messageNode,message:e},this.parent=oe(this.opts,this.parent,`${e.decoded.libname}.${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"SE":this.messageNode={parent:this.messageNode,message:e},this.parent=oe(this.opts,this.parent,e.decoded.name,e.decoded.libname,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"ER":this.messageNode=this.messageNode.parent;{const n=p("suiteResult");n.style.display="block",this.suiteErrored?(n.classList.add("ERROR"),n.textContent="Run Failed"):(n.classList.add("PASS"),n.textContent="Run Passed");const t=p("suiteRunStart");t&&(t.textContent+=` - Finished in: ${e.decoded.time_delta_in_seconds.toFixed(2)}s.`)}break;case"ET":this.messageNode=this.messageNode.parent;const r=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(r,this.parent,e),this.onEndSetStatusOrRemove(this.opts,r,e.decoded,this.parent,!1),this.summaryBuilder.onTestEndUpdateSummary(e),a=this.addDetailsCSSClasses(e.decoded.status,r),a&&(this.suiteErrored=!0,r.details.open=!0);break;case"EE":this.messageNode=this.messageNode.parent;let s=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(s,this.parent,e),this.onEndSetStatusOrRemove(this.opts,s,e.decoded,this.parent,!0),a=this.addDetailsCSSClasses(e.decoded.status,s),a&&(s.details.open=!0);break;case"S":const o=e.decoded.start_time_delta;(null==(t=null==(n=this.parent)?void 0:n.decodedMessage)?void 0:t.decoded)&&(this.parent.decodedMessage.decoded.time_delta_in_seconds=o);break;case"EA":const i=this.stack.at(-1);i.summaryInput.classList.contains("emptySummaryInput")?(i.summaryInput.textContent=`${e.decoded.name}=${e.decoded.value}`,i.summaryInput.classList.remove("emptySummaryInput")):i.summaryInput.textContent+=`, ${e.decoded.name}=${e.decoded.value}`;break;case"L":case"LH":const l=e.decoded.level,d=function(e){switch(e){case"E":case"F":return 2;case"W":return 1;default:return 0}}(l);if(d>this.parent.maxLevelFoundInHierarchy&&(this.parent.maxLevelFoundInHierarchy=d),ne(this.opts,d)){const n=oe(this.opts,this.parent,e.decoded.message,"",e,!1,void 0,void 0,this.messageNode,this.id.toString());n.maxLevelFoundInHierarchy=d,function(e,n){const t=document.createElement("span");t.textContent=`LOG ${function(e){switch(e){case"E":return"ERROR";case"F":return"FAIL";case"W":return"WARN";case"I":return"INFO";default:return e}}(n)}`,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}(n,l),this.addDetailsCSSClasses(d,n)}break;case"STB":case"TBE":case"TBV":case"ETB":const c=this.tbHandler.handle(e);c&&function(e,n){const t=b();t.classList.add("detailInfo");const a=b();a.classList.add("errorHeader"),a.textContent=n.exceptionMsg,t.appendChild(a);const r=[];for(const e of n.stack){let n=e.source;n.length>31&&(n=`... ${n.substring(27)}`),r.push(`File "${n}", line ${e.lineno}, in ${e.method}\\n`),r.push(`    ${e.lineContent}\\n`);for(const[n,t]of e.variables.entries())r.push(`        💠 ${n} = ${t}\\n`)}const s=b();s.classList.add("errorDetails"),s.style.whiteSpace="pre",s.textContent=r.join(""),t.appendChild(s),e.detailContainer.appendChild(t);const o=b();o.classList.add("detailInputs"),o.textContent=" ",e.detailContainer.appendChild(o),e.details.classList.add("parentNode")}(this.parent,c);break;case"T":const u=p("suiteRunStart");u&&(u.textContent=e.decoded.time)}}addDetailsCSSClasses(e,n){let t,a=!1;return t="string"==typeof e?te(e):e,t>=2?(n.details.classList.add("errorParent"),a=!0):1==t?n.details.classList.add("warnParent"):n.details.classList.add("passParent"),n.details.classList.contains("parentNode")||n.details.classList.contains("leafNode")||(0===n.ul.children.length?n.details.classList.add("leafNode"):n.details.classList.add("parentNode")),a}onEndUpdateMaxLevelFoundInHierarchyFromStatus(e,n,t){const a=te(t.decoded.status);a>e.maxLevelFoundInHierarchy&&(e.maxLevelFoundInHierarchy=a),e.maxLevelFoundInHierarchy>n.maxLevelFoundInHierarchy&&(n.maxLevelFoundInHierarchy=e.maxLevelFoundInHierarchy)}onEndSetStatusOrRemove(e,n,t,a,r){const s=t.status;if(ne(e,n.maxLevelFoundInHierarchy)){if(r&&n.maxLevelFoundInHierarchy<=0){const e=50;if(a.ul.childElementCount>e){const e=n.summaryName.textContent;if(e&&e.toLowerCase().includes("iteration")){const e=n.li.previousSibling,t=w(n.li);if(n.li.remove(),S(e))e.getElementsByClassName("FINAL_SPAN")[0].textContent=n.summaryName.textContent;else{const e=se(!1,t);e.summaryName.textContent=n.summaryName.textContent,e.summary.classList.add("HIDDEN");const r=v();r.setAttribute("role","button"),r.textContent="...",r.classList.add("label"),r.classList.add("HIDDEN"),r.classList.add("inline"),e.summaryDiv.appendChild(r);const s=v();s.setAttribute("role","button"),s.classList.add("FINAL_SPAN"),e.summaryDiv.appendChild(s),ee(e,"HIDDEN"),S(e.li,!0),a.ul.appendChild(e.li)}return}}}if(n.summary,ee(n,s),null!=n.source&&n.source.length>0){const e=function(e){let n=e,t=Math.max(e.lastIndexOf("/"),e.lastIndexOf("\\\\"));return t>0&&(n=e.substring(t+1)),n}(n.source),t=document.createElement("span");t.textContent=e,t.classList.add("summaryFileName"),t.title=n.source,n.summaryDiv.appendChild(t)}if(this.opts.showTime){const e=n.decodedMessage.decoded.time_delta_in_seconds;void 0!==e&&e>=0&&function(e,n){const t=document.createElement("span");t.textContent=` (${n.toFixed(2)}s)`,t.classList.add("timeLabel"),e.summaryDiv.appendChild(t)}(n,t.time_delta_in_seconds-e)}}else n.li.remove()}}var ve=(e,n,t)=>new Promise(((a,r)=>{var s=e=>{try{i(t.next(e))}catch(e){r(e)}},o=e=>{try{i(t.throw(e))}catch(e){r(e)}},i=e=>e.done?a(e.value):Promise.resolve(e.value).then(s,o);i((t=t.apply(e,n)).next())}));let ye;function be(){return ve(this,null,(function*(){ye=new ge,ye.clearAndInitializeTree(),yield ye.addInitialContents()}))}function we(e){let n={type:"event",seq:d(),event:"onClickReference"};n.data=e,s(n)}function Se(e){N();const n=m();n.runId=e.runId,n.initialContents=e.initialContents,void 0!==a&&(n.onClickReference=we),n.appendedContents=[],n.allRunIdsToLabel=e.allRunIdsToLabel,I(n.allRunIdsToLabel,n.runId),be()}t(739),i.setContents=Se,i.appendContents=function(e){const n=m();n.runId===e.runId&&(n.appendedContents.push(e.appendContents),void 0!==ye&&ye.onAppendedContents())},i.updateLabel=function(e){const n=m();n.allRunIdsToLabel[e.runId]=e.label,I(n.allRunIdsToLabel,n.runId)},window.onChangedRun=function(){const e=f("selectedRun").value;let n={type:"event",seq:d(),event:"onSetCurrentRunId"};n.data={runId:e},s(n)},window.onChangedFilterLevel=function(){!function(e){const n=m();n.state.filterLevel!==e&&(n.state.filterLevel=e,N(),be())}(f("filterLevel").value)},window.setContents=Se,window.setShowTime=function(e){m().showTime=e},window.setShowExpand=function(e){m().showExpand=e},window.getSampleContents=function(){return JSON.parse(\'"V 1\\\\nI \\\\"sys.platform=win32\\\\"\\\\nI \\\\"python=3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)]\\\\"\\\\nI \\\\"robot=5.1a3.dev1\\\\"\\\\nT 2022-10-19T09:48:34.018\\\\nM a:\\\\"Robot1\\\\"\\\\nM b:\\\\"s1\\\\"\\\\nM c:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\robot1.robot\\\\"\\\\nSS a|b|c|0.035\\\\nM d:\\\\"Simple Task\\\\"\\\\nM e:\\\\"s1-t1\\\\"\\\\nST d|e|16|0.036\\\\nM f:\\\\"First keyword\\\\"\\\\nM g:\\\\"\\\\"\\\\nM h:\\\\"KEYWORD\\\\"\\\\nSK f|g|h|g|c|17|0.036\\\\nM i:\\\\"No Operation\\\\"\\\\nM j:\\\\"BuiltIn\\\\"\\\\nM k:\\\\"Does absolutely nothing.\\\\"\\\\nSK i|j|h|k|c|8|0.037\\\\nM l:\\\\"PASS\\\\"\\\\nEK l|0.037\\\\nM m:\\\\"Log\\\\"\\\\nM n:\\\\"Logs the given message with the given level.\\\\"\\\\nSK m|j|h|n|c|10|0.037\\\\nM o:\\\\"Some warning message\\\\"\\\\nKA o\\\\nM p:\\\\"level=WARN\\\\"\\\\nKA p\\\\nEK l|0.046\\\\nM q:\\\\"Another keyword\\\\"\\\\nM r:\\\\"another\\\\"\\\\nSK q|r|h|g|c|11|0.047\\\\nM s:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\another.robot\\\\"\\\\nSK i|j|h|k|s|3|0.047\\\\nEK l|0.047\\\\nEK l|0.047\\\\nM t:\\\\"Another in sub keyword\\\\"\\\\nM u:\\\\"another_sub\\\\"\\\\nSK t|u|h|g|c|12|0.047\\\\nM v:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\sub\\\\\\\\\\\\\\\\another_sub.robot\\\\"\\\\nSK i|j|h|k|v|6|0.048\\\\nEK l|0.048\\\\nSK m|j|h|n|v|7|0.048\\\\nM w:\\\\"Some error message\\\\"\\\\nKA w\\\\nM x:\\\\"level=ERROR\\\\"\\\\nKA x\\\\nEK l|0.049\\\\nEK l|0.049\\\\nEK l|0.049\\\\nSK m|j|h|n|c|18|0.049\\\\nM y:\\\\"Some <data &encode <\\/script>\\\\"\\\\nKA y\\\\nEK l|0.049\\\\nM z:\\\\"Create Dictionary\\\\"\\\\nM A:\\\\"Creates and returns a dictionary based on the given ``items``.\\\\"\\\\nSK z|j|h|A|c|19|0.049\\\\nM B:\\\\"a=1\\\\"\\\\nKA B\\\\nM C:\\\\"b=1\\\\"\\\\nKA C\\\\nEK l|0.05\\\\nSK m|j|h|n|c|20|0.05\\\\nM D:\\\\"${dct}\\\\"\\\\nKA D\\\\nEK l|0.051\\\\nET l|g|0.051\\\\nM E:\\\\"Check 1\\\\"\\\\nM F:\\\\"s1-t2\\\\"\\\\nST E|F|22|0.051\\\\nSK f|g|h|g|c|23|0.051\\\\nSK i|j|h|k|c|8|0.052\\\\nEK l|0.052\\\\nSK m|j|h|n|c|10|0.052\\\\nKA o\\\\nKA p\\\\nEK l|0.052\\\\nSK q|r|h|g|c|11|0.053\\\\nSK i|j|h|k|s|3|0.053\\\\nEK l|0.053\\\\nEK l|0.053\\\\nSK t|u|h|g|c|12|0.053\\\\nSK i|j|h|k|v|6|0.054\\\\nEK l|0.054\\\\nSK m|j|h|n|v|7|0.054\\\\nKA w\\\\nKA x\\\\nEK l|0.054\\\\nEK l|0.055\\\\nEK l|0.055\\\\nM G:\\\\"${counter} IN RANGE [ 0 | 3 ]\\\\"\\\\nM H:\\\\"FOR\\\\"\\\\nSK G|g|H|g|c|25|0.055\\\\nM I:\\\\"${counter} = 0\\\\"\\\\nM J:\\\\"ITERATION\\\\"\\\\nSK I|g|J|g|c|25|0.055\\\\nM K:\\\\"${counter} == 2\\\\"\\\\nM L:\\\\"IF\\\\"\\\\nSK K|g|L|g|c|26|0.055\\\\nM M:\\\\"Fail\\\\"\\\\nM N:\\\\"Fails the test with the given message and optionally alters its tags.\\\\"\\\\nSK M|j|h|N|c|27|0.056\\\\nM O:\\\\"Failed execution for some reason...\\\\"\\\\nKA O\\\\nM P:\\\\"NOT RUN\\\\"\\\\nEK P|0.056\\\\nEK P|0.056\\\\nSK m|j|h|n|c|29|0.056\\\\nM Q:\\\\"${counter}\\\\"\\\\nKA Q\\\\nEK l|0.056\\\\nEK l|0.057\\\\nM R:\\\\"${counter} = 1\\\\"\\\\nSK R|g|J|g|c|25|0.057\\\\nSK K|g|L|g|c|26|0.057\\\\nSK M|j|h|N|c|27|0.057\\\\nKA O\\\\nEK P|0.057\\\\nEK P|0.057\\\\nSK m|j|h|n|c|29|0.058\\\\nKA Q\\\\nEK l|0.058\\\\nEK l|0.058\\\\nM S:\\\\"${counter} = 2\\\\"\\\\nSK S|g|J|g|c|25|0.058\\\\nSK K|g|L|g|c|26|0.058\\\\nSK M|j|h|N|c|27|0.059\\\\nKA O\\\\nM T:\\\\"FAIL\\\\"\\\\nEK T|0.059\\\\nEK T|0.059\\\\nSK m|j|h|n|c|29|0.059\\\\nKA Q\\\\nEK P|0.059\\\\nEK T|0.06\\\\nEK T|0.06\\\\nET T|O|0.06\\\\nM U:\\\\"Check 2\\\\"\\\\nM V:\\\\"s1-t3\\\\"\\\\nST U|V|32|0.06\\\\nM W:\\\\"Set Variable\\\\"\\\\nM X:\\\\"Returns the given values which can then be assigned to a variables.\\\\"\\\\nSK W|j|h|X|c|33|0.061\\\\nM Y:\\\\"3\\\\"\\\\nKA Y\\\\nEK l|0.061\\\\nM Z:\\\\"${counter} <= 2\\\\"\\\\nM 0:\\\\"WHILE\\\\"\\\\nSK Z|g|0|g|c|34|0.061\\\\nSK g|g|J|g|c|34|0.062\\\\nM 1:\\\\"Evaluate\\\\"\\\\nM 2:\\\\"Evaluates the given expression in Python and returns the result.\\\\"\\\\nSK 1|j|h|2|c|35|0.062\\\\nM 4:\\\\"$counter-1\\\\"\\\\nKA 4\\\\nEK P|0.062\\\\nSK m|j|h|n|c|36|0.062\\\\nM 5:\\\\"Current counter: ${counter}\\\\"\\\\nKA 5\\\\nKA p\\\\nEK P|0.062\\\\nEK P|0.062\\\\nEK P|0.063\\\\nET l|g|0.063\\\\nM 6:\\\\"Check 3\\\\"\\\\nM 7:\\\\"s1-t4\\\\"\\\\nST 6|7|39|0.064\\\\nM 8:\\\\"TRY\\\\"\\\\nSK g|g|8|g|c|40|0.064\\\\nSK i|j|h|k|c|41|0.064\\\\nEK l|0.064\\\\nEK l|0.064\\\\nM 9:\\\\"message\\\\"\\\\nM aa:\\\\"EXCEPT\\\\"\\\\nSK 9|g|aa|g|c|42|0.064\\\\nSK i|j|h|k|c|43|0.065\\\\nEK P|0.065\\\\nEK P|0.065\\\\nM ab:\\\\"FINALLY\\\\"\\\\nSK g|g|ab|g|c|44|0.065\\\\nSK i|j|h|k|c|45|0.065\\\\nEK l|0.065\\\\nEK l|0.065\\\\nET l|g|0.066\\\\nES T|0.067\\\\n"\')}},739:(e,n,t)=>{var a=t(379),r=t.n(a),s=t(599),o={injectType:"singletonStyleTag",insert:"head",singleton:!0};r()(s.Z,o),s.Z.locals},379:(e,n,t)=>{var a,r=function(){var e={};return function(n){if(void 0===e[n]){var t=document.querySelector(n);if(window.HTMLIFrameElement&&t instanceof window.HTMLIFrameElement)try{t=t.contentDocument.head}catch(e){t=null}e[n]=t}return e[n]}}(),s=[];function o(e){for(var n=-1,t=0;t<s.length;t++)if(s[t].identifier===e){n=t;break}return n}function i(e,n){for(var t={},a=[],r=0;r<e.length;r++){var i=e[r],l=n.base?i[0]+n.base:i[0],d=t[l]||0,c="".concat(l," ").concat(d);t[l]=d+1;var u=o(c),m={css:i[1],media:i[2],sourceMap:i[3]};-1!==u?(s[u].references++,s[u].updater(m)):s.push({identifier:c,updater:f(m,n),references:1}),a.push(c)}return a}function l(e){var n=document.createElement("style"),a=e.attributes||{};if(void 0===a.nonce){var s=t.nc;s&&(a.nonce=s)}if(Object.keys(a).forEach((function(e){n.setAttribute(e,a[e])})),"function"==typeof e.insert)e.insert(n);else{var o=r(e.insert||"head");if(!o)throw new Error("Couldn\'t find a style target. This probably means that the value for the \'insert\' parameter is invalid.");o.appendChild(n)}return n}var d,c=(d=[],function(e,n){return d[e]=n,d.filter(Boolean).join("\\n")});function u(e,n,t,a){var r=t?"":a.media?"@media ".concat(a.media," {").concat(a.css,"}"):a.css;if(e.styleSheet)e.styleSheet.cssText=c(n,r);else{var s=document.createTextNode(r),o=e.childNodes;o[n]&&e.removeChild(o[n]),o.length?e.insertBefore(s,o[n]):e.appendChild(s)}}function m(e,n,t){var a=t.css,r=t.media,s=t.sourceMap;if(r?e.setAttribute("media",r):e.removeAttribute("media"),s&&"undefined"!=typeof btoa&&(a+="\\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(s))))," */")),e.styleSheet)e.styleSheet.cssText=a;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(a))}}var h=null,p=0;function f(e,n){var t,a,r;if(n.singleton){var s=p++;t=h||(h=l(n)),a=u.bind(null,t,s,!1),r=u.bind(null,t,s,!0)}else t=l(n),a=m.bind(null,t,n),r=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(t)};return a(e),function(n){if(n){if(n.css===e.css&&n.media===e.media&&n.sourceMap===e.sourceMap)return;a(e=n)}else r()}}e.exports=function(e,n){(n=n||{}).singleton||"boolean"==typeof n.singleton||(n.singleton=(void 0===a&&(a=Boolean(window&&document&&document.all&&!window.atob)),a));var t=i(e=e||[],n);return function(e){if(e=e||[],"[object Array]"===Object.prototype.toString.call(e)){for(var a=0;a<t.length;a++){var r=o(t[a]);s[r].references--}for(var l=i(e,n),d=0;d<t.length;d++){var c=o(t[d]);0===s[c].references&&(s[c].updater(),s.splice(c,1))}t=l}}}}},n={};function t(a){var r=n[a];if(void 0!==r)return r.exports;var s=n[a]={id:a,exports:{}};return e[a](s,s.exports,t),s.exports}t.n=e=>{var n=e&&e.__esModule?()=>e.default:()=>e;return t.d(n,{a:n}),n},t.d=(e,n)=>{for(var a in n)t.o(n,a)&&!t.o(e,a)&&Object.defineProperty(e,a,{enumerable:!0,get:n[a]})},t.o=(e,n)=>Object.prototype.hasOwnProperty.call(e,n),t.nc=void 0,t(457),t(739)})();</script></body><script>window.setShowTime(true);\n    window.setShowExpand(false);\n    try {\n        const vscode = acquireVsCodeApi();\n        window.setVSCodeAPI(vscode);\n        document.getElementById("selectRunContainer").style.display = "block";\n    } catch (err) {\n        // That\'s ok (not running in VSCode).\n        window.setContents({\n            "initialContents": window.getSampleContents(),\n        });\n    }</script></html>'}
+FILE_CONTENTS = {'index.html': '<!doctype html><html><head><meta charset="utf-8"/><title class="suiteHeader">Robocorp Log</title><meta name="viewport" content="width=device-width,initial-scale=1"/></head><body><div class="headerTitleSection"><h3 class="suiteHeader">Robocorp Log</h3><span id="suiteResult" class="label" style="display: none;"></span></div><div id="suiteRunStart" class="headerRunDetails"></div><div class="headers"><span class="headerSource">Source</span> <span class="headerInputs">Input Arguments</span></div><div id="mainTree"></div><script>(()=>{"use strict";var e={599:(e,n,t)=>{t.d(n,{Z:()=>s});var a=t(645),o=t.n(a)()((function(e){return e[1]}));o.push([e.id,\'/* ******************************* */\\n/* CONTAINERS ETC */\\n\\n/* box model reset */\\n* {\\n    box-sizing: border-box;\\n}\\n\\nhtml,\\nbody {\\n    margin: 0;\\n    padding: 0;\\n    height: 100%;\\n}\\n\\n:root {\\n    --right-column-width-narrow: 40vw;\\n    --right-column-width-wide: 50vw;\\n    /* from here: https://qwtel.com/posts/software/the-monospaced-system-ui-css-font-stack/ */\\n    --sans-font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", "Roboto", "Oxygen", "Ubuntu",\\n        "Cantarell", "Fira Sans", "Droid Sans", "Helvetica Neue", Arial, sans-serif;\\n    /* from here: https://qwtel.com/posts/software/the-monospaced-system-ui-css-font-stack/ */\\n    --fixed-font-family: ui-monospace, Menlo, Monaco, "Cascadia Mono", "Segoe UI Mono", "Roboto Mono", "Oxygen Mono",\\n        "Ubuntu Monospace", "Source Code Pro", "Fira Mono", "Droid Sans Mono", "Courier New", monospace;\\n}\\n\\n/* ******************************* */\\n/* THEMING SUPPORT */\\n\\n@media (prefers-color-scheme: light) {\\n    :root {\\n        --log-color-error: #e84f5c;\\n        --log-color-success: #219f7f;\\n        --log-color-variable: #5070b4;\\n\\n        --log-color-warn: #93801c;\\n        --log-color-disabled: #999999;\\n        --log-color-border: #dddddd;\\n\\n        --log-color-text: #000000;\\n        --log-color-text-weaker: #444444;\\n        --log-color-text-weakest: #666666;\\n\\n        --log-color-bg: #ffffff;\\n        --log-color-bg-raised: #f3f3f3;\\n    }\\n}\\n\\n@media (prefers-color-scheme: dark) {\\n    :root {\\n        --log-color-error: #e84f5c;\\n        --log-color-success: #219f7f;\\n        --log-color-warn: #fff565;\\n        --log-color-variable: #4094c5;\\n\\n        --log-color-disabled: #666666;\\n        --log-color-border: #444444;\\n\\n        --log-color-text: #eeeeee;\\n        --log-color-text-weaker: #bbbbbb;\\n        --log-color-text-weakest: #666666;\\n\\n        --log-color-bg: #222222;\\n        --log-color-bg-raised: #333333;\\n    }\\n}\\n\\nbody {\\n    display: flex;\\n    flex-direction: column;\\n    padding: 1rem;\\n    font-size: 0.8rem;\\n    font-family: var(--sans-font-family);\\n    color: var(--log-color-text);\\n    background-color: var(--log-color-bg);\\n}\\n\\nul {\\n    list-style-type: none;\\n    padding-inline-start: 0px;\\n    margin-block-start: 0px;\\n}\\n\\n#mainTree {\\n    white-space: nowrap;\\n    overflow: auto;\\n    flex-grow: 1;\\n}\\n\\n/* ******************************* */\\n/* TREE */\\n\\n.tree li {\\n    display: block;\\n    position: relative;\\n    padding-left: 0px;\\n}\\n\\n/* nesting level vertical line */\\n.tree ul:not(:first-child),\\n.detailContainer {\\n    border-left: 1px solid var(--log-color-border);\\n\\n    /* centering the line with the icon */\\n    margin-left: 0.65rem;\\n\\n    /* nesting indentation */\\n    padding-left: 0.8rem;\\n}\\n\\ndetails.errorParent .tree ul:not(:first-child),\\ndetails.errorParent .detailContainer {\\n    border-color: var(--log-color-error);\\n}\\n\\n/* ******************************* */\\n/* SUMMARY ROW FOR EACH CODE ROW */\\n\\ndetails.parentNode > summary,\\ndetails.errorParent.leafNode > summary {\\n    cursor: pointer;\\n}\\n\\ndetails > summary {\\n    padding-top: 0.25rem;\\n    padding-bottom: 0.25rem;\\n    padding-left: 0.25rem;\\n\\n    /* chrome needs this, safari doesn\\\'t */\\n    list-style: none;\\n}\\n\\ndetails > summary:hover {\\n    background-color: var(--log-color-bg-raised);\\n    border-radius: 2px;\\n}\\n\\ndetails > summary::-webkit-details-marker {\\n    display: none;\\n}\\n\\ndetails > summary::marker {\\n    display: none;\\n}\\n\\ndetails > summary::before {\\n    background-color: var(--log-color-success);\\n}\\n\\ndetails.errorParent > summary::before {\\n    background-color: var(--log-color-error);\\n}\\n\\ndetails.warnParent > summary::before {\\n    background-color: var(--log-color-warn);\\n}\\n\\n/* icon from: https://github.com/twbs/icons/blob/main/icons/caret-right-square-fill.svg */\\ndetails > summary::before {\\n    position: absolute;\\n    left: 0.25rem;\\n    top: 4px;\\n\\n    /* chrome seems to need the \\\'-webkit\\\' prefix here */\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="black" class="bi bi-caret-right-square-fill" viewBox="0 0 16 16"><path d="M0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2V2zm5.5 10a.5.5 0 0 0 .832.374l4.5-4a.5.5 0 0 0 0-.748l-4.5-4A.5.5 0 0 0 5.5 4v8z"/></svg>\\\');\\n    width: 1rem;\\n    height: 1rem;\\n    display: inline-block;\\n    content: "";\\n}\\n\\n/* filled icon */\\n/*details.leafNode.passParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square-fill" viewBox="0 0 16 16"><path d="M2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2zm10.03 4.97a.75.75 0 0 1 .011 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.75.75 0 0 1 1.08-.022z"/></svg>\\\');\\n}*/\\n\\ndetails.leafNode.passParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path d="M14 1a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1h12zM2 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H2z"/><path d="M10.97 4.97a.75.75 0 0 1 1.071 1.05l-3.992 4.99a.75.75 0 0 1-1.08.02L4.324 8.384a.75.75 0 1 1 1.06-1.06l2.094 2.093 3.473-4.425a.235.235 0 0 1 .02-.022z"/></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (symbol-variable) */\\ndetails.leafNode.variableParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M2 5h2V4H1.5l-.5.5v8l.5.5H4v-1H2V5zm12.5-1H12v1h2v7h-2v1h2.5l.5-.5v-8l-.5-.5zm-2.74 2.57L12 7v2.51l-.3.45-4.5 2h-.46l-2.5-1.5-.24-.43v-2.5l.3-.46 4.5-2h.46l2.5 1.5zM5 9.71l1.5.9V9.28L5 8.38v1.33zm.58-2.15l1.45.87 3.39-1.5-1.45-.87-3.39 1.5zm1.95 3.17l3.5-1.56v-1.4l-3.5 1.55v1.41z"></path></svg>\\\');\\n    background-color: var(--log-color-variable);\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (bracket-error) */\\ndetails.leafNode.exceptionParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M6 2.97184V2.98361H5.91083C5.71113 2.98361 5.5238 3.02427 5.34802 3.10513C5.17461 3.18275 5.02193 3.28942 4.89086 3.42437C4.76421 3.55475 4.66135 3.71034 4.58238 3.89205C4.50833 4.07152 4.47134 4.26019 4.47134 4.45902C4.47134 4.68725 4.4753 4.9134 4.48321 5.13749C4.49125 5.36105 4.49127 5.58262 4.48324 5.80219C4.47914 6.01973 4.46082 6.2333 4.42826 6.44285C4.39513 6.65175 4.33913 6.85263 4.26039 7.04464C4.18091 7.23843 4.07258 7.42254 3.93616 7.59702C3.82345 7.74119 3.68538 7.87538 3.52283 8C3.68538 8.12462 3.82345 8.25881 3.93616 8.40298C4.07258 8.57746 4.18091 8.76157 4.26039 8.95536C4.33921 9.14757 4.39513 9.35024 4.42823 9.56312C4.46084 9.76883 4.47914 9.98246 4.48324 10.2039C4.49127 10.4195 4.49125 10.6411 4.48321 10.8686C4.4753 11.0885 4.47134 11.3127 4.47134 11.541C4.47134 11.744 4.50838 11.9346 4.58223 12.1137C4.66104 12.2911 4.76386 12.4469 4.89086 12.5818C5.02194 12.7126 5.17396 12.8191 5.34763 12.9008C5.52346 12.9777 5.71095 13.0164 5.91083 13.0164H6V13.2V14H5.91083C5.59743 14 5.29407 13.9384 5.00128 13.8153C4.70818 13.692 4.44942 13.5153 4.22578 13.285C4.00311 13.0558 3.83793 12.805 3.73283 12.5323L3.73232 12.531C3.63387 12.265 3.56819 11.9903 3.53535 11.7072L3.53516 11.7055C3.50677 11.4215 3.4987 11.1316 3.51084 10.8357C3.52272 10.5462 3.52866 10.2567 3.52866 9.96721C3.52866 9.76883 3.48986 9.58047 3.41201 9.40108L3.41129 9.39942C3.33659 9.21871 3.23428 9.0637 3.10412 8.93352L3.10221 8.93161C2.97577 8.79762 2.82457 8.69157 2.64742 8.61396L2.64601 8.61334C2.47001 8.53238 2.28465 8.4918 2.08917 8.4918H2V8.4V7.6V7.5082H2.08917C2.28497 7.5082 2.4706 7.46954 2.64672 7.3925C2.82466 7.31055 2.97644 7.20405 3.10317 7.07359C3.23423 6.93866 3.33687 6.78296 3.4116 6.60601L3.412 6.60507C3.48974 6.42594 3.52866 6.23556 3.52866 6.03279C3.52866 5.74329 3.52272 5.45379 3.51084 5.16428C3.4987 4.86844 3.50678 4.5805 3.53519 4.30053L3.53533 4.29917C3.56814 4.01201 3.63382 3.7352 3.73233 3.46898L3.73282 3.46766C3.83792 3.19498 4.00311 2.94422 4.22578 2.71498C4.44942 2.48474 4.70818 2.30798 5.00128 2.18473C5.29407 2.06161 5.59743 2 5.91083 2H6V2.97184ZM13.9232 8.4918H14V8.4V7.6V7.5082H13.9108C13.7153 7.5082 13.53 7.46762 13.354 7.38666L13.3526 7.38604C13.1754 7.30844 13.0242 7.20238 12.8978 7.06839L12.8959 7.06648C12.7657 6.9363 12.6634 6.78129 12.5887 6.60058L12.588 6.59892C12.5101 6.41953 12.4713 6.23117 12.4713 6.03279C12.4713 5.74329 12.4773 5.45379 12.4892 5.16428C12.5013 4.86842 12.4932 4.57848 12.4648 4.29454L12.4646 4.29285C12.4318 4.00971 12.3661 3.73502 12.2677 3.46897L12.2672 3.46766C12.1621 3.19499 11.9969 2.94422 11.7742 2.71498C11.5506 2.48474 11.2918 2.30798 10.9987 2.18473C10.7059 2.06161 10.4026 2 10.0892 2H10V2.8V2.98361H10.0892C10.2891 2.98361 10.4765 3.0223 10.6524 3.09917C10.826 3.18092 10.9781 3.28736 11.1091 3.41823C11.2361 3.55305 11.339 3.70889 11.4178 3.88628C11.4916 4.0654 11.5287 4.25596 11.5287 4.45902C11.5287 4.68727 11.5247 4.91145 11.5168 5.13142C11.5088 5.35894 11.5087 5.58049 11.5168 5.79605C11.5209 6.01754 11.5392 6.23117 11.5718 6.43688C11.6049 6.64976 11.6608 6.85243 11.7396 7.04464C11.8191 7.23843 11.9274 7.42254 12.0638 7.59702C12.1765 7.74119 12.3146 7.87538 12.4772 8L12.4456 8.02455C12.9764 8.08338 13.4758 8.24605 13.9232 8.4918Z"></path><path fill-rule="evenodd" clip-rule="evenodd" d="M10.3333 9.50559C10.8266 9.17595 11.4067 9 12 9C12.7954 9.00098 13.5578 9.31736 14.1202 9.87976C14.6826 10.4422 14.999 11.2047 15 12C15 12.5933 14.8241 13.1734 14.4944 13.6667C14.1648 14.1601 13.6962 14.5446 13.1481 14.7716C12.5999 14.9987 11.9967 15.0581 11.4147 14.9424C10.8328 14.8266 10.2982 14.5409 9.87868 14.1213C9.45912 13.7018 9.1734 13.1672 9.05765 12.5853C8.94189 12.0033 9.0013 11.4001 9.22836 10.8519C9.45543 10.3038 9.83994 9.83524 10.3333 9.50559ZM13.1464 10.1464L12 11.2929L10.8536 10.1464L10.1465 10.8535L11.2929 12L10.1464 13.1464L10.8536 13.8536L12 12.7071L13.1465 13.8535L13.8536 13.1464L12.7071 12L13.8536 10.8536L13.1464 10.1464Z"></path></svg>\\\');\\n    background-color: var(--log-color-error);\\n}\\n.exceptionParent {\\n    font-weight: bold;\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (error) */\\ndetails.leafNode.errorParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M8.6 1c1.6.1 3.1.9 4.2 2 1.3 1.4 2 3.1 2 5.1 0 1.6-.6 3.1-1.6 4.4-1 1.2-2.4 2.1-4 2.4-1.6.3-3.2.1-4.6-.7-1.4-.8-2.5-2-3.1-3.5C.9 9.2.8 7.5 1.3 6c.5-1.6 1.4-2.9 2.8-3.8C5.4 1.3 7 .9 8.6 1zm.5 12.9c1.3-.3 2.5-1 3.4-2.1.8-1.1 1.3-2.4 1.2-3.8 0-1.6-.6-3.2-1.7-4.3-1-1-2.2-1.6-3.6-1.7-1.3-.1-2.7.2-3.8 1-1.1.8-1.9 1.9-2.3 3.3-.4 1.3-.4 2.7.2 4 .6 1.3 1.5 2.3 2.7 3 1.2.7 2.6.9 3.9.6zM7.9 7.5L10.3 5l.7.7-2.4 2.5 2.4 2.5-.7.7-2.4-2.5-2.4 2.5-.7-.7 2.4-2.5-2.4-2.5.7-.7 2.4 2.5z"/></svg>\\\');\\n}\\n\\n/* https://www.svgrepo.com/collection/codicons-coding-icons/ (warn) */\\ndetails.leafNode.warnParent > summary::before {\\n    -webkit-mask: url(\\\'data:image/svg+xml;charset=UTF-8,<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-check-square" viewBox="0 0 16 16"><path fill-rule="evenodd" clip-rule="evenodd" d="M7.56 1h.88l6.54 12.26-.44.74H1.44L1 13.26 7.56 1zM8 2.28L2.28 13H13.7L8 2.28zM8.625 12v-1h-1.25v1h1.25zm-1.25-2V6h1.25v4h-1.25z"/></svg>\\\');\\n}\\n\\ndetails.parentNode > summary::before,\\ndetails.parentNode.errorParent > summary::before {\\n    transform-origin: 8px 8px;\\n    transform: rotate(0deg);\\n    transition: transform 0.2s ease-out !important;\\n}\\n\\ndetails[open].parentNode > summary::before,\\ndetails[open].parentNode.errorParent > summary::before {\\n    transform: rotate(90deg);\\n}\\n\\ndetails[open] > summary > .summaryDiv > .summaryInput {\\n    /* Display full input parameters when expanded by adjusting the\\n       white-space to wrap the contents. Even nodes that don\\\'t have\\n       children can be expanded in this way, but it is not obvious\\n       since there is no triangle icon next to them. */\\n    white-space: initial;\\n}\\n\\n.summaryDiv {\\n    /* aligns code line correctly with the icon */\\n    display: flex;\\n    margin-left: 1.2rem;\\n}\\n\\n.summaryDiv > .label {\\n    order: 2;\\n}\\n\\n.summaryDiv > .summaryName {\\n    order: 1;\\n\\n    margin-left: 0.5rem;\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n}\\n\\n.summaryDiv > .summaryName,\\n.detailContainer > .detailInfo {\\n    /* this forces the correct column size, see:\\n       https://makandracards.com/makandra/66994-css-flex-and-min-width */\\n    min-width: 0;\\n}\\n\\ndetails.errorParent > summary > .summaryDiv > .summaryName {\\n    font-weight: bold;\\n}\\n\\n.summaryDiv > .summaryInput {\\n    order: 4;\\n    margin-left: auto;\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n.summaryDiv > .summaryInput.emptySummaryInput {\\n    color: var(--log-color-text-weakest);\\n}\\n\\n.detailContainer {\\n    display: flex;\\n}\\n\\n.detailContainer > .detailInfo {\\n    margin-right: auto;\\n}\\n\\n.summaryDiv > .summaryInput,\\n.detailContainer > .detailInputs {\\n    flex: 0 0 var(--right-column-width-wide);\\n    padding-left: 0.5rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n}\\n\\n.summaryDiv .timeLabel,\\n.summaryDiv .summaryFileName {\\n    order: 3;\\n    color: var(--log-color-text-weakest);\\n    margin-left: 0.5rem;\\n}\\n\\ndetails > summary:hover .timeLabel,\\ndetails > summary:hover .summaryFileName {\\n    color: var(--log-color-text-weaker);\\n}\\n\\ndetails > summary:hover .summaryInput:not(.emptySummaryInput) {\\n    color: var(--log-color-text) !important;\\n}\\n\\n/* ******************************* */\\n/* RESPONSIVE SIZING */\\n\\n@media only screen and (max-width: 840px) {\\n    .summaryDiv > .summaryInput,\\n    .detailContainer > .detailInputs,\\n    .headerInputs {\\n        display: none;\\n    }\\n}\\n\\n@media only screen and (max-width: 960px) {\\n    .headerInputs {\\n        width: var(--right-column-width-narrow) !important;\\n    }\\n\\n    .summaryDiv > .summaryInput,\\n    .detailContainer > .detailInputs {\\n        flex: 0 0 var(--right-column-width-narrow) !important;\\n    }\\n}\\n\\n/* ******************************* */\\n/* ERROR OUTPUT */\\n\\n.detailInfo {\\n    margin: 0.25rem 0;\\n    padding: 0.25rem 0;\\n    border-radius: 3px;\\n    font-size: 0.8rem;\\n}\\n\\n.errorHeader {\\n    font-weight: bold;\\n    margin-bottom: 0.35rem;\\n    overflow: hidden;\\n    text-overflow: ellipsis;\\n\\n    /* forces wrapping */\\n    white-space: initial;\\n}\\n\\n.errorDetails {\\n    font-family: var(--fixed-font-family);\\n    font-size: 0.75rem;\\n\\n    /* forces wrapping */\\n    white-space: initial;\\n\\n    color: var(--log-color-text-weaker);\\n}\\n\\n/* ******************************* */\\n/* HEADERS */\\n\\n.headers {\\n    display: flex;\\n    border-bottom: 1px solid var(--log-color-border);\\n    padding-bottom: 1rem;\\n    margin-bottom: 1rem;\\n}\\n\\n.headerSource,\\n.headerInputs {\\n    font-weight: 600;\\n    text-transform: uppercase;\\n    font-size: 0.75rem;\\n    letter-spacing: 0.3px;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n.headerInputs {\\n    margin-left: auto;\\n    width: var(--right-column-width-wide);\\n    padding-left: 0.5rem;\\n}\\n\\n.headerRunDetails {\\n    margin: 0;\\n    margin-bottom: 1.5rem;\\n    color: var(--log-color-text-weaker);\\n}\\n\\n/* ******************************* */\\n/* LABEL IS THE PASS/ERROR BADGE */\\n\\n.label {\\n    display: inline-block;\\n    margin-left: 0.5rem;\\n    color: white;\\n    font-weight: 600;\\n    font-size: 10px;\\n    border-radius: 2px;\\n    padding: 0 4px;\\n    height: 1rem;\\n    line-height: 1rem;\\n    letter-spacing: 0;\\n    display: none;\\n}\\n\\n.errorParent.leafNode .label.F,\\n.errorParent.leafNode .label.E,\\n.errorParent.leafNode .label.FAIL,\\n.errorParent.leafNode .label.ERROR {\\n    display: block;\\n    background-color: var(--log-color-error);\\n}\\n\\n/* hide labels when everything was successful */\\n/*\\n.label.PASS,\\n.label.I,\\n.label.INFO {\\n}\\n*/\\n.errorParent.leafNode .label.W,\\n.errorParent.leafNode .label.WARN {\\n    background-color: var(--log-color-warn);\\n}\\n\\n.label.NOT_RUN {\\n    background-color: var(--log-color-disabled);\\n}\\n\\n/* ******************************* */\\n/* HEADER TITLE ROW */\\n\\n.headerTitleSection {\\n    display: flex;\\n    align-items: center;\\n    margin-top: 0.3rem;\\n    margin-bottom: 0.5rem;\\n}\\n\\n.headerTitleSection h3 {\\n    margin: 0;\\n    padding: 0;\\n    font-size: 1.5rem;\\n}\\n\\n#suiteResult {\\n    font-size: 0.82rem;\\n    padding: 0.1rem 0.3rem 0.15rem 0.3rem;\\n    height: auto;\\n    margin-left: 0.75rem;\\n    display: inline-block;\\n}\\n.headerTitleSection .ERROR {\\n    background-color: var(--log-color-error);\\n}\\n.headerTitleSection .PASS {\\n    background-color: var(--log-color-success);\\n}\\n\',""]);const s=o},645:e=>{e.exports=function(e){var n=[];return n.toString=function(){return this.map((function(n){var t=e(n);return n[2]?"@media ".concat(n[2]," {").concat(t,"}"):t})).join("")},n.i=function(e,t,a){"string"==typeof e&&(e=[[null,e,""]]);var o={};if(a)for(var s=0;s<this.length;s++){var r=this[s][0];null!=r&&(o[r]=!0)}for(var i=0;i<e.length;i++){var l=[].concat(e[i]);a&&o[l[0]]||(t&&(l[2]?l[2]="".concat(t," and ").concat(l[2]):l[2]=t),n.push(l))}},n}},457:(e,n,t)=>{let a;window.setVSCodeAPI=function(e){a=e};let o={};function s(e){let n;try{n=a}catch(e){}n&&n.postMessage(e)}let r={output:void 0},i={setContents:void 0,appendContents:void 0,updateLabel:void 0};window.addEventListener("message",(e=>{let n=e.data;if(n)switch(n.type){case"response":let e=n,t=o[e.request_seq];t&&(delete o[e.request_seq],t(e));break;case"event":let a=r[n.event];a?a(n):console.log("Unhandled event: ",n);break;case"request":let s=i[n.command];s?s(n):console.log("Unhandled request: ",n)}}));let l=0;function d(){return l+=1,l}let c={filterLevel:"PASS",runIdToTreeState:{},runIdLRU:[]},u={initialContents:void 0,runId:void 0,state:void 0,onClickReference:void 0,appendedContents:[],allRunIdsToLabel:{},showTime:!0,showExpand:!0};function m(){return void 0===u.state&&(u.state=function(){let e;try{e=a}catch(e){}if(e){let n=e.getState();return n||(n=c),void 0===n.filterLevel&&(n.filterLevel="PASS"),void 0===n.runIdToTreeState&&(n.runIdToTreeState={}),void 0===!n.runIdLRU&&(n.runIdLRU=[]),n}return c}()),u}function h(e){return document.getElementById(e)}function p(e){return h(e)}function f(e){return h(e)}function g(e){const n=document.createElement("ul");return n.setAttribute("data-tree-id",e),n}function v(){return document.createElement("span")}function E(){return document.createElement("button")}function y(){return document.createElement("div")}function C(e){return e.getAttribute("data-tree-id")}function b(e,n=undefined){if(void 0===n)return"1"===e.getAttribute("data-hidden");n?e.setAttribute("data-hidden","1"):e.removeAttribute("data-hidden")}function w(e){var n=document.createElement("template");return e=e.trim(),n.innerHTML=e,n.content.firstChild}function S(e,n){for(let t of n.childNodes)if(t instanceof HTMLDetailsElement){for(let n of t.childNodes)n instanceof HTMLUListElement&&L(e,n);t.open?e.openNodes[C(n)]="open":delete e.openNodes[C(n)]}}function L(e,n){for(let t of n.childNodes)t instanceof HTMLLIElement&&S(e,t)}const x=((e,n)=>{let t;return function(...e){clearTimeout(t),t=setTimeout((()=>{clearTimeout(t),(()=>{T()})(...e)}),500)}})();function T(){const e=m();!function(e,n){const t=p("mainTree");let a={openNodes:{}};if(void 0===e.runIdLRU&&(e.runIdLRU=[]),void 0===e.runIdToTreeState)e.runIdToTreeState={};else{const t=e.runIdToTreeState[n];t&&(a=t)}for(let e of t.childNodes)e instanceof HTMLUListElement&&L(a,e);e.runIdToTreeState[n]=a;const o=e.runIdLRU.indexOf(n);for(o>-1&&e.runIdLRU.splice(o,1),e.runIdLRU.push(n);e.runIdLRU.length>15;){const n=e.runIdLRU.splice(0,1);delete e.runIdToTreeState[n[0]]}}(e.state,e.runId),function(e){let n;try{n=a}catch(e){}n?n.setState(e):c=e}(e.state)}function N(e,n){if(void 0===e)return;const t=f("selectedRun"),a=new Map;for(let o of t.childNodes)if(o instanceof HTMLOptionElement){const t=o,s=t.value,r=e[s];if(void 0===r)o.remove();else{t.text!==r&&(t.text=r),a.set(s,r);const e=n==s;t.selected=e}}for(const o of Object.keys(e)){if(void 0===o)continue;const s=n==o;if(!a.has(o)){const n=document.createElement("option"),r=e[o];n.value=o,t.appendChild(n),n.selected=s,n.text=r,a.set(o,r)}}}Math.pow(10,8);var I=36e5;function M(e,n){var t;!function(e,n){if(n.length<1)throw new TypeError("1 argument required, but only "+n.length+" present")}(0,arguments);var a=function(e){if(null===e||!0===e||!1===e)return NaN;var n=Number(e);return isNaN(n)?n:n<0?Math.ceil(n):Math.floor(n)}(null!==(t=null==n?void 0:n.additionalDigits)&&void 0!==t?t:2);if(2!==a&&1!==a&&0!==a)throw new RangeError("additionalDigits must be 0, 1 or 2");if("string"!=typeof e&&"[object String]"!==Object.prototype.toString.call(e))return new Date(NaN);var o,s=function(e){var n,t={},a=e.split(k.dateTimeDelimiter);if(a.length>2)return t;if(/:/.test(a[0])?n=a[0]:(t.date=a[0],n=a[1],k.timeZoneDelimiter.test(t.date)&&(t.date=e.split(k.timeZoneDelimiter)[0],n=e.substr(t.date.length,e.length))),n){var o=k.timezone.exec(n);o?(t.time=n.replace(o[1],""),t.timezone=o[1]):t.time=n}return t}(e);if(s.date){var r=function(e,n){var t=new RegExp("^(?:(\\\\d{4}|[+-]\\\\d{"+(4+n)+"})|(\\\\d{2}|[+-]\\\\d{"+(2+n)+"})$)"),a=e.match(t);if(!a)return{year:NaN,restDateString:""};var o=a[1]?parseInt(a[1]):null,s=a[2]?parseInt(a[2]):null;return{year:null===s?o:100*s,restDateString:e.slice((a[1]||a[2]).length)}}(s.date,a);o=function(e,n){if(null===n)return new Date(NaN);var t=e.match(R);if(!t)return new Date(NaN);var a=!!t[4],o=D(t[1]),s=D(t[2])-1,r=D(t[3]),i=D(t[4]),l=D(t[5])-1;if(a)return function(e,n,t){return n>=1&&n<=53&&t>=0&&t<=6}(0,i,l)?function(e,n,t){var a=new Date(0);a.setUTCFullYear(e,0,4);var o=7*(n-1)+t+1-(a.getUTCDay()||7);return a.setUTCDate(a.getUTCDate()+o),a}(n,i,l):new Date(NaN);var d=new Date(0);return function(e,n,t){return n>=0&&n<=11&&t>=1&&t<=(F[n]||(O(e)?29:28))}(n,s,r)&&function(e,n){return n>=1&&n<=(O(e)?366:365)}(n,o)?(d.setUTCFullYear(n,s,Math.max(o,r)),d):new Date(NaN)}(r.restDateString,r.year)}if(!o||isNaN(o.getTime()))return new Date(NaN);var i,l=o.getTime(),d=0;if(s.time&&(d=function(e){var n=e.match(A);if(!n)return NaN;var t=H(n[1]),a=H(n[2]),o=H(n[3]);return function(e,n,t){return 24===e?0===n&&0===t:t>=0&&t<60&&n>=0&&n<60&&e>=0&&e<25}(t,a,o)?t*I+6e4*a+1e3*o:NaN}(s.time),isNaN(d)))return new Date(NaN);if(!s.timezone){var c=new Date(l+d),u=new Date(0);return u.setFullYear(c.getUTCFullYear(),c.getUTCMonth(),c.getUTCDate()),u.setHours(c.getUTCHours(),c.getUTCMinutes(),c.getUTCSeconds(),c.getUTCMilliseconds()),u}return i=function(e){if("Z"===e)return 0;var n=e.match(_);if(!n)return 0;var t="+"===n[1]?-1:1,a=parseInt(n[2]),o=n[3]&&parseInt(n[3])||0;return function(e,n){return n>=0&&n<=59}(0,o)?t*(a*I+6e4*o):NaN}(s.timezone),isNaN(i)?new Date(NaN):new Date(l+d+i)}var k={dateTimeDelimiter:/[T ]/,timeZoneDelimiter:/[Z ]/i,timezone:/([Z+-].*)$/},R=/^-?(?:(\\d{3})|(\\d{2})(?:-?(\\d{2}))?|W(\\d{2})(?:-?(\\d{1}))?|)$/,A=/^(\\d{2}(?:[.,]\\d*)?)(?::?(\\d{2}(?:[.,]\\d*)?))?(?::?(\\d{2}(?:[.,]\\d*)?))?$/,_=/^([+-])(\\d{2})(?::?(\\d{2}))?$/;function D(e){return e?parseInt(e):1}function H(e){return e&&parseFloat(e.replace(",","."))||0}var F=[31,null,31,30,31,30,31,31,30,31,30,31];function O(e){return e%400==0||e%4==0&&e%100!=0}function P(e,n){const t=e.memo[n];return void 0===t?`<ref not found: ${n}>`:t}function U(e,n){return parseFloat(n)}function z(e,n){return parseInt(n)}function B(e,n){return n}function V(e){const n=[],t=new Map;for(let a of e.split(",")){a=a.trim();let e="oid";if(-1!=a.indexOf(":")&&([a,e]=a.split(":",2)),n.push(a),"oid"===e)t.set(a,P);else if("int"===e)t.set(a,z);else if("float"===e)t.set(a,U);else{if("str"!==e)throw new Error("Unexpected: "+e);t.set(a,B)}}return function(e,a){const o=a.split("|",n.length),s={};for(let a=0;a<o.length;a++){const r=o[a],i=n[a];s[i]=t.get(i)(e,r)}return s}}const j=V("name:oid, time_delta_in_seconds:float"),$=V("status:oid, time_delta_in_seconds:float"),q=V("name:oid, libname:oid, source:oid, lineno:int, time_delta_in_seconds:float"),W=V("status:oid, message:oid, time_delta_in_seconds:float"),Z=V("name:oid, libname:oid, type:oid, doc:oid, source:oid, lineno:int, time_delta_in_seconds:float"),J=V("status:oid, time_delta_in_seconds:float"),Y=V("level:str, message:oid, source:oid, lineno:int, time_delta_in_seconds:float"),G={V:function(e,n){return{message:n}},ID:V("part:int, id:str"),I:function(e,n){return JSON.parse(n)},T:function(e,n){return{time:M(n).toString()}},M:function(e,n){var t,a;const o=Q(n,":");if(o){[t,a]=o;try{a=JSON.parse(a)}catch(e){return console.log("Error parsing json: "+a),console.log(e),null}e.memo[t]=a}return null},SR:j,RR:j,ER:$,ST:q,RT:q,ET:W,SE:Z,RE:Z,EE:J,EA:V("name:oid, type:oid, value:oid"),AS:V("source:oid, lineno:int, target:oid, type:oid, value:oid, time_delta_in_seconds:float"),L:Y,LH:Y,TG:V("tag:oid"),S:V("start_time_delta:float"),STB:V("message:oid, time_delta_in_seconds:float"),RTB:V("message:oid, time_delta_in_seconds:float"),TBE:V("source:oid, lineno:int, method:oid, line_content:oid"),TBV:V("name:oid, type:oid, value:oid"),ETB:V("time_delta_in_seconds:float")};class K{constructor(){this.memo={}}decode_message_type(e,n){return(0,G[e])(this,n)}}function Q(e,n){const t=e.indexOf(n);if(t>0)return[e.substring(0,t),e.substring(t+1)]}function*X(e,n){var t,a,o;for(let s of e.split(/\\r?\\n/))if(s=s.trim(),s)try{const e=Q(s," ");if(e&&([o,a]=e,t=n.decode_message_type(o,a))){const e={message_type:o,decoded:t};yield e}}catch(e){console.log("Unable to decode message: "+s),console.log(e)}}function ee(e,n){const t=document.createElement("span");t.textContent=n,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}function ne(e,n){switch(e.state.filterLevel){case"FAIL":return n>=2;case"WARN":return n>=1;case"PASS":return n>=0;case"NOT RUN":return!0}}function te(e){switch(e){case"FAIL":case"ERROR":return 2;case"WARN":return 1;case"NOT RUN":case"NOT_RUN":return-1;default:return 0}}class ae{constructor(e){this.stack=[],this.exceptionMsg=e}pushEntry(e,n,t,a){const o=new Map;this.stack.push({source:e,lineno:n,method:t,lineContent:a,variables:o})}pushVar(e,n,t){this.stack.at(-1).variables.set(e,[n,t])}}class oe{constructor(){this.totalTests=0,this.totalFailures=0}clear(){this.totalTests=0,this.totalFailures=0,this.updateSummary()}onTestEndUpdateSummary(e){const n=e.decoded.status;this.totalTests+=1,"FAIL"!=n&&"ERROR"!=n||(this.totalFailures+=1),this.updateSummary()}updateSummary(){const e=p("summary");if(!e)return;const n=(""+this.totalTests).padStart(4),t=(""+this.totalFailures).padStart(4);if(e.textContent=`Total: ${n} Failures: ${t}`,0==this.totalFailures&&0==this.totalTests){const e=p("summary");e.classList.add("NOT_RUN"),e.classList.remove("PASS"),e.classList.remove("FAIL")}else if(1==this.totalFailures){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("PASS"),e.classList.add("FAIL")}else if(0==this.totalFailures&&1==this.totalTests){const e=p("summary");e.classList.remove("NOT_RUN"),e.classList.remove("FAIL")}}}function se(e,n){const t=function(e){const n=document.createElement("li");return n.setAttribute("data-tree-id",e),n}(n),a=document.createElement("details");e&&(a.open=e),a.classList.add("NO_CHILDREN"),t.appendChild(a);const o=y();o.classList.add("detailContainer"),a.appendChild(o);const s=document.createElement("summary"),r=y();r.classList.add("summaryDiv"),s.appendChild(r);const i=v();i.className="summaryName",i.textContent="[summaryName]",r.appendChild(i);const l=v();return l.className="summaryInput emptySummaryInput",l.textContent="",r.appendChild(l),a.appendChild(s),{li:t,details:a,summary:s,summaryDiv:r,summaryName:i,summaryInput:l,detailContainer:o}}function re(e,n,t,a,o,s,r,i,l,d){const c=e.state.runIdToTreeState[e.runId],u="li_"+d;if(c){const e=c.openNodes;e&&(s=e[u])}const m=se(s,u),h=m.li,p=m.details,f=m.detailContainer,v=m.summary,E=m.summaryDiv,y=m.summaryName,C=m.summaryInput;if("LH"===o.message_type){y.textContent="";const e=w(t);y.appendChild(e)}else y.textContent=t;a&&(y.title=a),e.onClickReference&&(y.classList.add("span_link"),y.onclick=n=>{const t=[];let a=l.parent;for(;void 0!==a&&void 0!==a.message;)t.push(a.message),a=a.parent;n.preventDefault(),e.onClickReference({source:r,lineno:i,message:o.decoded,messageType:o.message_type,scope:t})});const b=g("ul_"+d);p.appendChild(b);const S={ul:b,li:h,details:p,detailContainer:f,summary:v,summaryName:y,summaryInput:C,source:r,lineno:i,appendContentChild:void 0,decodedMessage:o,maxLevelFoundInHierarchy:-1,summaryDiv:E};return S.appendContentChild=ue.bind(S),n.appendContentChild(S),S}let ie,le;function*de(e){for(let n of e.childNodes)if(n instanceof HTMLDetailsElement){for(let e of n.childNodes)if(e instanceof HTMLUListElement)for(let n of ce(e))yield n;yield n}}function*ce(e){for(let n of e.childNodes)if(n instanceof HTMLLIElement)for(let e of de(n))yield e}function ue(e){const n=this;n.ul.appendChild(e.li),n.details.classList.contains("NO_CHILDREN")&&(n.details.classList.remove("NO_CHILDREN"),n.details.addEventListener("toggle",(function(){x()})),m().showExpand&&n.summary.addEventListener("mouseover",(e=>{!function(e){if(void 0===ie){ie=y(),ie.classList.add("toolbarContainer");const e=E();e.appendChild(w(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path d="M7 12V7H6v5h1z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),e.onclick=()=>{!function(){if(void 0!==le){le.details.open=!0;for(let e of ce(le.ul))e.classList.contains("NO_CHILDREN")||(e.open=!0)}}()},e.classList.add("toolbarButton");const n=E();return n.appendChild(w(\'<svg xmlns="http://www.w3.org/2000/svg" width="16px" height="16px" preserveAspectRatio="xMidYMid meet" viewBox="0 0 16 16"><g fill="currentColor"><path d="M9 9H4v1h5V9z"/><path fill-rule="evenodd" d="m5 3l1-1h7l1 1v7l-1 1h-2v2l-1 1H3l-1-1V6l1-1h2V3zm1 2h4l1 1v4h2V3H6v2zm4 1H3v7h7V6z" clip-rule="evenodd"/></g></svg>\')),n.classList.add("toolbarButton"),n.onclick=()=>{!function(){if(void 0!==le){le.details.open=!1;for(let e of ce(le.ul))e.open=!1}}()},ie.appendChild(n),void ie.appendChild(e)}le=e,e.summaryDiv.appendChild(ie)}(n)})))}var me=(e,n,t)=>new Promise(((a,o)=>{var s=e=>{try{i(t.next(e))}catch(e){o(e)}},r=e=>{try{i(t.throw(e))}catch(e){o(e)}},i=e=>e.done?a(e.value):Promise.resolve(e.value).then(s,r);i((t=t.apply(e,n)).next())}));let he=0,pe=-1;class fe{constructor(){this.stack=[]}handle(e){let n;switch(e.message_type){case"STB":return void this.stack.push(new ae(e.decoded.message));case"TBE":return n=this.stack.at(-1),void n.pushEntry(e.decoded.source,e.decoded.lineno,e.decoded.method,e.decoded.line_content);case"TBV":return;case"ETB":return n=this.stack.pop(),n.stack.reverse(),n}}}class ge{constructor(){this.stack=[],this.messageNode={parent:void 0,message:void 0},this.id=0,this.finishedAddingInitialContents=!1,this.appendedMessagesIndex=-1,this.decoder=new K,this.seenSuiteTaskOrElement=!1,this.tbHandler=new fe,this.suiteErrored=!1,this.opts=m(),this.runId=this.opts.runId,this.summaryBuilder=new oe,this.lease=(he+=1,pe=he,he),this.resetState()}resetState(){this.seenSuiteTaskOrElement=!1}isCurrentTreeBuilder(){return this.lease===pe&&this.runId==this.opts.runId}clearAndInitializeTree(){this.summaryBuilder.clear(),this.resetState();const e=f("filterLevel");e&&(e.value=this.opts.state.filterLevel);const n=p("mainTree");n.replaceChildren();const t=g("ul_root");t.classList.add("tree"),n.appendChild(t),this.parent={ul:void 0,li:void 0,details:void 0,detailContainer:void 0,summary:void 0,summaryName:void 0,summaryInput:void 0,source:void 0,lineno:void 0,decodedMessage:void 0,appendContentChild:function(e){t.appendChild(e.li)},maxLevelFoundInHierarchy:-1,summaryDiv:void 0},this.stack.push(this.parent)}addInitialContents(){return me(this,null,(function*(){for(const e of X(this.opts.initialContents,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}this.finishedAddingInitialContents=!0,yield this.onAppendedContents()}))}onAppendedContents(){return me(this,null,(function*(){if(!this.finishedAddingInitialContents)return;if(!this.isCurrentTreeBuilder())return;const e=m();for(;this.appendedMessagesIndex+1<e.appendedContents.length;){this.appendedMessagesIndex+=1;const n=e.appendedContents[this.appendedMessagesIndex];for(const e of X(n,this.decoder)){if(!this.isCurrentTreeBuilder())return;yield this.addOneMessage(e)}}}))}addOneMessage(e){return me(this,null,(function*(){if(this.isCurrentTreeBuilder())try{this.addOneMessageSync(e)}catch(n){console.log("Error: handling message: "+JSON.stringify(e)+": "+n+" - "+JSON.stringify(n))}}))}addOneMessageSync(e){var n,t;let a,o,s=e.message_type;switch(s){case"SR":case"ST":case"SE":case"STB":this.seenSuiteTaskOrElement=!0;break;case"RR":if(this.seenSuiteTaskOrElement)return;s="SR";break;case"RT":if(this.seenSuiteTaskOrElement)return;s="ST";break;case"RE":if(this.seenSuiteTaskOrElement)return;s="SE";break;case"RTB":if(this.seenSuiteTaskOrElement)return;s="STB"}switch(this.id+=1,s){case"SR":this.messageNode={parent:this.messageNode,message:e};for(const n of document.querySelectorAll(".suiteHeader"))n.textContent=e.decoded.name;break;case"AS":o=re(this.opts,this.parent,`${e.decoded.target} = `,`Assign to name: ${e.decoded.target}\\nAn object of type: ${e.decoded.type}\\nWith representation:\\n${e.decoded.value}`,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),function(e,n){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${n}`,e.summaryInput.classList.remove("emptySummaryInput")):e.summaryInput.textContent+=`, ${n}`}(o,e.decoded.value),this.addAssignCssClass(o);break;case"ST":this.messageNode={parent:this.messageNode,message:e},this.parent=re(this.opts,this.parent,`${e.decoded.libname}.${e.decoded.name}`,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"SE":this.messageNode={parent:this.messageNode,message:e},this.parent=re(this.opts,this.parent,e.decoded.name,e.decoded.libname,e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString()),this.stack.push(this.parent);break;case"ER":this.messageNode=this.messageNode.parent;{const n=p("suiteResult");n.style.display="block",this.suiteErrored?(n.classList.add("ERROR"),n.textContent="Run Failed"):(n.classList.add("PASS"),n.textContent="Run Passed");const t=p("suiteRunStart");t&&(t.textContent+=` - Finished in: ${e.decoded.time_delta_in_seconds.toFixed(2)}s.`)}break;case"ET":this.messageNode=this.messageNode.parent;const s=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(s,this.parent,e),this.onEndSetStatusOrRemove(this.opts,s,e.decoded,this.parent,!1),this.summaryBuilder.onTestEndUpdateSummary(e),a=this.addDetailsCSSClasses(e.decoded.status,s),a&&(this.suiteErrored=!0,s.details.open=!0);break;case"EE":this.messageNode=this.messageNode.parent;let r=this.parent;this.stack.pop(),this.parent=this.stack.at(-1),this.onEndUpdateMaxLevelFoundInHierarchyFromStatus(r,this.parent,e),this.onEndSetStatusOrRemove(this.opts,r,e.decoded,this.parent,!0),a=this.addDetailsCSSClasses(e.decoded.status,r),a&&(r.details.open=!0);break;case"S":const i=e.decoded.start_time_delta;(null==(t=null==(n=this.parent)?void 0:n.decodedMessage)?void 0:t.decoded)&&(this.parent.decodedMessage.decoded.time_delta_in_seconds=i);break;case"EA":o=this.stack.at(-1),function(e,n,t,a){e.summaryInput.classList.contains("emptySummaryInput")?(e.summaryInput.textContent=`${n} (${t}) = ${a}`,e.summaryInput.classList.remove("emptySummaryInput")):e.summaryInput.textContent+=`, ${n} (${t}) = ${a}`}(o,e.decoded.name,e.decoded.type,e.decoded.value);break;case"L":case"LH":const l=e.decoded.level,d=function(e){switch(e){case"E":case"F":return 2;case"W":return 1;default:return 0}}(l);if(d>this.parent.maxLevelFoundInHierarchy&&(this.parent.maxLevelFoundInHierarchy=d),ne(this.opts,d)){const n=re(this.opts,this.parent,e.decoded.message,"",e,!1,e.decoded.source,e.decoded.lineno,this.messageNode,this.id.toString());n.maxLevelFoundInHierarchy=d,function(e,n){const t=document.createElement("span");t.textContent=`LOG ${function(e){switch(e){case"E":return"ERROR";case"F":return"FAIL";case"W":return"WARN";case"I":return"INFO";default:return e}}(n)}`,t.classList.add("label"),t.classList.add(n.replace(" ","_")),e.summaryDiv.insertBefore(t,e.summaryDiv.firstChild)}(n,l),this.addDetailsCSSClasses(d,n)}break;case"STB":case"TBE":case"TBV":case"ETB":const c=this.tbHandler.handle(e);if(c&&c.stack.length>0){const n=c.stack[0];o=re(this.opts,this.parent,c.exceptionMsg,"",e,!1,n.source,n.lineno,this.messageNode,this.id.toString()),this.addExceptionCssClass(o)}break;case"T":const u=p("suiteRunStart");u&&(u.textContent=e.decoded.time)}}addAssignCssClass(e){e.details.classList.add("variableParent"),e.details.classList.add("leafNode")}addExceptionCssClass(e){e.details.classList.add("exceptionParent"),e.details.classList.add("leafNode")}addDetailsCSSClasses(e,n){let t,a=!1;return t="string"==typeof e?te(e):e,t>=2?(n.details.classList.add("errorParent"),a=!0):1==t?n.details.classList.add("warnParent"):n.details.classList.add("passParent"),n.details.classList.contains("parentNode")||n.details.classList.contains("leafNode")||(0===n.ul.children.length?n.details.classList.add("leafNode"):n.details.classList.add("parentNode")),a}onEndUpdateMaxLevelFoundInHierarchyFromStatus(e,n,t){const a=te(t.decoded.status);a>e.maxLevelFoundInHierarchy&&(e.maxLevelFoundInHierarchy=a),e.maxLevelFoundInHierarchy>n.maxLevelFoundInHierarchy&&(n.maxLevelFoundInHierarchy=e.maxLevelFoundInHierarchy)}onEndSetStatusOrRemove(e,n,t,a,o){const s=t.status;if(ne(e,n.maxLevelFoundInHierarchy)){if(o&&n.maxLevelFoundInHierarchy<=0){const e=50;if(a.ul.childElementCount>e){const e=n.summaryName.textContent;if(e&&e.toLowerCase().includes("iteration")){const e=n.li.previousSibling,t=C(n.li);if(n.li.remove(),b(e))e.getElementsByClassName("FINAL_SPAN")[0].textContent=n.summaryName.textContent;else{const e=se(!1,t);e.summaryName.textContent=n.summaryName.textContent,e.summary.classList.add("HIDDEN");const o=v();o.setAttribute("role","button"),o.textContent="...",o.classList.add("label"),o.classList.add("HIDDEN"),o.classList.add("inline"),e.summaryDiv.appendChild(o);const s=v();s.setAttribute("role","button"),s.classList.add("FINAL_SPAN"),e.summaryDiv.appendChild(s),ee(e,"HIDDEN"),b(e.li,!0),a.ul.appendChild(e.li)}return}}}if(n.summary,ee(n,s),null!=n.source&&n.source.length>0){const e=function(e){let n=e,t=Math.max(e.lastIndexOf("/"),e.lastIndexOf("\\\\"));return t>0&&(n=e.substring(t+1)),n}(n.source),t=document.createElement("span");t.textContent=e,t.classList.add("summaryFileName"),t.title=n.source,n.summaryDiv.appendChild(t)}if(this.opts.showTime){const e=n.decodedMessage.decoded.time_delta_in_seconds;void 0!==e&&e>=0&&function(e,n){const t=document.createElement("span");t.textContent=` (${n.toFixed(2)}s)`,t.classList.add("timeLabel"),e.summaryDiv.appendChild(t)}(n,t.time_delta_in_seconds-e)}}else n.li.remove()}}var ve=(e,n,t)=>new Promise(((a,o)=>{var s=e=>{try{i(t.next(e))}catch(e){o(e)}},r=e=>{try{i(t.throw(e))}catch(e){o(e)}},i=e=>e.done?a(e.value):Promise.resolve(e.value).then(s,r);i((t=t.apply(e,n)).next())}));let Ee;function ye(){return ve(this,null,(function*(){Ee=new ge,Ee.clearAndInitializeTree(),yield Ee.addInitialContents()}))}function Ce(e){let n={type:"event",seq:d(),event:"onClickReference"};n.data=e,s(n)}function be(e){T();const n=m();n.runId=e.runId,n.initialContents=e.initialContents,void 0!==a&&(n.onClickReference=Ce),n.appendedContents=[],n.allRunIdsToLabel=e.allRunIdsToLabel,N(n.allRunIdsToLabel,n.runId),ye()}t(739),i.setContents=be,i.appendContents=function(e){const n=m();n.runId===e.runId&&(n.appendedContents.push(e.appendContents),void 0!==Ee&&Ee.onAppendedContents())},i.updateLabel=function(e){const n=m();n.allRunIdsToLabel[e.runId]=e.label,N(n.allRunIdsToLabel,n.runId)},window.onChangedRun=function(){const e=f("selectedRun").value;let n={type:"event",seq:d(),event:"onSetCurrentRunId"};n.data={runId:e},s(n)},window.onChangedFilterLevel=function(){!function(e){const n=m();n.state.filterLevel!==e&&(n.state.filterLevel=e,T(),ye())}(f("filterLevel").value)},window.setContents=be,window.setShowTime=function(e){m().showTime=e},window.setShowExpand=function(e){m().showExpand=e},window.getSampleContents=function(){return JSON.parse(\'"V 1\\\\nI \\\\"sys.platform=win32\\\\"\\\\nI \\\\"python=3.7.6 (default, Jan  8 2020, 20:23:39) [MSC v.1916 64 bit (AMD64)]\\\\"\\\\nI \\\\"robot=5.1a3.dev1\\\\"\\\\nT 2022-10-19T09:48:34.018\\\\nM a:\\\\"Robot1\\\\"\\\\nM b:\\\\"s1\\\\"\\\\nM c:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\robot1.robot\\\\"\\\\nSR a|b|c|0.035\\\\nM d:\\\\"Simple Task\\\\"\\\\nM e:\\\\"s1-t1\\\\"\\\\nST d|e|16|0.036\\\\nM f:\\\\"First keyword\\\\"\\\\nM g:\\\\"\\\\"\\\\nM h:\\\\"KEYWORD\\\\"\\\\nSE f|g|h|g|c|17|0.036\\\\nM i:\\\\"No Operation\\\\"\\\\nM j:\\\\"BuiltIn\\\\"\\\\nM k:\\\\"Does absolutely nothing.\\\\"\\\\nSE i|j|h|k|c|8|0.037\\\\nM l:\\\\"PASS\\\\"\\\\nEE l|0.037\\\\nM m:\\\\"Log\\\\"\\\\nM n:\\\\"Logs the given message with the given level.\\\\"\\\\nSE m|j|h|n|c|10|0.037\\\\nM o:\\\\"Some warning message\\\\"\\\\nEA o\\\\nM p:\\\\"level=WARN\\\\"\\\\nEA p\\\\nEE l|0.046\\\\nM q:\\\\"Another keyword\\\\"\\\\nM r:\\\\"another\\\\"\\\\nSE q|r|h|g|c|11|0.047\\\\nM s:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\another.robot\\\\"\\\\nSE i|j|h|k|s|3|0.047\\\\nEE l|0.047\\\\nEE l|0.047\\\\nM t:\\\\"Another in sub keyword\\\\"\\\\nM u:\\\\"another_sub\\\\"\\\\nSE t|u|h|g|c|12|0.047\\\\nM v:\\\\"C:\\\\\\\\\\\\\\\\Users\\\\\\\\\\\\\\\\fabio\\\\\\\\\\\\\\\\AppData\\\\\\\\\\\\\\\\Local\\\\\\\\\\\\\\\\Temp\\\\\\\\\\\\\\\\pytest-of-fabio\\\\\\\\\\\\\\\\pytest-421\\\\\\\\\\\\\\\\test_robot_out_stream0\\\\\\\\\\\\\\\\test_robot_out_stream\\\\\\\\\\\\\\\\sub\\\\\\\\\\\\\\\\another_sub.robot\\\\"\\\\nSE i|j|h|k|v|6|0.048\\\\nEE l|0.048\\\\nSE m|j|h|n|v|7|0.048\\\\nM w:\\\\"Some error message\\\\"\\\\nEA w\\\\nM x:\\\\"level=ERROR\\\\"\\\\nEA x\\\\nEE l|0.049\\\\nEE l|0.049\\\\nEE l|0.049\\\\nSE m|j|h|n|c|18|0.049\\\\nM y:\\\\"Some <data &encode <\\/script>\\\\"\\\\nEA y\\\\nEE l|0.049\\\\nM z:\\\\"Create Dictionary\\\\"\\\\nM A:\\\\"Creates and returns a dictionary based on the given ``items``.\\\\"\\\\nSE z|j|h|A|c|19|0.049\\\\nM B:\\\\"a=1\\\\"\\\\nEA B\\\\nM C:\\\\"b=1\\\\"\\\\nEA C\\\\nEE l|0.05\\\\nSE m|j|h|n|c|20|0.05\\\\nM D:\\\\"${dct}\\\\"\\\\nEA D\\\\nEE l|0.051\\\\nET l|g|0.051\\\\nM E:\\\\"Check 1\\\\"\\\\nM F:\\\\"s1-t2\\\\"\\\\nST E|F|22|0.051\\\\nSE f|g|h|g|c|23|0.051\\\\nSE i|j|h|k|c|8|0.052\\\\nEE l|0.052\\\\nSE m|j|h|n|c|10|0.052\\\\nEA o\\\\nEA p\\\\nEE l|0.052\\\\nSE q|r|h|g|c|11|0.053\\\\nSE i|j|h|k|s|3|0.053\\\\nEE l|0.053\\\\nEE l|0.053\\\\nSE t|u|h|g|c|12|0.053\\\\nSE i|j|h|k|v|6|0.054\\\\nEE l|0.054\\\\nSE m|j|h|n|v|7|0.054\\\\nEA w\\\\nEA x\\\\nEE l|0.054\\\\nEE l|0.055\\\\nEE l|0.055\\\\nM G:\\\\"${counter} IN RANGE [ 0 | 3 ]\\\\"\\\\nM H:\\\\"FOR\\\\"\\\\nSE G|g|H|g|c|25|0.055\\\\nM I:\\\\"${counter} = 0\\\\"\\\\nM J:\\\\"ITERATION\\\\"\\\\nSE I|g|J|g|c|25|0.055\\\\nM K:\\\\"${counter} == 2\\\\"\\\\nM L:\\\\"IF\\\\"\\\\nSE K|g|L|g|c|26|0.055\\\\nM M:\\\\"Fail\\\\"\\\\nM N:\\\\"Fails the test with the given message and optionally alters its tags.\\\\"\\\\nSE M|j|h|N|c|27|0.056\\\\nM O:\\\\"Failed execution for some reason...\\\\"\\\\nEA O\\\\nM P:\\\\"NOT RUN\\\\"\\\\nEE P|0.056\\\\nEE P|0.056\\\\nSE m|j|h|n|c|29|0.056\\\\nM Q:\\\\"${counter}\\\\"\\\\nEA Q\\\\nEE l|0.056\\\\nEE l|0.057\\\\nM R:\\\\"${counter} = 1\\\\"\\\\nSE R|g|J|g|c|25|0.057\\\\nSE K|g|L|g|c|26|0.057\\\\nSE M|j|h|N|c|27|0.057\\\\nEA O\\\\nEE P|0.057\\\\nEE P|0.057\\\\nSE m|j|h|n|c|29|0.058\\\\nEA Q\\\\nEE l|0.058\\\\nEE l|0.058\\\\nM S:\\\\"${counter} = 2\\\\"\\\\nSE S|g|J|g|c|25|0.058\\\\nSE K|g|L|g|c|26|0.058\\\\nSE M|j|h|N|c|27|0.059\\\\nEA O\\\\nM T:\\\\"FAIL\\\\"\\\\nEE T|0.059\\\\nEE T|0.059\\\\nSE m|j|h|n|c|29|0.059\\\\nEA Q\\\\nEE P|0.059\\\\nEE T|0.06\\\\nEE T|0.06\\\\nET T|O|0.06\\\\nM U:\\\\"Check 2\\\\"\\\\nM V:\\\\"s1-t3\\\\"\\\\nST U|V|32|0.06\\\\nM W:\\\\"Set Variable\\\\"\\\\nM X:\\\\"Returns the given values which can then be assigned to a variables.\\\\"\\\\nSE W|j|h|X|c|33|0.061\\\\nM Y:\\\\"3\\\\"\\\\nEA Y\\\\nEE l|0.061\\\\nM Z:\\\\"${counter} <= 2\\\\"\\\\nM 0:\\\\"WHILE\\\\"\\\\nSE Z|g|0|g|c|34|0.061\\\\nSE g|g|J|g|c|34|0.062\\\\nM 1:\\\\"Evaluate\\\\"\\\\nM 2:\\\\"Evaluates the given expression in Python and returns the result.\\\\"\\\\nSE 1|j|h|2|c|35|0.062\\\\nM 4:\\\\"$counter-1\\\\"\\\\nEA 4\\\\nEE P|0.062\\\\nSE m|j|h|n|c|36|0.062\\\\nM 5:\\\\"Current counter: ${counter}\\\\"\\\\nEA 5\\\\nEA p\\\\nEE P|0.062\\\\nEE P|0.062\\\\nEE P|0.063\\\\nET l|g|0.063\\\\nM 6:\\\\"Check 3\\\\"\\\\nM 7:\\\\"s1-t4\\\\"\\\\nST 6|7|39|0.064\\\\nM 8:\\\\"TRY\\\\"\\\\nSE g|g|8|g|c|40|0.064\\\\nSE i|j|h|k|c|41|0.064\\\\nEE l|0.064\\\\nEE l|0.064\\\\nM 9:\\\\"message\\\\"\\\\nM aa:\\\\"EXCEPT\\\\"\\\\nSE 9|g|aa|g|c|42|0.064\\\\nSE i|j|h|k|c|43|0.065\\\\nEE P|0.065\\\\nEE P|0.065\\\\nM ab:\\\\"FINALLY\\\\"\\\\nSE g|g|ab|g|c|44|0.065\\\\nSE i|j|h|k|c|45|0.065\\\\nEE l|0.065\\\\nEE l|0.065\\\\nET l|g|0.066\\\\nER T|0.067\\\\n"\')}},739:(e,n,t)=>{var a=t(379),o=t.n(a),s=t(599),r={injectType:"singletonStyleTag",insert:"head",singleton:!0};o()(s.Z,r),s.Z.locals},379:(e,n,t)=>{var a,o=function(){var e={};return function(n){if(void 0===e[n]){var t=document.querySelector(n);if(window.HTMLIFrameElement&&t instanceof window.HTMLIFrameElement)try{t=t.contentDocument.head}catch(e){t=null}e[n]=t}return e[n]}}(),s=[];function r(e){for(var n=-1,t=0;t<s.length;t++)if(s[t].identifier===e){n=t;break}return n}function i(e,n){for(var t={},a=[],o=0;o<e.length;o++){var i=e[o],l=n.base?i[0]+n.base:i[0],d=t[l]||0,c="".concat(l," ").concat(d);t[l]=d+1;var u=r(c),m={css:i[1],media:i[2],sourceMap:i[3]};-1!==u?(s[u].references++,s[u].updater(m)):s.push({identifier:c,updater:f(m,n),references:1}),a.push(c)}return a}function l(e){var n=document.createElement("style"),a=e.attributes||{};if(void 0===a.nonce){var s=t.nc;s&&(a.nonce=s)}if(Object.keys(a).forEach((function(e){n.setAttribute(e,a[e])})),"function"==typeof e.insert)e.insert(n);else{var r=o(e.insert||"head");if(!r)throw new Error("Couldn\'t find a style target. This probably means that the value for the \'insert\' parameter is invalid.");r.appendChild(n)}return n}var d,c=(d=[],function(e,n){return d[e]=n,d.filter(Boolean).join("\\n")});function u(e,n,t,a){var o=t?"":a.media?"@media ".concat(a.media," {").concat(a.css,"}"):a.css;if(e.styleSheet)e.styleSheet.cssText=c(n,o);else{var s=document.createTextNode(o),r=e.childNodes;r[n]&&e.removeChild(r[n]),r.length?e.insertBefore(s,r[n]):e.appendChild(s)}}function m(e,n,t){var a=t.css,o=t.media,s=t.sourceMap;if(o?e.setAttribute("media",o):e.removeAttribute("media"),s&&"undefined"!=typeof btoa&&(a+="\\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(s))))," */")),e.styleSheet)e.styleSheet.cssText=a;else{for(;e.firstChild;)e.removeChild(e.firstChild);e.appendChild(document.createTextNode(a))}}var h=null,p=0;function f(e,n){var t,a,o;if(n.singleton){var s=p++;t=h||(h=l(n)),a=u.bind(null,t,s,!1),o=u.bind(null,t,s,!0)}else t=l(n),a=m.bind(null,t,n),o=function(){!function(e){if(null===e.parentNode)return!1;e.parentNode.removeChild(e)}(t)};return a(e),function(n){if(n){if(n.css===e.css&&n.media===e.media&&n.sourceMap===e.sourceMap)return;a(e=n)}else o()}}e.exports=function(e,n){(n=n||{}).singleton||"boolean"==typeof n.singleton||(n.singleton=(void 0===a&&(a=Boolean(window&&document&&document.all&&!window.atob)),a));var t=i(e=e||[],n);return function(e){if(e=e||[],"[object Array]"===Object.prototype.toString.call(e)){for(var a=0;a<t.length;a++){var o=r(t[a]);s[o].references--}for(var l=i(e,n),d=0;d<t.length;d++){var c=r(t[d]);0===s[c].references&&(s[c].updater(),s.splice(c,1))}t=l}}}}},n={};function t(a){var o=n[a];if(void 0!==o)return o.exports;var s=n[a]={id:a,exports:{}};return e[a](s,s.exports,t),s.exports}t.n=e=>{var n=e&&e.__esModule?()=>e.default:()=>e;return t.d(n,{a:n}),n},t.d=(e,n)=>{for(var a in n)t.o(n,a)&&!t.o(e,a)&&Object.defineProperty(e,a,{enumerable:!0,get:n[a]})},t.o=(e,n)=>Object.prototype.hasOwnProperty.call(e,n),t.nc=void 0,t(457),t(739)})();</script></body><script>window.setShowTime(true);\n    window.setShowExpand(false);\n    try {\n        const vscode = acquireVsCodeApi();\n        window.setVSCodeAPI(vscode);\n        document.getElementById("selectRunContainer").style.display = "block";\n    } catch (err) {\n        // That\'s ok (not running in VSCode).\n        window.setContents({\n            "initialContents": window.getSampleContents(),\n        });\n    }</script></html>'}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `robocorp_logging-0.0.8/PKG-INFO` & `robocorp_logging-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-logging
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automatic trace logging for Python
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

