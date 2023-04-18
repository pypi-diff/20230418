# Comparing `tmp/ephemeris-0.8.0.tar.gz` & `tmp/ephemeris-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ephemeris-0.8.0.tar", last modified: Fri Dec 29 20:56:20 2017, max compression
+gzip compressed data, was "dist/ephemeris-0.9.0.tar", last modified: Wed May 23 10:37:46 2018, max compression
```

## Comparing `ephemeris-0.8.0.tar` & `ephemeris-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 bag       (1001) bag       (1001)        0 2017-12-29 20:56:20.000000 ephemeris-0.8.0/
-drwxr-xr-x   0 bag       (1001) bag       (1001)        0 2017-12-29 20:56:20.000000 ephemeris-0.8.0/ephemeris/
--rw-r--r--   0 bag       (1001) bag       (1001)     1514 2017-11-07 23:13:56.000000 ephemeris-0.8.0/ephemeris/workflow_install.py
--rw-r--r--   0 bag       (1001) bag       (1001)     1761 2017-12-29 20:56:19.000000 ephemeris-0.8.0/ephemeris/__init__.py
--rw-r--r--   0 bag       (1001) bag       (1001)     4437 2017-11-07 23:13:39.000000 ephemeris-0.8.0/ephemeris/generate_tool_list_from_ga_workflow_files.py
--rw-r--r--   0 bag       (1001) bag       (1001)    10085 2017-12-28 12:19:25.000000 ephemeris-0.8.0/ephemeris/run_data_managers.py
--rw-r--r--   0 bag       (1001) bag       (1001)     1027 2017-11-07 23:13:39.000000 ephemeris-0.8.0/ephemeris/common_parser.py
--rwxr-xr-x   0 bag       (1001) bag       (1001)     2315 2017-11-07 23:13:56.000000 ephemeris-0.8.0/ephemeris/sleep.py
--rw-r--r--   0 bag       (1001) bag       (1001)     1653 2017-12-28 12:19:25.000000 ephemeris-0.8.0/ephemeris/ephemeris_log.py
--rw-r--r--   0 bag       (1001) bag       (1001)     2426 2017-11-07 23:13:39.000000 ephemeris-0.8.0/ephemeris/setup_data_libraries.py
--rw-r--r--   0 bag       (1001) bag       (1001)    35188 2017-12-28 12:19:25.000000 ephemeris-0.8.0/ephemeris/shed_tools.py
--rw-r--r--   0 bag       (1001) bag       (1001)     7514 2017-12-28 12:19:25.000000 ephemeris-0.8.0/ephemeris/get_tool_list_from_galaxy.py
--rw-rw-r--   0 bag       (1001) bag       (1001)      310 2017-12-29 20:56:20.000000 ephemeris-0.8.0/setup.cfg
--rw-r--r--   0 bag       (1001) bag       (1001)     6467 2017-12-29 20:56:20.000000 ephemeris-0.8.0/PKG-INFO
-drwxr-xr-x   0 bag       (1001) bag       (1001)        0 2017-12-29 20:56:20.000000 ephemeris-0.8.0/ephemeris.egg-info/
--rw-r--r--   0 bag       (1001) bag       (1001)     6467 2017-12-29 20:56:19.000000 ephemeris-0.8.0/ephemeris.egg-info/PKG-INFO
--rw-r--r--   0 bag       (1001) bag       (1001)      638 2017-12-29 20:56:19.000000 ephemeris-0.8.0/ephemeris.egg-info/SOURCES.txt
--rw-r--r--   0 bag       (1001) bag       (1001)       10 2017-12-29 20:56:19.000000 ephemeris-0.8.0/ephemeris.egg-info/top_level.txt
--rw-r--r--   0 bag       (1001) bag       (1001)        1 2017-12-29 20:56:19.000000 ephemeris-0.8.0/ephemeris.egg-info/not-zip-safe
--rw-r--r--   0 bag       (1001) bag       (1001)      440 2017-12-29 20:56:19.000000 ephemeris-0.8.0/ephemeris.egg-info/entry_points.txt
--rw-r--r--   0 bag       (1001) bag       (1001)       42 2017-12-29 20:56:19.000000 ephemeris-0.8.0/ephemeris.egg-info/requires.txt
--rw-r--r--   0 bag       (1001) bag       (1001)        1 2017-12-29 20:56:19.000000 ephemeris-0.8.0/ephemeris.egg-info/dependency_links.txt
--rw-rw-r--   0 bag       (1001) bag       (1001)    11158 2016-09-25 14:05:57.000000 ephemeris-0.8.0/LICENSE
--rw-r--r--   0 bag       (1001) bag       (1001)     2974 2017-12-28 12:19:25.000000 ephemeris-0.8.0/setup.py
--rw-r--r--   0 bag       (1001) bag       (1001)     4183 2017-11-07 23:13:39.000000 ephemeris-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 bag       (1001) bag       (1001)     5386 2017-11-07 23:13:39.000000 ephemeris-0.8.0/CODE_OF_CONDUCT.rst
--rw-rw-r--   0 bag       (1001) bag       (1001)     1079 2016-09-25 14:05:57.000000 ephemeris-0.8.0/README.rst
--rw-r--r--   0 bag       (1001) bag       (1001)     3411 2017-12-29 20:56:19.000000 ephemeris-0.8.0/HISTORY.rst
--rw-rw-r--   0 bag       (1001) bag       (1001)       22 2016-09-25 14:05:57.000000 ephemeris-0.8.0/MANIFEST.in
+drwxr-xr-x   0 john       (502) staff       (20)        0 2018-05-23 10:37:46.000000 ephemeris-0.9.0/
+-rw-r--r--   0 john       (502) staff       (20)     5386 2017-06-16 19:41:07.000000 ephemeris-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 john       (502) staff       (20)     4183 2017-11-24 20:14:37.000000 ephemeris-0.9.0/CONTRIBUTING.rst
+drwxr-xr-x   0 john       (502) staff       (20)        0 2018-05-23 10:37:46.000000 ephemeris-0.9.0/ephemeris/
+-rw-r--r--   0 john       (502) staff       (20)     1870 2018-05-23 10:37:44.000000 ephemeris-0.9.0/ephemeris/__init__.py
+-rw-r--r--   0 john       (502) staff       (20)     1374 2018-05-07 17:48:44.000000 ephemeris-0.9.0/ephemeris/common_parser.py
+-rw-r--r--   0 john       (502) staff       (20)     2035 2018-05-07 17:48:44.000000 ephemeris-0.9.0/ephemeris/ephemeris_log.py
+-rw-r--r--   0 john       (502) staff       (20)     4439 2018-05-23 09:27:51.000000 ephemeris-0.9.0/ephemeris/generate_tool_list_from_ga_workflow_files.py
+-rw-r--r--   0 john       (502) staff       (20)     8225 2018-05-23 09:27:51.000000 ephemeris-0.9.0/ephemeris/get_tool_list_from_galaxy.py
+-rw-r--r--   0 john       (502) staff       (20)    13175 2018-05-07 17:48:44.000000 ephemeris-0.9.0/ephemeris/run_data_managers.py
+-rw-r--r--   0 john       (502) staff       (20)     5506 2018-05-23 09:27:51.000000 ephemeris-0.9.0/ephemeris/setup_data_libraries.py
+-rw-r--r--   0 john       (502) staff       (20)    43389 2018-05-23 09:27:51.000000 ephemeris-0.9.0/ephemeris/shed_tools.py
+-rwxr-xr-x   0 john       (502) staff       (20)     2315 2017-11-24 20:14:37.000000 ephemeris-0.9.0/ephemeris/sleep.py
+-rw-r--r--   0 john       (502) staff       (20)     1845 2018-03-12 18:58:57.000000 ephemeris-0.9.0/ephemeris/workflow_install.py
+drwxr-xr-x   0 john       (502) staff       (20)        0 2018-05-23 10:37:46.000000 ephemeris-0.9.0/ephemeris.egg-info/
+-rw-r--r--   0 john       (502) staff       (20)        1 2018-05-23 10:37:46.000000 ephemeris-0.9.0/ephemeris.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (502) staff       (20)      440 2018-05-23 10:37:46.000000 ephemeris-0.9.0/ephemeris.egg-info/entry_points.txt
+-rw-r--r--   0 john       (502) staff       (20)        1 2018-05-23 10:37:46.000000 ephemeris-0.9.0/ephemeris.egg-info/not-zip-safe
+-rw-r--r--   0 john       (502) staff       (20)     9490 2018-05-23 10:37:46.000000 ephemeris-0.9.0/ephemeris.egg-info/PKG-INFO
+-rw-r--r--   0 john       (502) staff       (20)       61 2018-05-23 10:37:46.000000 ephemeris-0.9.0/ephemeris.egg-info/requires.txt
+-rw-r--r--   0 john       (502) staff       (20)      638 2018-05-23 10:37:46.000000 ephemeris-0.9.0/ephemeris.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (502) staff       (20)       10 2018-05-23 10:37:46.000000 ephemeris-0.9.0/ephemeris.egg-info/top_level.txt
+-rw-r--r--   0 john       (502) staff       (20)     5788 2018-05-23 10:37:44.000000 ephemeris-0.9.0/HISTORY.rst
+-rw-r--r--   0 john       (502) staff       (20)    11158 2017-06-09 14:29:04.000000 ephemeris-0.9.0/LICENSE
+-rw-r--r--   0 john       (502) staff       (20)       22 2017-06-09 14:29:04.000000 ephemeris-0.9.0/MANIFEST.in
+-rw-r--r--   0 john       (502) staff       (20)     9490 2018-05-23 10:37:46.000000 ephemeris-0.9.0/PKG-INFO
+-rw-r--r--   0 john       (502) staff       (20)     1341 2018-03-12 18:58:57.000000 ephemeris-0.9.0/README.rst
+-rw-r--r--   0 john       (502) staff       (20)      310 2018-05-23 10:37:46.000000 ephemeris-0.9.0/setup.cfg
+-rw-r--r--   0 john       (502) staff       (20)     2974 2018-03-12 15:25:17.000000 ephemeris-0.9.0/setup.py
```

### Comparing `ephemeris-0.8.0/ephemeris/workflow_install.py` & `ephemeris-0.9.0/ephemeris/workflow_install.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,45 +4,49 @@
 import json
 import os
 
 from . import get_galaxy_connection
 from .common_parser import get_common_args
 
 
