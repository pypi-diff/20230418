# Comparing `tmp/fusesoc-2.1.tar.gz` & `tmp/fusesoc-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusesoc-2.1.tar", last modified: Thu Mar 23 20:00:47 2023, max compression
+gzip compressed data, was "fusesoc-2.2.tar", last modified: Tue Apr 18 10:07:46 2023, max compression
```

## Comparing `fusesoc-2.1.tar` & `fusesoc-2.2.tar`

### file list

```diff
@@ -1,256 +1,265 @@
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.975579 fusesoc-2.1/
--rw-r--r--   0 olof      (1000) olof      (1000)      421 2023-02-28 12:23:16.000000 fusesoc-2.1/.editorconfig
--rw-r--r--   0 olof      (1000) olof      (1000)       30 2023-02-28 12:28:34.000000 fusesoc-2.1/.flake8
--rw-r--r--   0 olof      (1000) olof      (1000)       85 2023-02-28 12:23:16.000000 fusesoc-2.1/.git-blame-ignore-revs
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.940572 fusesoc-2.1/.github/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.950574 fusesoc-2.1/.github/workflows/
--rw-r--r--   0 olof      (1000) olof      (1000)     1461 2023-02-28 12:28:15.000000 fusesoc-2.1/.github/workflows/ci.yml
--rw-r--r--   0 olof      (1000) olof      (1000)      226 2022-09-29 19:36:09.000000 fusesoc-2.1/.github/workflows/lint.yml
--rw-r--r--   0 olof      (1000) olof      (1000)      227 2022-09-29 19:36:09.000000 fusesoc-2.1/.gitignore
--rw-r--r--   0 olof      (1000) olof      (1000)     1182 2023-02-28 12:32:13.000000 fusesoc-2.1/.pre-commit-config.yaml
--rw-r--r--   0 olof      (1000) olof      (1000)      444 2023-02-28 12:23:16.000000 fusesoc-2.1/.readthedocs.yml
--rw-r--r--   0 olof      (1000) olof      (1000)     1315 2022-09-29 19:36:09.000000 fusesoc-2.1/LICENSE
--rw-r--r--   0 olof      (1000) olof      (1000)    17241 2023-03-23 19:56:33.000000 fusesoc-2.1/NEWS
--rw-r--r--   0 olof      (1000) olof      (1000)     6131 2023-03-23 20:00:47.975579 fusesoc-2.1/PKG-INFO
--rw-r--r--   0 olof      (1000) olof      (1000)     5491 2023-02-28 12:32:13.000000 fusesoc-2.1/README.md
--rw-r--r--   0 olof      (1000) olof      (1000)      259 2023-02-28 12:28:15.000000 fusesoc-2.1/dev-requirements.txt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.950574 fusesoc-2.1/doc/
--rw-r--r--   0 olof      (1000) olof      (1000)       59 2023-02-28 12:23:16.000000 fusesoc-2.1/doc/requirements.txt
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.950574 fusesoc-2.1/doc/source/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.951574 fusesoc-2.1/doc/source/_static/
--rw-r--r--   0 olof      (1000) olof      (1000)      365 2022-09-29 19:36:09.000000 fusesoc-2.1/doc/source/_static/theme_overrides.css
--rw-r--r--   0 olof      (1000) olof      (1000)     6282 2023-02-28 12:28:15.000000 fusesoc-2.1/doc/source/conf.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.951574 fusesoc-2.1/doc/source/dev/
--rw-r--r--   0 olof      (1000) olof      (1000)     4668 2023-02-28 12:28:15.000000 fusesoc-2.1/doc/source/dev/devsetup.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      143 2022-09-29 19:36:09.000000 fusesoc-2.1/doc/source/dev/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      839 2022-09-29 19:36:09.000000 fusesoc-2.1/doc/source/index.rst
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.951574 fusesoc-2.1/doc/source/ref/
--rw-r--r--   0 olof      (1000) olof      (1000)    15496 2023-02-28 12:23:16.000000 fusesoc-2.1/doc/source/ref/capi1.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1723 2023-02-28 12:28:15.000000 fusesoc-2.1/doc/source/ref/glossary.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      175 2023-02-28 12:28:15.000000 fusesoc-2.1/doc/source/ref/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)    10054 2023-02-28 12:23:16.000000 fusesoc-2.1/doc/source/ref/migrations.rst
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.952574 fusesoc-2.1/doc/source/user/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.953574 fusesoc-2.1/doc/source/user/build_system/
--rw-r--r--   0 olof      (1000) olof      (1000)    12263 2023-02-28 12:28:15.000000 fusesoc-2.1/doc/source/user/build_system/core_files.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     7514 2023-02-28 12:23:16.000000 fusesoc-2.1/doc/source/user/build_system/dependencies.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1603 2023-02-28 12:32:13.000000 fusesoc-2.1/doc/source/user/build_system/eda_flows.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     7507 2023-02-28 12:28:34.000000 fusesoc-2.1/doc/source/user/build_system/flags.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     2978 2023-02-28 12:32:13.000000 fusesoc-2.1/doc/source/user/build_system/flow_options.rst
--rw-r--r--   0 olof      (1000) olof      (1000)    12067 2023-02-28 12:32:13.000000 fusesoc-2.1/doc/source/user/build_system/generators.rst
--rw-r--r--   0 olof      (1000) olof      (1000)      129 2022-09-29 19:36:09.000000 fusesoc-2.1/doc/source/user/build_system/hooks.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1902 2023-02-28 12:32:13.000000 fusesoc-2.1/doc/source/user/build_system/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     2267 2023-02-28 12:32:13.000000 fusesoc-2.1/doc/source/user/build_system/tool_options.rst
--rw-r--r--   0 olof      (1000) olof      (1000)       87 2022-09-29 19:36:09.000000 fusesoc-2.1/doc/source/user/build_system/vpi.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1502 2023-02-28 12:28:34.000000 fusesoc-2.1/doc/source/user/cli.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1149 2022-09-29 19:36:09.000000 fusesoc-2.1/doc/source/user/index.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     3941 2023-02-28 12:28:34.000000 fusesoc-2.1/doc/source/user/installation.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     2015 2022-09-29 19:36:09.000000 fusesoc-2.1/doc/source/user/introduction.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     1381 2022-09-29 19:36:09.000000 fusesoc-2.1/doc/source/user/knowledgebase.rst
--rw-r--r--   0 olof      (1000) olof      (1000)     6678 2023-02-28 12:28:34.000000 fusesoc-2.1/doc/source/user/overview.rst
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.953574 fusesoc-2.1/doc/source/user/package_manager/
--rw-r--r--   0 olof      (1000) olof      (1000)     2888 2023-02-28 12:32:13.000000 fusesoc-2.1/doc/source/user/package_manager/index.rst
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.954574 fusesoc-2.1/extras/
--rw-r--r--   0 olof      (1000) olof      (1000)      766 2022-09-29 19:36:09.000000 fusesoc-2.1/extras/bash-completion
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.955575 fusesoc-2.1/fusesoc/
--rw-r--r--   0 olof      (1000) olof      (1000)      250 2022-09-29 19:36:09.000000 fusesoc-2.1/fusesoc/__init__.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.956575 fusesoc-2.1/fusesoc/capi2/
--rw-r--r--   0 olof      (1000) olof      (1000)      141 2022-09-29 19:36:09.000000 fusesoc-2.1/fusesoc/capi2/__init__.py
--rw-r--r--   0 olof      (1000) olof      (1000)    42875 2023-03-23 19:51:07.000000 fusesoc-2.1/fusesoc/capi2/core.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5824 2023-03-23 19:51:07.000000 fusesoc-2.1/fusesoc/capi2/exprs.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2048 2023-02-28 12:32:13.000000 fusesoc-2.1/fusesoc/capi2/generator.py
--rw-r--r--   0 olof      (1000) olof      (1000)     6424 2023-02-28 12:32:13.000000 fusesoc-2.1/fusesoc/config.py
--rw-r--r--   0 olof      (1000) olof      (1000)      340 2023-02-28 12:28:15.000000 fusesoc-2.1/fusesoc/core.py
--rw-r--r--   0 olof      (1000) olof      (1000)    13796 2023-02-28 12:32:13.000000 fusesoc-2.1/fusesoc/coremanager.py
--rw-r--r--   0 olof      (1000) olof      (1000)    25516 2023-03-23 19:51:07.000000 fusesoc-2.1/fusesoc/edalizer.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2870 2023-02-28 12:32:13.000000 fusesoc-2.1/fusesoc/librarymanager.py
--rw-r--r--   0 olof      (1000) olof      (1000)    21973 2023-03-23 19:51:07.000000 fusesoc-2.1/fusesoc/main.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.957575 fusesoc-2.1/fusesoc/provider/
--rw-r--r--   0 olof      (1000) olof      (1000)      279 2023-02-28 12:28:15.000000 fusesoc-2.1/fusesoc/provider/__init__.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2253 2023-02-28 12:53:14.000000 fusesoc-2.1/fusesoc/provider/git.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1364 2023-02-28 12:28:15.000000 fusesoc-2.1/fusesoc/provider/github.py
--rw-r--r--   0 olof      (1000) olof      (1000)      602 2023-02-28 12:28:15.000000 fusesoc-2.1/fusesoc/provider/local.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1188 2022-09-29 19:36:09.000000 fusesoc-2.1/fusesoc/provider/opencores.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2673 2023-02-28 12:28:34.000000 fusesoc-2.1/fusesoc/provider/provider.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1852 2023-02-28 12:28:15.000000 fusesoc-2.1/fusesoc/provider/url.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5392 2023-02-28 12:32:13.000000 fusesoc-2.1/fusesoc/utils.py
--rw-r--r--   0 olof      (1000) olof      (1000)      171 2023-03-23 20:00:47.000000 fusesoc-2.1/fusesoc/version.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5135 2023-02-28 12:28:15.000000 fusesoc-2.1/fusesoc/vlnv.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.956575 fusesoc-2.1/fusesoc.egg-info/
--rw-r--r--   0 olof      (1000) olof      (1000)     6131 2023-03-23 20:00:47.000000 fusesoc-2.1/fusesoc.egg-info/PKG-INFO
--rw-r--r--   0 olof      (1000) olof      (1000)     6373 2023-03-23 20:00:47.000000 fusesoc-2.1/fusesoc.egg-info/SOURCES.txt
--rw-r--r--   0 olof      (1000) olof      (1000)        1 2023-03-23 20:00:47.000000 fusesoc-2.1/fusesoc.egg-info/dependency_links.txt
--rw-r--r--   0 olof      (1000) olof      (1000)       46 2023-03-23 20:00:47.000000 fusesoc-2.1/fusesoc.egg-info/entry_points.txt
--rw-r--r--   0 olof      (1000) olof      (1000)       49 2023-03-23 20:00:47.000000 fusesoc-2.1/fusesoc.egg-info/requires.txt
--rw-r--r--   0 olof      (1000) olof      (1000)        8 2023-03-23 20:00:47.000000 fusesoc-2.1/fusesoc.egg-info/top_level.txt
--rw-r--r--   0 olof      (1000) olof      (1000)       38 2023-03-23 20:00:47.975579 fusesoc-2.1/setup.cfg
--rw-r--r--   0 olof      (1000) olof      (1000)     1645 2023-02-28 12:32:13.000000 fusesoc-2.1/setup.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.958575 fusesoc-2.1/tests/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.944573 fusesoc-2.1/tests/capi2_cores/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.959576 fusesoc-2.1/tests/capi2_cores/deptree/
--rw-r--r--   0 olof      (1000) olof      (1000)      375 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/deptree/child1.core
--rw-r--r--   0 olof      (1000) olof      (1000)      338 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/deptree/child2.core
--rw-r--r--   0 olof      (1000) olof      (1000)      338 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/deptree/child3.core
--rw-r--r--   0 olof      (1000) olof      (1000)      304 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/deptree/child4.core
--rw-r--r--   0 olof      (1000) olof      (1000)     1288 2023-02-28 12:23:16.000000 fusesoc-2.1/tests/capi2_cores/deptree/generated_child_a.core
--rw-r--r--   0 olof      (1000) olof      (1000)      444 2023-02-28 12:23:16.000000 fusesoc-2.1/tests/capi2_cores/deptree/generated_child_a.py
--rw-r--r--   0 olof      (1000) olof      (1000)      802 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/deptree/root.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.959576 fusesoc-2.1/tests/capi2_cores/files_out_of_hierarchy/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2023-02-28 12:23:16.000000 fusesoc-2.1/tests/capi2_cores/files_out_of_hierarchy/bad.sv
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.960576 fusesoc-2.1/tests/capi2_cores/files_out_of_hierarchy/subdir/
--rw-r--r--   0 olof      (1000) olof      (1000)      533 2023-02-28 12:23:16.000000 fusesoc-2.1/tests/capi2_cores/files_out_of_hierarchy/subdir/files_out_of_hierarchy.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2023-02-28 12:23:16.000000 fusesoc-2.1/tests/capi2_cores/files_out_of_hierarchy/subdir/good.sv
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.963576 fusesoc-2.1/tests/capi2_cores/misc/
--rw-r--r--   0 olof      (1000) olof      (1000)      493 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/append.core
--rw-r--r--   0 olof      (1000) olof      (1000)      646 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/depends.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/dontpickthisfile
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/dummy.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/empty.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/f1
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/f2
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/f3
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/f4
--rw-r--r--   0 olof      (1000) olof      (1000)     1496 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/files.core
--rw-r--r--   0 olof      (1000) olof      (1000)      447 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/capi2_cores/misc/flags.core
--rw-r--r--   0 olof      (1000) olof      (1000)      502 2023-02-28 12:28:43.000000 fusesoc-2.1/tests/capi2_cores/misc/flow.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.964576 fusesoc-2.1/tests/capi2_cores/misc/generate/
--rw-r--r--   0 olof      (1000) olof      (1000)       10 2023-02-28 12:32:13.000000 fusesoc-2.1/tests/capi2_cores/misc/generate/file_cachetest
--rw-r--r--   0 olof      (1000) olof      (1000)      914 2023-02-28 12:32:13.000000 fusesoc-2.1/tests/capi2_cores/misc/generate/generate.core
--rw-r--r--   0 olof      (1000) olof      (1000)      375 2023-02-28 12:32:13.000000 fusesoc-2.1/tests/capi2_cores/misc/generate/generators.core
--rw-r--r--   0 olof      (1000) olof      (1000)      553 2023-02-28 12:23:16.000000 fusesoc-2.1/tests/capi2_cores/misc/generate/testgen.py
--rw-r--r--   0 olof      (1000) olof      (1000)      886 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/hooks.core
--rw-r--r--   0 olof      (1000) olof      (1000)     1471 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/parameters.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/scriptfile
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.964576 fusesoc-2.1/tests/capi2_cores/misc/subdir/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/subdir/dummy.extra
--rw-r--r--   0 olof      (1000) olof      (1000)      356 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/targets.core
--rw-r--r--   0 olof      (1000) olof      (1000)      301 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/toplevel.core
--rw-r--r--   0 olof      (1000) olof      (1000)      609 2023-02-28 12:28:34.000000 fusesoc-2.1/tests/capi2_cores/misc/typecheck.core
--rw-r--r--   0 olof      (1000) olof      (1000)      279 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/uncachable.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/vhdlfile
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/vlogfile
--rw-r--r--   0 olof      (1000) olof      (1000)      562 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/vpi.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/capi2_cores/misc/vpifile
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.965577 fusesoc-2.1/tests/capi2_cores/providers/
--rw-r--r--   0 olof      (1000) olof      (1000)      309 2023-02-28 12:28:43.000000 fusesoc-2.1/tests/capi2_cores/providers/url_simple.core
--rw-r--r--   0 olof      (1000) olof      (1000)      348 2023-02-28 12:28:43.000000 fusesoc-2.1/tests/capi2_cores/providers/url_simple_with_user_agent.core
--rw-r--r--   0 olof      (1000) olof      (1000)      308 2023-02-28 12:28:43.000000 fusesoc-2.1/tests/capi2_cores/providers/url_tar.core
--rw-r--r--   0 olof      (1000) olof      (1000)      305 2023-02-28 12:28:43.000000 fusesoc-2.1/tests/capi2_cores/providers/url_zip.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.966577 fusesoc-2.1/tests/capi2_cores/virtual/
--rw-r--r--   0 olof      (1000) olof      (1000)      325 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/capi2_cores/virtual/impl1.core
--rw-r--r--   0 olof      (1000) olof      (1000)      325 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/capi2_cores/virtual/impl2.core
--rw-r--r--   0 olof      (1000) olof      (1000)      349 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/capi2_cores/virtual/user.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.947573 fusesoc-2.1/tests/cores/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.966577 fusesoc-2.1/tests/cores/adv_debug_sys/
--rw-r--r--   0 olof      (1000) olof      (1000)     1225 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/adv_debug_sys/adv_debug_sys.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.966577 fusesoc-2.1/tests/cores/atlys/
--rw-r--r--   0 olof      (1000) olof      (1000)     2269 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/atlys/atlys.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.966577 fusesoc-2.1/tests/cores/atlys/data/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/atlys/data/atlys.ucf
--rw-r--r--   0 olof      (1000) olof      (1000)      176 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/atlys/data/dummy_backend_tcl_file.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.967577 fusesoc-2.1/tests/cores/elf-loader/
--rwxr-xr-x   0 olof      (1000) olof      (1000)      184 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/elf-loader/check_libelf.sh
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/elf-loader/elf-loader.c
--rw-r--r--   0 olof      (1000) olof      (1000)     1458 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/elf-loader/elf-loader.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/elf-loader/vpi_wrapper.c
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.967577 fusesoc-2.1/tests/cores/gpio/
--rw-r--r--   0 olof      (1000) olof      (1000)      379 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/gpio/gpio.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.967577 fusesoc-2.1/tests/cores/jtag_tap/
--rw-r--r--   0 olof      (1000) olof      (1000)      474 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/jtag_tap/jtag_tap-1.13.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.967577 fusesoc-2.1/tests/cores/libstorage/
--rw-r--r--   0 olof      (1000) olof      (1000)      529 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/libstorage/libstorage-1.0.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.969577 fusesoc-2.1/tests/cores/misc/
--rw-r--r--   0 olof      (1000) olof      (1000)     1051 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/misc/c3demo.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/c3demo.pcf
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.970578 fusesoc-2.1/tests/cores/misc/copytocore/
--rw-r--r--   0 olof      (1000) olof      (1000)      421 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/copytocore/copytocore.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/copytocore/dummy.tcl
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.970578 fusesoc-2.1/tests/cores/misc/copytocore/subdir/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/copytocore/subdir/dummy.extra
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/dummy.tcl
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/dummy.xci
--rw-r--r--   0 olof      (1000) olof      (1000)      854 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/misc/filetypes.core
--rw-r--r--   0 olof      (1000) olof      (1000)     1391 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/misc/ghdltest.core
--rw-r--r--   0 olof      (1000) olof      (1000)      356 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/misc/gitcore.core
--rw-r--r--   0 olof      (1000) olof      (1000)      698 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/misc/no_exe_script.core
--rw-r--r--   0 olof      (1000) olof      (1000)      234 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/misc/nomain.core
--rw-r--r--   0 olof      (1000) olof      (1000)      399 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/misc/opencorescore.core
--rw-r--r--   0 olof      (1000) olof      (1000)     2482 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/misc/paramtest.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.970578 fusesoc-2.1/tests/cores/misc/scripts/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/scripts/no_exe_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      192 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/scripts/post_build_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      173 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/scripts/post_run_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      191 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/scripts/pre_build_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      172 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/scripts/pre_run_script
--rw-r--r--   0 olof      (1000) olof      (1000)     1474 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/misc/scriptscore.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.970578 fusesoc-2.1/tests/cores/misc/subdir/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/misc/subdir/dummy.extra
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.970578 fusesoc-2.1/tests/cores/mor1kx/
--rw-r--r--   0 olof      (1000) olof      (1000)     2807 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/mor1kx/mor1kx-3.1.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.971578 fusesoc-2.1/tests/cores/mor1kx-arty/
--rw-r--r--   0 olof      (1000) olof      (1000)      702 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/mor1kx-arty/mor1kx-arty.core
--rw-r--r--   0 olof      (1000) olof      (1000)      337 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/mor1kx-arty/mor1kx-arty.system
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.971578 fusesoc-2.1/tests/cores/mor1kx-generic/
--rw-r--r--   0 olof      (1000) olof      (1000)     3024 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/mor1kx-generic/mor1kx-generic.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.971578 fusesoc-2.1/tests/cores/mor1kx-generic/scripts/
--rwxr-xr-x   0 olof      (1000) olof      (1000)      173 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/mor1kx-generic/scripts/post_run_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      174 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/mor1kx-generic/scripts/pre_build_script
--rwxr-xr-x   0 olof      (1000) olof      (1000)      172 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/mor1kx-generic/scripts/pre_run_script
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.971578 fusesoc-2.1/tests/cores/sockit/
--rw-r--r--   0 olof      (1000) olof      (1000)     1596 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/sockit/sockit.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.971578 fusesoc-2.1/tests/cores/uart16550/
--rw-r--r--   0 olof      (1000) olof      (1000)      920 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/uart16550/uart16550-1.5.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.972578 fusesoc-2.1/tests/cores/verilator_tb_utils/
--rw-r--r--   0 olof      (1000) olof      (1000)      715 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/verilator_tb_utils/verilator_tb_utils.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.972578 fusesoc-2.1/tests/cores/verilog-arbiter/
--rw-r--r--   0 olof      (1000) olof      (1000)      761 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/verilog-arbiter/verilog-arbiter-r1.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.972578 fusesoc-2.1/tests/cores/verilog_utils/
--rw-r--r--   0 olof      (1000) olof      (1000)      573 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/verilog_utils/verilog_utils.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/verilog_utils/verilog_utils.vh
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.972578 fusesoc-2.1/tests/cores/vga_lcd/
--rw-r--r--   0 olof      (1000) olof      (1000)     1200 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/vga_lcd/vga_lcd.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.972578 fusesoc-2.1/tests/cores/vlog_tb_utils/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.972578 fusesoc-2.1/tests/cores/vlog_tb_utils/files/
--rw-r--r--   0 olof      (1000) olof      (1000)      554 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/vlog_tb_utils/files/0001-testpatch.patch
--rw-r--r--   0 olof      (1000) olof      (1000)     1456 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/vlog_tb_utils/vlog_tb_utils-1.1.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.973578 fusesoc-2.1/tests/cores/wb_common/
--rw-r--r--   0 olof      (1000) olof      (1000)      655 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/wb_common/wb_common.core
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/wb_common/wb_common.v
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/wb_common/wb_common_params.v
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.973578 fusesoc-2.1/tests/cores/wb_intercon/
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/cores/wb_intercon/dummy_icarus.v
--rw-r--r--   0 olof      (1000) olof      (1000)     1329 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/cores/wb_intercon/wb_intercon-1.0.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.973578 fusesoc-2.1/tests/test_capi2/
--rw-r--r--   0 olof      (1000) olof      (1000)       90 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/test_capi2/generators.info
--rw-r--r--   0 olof      (1000) olof      (1000)      207 2023-02-28 12:28:15.000000 fusesoc-2.1/tests/test_capi2/targets.info
--rw-r--r--   0 olof      (1000) olof      (1000)    17622 2023-03-23 19:51:07.000000 fusesoc-2.1/tests/test_capi2.py
--rw-r--r--   0 olof      (1000) olof      (1000)      335 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/test_common.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2230 2023-02-28 12:28:34.000000 fusesoc-2.1/tests/test_config.py
--rw-r--r--   0 olof      (1000) olof      (1000)     7657 2023-03-23 19:51:07.000000 fusesoc-2.1/tests/test_coremanager.py
--rw-r--r--   0 olof      (1000) olof      (1000)     3988 2023-03-23 19:51:07.000000 fusesoc-2.1/tests/test_edalizer.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1619 2023-03-23 19:51:07.000000 fusesoc-2.1/tests/test_exprs.py
--rw-r--r--   0 olof      (1000) olof      (1000)     1484 2023-02-28 12:28:34.000000 fusesoc-2.1/tests/test_ignored_dirs.py
--rw-r--r--   0 olof      (1000) olof      (1000)     5516 2023-02-28 12:32:13.000000 fusesoc-2.1/tests/test_libraries.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.974578 fusesoc-2.1/tests/test_provider/
--rw-r--r--   0 olof      (1000) olof      (1000)      114 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/test_provider/file.tar.gz
--rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/test_provider/file.v
--rw-r--r--   0 olof      (1000) olof      (1000)      162 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/test_provider/file.zip
--rw-r--r--   0 olof      (1000) olof      (1000)     1141 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/test_provider/vlog_functions.v
--rw-r--r--   0 olof      (1000) olof      (1000)     2746 2023-02-28 12:32:13.000000 fusesoc-2.1/tests/test_provider.py
--rw-r--r--   0 olof      (1000) olof      (1000)     2177 2023-02-28 12:23:16.000000 fusesoc-2.1/tests/test_vlnv.py
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.948573 fusesoc-2.1/tests/userguide/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.974578 fusesoc-2.1/tests/userguide/blinky/
--rw-r--r--   0 olof      (1000) olof      (1000)     1743 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/userguide/blinky/blinky.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.974578 fusesoc-2.1/tests/userguide/blinky/data/
--rw-r--r--   0 olof      (1000) olof      (1000)      458 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/userguide/blinky/data/nexys_video.xdc
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.974578 fusesoc-2.1/tests/userguide/blinky/rtl/
--rw-r--r--   0 olof      (1000) olof      (1000)      636 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/userguide/blinky/rtl/blinky.sv
--rw-r--r--   0 olof      (1000) olof      (1000)      153 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/userguide/blinky/rtl/macros.svh
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.974578 fusesoc-2.1/tests/userguide/blinky/tb/
--rw-r--r--   0 olof      (1000) olof      (1000)     1031 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/userguide/blinky/tb/blinky_tb.sv
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.975579 fusesoc-2.1/tests/userguide/dualblinky/
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.975579 fusesoc-2.1/tests/userguide/dualblinky/data/
--rw-r--r--   0 olof      (1000) olof      (1000)      574 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/userguide/dualblinky/data/nexys_video.xdc
--rw-r--r--   0 olof      (1000) olof      (1000)      792 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/userguide/dualblinky/dualblinky.core
-drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-03-23 20:00:47.975579 fusesoc-2.1/tests/userguide/dualblinky/rtl/
--rw-r--r--   0 olof      (1000) olof      (1000)      665 2022-09-29 19:36:09.000000 fusesoc-2.1/tests/userguide/dualblinky/rtl/dualblinky.sv
--rw-r--r--   0 olof      (1000) olof      (1000)     3014 2023-02-28 12:32:13.000000 fusesoc-2.1/tox.ini
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.593973 fusesoc-2.2/
+-rw-r--r--   0 olof      (1000) olof      (1000)      421 2023-02-28 12:23:16.000000 fusesoc-2.2/.editorconfig
+-rw-r--r--   0 olof      (1000) olof      (1000)       30 2023-02-28 12:28:34.000000 fusesoc-2.2/.flake8
+-rw-r--r--   0 olof      (1000) olof      (1000)       85 2023-02-28 12:23:16.000000 fusesoc-2.2/.git-blame-ignore-revs
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.530973 fusesoc-2.2/.github/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.544973 fusesoc-2.2/.github/workflows/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1461 2023-02-28 12:28:15.000000 fusesoc-2.2/.github/workflows/ci.yml
+-rw-r--r--   0 olof      (1000) olof      (1000)      226 2022-09-29 19:36:09.000000 fusesoc-2.2/.github/workflows/lint.yml
+-rw-r--r--   0 olof      (1000) olof      (1000)      227 2022-09-29 19:36:09.000000 fusesoc-2.2/.gitignore
+-rw-r--r--   0 olof      (1000) olof      (1000)     1182 2023-02-28 12:32:13.000000 fusesoc-2.2/.pre-commit-config.yaml
+-rw-r--r--   0 olof      (1000) olof      (1000)      444 2023-02-28 12:23:16.000000 fusesoc-2.2/.readthedocs.yml
+-rw-r--r--   0 olof      (1000) olof      (1000)     1315 2022-09-29 19:36:09.000000 fusesoc-2.2/LICENSE
+-rw-r--r--   0 olof      (1000) olof      (1000)    17659 2023-04-18 10:07:10.000000 fusesoc-2.2/NEWS
+-rw-r--r--   0 olof      (1000) olof      (1000)     6131 2023-04-18 10:07:46.592973 fusesoc-2.2/PKG-INFO
+-rw-r--r--   0 olof      (1000) olof      (1000)     5491 2023-02-28 12:32:13.000000 fusesoc-2.2/README.md
+-rw-r--r--   0 olof      (1000) olof      (1000)      259 2023-02-28 12:28:15.000000 fusesoc-2.2/dev-requirements.txt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.544973 fusesoc-2.2/doc/
+-rw-r--r--   0 olof      (1000) olof      (1000)       59 2023-02-28 12:23:16.000000 fusesoc-2.2/doc/requirements.txt
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.545973 fusesoc-2.2/doc/source/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.545973 fusesoc-2.2/doc/source/_static/
+-rw-r--r--   0 olof      (1000) olof      (1000)      365 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/_static/theme_overrides.css
+-rw-r--r--   0 olof      (1000) olof      (1000)     6282 2023-02-28 12:28:15.000000 fusesoc-2.2/doc/source/conf.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.545973 fusesoc-2.2/doc/source/dev/
+-rw-r--r--   0 olof      (1000) olof      (1000)     4668 2023-02-28 12:28:15.000000 fusesoc-2.2/doc/source/dev/devsetup.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      143 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/dev/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      839 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/index.rst
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.546973 fusesoc-2.2/doc/source/ref/
+-rw-r--r--   0 olof      (1000) olof      (1000)    15496 2023-02-28 12:23:16.000000 fusesoc-2.2/doc/source/ref/capi1.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1723 2023-02-28 12:28:15.000000 fusesoc-2.2/doc/source/ref/glossary.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      175 2023-02-28 12:28:15.000000 fusesoc-2.2/doc/source/ref/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)    10054 2023-02-28 12:23:16.000000 fusesoc-2.2/doc/source/ref/migrations.rst
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.548973 fusesoc-2.2/doc/source/user/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.550973 fusesoc-2.2/doc/source/user/build_system/
+-rw-r--r--   0 olof      (1000) olof      (1000)    12263 2023-02-28 12:28:15.000000 fusesoc-2.2/doc/source/user/build_system/core_files.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     7514 2023-02-28 12:23:16.000000 fusesoc-2.2/doc/source/user/build_system/dependencies.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1603 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/build_system/eda_flows.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     7507 2023-02-28 12:28:34.000000 fusesoc-2.2/doc/source/user/build_system/flags.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     2978 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/build_system/flow_options.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)    12067 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/build_system/generators.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)      129 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/user/build_system/hooks.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1902 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/build_system/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     2267 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/build_system/tool_options.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)       87 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/user/build_system/vpi.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1502 2023-02-28 12:28:34.000000 fusesoc-2.2/doc/source/user/cli.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1149 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/user/index.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     4013 2023-04-17 12:12:08.000000 fusesoc-2.2/doc/source/user/installation.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     2015 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/user/introduction.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     1381 2022-09-29 19:36:09.000000 fusesoc-2.2/doc/source/user/knowledgebase.rst
+-rw-r--r--   0 olof      (1000) olof      (1000)     6678 2023-02-28 12:28:34.000000 fusesoc-2.2/doc/source/user/overview.rst
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.551973 fusesoc-2.2/doc/source/user/package_manager/
+-rw-r--r--   0 olof      (1000) olof      (1000)     2888 2023-02-28 12:32:13.000000 fusesoc-2.2/doc/source/user/package_manager/index.rst
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.551973 fusesoc-2.2/extras/
+-rw-r--r--   0 olof      (1000) olof      (1000)      766 2022-09-29 19:36:09.000000 fusesoc-2.2/extras/bash-completion
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.553973 fusesoc-2.2/fusesoc/
+-rw-r--r--   0 olof      (1000) olof      (1000)      250 2022-09-29 19:36:09.000000 fusesoc-2.2/fusesoc/__init__.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.557973 fusesoc-2.2/fusesoc/capi2/
+-rw-r--r--   0 olof      (1000) olof      (1000)      141 2022-09-29 19:36:09.000000 fusesoc-2.2/fusesoc/capi2/__init__.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    21425 2023-04-18 10:07:10.000000 fusesoc-2.2/fusesoc/capi2/core.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5895 2023-04-18 10:07:10.000000 fusesoc-2.2/fusesoc/capi2/coredata.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      720 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/capi2/coreparser.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5825 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/capi2/exprs.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2046 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/capi2/generator.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    22016 2023-04-18 10:07:10.000000 fusesoc-2.2/fusesoc/capi2/json_schema.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     6424 2023-02-28 12:32:13.000000 fusesoc-2.2/fusesoc/config.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      340 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/core.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    14081 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/coremanager.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    25699 2023-04-17 12:20:14.000000 fusesoc-2.2/fusesoc/edalizer.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2870 2023-02-28 12:32:13.000000 fusesoc-2.2/fusesoc/librarymanager.py
+-rw-r--r--   0 olof      (1000) olof      (1000)    22647 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/main.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.557973 fusesoc-2.2/fusesoc/parser/
+-rw-r--r--   0 olof      (1000) olof      (1000)      141 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/parser/__init__.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2335 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/parser/coreparser.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.559973 fusesoc-2.2/fusesoc/provider/
+-rw-r--r--   0 olof      (1000) olof      (1000)      279 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/provider/__init__.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2253 2023-02-28 12:53:14.000000 fusesoc-2.2/fusesoc/provider/git.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1364 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/provider/github.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      602 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/provider/local.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1188 2022-09-29 19:36:09.000000 fusesoc-2.2/fusesoc/provider/opencores.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2673 2023-02-28 12:28:34.000000 fusesoc-2.2/fusesoc/provider/provider.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1852 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/provider/url.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5521 2023-04-17 12:12:08.000000 fusesoc-2.2/fusesoc/utils.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      171 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc/version.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5135 2023-02-28 12:28:15.000000 fusesoc-2.2/fusesoc/vlnv.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.554973 fusesoc-2.2/fusesoc.egg-info/
+-rw-r--r--   0 olof      (1000) olof      (1000)     6131 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/PKG-INFO
+-rw-r--r--   0 olof      (1000) olof      (1000)     6624 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/SOURCES.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)        1 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/dependency_links.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)       46 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/entry_points.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)       64 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/requires.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)        8 2023-04-18 10:07:46.000000 fusesoc-2.2/fusesoc.egg-info/top_level.txt
+-rw-r--r--   0 olof      (1000) olof      (1000)       38 2023-04-18 10:07:46.593973 fusesoc-2.2/setup.cfg
+-rw-r--r--   0 olof      (1000) olof      (1000)     1689 2023-04-17 12:12:08.000000 fusesoc-2.2/setup.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.562973 fusesoc-2.2/tests/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.533973 fusesoc-2.2/tests/capi2_cores/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.564973 fusesoc-2.2/tests/capi2_cores/deptree/
+-rw-r--r--   0 olof      (1000) olof      (1000)      375 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/deptree/child1.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      338 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/deptree/child2.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      338 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/deptree/child3.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      304 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/deptree/child4.core
+-rw-r--r--   0 olof      (1000) olof      (1000)     1288 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/deptree/generated_child_a.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      444 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/deptree/generated_child_a.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      802 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/deptree/root.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.564973 fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/bad.sv
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.565973 fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/subdir/
+-rw-r--r--   0 olof      (1000) olof      (1000)      533 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/subdir/files_out_of_hierarchy.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/subdir/good.sv
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.572973 fusesoc-2.2/tests/capi2_cores/misc/
+-rw-r--r--   0 olof      (1000) olof      (1000)      493 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/append.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      646 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/depends.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/dontpickthisfile
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/dummy.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/empty.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/f1
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/f2
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/f3
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/f4
+-rw-r--r--   0 olof      (1000) olof      (1000)     1496 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/files.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      447 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/capi2_cores/misc/flags.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      502 2023-02-28 12:28:43.000000 fusesoc-2.2/tests/capi2_cores/misc/flow.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.573973 fusesoc-2.2/tests/capi2_cores/misc/generate/
+-rw-r--r--   0 olof      (1000) olof      (1000)       10 2023-02-28 12:32:13.000000 fusesoc-2.2/tests/capi2_cores/misc/generate/file_cachetest
+-rw-r--r--   0 olof      (1000) olof      (1000)      914 2023-02-28 12:32:13.000000 fusesoc-2.2/tests/capi2_cores/misc/generate/generate.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      375 2023-02-28 12:32:13.000000 fusesoc-2.2/tests/capi2_cores/misc/generate/generators.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      553 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/capi2_cores/misc/generate/testgen.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      886 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/hooks.core
+-rw-r--r--   0 olof      (1000) olof      (1000)     1471 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/parameters.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/scriptfile
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.574973 fusesoc-2.2/tests/capi2_cores/misc/subdir/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/subdir/dummy.extra
+-rw-r--r--   0 olof      (1000) olof      (1000)      356 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/targets.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      301 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/toplevel.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      609 2023-02-28 12:28:34.000000 fusesoc-2.2/tests/capi2_cores/misc/typecheck.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      244 2023-04-17 12:12:08.000000 fusesoc-2.2/tests/capi2_cores/misc/uncachable.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/vhdlfile
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/vlogfile
+-rw-r--r--   0 olof      (1000) olof      (1000)      562 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/vpi.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/capi2_cores/misc/vpifile
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.574973 fusesoc-2.2/tests/capi2_cores/parser/
+-rw-r--r--   0 olof      (1000) olof      (1000)      334 2023-04-17 12:12:08.000000 fusesoc-2.2/tests/capi2_cores/parser/no_additional_properties.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      482 2023-04-17 12:12:08.000000 fusesoc-2.2/tests/capi2_cores/parser/with_additional_properties.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.576973 fusesoc-2.2/tests/capi2_cores/providers/
+-rw-r--r--   0 olof      (1000) olof      (1000)      309 2023-02-28 12:28:43.000000 fusesoc-2.2/tests/capi2_cores/providers/url_simple.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      348 2023-02-28 12:28:43.000000 fusesoc-2.2/tests/capi2_cores/providers/url_simple_with_user_agent.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      308 2023-02-28 12:28:43.000000 fusesoc-2.2/tests/capi2_cores/providers/url_tar.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      305 2023-02-28 12:28:43.000000 fusesoc-2.2/tests/capi2_cores/providers/url_zip.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.577973 fusesoc-2.2/tests/capi2_cores/virtual/
+-rw-r--r--   0 olof      (1000) olof      (1000)      325 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/capi2_cores/virtual/impl1.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      325 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/capi2_cores/virtual/impl2.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      349 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/capi2_cores/virtual/user.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.539973 fusesoc-2.2/tests/cores/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.577973 fusesoc-2.2/tests/cores/adv_debug_sys/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1225 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/adv_debug_sys/adv_debug_sys.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.577973 fusesoc-2.2/tests/cores/atlys/
+-rw-r--r--   0 olof      (1000) olof      (1000)     2269 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/atlys/atlys.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.578973 fusesoc-2.2/tests/cores/atlys/data/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/atlys/data/atlys.ucf
+-rw-r--r--   0 olof      (1000) olof      (1000)      176 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/atlys/data/dummy_backend_tcl_file.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.579973 fusesoc-2.2/tests/cores/elf-loader/
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      184 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/elf-loader/check_libelf.sh
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/elf-loader/elf-loader.c
+-rw-r--r--   0 olof      (1000) olof      (1000)     1458 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/elf-loader/elf-loader.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/elf-loader/vpi_wrapper.c
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.579973 fusesoc-2.2/tests/cores/gpio/
+-rw-r--r--   0 olof      (1000) olof      (1000)      379 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/gpio/gpio.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.579973 fusesoc-2.2/tests/cores/jtag_tap/
+-rw-r--r--   0 olof      (1000) olof      (1000)      474 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/jtag_tap/jtag_tap-1.13.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.580973 fusesoc-2.2/tests/cores/libstorage/
+-rw-r--r--   0 olof      (1000) olof      (1000)      529 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/libstorage/libstorage-1.0.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.583973 fusesoc-2.2/tests/cores/misc/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1051 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/c3demo.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/c3demo.pcf
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.583973 fusesoc-2.2/tests/cores/misc/copytocore/
+-rw-r--r--   0 olof      (1000) olof      (1000)      421 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/copytocore/copytocore.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/copytocore/dummy.tcl
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.583973 fusesoc-2.2/tests/cores/misc/copytocore/subdir/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/copytocore/subdir/dummy.extra
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/dummy.tcl
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/dummy.xci
+-rw-r--r--   0 olof      (1000) olof      (1000)      854 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/filetypes.core
+-rw-r--r--   0 olof      (1000) olof      (1000)     1391 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/ghdltest.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      356 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/gitcore.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      698 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/no_exe_script.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      234 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/nomain.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      399 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/opencorescore.core
+-rw-r--r--   0 olof      (1000) olof      (1000)     2482 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/paramtest.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.584973 fusesoc-2.2/tests/cores/misc/scripts/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/scripts/no_exe_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      192 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/scripts/post_build_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      173 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/scripts/post_run_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      191 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/scripts/pre_build_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      172 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/scripts/pre_run_script
+-rw-r--r--   0 olof      (1000) olof      (1000)     1474 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/misc/scriptscore.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.584973 fusesoc-2.2/tests/cores/misc/subdir/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/misc/subdir/dummy.extra
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.585973 fusesoc-2.2/tests/cores/mor1kx/
+-rw-r--r--   0 olof      (1000) olof      (1000)     2807 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/mor1kx/mor1kx-3.1.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.585973 fusesoc-2.2/tests/cores/mor1kx-arty/
+-rw-r--r--   0 olof      (1000) olof      (1000)      702 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/mor1kx-arty/mor1kx-arty.core
+-rw-r--r--   0 olof      (1000) olof      (1000)      337 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/mor1kx-arty/mor1kx-arty.system
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.585973 fusesoc-2.2/tests/cores/mor1kx-generic/
+-rw-r--r--   0 olof      (1000) olof      (1000)     3024 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/mor1kx-generic/mor1kx-generic.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.586973 fusesoc-2.2/tests/cores/mor1kx-generic/scripts/
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      173 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/mor1kx-generic/scripts/post_run_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      174 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/mor1kx-generic/scripts/pre_build_script
+-rwxr-xr-x   0 olof      (1000) olof      (1000)      172 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/mor1kx-generic/scripts/pre_run_script
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.586973 fusesoc-2.2/tests/cores/sockit/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1596 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/sockit/sockit.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.586973 fusesoc-2.2/tests/cores/uart16550/
+-rw-r--r--   0 olof      (1000) olof      (1000)      920 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/uart16550/uart16550-1.5.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.587973 fusesoc-2.2/tests/cores/verilator_tb_utils/
+-rw-r--r--   0 olof      (1000) olof      (1000)      715 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/verilator_tb_utils/verilator_tb_utils.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.587973 fusesoc-2.2/tests/cores/verilog-arbiter/
+-rw-r--r--   0 olof      (1000) olof      (1000)      761 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/verilog-arbiter/verilog-arbiter-r1.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.588973 fusesoc-2.2/tests/cores/verilog_utils/
+-rw-r--r--   0 olof      (1000) olof      (1000)      573 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/verilog_utils/verilog_utils.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/verilog_utils/verilog_utils.vh
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.588973 fusesoc-2.2/tests/cores/vga_lcd/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1200 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/vga_lcd/vga_lcd.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.588973 fusesoc-2.2/tests/cores/vlog_tb_utils/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.588973 fusesoc-2.2/tests/cores/vlog_tb_utils/files/
+-rw-r--r--   0 olof      (1000) olof      (1000)      554 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/vlog_tb_utils/files/0001-testpatch.patch
+-rw-r--r--   0 olof      (1000) olof      (1000)     1456 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/vlog_tb_utils/vlog_tb_utils-1.1.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.589973 fusesoc-2.2/tests/cores/wb_common/
+-rw-r--r--   0 olof      (1000) olof      (1000)      655 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/wb_common/wb_common.core
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/wb_common/wb_common.v
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/wb_common/wb_common_params.v
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.589973 fusesoc-2.2/tests/cores/wb_intercon/
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/cores/wb_intercon/dummy_icarus.v
+-rw-r--r--   0 olof      (1000) olof      (1000)     1329 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/cores/wb_intercon/wb_intercon-1.0.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.590973 fusesoc-2.2/tests/test_capi2/
+-rw-r--r--   0 olof      (1000) olof      (1000)       90 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/test_capi2/generators.info
+-rw-r--r--   0 olof      (1000) olof      (1000)      207 2023-02-28 12:28:15.000000 fusesoc-2.2/tests/test_capi2/targets.info
+-rw-r--r--   0 olof      (1000) olof      (1000)    21205 2023-04-17 12:27:19.000000 fusesoc-2.2/tests/test_capi2.py
+-rw-r--r--   0 olof      (1000) olof      (1000)      335 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/test_common.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2230 2023-02-28 12:28:34.000000 fusesoc-2.2/tests/test_config.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     7657 2023-03-23 19:51:07.000000 fusesoc-2.2/tests/test_coremanager.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     3988 2023-03-23 19:51:07.000000 fusesoc-2.2/tests/test_edalizer.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1619 2023-03-23 19:51:07.000000 fusesoc-2.2/tests/test_exprs.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     1484 2023-02-28 12:28:34.000000 fusesoc-2.2/tests/test_ignored_dirs.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     5516 2023-02-28 12:32:13.000000 fusesoc-2.2/tests/test_libraries.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.590973 fusesoc-2.2/tests/test_provider/
+-rw-r--r--   0 olof      (1000) olof      (1000)      114 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/test_provider/file.tar.gz
+-rw-r--r--   0 olof      (1000) olof      (1000)        0 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/test_provider/file.v
+-rw-r--r--   0 olof      (1000) olof      (1000)      162 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/test_provider/file.zip
+-rw-r--r--   0 olof      (1000) olof      (1000)     1141 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/test_provider/vlog_functions.v
+-rw-r--r--   0 olof      (1000) olof      (1000)     3000 2023-04-17 12:12:08.000000 fusesoc-2.2/tests/test_provider.py
+-rw-r--r--   0 olof      (1000) olof      (1000)     2177 2023-02-28 12:23:16.000000 fusesoc-2.2/tests/test_vlnv.py
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.540973 fusesoc-2.2/tests/userguide/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.591973 fusesoc-2.2/tests/userguide/blinky/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1743 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/blinky/blinky.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.591973 fusesoc-2.2/tests/userguide/blinky/data/
+-rw-r--r--   0 olof      (1000) olof      (1000)      458 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/blinky/data/nexys_video.xdc
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.591973 fusesoc-2.2/tests/userguide/blinky/rtl/
+-rw-r--r--   0 olof      (1000) olof      (1000)      636 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/blinky/rtl/blinky.sv
+-rw-r--r--   0 olof      (1000) olof      (1000)      153 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/blinky/rtl/macros.svh
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.592973 fusesoc-2.2/tests/userguide/blinky/tb/
+-rw-r--r--   0 olof      (1000) olof      (1000)     1031 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/blinky/tb/blinky_tb.sv
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.592973 fusesoc-2.2/tests/userguide/dualblinky/
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.592973 fusesoc-2.2/tests/userguide/dualblinky/data/
+-rw-r--r--   0 olof      (1000) olof      (1000)      574 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/dualblinky/data/nexys_video.xdc
+-rw-r--r--   0 olof      (1000) olof      (1000)      792 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/dualblinky/dualblinky.core
+drwxr-xr-x   0 olof      (1000) olof      (1000)        0 2023-04-18 10:07:46.592973 fusesoc-2.2/tests/userguide/dualblinky/rtl/
+-rw-r--r--   0 olof      (1000) olof      (1000)      665 2022-09-29 19:36:09.000000 fusesoc-2.2/tests/userguide/dualblinky/rtl/dualblinky.sv
+-rw-r--r--   0 olof      (1000) olof      (1000)     3014 2023-02-28 12:32:13.000000 fusesoc-2.2/tox.ini
```

### Comparing `fusesoc-2.1/.github/workflows/ci.yml` & `fusesoc-2.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/.pre-commit-config.yaml` & `fusesoc-2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/LICENSE` & `fusesoc-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/NEWS` & `fusesoc-2.2/NEWS`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+2.2 2023-04-18 Olof Kindgren <olof.kindgren@gmail.com>
+======================================================
+* Use jsonschema to describe anv validate CAPI2 files
+* Add switch to allow additional CAPI2 properties
+* Support use expansion everywhere
+* Support setting tags on files
+
+Contributors:
+Erik Waling <erik.waling@gmail.com>
+Olof Kindgren <olof.kindgren@gmail.com>
+Patcharapol Sankaew <meen.sankaew@gmail.com>
+
 2.1 2023-03-23 Olof Kindgren <olof.kindgren@gmail.com>
 ======================================================
 * Add caching of generators
 * Allow setting library version when adding libraries
 * Allow cloning repos that don't support shallow clones
 * Avoid cleaning out existing work roots
 * Only re-export changed files
```

