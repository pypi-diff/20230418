# Comparing `tmp/sceptre-4.0.2.tar.gz` & `tmp/sceptre-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sceptre-4.0.2.tar", last modified: Mon Feb 20 15:17:30 2023, max compression
+gzip compressed data, was "sceptre-4.1.0.tar", last modified: Tue Apr 18 03:47:31 2023, max compression
```

## Comparing `sceptre-4.0.2.tar` & `sceptre-4.1.0.tar`

### file list

```diff
@@ -1,222 +1,231 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.696064 sceptre-4.0.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31009 2023-02-20 15:15:15.000000 sceptre-4.0.2/CHANGELOG.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7802 2023-02-20 15:15:15.000000 sceptre-4.0.2/CONTRIBUTING.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-02-20 15:15:15.000000 sceptre-4.0.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      361 2023-02-20 15:15:15.000000 sceptre-4.0.2/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)      127 2023-02-20 15:15:15.000000 sceptre-4.0.2/NOTICE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11167 2023-02-20 15:17:30.696064 sceptre-4.0.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10458 2023-02-20 15:15:15.000000 sceptre-4.0.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.652064 sceptre-4.0.2/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/Makefile
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.656064 sceptre-4.0.2/docs/_source/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1794 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/about.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.656064 sceptre-4.0.2/docs/_source/apidoc/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/apidoc/modules.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2044 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/apidoc/sceptre.cli.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      632 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/apidoc/sceptre.config.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      510 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/apidoc/sceptre.diffing.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      499 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/apidoc/sceptre.hooks.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      602 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/apidoc/sceptre.plan.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      746 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/apidoc/sceptre.resolvers.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1489 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/apidoc/sceptre.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6615 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/conf.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.660064 sceptre-4.0.2/docs/_source/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4039 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/architecture.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3359 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/cli.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8177 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/faq.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5011 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/get_started.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6100 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/hooks.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1847 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/install.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9931 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/permissions.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13541 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/resolvers.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23726 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/stack_config.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14126 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/stack_group_config.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7056 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/template_handlers.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8179 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/templates.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3406 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/docs/terminology.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      656 2023-02-20 15:15:15.000000 sceptre-4.0.2/docs/_source/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1113 2023-02-20 15:15:15.000000 sceptre-4.0.2/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.660064 sceptre-4.0.2/requirements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      315 2023-02-20 15:15:15.000000 sceptre-4.0.2/requirements/prod.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.664064 sceptre-4.0.2/sceptre/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.668064 sceptre-4.0.2/sceptre/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3188 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1877 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/create.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2115 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/delete.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/describe.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7349 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/diff.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3297 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/drift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1493 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/dump.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1441 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/execute.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13964 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7611 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/launch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4357 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/list.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/new.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1366 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/policy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6488 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/prune.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/status.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5153 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3152 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/cli/update.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.668064 sceptre-4.0.2/sceptre/config/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/config/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3318 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/config/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23297 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/config/reader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1450 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/config/strategies.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21662 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/connection_manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4767 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/context.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.668064 sceptre-4.0.2/sceptre/diffing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/diffing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8016 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/diffing/diff_writer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18981 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/diffing/stack_differ.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3959 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6579 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/helpers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.668064 sceptre-4.0.2/sceptre/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3243 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3268 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/hooks/asg_scaling_processes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/hooks/cmd.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.672064 sceptre-4.0.2/sceptre/plan/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/plan/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39889 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/plan/actions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/plan/executor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13822 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/plan/plan.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.672064 sceptre-4.0.2/sceptre/resolvers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16192 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/resolvers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      676 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/resolvers/environment_variable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/resolvers/file_contents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/resolvers/no_value.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3813 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/resolvers/placeholders.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2074 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/resolvers/stack_attr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5990 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/resolvers/stack_output.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18051 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/stack.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.672064 sceptre-4.0.2/sceptre/stack_policies/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/stack_policies/lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/stack_policies/unlock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/stack_status.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2382 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/stack_status_colourer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8776 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.672064 sceptre-4.0.2/sceptre/template_handlers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2864 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/template_handlers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2305 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/template_handlers/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4800 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/template_handlers/helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5040 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/template_handlers/http.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3264 2023-02-20 15:15:15.000000 sceptre-4.0.2/sceptre/template_handlers/s3.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.664064 sceptre-4.0.2/sceptre.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11167 2023-02-20 15:17:30.000000 sceptre-4.0.2/sceptre.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5953 2023-02-20 15:17:30.000000 sceptre-4.0.2/sceptre.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-20 15:17:30.000000 sceptre-4.0.2/sceptre.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      716 2023-02-20 15:17:30.000000 sceptre-4.0.2/sceptre.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-20 15:17:30.000000 sceptre-4.0.2/sceptre.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-02-20 15:17:30.000000 sceptre-4.0.2/sceptre.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-02-20 15:17:30.000000 sceptre-4.0.2/sceptre.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      432 2023-02-20 15:17:30.700064 sceptre-4.0.2/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3429 2023-02-20 15:15:15.000000 sceptre-4.0.2/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.676064 sceptre-4.0.2/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.652064 sceptre-4.0.2/tests/fixtures/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.684064 sceptre-4.0.2/tests/fixtures/config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.652064 sceptre-4.0.2/tests/fixtures/config/account/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.684064 sceptre-4.0.2/tests/fixtures/config/account/stack-group/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/config/account/stack-group/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.684064 sceptre-4.0.2/tests/fixtures/config/account/stack-group/region/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/config/account/stack-group/region/config.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/config/account/stack-group/region/construct_nodes.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      293 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/config/account/stack-group/region/security_groups.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/config/account/stack-group/region/subnets.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       91 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/config/account/stack-group/region/vpc.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/config/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.684064 sceptre-4.0.2/tests/fixtures/config/top/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/config/top/level.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.684064 sceptre-4.0.2/tests/fixtures/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/hooks/custom_hook.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.684064 sceptre-4.0.2/tests/fixtures/resolvers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/resolvers/custom_resolver.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.688063 sceptre-4.0.2/tests/fixtures/stack_policies/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/stack_policies/lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/stack_policies/unlock.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.692064 sceptre-4.0.2/tests/fixtures/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/chdir.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/compiled_vpc.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/compiled_vpc.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/compiled_vpc_sud.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/sg.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc.template
--rw-r--r--   0 circleci  (1001) circleci  (1002)      589 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc.without_start_marker.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc.yaml.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc_sgt.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      825 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc_sud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc_sud_incorrect_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc_sud_incorrect_handler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      837 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures/templates/vpc_t.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.652064 sceptre-4.0.2/tests/fixtures-vpc/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.676064 sceptre-4.0.2/tests/fixtures-vpc/config/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.652064 sceptre-4.0.2/tests/fixtures-vpc/config/account/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.676064 sceptre-4.0.2/tests/fixtures-vpc/config/account/stack-group/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/config/account/stack-group/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.680064 sceptre-4.0.2/tests/fixtures-vpc/config/account/stack-group/region/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/config/account/stack-group/region/config.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/config/account/stack-group/region/vpc.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/config/config.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.680064 sceptre-4.0.2/tests/fixtures-vpc/config/top/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/config/top/level.yaml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.680064 sceptre-4.0.2/tests/fixtures-vpc/hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/hooks/custom_hook.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.680064 sceptre-4.0.2/tests/fixtures-vpc/resolvers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/resolvers/custom_resolver.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.680064 sceptre-4.0.2/tests/fixtures-vpc/stack_policies/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/stack_policies/lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/stack_policies/unlock.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.684064 sceptre-4.0.2/tests/fixtures-vpc/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/compiled_vpc.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/compiled_vpc_sud.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/sg.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc.template
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc.yaml.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc_sgt.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      825 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc_sud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc_sud_incorrect_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc_sud_incorrect_handler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      837 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/fixtures-vpc/templates/vpc_t.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    59434 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_actions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.692064 sceptre-4.0.2/tests/test_cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    40000 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_cli/test_cli_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7929 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_cli/test_launch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7424 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_cli/test_prune.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20760 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_config_reader.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32490 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_connection_manager.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3854 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_context.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.692064 sceptre-4.0.2/tests/test_diffing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_diffing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14190 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_diffing/test_diff_writer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_diffing/test_stack_differ.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6111 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_helpers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.696064 sceptre-4.0.2/tests/test_hooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_hooks/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5290 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_hooks/test_asg_scaling_processes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1226 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_hooks/test_cmd.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2580 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_hooks/test_hooks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2622 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_plan.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.696064 sceptre-4.0.2/tests/test_resolvers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_resolvers/test_environment_variable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_resolvers/test_file_contents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2690 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_resolvers/test_placeholders.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19669 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_resolvers/test_resolver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1996 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_resolvers/test_stack_attr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10392 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_resolvers/test_stack_output.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12911 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_stack.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2245 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_stack_status_colourer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13844 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_template.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-20 15:17:30.696064 sceptre-4.0.2/tests/test_template_handlers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4064 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_template_handlers/test_file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3226 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_template_handlers/test_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4661 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_template_handlers/test_http.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4453 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_template_handlers/test_s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1017 2023-02-20 15:15:15.000000 sceptre-4.0.2/tests/test_template_handlers/test_template_handlers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.221266 sceptre-4.1.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31379 2023-04-18 03:45:00.000000 sceptre-4.1.0/CHANGELOG.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7802 2023-04-18 03:45:00.000000 sceptre-4.1.0/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-04-18 03:45:00.000000 sceptre-4.1.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      361 2023-04-18 03:45:00.000000 sceptre-4.1.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      127 2023-04-18 03:45:00.000000 sceptre-4.1.0/NOTICE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11167 2023-04-18 03:47:31.221266 sceptre-4.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10458 2023-04-18 03:45:00.000000 sceptre-4.1.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.193266 sceptre-4.1.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/Makefile
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.193266 sceptre-4.1.0/docs/_source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1794 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/about.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.197265 sceptre-4.1.0/docs/_source/apidoc/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/modules.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2044 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.cli.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      632 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.config.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      510 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.diffing.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      499 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.hooks.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      602 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.plan.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      746 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.resolvers.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1489 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/apidoc/sceptre.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6615 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/conf.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.197265 sceptre-4.1.0/docs/_source/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4039 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/architecture.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3359 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/cli.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8177 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/faq.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5011 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/get_started.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6231 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/hooks.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1847 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/install.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9931 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/permissions.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18998 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/resolvers.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24147 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/stack_config.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14126 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/stack_group_config.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7056 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/template_handlers.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8179 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/templates.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3406 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/docs/terminology.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      656 2023-04-18 03:45:00.000000 sceptre-4.1.0/docs/_source/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1113 2023-04-18 03:45:00.000000 sceptre-4.1.0/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.197265 sceptre-4.1.0/requirements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      315 2023-04-18 03:45:00.000000 sceptre-4.1.0/requirements/prod.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.197265 sceptre-4.1.0/sceptre/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      568 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.201265 sceptre-4.1.0/sceptre/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3188 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1877 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/create.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2115 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/delete.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/describe.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7349 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/diff.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3297 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/drift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1493 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/dump.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1441 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/execute.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13964 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7611 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/launch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4357 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/list.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/new.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1366 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/policy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6488 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/prune.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1162 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/status.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5153 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3152 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/cli/update.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.201265 sceptre-4.1.0/sceptre/config/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/config/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3318 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/config/graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23298 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/config/reader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1450 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/config/strategies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21662 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/connection_manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4767 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/context.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.205266 sceptre-4.1.0/sceptre/diffing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/diffing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8016 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/diffing/diff_writer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18981 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/diffing/stack_differ.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4089 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7540 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/helpers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.205266 sceptre-4.1.0/sceptre/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2914 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3268 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/hooks/asg_scaling_processes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/hooks/cmd.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/logging.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.205266 sceptre-4.1.0/sceptre/plan/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      408 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/plan/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    39889 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/plan/actions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1972 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/plan/executor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13822 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/plan/plan.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.205266 sceptre-4.1.0/sceptre/resolvers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20784 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      676 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/environment_variable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/file_contents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1303 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/join.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/no_value.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3622 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/placeholders.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1855 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/select.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1312 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/split.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2074 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/stack_attr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5962 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/stack_output.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1784 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/resolvers/sub.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18051 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/stack.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/sceptre/stack_policies/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/stack_policies/lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/stack_policies/unlock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      539 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/stack_status.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2382 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/stack_status_colourer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8848 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/sceptre/template_handlers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2937 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template_handlers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2305 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template_handlers/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4800 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template_handlers/helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5040 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template_handlers/http.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3267 2023-04-18 03:45:00.000000 sceptre-4.1.0/sceptre/template_handlers/s3.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.201265 sceptre-4.1.0/sceptre.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11167 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6216 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      862 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-04-18 03:47:31.000000 sceptre-4.1.0/sceptre.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      432 2023-04-18 03:47:31.221266 sceptre-4.1.0/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3635 2023-04-18 03:45:00.000000 sceptre-4.1.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.193266 sceptre-4.1.0/tests/fixtures/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.193266 sceptre-4.1.0/tests/fixtures/config/account/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/config/account/stack-group/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/config.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      279 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/construct_nodes.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      293 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/security_groups.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/subnets.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       91 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/account/stack-group/region/vpc.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/config/top/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/config/top/level.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/hooks/custom_hook.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/resolvers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/resolvers/custom_resolver.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures/stack_policies/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/stack_policies/lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/stack_policies/unlock.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.217266 sceptre-4.1.0/tests/fixtures/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/chdir.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/compiled_vpc.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/compiled_vpc.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/compiled_vpc_sud.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/sg.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.template
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      589 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.without_start_marker.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc.yaml.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc_sgt.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      825 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc_sud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc_sud_incorrect_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc_sud_incorrect_handler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      837 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures/templates/vpc_t.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.193266 sceptre-4.1.0/tests/fixtures-vpc/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/config/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.189265 sceptre-4.1.0/tests/fixtures-vpc/config/account/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/config/account/stack-group/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/config/account/stack-group/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/config/account/stack-group/region/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/config/account/stack-group/region/config.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/config/account/stack-group/region/vpc.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      108 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/config/config.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/config/top/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       35 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/config/top/level.yaml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/hooks/custom_hook.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/resolvers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      223 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/resolvers/custom_resolver.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.209266 sceptre-4.1.0/tests/fixtures-vpc/stack_policies/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/stack_policies/lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      140 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/stack_policies/unlock.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.213266 sceptre-4.1.0/tests/fixtures-vpc/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/compiled_vpc.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/compiled_vpc_sud.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/sg.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1093 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.template
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      150 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.yaml.j2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1560 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_sgt.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      825 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_sud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_sud_incorrect_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_sud_incorrect_handler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      837 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_t.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    59434 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_actions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.217266 sceptre-4.1.0/tests/test_cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    40000 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_cli/test_cli_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7929 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_cli/test_launch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7424 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_cli/test_prune.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20760 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_config_reader.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32490 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_connection_manager.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3854 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_context.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.217266 sceptre-4.1.0/tests/test_diffing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_diffing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14190 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_diffing/test_diff_writer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_diffing/test_stack_differ.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6911 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_helpers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.217266 sceptre-4.1.0/tests/test_hooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_hooks/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5332 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_hooks/test_asg_scaling_processes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1268 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_hooks/test_cmd.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3199 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_hooks/test_hooks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2622 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_plan.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.221266 sceptre-4.1.0/tests/test_resolvers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_environment_variable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1008 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_file_contents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2106 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_join.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_placeholders.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25717 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_resolver.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2308 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_select.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1100 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_split.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2038 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_stack_attr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10626 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_stack_output.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1624 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_resolvers/test_sub.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12911 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_stack.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2245 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_stack_status_colourer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13844 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 03:47:31.221266 sceptre-4.1.0/tests/test_template_handlers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4064 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template_handlers/test_file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3226 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template_handlers/test_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4661 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template_handlers/test_http.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4453 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template_handlers/test_s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1456 2023-04-18 03:45:00.000000 sceptre-4.1.0/tests/test_template_handlers/test_template_handlers.py
```

### Comparing `sceptre-4.0.2/CHANGELOG.md` & `sceptre-4.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # CHANGELOG
 
 Categories: Added, Removed, Changed, Fixed, Nonfunctional, Deprecated
 
 ## Unreleased
 
