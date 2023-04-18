# Comparing `tmp/imit-1.0.9.tar.gz` & `tmp/imit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imit-1.0.9.tar", last modified: Fri Nov 27 04:33:57 2020, max compression
+gzip compressed data, was "imit-1.1.0.tar", last modified: Tue Apr 18 08:03:59 2023, max compression
```

## Comparing `imit-1.0.9.tar` & `imit-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 leytou     (501) staff       (20)        0 2020-11-27 04:33:57.899216 imit-1.0.9/
--rw-r--r--   0 leytou     (501) staff       (20)      401 2020-11-27 04:33:57.898569 imit-1.0.9/PKG-INFO
--rw-r--r--   0 leytou     (501) staff       (20)       66 2020-07-15 09:57:20.000000 imit-1.0.9/README.md
-drwxr-xr-x   0 leytou     (501) staff       (20)        0 2020-11-27 04:33:57.889763 imit-1.0.9/imit.egg-info/
--rw-r--r--   0 leytou     (501) staff       (20)      401 2020-11-27 04:33:57.000000 imit-1.0.9/imit.egg-info/PKG-INFO
--rw-r--r--   0 leytou     (501) staff       (20)      374 2020-11-27 04:33:57.000000 imit-1.0.9/imit.egg-info/SOURCES.txt
--rw-r--r--   0 leytou     (501) staff       (20)        1 2020-11-27 04:33:57.000000 imit-1.0.9/imit.egg-info/dependency_links.txt
--rw-r--r--   0 leytou     (501) staff       (20)       40 2020-11-27 04:33:57.000000 imit-1.0.9/imit.egg-info/entry_points.txt
--rw-r--r--   0 leytou     (501) staff       (20)        1 2020-11-27 04:33:57.000000 imit-1.0.9/imit.egg-info/not-zip-safe
--rw-r--r--   0 leytou     (501) staff       (20)       37 2020-11-27 04:33:57.000000 imit-1.0.9/imit.egg-info/requires.txt
--rw-r--r--   0 leytou     (501) staff       (20)        4 2020-11-27 04:33:57.000000 imit-1.0.9/imit.egg-info/top_level.txt
--rw-r--r--   0 leytou     (501) staff       (20)       38 2020-11-27 04:33:57.899314 imit-1.0.9/setup.cfg
--rwxr-xr-x   0 leytou     (501) staff       (20)      811 2020-11-27 04:33:32.000000 imit-1.0.9/setup.py
-drwxr-xr-x   0 leytou     (501) staff       (20)        0 2020-11-27 04:33:57.897544 imit-1.0.9/src/
--rw-r--r--   0 leytou     (501) staff       (20)        0 2020-08-05 06:32:56.000000 imit-1.0.9/src/__init__.py
--rw-r--r--   0 leytou     (501) staff       (20)     4279 2020-08-05 06:33:18.000000 imit-1.0.9/src/commit_inquirer.py
--rw-r--r--   0 leytou     (501) staff       (20)      778 2020-09-18 01:21:40.000000 imit-1.0.9/src/config.py
--rw-r--r--   0 leytou     (501) staff       (20)      520 2020-08-05 06:32:56.000000 imit-1.0.9/src/des.py
--rw-r--r--   0 leytou     (501) staff       (20)     2040 2020-09-18 01:29:03.000000 imit-1.0.9/src/git_handler.py
--rwxr-xr-x   0 leytou     (501) staff       (20)     3467 2020-11-27 04:28:32.000000 imit-1.0.9/src/imit.py
--rw-r--r--   0 leytou     (501) staff       (20)     1497 2020-11-05 02:09:56.000000 imit-1.0.9/src/jira_issues.py
--rw-r--r--   0 leytou     (501) staff       (20)     2140 2020-11-27 04:19:05.000000 imit-1.0.9/src/option_handler.py
--rw-r--r--   0 leytou     (501) staff       (20)     1953 2020-08-05 06:32:56.000000 imit-1.0.9/src/version_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:03:59.959975 imit-1.1.0/
+-rw-rw-rw-   0        0        0     1063 2023-04-18 02:21:11.000000 imit-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      407 2023-04-18 08:03:59.959975 imit-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2023-04-18 02:21:11.000000 imit-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 08:03:59.955973 imit-1.1.0/imit.egg-info/
+-rw-rw-rw-   0        0        0      407 2023-04-18 08:03:59.000000 imit-1.1.0/imit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-04-18 08:03:59.000000 imit-1.1.0/imit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:03:59.000000 imit-1.1.0/imit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-18 08:03:59.000000 imit-1.1.0/imit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 08:03:59.000000 imit-1.1.0/imit.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       37 2023-04-18 08:03:59.000000 imit-1.1.0/imit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-18 08:03:59.000000 imit-1.1.0/imit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 08:03:59.959975 imit-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      811 2023-04-18 08:03:04.000000 imit-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:03:59.958976 imit-1.1.0/src/
+-rw-rw-rw-   0        0        0        0 2023-04-18 02:21:11.000000 imit-1.1.0/src/__init__.py
+-rw-rw-rw-   0        0        0     4309 2023-04-18 07:37:58.000000 imit-1.1.0/src/commit_inquirer.py
+-rw-rw-rw-   0        0        0      796 2023-04-18 02:21:11.000000 imit-1.1.0/src/config.py
+-rw-rw-rw-   0        0        0      520 2023-04-18 02:21:11.000000 imit-1.1.0/src/des.py
+-rw-rw-rw-   0        0        0     2098 2023-04-18 07:38:31.000000 imit-1.1.0/src/git_handler.py
+-rw-rw-rw-   0        0        0     3401 2023-04-18 07:33:21.000000 imit-1.1.0/src/imit.py
+-rw-rw-rw-   0        0        0     1497 2023-04-18 02:21:11.000000 imit-1.1.0/src/jira_issues.py
+-rw-rw-rw-   0        0        0     2184 2023-04-18 07:31:13.000000 imit-1.1.0/src/option_handler.py
+-rw-rw-rw-   0        0        0     5043 2023-04-18 07:55:05.000000 imit-1.1.0/src/version_handler.py
```

### Comparing `imit-1.0.9/setup.py` & `imit-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='imit',
-    version="1.0.9",
+    version="1.1.0",
     description="提供交互或命令行的形式规范地提交git commit",
     long_description="""提供交互或命令行的形式规范地提交git commit""",
     keywords='python commit git',
     author='leytou',
     author_email='hi_litao@163.com',
     url='https://github.com/leytou',
     license='MIT',