### Comparing `fusesoc-2.1/PKG-INFO` & `fusesoc-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusesoc
-Version: 2.1
+Version: 2.2
 Summary: FuseSoC is a package manager and a set of build tools for HDL (Hardware Description Language) code.
 Home-page: https://github.com/olofk/fusesoc
 Author: Olof Kindgren
 Author-email: olof.kindgren@gmail.com
 License: BSD-2-Clause
 Keywords: VHDL,verilog,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fusesoc-2.1/README.md` & `fusesoc-2.2/README.md`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/conf.py` & `fusesoc-2.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/dev/devsetup.rst` & `fusesoc-2.2/doc/source/dev/devsetup.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/index.rst` & `fusesoc-2.2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/ref/capi1.rst` & `fusesoc-2.2/doc/source/ref/capi1.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/ref/glossary.rst` & `fusesoc-2.2/doc/source/ref/glossary.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/ref/migrations.rst` & `fusesoc-2.2/doc/source/ref/migrations.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/build_system/core_files.rst` & `fusesoc-2.2/doc/source/user/build_system/core_files.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/build_system/dependencies.rst` & `fusesoc-2.2/doc/source/user/build_system/dependencies.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/build_system/eda_flows.rst` & `fusesoc-2.2/doc/source/user/build_system/eda_flows.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/build_system/flags.rst` & `fusesoc-2.2/doc/source/user/build_system/flags.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/build_system/flow_options.rst` & `fusesoc-2.2/doc/source/user/build_system/flow_options.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/build_system/generators.rst` & `fusesoc-2.2/doc/source/user/build_system/generators.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/build_system/index.rst` & `fusesoc-2.2/doc/source/user/build_system/index.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/build_system/tool_options.rst` & `fusesoc-2.2/doc/source/user/build_system/tool_options.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/cli.rst` & `fusesoc-2.2/doc/source/user/cli.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/index.rst` & `fusesoc-2.2/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/installation.rst` & `fusesoc-2.2/doc/source/user/installation.rst`

 * *Files 4% similar despite different names*