+## 4.1.0 (2023.04.17)
+### Added
+ - [Resolve #1304] Adding StackLoggerAdapter to hooks, resolvers, and template handler
+ - [Resolve #1263] Stack output caching
+ - [Resolve #1252] Supporting resolvers in Hook and Resolver arguments, with new
+   !substitute, !join, !split, and !select resolvers!
+
+### Nonfunctional
+ - add a pre-commit linter to validate circleci configs
+
 ## 4.0.2 (2023.02.20)
 ### Fixed
  - [Resolve #1307] Fixing Connection Manager bug (#1308)
 
 ## 4.0.1 (2023.02.12)
 
 ### Changed
```

### Comparing `sceptre-4.0.2/CONTRIBUTING.md` & `sceptre-4.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/LICENSE` & `sceptre-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/PKG-INFO` & `sceptre-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sceptre
-Version: 4.0.2
+Version: 4.1.0
 Summary: Cloud Provisioning Tool
 Home-page: https://github.com/Sceptre/sceptre
 Author: Cloudreach
 Author-email: sceptre@cloudreach.com
 License: Apache2
 Keywords: sceptre
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sceptre-4.0.2/README.md` & `sceptre-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/Makefile` & `sceptre-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/about.rst` & `sceptre-4.1.0/docs/_source/about.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/apidoc/sceptre.cli.rst` & `sceptre-4.1.0/docs/_source/apidoc/sceptre.cli.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/apidoc/sceptre.config.rst` & `sceptre-4.1.0/docs/_source/apidoc/sceptre.config.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/apidoc/sceptre.plan.rst` & `sceptre-4.1.0/docs/_source/apidoc/sceptre.plan.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/apidoc/sceptre.resolvers.rst` & `sceptre-4.1.0/docs/_source/apidoc/sceptre.resolvers.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/apidoc/sceptre.rst` & `sceptre-4.1.0/docs/_source/apidoc/sceptre.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/conf.py` & `sceptre-4.1.0/docs/_source/conf.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/docs/architecture.rst` & `sceptre-4.1.0/docs/_source/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/docs/cli.rst` & `sceptre-4.1.0/docs/_source/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/docs/faq.rst` & `sceptre-4.1.0/docs/_source/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/docs/get_started.rst` & `sceptre-4.1.0/docs/_source/docs/get_started.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/docs/hooks.rst` & `sceptre-4.1.0/docs/_source/docs/hooks.rst`

 * *Files 8% similar despite different names*

```diff
@@ -203,15 +203,17 @@
      type: <...>
    hooks:
      before_create:
        - !custom_hook_command_name <argument> # The argument is accessible via self.argument
 
 hook arguments
 ^^^^^^^^^^^^^^
-Hook arguments can be a simple string or a complex data structure.
+Hook arguments can be a simple string or a complex data structure. You can even use resolvers in
+hook arguments, so long as they're nested in a list or a dict.
+
 Assume a Sceptre `copy` hook that calls the `cp command`_:
 
 .. code-block:: yaml
 
    template:
      path: <...>
      type: <...>
@@ -220,15 +222,15 @@
        - !copy "-r from_dir to_dir"
      before_update:
        - !copy {"options":"-r", "source": "from_dir", "destination": "to_dir"}
      after_update:
        - !copy
            options: "-r"
            source: "from_dir"
-           destination: "to_dir"
+           destination: !stack_output my/other/stack::CopyDestination
 
 .. _Custom Hooks: #custom-hooks
 .. _subprocess documentation: https://docs.python.org/3/library/subprocess.html
 .. _documentation: http://docs.aws.amazon.com/autoscaling/latest/userguide/as-suspend-resume-processes.html
 .. _this is great place to start: https://docs.python.org/3/distributing/
 .. _cp command: http://man7.org/linux/man-pages/man1/cp.1.html
```

### Comparing `sceptre-4.0.2/docs/_source/docs/install.rst` & `sceptre-4.1.0/docs/_source/docs/install.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/docs/permissions.rst` & `sceptre-4.1.0/docs/_source/docs/permissions.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/docs/resolvers.rst` & `sceptre-4.1.0/docs/_source/docs/resolvers.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Resolvers
 =========
 
 Sceptre implements resolvers, which can be used to resolve a value of a
 CloudFormation ``parameter`` or ``sceptre_user_data`` value at runtime. This is
 most commonly used to chain the outputs of one Stack to the inputs of another.
 
+You can use resolvers with any resolvable property on a StackConfig, as well as in the arguments
+of hooks and other resolvers.
+
 If required, users can create their own resolvers, as described in the section
 on `Custom Resolvers`_.
 
 Syntax:
 
 .. code-block:: yaml
 
@@ -48,14 +51,35 @@
 Refer to `sceptre-file-resolver <https://github.com/Sceptre/sceptre-file-resolver/>`_ for documentation.
 
 file_contents
 ~~~~~~~~~~~~~
 
 **deprecated**: Consider using the `file`_ resolver instead.
 
+join
+~~~~
+
+This resolver allows you to join multiple strings together to form a single string. This is great
+for combining the outputs of multiple resolvers. This resolver works just like CloudFormation's
+``!Join`` intrinsic function.
+
+The argument for this resolver should be a list with two elements: (1) A string to join the elements
+on and (2) a list of items to join.
+
+Example:
+
+.. code-block:: yaml
+
+   parameters:
+     BaseUrl: !join
+       - ":"
+       - - !stack_output my/app/stack.yaml::HostName
+         - !stack_output my/other/stack.yaml::Port
+
+
 no_value
 ~~~~~~~~
 
 This resolver "resolves to nothing", functioning just as if it was not set at all. This works just
 like the "AWS::NoValue" special variable that you can reference on a CloudFormation template. It
 can help simplify Stack and StackGroup config Jinja logic in cases where, if a condition is met, a
 value is passed, otherwise no value is passed.
@@ -75,14 +99,56 @@
 rcmd
 ~~~~
 
 A resolver to execute any shell command.
 
 Refer to `sceptre-resolver-cmd <https://github.com/Sceptre/sceptre-resolver-cmd/>`_ for documentation.
 
+select
+~~~~~~
+
+This resolver allows you to select a specific index of a list of items. This is great for combining
+with the ``!split`` resolver to obtain part of a string. This function works almost the same as
+CloudFormation's ``!Select`` intrinsic function, **except you can use this with negative indices to
+select from the end of a list**.
+
+The argument for this resolver should be a list with two elements: (1) A numerical index and (2) a
+list of items to select out of. If the index is negative, it will select from the end of the list.
+For example, "-1" would select the last element and "-2" would select the second-to-last element.
+
+Example:
+
+.. code-block:: yaml
+
+   sceptre_user_data:
+     # This selects the last element after you split the connection string on "/"
+     DatabaseName: !select
+       - -1
+       - !split ["/", !stack_output my/database/stack.yaml::ConnectionString]
+
+split
+~~~~~
+
+This resolver will split a value on a given delimiter string. This is great when combining with the
+``!select`` resolver. This function works the same as CloudFormation's ``!Split`` intrinsic function.
+
+Note: The return value of this resolver is a *list*, not a string. This will not work to set Stack
+configurations that expect strings, but it WILL work to set Stack configurations that expect lists.
+
+The argument for this resolver should be a list with two elements: (1) The delimiter to split on and
+(2) a string to split.
+
+Example:
+
+.. code-block:: yaml
+
+   notifications: !split
+     - ";"
+     - !stack_output my/sns/topics.yaml::SemicolonDelimitedArns
+
 .. _stack_attr_resolver:
 
 stack_attr
 ~~~~~~~~~~
 
 This resolver resolves to the values of other fields on the same Stack Config or those
 inherited from StackGroups in which the current Stack Config exists, even when those other fields are
@@ -177,14 +243,75 @@
 Example:
 
 .. code-block:: yaml
 
    parameters:
      VpcIdParameter: !stack_output_external prj-network-vpc::VpcIdOutput prod
 
+
+sub
+~~~
+
+This resolver allows you to create a string using Python string format syntax. This functions as a
+great way to combine together a number of resolver outputs into a single string. This functions
+similarly to Cloudformation's ``!Sub`` intrinsic function.
+
+It should be noted that Jinja2 syntax is far more capable of interpolating values than this resolver,
+so you should use Jinja2 if all you need is to interpolate raw values from environment variables,
+variables from stack group configs, var files, and ``--var`` arguments. **The one thing that Jinja2
+interpolation can't do is interpolate resolver arguments into a string.** And that's what ``!sub``
+can do. For more information on why Jinja2 can't reference resolvers directly, see
+:ref:`resolution_order`.
+
+The argument to this resolver should be a two-element list: (1) Is the format string, using
+curly-brace templates to indicate variables, and (2) a dictionary where the keys are the format
+string's variable names and the values are the variable values.
+
+Example:
+
+.. code-block:: yaml
+
+   parameters:
+     ConnectionString: !sub
+       - "postgres://{username}:{password}@{hostname}:{port}/{database}"
+       # Notice how we're interpolating a username and database via Jinja2? Technically it's not
+       # necessary to pass them this way. They could be interpolated directly. But it might be
+       # easier to read this way if you pass them explicitly like this. See example below for the
+       # other way this can be done.
+       - username: {{ var.username }}
+         password: !ssm /my/ssm/password
+         hostname: !stack_output my/database/stack.yaml::HostName
+         port: !stack_output my/database/stack.yaml::Port
+         database: {{var.database}}
+
+
+It's relevant to note that this functions similarly to the *more verbose* form of CloudFormation's
+``!Sub`` intrinsic function, where you use a list argument and supply the interpolated values as a
+second list item in a dictionary. **Important**: Sceptre's ``!sub`` resolver will not work without
+a list argument. It does **not** directly reference variables without you directly passing them
+in the second list item in its argument.
+
+You *can* combine Jinja2 syntax with this resolver if you want to interpolate in other variables
+that Jinja2 has access to.
+
+Example:
+
+.. code-block:: yaml
+
+   parameters:
+     ConnectionString: !sub
+       # Notice the double-curly braces. That's Jinja2 syntax. Jinja2 will render the username into
+       # the string even before the yaml is loaded. If you use Jinja2 to interpolate the value, then
+       # it's not a template string variable you need to pass in the second list item passed to
+       # !sub.
+       - "postgres://{{ var.username }}:{password}@{hostname}:{port}/{{ stack_group_config.database }}"
+       - password: !ssm /my/ssm/password
+         hostname: !stack_output my/database/stack.yaml::HostName
+         port: !stack_output my/database/stack.yaml::Port
+
 Custom Resolvers
 ----------------
 
 Users can define their own resolvers which are used by Sceptre to resolve the
 value of a parameter before it is passed to the CloudFormation template.
 
 A resolver is a Python class which inherits from abstract base class
@@ -302,26 +429,30 @@
 
 For details on calling AWS services or invoking AWS-related third party tools in your resolver, see
 :ref:`using_connection_manager`
 
 
 Resolver arguments
 ^^^^^^^^^^^^^^^^^^
-Resolver arguments can be a simple string or a complex data structure.
+Resolver arguments can be a simple string or a complex data structure. You can even use
+other resolvers in the arguments to resolvers! (Note: Other resolvers can only be passed in
+arguments when they're passed in lists and dicts.)
 
 .. code-block:: yaml
 
    template:
      path: <...>
      type: <...>
-    parameters:
-      Param1: !ssm "/dev/DbPassword"
-      Param2: !ssm {"name": "/dev/DbPassword"}
-      Param3: !ssm
-        name: "/dev/DbPassword"
+   parameters:
+     Param1: !ssm "/dev/DbPassword"
+     Param2: !ssm {"name": "/dev/DbPassword"}
+     Param3: !ssm
+       name: "/dev/DbPassword"
+     Param4: !ssm
+       name: !stack_output my/other/stack.yaml::MySsmParameterName
 
 .. _Custom Resolvers: #custom-resolvers
 .. _this is great place to start: https://docs.python.org/3/distributing/
 
 Resolving to nothing
 ^^^^^^^^^^^^^^^^^^^^
 When a resolver returns ``None``, this means that it resolves to "nothing". For resolvers set for
```

### Comparing `sceptre-4.0.2/docs/_source/docs/stack_config.rst` & `sceptre-4.1.0/docs/_source/docs/stack_config.rst`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
    "inherited" by every stack within that StackGroup. If one of those dependencies *inherits* that
    list of dependencies, it will cause a circular dependency. If this happens, you can resolve the
    situation by either (a) setting those ``dependencies`` on individual Stack Configs rather than the
    the StackGroup Config, or (b) moving those dependency stacks outside of the StackGroup.
 
 hooks
 ~~~~~
-* Resolvable: No
+* Resolvable: No (but you can use resolvers _in_ hook arguments!)
 * Can be inherited from StackGroup: Yes
 * Inheritance strategy: Overrides parent if set
 
 A list of arbitrary shell or Python commands or scripts to run. Find out more
 in the :doc:`hooks` section.
 
 ignore
@@ -552,24 +552,30 @@
 
 "Render Time" vs. "Resolve Time"
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 A common point of confusion tends to be around the distinction between **"render time"** (phase 3, when
 Jinja logic is applied) and **"resolve time"** (phase 6, when resolvers are resolved). You cannot use
 a resolver via Jinja during "render time", since the resolver won't exist or be ready to use yet. You can,
-however, use Jinja logic to indicate *whether*, *which*, or *how* a resolver is configured.
+however, use Jinja logic to indicate *whether*, *which*, or *how* a resolver is configured. You can
+also use resolvers like ``!sub`` to interpolate resolved values when Jinja isn't available.
 
 For example, you **can** do something like this:
 
 .. code-block:: yaml
 
    parameters:
      {% if var.use_my_parameter %}
        my_parameter: !stack_output {{ var.stack_name }}::{{ var.output_name }}
      {% endif %}
+       # !sub will let you combine outputs of multiple resolvers into a single string
+       my_combined_parameter: !sub
+         - "{fist_part} - {second_part}"
+         - first_part: !stack_output my/stack/name.yaml::Output
+         - second_part: {{ var.second_part }}
 
 Accessing resolved values in other fields
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Sometimes you might want to reference the resolved value of one field in another field. Since you cannot
 use Jinja to access resolved values, there is another way to this. The :ref:`stack_attr_resolver`
 resolver is meant for addressing just this need. It's a resolver that will resolve to the value of
```

### Comparing `sceptre-4.0.2/docs/_source/docs/stack_group_config.rst` & `sceptre-4.1.0/docs/_source/docs/stack_group_config.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/docs/template_handlers.rst` & `sceptre-4.1.0/docs/_source/docs/template_handlers.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/docs/templates.rst` & `sceptre-4.1.0/docs/_source/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/docs/terminology.rst` & `sceptre-4.1.0/docs/_source/docs/terminology.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/docs/_source/index.rst` & `sceptre-4.1.0/docs/_source/index.rst`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/pyproject.toml` & `sceptre-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/__init__.py` & `sceptre-4.1.0/sceptre/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import sys
 import warnings
 
 
 __author__ = "Cloudreach"
 __email__ = "sceptre@cloudreach.com"
-__version__ = "4.0.2"
+__version__ = "4.1.0"
 
 
 # Set up logging to ``/dev/null`` like a library is supposed to.
 # http://docs.python.org/3.3/howto/logging.html#configuring-logging-for-a-library
 class NullHandler(logging.Handler):  # pragma: no cover
     def emit(self, record):
         pass
```

### Comparing `sceptre-4.0.2/sceptre/cli/__init__.py` & `sceptre-4.1.0/sceptre/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/create.py` & `sceptre-4.1.0/sceptre/cli/create.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/delete.py` & `sceptre-4.1.0/sceptre/cli/delete.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/describe.py` & `sceptre-4.1.0/sceptre/cli/describe.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/diff.py` & `sceptre-4.1.0/sceptre/cli/diff.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/drift.py` & `sceptre-4.1.0/sceptre/cli/drift.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/dump.py` & `sceptre-4.1.0/sceptre/cli/dump.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/execute.py` & `sceptre-4.1.0/sceptre/cli/execute.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/helpers.py` & `sceptre-4.1.0/sceptre/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/launch.py` & `sceptre-4.1.0/sceptre/cli/launch.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/list.py` & `sceptre-4.1.0/sceptre/cli/list.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/new.py` & `sceptre-4.1.0/sceptre/cli/new.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/policy.py` & `sceptre-4.1.0/sceptre/cli/policy.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/prune.py` & `sceptre-4.1.0/sceptre/cli/prune.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/status.py` & `sceptre-4.1.0/sceptre/cli/status.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/template.py` & `sceptre-4.1.0/sceptre/cli/template.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/cli/update.py` & `sceptre-4.1.0/sceptre/cli/update.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/config/graph.py` & `sceptre-4.1.0/sceptre/config/graph.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/config/reader.py` & `sceptre-4.1.0/sceptre/config/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
             :param node_class: Class representing the node.
             :type node_class: class
             :returns: Class initialiser.
             :rtype: func
             """
 
-            # This function signture is required by PyYAML
+            # This function signature is required by PyYAML
             def class_constructor(loader, node):
                 return node_class(
                     loader.construct_object(self.resolve_node_tag(loader, node))
                 )  # pragma: no cover
 
             return class_constructor
```

### Comparing `sceptre-4.0.2/sceptre/config/strategies.py` & `sceptre-4.1.0/sceptre/config/strategies.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/connection_manager.py` & `sceptre-4.1.0/sceptre/connection_manager.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/context.py` & `sceptre-4.1.0/sceptre/context.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/diffing/diff_writer.py` & `sceptre-4.1.0/sceptre/diffing/diff_writer.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/diffing/stack_differ.py` & `sceptre-4.1.0/sceptre/diffing/stack_differ.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/exceptions.py` & `sceptre-4.1.0/sceptre/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -215,7 +215,13 @@
 
 
 class CannotPruneStackError(SceptreException):
     """
     Error raised when an obsolete stack cannot be pruned because another stack depends on it that is
     not itself obsolete.
     """
+
+
+class InvalidResolverArgumentError(SceptreException):
+    """
+    Indicates a resolver argument is invalid in some way.
+    """
```

### Comparing `sceptre-4.0.2/sceptre/helpers.py` & `sceptre-4.1.0/sceptre/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from contextlib import contextmanager
 from datetime import datetime
 from os import sep
-from typing import Optional, Any, List
+from typing import Optional, Any, List, Tuple, Union
 
 import dateutil.parser
 import deprecation
 
 from sceptre.exceptions import PathConversionError
 from sceptre import __version__
 
@@ -64,14 +64,36 @@
             func_on_instance(key)
     elif isinstance(attr, list):
         for index, value in enumerate(attr):
             func_on_instance(index)
     return attr
 
 
+Container = Union[list, dict]
+Key = Union[str, int]
+
+
+def delete_keys_from_containers(keys_to_delete: List[Tuple[Container, Key]]):
+    """Removes the indicated keys/indexes from their paired containers."""
+    list_items_to_delete = []
+    for container, key in keys_to_delete:
+        if isinstance(container, list):
+            # If it's a list, we want to gather up the items to remove from the list.
+            # We don't want to modify the list length yet, since removals will change all the other
+            # list indexes. Instead, we'll get the actual items at those indexes to remove later.
+            list_items_to_delete.append((container, container[key]))
+        else:
+            del container[key]
+
+    # Finally, now that we have all the items we want to remove the lists, we'll remove those
+    # items specifically from the lists.
+    for containing_list, item in list_items_to_delete:
+        containing_list.remove(item)
+
+
 def normalise_path(path):
     """
     Converts a path to use correct path separator.
     Raises an PathConversionError if the path has a
     trailing slash.
     :param path: A directory path
     :type path: str
```

### Comparing `sceptre-4.0.2/sceptre/hooks/__init__.py` & `sceptre-4.1.0/sceptre/hooks/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,25 @@
 import abc
 import logging
 from functools import wraps
+from typing import TYPE_CHECKING
 
 from sceptre.helpers import _call_func_on_values
+from sceptre.resolvers import CustomYamlTagBase
 
+if TYPE_CHECKING:
+    from sceptre.stack import Stack
 
-class Hook(object):
-    """
-    Hook is an abstract base class that should be inherited by all hooks.
 
-    :param argument: The argument of the hook.
-    :type argument: str
-    :param stack: The associated stack of the hook.
-    :type stack: sceptre.stack.Stack
+class Hook(CustomYamlTagBase, metaclass=abc.ABCMeta):
+    """
+    Hook is an abstract base class that should be subclassed by all hooks.
     """
 
-    __metaclass__ = abc.ABCMeta
-
-    def __init__(self, argument=None, stack=None):
-        self.logger = logging.getLogger(__name__)
-        self.argument = argument
-        self.stack = stack
-
-    def setup(self):
-        """
-        setup is a method that may be overwritten by inheriting classes. Allows
-        hooks to run so initalisation steps when config is first read.
-        """
-        pass  # pragma: no cover
+    logger = logging.getLogger(__name__)
 
     @abc.abstractmethod
     def run(self):
         """
         run is an abstract method which must be overwritten by all
         inheriting classes. Run should execute the logic of the hook.
         """
@@ -57,24 +45,24 @@
         Attribute getter for Hook containing data structure.
 
         :return: The attribute stored with the suffix ``name`` in the instance.
         :rtype: dict or list
         """
         return getattr(instance, self.name)
 
-    def __set__(self, instance, value):
+    def __set__(self, instance: "Stack", value):
         """
         Attribute setter which adds a stack reference to any hooks in the
         data structure `value` and calls the setup method.
 
         """
 
-        def setup(attr, key, value):
-            value.stack = instance
-            value.setup()
+        def setup(attr, key, value: Hook):
+            attr[key] = clone = value.clone_for_stack(instance)
+            clone.setup()
 
         _call_func_on_values(setup, value, Hook)
         setattr(instance, self.name, value)
 
 
 def execute_hooks(hooks):
     """
```

### Comparing `sceptre-4.0.2/sceptre/hooks/asg_scaling_processes.py` & `sceptre-4.1.0/sceptre/hooks/asg_scaling_processes.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/hooks/cmd.py` & `sceptre-4.1.0/sceptre/hooks/cmd.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/plan/actions.py` & `sceptre-4.1.0/sceptre/plan/actions.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/plan/executor.py` & `sceptre-4.1.0/sceptre/plan/executor.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/plan/plan.py` & `sceptre-4.1.0/sceptre/plan/plan.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/resolvers/__init__.py` & `sceptre-4.1.0/sceptre/resolvers/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,206 @@
 # -*- coding: utf-8 -*-
 import abc
 import logging
 from contextlib import contextmanager
 from threading import RLock
 from typing import Any, TYPE_CHECKING, Type, Union, TypeVar
 
-from sceptre.helpers import _call_func_on_values
+from sceptre.exceptions import InvalidResolverArgumentError
+from sceptre.helpers import _call_func_on_values, delete_keys_from_containers
+from sceptre.logging import StackLoggerAdapter
 from sceptre.resolvers.placeholders import (
     create_placeholder_value,
     are_placeholders_enabled,
     PlaceholderType,
 )
 
 if TYPE_CHECKING:
     from sceptre import stack
 
 T_Container = TypeVar("T_Container", bound=Union[dict, list])
+Self = TypeVar("Self")
 
 
 class RecursiveResolve(Exception):
     pass
 
 
-class Resolver(abc.ABC):
-    """
-    Resolver is an abstract base class that should be inherited by all
-    Resolvers.
+class CustomYamlTagBase:
+    """A base class for custom Yaml Elements (i.e. hooks and resolvers).
+
+    This base class takes care of common functionality needed by subclasses:
+    | * logging setup (associated with stacks)
+    | * Creating unique clones associated with individual stacks (applied recursively down to all
+    |   resolvers in the argument)
+    | * On-stack-connect setup that might be needed once connected to a Stack (applied recursively down to
+    |   all resolvers in the argument)
+    | * Automatically resolving resolvers in the argument when accessing self.argument
 
-    :param argument: The argument of the resolver.
-    :param stack: The associated stack of the resolver.
     """
 
+    logger = logging.getLogger(__name__)
+
     def __init__(self, argument: Any = None, stack: "stack.Stack" = None):
-        self.logger = logging.getLogger(__name__)
-        self.argument = argument
+        """Initializes a custom yaml tag object.
+
+        :param argument: The argument passed to the yaml tag. This could be a string, number, list,
+            or dict. Resolvers are supported in the argument, but they must be in either list or dict
+            arguments.
+        :param stack: The stack object associated with this instance. NOTE: When first instantiated
+            from loading the YAML, there will be no Stack. A Stack instance will only be passed into
+            the instance when "clone_for_stack" is invoked when the tag is associated with a specific
+            stack.
+        """
+        if stack is not None:
+            self.logger = StackLoggerAdapter(self.logger, stack.name)
+
         self.stack = stack
 
+        self._argument = argument
+        self._argument_is_resolved = False
+
+    @property
+    def argument(self) -> Any:
+        """This is the resolver or hook's argument.
+
+        This property will resolve all nested resolvers inside the argument, but only if this
+        instance has been associated with a Stack.
+
+        Resolving nested resolvers will result in their values being replaced in the dict/list they
+        were in with their resolved value, so we won't have to resolve them again.
+
+        Any resolvers that "resolve to nothing" (i.e. return None) will be removed from the dict/list
+        they were in.
+
+        If this property is accessed BEFORE the instance has a stack, it will return
+        the raw argument value. This is to safeguard any __init__() behaviors from triggering
+        resolution prematurely.
+        """
+        if self.stack is not None and not self._argument_is_resolved:
+            # Since resolving the argument updates the argument list or dict so that there aren't
+            # resolvers in it any more, we only need to do this resolution once per instance.
+            self._resolve_argument()
+
+        return self._argument
+
+    @argument.setter
+    def argument(self, value):
+        self._argument = value
+
+    def _resolve_argument(self):
+        """Resolves all argument resolvers recursively."""
+
+        keys_to_delete = []
+
+        def resolve(containing_list_or_dict, key, obj: Resolver):
+            result = obj.resolve()
+            # If the resolver "resolves to nothing", then it should get deleted out of its container.
+            if result is None:
+                keys_to_delete.append((containing_list_or_dict, key))
+            else:
+                containing_list_or_dict[key] = result
+
+        _call_func_on_values(resolve, self._argument, Resolver)
+        delete_keys_from_containers(keys_to_delete)
+
+        self._argument_is_resolved = True
+
+    def _recursively_setup(self):
+        """Ensures all nested resolvers in this resolver's argument are also setup when this
+        instance's setup method is called.
+        """
+        self.setup()
+
+        def setup_nested(containing_list_or_dict, key, obj: Resolver):
+            obj._recursively_setup()
+
+        _call_func_on_values(setup_nested, self._argument, Resolver)
+
+    def _recursively_clone(self: Self, stack: "stack.Stack") -> Self:
+        """Recursively clones the instance and its arguments.
+
+        The returned instance will have an identical argument that is a different memory reference,
+        so that instances inherited from a stack group and applied across multiple stacks are
+        independent of each other.
+
+        Furthermore, all nested resolvers in this resolver's argument will also be cloned to ensure
+        they themselves are also independent and fully configured for the current stack.
+        """
+
+        def recursively_clone_arguments(obj):
+            if isinstance(obj, Resolver):
+                return obj._recursively_clone(stack)
+            if isinstance(obj, list):
+                return [recursively_clone_arguments(item) for item in obj]
+            elif isinstance(obj, dict):
+                return {
+                    key: recursively_clone_arguments(val) for key, val in obj.items()
+                }
+            return obj
+
+        argument = recursively_clone_arguments(self._argument)
+        clone = type(self)(argument, stack)
+        return clone
+
+    def clone_for_stack(self: Self, stack: "stack.Stack") -> Self:
+        """
+        Obtains a clone of the current object, setup and ready for use for a given Stack instance.
+        """
+        clone = self._recursively_clone(stack)
+        clone._recursively_setup()
+        return clone
+
     def setup(self):
         """
-        This method is called at during stack initialisation.
+        This method is called when the object is connected to a Stack instance.
         Implementation of this method in subclasses can be used to do any
         initial setup of the object.
         """
         pass  # pragma: no cover
 
+    def __repr__(self) -> str:
+        """Returns a string representation of the resolver.
+
+        This is mostly used for resolver placeholders. In cases where we cannot resolve a resolver
+        YET, such as when we're generating a template or diff and there's a dependency on a stack
+        output of a stack that hasn't been deployed yet, placeholders need to render the resolver
+        in a way that is useful.
+
+        We use self._argument instead of self.argument because if there are resolvers nested in this
+        resolver's argument and one of those cannot be resolved, we'll need those resolvers to also
+        be converted to useful placeholder values.
+        """
+        as_str = f"!{self.__class__.__name__}"
+        if self._argument is not None:
+            as_str += f"({self._argument})"
+
+        return as_str
+
+
+class Resolver(CustomYamlTagBase, metaclass=abc.ABCMeta):
+    """
+    Resolver is an abstract base class that should be subclassed by all Resolvers.
+    """
+
     @abc.abstractmethod
     def resolve(self):
         """
         An abstract method which must be overwritten by all inheriting classes.
         This method is called to retrieve the final desired value.
         Implementation of this method in subclasses must return a suitable
         object or primitive type.
         """
         pass  # pragma: no cover
 
-    def clone(self, stack: "stack.Stack") -> "Resolver":
-        """
-        Produces a "fresh" copy of the Resolver, with the specified stack.
-
-        :param stack: The stack to set on the cloned resolver
-        """
-        return type(self)(self.argument, stack)
+    def raise_invalid_argument_error(self, message, from_: Exception = None):
+        error_message = f"{self.stack.name} - {message}"
+        if from_:
+            raise InvalidResolverArgumentError(error_message) from from_
+        raise InvalidResolverArgumentError(error_message)
 
 
 class ResolvableProperty(abc.ABC):
     """
     This is an abstract base class for a descriptor used to store an attribute that have values
     associated with Resolver objects.
 
@@ -119,31 +255,14 @@
             )
         setattr(stack, get_status_name, True)
         try:
             yield
         finally:
             setattr(stack, get_status_name, False)
 
-    def get_setup_resolver_for_stack(
-        self, stack: "stack.Stack", resolver: Resolver
-    ) -> Resolver:
-        """Obtains a clone of the resolver with the stack set on it and the setup method having
-        been called on it.
-
-        :param stack: The stack to set on the Resolver
-        :param resolver: The Resolver to clone and set up
-        :return: The cloned resolver.
-        """
-        # We clone the resolver when we assign the value so that every stack gets its own resolver
-        # rather than potentially having one resolver instance shared in memory across multiple
-        # stacks.
-        clone = resolver.clone(stack)
-        clone.setup()
-        return clone
-
     @abc.abstractmethod
     def get_resolved_value(
         self, stack: "stack.Stack", stack_class: Type["stack.Stack"]
     ) -> Any:
         """Implement this method to return the value of the resolvable_property."""
         pass
 
@@ -246,28 +365,15 @@
                     self.name,
                     key,
                     lambda: value.resolve(),
                 )
 
         container = getattr(stack, self.name)
         _call_func_on_values(resolve, container, Resolver)
-        # Remove keys and indexes from their containers that had resolvers resolve to None.
-        list_items_to_delete = []
-        for attr, key in keys_to_delete:
-            if isinstance(attr, list):
-                # If it's a list, we want to gather up the items to remove from the list.
-                # We don't want to modify the list length yet.
-                # Since removals will change all the other list indexes,
-                # we don't wan't to modify lists yet.
-                list_items_to_delete.append((attr, attr[key]))
-            else:
-                del attr[key]
-
-        for containing_list, item in list_items_to_delete:
-            containing_list.remove(item)
+        delete_keys_from_containers(keys_to_delete)
 
         return container
 
     def assign_value_to_stack(self, stack: "stack.Stack", value: Union[dict, list]):
         """Assigns a COPY of the specified value to the stack instance. This method copies the value
         rather than directly assigns it to avoid bugs related to shared objects in memory.
 
@@ -286,15 +392,15 @@
         :param container: The container being recursed into and cloned
         :param stack: The stack the container is being copied for
         :return: The fully copied container with resolvers fully set up.
         """
 
         def recurse(obj):
             if isinstance(obj, Resolver):
-                return self.get_setup_resolver_for_stack(stack, obj)
+                return obj.clone_for_stack(stack)
             if isinstance(obj, list):
                 return [recurse(item) for item in obj]
             elif isinstance(obj, dict):
                 return {key: recurse(val) for key, val in obj.items()}
             return obj
 
         return recurse(container)
@@ -381,9 +487,9 @@
         """Assigns the value to the Stack instance passed, setting up and cloning the value if it
         is a Resolver.
 
         :param stack: The Stack instance to set the value on
         :param value: The value to set
         """
         if isinstance(value, Resolver):
-            value = self.get_setup_resolver_for_stack(stack, value)
+            value = value.clone_for_stack(stack)
         setattr(stack, self.name, value)
```

### Comparing `sceptre-4.0.2/sceptre/resolvers/environment_variable.py` & `sceptre-4.1.0/sceptre/resolvers/environment_variable.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/resolvers/file_contents.py` & `sceptre-4.1.0/sceptre/resolvers/file_contents.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/resolvers/no_value.py` & `sceptre-4.1.0/sceptre/resolvers/no_value.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/resolvers/placeholders.py` & `sceptre-4.1.0/sceptre/resolvers/placeholders.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,18 +61,15 @@
       * { !ClassName } -> used when there is no argument
       * { !ClassName(argument) } -> used when there is a string argument
       * { !ClassName({'key': 'value'}) } -> used when there is a dict argument
 
     :param resolver: The resolver to create a placeholder for
     :return: The placeholder value
     """
-    base = f"!{type(resolver).__name__}"
-    suffix = f"({resolver.argument})" if resolver.argument is not None else ""
-    # double-braces in an f-string is just an escaped single brace
-    return f"{{ {base}{suffix} }}"
+    return f"{{ {resolver} }}"
 
 
 def _create_alphanumeric_placeholder(resolver: "resolvers.Resolver") -> str:
     """Creates a placeholder value that is only composed of alphanumeric characters. This is more
     useful when performing operations that send a template to CloudFormation, which will have stricter
     requirements for values in templates.
```

### Comparing `sceptre-4.0.2/sceptre/resolvers/stack_attr.py` & `sceptre-4.1.0/sceptre/resolvers/stack_attr.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/resolvers/stack_output.py` & `sceptre-4.1.0/sceptre/resolvers/stack_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # -*- coding: utf-8 -*-
 
-import abc
-import six
+import functools
 import logging
 import shlex
 
 from botocore.exceptions import ClientError
 
+from sceptre.exceptions import DependencyStackMissingOutputError, StackDoesNotExistError
 from sceptre.helpers import normalise_path, sceptreise_path
 from sceptre.resolvers import Resolver
-from sceptre.exceptions import DependencyStackMissingOutputError
-from sceptre.exceptions import StackDoesNotExistError
 
 TEMPLATE_EXTENSION = ".yaml"
 
 
-@six.add_metaclass(abc.ABCMeta)
 class StackOutputBase(Resolver):
     """
     A abstract base class which provides methods for getting Stack outputs.
     """
 
     def __init__(self, *args, **kwargs):
         self.logger = logging.getLogger(__name__)
@@ -46,14 +43,15 @@
         except KeyError:
             raise DependencyStackMissingOutputError(
                 "The Stack '{0}' does not have an output named '{1}'".format(
                     stack_name, output_key
                 )
             )
 
+    @functools.lru_cache(maxsize=4096)
     def _get_stack_outputs(
         self, stack_name, profile=None, region=None, sceptre_role=None
     ):
         """
         Communicates with AWS CloudFormation to fetch outputs from a specific
         Stack.
```

### Comparing `sceptre-4.0.2/sceptre/stack.py` & `sceptre-4.1.0/sceptre/stack.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/stack_status.py` & `sceptre-4.1.0/sceptre/stack_status.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/stack_status_colourer.py` & `sceptre-4.1.0/sceptre/stack_status_colourer.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/template.py` & `sceptre-4.1.0/sceptre/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import threading
 import botocore
 import sys
 
 import sceptre.helpers
 
 from sceptre.exceptions import TemplateHandlerNotFoundError
+from sceptre.logging import StackLoggerAdapter
 
 
 class Template(object):
     """
     Template represents an AWS CloudFormation template. It is responsible for
     loading, storing and optionally uploading local templates for use by
     CloudFormation.
@@ -50,16 +51,15 @@
         name,
         handler_config,
         sceptre_user_data,
         stack_group_config,
         connection_manager=None,
         s3_details=None,
     ):
-        self.logger = logging.getLogger(__name__)
-
+        self.logger = StackLoggerAdapter(logging.getLogger(__name__), name)
         self.name = name
         self.handler_config = handler_config
         if self.handler_config is not None and self.handler_config.get("type") is None:
             self.handler_config["type"] = "file"
         self.sceptre_user_data = sceptre_user_data
         self.stack_group_config = stack_group_config
         self.connection_manager = connection_manager
```

### Comparing `sceptre-4.0.2/sceptre/template_handlers/__init__.py` & `sceptre-4.1.0/sceptre/template_handlers/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import abc
 import logging
 
 import six
 from jsonschema import validate, ValidationError
 
 from sceptre.exceptions import TemplateHandlerArgumentsInvalidError
+from sceptre.logging import StackLoggerAdapter
 
 
 @six.add_metaclass(abc.ABCMeta)
 class TemplateHandler:
     """
     TemplateHandler is an abstract base class that should be inherited
     by all Template Handlers.
@@ -45,15 +46,15 @@
         self,
         name,
         arguments=None,
         sceptre_user_data=None,
         connection_manager=None,
         stack_group_config=None,
     ):
-        self.logger = logging.getLogger(__name__)
+        self.logger = StackLoggerAdapter(logging.getLogger(__name__), name)
         self.name = name
         self.arguments = arguments
         self.sceptre_user_data = sceptre_user_data
         self.connection_manager = connection_manager
 
         if stack_group_config is None:
             stack_group_config = {}
```

### Comparing `sceptre-4.0.2/sceptre/template_handlers/file.py` & `sceptre-4.1.0/sceptre/template_handlers/file.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/template_handlers/helper.py` & `sceptre-4.1.0/sceptre/template_handlers/helper.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/template_handlers/http.py` & `sceptre-4.1.0/sceptre/template_handlers/http.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/sceptre/template_handlers/s3.py` & `sceptre-4.1.0/sceptre/template_handlers/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,9 +88,9 @@
             response = self.connection_manager.call(
                 service="s3",
                 command="get_object",
                 kwargs={"Bucket": bucket, "Key": key},
             )
             return response["Body"].read()
         except Exception as e:
-            self.logger.fatal(e)
+            self.logger.critical(e)
             raise e
```

### Comparing `sceptre-4.0.2/sceptre.egg-info/PKG-INFO` & `sceptre-4.1.0/sceptre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sceptre
-Version: 4.0.2
+Version: 4.1.0
 Summary: Cloud Provisioning Tool
 Home-page: https://github.com/Sceptre/sceptre
 Author: Cloudreach
 Author-email: sceptre@cloudreach.com
 License: Apache2
 Keywords: sceptre
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sceptre-4.0.2/sceptre.egg-info/SOURCES.txt` & `sceptre-4.1.0/sceptre.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 docs/_source/docs/terminology.rst
 requirements/prod.txt
 sceptre/__init__.py
 sceptre/connection_manager.py
 sceptre/context.py
 sceptre/exceptions.py
 sceptre/helpers.py
+sceptre/logging.py
 sceptre/stack.py
 sceptre/stack_status.py
 sceptre/stack_status_colourer.py
 sceptre/template.py
 sceptre.egg-info/PKG-INFO
 sceptre.egg-info/SOURCES.txt
 sceptre.egg-info/dependency_links.txt
@@ -79,18 +80,22 @@
 sceptre/plan/__init__.py
 sceptre/plan/actions.py
 sceptre/plan/executor.py
 sceptre/plan/plan.py
 sceptre/resolvers/__init__.py
 sceptre/resolvers/environment_variable.py
 sceptre/resolvers/file_contents.py
+sceptre/resolvers/join.py
 sceptre/resolvers/no_value.py
 sceptre/resolvers/placeholders.py
+sceptre/resolvers/select.py
+sceptre/resolvers/split.py
 sceptre/resolvers/stack_attr.py
 sceptre/resolvers/stack_output.py
+sceptre/resolvers/sub.py
 sceptre/stack_policies/lock.json
 sceptre/stack_policies/unlock.json
 sceptre/template_handlers/__init__.py
 sceptre/template_handlers/file.py
 sceptre/template_handlers/helper.py
 sceptre/template_handlers/http.py
 sceptre/template_handlers/s3.py
@@ -164,16 +169,20 @@
 tests/test_diffing/test_stack_differ.py
 tests/test_hooks/__init__.py
 tests/test_hooks/test_asg_scaling_processes.py
 tests/test_hooks/test_cmd.py
 tests/test_hooks/test_hooks.py
 tests/test_resolvers/test_environment_variable.py
 tests/test_resolvers/test_file_contents.py
+tests/test_resolvers/test_join.py
 tests/test_resolvers/test_placeholders.py
 tests/test_resolvers/test_resolver.py
+tests/test_resolvers/test_select.py
+tests/test_resolvers/test_split.py
 tests/test_resolvers/test_stack_attr.py
 tests/test_resolvers/test_stack_output.py
+tests/test_resolvers/test_sub.py
 tests/test_template_handlers/test_file.py
 tests/test_template_handlers/test_helper.py
 tests/test_template_handlers/test_http.py
 tests/test_template_handlers/test_s3.py
 tests/test_template_handlers/test_template_handlers.py
```

### Comparing `sceptre-4.0.2/sceptre.egg-info/entry_points.txt` & `sceptre-4.1.0/sceptre.egg-info/entry_points.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 [sceptre.hooks]
 asg_scheduled_actions = sceptre.hooks.asg_scaling_processes:ASGScalingProcesses
 cmd = sceptre.hooks.cmd:Cmd
 
 [sceptre.resolvers]
 environment_variable = sceptre.resolvers.environment_variable:EnvironmentVariable
 file_contents = sceptre.resolvers.file_contents:FileContents
+join = sceptre.resolvers.join:Join
 no_value = sceptre.resolvers.no_value:NoValue
+select = sceptre.resolvers.select:Select
+split = sceptre.resolvers.split:Split
 stack_attr = sceptre.resolvers.stack_attr:StackAttr
 stack_output = sceptre.resolvers.stack_output:StackOutput
 stack_output_external = sceptre.resolvers.stack_output:StackOutputExternal
+sub = sceptre.resolvers.sub:Sub
 
 [sceptre.template_handlers]
 file = sceptre.template_handlers.file:File
 http = sceptre.template_handlers.http:Http
 s3 = sceptre.template_handlers.s3:S3
```

### Comparing `sceptre-4.0.2/setup.py` & `sceptre-4.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,19 @@
             "environment_variable ="
             "sceptre.resolvers.environment_variable:EnvironmentVariable",
             "file_contents = sceptre.resolvers.file_contents:FileContents",
             "stack_output = sceptre.resolvers.stack_output:StackOutput",
             "stack_output_external ="
             "sceptre.resolvers.stack_output:StackOutputExternal",
             "no_value = sceptre.resolvers.no_value:NoValue",
+            "select = sceptre.resolvers.select:Select",
             "stack_attr = sceptre.resolvers.stack_attr:StackAttr",
+            "sub = sceptre.resolvers.sub:Sub",
+            "split = sceptre.resolvers.split:Split",
+            "join = sceptre.resolvers.join:Join",
         ],
         "sceptre.template_handlers": [
             "file = sceptre.template_handlers.file:File",
             "s3 = sceptre.template_handlers.s3:S3",
             "http = sceptre.template_handlers.http:Http",
         ],
     },
```

### Comparing `sceptre-4.0.2/tests/fixtures/templates/compiled_vpc.json` & `sceptre-4.1.0/tests/fixtures/templates/compiled_vpc.json`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures/templates/compiled_vpc_sud.json` & `sceptre-4.1.0/tests/fixtures/templates/compiled_vpc_sud.json`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures/templates/vpc.py` & `sceptre-4.1.0/tests/fixtures/templates/vpc.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures/templates/vpc.template` & `sceptre-4.1.0/tests/fixtures/templates/vpc.template`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures/templates/vpc.without_start_marker.yaml` & `sceptre-4.1.0/tests/fixtures/templates/vpc.without_start_marker.yaml`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures/templates/vpc.yaml` & `sceptre-4.1.0/tests/fixtures/templates/vpc.yaml`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures/templates/vpc_sgt.py` & `sceptre-4.1.0/tests/fixtures/templates/vpc_sgt.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures/templates/vpc_sud.py` & `sceptre-4.1.0/tests/fixtures/templates/vpc_sud.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures/templates/vpc_t.py` & `sceptre-4.1.0/tests/fixtures/templates/vpc_t.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures-vpc/templates/compiled_vpc.json` & `sceptre-4.1.0/tests/fixtures-vpc/templates/compiled_vpc.json`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures-vpc/templates/compiled_vpc_sud.json` & `sceptre-4.1.0/tests/fixtures-vpc/templates/compiled_vpc_sud.json`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures-vpc/templates/vpc.json` & `sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.json`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures-vpc/templates/vpc.py` & `sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures-vpc/templates/vpc.template` & `sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.template`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures-vpc/templates/vpc.yaml` & `sceptre-4.1.0/tests/fixtures-vpc/templates/vpc.yaml`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures-vpc/templates/vpc_sgt.py` & `sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_sgt.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures-vpc/templates/vpc_sud.py` & `sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_sud.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/fixtures-vpc/templates/vpc_t.py` & `sceptre-4.1.0/tests/fixtures-vpc/templates/vpc_t.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_actions.py` & `sceptre-4.1.0/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_cli/test_cli_commands.py` & `sceptre-4.1.0/tests/test_cli/test_cli_commands.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_cli/test_launch.py` & `sceptre-4.1.0/tests/test_cli/test_launch.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_cli/test_prune.py` & `sceptre-4.1.0/tests/test_cli/test_prune.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_config_reader.py` & `sceptre-4.1.0/tests/test_config_reader.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_connection_manager.py` & `sceptre-4.1.0/tests/test_connection_manager.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_context.py` & `sceptre-4.1.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_diffing/test_diff_writer.py` & `sceptre-4.1.0/tests/test_diffing/test_diff_writer.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_diffing/test_stack_differ.py` & `sceptre-4.1.0/tests/test_diffing/test_stack_differ.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_helpers.py` & `sceptre-4.1.0/tests/test_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import deprecation
 import pytest
 
 from os.path import join, sep
 from datetime import datetime, timezone, timedelta
 
 from sceptre.exceptions import PathConversionError
-from sceptre.helpers import get_external_stack_name, create_deprecated_alias_property
+from sceptre.helpers import (
+    get_external_stack_name,
+    create_deprecated_alias_property,
+    delete_keys_from_containers,
+)
 from sceptre.helpers import normalise_path
 from sceptre.helpers import sceptreise_path
 from sceptre.helpers import extract_datetime_from_aws_response_headers, gen_repr
 from sceptre import __version__
 
 
 class SomeClass(object):
@@ -167,7 +171,26 @@
         obj = MyClass()
 
         with warnings.catch_warnings(record=True) as messages:
             obj.alias = "winner"
 
         assert len(messages) == 1
         assert messages[0].category == deprecation.DeprecatedWarning
+
+    def test_delete_keys_from_containers__removes_keys_from_dicts(self):
+        a = {"keep": "me", "kill": "me"}
+        b = {"keep": "me", "take": "me out"}
+        c = {"keep": "me", "destroy": "me"}
+
+        arg = [(a, "kill"), (b, "take"), (c, "destroy")]
+        delete_keys_from_containers(arg)
+        expected = {"keep": "me"}
+        assert a == b == c == expected
+
+    def test_delete_keys_from_containers__removes_indexes_from_lists(self):
+        a = ["keep me", "kill me", "keep me", "destroy me"]
+        b = ["take me out", "keep me", "send me the true death", "keep me"]
+
+        arg = [(a, 1), (a, 3), (b, 0), (b, 2)]
+        delete_keys_from_containers(arg)
+        expected = ["keep me", "keep me"]
+        assert a == b == expected
```

### Comparing `sceptre-4.0.2/tests/test_hooks/test_asg_scaling_processes.py` & `sceptre-4.1.0/tests/test_hooks/test_asg_scaling_processes.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from sceptre.hooks.asg_scaling_processes import ASGScalingProcesses
 from sceptre.stack import Stack
 
 
 class TestASGScalingProcesses(object):
     def setup_method(self, test_method):
         self.stack = MagicMock(spec=Stack)
+        self.stack.name = "my/stack.yaml"
         self.stack.connection_manager = MagicMock(spec=ConnectionManager)
         self.stack.external_name = "external_name"
         self.asg_scaling_processes = ASGScalingProcesses(None, self.stack)
 
     def test_get_stack_resources_sends_correct_request(self):
         self.stack.connection_manager.call.return_value = {
             "StackResources": [
```

### Comparing `sceptre-4.0.2/tests/test_hooks/test_cmd.py` & `sceptre-4.1.0/tests/test_hooks/test_cmd.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from sceptre.hooks.cmd import Cmd
 from sceptre.stack import Stack
 
 
 class TestCmd(object):
     def setup_method(self, test_method):
         self.stack = Mock(Stack)
+        self.stack.name = "my/stack.yaml"
         self.cmd = Cmd(stack=self.stack)
 
     def test_run_with_non_str_argument(self):
         self.cmd.argument = None
         with pytest.raises(InvalidHookArgumentTypeError):
             self.cmd.run()
```

### Comparing `sceptre-4.0.2/tests/test_hooks/test_hooks.py` & `sceptre-4.1.0/tests/test_hooks/test_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
-from unittest.mock import MagicMock
+from unittest import TestCase
+from unittest.mock import MagicMock, Mock
 
 from sceptre.hooks import Hook, HookProperty, add_stack_hooks, execute_hooks
+from sceptre.resolvers import Resolver
+from sceptre.stack import Stack
+import logging
 
 
 class MockHook(Hook):
-    def __init__(self, *args, **kwargs):
-        super(MockHook, self).__init__(*args, **kwargs)
-
     def run(self):
         pass
 
 
 class TestHooksFunctions(object):
     def setup_method(self, test_method):
         pass
@@ -56,33 +57,51 @@
         hook_1 = MagicMock(spec=Hook)
         hook_2 = MagicMock(spec=Hook)
         execute_hooks([hook_1, hook_2])
         hook_1.run.called_once_with()
         hook_2.run.called_once_with()
 
 
-class TestHook(object):
-    def setup_method(self, test_method):
-        self.hook = MockHook()
-
-    def test_hook_inheritance(self):
-        assert isinstance(self.hook, Hook)
+class MyResolver(Resolver):
+    def resolve(self):
+        return self.argument
+
+
+class TestHook(TestCase):
+    def setUp(self):
+        self.stack = Mock(Stack)
+        self.stack.name = "my/stack"
+        self.hook = MockHook(stack=self.stack)
+
+    def test_logger__logs_have_stack_name_prefix(self):
+        with self.assertLogs(self.hook.logger.name, logging.INFO) as handler:
+            self.hook.logger.info("Bonjour")
+
+        assert handler.records[0].message == f"{self.stack.name} - Bonjour"
+
+    def test_argument__supports_resolvers_in_arguments(self):
+        arg = [MyResolver("hello")]
+        hook = MockHook(arg, self.stack)
+        self.assertEqual(["hello"], hook.argument)
 
 
 class MockClass(object):
     hook_property = HookProperty("hook_property")
     config = MagicMock()
+    name = "my/stack.yaml"
 
 
 class TestHookPropertyDescriptor(object):
     def setup_method(self, test_method):
         self.mock_object = MockClass()
 
     def test_setting_hook_property(self):
         mock_hook = MagicMock(spec=MockHook)
 
         self.mock_object.hook_property = [mock_hook]
-        assert self.mock_object._hook_property == [mock_hook]
+        assert self.mock_object._hook_property == [
+            mock_hook.clone_for_stack.return_value
+        ]
 
     def test_getting_hook_property(self):
         self.mock_object._hook_property = self.mock_object
         assert self.mock_object.hook_property == self.mock_object
```

### Comparing `sceptre-4.0.2/tests/test_plan.py` & `sceptre-4.1.0/tests/test_plan.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_resolvers/test_environment_variable.py` & `sceptre-4.1.0/tests/test_resolvers/test_environment_variable.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_resolvers/test_file_contents.py` & `sceptre-4.1.0/tests/test_resolvers/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_resolvers/test_placeholders.py` & `sceptre-4.1.0/tests/test_resolvers/test_placeholders.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 from sceptre.resolvers.placeholders import (
     use_resolver_placeholders_on_error,
     PlaceholderType,
     create_placeholder_value,
 )
 
 
+class MyResolver(Resolver):
+    def resolve(self):
+        return self.argument
+
+
 class TestPlaceholders:
     def test_are_placeholders_enabled__returns_false(self):
         assert are_placeholders_enabled() is False
 
     def test_are_placeholders_enabled__in_placeholder_context__returns_true(self):
         with use_resolver_placeholders_on_error():
             assert are_placeholders_enabled() is True
@@ -48,35 +53,45 @@
             pytest.param(
                 PlaceholderType.explicit,
                 {"key": "value"},
                 "{ !MyResolver({'key': 'value'}) }",
                 id="explicit dict argument",
             ),
             pytest.param(
+                PlaceholderType.explicit,
+                {"some_key": MyResolver("some value")},
+                "{ !MyResolver({'some_key': !MyResolver(some value)}) }",
+                id="explicit with nested resolvers",
+            ),
+            pytest.param(
                 PlaceholderType.alphanum, None, "MyResolver", id="alphanum no argument"
             ),
             pytest.param(
                 PlaceholderType.alphanum,
                 "argument",
                 "MyResolverargument",
                 id="alphanum string argument",
             ),
             pytest.param(
                 PlaceholderType.alphanum,
                 {"key": "value"},
                 "MyResolverkeyvalue",
                 id="alphanum dict argument",
             ),
-            pytest.param(PlaceholderType.none, "something", None),
+            pytest.param(
+                PlaceholderType.alphanum,
+                {"some_key": MyResolver("some value")},
+                "MyResolversomekeyMyResolversomevalue",
+                id="alphanum with nested resolvers",
+            ),
+            pytest.param(
+                PlaceholderType.none, "something", None, id="none type placeholder type"
+            ),
         ],
     )
     def test_create_placeholder_value(self, placeholder_type, argument, expected):
-        class MyResolver(Resolver):
-            def resolve(self):
-                pass
-
         resolver = MyResolver(argument)
 
         with use_resolver_placeholders_on_error():
             result = create_placeholder_value(resolver, placeholder_type)
 
         assert result == expected
```

### Comparing `sceptre-4.0.2/tests/test_resolvers/test_resolver.py` & `sceptre-4.1.0/tests/test_resolvers/test_resolver.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
-from unittest.mock import call, Mock
+import logging
+from unittest import TestCase
+from unittest.mock import call, Mock, sentinel, MagicMock
 
 import pytest
-from unittest.mock import sentinel, MagicMock
 
+from sceptre.exceptions import InvalidResolverArgumentError
 from sceptre.resolvers import (
     Resolver,
     ResolvableContainerProperty,
     ResolvableValueProperty,
     RecursiveResolve,
 )
 from sceptre.resolvers.placeholders import (
@@ -20,42 +22,207 @@
 class MockResolver(Resolver):
     """
     MockResolver inherits from the abstract base class Resolver, and
     implements the abstract methods. It is used to allow testing on
     Resolver, which is not otherwise instantiable.
     """
 
+    setup_has_been_called = False
+
     def resolve(self):
         pass
 
+    def setup(self):
+        self.setup_has_been_called = True
+
+
+class NestedResolver(Resolver):
+    setup_has_been_called = False
+    resolve_count = 0
+
+    def setup(self):
+        self.setup_has_been_called = True
+
+    def resolve(self):
+        self.resolve_count += 1
+        return self.argument
+
 
 class MockClass(object):
     resolvable_container_property = ResolvableContainerProperty(
         "resolvable_container_property"
     )
     container_with_alphanum_placeholder = ResolvableContainerProperty(
         "container_with_placeholder_override", PlaceholderType.alphanum
     )
     resolvable_value_property = ResolvableValueProperty("resolvable_value_property")
     value_with_none_placeholder = ResolvableValueProperty(
         "value_with_placeholder_override", PlaceholderType.none
     )
     config = MagicMock()
 
+    name = "my/stack"
 
-class TestResolver(object):
-    def setup_method(self, test_method):
+
+class TestResolver(TestCase):
+    def setUp(self):
         self.mock_resolver = MockResolver(
             argument=sentinel.argument, stack=sentinel.stack
         )
 
     def test_init(self):
         assert self.mock_resolver.stack == sentinel.stack
         assert self.mock_resolver.argument == sentinel.argument
 
+    def test_logger__logs_have_stack_name_prefix(self):
+        with self.assertLogs(self.mock_resolver.logger.name, logging.INFO) as handler:
+            self.mock_resolver.logger.info("Bonjour")
+
+        assert handler.records[0].message == f"{sentinel.stack.name} - Bonjour"
+
+    def test_invalid_argument_error__raises_invalid_argument_error_with_stack_name_prefix(
+        self,
+    ):
+        with pytest.raises(
+            InvalidResolverArgumentError, match=f"{sentinel.stack.name} - danger"
+        ):
+            self.mock_resolver.raise_invalid_argument_error("danger")
+
+
+class TestCustomYamlTagBase(TestCase):
+    def setUp(self):
+        self.stack = Mock()
+        self.stack.name = "My Stack"
+
+    def test_clone_for_stack__dict_argument_is_cloned(self):
+        arg = {"greeting": "hello"}
+        resolver = MockResolver(arg)
+        clone = resolver.clone_for_stack(self.stack)
+        self.assertIsNot(clone.argument, arg)
+
+    def test_clone_for_stack__list_argument_is_cloned(self):
+        arg = ["hello"]
+        resolver = MockResolver(arg)
+        clone = resolver.clone_for_stack(self.stack)
+        self.assertIsNot(clone.argument, arg)
+
+    def test_clone_for_stack__nested_dict_argument_is_cloned(self):
+        arg = {"greetings": {"French": "bonjour"}}
+        resolver = MockResolver(arg)
+        clone = resolver.clone_for_stack(None)
+        self.assertIsNot(clone.argument["greetings"], arg["greetings"])
+
+    def test_clone_for_stack__nested_list_argument_is_cloned(self):
+        arg = [{"French": "bonjour"}]
+        resolver = MockResolver(arg)
+        clone = resolver.clone_for_stack(None)
+        self.assertIsNot(clone.argument[0], arg[0])
+
+    def test_clone_for_stack__nested_resolvers_are_cloned(self):
+        arg = {"greetings": {"French": NestedResolver("bonjour")}}
+        resolver = MockResolver(arg)
+        clone = resolver.clone_for_stack(None)
+        self.assertIsNot(
+            clone.argument["greetings"]["French"], arg["greetings"]["French"]
+        )
+
+    def test_clone_for_stack__calls_setup(self):
+        arg = {"greetings": {"French": NestedResolver("bonjour")}}
+        resolver = MockResolver(arg)
+        clone = resolver.clone_for_stack(self.stack)
+        self.assertTrue(clone.setup_has_been_called)
+
+    def test_clone_for_stack__nested_resolvers_are_setup(self):
+        arg = {"greetings": {"French": NestedResolver("bonjour")}}
+        resolver = MockResolver(arg)
+        # Passing None here will mean that the argument won't actually be resolved, so it lets us
+        # access the actual resolver instance.
+        clone = resolver.clone_for_stack(None)
+
+        self.assertTrue(clone.argument["greetings"]["French"].setup_has_been_called)
+
+    def test_clone_for_stack__resolvers_inside_resolvers_are_cloned(self):
+        arg = {
+            "greetings": {
+                "French": NestedResolver({"informal": NestedResolver("salut")})
+            }
+        }
+        resolver = MockResolver(arg)
+        # Passing None here will mean that the argument won't actually be resolved, so it lets us
+        # access the actual resolver instance.
+        clone = resolver.clone_for_stack(None)
+        self.assertIsNot(
+            clone.argument["greetings"]["French"].argument["informal"],
+            arg["greetings"]["French"].argument["informal"],
+        )
+
+    def test_clone_for_stack__resolvers_inside_resolvers_are_setup(self):
+        arg = {
+            "greetings": {
+                "French": NestedResolver({"informal": NestedResolver("salut")})
+            }
+        }
+        resolver = MockResolver(arg)
+        # Passing None here will mean that the argument won't actually be resolved, so it lets us
+        # access the actual resolver instance.
+        clone = resolver.clone_for_stack(None)
+        self.assertTrue(
+            clone.argument["greetings"]["French"]
+            .argument["informal"]
+            .setup_has_been_called
+        )
+
+    def test_argument__has_stack__arg_is_string__resolves_to_string(self):
+        arg = "hello"
+        resolver = MockResolver(arg)
+        clone = resolver.clone_for_stack(self.stack)
+
+        self.assertEqual("hello", clone.argument)
+
+    def test_argument__cloned_for_stack__resolves_arg_resolver(self):
+        arg = {"greetings": {"French": NestedResolver("bonjour")}}
+        resolver = MockResolver(arg).clone_for_stack(self.stack)
+        expected = {"greetings": {"French": "bonjour"}}
+        self.assertEqual(expected, resolver.argument)
+
+    def test_argument__cloned_for_stack__nested_argument_in_nested_argument__results_all_resolvers(
+        self,
+    ):
+        arg = {
+            "greetings": {
+                "French": NestedResolver({"informal": NestedResolver("salut")})
+            }
+        }
+        resolver = MockResolver(arg).clone_for_stack(self.stack)
+        expected = {"greetings": {"French": {"informal": "salut"}}}
+        self.assertEqual(expected, resolver.argument)
+
+    def test_argument__cloned_for_stack__nested_argument_in_dict_resolves_to_nothing__removes_it_from_argument(
+        self,
+    ):
+        arg = {"greetings": {"French": NestedResolver(None)}}
+        resolver = MockResolver(arg).clone_for_stack(self.stack)
+        expected = {"greetings": {}}
+        self.assertEqual(expected, resolver.argument)
+
+    def test_argument__nested_argument_in_list_resolves_to_nothing__removes_it_from_argument(
+        self,
+    ):
+        arg = {
+            "greetings": [
+                NestedResolver(None),
+                "Hello",
+                NestedResolver(None),
+                "Bonjour",
+            ]
+        }
+        resolver = MockResolver(arg).clone_for_stack(self.stack)
+        expected = {"greetings": ["Hello", "Bonjour"]}
+        self.assertEqual(expected, resolver.argument)
+
 
 class TestResolvableContainerPropertyDescriptor:
     def setup_method(self, test_method):
         self.mock_object = MockClass()
 
     def test_setting_resolvable_property_with_none(self):
         self.mock_object.resolvable_container_property = None
@@ -72,30 +239,30 @@
                 "String",
                 [[mock_resolver, "String", None], mock_resolver, "String"],
             ],
         ]
 
         cloned_data_structure = [
             "String",
-            mock_resolver.clone.return_value,
+            mock_resolver.clone_for_stack.return_value,
             [
-                mock_resolver.clone.return_value,
+                mock_resolver.clone_for_stack.return_value,
                 "String",
                 [
-                    [mock_resolver.clone.return_value, "String", None],
-                    mock_resolver.clone.return_value,
+                    [mock_resolver.clone_for_stack.return_value, "String", None],
+                    mock_resolver.clone_for_stack.return_value,
                     "String",
                 ],
             ],
         ]
 
         self.mock_object.resolvable_container_property = complex_data_structure
         assert self.mock_object._resolvable_container_property == cloned_data_structure
-        expected_calls = [call(self.mock_object), call().setup()] * 4
-        mock_resolver.clone.assert_has_calls(expected_calls)
+        expected_calls = [call(self.mock_object)] * 4
+        mock_resolver.clone_for_stack.assert_has_calls(expected_calls)
 
     def test_getting_resolvable_property_with_none(self):
         self.mock_object._resolvable_container_property = None
         assert self.mock_object.resolvable_container_property is None
 
     def test_getting_resolvable_property_with_nested_lists(self):
         mock_resolver = MagicMock(spec=MockResolver)
@@ -452,22 +619,18 @@
 
     def test_set__resolver__sets_private_variable_with_clone_of_resolver_with_instance(
         self,
     ):
         resolver = Mock(spec=MockResolver)
         self.mock_object.resolvable_value_property = resolver
         assert (
-            self.mock_object._resolvable_value_property == resolver.clone.return_value
+            self.mock_object._resolvable_value_property
+            == resolver.clone_for_stack.return_value
         )
 
-    def test_set__resolver__sets_up_cloned_resolver(self):
-        resolver = Mock(spec=MockResolver)
-        self.mock_object.resolvable_value_property = resolver
-        resolver.clone.return_value.setup.assert_any_call()
-
     @pytest.mark.parametrize("value", ["string", True, 123, 1.23, None])
     def test_get__non_resolver__returns_value(self, value):
         self.mock_object._resolvable_value_property = value
         assert self.mock_object.resolvable_value_property == value
 
     def test_get__resolver__returns_resolved_value(self):
         resolver = Mock(spec=MockResolver)
```

### Comparing `sceptre-4.0.2/tests/test_resolvers/test_stack_attr.py` & `sceptre-4.1.0/tests/test_resolvers/test_stack_attr.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from sceptre.stack import Stack
 
 
 class TestResolver(object):
     def setup_method(self, test_method):
         self.stack_group_config = {}
         self.stack = Mock(spec=Stack, stack_group_config=self.stack_group_config)
+        self.stack.name = "my/stack.yaml"
 
         self.resolver = StackAttr(stack=self.stack)
 
     def test__resolve__returns_attribute_off_stack(self):
         self.resolver.argument = "testing_this"
         self.stack.testing_this = "hurray!"
         result = self.resolver.resolve()
```

### Comparing `sceptre-4.0.2/tests/test_resolvers/test_stack_output.py` & `sceptre-4.1.0/tests/test_resolvers/test_stack_output.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from sceptre.stack import Stack
 
 
 class TestStackOutputResolver(object):
     @patch("sceptre.resolvers.stack_output.StackOutput._get_output_value")
     def test_resolver(self, mock_get_output_value):
         stack = MagicMock(spec=Stack)
+        stack.name = "my/stack"
         stack.dependencies = []
         stack.project_code = "project-code"
         stack._connection_manager = MagicMock(spec=ConnectionManager)
 
         dependency = MagicMock()
         dependency.project_code = "meh"
         dependency.name = "account/dev/vpc"
@@ -48,14 +49,15 @@
             region="dependency_region",
             sceptre_role="dependency_sceptre_role",
         )
 
     @patch("sceptre.resolvers.stack_output.StackOutput._get_output_value")
     def test_resolver_with_existing_dependencies(self, mock_get_output_value):
         stack = MagicMock(spec=Stack)
