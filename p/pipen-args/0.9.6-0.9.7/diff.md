# Comparing `tmp/pipen_args-0.9.6.tar.gz` & `tmp/pipen_args-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_args-0.9.6.tar", max compression
+gzip compressed data, was "pipen_args-0.9.7.tar", max compression
```

## Comparing `pipen_args-0.9.6.tar` & `pipen_args-0.9.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2173 2023-04-17 23:32:26.608250 pipen_args-0.9.6/README.md
--rw-r--r--   0        0        0      969 2023-04-17 23:32:26.608250 pipen_args-0.9.6/pipen_args/__init__.py
--rw-r--r--   0        0        0     3872 2023-04-17 23:32:26.608250 pipen_args-0.9.6/pipen_args/defaults.py
--rw-r--r--   0        0        0     9934 2023-04-17 23:32:26.608250 pipen_args-0.9.6/pipen_args/parser_.py
--rw-r--r--   0        0        0     8055 2023-04-17 23:32:26.608250 pipen_args-0.9.6/pipen_args/plugin.py
--rw-r--r--   0        0        0     3277 2023-04-17 23:32:26.608250 pipen_args-0.9.6/pipen_args/procgroup.py
--rw-r--r--   0        0        0       22 2023-04-17 23:32:26.608250 pipen_args-0.9.6/pipen_args/version.py
--rw-r--r--   0        0        0     1185 2023-04-17 23:32:26.612250 pipen_args-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     3016 1970-01-01 00:00:00.000000 pipen_args-0.9.6/setup.py
--rw-r--r--   0        0        0     2864 1970-01-01 00:00:00.000000 pipen_args-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     2172 2023-04-18 06:25:41.328574 pipen_args-0.9.7/README.md
+-rw-r--r--   0        0        0      969 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/__init__.py
+-rw-r--r--   0        0        0     3871 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/defaults.py
+-rw-r--r--   0        0        0     9934 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/parser_.py
+-rw-r--r--   0        0        0     8053 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/plugin.py
+-rw-r--r--   0        0        0     3277 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/procgroup.py
+-rw-r--r--   0        0        0       22 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pipen_args/version.py
+-rw-r--r--   0        0        0     1185 2023-04-18 06:25:41.328574 pipen_args-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     3015 1970-01-01 00:00:00.000000 pipen_args-0.9.7/setup.py
+-rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 pipen_args-0.9.7/PKG-INFO
```

### Comparing `pipen_args-0.9.6/README.md` & `pipen_args-0.9.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 Pipeline Options:
   --name NAME           The name for the pipeline, will affect the default workdir and
                         outdir. [default: pipen-0]
   --profile PROFILE     The default profile from the configuration to run the pipeline.
                         This profile will be used unless a profile is specified in the
                         process or in the .run method of pipen. You can check the
                         available profiles by running `pipen profile`
-  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>_results]
+  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>-output]
   --forks FORKS         How many jobs to run simultaneously by the scheduler
   --scheduler SCHEDULER
                         The scheduler to run the jobs
 
 Namespace <in>:
   --in.a A [A ...]      Input data
```

### Comparing `pipen_args-0.9.6/pipen_args/__init__.py` & `pipen_args-0.9.7/pipen_args/__init__.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.6/pipen_args/defaults.py` & `pipen_args-0.9.7/pipen_args/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         help=(
             "The language interpreter to use for the pipeline/process "
             "[default: bash]"
         ),
         show=False,
     ),
     outdir=Diot(
-        help="The output directory of the pipeline [default: ./<name>_results]",
+        help="The output directory of the pipeline [default: ./<name>-output]",
         type="path",
     ),
     loglevel=Diot(
         help=(
             "The logging level for the main logger, only takes effect "
             "after pipeline is initialized [default: INFO]"
         ),
```

### Comparing `pipen_args-0.9.6/pipen_args/parser_.py` & `pipen_args-0.9.7/pipen_args/parser_.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.6/pipen_args/plugin.py` & `pipen_args-0.9.7/pipen_args/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         ):
             if getattr(parsed, key, None) is not None:
                 config[key] = getattr(parsed, key)
 
         # The original name
         pipen_name = pipen.name
         # The default outdir
-        pipen_outdir = Path(f"./{pipen_name}_results").resolve()
+        pipen_outdir = Path(f"./{pipen_name}-output").resolve()
         # The default workdir
         pipen_workdir = Path(f"./{config['workdir']}/{pipen_name}").resolve()
 
         # Update the name
         if parsed.name not in (None, pipen_name):
             pipen.name = parsed.name
 
@@ -92,15 +92,15 @@
         if pipen.outdir in (None, pipen_outdir):
             # The outdir is still some default values, that means it is not set
             # by higher priority (Pipen.outdir, or Pipen(outdir=...))
             # So we can use the value from arguments
             if parsed.outdir == pipen.outdir:
                 # if outdir is not passed from cli,
                 # use the name to infer the outdir