```diff
@@ -117,10 +117,12 @@
 
    $ pip3 uninstall fusesoc
 
 
 Installation under macOS
 ========================
 
-.. todo::
+You can use ``pip`` to install as same as Linux.
 
-    Add macOS installation instructions.
+.. code-block:: shell-session
+
+   $ pip3 install --upgrade --user fusesoc
```

### Comparing `fusesoc-2.1/doc/source/user/introduction.rst` & `fusesoc-2.2/doc/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/knowledgebase.rst` & `fusesoc-2.2/doc/source/user/knowledgebase.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/overview.rst` & `fusesoc-2.2/doc/source/user/overview.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/doc/source/user/package_manager/index.rst` & `fusesoc-2.2/doc/source/user/package_manager/index.rst`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/extras/bash-completion` & `fusesoc-2.2/extras/bash-completion`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/fusesoc/capi2/exprs.py` & `fusesoc-2.2/fusesoc/capi2/exprs.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     To avoid creating the parser repeatedly, this function is memoized.
 
     """
     global _PARSER
     if _PARSER is not None:
         return _PARSER
 
-    word = Word(alphanums + '`:<>.[]_-,=~/^+"')
+    word = Word(alphanums + '`:<>.[]_-,=~/^+"$')
     exprs = Forward()
 
     conditional = (
         Optional("!")
         + word
         + Suppress("?")
         + Suppress("(")
```

### Comparing `fusesoc-2.1/fusesoc/capi2/generator.py` & `fusesoc-2.2/fusesoc/capi2/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     def write(self):
         coredata = {
             "name": self.vlnv,
             "filesets": self.filesets,
             "parameters": self.parameters,
             "targets": self.targets,
         }
-        return utils.yaml_fwrite(self.core_file, coredata, "CAPI=2:\n")
+        return utils.yaml_fwrite(self.core_file, coredata, "CAPI=2:")
```

### Comparing `fusesoc-2.1/fusesoc/config.py` & `fusesoc-2.2/fusesoc/config.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/fusesoc/coremanager.py` & `fusesoc-2.2/fusesoc/coremanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from simplesat.constraints import PrettyPackageStringParser, Requirement
 from simplesat.dependency_solver import DependencySolver
 from simplesat.errors import NoPackageFound, SatisfiabilityError
 from simplesat.pool import Pool
 from simplesat.repository import Repository
 from simplesat.request import Request
 
+from fusesoc.capi2.coreparser import Core2Parser
 from fusesoc.core import Core
 from fusesoc.librarymanager import LibraryManager
 
 logger = logging.getLogger(__name__)
 
 
 class DependencyError(Exception):
@@ -131,26 +132,28 @@
         cores = [x["core"] for x in self._cores.values()]
         for core in cores:
             if only_matching_vlnv:
                 if not any(
                     [eq_vln(core.name, top_core)]
                     + [
                         eq_vln(virtual_vlnv, top_core)
-                        for virtual_vlnv in core.get_virtuals()
+                        for virtual_vlnv in core.get_virtuals(_flags)
                     ]
                 ):
                     continue
 
             # Build a "pretty" package string in a format expected by
             # PrettyPackageStringParser()
             package_str = "{} {}-{}".format(
-                self._package_name(core.name), core.name.version, core.name.revision
+                self._package_name(core.name),
+                core.name.version,
+                core.name.revision,
             )
 
-            _virtuals = core.get_virtuals()
+            _virtuals = core.get_virtuals(_flags)
             if _virtuals:
                 _s = "; provides ( {} )"
                 package_str += _s.format(self._parse_virtual(_virtuals))
 
             # Add dependencies only if we want to build the whole dependency
             # tree.
             if not only_matching_vlnv:
@@ -200,19 +203,23 @@
         # Cache the solution for further lookups
         self._solver_cache_store(solver_cache_key, result)
 
         return result
 
 
 class CoreManager:
-    def __init__(self, config, resolve_env_vars=False):
+    def __init__(
+        self, config, resolve_env_vars=False, allow_additional_properties=False
+    ):
         self.config = config
         self.db = CoreDB()
         self._lm = LibraryManager(config.library_root)
         self.resolve_env_vars = resolve_env_vars
+        self.allow_additional_properties = allow_additional_properties
+        self.core2parser = Core2Parser(resolve_env_vars, allow_additional_properties)
 
     def find_cores(self, library, ignored_dirs):
         found_cores = []
         path = os.path.expanduser(library.location)
         exclude = {".git"}
         if os.path.isdir(path) == False:
             raise OSError(path + " is not a directory")
@@ -258,17 +265,17 @@
                             )
                             continue
                         elif capi_version == -1:
                             # Skip core files which are not FuseSoc format at all.
                             continue
 
                         core = Core(
+                            parser=self.core2parser,
                             core_file=core_file,
                             cache_root=self.config.cache_root,
-                            resolve_env_vars=self.resolve_env_vars,
                         )
                         found_cores.append(core)
                     except SyntaxError as e:
                         w = "Parse error. Ignoring file " + core_file + ": " + e.msg
                         logger.warning(w)
                     except ImportError as e:
                         w = 'Failed to register "{}" due to unknown provider: {}'
```

### Comparing `fusesoc-2.1/fusesoc/edalizer.py` & `fusesoc-2.2/fusesoc/edalizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging
 import os
 import pathlib
 import shutil
 from filecmp import cmp
 
 from fusesoc import utils
+from fusesoc.capi2.coreparser import Core2Parser
 from fusesoc.coremanager import DependencyError
 from fusesoc.utils import merge_dict
 from fusesoc.vlnv import Vlnv
 
 logger = logging.getLogger(__name__)
 
 
@@ -119,57 +120,54 @@
             logger.info("Preparing " + str(core.name))
             core.setup()
 
     def extract_generators(self):
         """Get all registered generators from the cores"""
         generators = {}
         for core in self.cores:
+            _flags = self._core_flags(core)
             logger.debug("Searching for generators in " + str(core.name))
-            if hasattr(core, "get_generators"):
-                core_generators = core.get_generators()
-                if core_generators:
-                    logger.debug(f"Found generators: {core_generators.keys()}")
-                generators.update(core_generators)
+            core_generators = core.get_generators(_flags)
+            logger.debug(f"Found generators: {core_generators.keys()}")
+            generators.update(core_generators)
 
         self.generators = generators
 
     def run_generators(self):
         """Run all generators"""
         self._resolved_or_generated_cores = []
         self._generated_core_dirs_to_remove = []
         for core in self.cores:
             logger.debug("Running generators in " + str(core.name))
             core_flags = self._core_flags(core)
             self._resolved_or_generated_cores.append(core)
-            if hasattr(core, "get_ttptttg"):
-                for ttptttg_data in core.get_ttptttg(core_flags):
-                    _ttptttg = Ttptttg(
-                        ttptttg_data,
-                        core,
-                        self.generators,
-                        resolve_env_vars=self.resolve_env_vars,
-                    )
-                    for gen_core in _ttptttg.generate():
-                        gen_core.pos = _ttptttg.pos
-                        self._resolved_or_generated_cores.append(gen_core)
-                        if not (
-                            _ttptttg.is_generator_cacheable()
-                            or _ttptttg.is_input_cacheable()
-                        ):
-                            self._generated_core_dirs_to_remove.append(
-                                gen_core.core_root
-                            )
+            for ttptttg_data in core.get_ttptttg(core_flags):
+                _ttptttg = Ttptttg(
+                    ttptttg_data,
+                    core,
+                    self.generators,
+                    self.work_root if not self.export_root else None,
+                    resolve_env_vars=self.resolve_env_vars,
+                )
+                for gen_core in _ttptttg.generate():
+                    gen_core.pos = _ttptttg.pos
+                    self._resolved_or_generated_cores.append(gen_core)
+                    if self.export_root and not (
+                        _ttptttg.is_generator_cacheable()
+                        or _ttptttg.is_input_cacheable()
+                    ):
+                        self._generated_core_dirs_to_remove.append(gen_core.core_root)
 
     def export(self):
         for core in self.cores:
             _flags = self._core_flags(core)
 
             # Export core files
             if self.export_root:
-                files_root = os.path.join(self.export_root, core.sanitized_name)
+                files_root = os.path.join(self.export_root, core.name.sanitized_name)
                 core.export(files_root, _flags)
             else:
                 files_root = core.files_root
 
             # Add copyto files
             for file in core.get_files(_flags):
                 if file.get("copyto"):
@@ -205,15 +203,15 @@
             _flags = self._core_flags(core)
 
             # Extract direct dependencies
             snippet["dependencies"] = {str(core.name): core.direct_deps}
 
             # Extract files
             if self.export_root:
-                files_root = os.path.join(self.export_root, core.sanitized_name)
+                files_root = os.path.join(self.export_root, core.name.sanitized_name)
             else:
                 files_root = core.files_root
 
             rel_root = os.path.relpath(files_root, self.work_root)
 
             # Extract parameters
             snippet["parameters"] = core.get_parameters(_flags, parameters)
@@ -229,33 +227,31 @@
             snippet["flow_options"] = core.get_flow_options(_flags)
 
             # Extract scripts
             snippet["hooks"] = core.get_scripts(rel_root, _flags)
 
             _files = []
             for file in core.get_files(_flags):
-                # Copy original file object to be put into EDAM
-                _f = file.copy()
-
-                # copyto tag shouldn't be in EDAM
-                _f.pop("copyto", None)
 
                 # Reparent file path
-                _f["name"] = str(
+                file["name"] = str(
                     file.get("copyto", os.path.join(rel_root, file["name"]))
                 )
 
                 # Set owning core
-                _f["core"] = str(core.name)
+                file["core"] = str(core.name)
+
+                # copyto tag shouldn't be in EDAM
+                file.pop("copyto", None)
 
                 # Reparent include paths
                 if file.get("include_path"):
-                    _f["include_path"] = os.path.join(rel_root, file["include_path"])
+                    file["include_path"] = os.path.join(rel_root, file["include_path"])
 
-                _files.append(_f)
+                _files.append(file)
 
             snippet["files"] = _files
 
             # Extract VPI modules
             snippet["vpi"] = []
             for _vpi in core.get_vpi(_flags):
                 snippet["vpi"].append(
@@ -283,15 +279,15 @@
 
         top_core = self.resolved_cores[-1]
         self.edam = {
             "version": "0.2.1",
             "dependencies": {},
             "files": [],
             "hooks": {},
-            "name": self.system_name or top_core.sanitized_name,
+            "name": self.system_name or top_core.name.sanitized_name,
             "parameters": {},
             "tool_options": {},
             "toplevel": top_core.get_toplevel(self.flags),
             "vpi": [],
         }
 
         for snippet in first_snippets + snippets + last_snippets:
@@ -500,34 +496,36 @@
                 continue
             _value = value[0] if type(value) == list else value
             args_dict[key] = _value
 
         self.add_parsed_args(backend_class, args_dict)
 
     def to_yaml(self, edam_file):
+        pathlib.Path(edam_file).parent.mkdir(parents=True, exist_ok=True)
         return utils.yaml_fwrite(edam_file, self.edam)
 
 
 from fusesoc.core import Core
 from fusesoc.utils import Launcher
 
 
 class Ttptttg:
-    def __init__(self, ttptttg, core, generators, resolve_env_vars=False):
+    def __init__(self, ttptttg, core, generators, gen_root, resolve_env_vars=False):
         generator_name = ttptttg["generator"]
         if not generator_name in generators:
             raise RuntimeError(
                 "Could not find generator '{}' requested by {}".format(
                     generator_name, core.name
                 )
             )
         self.core = core
         self.generator = generators[generator_name]
         self.name = ttptttg["name"]
         self.pos = ttptttg["pos"]
+        self.gen_root = gen_root
         self.resolve_env_vars = resolve_env_vars
         parameters = ttptttg["config"]
 
         vlnv_str = ":".join(
             [
                 core.name.vendor,
                 core.name.library,
@@ -548,17 +546,18 @@
         return hashlib.sha256(
             utils.yaml_dump(self.generator_input).encode()
         ).hexdigest()
 
     def _sha256_file_input_hexdigest(self):
         input_files = []
         logger.debug(
-            "Configured file_input_parameters: " + self.generator.file_input_parameters
+            "Configured file_input_parameters: "
+            + self.generator["file_input_parameters"]
         )
-        for param in self.generator.file_input_parameters.split():
+        for param in self.generator["file_input_parameters"].split():
             try:
                 input_files.append(self.generator_input["parameters"][param])
             except KeyError:
                 logger.debug(
                     f"Parameter {param} does not exist in parameters. File input will not be included in file input hash calculation."
                 )
 
@@ -591,42 +590,49 @@
 
         generator_input_file = os.path.join(generator_cwd, self.name + "_input.yml")
 
         pathlib.Path(generator_cwd).mkdir(parents=True, exist_ok=True)
         utils.yaml_fwrite(generator_input_file, self.generator_input)
 
         args = [
-            os.path.join(os.path.abspath(self.generator.root), self.generator.command),
+            os.path.join(
+                os.path.abspath(self.generator["root"]), self.generator["command"]
+            ),
             os.path.abspath(generator_input_file),
         ]
 
-        if self.generator.interpreter:
-            args[0:0] = [self.generator.interpreter]
+        if "interpreter" in self.generator:
+            args[0:0] = [self.generator["interpreter"]]
 
         Launcher(args[0], args[1:], cwd=generator_cwd).run()
 
     def is_input_cacheable(self):
-        return self.generator.cache_type and self.generator.cache_type == "input"
+        return (
+            "cache_type" in self.generator and self.generator["cache_type"] == "input"
+        )
 
     def is_generator_cacheable(self):
-        return self.generator.cache_type and self.generator.cache_type == "generator"
+        return (
+            "cache_type" in self.generator
+            and self.generator["cache_type"] == "generator"
+        )
 
     def generate(self):
         """Run a parametrized generator
 
         Returns:
             list: Cores created by the generator
         """
 
         hexdigest = self._sha256_input_yaml_hexdigest()
 
         logger.debug("Generator input yaml hash: " + hexdigest)
 
         generator_cwd = os.path.join(
-            self.core.cache_root,
+            self.gen_root or self.core.cache_root,
             "generator_cache",
             self.vlnv.sanitized_name + "-" + hexdigest,
         )
 
         if os.path.lexists(generator_cwd) and not os.path.isdir(generator_cwd):
             raise RuntimeError(
                 "Unable to create generator working directory since it already exists and is not a directory: "
@@ -638,15 +644,15 @@
         if self.is_input_cacheable():
             # Input cache enabled. Check if cached output already exists in generator_cwd.
             logger.debug("Input cache enabled.")
 
             # If file_input_parameters has been configured in the generator
             # parameters will be iterated to look for files to add to the
             # input files hash calculation.
-            if self.generator.file_input_parameters:
+            if "file_input_parameters" in self.generator:
                 file_input_hash = self._sha256_file_input_hexdigest()
 
                 logger.debug("Generator file input hash: " + file_input_hash)
 
                 hashfile = os.path.join(generator_cwd, ".fusesoc_file_input_hash")
 
                 rerun = False
@@ -687,23 +693,24 @@
             # caching is changed to no caching.
             logger.debug("Generator cache is not enabled.")
             shutil.rmtree(generator_cwd, ignore_errors=True)
             self._run(generator_cwd)
 
         cores = []
         logger.debug("Looking for generated or cached cores in " + generator_cwd)
+        parser = Core2Parser(self.resolve_env_vars, allow_additional_properties=False)
         for root, dirs, files in os.walk(generator_cwd):
             for f in files:
                 if f.endswith(".core"):
                     try:
                         cores.append(
                             Core(
+                                parser,
                                 os.path.join(root, f),
                                 generated=True,
-                                resolve_env_vars=self.resolve_env_vars,
                             )
                         )
                     except SyntaxError as e:
                         w = "Failed to parse generated core file " + f + ": " + e.msg
                         raise RuntimeError(w)
         logger.debug("Found " + ", ".join(str(c.name) for c in cores))
         return cores
```

### Comparing `fusesoc-2.1/fusesoc/librarymanager.py` & `fusesoc-2.2/fusesoc/librarymanager.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/fusesoc/main.py` & `fusesoc-2.2/fusesoc/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     for name in sorted(cores.keys()):
         core = cores[name]
         print(
             name.ljust(maxlen)
             + " : "
             + core.cache_status().rjust(10)
             + " : "
-            + (core.description or "<No description>")
+            + (core.get_description() or "<No description>")
         )
 
 
 def list_tools(cm, args):
     from edalize.edatool import walk_tool_packages
 
     _tp = list(walk_tool_packages())
@@ -219,15 +219,15 @@
         print("=" * (maxlen + 12))
         for core in sorted(cores.keys()):
             for generator_name, generator_data in cores[core].items():
                 print(
                     "{} : {} : {}".format(
                         core.ljust(maxlen),
                         generator_name,
-                        generator_data.description or "<No description>",
+                        generator_data["description"] or "<No description>",
                     )
                 )
 
 
 def gen_show(cm, args):
     cores = cm.get_generators()
     for core in sorted(cores.keys()):
@@ -239,16 +239,16 @@
 Generator   : {}
 Description : {}
 Usage       :
 
 {}""".format(
                         core,
                         generator_name,
-                        generator_data.description or "<No description>",
-                        generator_data.usage or "",
+                        generator_data["description"] or "<No description>",
+                        generator_data["usage"] or "",
                     )
                 )
 
 
 def core_info(cm, args):
     core = _get_core(cm, args.core)
     print(core.info())