+        stack.name = "my/stack"
         stack.dependencies = ["existing"]
         stack.project_code = "project-code"
         stack._connection_manager = MagicMock(spec=ConnectionManager)
 
         dependency = MagicMock()
         dependency.project_code = "meh"
         dependency.name = "account/dev/vpc"
@@ -80,14 +82,15 @@
             region="dependency_region",
             sceptre_role="dependency_sceptre_role",
         )
 
     @patch("sceptre.resolvers.stack_output.StackOutput._get_output_value")
     def test_resolve_with_implicit_stack_reference(self, mock_get_output_value):
         stack = MagicMock(spec=Stack)
+        stack.name = "my/stack"
         stack.dependencies = []
         stack.project_code = "project-code"
         stack.name = "account/dev/stack"
         stack._connection_manager = MagicMock(spec=ConnectionManager)
 
         dependency = MagicMock()
         dependency.project_code = "meh"
@@ -115,14 +118,15 @@
         )
 
     @patch("sceptre.resolvers.stack_output.StackOutput._get_output_value")
     def test_resolve_with_implicit_stack_reference_top_level(
         self, mock_get_output_value
     ):
         stack = MagicMock(spec=Stack)
+        stack.name = "my/stack"
         stack.dependencies = []
         stack.project_code = "project-code"
         stack.name = "stack"
         stack._connection_manager = MagicMock(spec=ConnectionManager)
 
         dependency = MagicMock()
         dependency.project_code = "meh"
