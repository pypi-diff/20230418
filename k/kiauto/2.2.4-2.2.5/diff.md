# Comparing `tmp/kiauto-2.2.4.tar.gz` & `tmp/kiauto-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiauto-2.2.4.tar", last modified: Thu Apr 13 14:15:04 2023, max compression
+gzip compressed data, was "kiauto-2.2.5.tar", last modified: Tue Apr 18 10:46:40 2023, max compression
```

## Comparing `kiauto-2.2.4.tar` & `kiauto-2.2.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:15:04.587207 kiauto-2.2.4/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-12 16:15:23.000000 kiauto-2.2.4/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       67 2023-04-12 16:15:23.000000 kiauto-2.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    17079 2023-04-13 14:15:04.587207 kiauto-2.2.4/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    13874 2023-04-12 16:15:23.000000 kiauto-2.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:15:04.587207 kiauto-2.2.4/kiauto/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    14848 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/file_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:15:04.587207 kiauto-2.2.4/kiauto/interposer/
--rwxrwxr-x   0 root         (0) root         (0)    27344 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/interposer/libinterposer.so
--rw-rw-r--   0 root         (0) root         (0)    27969 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/interposer.py
--rw-rw-r--   0 root         (0) root         (0)     3755 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/log.py
--rw-rw-r--   0 root         (0) root         (0)    14310 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/misc.py
--rw-rw-r--   0 root         (0) root         (0)    18923 2023-04-12 16:15:23.000000 kiauto-2.2.4/kiauto/ui_automation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:15:04.587207 kiauto-2.2.4/kiauto.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17079 2023-04-13 14:15:04.000000 kiauto-2.2.4/kiauto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-13 14:15:04.000000 kiauto-2.2.4/kiauto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 14:15:04.000000 kiauto-2.2.4/kiauto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-13 14:15:04.000000 kiauto-2.2.4/kiauto.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 14:15:04.000000 kiauto-2.2.4/kiauto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 14:15:04.587207 kiauto-2.2.4/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1410 2023-04-12 16:15:23.000000 kiauto-2.2.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 14:15:04.587207 kiauto-2.2.4/src/
--rwxrwxr-x   0 root         (0) root         (0)    40781 2023-04-12 16:15:23.000000 kiauto-2.2.4/src/eeschema_do
--rwxrwxr-x   0 root         (0) root         (0)     6979 2023-04-12 16:15:23.000000 kiauto-2.2.4/src/kicad2step_do
--rwxrwxr-x   0 root         (0) root         (0)    75176 2023-04-12 16:15:23.000000 kiauto-2.2.4/src/pcbnew_do
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:46:40.004420 kiauto-2.2.5/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-04-18 10:45:17.000000 kiauto-2.2.5/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-04-18 10:45:17.000000 kiauto-2.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17079 2023-04-18 10:46:40.004420 kiauto-2.2.5/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    13874 2023-04-18 10:45:17.000000 kiauto-2.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:46:40.004420 kiauto-2.2.5/kiauto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    14942 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/file_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:46:40.004420 kiauto-2.2.5/kiauto/interposer/
+-rwxrwxr-x   0 root         (0) root         (0)    27344 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/interposer/libinterposer.so
+-rw-rw-r--   0 root         (0) root         (0)    28139 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/interposer.py
+-rw-rw-r--   0 root         (0) root         (0)     3755 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/log.py
+-rw-rw-r--   0 root         (0) root         (0)    14340 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    19007 2023-04-18 10:45:17.000000 kiauto-2.2.5/kiauto/ui_automation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:46:40.004420 kiauto-2.2.5/kiauto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17079 2023-04-18 10:46:39.000000 kiauto-2.2.5/kiauto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-18 10:46:39.000000 kiauto-2.2.5/kiauto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 10:46:39.000000 kiauto-2.2.5/kiauto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-18 10:46:39.000000 kiauto-2.2.5/kiauto.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-18 10:46:39.000000 kiauto-2.2.5/kiauto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 10:46:40.004420 kiauto-2.2.5/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1410 2023-04-18 10:45:17.000000 kiauto-2.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 10:46:40.004420 kiauto-2.2.5/src/
+-rwxrwxr-x   0 root         (0) root         (0)    43160 2023-04-18 10:45:17.000000 kiauto-2.2.5/src/eeschema_do
+-rwxrwxr-x   0 root         (0) root         (0)     6979 2023-04-18 10:45:17.000000 kiauto-2.2.5/src/kicad2step_do
+-rwxrwxr-x   0 root         (0) root         (0)    75176 2023-04-18 10:45:17.000000 kiauto-2.2.5/src/pcbnew_do
```

### Comparing `kiauto-2.2.4/LICENSE` & `kiauto-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.4/PKG-INFO` & `kiauto-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiauto
-Version: 2.2.4
+Version: 2.2.5
 Summary: KiCad Automation Scripts
 Home-page: https://github.com/INTI-CMNB/KiAuto/
 Author: Salvador E. Tropea
 Author-email: stropea@inti.gob.ar
 License: Apache License 2.0
 Description: 
         KiAuto
