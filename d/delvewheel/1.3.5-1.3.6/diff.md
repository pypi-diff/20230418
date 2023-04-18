# Comparing `tmp/delvewheel-1.3.5.tar.gz` & `tmp/delvewheel-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delvewheel-1.3.5.tar", last modified: Fri Mar 24 15:08:16 2023, max compression
+gzip compressed data, was "delvewheel-1.3.6.tar", last modified: Tue Apr 18 13:53:35 2023, max compression
```

## Comparing `delvewheel-1.3.5.tar` & `delvewheel-1.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 15:08:16.435539 delvewheel-1.3.5/
--rw-rw-rw-   0        0        0     1073 2023-03-24 15:07:29.000000 delvewheel-1.3.5/LICENSE
--rw-rw-rw-   0        0        0    10124 2023-03-24 15:08:16.435539 delvewheel-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     9004 2023-03-24 15:07:29.000000 delvewheel-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-24 15:08:16.419913 delvewheel-1.3.5/delvewheel/
--rw-rw-rw-   0        0        0        0 2023-03-24 15:07:29.000000 delvewheel-1.3.5/delvewheel/__init__.py
--rw-rw-rw-   0        0        0     4987 2023-03-24 15:07:29.000000 delvewheel-1.3.5/delvewheel/__main__.py
--rw-rw-rw-   0        0        0   138556 2023-03-24 15:07:29.000000 delvewheel-1.3.5/delvewheel/_dll_list.py
--rw-rw-rw-   0        0        0    32890 2023-03-24 15:07:29.000000 delvewheel-1.3.5/delvewheel/_dll_utils.py
--rw-rw-rw-   0        0        0       23 2023-03-24 15:07:29.000000 delvewheel-1.3.5/delvewheel/_version.py
--rw-rw-rw-   0        0        0    40847 2023-03-24 15:07:29.000000 delvewheel-1.3.5/delvewheel/_wheel_repair.py
-drwxrwxrwx   0        0        0        0 2023-03-24 15:08:16.435539 delvewheel-1.3.5/delvewheel.egg-info/
--rw-rw-rw-   0        0        0    10124 2023-03-24 15:08:16.000000 delvewheel-1.3.5/delvewheel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-03-24 15:08:16.000000 delvewheel-1.3.5/delvewheel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 15:08:16.000000 delvewheel-1.3.5/delvewheel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-03-24 15:08:16.000000 delvewheel-1.3.5/delvewheel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-03-24 15:08:16.000000 delvewheel-1.3.5/delvewheel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-24 15:08:16.000000 delvewheel-1.3.5/delvewheel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      117 2023-03-24 15:07:29.000000 delvewheel-1.3.5/pyproject.toml
--rw-rw-rw-   0        0        0     1214 2023-03-24 15:08:16.435539 delvewheel-1.3.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 13:53:35.003922 delvewheel-1.3.6/
+-rw-rw-rw-   0        0        0     1073 2023-04-18 13:53:04.000000 delvewheel-1.3.6/LICENSE
+-rw-rw-rw-   0        0        0    10121 2023-04-18 13:53:35.003922 delvewheel-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9001 2023-04-18 13:53:04.000000 delvewheel-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 13:53:34.988566 delvewheel-1.3.6/delvewheel/
+-rw-rw-rw-   0        0        0        0 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/__init__.py
+-rw-rw-rw-   0        0        0     5169 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/__main__.py
+-rw-rw-rw-   0        0        0   138556 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/_dll_list.py
+-rw-rw-rw-   0        0        0    32890 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/_dll_utils.py
+-rw-rw-rw-   0        0        0       23 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/_version.py
+-rw-rw-rw-   0        0        0    41066 2023-04-18 13:53:04.000000 delvewheel-1.3.6/delvewheel/_wheel_repair.py
+drwxrwxrwx   0        0        0        0 2023-04-18 13:53:35.003922 delvewheel-1.3.6/delvewheel.egg-info/
+-rw-rw-rw-   0        0        0    10121 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-18 13:53:34.000000 delvewheel-1.3.6/delvewheel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      117 2023-04-18 13:53:04.000000 delvewheel-1.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1214 2023-04-18 13:53:35.003922 delvewheel-1.3.6/setup.cfg
```

### Comparing `delvewheel-1.3.5/LICENSE` & `delvewheel-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.5/PKG-INFO` & `delvewheel-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.3.5
+Version: 1.3.6
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
@@ -96,8 +96,8 @@
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
 - `delvewheel` creates or patches `__init__.py` in each top-level package so that the DLLs are loaded properly during import. This will cause issues if you have a top-level namespace package that requires `__init__.py` to be absent to function properly.