@@ -150,14 +154,15 @@
         )
 
 
 class TestStackOutputExternalResolver(object):
     @patch("sceptre.resolvers.stack_output.StackOutputExternal._get_output_value")
     def test_resolve(self, mock_get_output_value):
         stack = MagicMock(spec=Stack)
+        stack.name = "my/stack"
         stack.dependencies = []
         stack._connection_manager = MagicMock(spec=ConnectionManager)
         stack_output_external_resolver = StackOutputExternal(
             "another/account-vpc::VpcId", stack
         )
         mock_get_output_value.return_value = "output_value"
         stack_output_external_resolver.resolve()
@@ -165,14 +170,15 @@
             "another/account-vpc", "VpcId", None, None, None
         )
         assert stack.dependencies == []
 
     @patch("sceptre.resolvers.stack_output.StackOutputExternal._get_output_value")
     def test_resolve_with_args(self, mock_get_output_value):
         stack = MagicMock(spec=Stack)
+        stack.name = "my/stack"
         stack.dependencies = []
         stack._connection_manager = MagicMock(spec=ConnectionManager)
         stack_output_external_resolver = StackOutputExternal(
             "another/account-vpc::VpcId region::profile::sceptre_role", stack
         )
         mock_get_output_value.return_value = "output_value"
         stack_output_external_resolver.resolve()