@@ -402,14 +402,19 @@
         core_manager=cm,
         work_root=work_root,
         export_root=export_root,
         system_name=system_name,
         resolve_env_vars=resolve_env_vars,
     )
 
+    # Unconditionally clean out the work root on fresh builds
+    # if we use the old tool API
+    if do_configure and not flow:
+        prepare_work_root(work_root)
+
     try:
         edam = edalizer.run()
         edalizer.parse_args(backend_class, backendargs, edam)
         edalizer.export()
     except SyntaxError as e:
         logger.error(e.msg)
         exit(1)
@@ -481,17 +486,26 @@
 
     if monochrome:
         logger.debug("Monochrome output")
     else:
         logger.debug("Colorful output")
 
 
-def init_coremanager(config, args_cores_root, args_resolve_env_vars=False):
+def init_coremanager(
+    config,
+    args_cores_root,
+    args_resolve_env_vars=False,
+    args_allow_additional_properties=False,
+):
     logger.debug("Initializing core manager")
-    cm = CoreManager(config, resolve_env_vars=args_resolve_env_vars)
+    cm = CoreManager(
+        config,
+        resolve_env_vars=args_resolve_env_vars,
+        allow_additional_properties=args_allow_additional_properties,
+    )
 
     args_libs = [Library(acr, acr) for acr in args_cores_root]
     # Add libraries from config file, env var and command-line
     for library in config.libraries + args_libs:
         try:
             cm.add_library(library, config.ignored_dirs)
         except (RuntimeError, OSError) as e:
@@ -691,14 +705,19 @@
         "--resolve-env-vars-early",
         action="store_true",
         help="Resolve environment variables in FuseSoC (defaults to no resolution)",
     )
     parser_run.add_argument(
         "--system-name", help="Override default VLNV name for system"
     )
+    parser_run.add_argument(
+        "--allow-additional-properties",
+        action="store_true",
+        help="Allow additional properties in core files",
+    )
     parser_run.add_argument("system", help="Select a system to operate on")
     parser_run.add_argument(
         "backendargs", nargs=argparse.REMAINDER, help="arguments to be sent to backend"
     )
     parser_run.set_defaults(func=run)
 
     return parser
@@ -722,18 +741,20 @@
     init_logging(args.verbose, args.monochrome, args.log_file)
     config = Config(args.config)
 
     resolve_env_vars_early = False
     if hasattr(args, "resolve_env_vars_early"):
         resolve_env_vars_early = args.resolve_env_vars_early
 
+    allow_additional_properties = False
+    if hasattr(args, "allow_additional_properties"):
+        allow_additional_properties = args.allow_additional_properties
+
     cm = init_coremanager(
-        config,
-        args.cores_root,
-        resolve_env_vars_early,
+        config, args.cores_root, resolve_env_vars_early, allow_additional_properties
     )
     # Run the function
     args.func(cm, args)
 
 
 def main():
     args = parse_args(sys.argv[1:])
