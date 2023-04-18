# Comparing `tmp/eons-2.3.5.tar.gz` & `tmp/eons-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.3.5.tar", last modified: Sat Apr 15 21:24:28 2023, max compression
+gzip compressed data, was "eons-2.3.6.tar", last modified: Tue Apr 18 14:54:08 2023, max compression
```

## Comparing `eons-2.3.5.tar` & `eons-2.3.6.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:28.065014 eons-2.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-15 21:24:28.065014 eons-2.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-04-15 21:24:13.000000 eons-2.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:28.061014 eons-2.3.5/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:28.061014 eons-2.3.5/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 21:24:20.000000 eons-2.3.5/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81676 2023-04-15 21:24:20.000000 eons-2.3.5/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:28.065014 eons-2.3.5/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:24:20.000000 eons-2.3.5/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-15 21:23:54.000000 eons-2.3.5/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-15 21:23:54.000000 eons-2.3.5/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-15 21:23:54.000000 eons-2.3.5/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-15 21:23:54.000000 eons-2.3.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-15 21:23:54.000000 eons-2.3.5/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:24:28.061014 eons-2.3.5/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-15 21:24:28.000000 eons-2.3.5/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-15 21:24:28.000000 eons-2.3.5/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:24:28.000000 eons-2.3.5/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-15 21:24:28.000000 eons-2.3.5/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 21:24:28.000000 eons-2.3.5/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-15 21:24:20.000000 eons-2.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-15 21:24:28.065014 eons-2.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.061581 eons-2.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-18 14:54:08.061581 eons-2.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-04-18 14:53:49.000000 eons-2.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.057581 eons-2.3.6/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.057581 eons-2.3.6/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 14:53:58.000000 eons-2.3.6/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82395 2023-04-18 14:53:58.000000 eons-2.3.6/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.057581 eons-2.3.6/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:53:58.000000 eons-2.3.6/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.061581 eons-2.3.6/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:53:58.000000 eons-2.3.6/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.057581 eons-2.3.6/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-18 14:54:08.000000 eons-2.3.6/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-18 14:54:08.000000 eons-2.3.6/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:54:08.000000 eons-2.3.6/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 14:54:08.000000 eons-2.3.6/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 14:54:08.000000 eons-2.3.6/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-18 14:53:58.000000 eons-2.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-18 14:54:08.061581 eons-2.3.6/setup.cfg
```

### Comparing `eons-2.3.5/PKG-INFO` & `eons-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.3.5
+Version: 2.3.6
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.3.5/README.md` & `eons-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.3.5/pkg/eons/eons.py` & `eons-2.3.6/pkg/eons/eons.py`

 * *Files 2% similar despite different names*

```diff
@@ -431,22 +431,22 @@
 
 	# Undo any changes made by Function.
 	# Please override this too!
 	def Rollback(this):
 		pass
 
 
-	# Override this to check results of operation and report on status.
-	# Override this to perform whatever success checks are necessary.
+	# Return whether or not Function was successful.
+	# Override this to perform whatever success and failure checks are necessary.
 	def DidFunctionSucceed(this):
 		return this.functionSucceeded
 
 
 	# RETURN whether or not the Rollback was successful.
-	# Override this to perform whatever success checks are necessary.
+	# Override this to perform whatever success and failure checks are necessary.
 	def DidRollbackSucceed(this):
 		return this.rollbackSucceeded
 
 
 	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
 	def ParseInitialArgs(this):
 		pass
@@ -794,22 +794,35 @@
 
 
 	# Call the next Functor.
 	# RETURN the result of the next Functor or None.
 	def CallNext(this):
 		if (not this.next):
 			return None
+		
+		# Something odd happens here; we've been getting:
+		# AttributeError("'builtin_function_or_method' object has no attribute 'pop'")
+		# But that implies we're getting a valid next object that is not a list.
+		# FIXME: Debug this.
+		proceedToNext = False
+		next = None
+		try:
+			next = this.next.pop(0)
+			proceedToNext = True
+		except Exception as e:
+			logging.error(f"{this.name} not proceeding to next: {e}; next: {this.next}")
+			return None
 
 		if (this.GetExecutor() is None):
 			raise InvalidNext(f"{this.name} has no executor and cannot execute next ({this.next}).")
 