```

### Comparing `kiauto-2.2.4/README.md` & `kiauto-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.4/kiauto/file_util.py` & `kiauto-2.2.5/kiauto/file_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,18 @@
                     logger.error('Syntax error at line {} in filter file `{}`: `{}`'.format(ln, file, line))
                     logger.error('Use `ERROR_NUMBER,REGEX` format')
                     exit(WRONG_ARGUMENTS)
             ln = ln+1
         logger.info('Loaded {} error filters from `{}`'.format(fl, file))
 
 
+def add_filter(cfg, id, regex):
+    cfg.err_filters.append((id, regex))
+
+
 def apply_filters(cfg, err_name, wrn_name):
     """ Apply the error filters to the list of errors and unconnecteds """
     if len(cfg.err_filters) == 0:
         return (0, 0)
     skip_err = 0
     for i, err in enumerate(cfg.errs):
         for f in cfg.err_filters:
@@ -131,26 +135,26 @@
     return skip_err, skip_wrn
 
 
 def list_errors(cfg):
     for err in cfg.errs:
         if err:
             if "; Severity: warning" in err:
-                logger.warning(err.replace("; Severity: warning", ''))
+                logger.warning(re.sub(" +; Severity: warning\n?", '', err))
             else:
-                logger.error(err.replace("; Severity: error", ''))
+                logger.error(re.sub(" +; Severity: error\n?", '', err))
 
 
 def list_warnings(cfg):
     for wrn in cfg.wrns:
         if wrn:
             if "; Severity: error" in wrn:
-                logger.error(wrn.replace("; Severity: error", ''))
+                logger.error(re.sub(" +; Severity: error\n?", ''), wrn)
             else:
-                logger.warning(wrn.replace("; Severity: warning", ''))
+                logger.warning(re.sub(" +; Severity: warning\n?", '', wrn))
 
 
 def check_kicad_config_dir(cfg):
     if not os.path.isdir(cfg.kicad_conf_path):
         logger.debug('Creating KiCad config dir')
         os.makedirs(cfg.kicad_conf_path, exist_ok=True)
```

### Comparing `kiauto-2.2.4/kiauto/interposer/libinterposer.so` & `kiauto-2.2.5/kiauto/interposer/libinterposer.so`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.4/kiauto/interposer.py` & `kiauto-2.2.5/kiauto/interposer.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,34 +249,38 @@
             return KICAD_EXIT_MSG
         cfg.logger.debug('= KiCad finally sleeping')
     else:
         cfg.logger.debug('= KiCad already sleeping ({})'.format(status))
     return res
 
 
-def open_dialog_i(cfg, name, keys, no_show=False, no_wait=False, no_main=False, extra_msg=None):
+def open_dialog_i(cfg, name, keys, no_show=False, no_wait=False, no_main=False, extra_msg=None, raise_if=None):
     wait_point(cfg)
     # Wait for KiCad to be sleeping
     wait_kicad_ready_i(cfg)
     cfg.logger.info('Opening dialog `{}` {}'.format(name, '('+extra_msg+')' if extra_msg is not None else ''))
     if isinstance(keys, str):
         keys = ['key', keys]
     xdotool(keys)
     pre_gtk_title = 'GTK:Window Title:'
     pre_gtk = pre_gtk_title if no_show else 'GTK:Window Show:'
     if isinstance(name, str):
         name = [name]
     name_w_pre = [pre_gtk+f for f in name]
+    if raise_if is not None:
+        name_w_pre.extend(raise_if)
     # Add the async dialogs
     for t in ASYNC_DIALOGS:
         name_w_pre.append(pre_gtk_title+t)
     # Wait for our dialog or any async dialog
     # Note: wait_queue won't dismiss them because we use "with_windows=True"
     while True:
         res = wait_queue(cfg, name_w_pre, with_windows=True)
+        if raise_if is not None and res in raise_if:
+            raise InterruptedError()
         title = res[len(pre_gtk_title):]
         if title not in ASYNC_DIALOGS:
             break
         if title in INFO_DIALOGS:
             # Get rid of the info dialog
             dismiss_pcb_info(cfg, title)
         else:
```

