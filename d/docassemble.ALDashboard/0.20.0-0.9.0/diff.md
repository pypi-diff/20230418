# Comparing `tmp/docassemble.ALDashboard-0.20.0.tar.gz` & `tmp/docassemble.ALDashboard-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.ALDashboard-0.20.0.tar", last modified: Tue Apr 18 15:40:08 2023, max compression
+gzip compressed data, was "dist/docassemble.ALDashboard-0.9.0.tar", last modified: Tue Oct 26 18:13:40 2021, max compression
```

## Comparing `docassemble.ALDashboard-0.20.0.tar` & `docassemble.ALDashboard-0.9.0.tar`

### file list

```diff
@@ -1,52 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:40:08.985417 docassemble.ALDashboard-0.20.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-04-18 15:40:08.985417 docassemble.ALDashboard-0.20.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2399 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:40:08.981417 docassemble.ALDashboard-0.20.0/docassemble/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:40:08.981417 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8820 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/aldashboard.py
--rw-r--r--   0 runner    (1001) docker     (122)    10973 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/create_package.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:40:08.981417 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:40:08.985417 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/
--rw-r--r--   0 runner    (1001) docker     (122)     4253 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/compile_bootstrap.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1060 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/generate_translation.yml
--rw-r--r--   0 runner    (1001) docker     (122)    23542 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/install_assembly_line.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/install_packages.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/list_sessions.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3053 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/manage_users.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/menu.yml
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/nav.yml
--rw-r--r--   0 runner    (1001) docker     (122)     7514 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/package_scanner.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3617 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/pdf_wrangling.yml
--rw-r--r--   0 runner    (1001) docker     (122)     7673 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/review_screen_generator.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/update_packages.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1502 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/validate_attachment.yml
--rw-r--r--   0 runner    (1001) docker     (122)      961 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/validate_docx.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4402 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/validate_translation.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:40:08.985417 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:40:08.985417 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/static/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/static/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/static/al_dashboard.css
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/static/bootstrap.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:40:08.985417 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     7493 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/templates/pkg_scanner_report.docx
--rw-r--r--   0 runner    (1001) docker     (122)     7595 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/package_scanner.py
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)    21481 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3761 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/validate_docx.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/docassemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 15:40:08.981417 docassemble.ALDashboard-0.20.0/docassemble.ALDashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2524 2023-04-18 15:40:08.000000 docassemble.ALDashboard-0.20.0/docassemble.ALDashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2023-04-18 15:40:08.000000 docassemble.ALDashboard-0.20.0/docassemble.ALDashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 15:40:08.000000 docassemble.ALDashboard-0.20.0/docassemble.ALDashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-18 15:40:08.000000 docassemble.ALDashboard-0.20.0/docassemble.ALDashboard.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 15:40:08.000000 docassemble.ALDashboard-0.20.0/docassemble.ALDashboard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-18 15:40:08.000000 docassemble.ALDashboard-0.20.0/docassemble.ALDashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-18 15:40:08.000000 docassemble.ALDashboard-0.20.0/docassemble.ALDashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      988 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-18 15:40:08.985417 docassemble.ALDashboard-0.20.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4764 2023-04-18 15:39:57.000000 docassemble.ALDashboard-0.20.0/setup.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/
+-rw-r--r--   0 www-data    (33) www-data    (33)       18 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/MANIFEST.in
+-rw-r--r--   0 www-data    (33) www-data    (33)     2933 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)     2195 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.845167 docassemble.ALDashboard-0.9.0/docassemble/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/
+-rw-r--r--   0 www-data    (33) www-data    (33)       22 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/__init__.py
+-rw-r--r--   0 www-data    (33) www-data    (33)     4889 2021-10-26 16:03:52.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/aldashboard.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.845167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/
+-rw-r--r--   0 www-data    (33) www-data    (33)     2791 2021-10-26 15:39:12.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/install_assembly_line.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     2685 2021-10-26 15:01:33.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/install_packages.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     1563 2021-07-31 17:09:32.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/list_sessions.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     2542 2021-10-18 16:49:09.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/manage_users.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     1120 2021-10-26 15:37:24.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/menu.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)      143 2021-07-31 17:13:17.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/nav.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     2087 2021-10-26 15:01:33.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/update_packages.yml
+-rw-r--r--   0 www-data    (33) www-data    (33)     4402 2021-07-31 17:11:53.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/validate_translation.yml
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/sources/
+-rw-r--r--   0 www-data    (33) www-data    (33)      134 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/sources/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/static/
+-rw-r--r--   0 www-data    (33) www-data    (33)      105 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/static/README.md
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/templates/
+-rw-r--r--   0 www-data    (33) www-data    (33)      102 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/templates/README.md
+-rw-r--r--   0 www-data    (33) www-data    (33)      155 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble/__init__.py
+drwxr-xr-x   0 www-data    (33) www-data    (33)        0 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/
+-rw-r--r--   0 www-data    (33) www-data    (33)     2933 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/PKG-INFO
+-rw-r--r--   0 www-data    (33) www-data    (33)     1027 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/namespace_packages.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)        1 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/not-zip-safe
+-rw-r--r--   0 www-data    (33) www-data    (33)       12 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/top_level.txt
+-rw-r--r--   0 www-data    (33) www-data    (33)       79 2021-10-26 18:13:40.849167 docassemble.ALDashboard-0.9.0/setup.cfg
+-rw-r--r--   0 www-data    (33) www-data    (33)     4667 2021-10-26 18:13:40.000000 docassemble.ALDashboard-0.9.0/setup.py
```

### Comparing `docassemble.ALDashboard-0.20.0/README.md` & `docassemble.ALDashboard-0.9.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# ALDashboard: a docassemble Admin and Configuration Tool
-
-[![PyPI version](https://badge.fury.io/py/docassemble.ALDashboard.svg)](https://badge.fury.io/py/docassemble.ALDashboard)
+# Backend Configuration Tool
 
 A single pane of glass that centralizes some tedious Docassemble admin configuration tasks
 
 ![image](https://user-images.githubusercontent.com/7645641/123702117-bdd7d300-d830-11eb-8c0e-8e204d912ff8.png)
 
+Done: 
+
 1. Install the Document Assembly Line packages (support files for [Court Forms Online](https://courtformsonline.org))
 1. Searchable user management - reset passwords and change privileges.
 1. Installing or updating several packages at once.
 1. Listing and viewing the contents of an (unencrypted) interview to facilitate debugging errors on production servers.
 1. View analytics/stats captured with store_variable_snapshot.
-1. List the files inside a particular package installed on the server.
-1. Gather files from a user who left the organization/unknown username and password.
-1. Review screen generator
-1. validate DOCX Jinja2 templates
 
-Ideas:
+
+TODO:
+
+1. List the files inside a particular package installed on the server.
 1. Add a link to the dispatch directive for an existing file in an existing package.
 1. Generating translation files [TBD].
+1. Gather files from a user who left the organization/unknown username and password.
 
 To use, you must create a docassemble API key and add it to your
 configuration, like this:
 
 `install packages api key: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`
 
 ## Some screenshots
```

### Comparing `docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/install_packages.yml` & `docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/install_packages.yml`

 * *Files 24% similar despite different names*

```diff
@@ -2,87 +2,101 @@
   title: Bulk Package Install
   sessions are unique: True
   required privileges:
     - admin
     - developer
   temporary session: True
 ---
-modules:
-  - .aldashboard
----
 objects:
+  - daREST: DAWeb.using(base_url=get_config('url root',"https://" + get_config('external hostname',"")) + "/api" )
   - packages: DAList.using(object_type=DAObject, there_are_any=True, complete_attribute="github_url")
 ---
+code: |
+  install_packages_api_key = get_config('install packages api key')
+---
 mandatory: True
 id: interview order
 code: |
+  if not install_packages_api_key:
+    exit_no_api_key
   packages.gather()
   if install_packages_task.ready():
     ending_screen
   else:
     waiting_screen
 ---
+event: exit_no_api_key
+question: |
+  Please add an API key!
+subquestion: |
+  This interview requires an API key to work.
+  
+  You can create an API key by going to your profile. Please
+  create an API key with either IP restrictions or no restrictions.
+  
+  Then add it to the [configuration file](${ url_of('config') }) like this:
+  
+  ```
+  install packages api key: x7123aG...
+  ```
+---
 question: |
   What packages do you want to install?
 list collect: True
 fields:
   - Github URL: packages[i].github_url
   - YAML filename: packages[i].yaml_name
   - Short name or alias (no spaces): packages[i].alias
-    validate: |
-      lambda y: y.isidentifier()
 ---
 code: |
   install_packages_task = background_action('install_packages_event')
 ---
 event: install_packages_event
 code: |
-  background_error_action("bg_failure")
   for package in packages:
-    pkgname = install_from_github_url(package.github_url)
-    reset(pkgname)
-
-  the_config = da_get_config()
-  if not the_config.get("dispatch"):
-    the_config["dispatch"] = {}
-  for package in packages:
-      package_regex = r"https:\/\/github\.com\/.*\/docassemble-([\w]*)"
-      match = re.search(package_regex, package.github_url)
-      if match:
-        package_path = f"docassemble.{ match.groups()[0] }:data/questions/{ package.yaml_name }"
-        the_config["dispatch"][package.alias] = package_path
-  results = da_write_config(the_config)
-
-  background_response_action("bg_success")
----
-event: bg_success
-code: |
-  it_worked = True
+    data = {"key": install_packages_api_key,
+            "github_url": package.github_url
+            }
+    # This won't persist after backround task completes
+    package.status = daREST.post("package",data=data)
   background_response()
 ---  
 event: waiting_screen
 question: |
-  Wait here while we start the installation process
-reload: True
+  Wait here
+reload: True  
 ---
-event: bg_failure
 code: |
-  it_worked = False
-  background_response()
+  dispatch_temp = ""
+  for package in packages:
+    package_regex = r"https:\/\/github\.com\/.*\/docassemble-([\w]*)"
+    match = re.search(package_regex, package.github_url)
+    if match:
+      dispatch_temp += '  "' + package.alias + '": '  
+      package_name = "docassemble." + match.groups()[0]
+      dispatch_temp += '"' + package_name + ':data/questions/' + package.yaml_name + '"'
+      dispatch_temp += "\n"
+  dispatch_directive = dispatch_temp
+  del dispatch_temp
+  del match
 ---
 event: ending_screen
 question: |
   All done
 subquestion: |
-  % if it_worked:
-  It may take a few minutes for the installation process to complete.
-
-  You can now use these links to reach your interviews:
+  Copy the dispatch directive below into the right place in the 
+  configuration file.
+  
+  
+  ${ indent(dispatch_directive) }
+  
+  
+  IOnce you install the dispatch directive, you can use these
+  links to reach your interviews:
   
+  Alias | Link
+  ------|--------
   % for package in packages:
-  * [${package.alias}](/start/${package.alias})
+  ${ package.alias } | [${package.alias}](/start/${package.alias})
   % endfor
-  % else:
-  Something went wrong. Check the [worker.log](/logs?file=worker.log) to learn what.
-  % endif
 buttons:
   - Restart: restart
```

### Comparing `docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/list_sessions.yml` & `docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/list_sessions.yml`

 * *Files 6% similar despite different names*

```diff
@@ -35,17 +35,17 @@
 mandatory: True
 event: load_answer
 question: |
   Recently generated sessions for ${ filename }
 subquestion: |
   
   % for interview in sessions_list:
-  * <a href="${ interview_url(i=interview.filename, session=interview.key) }">
-      ${ interviews.get(interview.filename,{'title': interview.filename}).get('title') }
+  * <a href="${ interview_url(i=interview['filename'], session=interview['key']) }">
+      ${ interviews.get(interview['filename'],{'title': interview['filename']}).get('title') }
     </a>
-    (Modified ${ format_date(interview.modtime) }), on page **${ interview.num_keys }**
-      * [View variables](${ interview_url_action('view_session_variables', session_id=interview.key) })
+    (Modified ${ format_date(interview['modtime']) }), on page **${ interview['num_keys'] }**
+      * [View variables](${ interview_url_action('view_session_variables', session_id=interview['key']) })
   % endfor
 ---
 event: view_session_variables
 code: |
-  json_response(get_session_variables(filename, action_argument('session_id'), simplify=True))
+  json_response(get_session_variables(filename, action_argument('session_id'),  simplify=True))
```

#### html2text {}

```diff
@@ -6,14 +6,14 @@
 code: | [{interview: interviews[interview].get('title')} for interview in
 interviews] - User (leave blank to view all sessions): chosen_user required:
 False datatype: integer input type: combobox code: | speedy_get_users() --- #
 next((item.get('title') for item in interviews if item.get('filename') ==
 interview['filename']), interview['filename'] ) --- code: | sessions_list =
 speedy_get_sessions(user_id=chosen_user, filename=filename) --- mandatory: True
 event: load_answer question: | Recently generated sessions for ${ filename }
-subquestion: | % for interview in sessions_list: * ${_interviews.get
-(interview.filename,{'title':_interview.filename}).get('title')_} (Modified $
-{ format_date(interview.modtime) }), on page **${ interview.num_keys }** *
-[View variables](${ interview_url_action('view_session_variables',
-session_id=interview.key) }) % endfor --- event: view_session_variables code: |
-json_response(get_session_variables(filename, action_argument('session_id'),
-simplify=True))
+subquestion: | % for interview in sessions_list: * ${_interviews.get(interview
+['filename'],{'title':_interview['filename']}).get('title')_} (Modified $
+{ format_date(interview['modtime']) }), on page **${ interview['num_keys'] }**
+* [View variables](${ interview_url_action('view_session_variables',
+session_id=interview['key']) }) % endfor --- event: view_session_variables
+code: | json_response(get_session_variables(filename, action_argument
+('session_id'), simplify=True))
```

### Comparing `docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/manage_users.yml` & `docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/manage_users.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,51 +7,43 @@
   sessions are unique: True
   required privileges:
     - admin
   temporary session: True
 ---
 modules:
   - .aldashboard
-  - .create_package
 ---
 mandatory: True
 id: interview order
 code: |
   chosen_user
   if user_task == 'reset_password':
     do_update_password
   elif user_task == 'elevate_permissions':
     do_update_privileges
-  elif user_task == 'download_playground':
-    do_download_playground
   ending_screen    
 ---
-code: |
-  user_lookup = {}
-  for user in get_users_and_name():
-    user_lookup[user[0]] = user[3]
----
 id: select user
 question: |
   Manage users
 fields:
   - User: chosen_user
     datatype: integer
     input type: combobox
     code: |
-      [{user[0]: f"{user[1]} {user[2]} {user[3]}"} for user in get_users_and_name()]
+      [{user[0]: f"{user['first_name']} {user['last_name']} {user['email']}"} for user in get_users_and_name()]      
     exclude:
       - "2"
     # User ID 2 is the "cron" user and should not be managed here        
   - What do you want to do?: user_task
     datatype: radio
     choices:
       - Reset password: reset_password
-      - Download playground files: download_playground
-      - Change user permissions: elevate_permissions      
+      # - Download playground files: download_playground
+      - Change user permissions: elevate_permissions
   - New password: new_user_password
     datatype: password
     show if:
       variable: user_task
       is: reset_password
     validate: valid_password      
   - Verify new password: new_user_password_2
@@ -80,23 +72,14 @@
   set_user_info(user_id=chosen_user, password=new_user_password)
   do_update_password = True
 ---
 code: |
   set_user_info(user_id=chosen_user, privileges=new_permission_level.true_values().elements )
   do_update_privileges = True
 ---
-id: download playground
-question: |
-  Playground download for ${ user_lookup[chosen_user] }
-subquestion: |
-  % for project in get_list_of_projects(chosen_user) + ['default']:
-  [${project}]( ${ create_user_playground_zip(chosen_user, space_to_underscore(user_lookup[chosen_user]), project).url_for() })
-  % endfor
-event: do_download_playground
----
 code: |
   def valid_password(pword):
     if not re.match(r"^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)[a-zA-Z\d]{6,}$", pword):
       validation_error(word("Password must have at least 6 characters with one lowercase letter, one uppercase letter and one number"))
     return True      
 ---
 event: ending_screen
```

### Comparing `docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/update_packages.yml` & `docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/update_packages.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,80 @@
 ---
 include:
   - nav.yml
 ---
-modules:
-  - .aldashboard  
----
 metadata:
   title: Bulk Package Update
   sessions are unique: True
   required privileges:
     - admin
     - developer
   temporary session: True
 ---
 objects:
+  - daREST: DAWeb.using(base_url=get_config('url root',"https://" + get_config('external hostname',"")) + "/api" )
   - packages: DAList.using(object_type=DAObject, there_are_any=True, complete_attribute="package_name")
 ---
 code: |
-  installed_packages = get_package_info()
+  installed_packages = daREST.get('package',{"key": install_packages_api_key })
+---
+code: |
+  install_packages_api_key = get_config('install packages api key')
 ---
 mandatory: True
 id: interview order
 code: |
+  if not install_packages_api_key:
+    exit_no_api_key
   packages.gather()
   if install_packages_task.ready():
     ending_screen
   else:
     waiting_screen
 ---
+event: exit_no_api_key
+question: |
+  Please add an API key!
+subquestion: |
+  This interview requires an API key to work.
+  
+  You can create an API key by going to your profile. Please
+  create an API key with either IP restrictions or no restrictions.
+  
+  Then add it to the [configuration file](${ url_of('config') }) like this:
+  
+  ```
+  install packages api key: x7123aG...
+  ```
+---
 question: |
   What packages do you want to update?
 fields:
   - no label: packages
     required: False
     datatype: checkboxes
     code: |
-      [
-        package.package.name
-        for package in installed_packages[0]
-        if (
-          package.package.name.startswith("docassemble")
-          and package.can_update
-          and package.package.name not in ["docassemble", "docassemble-backports", "docassemble.webapp", "docassemble-textstat", "docassemblekvsession"]
-        )
-      ]
+      [[package.get('name'),f"{package.get('name','')} ({package.get('version')})",True] for package in installed_packages if 'docassemble.' in package.get('name') and package.get('name') not in ['docassemble.demo','docassemble.webapp','docassemble.base']]
 ---
 code: |
   install_packages_task = background_action('install_packages_event')
 ---
 event: install_packages_event
 code: |
-  background_error_action("bg_failure")
-  for package in installed_packages[0]:
-    if package.package.name in packages.true_values():
-      if package.package.type and package.package.type == "git":
-        pkgname = install_from_github_url(package.package.giturl)
-        reset(pkgname)
-      elif package.package.type and package.package.type == "pip":
-        install_from_pypi(package.package.name)
-  background_response_action("bg_success")
----
-event: bg_success
-code: |
-  it_worked = True
+  for package in packages:
+    data = {"key": install_packages_api_key,
+            "update": package
+            }
+    # This won't persist after backround task completes
+    package.status = daREST.post("package",data=data)
   background_response()
 ---  
 event: waiting_screen
 question: |
-  Wait here while we start the installation process
+  Wait here
 reload: True
 ---
-event: bg_failure
-code: |
-  it_worked = False
-  background_response()
----
 event: ending_screen
 question: |
-  Your packages are installing
-subquestion: |
-  % if it_worked:
-  Check the log file to monitor progress. It may still take a few more minutes
-  for the installation process to complete.
-  % else:
-  Something went wrong. Check the [worker.log](/logs?file=worker.log) to learn what.
-  % endif
+  All done
 buttons:
   - Restart: restart
```

### Comparing `docassemble.ALDashboard-0.20.0/docassemble/ALDashboard/data/questions/validate_translation.yml` & `docassemble.ALDashboard-0.9.0/docassemble/ALDashboard/data/questions/validate_translation.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALDashboard-0.20.0/docassemble.ALDashboard.egg-info/SOURCES.txt` & `docassemble.ALDashboard-0.9.0/docassemble.ALDashboard.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,24 @@
-LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 docassemble/__init__.py
 docassemble.ALDashboard.egg-info/PKG-INFO
 docassemble.ALDashboard.egg-info/SOURCES.txt
 docassemble.ALDashboard.egg-info/dependency_links.txt
 docassemble.ALDashboard.egg-info/namespace_packages.txt
 docassemble.ALDashboard.egg-info/not-zip-safe
-docassemble.ALDashboard.egg-info/requires.txt
 docassemble.ALDashboard.egg-info/top_level.txt
 docassemble/ALDashboard/__init__.py
 docassemble/ALDashboard/aldashboard.py
-docassemble/ALDashboard/create_package.py
-docassemble/ALDashboard/package_scanner.py
-docassemble/ALDashboard/requirements.txt
-docassemble/ALDashboard/translation.py
-docassemble/ALDashboard/validate_docx.py
-docassemble/ALDashboard/data/questions/compile_bootstrap.yml
-docassemble/ALDashboard/data/questions/generate_translation.yml
 docassemble/ALDashboard/data/questions/install_assembly_line.yml
 docassemble/ALDashboard/data/questions/install_packages.yml
 docassemble/ALDashboard/data/questions/list_sessions.yml
 docassemble/ALDashboard/data/questions/manage_users.yml
 docassemble/ALDashboard/data/questions/menu.yml
 docassemble/ALDashboard/data/questions/nav.yml
-docassemble/ALDashboard/data/questions/package_scanner.yml
-docassemble/ALDashboard/data/questions/pdf_wrangling.yml
-docassemble/ALDashboard/data/questions/review_screen_generator.yml
 docassemble/ALDashboard/data/questions/update_packages.yml
-docassemble/ALDashboard/data/questions/validate_attachment.yml
-docassemble/ALDashboard/data/questions/validate_docx.yml
 docassemble/ALDashboard/data/questions/validate_translation.yml
 docassemble/ALDashboard/data/sources/README.md
 docassemble/ALDashboard/data/static/README.md
-docassemble/ALDashboard/data/static/al_dashboard.css
-docassemble/ALDashboard/data/static/bootstrap.svg
-docassemble/ALDashboard/data/templates/README.md
-docassemble/ALDashboard/data/templates/pkg_scanner_report.docx
+docassemble/ALDashboard/data/templates/README.md
```

### Comparing `docassemble.ALDashboard-0.20.0/setup.py` & `docassemble.ALDashboard-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import sys
 from setuptools import setup, find_packages
 from fnmatch import fnmatchcase
 from distutils.util import convert_path
 
 standard_exclude = ('*.pyc', '*~', '.*', '*.bak', '*.swp*')
 standard_exclude_directories = ('.*', 'CVS', '_darcs', './build', './dist', 'EGG-INFO', '*.egg-info')
-
 def find_package_data(where='.', package='', exclude=standard_exclude, exclude_directories=standard_exclude_directories):
     out = {}
     stack = [(convert_path(where), '', package)]
     while stack:
         where, prefix, package = stack.pop(0)
         for name in os.listdir(where):
             fn = os.path.join(where, name)
@@ -40,22 +39,22 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.ALDashboard',
-      version='0.20.0',
+      version='0.9.0',
       description=('Dashboard for some admin tasks'),
-      long_description='# Backend Configuration Tool\r\n\r\nA single pane of glass that centralizes some tedious Docassemble admin configuration tasks\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702117-bdd7d300-d830-11eb-8c0e-8e204d912ff8.png)\r\n\r\n1. Install the Document Assembly Line packages (support files for [Court Forms Online](https://courtformsonline.org))\r\n1. Searchable user management - reset passwords and change privileges.\r\n1. Installing or updating several packages at once.\r\n1. Listing and viewing the contents of an (unencrypted) interview to facilitate debugging errors on production servers.\r\n1. View analytics/stats captured with store_variable_snapshot.\r\n1. List the files inside a particular package installed on the server.\r\n1. Gather files from a user who left the organization/unknown username and password.\r\n1. Review screen generator\r\n1. validate DOCX Jinja2 templates\r\n\r\nIdeas:\r\n1. Add a link to the dispatch directive for an existing file in an existing package.\r\n1. Generating translation files [TBD].\r\n\r\nTo use, you must create a docassemble API key and add it to your\r\nconfiguration, like this:\r\n\r\n`install packages api key: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`\r\n\r\n## Some screenshots\r\n\r\n### Main page\r\n![image](https://user-images.githubusercontent.com/7645641/123702117-bdd7d300-d830-11eb-8c0e-8e204d912ff8.png)\r\n\r\n### Manage users\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702231-e069ec00-d830-11eb-94dc-5ec0abb86bc9.png)\r\n\r\n### Bulk install packages from GitHub\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702290-efe93500-d830-11eb-9fdf-a5935ff4078e.png)\r\n\r\n### Bulk update packages\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702362-068f8c00-d831-11eb-9ce4-df7a67ffcfeb.png)\r\n\r\n### View / search sessions by user and interview name\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702422-1d35e300-d831-11eb-84d5-5e7385deb901.png)\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702464-2cb52c00-d831-11eb-80fc-f2291e824eae.png)\r\n\r\n### View interview stats captured with `store_variables_snapshot()`\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702623-5e2df780-d831-11eb-8937-6625df74ab22.png)\r\n\r\n',
+      long_description='# Backend Configuration Tool\r\n\r\nA single pane of glass that centralizes some tedious Docassemble admin configuration tasks\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702117-bdd7d300-d830-11eb-8c0e-8e204d912ff8.png)\r\n\r\nDone: \r\n\r\n1. Install the Document Assembly Line packages (support files for [Court Forms Online](https://courtformsonline.org))\r\n1. Searchable user management - reset passwords and change privileges.\r\n1. Installing or updating several packages at once.\r\n1. Listing and viewing the contents of an (unencrypted) interview to facilitate debugging errors on production servers.\r\n1. View analytics/stats captured with store_variable_snapshot.\r\n\r\n\r\nTODO:\r\n\r\n1. List the files inside a particular package installed on the server.\r\n1. Add a link to the dispatch directive for an existing file in an existing package.\r\n1. Generating translation files [TBD].\r\n1. Gather files from a user who left the organization/unknown username and password.\r\n\r\nTo use, you must create a docassemble API key and add it to your\r\nconfiguration, like this:\r\n\r\n`install packages api key: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`\r\n\r\n## Some screenshots\r\n\r\n### Main page\r\n![image](https://user-images.githubusercontent.com/7645641/123702117-bdd7d300-d830-11eb-8c0e-8e204d912ff8.png)\r\n\r\n### Manage users\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702231-e069ec00-d830-11eb-94dc-5ec0abb86bc9.png)\r\n\r\n### Bulk install packages from GitHub\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702290-efe93500-d830-11eb-9fdf-a5935ff4078e.png)\r\n\r\n### Bulk update packages\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702362-068f8c00-d831-11eb-9ce4-df7a67ffcfeb.png)\r\n\r\n### View / search sessions by user and interview name\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702422-1d35e300-d831-11eb-84d5-5e7385deb901.png)\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702464-2cb52c00-d831-11eb-80fc-f2291e824eae.png)\r\n\r\n### View interview stats captured with `store_variables_snapshot()`\r\n\r\n![image](https://user-images.githubusercontent.com/7645641/123702623-5e2df780-d831-11eb-8937-6625df74ab22.png)\r\n\r\n',
       long_description_content_type='text/markdown',
       author='Quinten Steenhuis',
       author_email='qsteenhuis@gmail.com',
       license='The MIT License (MIT)',
-      url='https://github.com/SuffolkLITLab/docassemble-ALDashboard',
+      url='https://docassemble.org',
       packages=find_packages(),
       namespace_packages=['docassemble'],
-      install_requires=['PyGithub>=1.55'],
+      install_requires=[],
       zip_safe=False,
       package_data=find_package_data(where='docassemble/ALDashboard/', package='docassemble.ALDashboard'),
      )
```