-def import_workflow(gi, path):
+def import_workflow(gi, path, publish_wf=False):
     """
     Given a connection to a Galaxy Instance (gi) and a path to a Galaxy workflow file,
     this function will import the worklfow into Galaxy.
     """
     with open(path, 'r') as wf_file:
         import_uuid = json.load(wf_file).get('uuid')
     existing_uuids = [d.get('latest_workflow_uuid') for d in gi.workflows.get_workflows()]
     if import_uuid not in existing_uuids:
-        gi.workflows.import_workflow_from_local_path(path)
+        gi.workflows.import_workflow_from_local_path(path, publish=publish_wf)
 
 
 def _parser():
     parent = get_common_args()
     parser = argparse.ArgumentParser(parents=[parent])
     parser.add_argument("-w", "--workflow_path",
                         required=True,
                         help='Path to a workflow file or a directory with multiple workflow files ending with ".ga"')
+    parser.add_argument("--publish_workflows",
+                        required=False,
+                        action='store_true',
+                        help='Flag to publish all imported workflows, so that they are viewable by other users')
     return parser
 
 
 def main():
     """
         This script uses bioblend to import .ga workflow files into a running instance of Galaxy
     """
     args = _parser().parse_args()
     gi = get_galaxy_connection(args)
 
     if os.path.isdir(args.workflow_path):
         for file_path in os.listdir(args.workflow_path):
             if file_path.endswith('.ga'):
-                import_workflow(gi, os.path.join(args.workflow_path, file_path))
+                import_workflow(gi, os.path.join(args.workflow_path, file_path), args.publish_workflows)
     else:
-        import_workflow(gi, args.workflow_path)
+        import_workflow(gi, args.workflow_path, args.publish_workflows)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ephemeris-0.8.0/ephemeris/__init__.py` & `ephemeris-0.9.0/ephemeris/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+
 # -*- coding: utf-8 -*-
 
 import yaml
 from bioblend import galaxy
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 PROJECT_NAME = "ephemeris"
 PROJECT_OWNER = PROJECT_USERAME = "galaxyproject"
 PROJECT_URL = "https://github.com/galaxyproject/ephemeris"
 PROJECT_AUTHOR = 'Galaxy Project and Community'
 PROJECT_EMAIL = 'jmchilton@gmail.com'
 RAW_CONTENT_URL = "https://raw.github.com/%s/%s/master/" % (
@@ -19,15 +20,15 @@
     if not url.startswith('http'):
         if log:
             log.warning('URL should start with http:// or https://. https:// chosen by default.')
         url = 'https://' + url
     return url
 
 
-def get_galaxy_connection(args, file=None, log=None):
+def get_galaxy_connection(args, file=None, log=None, login_required=True):
     """
     Return a Galaxy connection, given a user or an API key.
     If not given gets the arguments from the file.
     If either is missing returns None.
     """
     if file:
         file_content = load_yaml_file(file)
@@ -38,23 +39,25 @@
     galaxy_url = check_url(url, log)
     api_key = args.api_key or file_content.get('api_key')
 
     if args.user and args.password:
         return galaxy.GalaxyInstance(url=galaxy_url, email=args.user, password=args.password)
     elif api_key:
         return galaxy.GalaxyInstance(url=galaxy_url, key=api_key)
+    elif not login_required:
+        return galaxy.GalaxyInstance(url=galaxy_url)
     return None
 
 
 def load_yaml_file(filename):
     """
     Load YAML from the `tool_list_file` and return a dict with the content.
     """
     with open(filename, 'r') as f:
-        dictionary = yaml.load(f)
+        dictionary = yaml.safe_load(f)
     return dictionary
 
 
 def dump_to_yaml_file(content, file_name):
     """
     Dump YAML-compatible `content` to `file_name`.
     """
```

### Comparing `ephemeris-0.8.0/ephemeris/generate_tool_list_from_ga_workflow_files.py` & `ephemeris-0.9.0/ephemeris/generate_tool_list_from_ga_workflow_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     for step in tool_dictionary.values():
         tsr = step.get("tool_shed_repository")
         if tsr:
             starting_tool_list.append(tsr)
     tool_list = []
     for tool in starting_tool_list:
         sub_dic = {'name': tool['name'], 'owner': tool['owner'], 'revisions': [tool['changeset_revision']],
-                   'tool_panel_section_label': panel_label, 'tool_shed_url': 'https://'+tool['tool_shed']}
+                   'tool_panel_section_label': panel_label, 'tool_shed_url': 'https://' + tool['tool_shed']}
         tool_list.append(sub_dic)
     return tool_list
 
 
 def print_yaml_tool_list(tool_dictionary, output_file):
     with open(output_file, 'w') as F:
         F.write("\n".join([INSTALL_TOOL_DEPENDENCIES, INSTALL_REPOSITORY_DEPENDENCIES, INSTALL_RESOLVER_DEPENDENCIES, "", ""]))
@@ -71,18 +71,18 @@
 
 
 def reduce_tool_list(tool_list):
     for current_tool in tool_list:
         for tool in tool_list:
             if current_tool is tool:
                 continue
-            if (tool["name"] == current_tool['name']
-                    and tool['owner'] == current_tool['owner']
-                    and tool['tool_panel_section_label'] == current_tool['tool_panel_section_label']
-                    and tool['tool_shed_url'] == current_tool['tool_shed_url']):
+            if (tool["name"] == current_tool['name'] and
+                    tool['owner'] == current_tool['owner'] and
+                    tool['tool_panel_section_label'] == current_tool['tool_panel_section_label'] and
+                    tool['tool_shed_url'] == current_tool['tool_shed_url']):
                 current_tool["revisions"].extend(tool["revisions"])
                 tool_list.remove(tool)
         current_tool['revisions'] = list(set(current_tool['revisions']))
     return tool_list
 
 
 def generate_tool_list_from_workflow(workflow_files, panel_label, output_file):
```

### Comparing `ephemeris-0.8.0/ephemeris/run_data_managers.py` & `ephemeris-0.9.0/ephemeris/run_data_managers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-'''Run-data-managers is a tool for provisioning data on a galaxy instance.
+"""Run-data-managers is a tool for provisioning data on a galaxy instance.
 
 Run-data-managers has the ability to run multiple data managers that are interdependent.
 When a reference genome is needed for bwa-mem for example, Run-data-managers
 can first run a data manager to fetch the fasta file and run
 another data manager that indexes the fasta file for bwa-mem.
 This functionality depends on the "watch_tool_data_dir" setting in galaxy.ini to be True.
 Also, if a new data manager is installed, galaxy needs to be restarted in order for it's tool_data_dir to be watched.
@@ -17,35 +17,36 @@
 It checks it in the following way:
 * If the data manager has input variables "name" or "sequence_name" it will check if the "name" column in the data table already has this entry.
   "name" will take precedence over "sequence_name".
 * If the data manager has input variables "value", "sequence_id" or 'dbkey' it will check if
   the "value" column in the data table already has this entry.
   Value takes precedence over sequence_id which takes precedence over dbkey.
 * If none of the above input variables are specified the data manager will always run.
-'''
+"""
 import argparse
 import json
 import logging
 import time
 
-import yaml
 from bioblend.galaxy.tool_data import ToolDataClient
 from jinja2 import Template
 
 from . import get_galaxy_connection
+from . import load_yaml_file
 from .common_parser import get_common_args
 from .ephemeris_log import disable_external_library_logging, setup_global_logger
 
 
 DEFAULT_URL = "http://localhost"
+DEFAULT_SOURCE_TABLES = ["all_fasta"]
 
 
-def wait(gi, job_list):
+def wait(gi, job_list, log):
     """