### Comparing `kiauto-2.2.4/kiauto/log.py` & `kiauto-2.2.5/kiauto/log.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.4/kiauto/misc.py` & `kiauto-2.2.5/kiauto/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 NIGHTLY = 'nightly'
 # Scale factor for the timeouts
 TIME_OUT_MULT = 1.0
 
 KICAD_VERSION_5_99 = 5099000
 KICAD_VERSION_6_99 = 6099000
 KICAD_VERSION_7_99 = 7099000
+KICAD_VERSION_7_0_3 = 7000003
 KICAD_SHARE = '/usr/share/kicad/'
 KICAD_NIGHTLY_SHARE = '/usr/share/kicad-nightly/'
 
 
 @contextmanager
 def hide_stderr():
     """ Low level stderr supression, used to hide KiCad bugs. """
@@ -339,8 +340,8 @@
 __author__ = 'Salvador E. Tropea'
 __copyright__ = 'Copyright 2018-2023, INTI/Productize SPRL'
 __credits__ = ['Salvador E. Tropea', 'Seppe Stas', 'Jesse Vincent', 'Scott Bezek']
 __license__ = 'Apache 2.0'
 __email__ = 'stropea@inti.gob.ar'
 __status__ = 'stable'
 __url__ = 'https://github.com/INTI-CMNB/KiAuto/'
-__version__ = '2.2.4'
+__version__ = '2.2.5'
```

### Comparing `kiauto-2.2.4/kiauto/ui_automation.py` & `kiauto-2.2.5/kiauto/ui_automation.py`

 * *Files 0% similar despite different names*

```diff
@@ -411,37 +411,38 @@
 
 
 def wait_point(cfg):
     if cfg.wait_for_key:
         input('Press a key')
 
 
-def capture_window_region(window_id, x, y, w, h, name):
+def capture_window_region(window_id, x, y, w, h, name, to_capture=None):
     """ Capture a region of a window to a file """
     geometry = '{}x{}+{}+{}'.format(w, h, x, y)
     logger.debug('Capturing region {} from window {}'.format(geometry, window_id))
     name = os.path.join(img_tmp_dir, name)
     if not shutil.which('import'):
         logger.error("import isn't installed, please install it.\nThis is part of ImageMagick and GraphicsMagic packages.")
         sys.exit(MISSING_TOOL)
-    res = check_output(['import', '-window', str(window_id), '-crop', geometry, name], stderr=DEVNULL).decode()
+    res = check_output(['import', '-window', str(window_id), '-crop', geometry, name], stderr=DEVNULL,
+                       timeout=to_capture).decode()
     logger.debug('Import output: ' + res)
 
 
 def wait_window_get_ref(window_id, x, y, w, h):
     """ Takes a region of a window as reference image """
     global img_tmp_dir
     img_tmp_dir = mkdtemp(prefix='tmp-kiauto-images-')
     capture_window_region(window_id, x, y, w, h, "wait_ref.png")
 
 
-def wait_window_change(window_id, x, y, w, h, time_out):
+def wait_window_change(window_id, x, y, w, h, time_out, to_capture):
     """ Waits for a change in a window region """
     for i in range(int(time_out + 0.9)):