```

### Comparing `fusesoc-2.1/fusesoc/provider/git.py` & `fusesoc-2.2/fusesoc/provider/git.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/fusesoc/provider/github.py` & `fusesoc-2.2/fusesoc/provider/github.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/fusesoc/provider/local.py` & `fusesoc-2.2/fusesoc/provider/local.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/fusesoc/provider/opencores.py` & `fusesoc-2.2/fusesoc/provider/opencores.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/fusesoc/provider/provider.py` & `fusesoc-2.2/fusesoc/provider/provider.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/fusesoc/provider/url.py` & `fusesoc-2.2/fusesoc/provider/url.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/fusesoc/utils.py` & `fusesoc-2.2/fusesoc/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     return path.decode("ascii").strip()
 
 
 import os
 
 
 def unique_dirs(file_list):
-    return list({os.path.dirname(f.name) for f in file_list})
+    return list({os.path.dirname(f) for f in file_list})
 
 
 # With help from:
 # http://stackoverflow.com/questions/384076/how-can-i-color-python-logging-output
 # Very minimal direct copying so should be no license issues.
 
 BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE = range(8)
@@ -146,20 +146,23 @@
         package_logger.addHandler(ch)
         package_logger.setLevel(logging.WARNING)
     logger.debug(f"Setup logging at level {level}.")
 
 
 def yaml_fwrite(filepath, content, preamble=""):
     with open(filepath, "w") as f:
-        f.write(preamble)
-        f.write(yaml.dump(content, Dumper=YamlDumper))
+        if len(preamble) > 0:
+            f.write(preamble + "\n")
+        f.write(yaml.dump(content, Dumper=YamlDumper, sort_keys=False))
 
 
-def yaml_fread(filepath, resolve_env_vars=False):
+def yaml_fread(filepath, resolve_env_vars=False, remove_preamble=False):
     with open(filepath) as f:
+        if remove_preamble:
+            f.readline()
         if resolve_env_vars:
             return yaml.load(os.path.expandvars(f.read()), Loader=YamlLoader)
         else:
             return yaml.load(f.read(), Loader=YamlLoader)
 
 
 def yaml_read(data, resolve_env_vars=False):
```

### Comparing `fusesoc-2.1/fusesoc/vlnv.py` & `fusesoc-2.2/fusesoc/vlnv.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/fusesoc.egg-info/PKG-INFO` & `fusesoc-2.2/fusesoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusesoc
-Version: 2.1
+Version: 2.2
 Summary: FuseSoC is a package manager and a set of build tools for HDL (Hardware Description Language) code.
 Home-page: https://github.com/olofk/fusesoc
 Author: Olof Kindgren
 Author-email: olof.kindgren@gmail.com
 License: BSD-2-Clause
 Keywords: VHDL,verilog,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fusesoc-2.1/fusesoc.egg-info/SOURCES.txt` & `fusesoc-2.2/fusesoc.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,21 @@
 fusesoc.egg-info/SOURCES.txt
 fusesoc.egg-info/dependency_links.txt
 fusesoc.egg-info/entry_points.txt
 fusesoc.egg-info/requires.txt
 fusesoc.egg-info/top_level.txt
 fusesoc/capi2/__init__.py
 fusesoc/capi2/core.py
+fusesoc/capi2/coredata.py
+fusesoc/capi2/coreparser.py
 fusesoc/capi2/exprs.py
 fusesoc/capi2/generator.py