@@ -196,14 +202,15 @@
     def resolve(self):
         pass
 
 
 class TestStackOutputBaseResolver(object):
     def setup_method(self, test_method):
         self.stack = MagicMock(spec=Stack)
+        self.stack.name = "my/stack.yaml"
         self.stack._connection_manager = MagicMock(spec=ConnectionManager)
         self.base_stack_output_resolver = MockStackOutputBase(None, self.stack)
 
     @patch("sceptre.resolvers.stack_output.StackOutputBase._get_stack_outputs")
     def test_get_output_value_with_valid_key(self, mock_get_stack_outputs):
         mock_get_stack_outputs.return_value = {"key": "value"}
```

### Comparing `sceptre-4.0.2/tests/test_stack.py` & `sceptre-4.1.0/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_stack_status_colourer.py` & `sceptre-4.1.0/tests/test_stack_status_colourer.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_template.py` & `sceptre-4.1.0/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_template_handlers/test_file.py` & `sceptre-4.1.0/tests/test_template_handlers/test_file.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_template_handlers/test_helper.py` & `sceptre-4.1.0/tests/test_template_handlers/test_helper.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_template_handlers/test_http.py` & `sceptre-4.1.0/tests/test_template_handlers/test_http.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_template_handlers/test_s3.py` & `sceptre-4.1.0/tests/test_template_handlers/test_s3.py`

 * *Files identical despite different names*

### Comparing `sceptre-4.0.2/tests/test_template_handlers/test_template_handlers.py` & `sceptre-4.1.0/tests/test_template_handlers/test_template_handlers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import logging
+from unittest import TestCase
+
 import pytest
 
 from sceptre.exceptions import TemplateHandlerArgumentsInvalidError
 from sceptre.template_handlers import TemplateHandler
 
 
 class MockTemplateHandler(TemplateHandler):
@@ -15,18 +18,27 @@
             "required": ["argument"],
         }
 
     def handle(self):
         return "TestTemplateHandler"
 
 
-class TestTemplateHandlers(object):
+class TestTemplateHandlers(TestCase):
     def test_template_handler_validates_schema(self):
         handler = MockTemplateHandler(name="mock", arguments={"argument": "test"})
         handler.validate()
 
     def test_template_handler_errors_when_arguments_invalid(self):
         with pytest.raises(TemplateHandlerArgumentsInvalidError):
             handler = MockTemplateHandler(
                 name="mock", arguments={"non-existent": "test"}
             )
             handler.validate()
+
+    def test_logger__logs_have_stack_name_prefix(self):
+        template_handler = MockTemplateHandler(
+            name="mock", arguments={"argument": "test"}
+        )
+        with self.assertLogs(template_handler.logger.name, logging.INFO) as handler:
+            template_handler.logger.info("Bonjour")
+
+        assert handler.records[0].message == f"{template_handler.name} - Bonjour"
```

