# Comparing `tmp/acceptable-0.8.tar.gz` & `tmp/acceptable-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/acceptable-0.8.tar", last modified: Tue Apr 25 03:25:56 2017, max compression
+gzip compressed data, was "dist/acceptable-0.9.tar", last modified: Tue Jun 27 05:28:28 2017, max compression
```

## Comparing `acceptable-0.8.tar` & `acceptable-0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 thomi     (1000) thomi     (1000)        0 2017-04-25 03:25:56.000000 acceptable-0.8/
-drwxr-xr-x   0 thomi     (1000) thomi     (1000)        0 2017-04-25 03:25:56.000000 acceptable-0.8/acceptable/
--rw-r--r--   0 thomi     (1000) thomi     (1000)     4311 2017-04-05 01:11:00.000000 acceptable-0.8/acceptable/_doubles.py
--rw-r--r--   0 thomi     (1000) thomi     (1000)    10492 2017-04-19 22:42:06.000000 acceptable-0.8/acceptable/_build_doubles.py
--rw-r--r--   0 thomi     (1000) thomi     (1000)      386 2017-04-05 04:04:26.000000 acceptable-0.8/acceptable/__init__.py
--rw-r--r--   0 thomi     (1000) thomi     (1000)     6228 2017-04-25 03:24:13.000000 acceptable-0.8/acceptable/_validation.py
--rw-r--r--   0 thomi     (1000) thomi     (1000)     9774 2017-04-05 04:00:12.000000 acceptable-0.8/acceptable/_service.py
--rw-r--r--   0 thomi     (1000) thomi     (1000)     1293 2017-04-25 03:24:24.000000 acceptable-0.8/setup.py
--rw-r--r--   0 thomi     (1000) thomi     (1000)      309 2017-04-25 03:25:56.000000 acceptable-0.8/PKG-INFO
-drwxr-xr-x   0 thomi     (1000) thomi     (1000)        0 2017-04-25 03:25:56.000000 acceptable-0.8/acceptable.egg-info/
--rw-r--r--   0 thomi     (1000) thomi     (1000)       74 2017-04-25 03:25:56.000000 acceptable-0.8/acceptable.egg-info/entry_points.txt
--rw-r--r--   0 thomi     (1000) thomi     (1000)        1 2017-04-25 03:25:56.000000 acceptable-0.8/acceptable.egg-info/dependency_links.txt
--rw-r--r--   0 thomi     (1000) thomi     (1000)      338 2017-04-25 03:25:56.000000 acceptable-0.8/acceptable.egg-info/SOURCES.txt
--rw-r--r--   0 thomi     (1000) thomi     (1000)       17 2017-04-25 03:25:56.000000 acceptable-0.8/acceptable.egg-info/requires.txt
--rw-r--r--   0 thomi     (1000) thomi     (1000)      309 2017-04-25 03:25:56.000000 acceptable-0.8/acceptable.egg-info/PKG-INFO
--rw-r--r--   0 thomi     (1000) thomi     (1000)       11 2017-04-25 03:25:56.000000 acceptable-0.8/acceptable.egg-info/top_level.txt
--rw-r--r--   0 thomi     (1000) thomi     (1000)       38 2017-04-25 03:25:56.000000 acceptable-0.8/setup.cfg
+drwxr-xr-x   0 thomi     (1000) thomi     (1000)        0 2017-06-27 05:28:28.000000 acceptable-0.9/
+drwxr-xr-x   0 thomi     (1000) thomi     (1000)        0 2017-06-27 05:28:28.000000 acceptable-0.9/acceptable/
+-rw-r--r--   0 thomi     (1000) thomi     (1000)     4390 2017-06-27 05:27:43.000000 acceptable-0.9/acceptable/_doubles.py
+-rw-r--r--   0 thomi     (1000) thomi     (1000)    11235 2017-06-27 05:27:43.000000 acceptable-0.9/acceptable/_build_doubles.py
+-rw-r--r--   0 thomi     (1000) thomi     (1000)      386 2017-04-05 04:04:26.000000 acceptable-0.9/acceptable/__init__.py
+-rw-r--r--   0 thomi     (1000) thomi     (1000)     6228 2017-04-25 03:24:13.000000 acceptable-0.9/acceptable/_validation.py
+-rw-r--r--   0 thomi     (1000) thomi     (1000)     9774 2017-04-05 04:00:12.000000 acceptable-0.9/acceptable/_service.py
+-rw-r--r--   0 thomi     (1000) thomi     (1000)     1554 2017-05-02 14:58:56.000000 acceptable-0.9/README.rst
+-rw-r--r--   0 thomi     (1000) thomi     (1000)     1293 2017-06-27 05:27:52.000000 acceptable-0.9/setup.py
+-rw-r--r--   0 thomi     (1000) thomi     (1000)      309 2017-06-27 05:28:28.000000 acceptable-0.9/PKG-INFO
+drwxr-xr-x   0 thomi     (1000) thomi     (1000)        0 2017-06-27 05:28:28.000000 acceptable-0.9/acceptable.egg-info/
+-rw-r--r--   0 thomi     (1000) thomi     (1000)       74 2017-06-27 05:28:28.000000 acceptable-0.9/acceptable.egg-info/entry_points.txt
+-rw-r--r--   0 thomi     (1000) thomi     (1000)        1 2017-06-27 05:28:28.000000 acceptable-0.9/acceptable.egg-info/dependency_links.txt
+-rw-r--r--   0 thomi     (1000) thomi     (1000)      349 2017-06-27 05:28:28.000000 acceptable-0.9/acceptable.egg-info/SOURCES.txt
+-rw-r--r--   0 thomi     (1000) thomi     (1000)       17 2017-06-27 05:28:28.000000 acceptable-0.9/acceptable.egg-info/requires.txt
+-rw-r--r--   0 thomi     (1000) thomi     (1000)      309 2017-06-27 05:28:28.000000 acceptable-0.9/acceptable.egg-info/PKG-INFO
+-rw-r--r--   0 thomi     (1000) thomi     (1000)       11 2017-06-27 05:28:28.000000 acceptable-0.9/acceptable.egg-info/top_level.txt
+-rw-r--r--   0 thomi     (1000) thomi     (1000)       38 2017-06-27 05:28:28.000000 acceptable-0.9/setup.cfg
```

### Comparing `acceptable-0.8/acceptable/_doubles.py` & `acceptable-0.9/acceptable/_doubles.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,22 +45,23 @@
     # have a single RequestsMock instance shared across all ServiceMock
     # instances. This may cause bugs or unexpected behavior since the lifetime
     # of the service mock will be extended to be the lifetime of the longest
     # service mock.
     _requests_mock = None
 
     def __init__(self, service, methods, url, input_schema, output_schema,
-                 output):
+                 output, output_status=200):
         super().__init__()
         self._service = service
         self._methods = methods
         self._url = url
         self._input_schema = input_schema
         self._output_schema = output_schema
         self._output = output