-        Waits until a data_manager is finished or failed.
+        Waits until all jobs in a list are finished or failed.
         It will check the state of the created datasets every 30s.
         It will return a tuple: ( finished_jobs, failed_jobs )
     """
 
     failed_jobs = []
     successful_jobs = []
 
@@ -72,170 +73,226 @@
             job_list.remove(finished_job)
         # only sleep if job_list is not empty yet.
         if bool(job_list):
             time.sleep(30)
     return successful_jobs, failed_jobs
 
 
-def data_table_entry_exists(tool_data_client, data_table_name, entry, column='value'):
-    '''Checks whether an entry exists in the a specified column in the data_table.'''
-    try:
-        data_table_content = tool_data_client.show_data_table(data_table_name)
-    except Exception:
-        raise Exception('Table "%s" does not exist' % (data_table_name))
-
-    try:
-        column_index = data_table_content.get('columns').index(column)
-    except IndexError:
-        raise IndexError('Column "%s" does not exist in %s' % (column, data_table_name))
-
-    for field in data_table_content.get('fields'):
-        if field[column_index] == entry:
-            return True
-    return False
-
-
-def get_name_from_inputs(input_dict):
-    '''Returns the value that will most likely be recorded in the "name" column of the datatable. Or returns False'''
-    possible_keys = ['name', 'sequence_name']  # In order of importance!
-    for key in possible_keys:
+def get_first_valid_entry(input_dict, key_list):
+    """Iterates over key_list and returns the value of the first key that exists in the dictionary. Or returns None"""
+    for key in key_list:
         if key in input_dict:
             return input_dict.get(key)
-    return False
+    return None
 
 
-def get_value_from_inputs(input_dict):
-    '''Returns the value that will most likely be recorded in the "value" column of the datatable. Or returns False'''
-    possible_keys = ['value', 'sequence_id', 'dbkey']  # In order of importance!
-    for key in possible_keys:
-        if key in input_dict:
-            return input_dict.get(key)
-    return False
-
-
-def input_entries_exist_in_data_tables(tool_data_client, data_tables, input_dict):
-    '''Checks whether name and value entries from the input are already present in the data tables.
-    If an entry is missing in of the tables, this function returns False'''
-    value_entry = get_value_from_inputs(input_dict)
-    name_entry = get_name_from_inputs(input_dict)
-
-    # Return False if name and value entries are both False
-    if not value_entry and not name_entry:
-        return False
+class DataManagers:
+    def __init__(self, galaxy_instance, configuration):
+        """
+        :param galaxy_instance: A GalaxyInstance object (import from bioblend.galaxy)
+        :param configuration: A dictionary. Examples in the ephemeris documentation.
+        """
+        self.gi = galaxy_instance
+        self.config = configuration
+        self.tool_data_client = ToolDataClient(self.gi)
+        self.possible_name_keys = ['name', 'sequence_name']  # In order of importance!
+        self.possible_value_keys = ['value', 'sequence_id', 'dbkey']  # In order of importance!
+        self.data_managers = self.config.get('data_managers')
+        self.genomes = self.config.get('genomes', '')
+        self.source_tables = DEFAULT_SOURCE_TABLES
+        self.fetch_jobs = []
+        self.skipped_fetch_jobs = []
+        self.index_jobs = []
+        self.skipped_index_jobs = []
+
+    def initiate_job_lists(self):
+        """
+        Determines which data managers should be run to populate the data tables.
+        Distinguishes between fetch jobs (download files) and index jobs.
+        :return: populate self.fetch_jobs, self.skipped_fetch_jobs, self.index_jobs and self.skipped_index_jobs
+        """
+        self.fetch_jobs = []
+        self.skipped_fetch_jobs = []
+        self.index_jobs = []
+        self.skipped_index_jobs = []
+        for dm in self.data_managers:
+            jobs, skipped_jobs = self.get_dm_jobs(dm)
+            if self.dm_is_fetcher(dm):
+                self.fetch_jobs.extend(jobs)
+                self.skipped_fetch_jobs.extend(skipped_jobs)
+            else:
+                self.index_jobs.extend(jobs)
+                self.skipped_index_jobs.extend(skipped_jobs)
 
-    # Check every data table for existance of name and value
-    # Return False as soon as entry is not present
-    for data_table in data_tables:
-        if value_entry:
-            if not data_table_entry_exists(tool_data_client, data_table, value_entry, column='value'):
-                return False
-        if name_entry:
-            if not data_table_entry_exists(tool_data_client, data_table, name_entry, column='name'):
-                return False
-    # If all checks are passed the entries are present in the database tables.
-    return True
-
-
-def parse_items(items, genomes):
-    if bool(genomes):
-        items_template = Template(json.dumps(items))
-        rendered_items = items_template.render(genomes=json.dumps(genomes))
-        # Remove trailing " if present
-        rendered_items = rendered_items.strip('"')
-        items = json.loads(rendered_items)
-    return items
-
-
-def run_dm(args):
-    args.galaxy = args.galaxy or DEFAULT_URL
-    gi = get_galaxy_connection(args, log=log)
-    # should test valid connection
-    # The following should throw a ConnectionError when invalid API key or password
-    genomes = gi.genomes.get_genomes()  # Does not get genomes but preconfigured dbkeys
-    log.info('Number of possible dbkeys: %s' % str(len(genomes)))
-
-    tool_data_client = ToolDataClient(gi)
-
-    number_skipped_jobs = 0
-    all_failed_jobs = []
-    all_successful_jobs = []
-
-    conf = yaml.load(open(args.config))
-    genomes = conf.get('genomes', '')
-    for dm in conf.get('data_managers'):
-        items = parse_items(dm.get('items', ['']), genomes)
+    def get_dm_jobs(self, dm):
+        """Gets the job entries for a single dm. Puts entries that already present in skipped_job_list.
+        :returns job_list, skipped_job_list"""
         job_list = []
+        skipped_job_list = []
+        items = self.parse_items(dm.get('items', ['']))
         for item in items:
             dm_id = dm['id']
             params = dm['params']
             inputs = dict()
             # Iterate over all parameters, replace occurences of {{item}} with the current processing item
             # and create the tool_inputs dict for running the data manager job
             for param in params:
                 key, value = list(param.items())[0]
                 value_template = Template(value)
                 value = value_template.render(item=item)
                 inputs.update({key: value})
 
+            job = dict(tool_id=dm_id, inputs=inputs)
+
             data_tables = dm.get('data_table_reload', [])
-            # Only run if not run before.
-            if input_entries_exist_in_data_tables(tool_data_client, data_tables, inputs) and not args.overwrite:
-                log.info('%s already run for %s' % (dm_id, inputs))
-                number_skipped_jobs += 1
+            if self.input_entries_exist_in_data_tables(data_tables, inputs):
+                skipped_job_list.append(job)
             else:
-                # run the DM-job
-                job = gi.tools.run_tool(history_id=None, tool_id=dm_id, tool_inputs=inputs)
-                log.info('Dispatched job %i. Running DM: "%s" with parameters: %s' % (job['outputs'][0]['hid'], dm_id, inputs))
                 job_list.append(job)
-        successful_jobs, failed_jobs = wait(gi, job_list)
-        if failed_jobs:
-            if not args.ignore_errors:
-                raise Exception('Not all jobs successful! aborting...')
-                break
-            else:
-                log.error('Not all jobs successful! ignoring...')
-        all_successful_jobs += successful_jobs
-        all_failed_jobs += failed_jobs
-    job_summary = dict()
-    job_summary['successful_jobs'] = len(all_successful_jobs)
-    job_summary['failed_jobs'] = len(all_failed_jobs)
-    job_summary['skipped_jobs'] = number_skipped_jobs
-    return job_summary
+        return job_list, skipped_job_list
+
+    def dm_is_fetcher(self, dm):
+        """Checks whether the data manager fetches a sequence instead of indexing.
+        This is based on the source table.
+        :returns True if dm is a fetcher. False if it is not."""
+        data_tables = dm.get('data_table_reload', [])
+        for data_table in data_tables:
+            if data_table in self.source_tables:
+                return True
+        return False
+
+    def data_table_entry_exists(self, data_table_name, entry, column='value'):
+        """Checks whether an entry exists in the a specified column in the data_table."""
+        try:
+            data_table_content = self.tool_data_client.show_data_table(data_table_name)
+        except Exception:
+            raise Exception('Table "%s" does not exist' % data_table_name)
+
+        try:
+            column_index = data_table_content.get('columns').index(column)
+        except IndexError:
+            raise IndexError('Column "%s" does not exist in %s' % (column, data_table_name))
+
+        for field in data_table_content.get('fields'):
+            if field[column_index] == entry:
+                return True
+        return False
+
+    def input_entries_exist_in_data_tables(self, data_tables, input_dict):
+        """Checks whether name and value entries from the input are already present in the data tables.
+        If an entry is missing in of the tables, this function returns False"""
+        value_entry = get_first_valid_entry(input_dict, self.possible_value_keys)
+        name_entry = get_first_valid_entry(input_dict, self.possible_name_keys)
+
+        # Return False if name and value entries are both None
+        if not value_entry and not name_entry:
+            return False
+
+        # Check every data table for existence of name and value
+        # Return False as soon as entry is not present
+        for data_table in data_tables:
+            if value_entry:
+                if not self.data_table_entry_exists(data_table, value_entry, column='value'):
+                    return False
+            if name_entry:
+                if not self.data_table_entry_exists(data_table, name_entry, column='name'):
+                    return False
+        # If all checks are passed the entries are present in the database tables.
+        return True
+
+    def parse_items(self, items):
+        """
+        Parses items with jinja2.
+        :param items: the items to be parsed
+        :return: the parsed items
+        """
+        if bool(self.genomes):
+            items_template = Template(json.dumps(items))
+            rendered_items = items_template.render(genomes=json.dumps(self.genomes))
+            # Remove trailing " if present
+            rendered_items = rendered_items.strip('"')
+            items = json.loads(rendered_items)
+        return items
+
+    def run(self, log, ignore_errors=False, overwrite=False):
+        """
+        Runs the data managers.
+        :param log: The log to be used.
+        :param ignore_errors: Ignore erroring data_managers. Continue regardless.
+        :param overwrite: Overwrite existing entries in data tables
+        """
+        self.initiate_job_lists()
+        all_succesful_jobs = []
+        all_failed_jobs = []
+        all_skipped_jobs = []
+
+        def run_jobs(jobs, skipped_jobs):
+            job_list = []
+            for skipped_job in skipped_jobs:
+                if overwrite:
+                    log.info('%s already run for %s. Entry will be overwritten.' %
+                             (skipped_job["tool_id"], skipped_job["inputs"]))
+                    jobs.append(skipped_job)
+                else:
+                    log.info('%s already run for %s. Skipping.' % (skipped_job["tool_id"], skipped_job["inputs"]))
+                    all_skipped_jobs.append(skipped_job)
+            for job in jobs:
+                started_job = self.gi.tools.run_tool(history_id=None, tool_id=job["tool_id"], tool_inputs=job["inputs"])
+                log.info('Dispatched job %i. Running DM: "%s" with parameters: %s' %
+                         (started_job['outputs'][0]['hid'], job["tool_id"], job["inputs"]))
+                job_list.append(started_job)
+
+            successful_jobs, failed_jobs = wait(self.gi, job_list, log)
+            if failed_jobs:
+                if not ignore_errors:
+                    log.error('Not all jobs successful! aborting...')
+                    raise Exception('Not all jobs successful! aborting...')
+                else:
+                    log.warning('Not all jobs successful! ignoring...')
+            all_succesful_jobs.extend(successful_jobs)
+            all_failed_jobs.extend(failed_jobs)
+
+        log.info("Running data managers that populate the following source data tables: %s" % self.source_tables)
+        run_jobs(self.fetch_jobs, self.skipped_fetch_jobs)
+        log.info("Running data managers that index sequences.")
+        run_jobs(self.index_jobs, self.skipped_index_jobs)
+
+        log.info('Finished running data managers. Results:')
+        log.info('Successful jobs: %i ' % len(all_succesful_jobs))
+        log.info('Skipped jobs: %i ' % len(all_skipped_jobs))
+        log.info('Failed jobs: %i ' % len(all_failed_jobs))
 
 
 def _parser():
-    '''returns the parser object.'''
-    parent = get_common_args()
+    """returns the parser object."""
+    parent = get_common_args(log_file=True)
 
     parser = argparse.ArgumentParser(
         parents=[parent],
-        description='Running Galaxy data managers in a defined order with defined parameters.')
+        description='Running Galaxy data managers in a defined order with defined parameters.'
+                    "'watch_tool_data_dir' in galaxy config should be set to true.'")
     parser.add_argument("--config", required=True,
                         help="Path to the YAML config file with the list of data managers and data to install.")
     parser.add_argument("--overwrite", action="store_true",
                         help="Disables checking whether the item already exists in the tool data table.")
     parser.add_argument("--ignore_errors", action="store_true",
                         help="Do not stop running when jobs have failed.")
     return parser
 
 
 def main():
-    global log
     disable_external_library_logging()
-    log = setup_global_logger(name=__name__, log_file='/tmp/galaxy_data_manager_install.log')
     parser = _parser()
     args = parser.parse_args()
+    log = setup_global_logger(name=__name__, log_file=args.log_file)
     if args.verbose:
-
         log.setLevel(logging.DEBUG)
     else:
         log.setLevel(logging.INFO)
-    log.info("Running data managers...")
-    job_summary = run_dm(args)
-    log.info('Finished running data managers. Results:')
-    log.info('Successful jobs: %i ' % job_summary['successful_jobs'])
-    log.info('Skipped jobs: %i ' % job_summary['skipped_jobs'])
-    log.info('Failed jobs: %i ' % job_summary['failed_jobs'])
+    gi = get_galaxy_connection(args, file=args.config, log=log, login_required=True)
+    config = load_yaml_file(args.config)
+    data_managers = DataManagers(gi, config)
+    data_managers.run(log, args.ignore_errors, args.overwrite)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ephemeris-0.8.0/ephemeris/sleep.py` & `ephemeris-0.9.0/ephemeris/sleep.py`

 * *Files identical despite different names*

### Comparing `ephemeris-0.8.0/ephemeris/ephemeris_log.py` & `ephemeris-0.9.0/ephemeris/ephemeris_log.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import tempfile
 
 
 class ProgressConsoleHandler(logging.StreamHandler):
     """
     A handler class which allows the cursor to stay on
     one line for selected messages
     """
@@ -45,11 +46,17 @@
     console = logging.StreamHandler()
     console.setFormatter(formatter)
 
     logger = logging.getLogger(name)
     logger.setLevel(logging.DEBUG)
     logger.addHandler(progress)
 
-    if log_file:
-        file_handler = logging.FileHandler(log_file)
-        logger.addHandler(file_handler)
+    if not log_file:
+        # delete = false is chosen here because it is always nice to have a log file
+        # ready if you need to debug. Not having the "if only I had set a log file"
+        # moment after the fact.
+        temp = tempfile.NamedTemporaryFile(prefix="ephemeris_", delete=False)
+        log_file = temp.name
+    file_handler = logging.FileHandler(log_file)
+    logger.addHandler(file_handler)
+    logger.info("Storing log file in: {0}".format(log_file))
     return logger
```

### Comparing `ephemeris-0.8.0/ephemeris/shed_tools.py` & `ephemeris-0.9.0/ephemeris/shed_tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,27 +32,30 @@
 `tool_config_file` to include it.
 """
 
 # Required libraries:
 # bioblend, pyyaml
 
 import datetime as dt