-                pipen.outdir = Path(f"./{pipen.name}_results").resolve()
+                pipen.outdir = Path(f"./{pipen.name}-output").resolve()
             else:
                 # otherwise, use it
                 pipen.outdir = parsed.outdir.resolve()
         elif parsed.outdir is not None and parsed.outdir != pipen.outdir:
             # The outdir is set by higher priority, and a value is passed by
             # arguments, so we need to warn the user that the value from
             # arguments will be ignored
```

### Comparing `pipen_args-0.9.6/pipen_args/procgroup.py` & `pipen_args-0.9.7/pipen_args/procgroup.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.9.6/pyproject.toml` & `pipen_args-0.9.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-args"
-version = "0.9.6"
+version = "0.9.7"
 description = "Command-line argument parser for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-args"
 repository = "https://github.com/pwwang/pipen-args"
```

### Comparing `pipen_args-0.9.6/setup.py` & `pipen_args-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['pipen-annotate>=0.7.1,<0.8.0']
 
 entry_points = \
 {'pipen': ['args = pipen_args.plugin:ArgsPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-args',
-    'version': '0.9.6',
+    'version': '0.9.7',
     'description': 'Command-line argument parser for pipen.',
-    'long_description': '# pipen-args\n\nCommand line argument parser for [pipen][1]\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n\n\nclass Process(Proc):\n    """My process\n\n    Input:\n        a: Input data\n    """\n    input = \'a\'\n    input_data = range(10)\n    script = \'echo {{in.a}}\'\n\nPipen().set_start(Process).run()\n```\n\n```shell\n$ python example.py --help\nUsage: test.py [-h | -h+] [options]\n\nUndescribed process.\nUse `@configfile` to load default values for the options.\n\nPipeline Options:\n  --name NAME           The name for the pipeline, will affect the default workdir and\n                        outdir. [default: pipen-0]\n  --profile PROFILE     The default profile from the configuration to run the pipeline.\n                        This profile will be used unless a profile is specified in the\n                        process or in the .run method of pipen. You can check the\n                        available profiles by running `pipen profile`\n  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>_results]\n  --forks FORKS         How many jobs to run simultaneously by the scheduler\n  --scheduler SCHEDULER\n                        The scheduler to run the jobs\n\nNamespace <in>:\n  --in.a A [A ...]      Input data\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n```\n\nSee more examples in `tests/pipelines/` folder.\n\n## Metadata for Proc envs items\n\nThe metadata in the docstring of env items determines how the arguments are defined.\n\n```python\nclass Process(Proc):\n    """My process\n\n    # other docstring sections\n\n    Envs:\n        a (<metadata>): ...\n    """\n```\n\nThe metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to\nseparate the key and value. The value is optional. If the value is not specified, it\nwill be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.\n\n[1]: https://github.com/pwwang/pipen\n',
+    'long_description': '# pipen-args\n\nCommand line argument parser for [pipen][1]\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n\n\nclass Process(Proc):\n    """My process\n\n    Input:\n        a: Input data\n    """\n    input = \'a\'\n    input_data = range(10)\n    script = \'echo {{in.a}}\'\n\nPipen().set_start(Process).run()\n```\n\n```shell\n$ python example.py --help\nUsage: test.py [-h | -h+] [options]\n\nUndescribed process.\nUse `@configfile` to load default values for the options.\n\nPipeline Options:\n  --name NAME           The name for the pipeline, will affect the default workdir and\n                        outdir. [default: pipen-0]\n  --profile PROFILE     The default profile from the configuration to run the pipeline.\n                        This profile will be used unless a profile is specified in the\n                        process or in the .run method of pipen. You can check the\n                        available profiles by running `pipen profile`\n  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>-output]\n  --forks FORKS         How many jobs to run simultaneously by the scheduler\n  --scheduler SCHEDULER\n                        The scheduler to run the jobs\n\nNamespace <in>:\n  --in.a A [A ...]      Input data\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n```\n\nSee more examples in `tests/pipelines/` folder.\n\n## Metadata for Proc envs items\n\nThe metadata in the docstring of env items determines how the arguments are defined.\n\n```python\nclass Process(Proc):\n    """My process\n\n    # other docstring sections\n\n    Envs:\n        a (<metadata>): ...\n    """\n```\n\nThe metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to\nseparate the key and value. The value is optional. If the value is not specified, it\nwill be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-args',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pipen_args-0.9.6/PKG-INFO` & `pipen_args-0.9.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-args
-Version: 0.9.6
+Version: 0.9.7
 Summary: Command-line argument parser for pipen.
 Home-page: https://github.com/pwwang/pipen-args
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -50,15 +50,15 @@
 Pipeline Options:
   --name NAME           The name for the pipeline, will affect the default workdir and
                         outdir. [default: pipen-0]
   --profile PROFILE     The default profile from the configuration to run the pipeline.
                         This profile will be used unless a profile is specified in the
                         process or in the .run method of pipen. You can check the
                         available profiles by running `pipen profile`
-  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>_results]
+  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>-output]
   --forks FORKS         How many jobs to run simultaneously by the scheduler
   --scheduler SCHEDULER
                         The scheduler to run the jobs
 
 Namespace <in>:
   --in.a A [A ...]      Input data
```