+        self._output_status = output_status
 
     def _setUp(self):
         if self._output_schema:
             error_list = validate(self._output, self._output_schema)
             if error_list:
                 msg = (
                     "While setting up a service mock for the '{s._service}' "
@@ -93,15 +94,15 @@
                     return (
                         400,
                         {'Content-Type': 'application/json'},
                         json.dumps(error_list),
                     )
             # TODO: Do we need to support more than just json responses?
             return (
-                200,
+                self._output_status,
                 {"Content-Type": "application/json"},
                 json.dumps(self._output)
             )
 
         if ServiceMock._requests_mock is None:
             ServiceMock._requests_mock = responses.RequestsMock(
                 assert_all_requests_are_fired=False
```

### Comparing `acceptable-0.8/acceptable/_build_doubles.py` & `acceptable-0.9/acceptable/_build_doubles.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,16 @@
     build_parser.set_defaults(func=build_service_doubles)
 
     return parser.parse_args(arg_list)
 
 
 def scan_file(args):
     service_schemas = extract_schemas_from_file(args.file)
-    print(render_service_double('UNKNOWN', service_schemas))
+    print(render_service_double(
+        'UNKNOWN', service_schemas, 'scan-file %s' % args.file))
 
 
 def build_service_doubles(args):
     with tempfile.TemporaryDirectory() as workdir:
         service_config = read_service_config_file(args.config_file)
         target_root = os.path.dirname(args.config_file)
         for service_name in service_config['services']:
@@ -67,15 +68,16 @@
             source_url = service['git_source']
             service_dir = fetch_service_source(
                 workdir, service_name, source_url)
             service_schemas = []
             for scan_path in service['scan_paths']:
                 abs_path = os.path.join(service_dir, scan_path)
                 service_schemas.extend(extract_schemas_from_file(abs_path))
-            rendered = render_service_double(service_name, service_schemas)
+            rendered = render_service_double(
+                service_name, service_schemas, 'build %s' % args.config_file)
             write_service_double_file(target_root, service_name, rendered)
             print("Rendered schemas file for %s service: %d schemas" % (
                 service, len(service_schemas)))
 
 
 def read_service_config_file(config_path):
     with open(config_path, 'r') as config_file:
@@ -203,45 +205,59 @@
     for function in functions:
         input_schema = None
         output_schema = None
         api_options = None
         for decorator in function.decorator_list:
             if isinstance(decorator.func, ast.Attribute):
                 decorator_name = decorator.func.value.id
+                # extract version this view was introduced at, which can be
+                # specified as an arg or a kwarg:
+                version = None
+                for kwarg in decorator.keywords:
+                    if kwarg.arg == 'introduced_at':
+                        version = ast.literal_eval(kwarg.value)
+                        break
+                if len(decorator.args) == 1:
+                    version = ast.literal_eval(decorator.args[0])
+
                 if decorator_name in acceptable_views:
                     api_options = acceptable_views[decorator_name]
+                    api_options['version'] = version
             else:
                 decorator_name = decorator.func.id
                 if decorator_name == 'validate_body':
                     # TODO: Check that nothing in the tree below
                     # decorator.args[0] is an instance of 'ast.Name', and
                     # print a nice error message if it is.
                     input_schema = ast.literal_eval(decorator.args[0])
                 if decorator_name == 'validate_output':
                     output_schema = ast.literal_eval(decorator.args[0])
         if api_options:
             schema = ViewSchema(
                     view_name=api_options['name'],
-                    version='1.0',
+                    version=api_options['version'],
                     input_schema=input_schema,
                     output_schema=output_schema,
                     methods=api_options['methods'],
                     url=api_options['url'],
                 )
             schemas_found.append(schema)
     return schemas_found
 
 
-def render_service_double(service_name, schemas):
+def render_service_double(service_name, schemas, regenerate_args):
     header = textwrap.dedent("""\
         # This file is AUTO GENERATED. Do not edit this file directly. Instead,
-        # re-generate it by running {progname}.
+        # re-generate it by running '{progname} {regenerate_args}'.
 
         from acceptable._doubles import service_mock
-        """.format(progname=sys.argv[0]))
+        """.format(
+            progname=os.path.basename(sys.argv[0]),
+            regenerate_args=regenerate_args,
+        ))
 
     rendered_schemas = []
     for schema in schemas:
         double_name = '%s_%s' % (
             schema.view_name, schema.version.replace('.', '_'))
         rendered_schema = textwrap.dedent("""\
         {double_name} = service_mock(
```

### Comparing `acceptable-0.8/acceptable/_validation.py` & `acceptable-0.9/acceptable/_validation.py`

 * *Files identical despite different names*

### Comparing `acceptable-0.8/acceptable/_service.py` & `acceptable-0.9/acceptable/_service.py`

 * *Files identical despite different names*

### Comparing `acceptable-0.8/setup.py` & `acceptable-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright 2017 Canonical Ltd.  This software is licensed under the
 # GNU Lesser General Public License version 3 (see the file LICENSE).
 
 import pkg_resources
 from setuptools import setup
 
 
-VERSION = '0.8'
+VERSION = '0.9'
 
 
 def parse_requirements_file(path):
     """Parse a requirements file, return a list of requirements as strings."""
     with open(path, 'r') as rfile:
         deps = []
         for requirement in rfile.readlines():
```