+import json
+import re
 import sys
 import time
 from argparse import ArgumentParser
 
 import yaml
 from bioblend.galaxy.client import ConnectionError
 from bioblend.galaxy.toolshed import ToolShedClient
 from bioblend.toolshed import ToolShedInstance
+from galaxy.tools.verify.interactor import GalaxyInteractorApi, verify_tool
 
 from . import get_galaxy_connection, load_yaml_file
 from .common_parser import get_common_args
 from .ephemeris_log import disable_external_library_logging, setup_global_logger
-from .get_tool_list_from_galaxy import GiToToolYaml
+from .get_tool_list_from_galaxy import GiToToolYaml, tools_for_repository
 
 # If no toolshed is specified for a tool/tool-suite, the Main Tool Shed is taken
 MTS = 'https://toolshed.g2.bx.psu.edu/'  # Main Tool Shed
 
 # The behavior of a tool installation and its dependencies can be controlled in a few ways.
 # You can add
 #   - install_tool_dependencies: True or False          (traditional Tool Shed dependencies)
@@ -61,14 +64,16 @@
 # to every tool section in the tool-yaml file or you can add these options to the top of the yaml
 # file (next to galaxy_instance or api_key) to set a global default value, which can be overwritten
 # later in every section. Not specifying any of these options will use the values below,
 # means traditional tool_dependencies will not be installed.
 INSTALL_TOOL_DEPENDENCIES = False
 INSTALL_REPOSITORY_DEPENDENCIES = True
 INSTALL_RESOLVER_DEPENDENCIES = True
+EXIT_CODE_INSTALL_ERRORS = 1
+EXIT_CODE_TOOL_TEST_ERRORS = 2
 
 
 def _ensure_log_configured(name):
     # For library-style usage - just ensure a log exists and use ephemeris name.
     if 'log' not in globals():
         global log
         log = setup_global_logger(name)
@@ -263,86 +268,108 @@
     for repo_dictionary in repository_dictionaries_list:
         category_list.append(repo_dictionary.get('id'))
     return set(category_list)
 
 
 def _parser():
     """construct the parser object"""