+fusesoc/capi2/json_schema.py
+fusesoc/parser/__init__.py
+fusesoc/parser/coreparser.py
 fusesoc/provider/__init__.py
 fusesoc/provider/git.py
 fusesoc/provider/github.py
 fusesoc/provider/local.py
 fusesoc/provider/opencores.py
 fusesoc/provider/provider.py
 fusesoc/provider/url.py
@@ -111,14 +116,16 @@
 tests/capi2_cores/misc/vpi.core
 tests/capi2_cores/misc/vpifile
 tests/capi2_cores/misc/generate/file_cachetest
 tests/capi2_cores/misc/generate/generate.core
 tests/capi2_cores/misc/generate/generators.core
 tests/capi2_cores/misc/generate/testgen.py
 tests/capi2_cores/misc/subdir/dummy.extra
+tests/capi2_cores/parser/no_additional_properties.core
+tests/capi2_cores/parser/with_additional_properties.core
 tests/capi2_cores/providers/url_simple.core
 tests/capi2_cores/providers/url_simple_with_user_agent.core
 tests/capi2_cores/providers/url_tar.core
 tests/capi2_cores/providers/url_zip.core
 tests/capi2_cores/virtual/impl1.core
 tests/capi2_cores/virtual/impl2.core
 tests/capi2_cores/virtual/user.core
```

### Comparing `fusesoc-2.1/setup.py` & `fusesoc-2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="fusesoc",
-    packages=["fusesoc", "fusesoc.capi2", "fusesoc.provider"],
+    packages=["fusesoc", "fusesoc.capi2", "fusesoc.provider", "fusesoc.parser"],
     use_scm_version={
         "relative_to": __file__,
         "write_to": "fusesoc/version.py",
     },
     author="Olof Kindgren",
     author_email="olof.kindgren@gmail.com",
     description=(
@@ -51,11 +51,12 @@
         "setuptools_scm; python_version>='3.7'",
     ],
     install_requires=[
         "edalize>=0.4.1",
         "pyparsing",
         "pyyaml",
         "simplesat>=0.8.0",
+        "fastjsonschema",
     ],
     # Supported Python versions: 3.6+
     python_requires=">=3.6, <4",
 )
```

### Comparing `fusesoc-2.1/tests/capi2_cores/deptree/generated_child_a.core` & `fusesoc-2.2/tests/capi2_cores/deptree/generated_child_a.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/capi2_cores/deptree/root.core` & `fusesoc-2.2/tests/capi2_cores/deptree/root.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/capi2_cores/files_out_of_hierarchy/subdir/files_out_of_hierarchy.core` & `fusesoc-2.2/tests/capi2_cores/files_out_of_hierarchy/subdir/files_out_of_hierarchy.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/capi2_cores/misc/depends.core` & `fusesoc-2.2/tests/capi2_cores/misc/depends.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/capi2_cores/misc/files.core` & `fusesoc-2.2/tests/capi2_cores/misc/files.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/capi2_cores/misc/generate/generate.core` & `fusesoc-2.2/tests/capi2_cores/misc/generate/generate.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/capi2_cores/misc/generate/testgen.py` & `fusesoc-2.2/tests/capi2_cores/misc/generate/testgen.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/capi2_cores/misc/hooks.core` & `fusesoc-2.2/tests/capi2_cores/misc/hooks.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/capi2_cores/misc/parameters.core` & `fusesoc-2.2/tests/capi2_cores/misc/parameters.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/capi2_cores/misc/typecheck.core` & `fusesoc-2.2/tests/capi2_cores/misc/typecheck.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/capi2_cores/misc/vpi.core` & `fusesoc-2.2/tests/capi2_cores/misc/vpi.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/adv_debug_sys/adv_debug_sys.core` & `fusesoc-2.2/tests/cores/adv_debug_sys/adv_debug_sys.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/atlys/atlys.core` & `fusesoc-2.2/tests/cores/atlys/atlys.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/elf-loader/elf-loader.core` & `fusesoc-2.2/tests/cores/elf-loader/elf-loader.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/libstorage/libstorage-1.0.core` & `fusesoc-2.2/tests/cores/libstorage/libstorage-1.0.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/misc/c3demo.core` & `fusesoc-2.2/tests/cores/misc/c3demo.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/misc/filetypes.core` & `fusesoc-2.2/tests/cores/misc/filetypes.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/misc/ghdltest.core` & `fusesoc-2.2/tests/cores/misc/ghdltest.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/misc/no_exe_script.core` & `fusesoc-2.2/tests/cores/misc/no_exe_script.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/misc/paramtest.core` & `fusesoc-2.2/tests/cores/misc/paramtest.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/misc/scriptscore.core` & `fusesoc-2.2/tests/cores/misc/scriptscore.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/mor1kx/mor1kx-3.1.core` & `fusesoc-2.2/tests/cores/mor1kx/mor1kx-3.1.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/mor1kx-arty/mor1kx-arty.core` & `fusesoc-2.2/tests/cores/mor1kx-arty/mor1kx-arty.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/mor1kx-generic/mor1kx-generic.core` & `fusesoc-2.2/tests/cores/mor1kx-generic/mor1kx-generic.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/sockit/sockit.core` & `fusesoc-2.2/tests/cores/sockit/sockit.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/uart16550/uart16550-1.5.core` & `fusesoc-2.2/tests/cores/uart16550/uart16550-1.5.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/verilator_tb_utils/verilator_tb_utils.core` & `fusesoc-2.2/tests/cores/verilator_tb_utils/verilator_tb_utils.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/verilog-arbiter/verilog-arbiter-r1.core` & `fusesoc-2.2/tests/cores/verilog-arbiter/verilog-arbiter-r1.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/verilog_utils/verilog_utils.core` & `fusesoc-2.2/tests/cores/verilog_utils/verilog_utils.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/vga_lcd/vga_lcd.core` & `fusesoc-2.2/tests/cores/vga_lcd/vga_lcd.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/vlog_tb_utils/files/0001-testpatch.patch` & `fusesoc-2.2/tests/cores/vlog_tb_utils/files/0001-testpatch.patch`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/vlog_tb_utils/vlog_tb_utils-1.1.core` & `fusesoc-2.2/tests/cores/vlog_tb_utils/vlog_tb_utils-1.1.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/wb_common/wb_common.core` & `fusesoc-2.2/tests/cores/wb_common/wb_common.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/cores/wb_intercon/wb_intercon-1.0.core` & `fusesoc-2.2/tests/cores/wb_intercon/wb_intercon-1.0.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/test_capi2.py` & `fusesoc-2.2/tests/test_capi2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,63 +11,67 @@
 cores_dir = os.path.join(tests_dir, "capi2_cores", "misc")
 
 
 def test_files_out_of_hierarchy():
     import os
     import tempfile
 
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     core_file = os.path.join(
         tests_dir,
         "capi2_cores",
         "files_out_of_hierarchy",
         "subdir",
         "files_out_of_hierarchy.core",
     )
-    core = Core(core_file)
+    core = Core(Core2Parser(), core_file)
     export_root = tempfile.mkdtemp(prefix="capi2_files_out_of_hierarchy_")
 
     with pytest.warns(FutureWarning, match="not within the directory"):
         core.export(export_root, {"target": "bad", "is_toplevel": True})
 
     with warnings.catch_warnings(record=True) as record:
         core.export(export_root, {"target": "good", "is_toplevel": True})
         assert not record
 
 
 def test_empty_core():
     import os
     import tempfile
 
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     core_file = os.path.join(tests_dir, "capi2_cores", "misc", "empty.core")
     with pytest.raises(SyntaxError) as excinfo:
-        core = Core(core_file)
-    assert "Error while trying to parse the core file" in str(excinfo.value)
+        core = Core(Core2Parser(), core_file)
+    assert "Error validating" in str(excinfo.value)
 
 
 def test_virtual():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
     from fusesoc.vlnv import Vlnv
 
     core_file = os.path.join(tests_dir, "capi2_cores", "virtual", "impl1.core")
-    core = Core(core_file)
+    core = Core(Core2Parser(), core_file)
     assert core.get_virtuals() == [Vlnv("::someinterface:0")]
 
 
 def test_capi2_export():
     import os
     import tempfile
 
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     core_file = os.path.join(tests_dir, "capi2_cores", "misc", "files.core")
-    core = Core(core_file)
+    core = Core(Core2Parser(), core_file)
 
     export_root = tempfile.mkdtemp(prefix="capi2_export_")
 
     core.export(export_root)
 
     expected = [
         "dontpickthisfile",
@@ -101,18 +105,19 @@
 
 
 def test_capi2_export_no_overwrite():
     import os
     import tempfile
     from filecmp import cmp
 
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     core_file = os.path.join(tests_dir, "capi2_cores", "misc", "files.core")
-    core = Core(core_file)
+    core = Core(Core2Parser(), core_file)
 
     export_root = tempfile.mkdtemp(prefix="capi2_export_")
 
     expected = [
         "dontpickthisfile",
         "dummy.tcl",
         "scriptfile",
@@ -141,17 +146,18 @@
     # Re-export and check for equality
     core.export(export_root)
     for f in expected:
         assert cmp(os.path.join(core.files_root, f), os.path.join(export_root, f))
 
 
 def test_capi2_append():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
-    core = Core(os.path.join(cores_dir, "append.core"))
+    core = Core(Core2Parser(), os.path.join(cores_dir, "append.core"))
 
     flags = {"is_toplevel": True}
 
     flags["target"] = "no_fs_no_fsappend"
     result = [x["name"] for x in core.get_files(flags)]
     expected = []
     assert expected == result
@@ -169,18 +175,21 @@
     flags["target"] = "fs_fsappend"
     result = [x["name"] for x in core.get_files(flags)]
     expected = ["file1", "file2", "file3", "file4"]
     assert expected == result
 
 
 def test_capi2_get_depends():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
     from fusesoc.vlnv import Vlnv
 
-    core = Core(os.path.join(tests_dir, "capi2_cores", "misc", "depends.core"))
+    core = Core(
+        Core2Parser(), os.path.join(tests_dir, "capi2_cores", "misc", "depends.core")
+    )
     flags = {}
     result = core.get_depends(flags)
 
     expected = [
         Vlnv("unversioned"),
         Vlnv("versioned-1.0"),
         Vlnv("<lt-1.0"),
@@ -202,18 +211,19 @@
     ]
     assert len(result) == len(expected)
     for i in range(len(result)):
         assert result[i] == expected[i]
 
 
 def test_capi2_get_files():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     core_file = os.path.join(tests_dir, "capi2_cores", "misc", "files.core")
-    core = Core(core_file)
+    core = Core(Core2Parser(), core_file)
 
     expected = [
         {
             "file_type": "vhdlSource",
             "logical_name": "overridden_logical_name",
             "name": "vlogfile",
         },
@@ -245,62 +255,66 @@
             "file_type": "user",
             "name": "pickthisfile",
         },
     ]
 
     flags = {"tool": "icarus"}
     result = core.get_files(flags)
+
     assert expected == result
 
 
 def test_capi2_type_check():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     core_file = os.path.join(tests_dir, "capi2_cores", "misc", "typecheck.core")
 
     with pytest.raises(SyntaxError) as excinfo:
-        core = Core(core_file)
-    assert "Object in file_type section must be a String" in str(excinfo.value)
+        core = Core(Core2Parser(), core_file)
+    assert "Error validating" in str(excinfo.value)
 
 
 def test_capi2_get_flags():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
-    core = Core(os.path.join(cores_dir, "flags.core"))
+    core = Core(Core2Parser(), os.path.join(cores_dir, "flags.core"))
 
     assert {} == core.get_flags("bad_target")
     assert {} == core.get_flags("noflags")
     assert {} == core.get_flags("emptyflags")
     assert {"tool": "mytool"} == core.get_flags("emptyflagstool")
     expected = {"flag1": False, "flag2": True, "flag3": True}
     assert expected == core.get_flags("allflags")
     expected["tool"] = "mytool"
     expected.pop("flag3")
     assert expected == core.get_flags("allflagstool")
 
 
 def test_capi2_get_generators():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
-    core = Core(os.path.join(cores_dir, "generate", "generators.core"))
+    core = Core(Core2Parser(), os.path.join(cores_dir, "generate", "generators.core"))
 
     generators = core.get_generators()
     assert len(generators) == 2
-    assert generators["generator1"].command == "testgen.py"
-    assert generators["generator2"].command == "testgen.py"
-    assert generators["generator2"].cache_type == "input"
-    assert generators["generator2"].file_input_parameters == "file_in_param1"
+    assert generators["generator1"]["command"] == "testgen.py"
+    assert generators["generator2"]["command"] == "testgen.py"
+    assert generators["generator2"]["cache_type"] == "input"
+    assert generators["generator2"]["file_input_parameters"] == "file_in_param1"
 
 
 def test_capi2_get_parameters():
-    from fusesoc.capi2.core import Generators
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     core_file = os.path.join(tests_dir, "capi2_cores", "misc", "parameters.core")
-    core = Core(core_file)
+    core = Core(Core2Parser(), core_file)
 
     param1 = {
         "datatype": "str",
         "paramtype": "vlogparam",
     }
     param2 = {
         "datatype": "str",
@@ -414,14 +428,15 @@
         "booltrue": booltrue,
         "realpi": realpi,
     }
     assert expected == core.get_parameters(flags)
 
 
 def test_capi2_get_scripts():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     simple1 = {
         "cmd": ["simple_cmd1"],
         "env": {"FILES_ROOT": "my_files_root"},
         "name": "simple1",
     }
@@ -447,15 +462,15 @@
     }
     multi_cmd = {
         "cmd": ["command", "with", "args"],
         "env": {"FILES_ROOT": "my_files_root"},
         "name": "multi_cmd",
     }
     core_file = os.path.join(tests_dir, "capi2_cores", "misc", "hooks.core")
-    core = Core(core_file)
+    core = Core(Core2Parser(), core_file)
 
     flags = {"is_toplevel": True}
     expected = {"pre_build": [simple1]}
     assert expected == core.get_scripts("my_files_root", flags)
 
     flags["target"] = "nohooks"
     expected = {}
@@ -488,18 +503,19 @@
 
     flags["tool"] = "icarus"
     expected = {"post_run": [simple1]}
     assert expected == core.get_scripts("my_files_root", flags)
 
 
 def test_capi2_get_tool_options():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     core_file = os.path.join(tests_dir, "capi2_cores", "misc", "targets.core")
-    core = Core(core_file)
+    core = Core(Core2Parser(), core_file)
 
     with pytest.raises(KeyError):
         core.get_tool_options({})
 
     assert {} == core.get_tool_options({"tool": "icarus"})
     flags = {"target": "target_with_tool_options", "is_toplevel": True}
 
@@ -513,34 +529,36 @@
 
     flags["tool"] = "invalid"
     expected = {}
     assert expected == core.get_tool_options(flags)
 
 
 def test_capi2_get_toplevel():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     core_file = os.path.join(tests_dir, "capi2_cores", "misc", "toplevel.core")
-    core = Core(core_file)
+    core = Core(Core2Parser(), core_file)
 
     flags = {"target": "no_toplevel"}
     with pytest.raises(SyntaxError):
         core.get_toplevel(flags)
 
     flags = {"target": "str_toplevel"}
     assert "toplevel_as_string" == core.get_toplevel(flags)
 
     flags = {"target": "list_toplevel"}
     assert "toplevel as list" == core.get_toplevel(flags)
 
 
 def test_capi2_get_ttptttg():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
-    core = Core(os.path.join(cores_dir, "generate", "generate.core"))
+    core = Core(Core2Parser(), os.path.join(cores_dir, "generate", "generate.core"))
 
     flags = {"is_toplevel": True}
     expected = [
         {
             "name": "testgenerate_without_params",
             "generator": "generator1",
             "pos": "append",
@@ -579,18 +597,19 @@
     )
 
     flags["target"] = "invalid_target"
     assert [] == core.get_ttptttg(flags)
 
 
 def test_capi2_get_vpi():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     core_file = os.path.join(tests_dir, "capi2_cores", "misc", "vpi.core")
-    core = Core(core_file)
+    core = Core(Core2Parser(), core_file)
 
     expected = [
         {
             "src_files": ["f1", "f3"],
             "include_dirs": [""],
             "libs": ["some_lib"],
             "name": "vpi1",
@@ -600,22 +619,103 @@
 
     assert [] == core.get_vpi({"is_toplevel": True, "target": "invalid"})
     assert expected == core.get_vpi({"is_toplevel": True})
     assert expected == core.get_vpi({"is_toplevel": False})
 
 
 def test_capi2_info():
+    from fusesoc.capi2.coreparser import Core2Parser
     from fusesoc.core import Core
 
     dirs_and_corenames = [("", "targets"), ("generate", "generators")]
 
     for subdir, core_name in dirs_and_corenames:
         core_file = os.path.join(
             tests_dir, "capi2_cores", "misc", subdir, core_name + ".core"
         )
-        core = Core(core_file)
+        core = Core(Core2Parser(), core_file)
 
         gen_info = "\n".join(
             [x for x in core.info().split("\n") if not "Core root" in x]
         )
         with open(os.path.join(tests_dir, __name__, core_name + ".info")) as f:
             assert f.read() == gen_info, core_name
+
+
+def test_core2parser():
+    import os
+    import tempfile
+
+    from fusesoc.capi2.coreparser import Core2Parser
+
+    core_file = os.path.join(
+        tests_dir, "capi2_cores", "parser", "no_additional_properties.core"
+    )
+
+    parser = Core2Parser(allow_additional_properties=False)
+    assert parser.get_version() == 2
+    assert parser.get_allow_additional_properties() == False
+    assert parser.get_preamble() == "CAPI=2:"
+
+    expected = {
+        "name": "::noadditionalproperties:0",
+        "filesets": {
+            "somename": {
+                "files": ["somefile1", {"someincludefile1": {"is_include_file": True}}]
+            }
+        },
+        "targets": {"default": {"filesets": ["somename"]}},
+    }
+
+    capi2_data = parser.read(core_file)
+    assert expected == capi2_data
+
+    tmpfile = tempfile.mktemp(prefix="capi2_parser_")
+    parser.write(tmpfile, capi2_data)
+    capi2_readback_data = parser.read(tmpfile)
+    os.remove(tmpfile)
+    assert capi2_data == capi2_readback_data
+
+    capi2_data["mycustomprop1"] = {
+        "one": "mystring",
+        "two": ["list_item_1", "list_item_2"],
+    }
+
+    with pytest.raises(SyntaxError) as excinfo:
+        parser.write(tmpfile, capi2_data)
+    assert "Error validating" in str(excinfo.value)
+
+    core_file = os.path.join(
+        tests_dir, "capi2_cores", "parser", "with_additional_properties.core"
+    )
+
+    with pytest.raises(SyntaxError) as excinfo:
+        parser.read(core_file)
+    assert "Error validating" in str(excinfo.value)
+
+    parser = Core2Parser(allow_additional_properties=True)
+    assert parser.get_allow_additional_properties() == True
+
+    expected = {
+        "name": "::withadditionalproperties:0",
+        "filesets": {
+            "somename": {
+                "files": ["somefile1", {"someincludefile1": {"is_include_file": True}}],
+                "mycustomprop1": "this is a custom property",
+                "mycustomprop2": 1,
+            }
+        },
+        "targets": {"default": {"filesets": ["somename"]}},
+        "mycustomprop3": {
+            "subitem1": "mystring",
+            "subitem2": ["list_item_1", "list_item_2"],
+        },
+    }
+
+    capi2_data = parser.read(core_file)
+    assert expected == capi2_data
+
+    capi2_data["mycustomprop4"] = "new string"
+    parser.write(tmpfile, capi2_data)
+    capi2_readback_data = parser.read(tmpfile)
+    os.remove(tmpfile)
+    assert capi2_data == capi2_readback_data
```