-        capture_window_region(window_id, x, y, w, h, "current.png")
+        capture_window_region(window_id, x, y, w, h, "current.png", to_capture)
         current = os.path.join(img_tmp_dir, "current.png")
         wait_ref = os.path.join(img_tmp_dir, "wait_ref.png")
         difference = os.path.join(img_tmp_dir, "difference.png")
         res = run(['compare', '-fuzz', '5%', '-metric', 'AE', current, wait_ref, difference],
                   stderr=PIPE).stderr.decode()
         ae = int(res)
         logger.debug('Difference ' + res)
```

### Comparing `kiauto-2.2.4/kiauto.egg-info/PKG-INFO` & `kiauto-2.2.5/kiauto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiauto
-Version: 2.2.4
+Version: 2.2.5
 Summary: KiCad Automation Scripts
 Home-page: https://github.com/INTI-CMNB/KiAuto/
 Author: Salvador E. Tropea
 Author-email: stropea@inti.gob.ar
 License: Apache License 2.0
 Description: 
         KiAuto
```

### Comparing `kiauto-2.2.4/setup.py` & `kiauto-2.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.4/src/eeschema_do` & `kiauto-2.2.5/src/eeschema_do`

 * *Files 3% similar despite different names*

```diff
@@ -38,18 +38,19 @@
 from kiauto import log
 log.set_domain(os.path.splitext(os.path.basename(__file__))[0])
 logger = None
 
 from kiauto.file_util import (load_filters, wait_for_file_created_by_process, apply_filters, list_errors, list_warnings,
                               check_kicad_config_dir, restore_config, backup_config, check_lib_table, create_user_hotkeys,
                               check_input_file, memorize_project, restore_project, get_log_files, create_kicad_config,
-                              set_time_out_scale as set_time_out_scale_f)
+                              set_time_out_scale as set_time_out_scale_f, add_filter)
 from kiauto.misc import (REC_W, REC_H, __version__, NO_SCHEMATIC, EESCHEMA_CFG_PRESENT, KICAD_CFG_PRESENT,
                          WAIT_START, WRONG_SCH_NAME, EESCHEMA_ERROR, Config, KICAD_VERSION_5_99, WONT_OVERWRITE,
-                         USER_HOTKEYS_PRESENT, __copyright__, __license__, TIME_OUT_MULT, get_en_locale, KICAD_CLI_ERROR)
+                         USER_HOTKEYS_PRESENT, __copyright__, __license__, TIME_OUT_MULT, get_en_locale, KICAD_CLI_ERROR,
+                         KICAD_VERSION_7_0_3)
 from kiauto.interposer import (check_interposer, dump_interposer_dialog, start_queue, wait_start_by_msg,
                                set_kicad_process, open_dialog_i,
                                paste_output_file_i, exit_kicad_i, paste_text_i, wait_queue,
                                paste_bogus_filename, setup_interposer_filename, send_keys, wait_create_i)
 from kiauto.ui_automation import (PopenContext, xdotool, wait_for_window, wait_not_focused, recorded_xvfb,
                                   wait_point, text_replace, set_time_out_scale, wait_xserver, wait_window_get_ref,
                                   wait_window_change, open_dialog_with_retry, ShowInfoAction)
@@ -317,14 +318,19 @@
     for i, line in enumerate(lines):
         m = err_regex.search(line)
         if m:
             msg = '({}) {}'.format(m.group(1), m.group(2))
             if cfg.kicad_version >= KICAD_VERSION_5_99 and i < len(lines):
                 # KiCad 6 moved the severity to the next line
                 line = lines[i+1]
+                # KiCad 7.0.2 bug: a message with two extra \n
+                # Error reading simulation model from symbol '#PWR03':\nFailed to read simulation model from fields.\n
+                if '; Severity' not in line and i+3 < len(lines) and lines[i+2] == '':
+                    msg += ' '+line
+                    line = lines[i+3]
             # Discard messages explicitly excluded using the GUI
             excluded = '(excluded)' in line
             if r'Severity: error' in line:
                 is_err = True
                 if excluded:
                     errors_excl += 1
                 else:
@@ -407,32 +413,65 @@
     # Close the ERC dialog
     send_keys(cfg, 'Exit ERC', 'alt+l', closes=dialog)
 
 
 def eeschema_run_erc_schematic_6_0_n(cfg):
     # Open the ERC dialog
     keys = ['key', 'Escape', 'ctrl+shift+i']
-    id = open_dialog_with_retry('Open Tools->Electrical Rules Checker', keys, 'Electrical Rules Checker dialog',
-                                'Electrical Rules Checker', cfg)
+    erc_name = 'Electrical Rules Checker dialog'
+    erc_title = 'Electrical Rules Checker'
+    erc_msg = 'Open Tools->Electrical Rules Checker'
+    id = open_dialog_with_retry(erc_msg, keys, erc_name, erc_title, cfg)
     wait_point(cfg)
     # Run the ERC
     logger.info('Run ERC')
     wait_point(cfg)
     wait_window_get_ref(id[0], 108, 27, 100, 10)
     xdotool(['key', 'Return'])
     #
     # Currently is impossible to know when it finished.
     #
-    wait_window_change(id[0], 108, 27, 100, 10, 45*cfg.time_out_scale)
+    try_again = False
+    try:
+        wait_window_change(id[0], 108, 27, 100, 10, 45*cfg.time_out_scale, 3*cfg.time_out_scale)
+    except subprocess.TimeoutExpired:
+        try_again = True
+    if try_again:
+        # KiCad 7.0.2 bug, closes ERC dialog after finishing
+        logger.warning('Time out capturing from the '+erc_name+', trying to open it again')
+        id = open_dialog_with_retry(erc_msg, keys, erc_name, erc_title, cfg)
     # Save the report
     logger.info('Open the save dialog')
     wait_point(cfg)
-    xdotool(['key', 'Tab', 'Tab', 'Tab', 'Tab', 'Tab', 'Tab', 'Tab', 'Tab', 'Return'])
+    keys_save = ['key', 'Tab', 'Tab', 'Tab', 'Tab', 'Tab', 'Tab', 'Tab', 'Tab', 'Return']
+    xdotool(keys_save)
     # Wait for the save dialog
-    wait_for_window('ERC File save dialog', 'Save Report to File')
+    try_again = False
+    try:
+        wait_for_window('ERC File save dialog', 'Save Report to File')
+    except RuntimeError:
+        if cfg.ki7:
+            try_again = True
+        else:
+            raise
+    if try_again:
+        # KiCad 7.0.2 bug, closes ERC dialog after finishing
+        found = False
+        try:
+            wait_for_window(erc_name, erc_title, timeout=1)
+            found = True
+        except RuntimeError:
+            pass
+        if found:
+            logger.error(erc_name+' not responding')
+            exit(EESCHEMA_ERROR)
+        logger.warning(erc_name+' suddenly closed, trying to open it again')
+        id = open_dialog_with_retry(erc_msg, keys, erc_name, erc_title, cfg)
+        xdotool(keys_save)
+        wait_for_window('ERC File save dialog', 'Save Report to File')
     # Paste the name
     logger.info('Pasting output file')
     wait_point(cfg)
     text_replace(cfg.output_file)
     # Wait for report created
     logger.info('Wait for ERC file creation')
     wait_point(cfg)
@@ -445,21 +484,31 @@
 
 
 def eeschema_run_erc_schematic_6_0_i(cfg):
     # KiCad 7.99 particularities:
     # 1. Forces ".rpt" in the name, no matter what name was selected in the dialog and no matter if it already has an extension
     # 2. The ERC dialog isn't destroyed, most probably hidden
     # Open the ERC dialog
-    dialog, _ = open_dialog_i(cfg, 'Electrical Rules Checker', 'ctrl+shift+i', no_main=True)
+    title = 'Electrical Rules Checker'
+    dialog, _ = open_dialog_i(cfg, title, 'ctrl+shift+i', no_main=True)
     # Run the ERC
     send_keys(cfg, 'Run ERC', 'Return')
     # Wait for completion. The Close button is refreshed at the end
     wait_queue(cfg, 'GTK:Button Label:C_lose')
     # Save the report