-    common_arguments = get_common_args()
+    common_arguments = get_common_args(log_file=True)
     parser = ArgumentParser()
     subparsers = parser.add_subparsers()
 
     # A list of defaults is needed. Otherwise the shed-tools install parser will not return
     # update_tools in the name space and shed-tool update will not return all the install
     # variables.
     parser.set_defaults(
-        update_tools=False,
+        action="install",
         tool_list_file=None,
         tool_yaml=None,
         owner=None,
         name=None,
         tool_panel_section_id=None,
         tool_panel_section_label=None,
         revisions=None,
         tool_shed_url=None,
         skip_tool_dependencies=False,
         install_resolver_dependencies=False,
-        force_latest_revision=False
+        force_latest_revision=False,
+        test=False,
+        test_user_api_key=None,
+        test_user="ephemeris@galaxyproject.org",
+        test_json="tool_test_output.json",
+        test_existing=False,
     )
     install_command_parser = subparsers.add_parser(
         "install",
         help="This installs tools in Galaxy from the Tool Shed."
              "Use shed-tools install --help for more information",
         parents=[common_arguments],
-        )
-    install_command_parser.add_argument(
-        "-t", "--toolsfile",
-        dest="tool_list_file",
-        help="Tools file to use (see tool_list.yaml.sample)",)
-    install_command_parser.add_argument(
-        "-y", "--yaml_tool",
-        dest="tool_yaml",
-        help="Install tool represented by yaml string",)
-    install_command_parser.add_argument(
-        "--name",
-        help="The name of the tool to install (only applicable "
-             "if the tools file is not provided).")
-    install_command_parser.add_argument(
-        "--owner",
-        help="The owner of the tool to install (only applicable "
-             "if the tools file is not provided).")
+    )
+    install_command_parser.set_defaults(
+        update_tools=False
+    )
+    update_command_parser = subparsers.add_parser(
+        "update",
+        help="This updates all tools in Galaxy to the latest revision. "
+             "Use shed-tools update --help for more information",
+        parents=[common_arguments])
+
+    test_command_parser = subparsers.add_parser(
+        "test",
+        help="This tests the supplied list of tools in Galaxy. "
+             "Use shed-tools test --help for more information",
+        parents=[common_arguments])
+
+    for command_parser in [install_command_parser, test_command_parser]:
+        command_parser.add_argument(
+            "-t", "--toolsfile",
+            dest="tool_list_file",
+            help="Tools file to use (see tool_list.yaml.sample)",)
+        command_parser.add_argument(
+            "-y", "--yaml_tool",
+            dest="tool_yaml",
+            help="Install tool represented by yaml string",)
+        command_parser.add_argument(
+            "--name",
+            help="The name of the tool to install (only applicable "
+                 "if the tools file is not provided).")
+        command_parser.add_argument(
+            "--owner",
+            help="The owner of the tool to install (only applicable "
+                 "if the tools file is not provided).")
+        command_parser.add_argument(
+            "--revisions",
+            default=None,
+            nargs='*',
+            dest="revisions",
+            help="The revisions of the tool repository that will be installed. "
+                 "All revisions must be specified after this flag by a space."
+                 "Example: --revisions 0a5c7992b1ac f048033da666"
+                 "(Only applicable if the tools file is not provided).")
+        command_parser.add_argument(
+            "--toolshed",
+            dest="tool_shed_url",
+            help="The Tool Shed URL where to install the tool from. "
+                 "This is applicable only if the tool info is "
+                 "provided as an option vs. in the tools file.")
+
     install_command_parser.add_argument(
         "--section",
         dest="tool_panel_section_id",
         help="Galaxy tool panel section ID where the tool will "
              "be installed (the section must exist in Galaxy; "
              "only applicable if the tools file is not provided).")
     install_command_parser.add_argument(
         "--section_label",
         default=None,
         dest="tool_panel_section_label",
         help="Galaxy tool panel section label where tool will be installed "
              "(if the section does not exist, it will be created; "
              "only applicable if the tools file is not provided).")
     install_command_parser.add_argument(
-        "--revisions",
-        default=None,
-        nargs='*',
-        dest="revisions",
-        help="The revisions of the tool repository that will be installed. "
-             "All revisions must be specified after this flag by a space."
-             "Example: --revisions 0a5c7992b1ac f048033da666"
-             "(Only applicable if the tools file is not provided).")
-    install_command_parser.add_argument(
-        "--toolshed",
-        dest="tool_shed_url",
-        help="The Tool Shed URL where to install the tool from. "
-             "This is applicable only if the tool info is "
-             "provided as an option vs. in the tools file.")
-    install_command_parser.add_argument(
         "--skip_install_tool_dependencies",
         action="store_true",
         dest="skip_tool_dependencies",
         help="Skip the installation of tool dependencies using classic toolshed packages. "
              "Can be overwritten on a per-tool basis in the tools file.")
     install_command_parser.add_argument(
         "--install_resolver_dependencies",
@@ -354,21 +381,83 @@
              "Can be overwritten on a per-tool basis in the tools file")
     install_command_parser.add_argument(
         "--latest",
         action="store_true",
         dest="force_latest_revision",
         help="Will override the revisions in the tools file and always install the latest revision.")
 