### Comparing `fusesoc-2.1/tests/test_config.py` & `fusesoc-2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/test_coremanager.py` & `fusesoc-2.2/tests/test_coremanager.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/test_edalizer.py` & `fusesoc-2.2/tests/test_edalizer.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/test_exprs.py` & `fusesoc-2.2/tests/test_exprs.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/test_ignored_dirs.py` & `fusesoc-2.2/tests/test_ignored_dirs.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/test_libraries.py` & `fusesoc-2.2/tests/test_libraries.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/test_provider/vlog_functions.v` & `fusesoc-2.2/tests/test_provider/vlog_functions.v`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/test_provider.py` & `fusesoc-2.2/tests/test_provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 import os
 import shutil
 import tempfile
 
 import pytest
 from test_common import tests_dir
 
+from fusesoc.capi2.coreparser import Core2Parser
 from fusesoc.core import Core
 
 cores_root = os.path.join(tests_dir, "cores")
 
 
 def test_git_provider():
     cache_root = tempfile.mkdtemp("git_")
-    core = Core(os.path.join(cores_root, "misc", "gitcore.core"), cache_root)
+    core = Core(
+        Core2Parser(), os.path.join(cores_root, "misc", "gitcore.core"), cache_root
+    )
 
     core.setup()
 
     for f in [
         "LICENSE",
         "README.md",
         "wb_common.core",
@@ -29,15 +32,17 @@
     ]:
         assert os.path.isfile(os.path.join(core.files_root, f))
 
 
 def test_github_provider():
     cache_root = tempfile.mkdtemp("github_")
     core = Core(
-        os.path.join(cores_root, "vlog_tb_utils", "vlog_tb_utils-1.1.core"), cache_root
+        Core2Parser(),
+        os.path.join(cores_root, "vlog_tb_utils", "vlog_tb_utils-1.1.core"),
+        cache_root,
     )
 
     core.setup()
 
     for f in [
         "LICENSE",
         "vlog_functions.v",
@@ -53,39 +58,49 @@
     ) as fgen:
         assert fref.read() == fgen.read(), f
 
 
 @pytest.mark.skip(reason="Problems connecting to OpenCores SVN")
 def test_opencores_provider():
     cache_root = tempfile.mkdtemp("opencores_")
-    core = Core(os.path.join(cores_root, "misc", "opencorescore.core"), cache_root)
+    core = Core(
+        Core2Parser(),
+        os.path.join(cores_root, "misc", "opencorescore.core"),
+        cache_root,
+    )
 
     core.setup()
 
     assert os.path.isfile(os.path.join(core.files_root, "tap_defines.v"))
     assert os.path.isfile(os.path.join(core.files_root, "tap_top.v"))
 
 
 def test_url_provider():
     cores_root = os.path.join(tests_dir, "capi2_cores", "providers")
 
     for corename in ["url_simple", "url_simple_with_user_agent", "url_tar", "url_zip"]:
         cache_root = tempfile.mkdtemp(prefix="url_")
-        core = Core(os.path.join(cores_root, corename + ".core"), cache_root)
+        core = Core(
+            Core2Parser(), os.path.join(cores_root, corename + ".core"), cache_root
+        )
         core.setup()
         assert os.path.isfile(os.path.join(core.files_root, "file.v"))
 
 
 def test_uncachable():
     cores_root = os.path.join(tests_dir, "capi2_cores", "misc")
     cache_root = tempfile.mkdtemp("uncachable_")
-    core = Core(os.path.join(cores_root, "uncachable.core"), cache_root)
+    core = Core(Core2Parser(), os.path.join(cores_root, "uncachable.core"), cache_root)
     assert core.cache_status() == "outofdate"
 
 
 @pytest.mark.skip(reason="Problems connecting to OpenCores SVN")
 def test_cachable():
     cache_root = tempfile.mkdtemp("opencores_")
-    core = Core(os.path.join(cores_root, "misc", "opencorescore.core"), cache_root)
+    core = Core(
+        Core2Parser(),
+        os.path.join(cores_root, "misc", "opencorescore.core"),
+        cache_root,
+    )
     assert core.cache_status() == "empty"
     core.setup()
     assert core.cache_status() == "downloaded"
```

### Comparing `fusesoc-2.1/tests/test_vlnv.py` & `fusesoc-2.2/tests/test_vlnv.py`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/userguide/blinky/blinky.core` & `fusesoc-2.2/tests/userguide/blinky/blinky.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/userguide/blinky/rtl/blinky.sv` & `fusesoc-2.2/tests/userguide/blinky/rtl/blinky.sv`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/userguide/blinky/tb/blinky_tb.sv` & `fusesoc-2.2/tests/userguide/blinky/tb/blinky_tb.sv`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/userguide/dualblinky/data/nexys_video.xdc` & `fusesoc-2.2/tests/userguide/dualblinky/data/nexys_video.xdc`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/userguide/dualblinky/dualblinky.core` & `fusesoc-2.2/tests/userguide/dualblinky/dualblinky.core`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tests/userguide/dualblinky/rtl/dualblinky.sv` & `fusesoc-2.2/tests/userguide/dualblinky/rtl/dualblinky.sv`

 * *Files identical despite different names*

### Comparing `fusesoc-2.1/tox.ini` & `fusesoc-2.2/tox.ini`

 * *Files identical despite different names*