```

### Comparing `imit-1.0.9/src/commit_inquirer.py` & `imit-1.1.0/src/commit_inquirer.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,25 +26,26 @@
                              carousel=True
                              )
     return inquirer.prompt([question])
 
 
 def QVersion(tags, commit_type, version_file_path):
     tags_index_tagged = []
-    nums = list(version_handler.TagNumDict(version_file_path).values())
+    version_processor = version_handler.VersionProcessor()
+    nums = list(version_processor.TagNumDict().values())
     index = 0
     for tag in tags:
         tag += '\t(%d) ' % nums[index]
         index += 1
         tags_index_tagged.append((tag, index))
-    print(tags_index_tagged)
-    current_version = version_handler.CurrentVersion(version_file_path)
+    # print(tags_index_tagged)
+    current_version = version_processor.CurrentVersion()
 
     index = -1
-    if commit_type == 'feature' or commit_type == 'refactor' :
+    if commit_type == 'feature' or commit_type == 'refactor':
         index = -2
 
     question = inquirer.List('version_index',
                              message='请选择要增加的版本号(当前: %s)' % current_version,
                              choices=tags_index_tagged,
                              carousel=True,
                              default=tags_index_tagged[index][1]
```

### Comparing `imit-1.0.9/src/config.py` & `imit-1.1.0/src/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     config = configparser.RawConfigParser()
     if os.path.exists(config_path):
         config.read(config_path, encoding="utf-8")
     if group not in config.sections():
         config.add_section(group)
 
     config.set(group, key, value)
-    with open(config_path, 'w') as configfile:
+    with open(config_path, 'w', encoding="utf-8") as configfile:
         config.write(configfile)
 
 
 def Get(key):
     config = configparser.RawConfigParser()
     if not os.path.exists(config_path):
         return ''
```

### Comparing `imit-1.0.9/src/des.py` & `imit-1.1.0/src/des.py`

 * *Files identical despite different names*

### Comparing `imit-1.0.9/src/git_handler.py` & `imit-1.1.0/src/git_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,16 +72,17 @@
 
 def UnstaedFiles():
     cmd = ['git', 'diff', '--name-only']
     return _ChangedFiles(cmd)
 
 
 def Handle(commit_option, version_file_path):
-    version_str_updated = version_handler.Handle(
-        commit_option['version_index'], version_file_path)
+    version_processor = version_handler.VersionProcessor()
+    version_str_updated = version_processor.IncreaseVersionAndSave(
+        commit_option['version_index'])
 
     msg_tags = [commit_option['commit_type'],
                 version_str_updated, commit_option['jira_id']]
     commit_msg = _GenerateCommitMsg(msg_tags, commit_option['commit_msg'])
     logging.debug('commit msg: ' + commit_msg)
 
     _Add(version_file_path)
```

### Comparing `imit-1.0.9/src/imit.py` & `imit-1.1.0/src/imit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Usage:
-    imit.py [-m|-b|-f|-R|-r] [-1|-2|-3|-4] [-M <msg>|<msg>] [-h|--help] [--log_level=<log_level>]
     imit.py config
+    imit.py [-m|-b|-f|-R|-r] [-1|-2|-3|-4] [-M <msg>|<msg>] [-h|--help] [--log_level=<log_level>]
 
 Options:
     -h,--help                   show usage
     -m                          set commit type: modify
     -b                          set commit type: bugfix
     -f                          set commit type: feature
     -R                          set commit type: refactor
@@ -30,14 +30,16 @@
 
 sys.path.append(os.path.dirname(os.path.realpath(__file__)))  # noqa
 import des
 import config
 import git_handler
 import option_handler
 import commit_inquirer
+import version_handler
+import fnmatch
 from pprint import pprint
 
 
 def InitLogger(args):
     log_level = args["--log_level"]
     if log_level is None:
 
@@ -56,30 +58,26 @@
     option_handler.UpdateOptionFromArgs(commit_option, args, commit_types)
     option_handler.UpdateOptionFromInquirer(
         commit_option, version_file_path, commit_types)
 
     return commit_option
 
 
-def EnvCheck(version_file_path):
+def EnvCheck():
     if sys.version_info < (3, 7):  # 3.7后dict默认为有序
         print('Please run imit with greater than python3.7.')
         exit(-1)
 
     git_root_path = git_handler.GetGitRootPath(os.getcwd())
     if not git_root_path:
         print('Please run imit in the git project path.')
         exit(-1)
 
     os.chdir(git_root_path)
 
-    if not os.path.exists(version_file_path):
-        print('File %s not found in current path.' % version_file_path)
-        exit(-1)
-
     if not git_handler.StagedFiles():
         print('No staged file, exit commit.')
         exit(-1)
 
 
 def Config():
     answer = commit_inquirer.QUsernamePassword()
@@ -91,27 +89,28 @@
 
 def main():
     commit_types = {'-m': 'modify',
                     '-b': 'bugfix',
                     '-f': 'feature',
                     '-R': 'refactor',
                     '-r': 'revert', }
-    version_file_path = 'version.properties'
 
     args = docopt.docopt(__doc__)
     InitLogger(args)
     logging.debug(args)
 
     if args['config']:
         Config()
         print('Username and password are encrypted and stored in file ~/.imitrc.ini')
         exit(0)
 
-    EnvCheck(version_file_path)
+    EnvCheck()
 
+    version_processor = version_handler.VersionProcessor()
+    version_file_path = version_processor.file_path
     commit_option = GetCommitOption(args, commit_types, version_file_path)
     logging.debug('commit option: ' + str(commit_option))
 
     git_handler.Handle(commit_option, version_file_path)
 
 
 if __name__ == "__main__":
```

### Comparing `imit-1.0.9/src/jira_issues.py` & `imit-1.1.0/src/jira_issues.py`

 * *Files identical despite different names*

### Comparing `imit-1.0.9/src/option_handler.py` & `imit-1.1.0/src/option_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     if commit_msg and 'commit_msg' not in commit_option:
         commit_option['commit_msg'] = commit_msg
 
     logging.debug('option from args: ' + str(commit_option))
 
 
 def UpdateOptionFromInquirer(commit_option, version_file_path, commit_types):
-    version_dict = version_handler.TagNumDict(version_file_path)
+    version_processor = version_handler.VersionProcessor()
+    version_dict = version_processor.TagNumDict()
     logging.debug('tag num dict: ' + str(version_dict))
 
     if 'commit_type' not in commit_option:
         answer = commit_inquirer.QType(list(commit_types.values()))
         commit_option.update(answer)
         logging.debug('option : '+str(answer))
```