-		next = this.next.pop(0)
-		if (not this.ValidateNext(next)):
-			raise InvalidNext(f"Failed to validate {next}")
-		return this.GetExecutor().Execute(next, precursor=this, next=this.next)
+		if (proceedToNext):
+			if (not this.ValidateNext(next)):
+				raise InvalidNext(f"Failed to validate {next}")
+			return this.GetExecutor().Execute(next, precursor=this, next=this.next)
 
 
 	def WarmUp(this, *args, **kwargs):
 
 		this.args = args
 		this.kwargs = kwargs
 		
@@ -1229,31 +1242,33 @@
 
 	# Run whatever.
 	# DANGEROUS!!!!!
 	# RETURN: Return value and, optionally, the output as a list of lines.
 	@method()
 	def RunCommand(this, command, saveout=False, raiseExceptions=True):
 		logging.debug(f"================ Running command: {command} ================")
-		p = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
+		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
 		output = []
-		while p.poll() is None:
-			line = p.stdout.readline().decode('utf8')[:-1]
+		while process.poll() is None:
+			line = process.stdout.readline().decode('utf8')[:-1]
 			if (saveout):
 				output.append(line)
 			if (line):
 				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
 
-		if (p.returncode is not None and p.returncode):
-			raise CommandUnsuccessful(f"Command returned {p.returncode}: {command}")
+		message = f"Command returned {process.returncode}: {command}"
+		logging.debug(message)
+		if (raiseExceptions and process.returncode is not None and process.returncode):
+			raise CommandUnsuccessful(message)
 		
 		logging.debug(f"================ Completed command: {command} ================")
 		if (saveout):
-			return p.returncode, output
+			return process.returncode, output
 		
-		return p.returncode
+		return process.returncode
 	######## END: UTILITIES ########
 
 
 # ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
 # This can be abused quite a bit, so please try to restrict usage of this to only:
 # * Ease of use global functions
 #
@@ -1928,14 +1943,15 @@
 
 	# Register included files early so that they can be used by the rest of the system.
 	# If we don't do this, we risk hitting infinite loops because modular functionality relies on these modules.
 	# NOTE: this method needs to be overridden in all children which ship included Functors, Data, etc. This is because __file__ is unique to the eons.py file, not the child's location.
 	def RegisterIncludedClasses(this):
 		includePaths = [
 			'resolve',
+			'method'
 		]
 		for path in includePaths:
 			this.RegisterAllClassesInDirectory(str(Path(__file__).resolve().parent.joinpath(path)))
 
 
 	# Executors should not have precursors
 	def PopulatePrecursor(this):
@@ -1997,14 +2013,17 @@
 		if (fetch):
 			# Take the highest of -v vs --verbosity
 			verbosity = this.EvaluateToType(this.Fetch('verbosity', 0, ['args', 'config', 'environment']))
 			if (verbosity > this.verbosity):
 				logging.debug(f"Setting verbosity to {verbosity}") # debug statements will be available when using external systems, like pytest.
 				this.verbosity = verbosity
 
+		if (this.verbosity == 0):
+			logging.getLogger().handlers[0].setLevel(logging.CRITICAL)
+			logging.getLogger().setLevel(logging.CRITICAL)
 		if (this.verbosity == 1):
 			logging.getLogger().handlers[0].setLevel(logging.WARNING)
 			logging.getLogger().setLevel(logging.WARNING)
 		elif (this.verbosity == 2):
 			logging.getLogger().handlers[0].setLevel(logging.INFO)
 			logging.getLogger().setLevel(logging.INFO)
 		elif(this.verbosity >= 3):
```

### Comparing `eons-2.3.5/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.3.6/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.5/pkg/eons/resolve/resolve_import_module.py` & `eons-2.3.6/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.3.6/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.5/pkg/eons.egg-info/PKG-INFO` & `eons-2.3.6/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.3.5
+Version: 2.3.6
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.3.5/setup.cfg` & `eons-2.3.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.3.5
+version = 2.3.6
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,17 +18,17 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	tqdm
-	requests
 	pyyaml
+	requests
+	tqdm
 	jsonpickle
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build =
```