-- Support for delay-load DLLs is limited. Delay-load DLLs are vendored into the wheel, but dependending on the environment, errors may occur when they are loaded at runtime. If your project requires better support for delay-load DLLs, then file an issue.
+- Support for delay-load DLLs is limited. Delay-load DLLs are vendored into the wheel, but depending on the environment, errors may occur when they are loaded at runtime. If your project requires better support for delay-load DLLs, then file an issue.
```

### Comparing `delvewheel-1.3.5/README.md` & `delvewheel-1.3.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
 - `delvewheel` creates or patches `__init__.py` in each top-level package so that the DLLs are loaded properly during import. This will cause issues if you have a top-level namespace package that requires `__init__.py` to be absent to function properly.
-- Support for delay-load DLLs is limited. Delay-load DLLs are vendored into the wheel, but dependending on the environment, errors may occur when they are loaded at runtime. If your project requires better support for delay-load DLLs, then file an issue.
+- Support for delay-load DLLs is limited. Delay-load DLLs are vendored into the wheel, but depending on the environment, errors may occur when they are loaded at runtime. If your project requires better support for delay-load DLLs, then file an issue.
```

### Comparing `delvewheel-1.3.5/delvewheel/__main__.py` & `delvewheel-1.3.6/delvewheel/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         subparser.add_argument('--extract-dir', help=argparse.SUPPRESS)
         subparser.add_argument('--test', default='', help=argparse.SUPPRESS)  # comma-separated testing options, internal use only
     parser_repair.add_argument('-w', '--wheel-dir', dest='target', default='wheelhouse', help='directory to write repaired wheel')
     parser_repair.add_argument('--no-mangle', default='', metavar='DLLS', type=_dll_names, help=f'DLL names(s) not to mangle, {os.pathsep!r}-delimited')
     parser_repair.add_argument('--no-mangle-all', action='store_true', help="don't mangle any DLL names")
     parser_repair.add_argument('--strip', action='store_true', help='strip DLLs that contain trailing data when name-mangling')
     parser_repair.add_argument('-L', '--lib-sdir', default='.libs', type=_subdir_suffix, help='directory suffix in package to store vendored DLLs (default .libs)')
+    parser_repair.add_argument('--no-diagnostic', action='store_true', help=argparse.SUPPRESS)  # don't write diagnostic information to DELVEWHEEL metadata file
     parser_needed.add_argument('file', help='path to a DLL or PYD file')
     parser_needed.add_argument('-v', action='count', default=0, help='verbosity')
     args = parser.parse_args()
 
     # handle command
     if args.command in ('show', 'repair'):
         add_paths = dict.fromkeys(os.path.abspath(path) for path in args.add_path.split(os.pathsep) if path)
@@ -65,15 +66,15 @@
 
         for wheel in args.wheel:
             wr = WheelRepair(wheel, args.extract_dir, add_dlls, no_dlls, args.ignore_in_wheel, args.v, args.test.split(','))
             if args.command == 'show':
                 wr.show()
             else:  # args.command == 'repair'
                 no_mangles = set(dll_name.lower() for dll_name in args.no_mangle.split(os.pathsep) if dll_name)
-                wr.repair(args.target, no_mangles, args.no_mangle_all, args.strip, args.lib_sdir)
+                wr.repair(args.target, no_mangles, args.no_mangle_all, args.strip, args.lib_sdir, args.no_diagnostic)
     else:  # args.command == 'needed'
         for dll_name in sorted(_dll_utils.get_direct_needed(args.file, True, False, args.v), key=str.lower):
             print(dll_name)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `delvewheel-1.3.5/delvewheel/_dll_list.py` & `delvewheel-1.3.6/delvewheel/_dll_list.py`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.5/delvewheel/_dll_utils.py` & `delvewheel-1.3.6/delvewheel/_dll_utils.py`

 * *Files identical despite different names*

### Comparing `delvewheel-1.3.5/delvewheel/_wheel_repair.py` & `delvewheel-1.3.6/delvewheel/_wheel_repair.py`

 * *Files 1% similar despite different names*

```diff
@@ -494,22 +494,24 @@
             for ignored_dll_name in ignored_dll_names:
                 print(f'    {ignored_dll_name}')
         else:
             print('    None')
         if not_found_dll_names:
             print('\nWarning: At least one dependent DLL needs to be copied into the wheel but was not found.')
 