-    update_command_parser = subparsers.add_parser(
-        "update",
-        help="This updates all tools in Galaxy to the latest revision."
-             "Use shed-tools update --help for more information",
-        parents=[common_arguments])
+    for command_parser in [update_command_parser, install_command_parser]:
+        command_parser.add_argument(
+            "--test",
+            action="store_true",
+            dest="test",
+            help="Run tool tests on install tools, requires Galaxy 18.05 or newer."
+        )
+        command_parser.add_argument(
+            "--test_existing",
+            action="store_true",
+            help="If testing tools during install, also run tool tests on repositories already installed "
+                 "(i.e. skipped repositories)."
+        )
+        command_parser.add_argument(
+            "--test_json",
+            dest="test_json",
+            help="If testing tools, record tool test output to specified file. "
+                 "This file can be turned into reports with ``planemo test_reports <output.json>``."
+        )
+        command_parser.add_argument(
+            "--test_user_api_key",
+            dest="test_json",
+            help="If testing tools, a user is needed to execute the tests. "
+                 "This can be different the --api_key which is assumed to be an admin key. "
+                 "If --api_key is a valid user (e.g. it is not a master API key) this does "
+                 "not need to be specified and --api_key will be reused."
+        )
+        command_parser.add_argument(
+            "--test_user",
+            dest="test_json",
+            help="If testing tools, a user is needed to execute the tests. "
+                 "If --api_key is a master api key (i.e. not tied to a real user) and "
+                 "--test_user_api_key isn't specified, this user email will be used. This "
+                 "user will be created if needed."
+        )
+
+    # Same test_json as above but language modified for test instead of install/update.
+    test_command_parser.add_argument(
+        "--test_json",
+        dest="test_json",
+        help="Record tool test output to specified file. "
+             "This file can be turned into reports with ``planemo test_reports <output.json>``."
+    )
+
+    test_command_parser.add_argument(
+        "--test_user_api_key",
+        dest="test_user_api_key",
+        help="A user is needed to execute the tests. "
+             "This can be different the --api_key which is assumed to be an admin key. "
+             "If --api_key is a valid user (e.g. it is not a master API key) this does "
+             "not need to be specified and --api_key will be reused."
+    )
+    test_command_parser.add_argument(
+        "--test_user",
+        dest="test_user",
+        help="A user is needed to execute the tests. "
+             "If --api_key is a master api key (i.e. not tied to a real user) and "
+             "--test_user_api_key isn't specified, this user email will be used. This "
+             "user will be created if needed."
+    )
+
     update_command_parser.set_defaults(
-        update_tools=True,
+        action="update",
+        update_tools=True
+    )
+
+    test_command_parser.set_defaults(
+        action="test",
+        update_tools=False
     )
 
     return parser
 
 
 def _parse_cli_options():
     """
@@ -401,15 +490,15 @@
             if key != 'revisions':
                 new_dictionary[key] = value
         return new_dictionary
 
     flattened_list = []
     for repo_info in repositories:
         revisions = repo_info.get('revisions', [])
-        if len(revisions) > 1:
+        if revisions is not None and len(revisions) > 1:
             for revision in revisions:
                 stripped_repo_info = _strip_revisions(repo_info)
                 stripped_repo_info['changeset_revision'] = revision
                 flattened_list.append(stripped_repo_info)
         elif revisions:  # A single revisions was defined so keep it
             stripped_repo_info = _strip_revisions(repo_info)
             stripped_repo_info['changeset_revision'] = revisions[0]
@@ -485,19 +574,20 @@
         install_repository_dependencies = repository_list.get(
             'install_repository_dependencies', INSTALL_REPOSITORY_DEPENDENCIES)
         install_resolver_dependencies = repository_list.get(
             'install_resolver_dependencies', INSTALL_RESOLVER_DEPENDENCIES)
         install_tool_dependencies = repository_list.get(
             'install_tool_dependencies', INSTALL_TOOL_DEPENDENCIES)
     elif options.tool_yaml:
-        repositories = [yaml.load(options.tool_yaml)]
-    elif options.update_tools:
+        repositories = [yaml.safe_load(options.tool_yaml)]
+    elif options.action == "update":
         get_repository_list = GiToToolYaml(
             gi=gi,
-            skip_tool_panel_section_name=False
+            skip_tool_panel_section_name=False,
+            get_data_managers=True
         )
         repository_list = get_repository_list.tool_list
         repositories = repository_list['tools']
     else:
         # An individual tool was specified on the command line
         repositories = [{
             "owner": options.owner,
@@ -514,49 +604,66 @@
 
     elif repo_list_file:
         install_tool_dependencies = install_tool_dependencies
         install_repository_dependencies = install_repository_dependencies
 
     install_resolver_dependencies = options.install_resolver_dependencies or install_resolver_dependencies
 
-    force_latest_revision = options.force_latest_revision or options.update_tools
+    force_latest_revision = options.force_latest_revision or options.action == "update"
 
     return InstallToolManager(repositories=repositories,
                               gi=gi,
                               default_install_tool_dependencies=install_tool_dependencies,
                               default_install_repository_dependencies=install_repository_dependencies,
                               default_install_resolver_dependencies=install_resolver_dependencies,
-                              force_latest_revision=force_latest_revision
+                              force_latest_revision=force_latest_revision,
+                              test=options.test,
+                              test_user=options.test_user,
+                              test_user_api_key=options.test_user_api_key,
+                              test_existing=options.test_existing,
+                              test_json=options.test_json,
                               )
 
 
 class InstallToolManager(object):
 
     def __init__(self,
                  repositories,
                  gi,
                  default_install_tool_dependencies=INSTALL_TOOL_DEPENDENCIES,
                  default_install_resolver_dependencies=INSTALL_RESOLVER_DEPENDENCIES,
                  default_install_repository_dependencies=INSTALL_REPOSITORY_DEPENDENCIES,
                  require_tool_panel_info=True,
-                 force_latest_revision=False):
+                 force_latest_revision=False,
+                 test=False,
+                 test_user_api_key=None,
+                 test_user="ephemeris@galaxyproject.org",
+                 test_existing=False,
+                 test_json="tool_test_output.json"):
         self.repositories = repositories
         self.gi = gi
         self.tsc = ToolShedClient(self.gi)
         self.require_tool_panel_info = require_tool_panel_info
         self.install_tool_dependencies = default_install_tool_dependencies
         self.install_resolver_dependencies = default_install_resolver_dependencies
         self.install_repository_dependencies = default_install_repository_dependencies
         self.force_latest_revision = force_latest_revision
         self.errored_repositories = []
         self.skipped_repositories = []
         self.installed_repositories = []
+        self.test = test
+        self.test_existing = test_existing
+        self.test_json = test_json
+        self.test_user_api_key = test_user_api_key
+        self.test_user = test_user
+        self.tests_passed = []
+        self.test_exceptions = []
 
     def install_repositories(self):
-        """
+        """Attempt to ensure each repository in ``self.repositories`` is installed.
         """
         installation_start = dt.datetime.now()
         installed_repositories_list = installed_repository_revisions(self.gi)  # installed tools list
         counter = 0
         repositories = _flatten_repo_info(self.repositories)
         total_num_repositories = len(repositories)
         default_err_msg = ('All repositories that you are attempting to install '
@@ -652,17 +759,99 @@
         log.info("Errored repositories ({0}): {1}".format(
             len(self.errored_repositories),
             [(
                 t['name'],
                 t.get('changeset_revision', "")
             ) for t in self.errored_repositories])
         )
-        log.info("All repositories have been processed.")
+        log.info("All repositories have been installed.")
+        if self.test:
+            target_repositories = self.installed_repositories
+            if self.test_existing:
+                target_repositories += self.skipped_repositories
+            self.test_repositories(target_repositories=target_repositories)
         log.info("Total run time: {0}".format(dt.datetime.now() - installation_start))
 
+    def test_repositories(self, target_repositories=None):
+        """Run tool tests for each tool in supplied repositories list or ``self.repositories``.
+        """
+        tool_test_start = dt.datetime.now()
+        if target_repositories is None:
+            # Consider a variant of this that doesn't even consume a tool list YAML? target
+            # something like installed_repository_revisions(self.gi)
+            target_repositories = self.repositories
+        installed_tools = []
+        for target_repository in target_repositories:
+            repo_tools = tools_for_repository(self.gi, target_repository)
+            installed_tools.extend(repo_tools)
+
+        all_test_results = []
+
+        for tool in installed_tools:
+            tool_test_results = self._test_tool(tool)
+            all_test_results.extend(tool_test_results)
+
+        report_obj = {
+            'version': '0.1',
+            'tests': all_test_results,
+        }
+        with open(self.test_json or "tool_test_output.json", "w") as f:
+            json.dump(report_obj, f)
+        log.info("Passed tool tests ({0}): {1}".format(
+            len(self.tests_passed),
+            [t for t in self.tests_passed])
+        )
+        log.info("Failed tool tests ({0}): {1}".format(
+            len(self.test_exceptions),
+            [t[0] for t in self.test_exceptions])
+        )
+        log.info("Total tool test time: {0}".format(dt.datetime.now() - tool_test_start))
+
+    def _test_tool(self, tool):
+        test_user_api_key = self.test_user_api_key
+        if test_user_api_key is None:
+            whoami = self.gi.make_get_request(self.gi.url + "/whoami").json()
+            if whoami is not None:
+                test_user_api_key = self.gi.key
+        galaxy_interactor_kwds = {
+            "galaxy_url": re.sub('/api', '', self.gi.url),
+            "master_api_key": self.gi.key,
+            "api_key": None,  # TODO
+            "keep_outputs_dir": '',
+        }
+        if test_user_api_key is None:
+            galaxy_interactor_kwds["test_user"] = self.test_user
+        galaxy_interactor = GalaxyInteractorApi(**galaxy_interactor_kwds)
+        tool_id = tool["id"]
+        tool_version = tool["version"]
+        tool_test_dicts = galaxy_interactor.get_tool_tests(tool_id, tool_version=tool_version)
+        test_indices = list(range(len(tool_test_dicts)))
+        tool_test_results = []
+
+        for test_index in test_indices:
+            test_id = tool_id + "-" + str(test_index)
+
+            def register(job_data):
+                tool_test_results.append({
+                    'id': test_id,
+                    'has_data': True,
+                    'data': job_data,
+                })
+
+            try:
+                verify_tool(
+                    tool_id, galaxy_interactor, test_index=test_index, tool_version=tool_version,
+                    register_job_data=register, quiet=True
+                )
+                self.tests_passed.append(test_id)
+            except Exception as e:
+                self.test_exceptions.append((test_id, e))
+
+        return tool_test_results
+
     def create_repository_install_payload(self, repository_info):
         """
         For each listed repository (repository_info) we generate a payload that contains all
         required parameters, filling up missing parameters with user-defined and/or default settings.
         Return `None` if a required parameter is missing
         """
         repository = dict()  # Payload for the repository we are installing
@@ -730,29 +919,34 @@
             repository['changeset_revision'] = installable_revisions[-1]
         return repository
 
 
 def main():
     global log
     disable_external_library_logging()
-    log = setup_global_logger(name=__name__, log_file='/tmp/galaxy_tool_install.log')
     options = _parse_cli_options()
+    log = setup_global_logger(name=__name__, log_file=options.log_file)
+    install_tool_manager = None
     if options.tool_list_file or options.tool_yaml or \
             options.name and options.owner and (options.tool_panel_section_id or options.tool_panel_section_label):
-        if options.update_tools:
-            sys.exit("--update can not be used together with tools to be installed.")
+        if options.action == "update":
+            sys.exit("update command can not be used together with tools to be installed.")
         install_tool_manager = get_install_repository_manager(options)
-        install_tool_manager.install_repositories()
-        if install_tool_manager.errored_repositories:
-            sys.exit(1)
+        if options.action == "test":
+            install_tool_manager.test_repositories()
+        else:
+            install_tool_manager.install_repositories()
     elif options.update_tools:
         install_tool_manager = get_install_repository_manager(options)
         install_tool_manager.install_repositories()
-        if install_tool_manager.errored_repositories:
-            sys.exit(1)
     else:
         sys.exit("Must provide a tool list file, individual tools info , a list of data manager tasks or issue the update command. "
                  "Look at usage.")
 
+    if install_tool_manager.errored_repositories:
+        sys.exit(EXIT_CODE_INSTALL_ERRORS)
+    elif install_tool_manager.test_exceptions:
+        sys.exit(EXIT_CODE_TOOL_TEST_ERRORS)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `ephemeris-0.8.0/ephemeris/get_tool_list_from_galaxy.py` & `ephemeris-0.9.0/ephemeris/get_tool_list_from_galaxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,97 +3,121 @@
 
 
 from argparse import ArgumentDefaultsHelpFormatter
 from argparse import ArgumentParser
 from distutils.version import StrictVersion
 
 import yaml
-from bioblend.galaxy import GalaxyInstance
 from bioblend.galaxy.tools import ToolClient
 
-from . import check_url
+from . import get_galaxy_connection
 from .common_parser import get_common_args
 
 
+def get_tool_panel(gi):
+    tool_client = ToolClient(gi)
+    return tool_client.get_tool_panel()
+
+
+def tools_for_repository(gi, repository):
+    tool_shed_url = repository.get('tool_shed_url')
+    name = repository['name']
+    owner = repository['owner']
+    changeset_revision = repository.get('changeset_revision')
+
+    tools = []
+
+    def handle_tool(tool_elem):
+        if not tool_elem.get('tool_shed_repository', None):
+            return
+        tsr = tool_elem['tool_shed_repository']
+        if tsr['name'] != name or tsr['owner'] != owner:
+            return
+
+        if tool_shed_url and tsr['tool_shed'] != tool_shed_url:
+            return
+
+        if changeset_revision and changeset_revision != tsr["changeset_revision"]:
+            return
+
+        tools.append(tool_elem)
+
+    walk_tools(get_tool_panel(gi), handle_tool)
+
+    return tools
+
+
+def walk_tools(tool_panel, f):
+    for elem in tool_panel:
+        if elem['model_class'] == 'Tool':
+            f(elem)
+        elif elem['model_class'] == 'ToolSection':
+            walk_tools(elem.get("elems", []), f)
+
+
 class GiToToolYaml:
     def __init__(self, gi,
                  include_tool_panel_section_id=False,
                  skip_tool_panel_section_name=True,
-                 skip_changeset_revision=False):
-
+                 skip_changeset_revision=False,
+                 get_data_managers=False):
         self.gi = gi
         self.include_tool_panel_section_id = include_tool_panel_section_id
         self.skip_tool_panel_section_name = skip_tool_panel_section_name
         self.skip_changeset_revision = skip_changeset_revision
+        self.get_data_managers = get_data_managers
         self.repository_list = self.get_repositories()
         self.repository_list = self.merge_tool_changeset_revisions()
         self.filter_section_name_or_id_or_changeset()
         self.tool_list = {"tools": self.repository_list}
 
     @property
     def toolbox(self):
         """
         Gets the toolbox elements from <galaxy_url>/api/tools
         """
+        return get_tool_panel(self.gi)
+
+    @property
+    def installed_tool_list(self):
+        """
+        gets a tool list from the toolclient
+        :return:
+        """
         tool_client = ToolClient(self.gi)
-        return tool_client.get_tool_panel()
+        return tool_client.get_tools()
 
     def get_repositories(self):
         """
         Toolbox elements returned by api/tools may be of class ToolSection or Tool.
         Parse these accordingly to get a list of repositories.
         """
         repositories = []
-        for elem in self.toolbox:
-            if elem['model_class'] == 'Tool':
-                repo = self.get_repo_from_tool(elem)
-                if repo:
-                    repositories.append(repo)
-            elif elem['model_class'] == 'ToolSection':
-                new_repos = self.get_repos_from_section(elem)
-                if new_repos:
-                    repositories.extend(new_repos)
-        return repositories
 
-    def get_repo_from_tool(self, tool):
-        """
-        Get the minimum items required for re-installing a (list of) tools
-        """
-        if not tool.get('tool_shed_repository', None):
-            return {}
-        tsr = tool['tool_shed_repository']
-        repo = {'name': tsr['name'],
-                'owner': tsr['owner'],
-                'tool_shed_url': tsr['tool_shed'],
-                'revisions': [tsr['changeset_revision']],
-                'tool_panel_section_id': tool['panel_section_id'],
-                'tool_panel_section_label': tool['panel_section_name']}
-        return repo
-
-    def get_repos_from_section(self, section):
-        repos = []
-        for elem in section['elems']:
-            if elem['model_class'] == 'Tool':
-                repo = self.get_repo_from_tool(elem)
-                if repo:
-                    repos.append(repo)
-            elif elem['model_class'] == 'ToolSection':
-                new_repos = self.get_repos_from_section(elem)
-                if new_repos:
-                    repos.extend(new_repos)
-        return repos
+        def record_repo(tool_elem):
+            repo = get_repo_from_tool(tool_elem)
+            if repo:
+                repositories.append(repo)
+
+        walk_tools(self.toolbox, record_repo)
+
+        if self.get_data_managers:
+            for tool in self.installed_tool_list:
+                if tool.get("model_class") == 'DataManagerTool':
+                    repositories.append(get_repo_from_tool(tool))
+        return repositories
 
     def merge_tool_changeset_revisions(self):
         """
         Each installed changeset revision of a tool is listed individually.
         Merge revisions of the same tool into a list.
         """
         repositories = {}
         repo_key_template = "{tool_shed_url}|{name}|{owner}|{tool_panel_section_id}|{tool_panel_section_label}"
-        for i, tool in enumerate(self.repository_list):
+        for tool in self.repository_list:
             repo_key = repo_key_template.format(**tool)
             if repo_key in repositories:
                 repositories[repo_key].extend(tool['revisions'])
             else:
                 repositories[repo_key] = tool['revisions']
         new_repository_list = []
         for repo_key, changeset_revisions in repositories.items():
@@ -124,41 +148,57 @@
     def write_to_yaml(self, output_file):
         with open(output_file, "w") as output:
             output.write(yaml.safe_dump(self.tool_list, default_flow_style=False))
 
 
 def _parser():
     '''Creates the parser object.'''
-    parent = get_common_args(login_required=False)
+    parent = get_common_args(login_required=True)
     parser = ArgumentParser(parents=[parent],
-                            usage="usage: python %(prog)s <options>",
-                            epilog='Example usage: python get_tool_yml_from_gi.py '
-                                   '-g https://usegalaxy.org/ -o tool_list.yml',
                             formatter_class=ArgumentDefaultsHelpFormatter)
     parser.add_argument("-o", "--output-file",
                         required=True,
                         dest="output",
                         help="tool_list.yml output file")
-    parser.add_argument("-include_id", "--include_tool_panel_id",
+    parser.add_argument("--include_tool_panel_id",
                         action="store_true",
                         help="Include tool_panel_id in tool_list.yml ? "
                              "Use this only if the tool panel id already exists. See "
                              "https://github.com/galaxyproject/ansible-galaxy-tools/blob/master/files/tool_list.yaml.sample")
-    parser.add_argument("-skip_name", "--skip_tool_panel_name",
+    parser.add_argument("--skip_tool_panel_name",
                         action="store_true",
                         help="Do not include tool_panel_name in tool_list.yml ?")
-    parser.add_argument("-skip_changeset", "--skip_changeset_revision",
+    parser.add_argument("--skip_changeset_revision",
                         action="store_true",
                         help="Do not include the changeset revision when generating the tool list."
                              "Use this if you would like to use the list to update all the tools in"
                              "your galaxy instance using shed-install."
                         )
+    parser.add_argument("--get_data_managers",
+                        action="store_true",
+                        help="Include the data managers in the tool list. Requires login details")
     return parser
 
 
+def get_repo_from_tool(tool):
+    """
+    Get the minimum items required for re-installing a (list of) tools
+    """
+    if not tool.get('tool_shed_repository', None):
+        return {}
+    tsr = tool['tool_shed_repository']
+    repo = {'name': tsr['name'],
+            'owner': tsr['owner'],
+            'tool_shed_url': tsr['tool_shed'],
+            'revisions': [tsr['changeset_revision']],
+            'tool_panel_section_id': tool['panel_section_id'],
+            'tool_panel_section_label': tool['panel_section_name']}
+    return repo
+
+
 def _parse_cli_options():
     """
     Parse command line options, returning `parse_args` from `ArgumentParser`.
     """
     parser = _parser()
     return parser.parse_args()
 
@@ -167,20 +207,20 @@
     version = gi.config.get_version()
     if StrictVersion(version['version_major']) < StrictVersion('16.04'):
         raise Exception('This script needs galaxy version 16.04 or newer')
 
 
 def main():
     options = _parse_cli_options()
-    galaxy_url = check_url(options.galaxy)
-    gi = GalaxyInstance(galaxy_url)
+    gi = get_galaxy_connection(options, login_required=False)
     check_galaxy_version(gi)
     gi_to_tool_yaml = GiToToolYaml(
         gi=gi,
         include_tool_panel_section_id=options.include_tool_panel_id,
         skip_tool_panel_section_name=options.skip_tool_panel_name,
-        skip_changeset_revision=options.skip_changeset_revision)
+        skip_changeset_revision=options.skip_changeset_revision,
+        get_data_managers=options.get_data_managers)
     gi_to_tool_yaml.write_to_yaml(options.output)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ephemeris-0.8.0/PKG-INFO` & `ephemeris-0.9.0/HISTORY.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,151 +1,143 @@
-Metadata-Version: 1.1
-Name: ephemeris
-Version: 0.8.0
-Summary: Ephemeris is an opinionated library and set of scripts for managing the bootstrapping of Galaxy project plugins - tools, index data, and workflows.
-Home-page: https://github.com/galaxyproject/ephemeris
-Author: Galaxy Project and Community
-Author-email: jmchilton@gmail.com
-License: AFL
-Description-Content-Type: UNKNOWN
-Description: 
-        .. image:: https://readthedocs.org/projects/pip/badge/?version=latest
-           :target: https://ephemeris.readthedocs.org
-        
-        .. image:: https://badge.fury.io/py/ephemeris.svg
-           :target: https://pypi.python.org/pypi/ephemeris/
-        
-        .. image:: https://travis-ci.org/galaxyproject/ephemeris.png?branch=master
-           :target: https://travis-ci.org/galaxyproject/ephemeris
-        
-        .. image:: https://coveralls.io/repos/galaxyproject/ephemeris/badge.svg?branch=master
-           :target: https://coveralls.io/r/galaxyproject/ephemeris?branch=master
-        
-        Ephemeris is a small Python library and set of scripts for managing the
-        bootstrapping of Galaxy_ plugins - tools, index data, and workflows.
-        
-        * Free software: Academic Free License version 3.0
-        * Documentation: https://ephemeris.readthedocs.org.
-        * Code: https://github.com/galaxyproject/ephemeris
-        
-        
-        .. _Galaxy: http://galaxyproject.org/
-        .. _GitHub: https://github.com/
-        .. _Docker: https://www.docker.com/
-        .. _Homebrew: http://brew.sh/
-        .. _linuxbrew: https://github.com/Homebrew/linuxbrew
-        .. _Vagrant: https://www.vagrantup.com/
-        .. _Travis CI: http://travis-ci.org/
-        
-        
-        
-        
-        History
-        -------
-        
-        .. to_doc
-        
-        ---------------------
-        0.8.1 (2017-12-29)
-        ---------------------
-        
-        ---------------------
-        0.8.0 (2017-12-29)
-        ---------------------
-        
-        * Many new documentation enhancements (thanks to @rhpvorderman, and others)
-        * rename of shed-install to shed-tools and add a new --latest and --revision argument (thanks to @rhpvorderman)
-        * many fixes and new tests by (thanks to @mvdbeek)
-        * Parallelization of run-data-managers (thanks to @rhpvorderman)
-        * ephemeris will now use https by default instead of http (thanks to @bgruening)
-        
-        ---------------------
-        0.7.0 (2017-06-27)
-        ---------------------
-        
-        * Many new documentation enhancements (thanks to @rhpvorderman, @erasche, and others) -
-          docs are now published to https://readthedocs.org/projects/ephemeris/.
-        * Fix problem with empty list options related to running data managers (thanks to @rhpvorderman).
-        * Enable data managers to run with API keys (thanks to @rhpvorderman).
-        * Add sleep command to wait for a Galaxy API to become available (thanks to @erasche).
-        * Preserve readable order of keys while processing tool lists (thanks to @drosofff).
-        
-        ---------------------
-        0.6.1 (2017-04-17)
-        ---------------------
-        
-        * Add Python 2 and 3 testing for all scripts against galaxy-docker-stable along with various
-          refactoring to reduce code duplication and Python 3 fixes. `#36
-          <https://github.com/galaxyproject/ephemeris/pull/36>`__
-        
-        ---------------------
-        0.6.0 (2017-04-10)
-        ---------------------
-        
-        * Add new connection options for setting up data libraries.
-        
-        ---------------------
-        0.5.1 (2017-04-07)
-        ---------------------
-        
-        * Fix new ``run-data-managers`` CLI entrypoint.
-        
-        ---------------------
-        0.5.0 (2017-04-06)
-        ---------------------
-        
-        * Add ``run-data-managers`` tool to trigger DM with multiple values and in order. `#30 <https://github.com/galaxyproject/ephemeris/pull/30>`_
-        * The workflow install tool now supports a directory of workflows. `#27 <https://github.com/galaxyproject/ephemeris/pull/27>`_
-        * enable global options in a tool yaml files, like `install_resolver_dependencies: true` `#26 <https://github.com/galaxyproject/ephemeris/pull/26>`_
-        * Mention mimum required galaxy versions. `#23 <https://github.com/galaxyproject/ephemeris/pull/23>`_ (thanks to @mvdbeek)
-            
-        
-        ---------------------
-        0.4.0 (2016-09-07)
-        ---------------------
-        
-        * Be more generic in determining a server time-out (thanks to @afgane).
-        * Get tool list entrypoint and improvements (thanks to @mvdbeek).
-        * Rename ``tool_panel_section_name`` to ``tool_panel_section_label`` like
-          ansible-galaxy-tools (thanks to @nturaga).
-        * Add missing file ``tool_list.yaml.sample`` (thanks to @nturaga).
-        
-        ---------------------
-        0.3.0 (2016-08-26)
-        ---------------------
-        
-        * More robust shed-install script, install dependencies by default, improve logging
-          (thanks to @mvdbeek).
-        
-        ---------------------
-        0.2.0 (2016-08-15)
-        ---------------------
-        
-        * Add tool generate a tool list from a Galaxy workflow file
-          (thanks to @drosofff).
-        * Fix various code quality issues including adding beta support
-          for Python 3 (thanks in part to @mvdbeek).
-        
-        ---------------------
-        0.1.0 (2016-06-15)
-        ---------------------
-        
-        * Setup project, pull in scripts from `ansible-galaxy-tools
-          <https://github.com/galaxyproject/ansible-galaxy-tools>`__
-          and adapt them for usage as a library.
-        
-        .. _bioblend: https://github.com/galaxyproject/bioblend/
-        .. _nose: https://nose.readthedocs.org/en/latest/
-        
-Keywords: galaxy
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+.. :changelog:
+
+History
+-------
+
+.. to_doc
+
+---------------------
+0.9.0 (2018-05-23)
+---------------------
+
+* Update data managers when updating tools (thanks to `@rhpvorderman`_).
+  `Pull Request 78`_, `Issue 69`_
+* Run data managers aggressive parallelization and refactoring (thanks to
+  `@rhpvorderman`_).
+  `Pull Request 79`_
+* Makes publishing of imported workflows available (thanks to `@pcm32`_).
+  `Pull Request 74`_
+* Add option to test tools on update/install for Galaxy 18.05 (thanks to `@jmchilton`_).
+  `Pull Request 81`_
+* Upload 2.0 support for data library creation (thanks to `@jmchilton`_).
+  `Pull Request 89`_
+* Fixes to revision parsing in tools.yaml (thanks to `@bgruening`_).
+  `Pull Request 70`_
+* Add Codacy monitoring and badge (thanks to `@jmchilton`_).
+  `Pull Request 73`_
+* Fix typo in project organization document (thanks to `@blankenberg`_).
+  `Pull Request 86`_
+* Fix hardcoded log paths (thanks to `@rhpvorderman`_).
+  `Pull Request 85`_
+* Fix ``shed-tools`` update argparse handling (thanks to `@rhpvorderman`_).
+  `Pull Request 88`_
+* Fix a few lint issues (thanks to `@jmchilton`_).
+  `Pull Request 90`_
+
+---------------------
+0.8.0 (2017-12-29)
+---------------------
+
+* Many new documentation enhancements (thanks to @rhpvorderman, and others)
+* rename of shed-install to shed-tools and add a new --latest and --revision argument (thanks to @rhpvorderman)
+* many fixes and new tests by (thanks to @mvdbeek)
+* Parallelization of run-data-managers (thanks to @rhpvorderman)
+* run-data-managers now uses more advanced templating for less repetitive input yamls (thanks to @rhpvorderman)
+* run-data-managers now checks if a genome index is already present before running the data manager (thanks to @rhpvorderman)
+* ephemeris will now use https by default instead of http (thanks to @bgruening)
+
+---------------------
+0.7.0 (2017-06-27)
+---------------------
+
+* Many new documentation enhancements (thanks to @rhpvorderman, @erasche, and others) -
+  docs are now published to https://readthedocs.org/projects/ephemeris/.
+* Fix problem with empty list options related to running data managers (thanks to @rhpvorderman).
+* Enable data managers to run with API keys (thanks to @rhpvorderman).
+* Add sleep command to wait for a Galaxy API to become available (thanks to @erasche).
+* Preserve readable order of keys while processing tool lists (thanks to @drosofff).
+
+---------------------
+0.6.1 (2017-04-17)
+---------------------
+
+* Add Python 2 and 3 testing for all scripts against galaxy-docker-stable along with various
+  refactoring to reduce code duplication and Python 3 fixes. `#36
+  <https://github.com/galaxyproject/ephemeris/pull/36>`__
+
+---------------------
+0.6.0 (2017-04-10)
+---------------------
+
+* Add new connection options for setting up data libraries.
+
+---------------------
+0.5.1 (2017-04-07)
+---------------------
+
+* Fix new ``run-data-managers`` CLI entrypoint.
+
+---------------------
+0.5.0 (2017-04-06)
+---------------------
+
+* Add ``run-data-managers`` tool to trigger DM with multiple values and in order. `#30 <https://github.com/galaxyproject/ephemeris/pull/30>`_
+* The workflow install tool now supports a directory of workflows. `#27 <https://github.com/galaxyproject/ephemeris/pull/27>`_
+* enable global options in a tool yaml files, like `install_resolver_dependencies: true` `#26 <https://github.com/galaxyproject/ephemeris/pull/26>`_
+* Mention mimum required galaxy versions. `#23 <https://github.com/galaxyproject/ephemeris/pull/23>`_ (thanks to @mvdbeek)
+    
+
+---------------------
+0.4.0 (2016-09-07)
+---------------------
+
+* Be more generic in determining a server time-out (thanks to @afgane).
+* Get tool list entrypoint and improvements (thanks to @mvdbeek).
+* Rename ``tool_panel_section_name`` to ``tool_panel_section_label`` like
+  ansible-galaxy-tools (thanks to @nturaga).
+* Add missing file ``tool_list.yaml.sample`` (thanks to @nturaga).
+
+---------------------
+0.3.0 (2016-08-26)
+---------------------
+
+* More robust shed-install script, install dependencies by default, improve logging
+  (thanks to @mvdbeek).
+
+---------------------
+0.2.0 (2016-08-15)
+---------------------
+
+* Add tool generate a tool list from a Galaxy workflow file
+  (thanks to @drosofff).
+* Fix various code quality issues including adding beta support
+  for Python 3 (thanks in part to @mvdbeek).
+
+---------------------
+0.1.0 (2016-06-15)
+---------------------
+
+* Setup project, pull in scripts from `ansible-galaxy-tools
+  <https://github.com/galaxyproject/ansible-galaxy-tools>`__
+  and adapt them for usage as a library.
+
+.. github_links
+.. _Pull Request 74: https://github.com/galaxyproject/ephemeris/pull/74
+.. _Issue 69: https://github.com/galaxyproject/ephemeris/issues/69
+.. _Pull Request 73: https://github.com/galaxyproject/ephemeris/pull/73
+.. _Pull Request 78: https://github.com/galaxyproject/ephemeris/pull/78
+.. _Pull Request 70: https://github.com/galaxyproject/ephemeris/pull/70
+.. _Pull Request 86: https://github.com/galaxyproject/ephemeris/pull/86
+.. _Pull Request 79: https://github.com/galaxyproject/ephemeris/pull/79
+.. _Pull Request 85: https://github.com/galaxyproject/ephemeris/pull/85
+.. _Pull Request 81: https://github.com/galaxyproject/ephemeris/pull/81
+.. _Pull Request 90: https://github.com/galaxyproject/ephemeris/pull/90
+.. _Pull Request 89: https://github.com/galaxyproject/ephemeris/pull/89
+.. _Pull Request 88: https://github.com/galaxyproject/ephemeris/pull/88
+.. _@bgruening: https://github.com/bgruening
+.. _@blankenberg: https://github.com/blankenberg
+.. _@rhpvorderman: https://github.com/rhpvorderman
+.. _@pcm32: https://github.com/pcm32
+.. _@jmchilton: https://github.com/jmchilton
+
+.. _bioblend: https://github.com/galaxyproject/bioblend/
+.. _nose: https://nose.readthedocs.org/en/latest/
```

### Comparing `ephemeris-0.8.0/ephemeris.egg-info/SOURCES.txt` & `ephemeris-0.9.0/ephemeris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephemeris-0.8.0/LICENSE` & `ephemeris-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ephemeris-0.8.0/setup.py` & `ephemeris-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ephemeris-0.8.0/CONTRIBUTING.rst` & `ephemeris-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ephemeris-0.8.0/CODE_OF_CONDUCT.rst` & `ephemeris-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `ephemeris-0.8.0/README.rst` & `ephemeris-0.9.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 .. image:: https://travis-ci.org/galaxyproject/ephemeris.png?branch=master
    :target: https://travis-ci.org/galaxyproject/ephemeris
 
 .. image:: https://coveralls.io/repos/galaxyproject/ephemeris/badge.svg?branch=master
    :target: https://coveralls.io/r/galaxyproject/ephemeris?branch=master
 
+.. image:: https://api.codacy.com/project/badge/Grade/73873ffd3ff04c46a0c5ee75b37bb5bb
+   :target: https://www.codacy.com/app/jmchilton/ephemeris?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=galaxyproject/ephemeris&amp;utm_campaign=Badge_Grade
+
 Ephemeris is a small Python library and set of scripts for managing the
 bootstrapping of Galaxy_ plugins - tools, index data, and workflows.
 
 * Free software: Academic Free License version 3.0
 * Documentation: https://ephemeris.readthedocs.org.
 * Code: https://github.com/galaxyproject/ephemeris
```