-    file_dlg, _ = open_dialog_i(cfg, 'Save Report to File', 'alt+s')
+    reopen = False
+    try:
+        # Catch the ERC unintentional close
+        file_dlg, _ = open_dialog_i(cfg, 'Save Report to File', 'alt+s', raise_if=['GTK:Window Destroy:'+title])
+    except InterruptedError:
+        reopen = True
+    if reopen:
+        # KiCad 7.0.2 bug, in some cases the dialog is closed, we just need to open it again
+        dialog, _ = open_dialog_i(cfg, title, 'ctrl+shift+i', no_main=True)
+        file_dlg, _ = open_dialog_i(cfg, 'Save Report to File', 'alt+s')
     # Paste the output file
     paste_bogus_filename(cfg)
     send_keys(cfg, 'Create the report', 'Return', closes=file_dlg, delay_io=True)
     # Wait until created
     wait_create_i(cfg, 'ERC', forced_ext='rpt')
     # Close the ERC dialog
     send_keys(cfg, 'Exit ERC', 'Escape', closes=dialog, no_destroy=cfg.ki8)
@@ -615,15 +664,16 @@
             # plot_ops['hpgl_paper_size'] = ??
             plot_ops['hpgl_pen_size'] = cfg.hpgl_pen_size
             eeconf = {'plot': plot_ops}
             eeconf['system'] = {"first_run_shown": True, "never_show_rescue_dialog": True}
             eeconf['appearance'] = {"show_sexpr_file_convert_warning": False, "color_theme": cfg.color_theme.lower()}
             eeconf['window'] = {"size_x": cfg.rec_width, "size_y": cfg.rec_height,
                                 # Select the user grid and the provided grid. X/Y the same.
-                                "grid": {"last_size": 7, "user_grid_x": "%d mil" % cfg.grid, "user_grid_y": "%d mil" % cfg.grid}}
+                                "grid": {"last_size": 7, "user_grid_x": "%d mil" % cfg.grid,
+                                         "user_grid_y": "%d mil" % cfg.grid}}
             text = json.dumps(eeconf)
             text_file.write(text)
             logger.debug(text)
         else:
             text_file.write('RescueNeverShow=1\n')
             text_file.write('ShowIllegalSymbolLibDialog=0\n')
             text_file.write('ShowSheetFileNameCaseSensitivityDlg=0\n')
@@ -781,16 +831,21 @@
     cfg.color_theme = getattr(args, 'color_theme', '_builtin_default')
     cfg.background_color = getattr(args, 'background_color', False)
     cfg.hpgl_origin = getattr(args, 'hpgl_origin', 0)
     cfg.hpgl_pen_size = getattr(args, 'hpgl_pen_size', 0.19)
     # Make sure the input file exists and has an extension
     check_input_file(cfg, NO_SCHEMATIC, WRONG_SCH_NAME)
     # Load filters
-    if args.command == 'run_erc' and args.errors_filter:
-        load_filters(cfg, args.errors_filter[0])
+    if args.command == 'run_erc':
+        if args.errors_filter:
+            load_filters(cfg, args.errors_filter[0])
+        if cfg.ki7 and cfg.kicad_version < KICAD_VERSION_7_0_3:
+            # Bug introduced in 7.0.2. But I want to potentially cover 7.0.2.1
+            logger.debug("Adding filters to workaround KiCad 7.0.2 simulation models bug")
+            add_filter(cfg, 'simulation_model_issue', r"from symbol '#")
 
     memorize_project(cfg)
     # Create output dir if it doesn't exist
     output_dir = os.path.abspath(args.output_dir)+'/'
     cfg.video_dir = cfg.output_dir = output_dir
     #
     # Configure KiCad in a deterministic way
```

### Comparing `kiauto-2.2.4/src/kicad2step_do` & `kiauto-2.2.5/src/kicad2step_do`

 * *Files identical despite different names*

### Comparing `kiauto-2.2.4/src/pcbnew_do` & `kiauto-2.2.5/src/pcbnew_do`

 * *Files identical despite different names*