-    def repair(self, target: str, no_mangles: set, no_mangle_all: bool, strip: bool, lib_sdir: str) -> None:
+    def repair(self, target: str, no_mangles: set, no_mangle_all: bool, strip: bool, lib_sdir: str, no_diagnostic: bool) -> None:
         """Repair the wheel in a manner similar to auditwheel.
         target is the target directory for storing the repaired wheel
         no_mangles is a set of lowercase DLL names that will not be mangled
         no_mangle_all is True if no DLL name mangling should happen at all
         strip is True if we should strip DLLs that contain trailing data when
             name-mangling
-        lib_sdir is the suffix for the directory to store the DLLs"""
+        lib_sdir is the suffix for the directory to store the DLLs
+        no_diagnostic is True if no diagnostic information is written to the
+            DELVEWHEEL metadata file"""
         print(f'repairing {self._whl_path}')
 
         # check whether wheel has already been repaired
         repair_version = self._get_repair_version()
         if repair_version:
             print(f'Delvewheel {repair_version} has already repaired this wheel.')
             return
@@ -672,15 +674,15 @@
             # include the distribution name and version in the load-order
             # filename. Do this regardless of whether the wheel actually
             # contains a top-level extension module.
             load_order_filename = f'.load-order-{self._distribution_name}-{self._version}'
             load_order_filepath = os.path.join(libs_dir, load_order_filename)
             if os.path.exists(load_order_filepath):
                 raise FileExistsError(f'{os.path.relpath(load_order_filepath, self._extract_dir)} already exists')
-            with open(os.path.join(libs_dir, load_order_filename), 'w') as file:
+            with open(os.path.join(libs_dir, load_order_filename), 'w', newline='\n') as file:
                 file.write('\n'.join(reversed(rev_dll_load_order)))
                 file.write('\n')
         else:
             load_order_filename = None
 
         # Create or patch top-level __init__.py in each package to load
         # dependent DLLs from correct location at runtime.
@@ -714,15 +716,17 @@
 
         # Create .dist-info/DELVEWHEEL file to log repair information. The
         # first line of the file must be 'Version: ' followed by the delvewheel
         # version. Further lines are for information purposes only and are
         # subject to change without notice between delvewheel versions.
         filename = os.path.join(self._extract_dir, dist_info_foldername, 'DELVEWHEEL')
         with open(filename, 'w', newline='\n') as file:
-            file.write(f'Version: {_version.__version__}\nArguments: {sys.argv}\n')
+            file.write(f'Version: {_version.__version__}\n')
+            if not no_diagnostic:
+                file.write(f'Arguments: {sys.argv}\n')
 
         # update record file, which tracks wheel contents and their checksums
         record_filepath = os.path.join(self._extract_dir, dist_info_foldername, 'RECORD')
         print(f'updating {os.path.join(dist_info_foldername, "RECORD")}')
         filepath_list = []
         for root, _, files in os.walk(self._extract_dir):
             for file in files:
```

### Comparing `delvewheel-1.3.5/delvewheel.egg-info/PKG-INFO` & `delvewheel-1.3.6/delvewheel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delvewheel
-Version: 1.3.5
+Version: 1.3.6
 Summary: Self-contained wheels for Windows
 Home-page: https://github.com/adang1345/delvewheel
 Author: Aohan Dang
 Author-email: adang1345@gmail.com
 License: MIT
 Platform: Windows
 Classifier: License :: OSI Approved :: MIT License
@@ -96,8 +96,8 @@
 
 - `delvewheel` reads DLL file headers to determine which libraries a wheel depends on. DLLs that are loaded at runtime using `ctypes`/`cffi` (from Python) or `LoadLibrary` (from C/C++) will be missed. You can, however, specify additional DLLs to vendor into the wheel using the `--add-dll` option. If you elect to do this, it is your responsibility to ensure that the additional DLL is found at load time.
 - Wheels created using `delvewheel` are not guaranteed to work on systems older than Windows 7 SP1. If you intend to create a wheel for an old Windows system, you should test the resultant wheel thoroughly. If it turns out that getting the wheel to work on an older system simply requires an extra DLL, you can use the `--add-dll` flag to vendor additional DLLs into the wheel.
 - To avoid DLL hell, we mangle the file names of most DLLs that are vendored into the wheel. This way, a Python process that tries loading a vendored DLL does not end up using a different DLL with the same name. Due to a limitation in how name-mangling is performed, `delvewheel` is unable to name-mangle DLLs whose dependents contain insufficient internal padding to fit the mangled names and contain trailing data at the end of the binary. An exception will be raised if such a DLL is encountered. Commonly, trailing data consist of symbols that can be safely removed using the GNU `strip` utility, although there exist situations where the data must be present for the DLL to function properly. To remove the trailing data, execute `strip -s EXAMPLE.dll` or use the `--strip` flag. To keep the trailing data and skip name mangling, use the `--no-mangle` or `--no-mangle-all` flag.
 - Any DLL containing an Authenticode signature will have its signature cleared if its dependencies are name-mangled.
 - `delvewheel` cannot repair a wheel that contains extension modules targeting more than one CPU architecture (e.g. both `win32` and `win_amd64`). You should create a separate wheel for each CPU architecture and repair each individually.
 - `delvewheel` creates or patches `__init__.py` in each top-level package so that the DLLs are loaded properly during import. This will cause issues if you have a top-level namespace package that requires `__init__.py` to be absent to function properly.
-- Support for delay-load DLLs is limited. Delay-load DLLs are vendored into the wheel, but dependending on the environment, errors may occur when they are loaded at runtime. If your project requires better support for delay-load DLLs, then file an issue.
+- Support for delay-load DLLs is limited. Delay-load DLLs are vendored into the wheel, but depending on the environment, errors may occur when they are loaded at runtime. If your project requires better support for delay-load DLLs, then file an issue.
```

### Comparing `delvewheel-1.3.5/setup.cfg` & `delvewheel-1.3.6/setup.cfg`

 * *Files identical despite different names*

