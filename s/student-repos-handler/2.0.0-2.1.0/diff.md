# Comparing `tmp/student-repos-handler-2.0.0.tar.gz` & `tmp/student-repos-handler-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "student-repos-handler-2.0.0.tar", last modified: Tue Apr 18 00:10:21 2023, max compression
+gzip compressed data, was "student-repos-handler-2.1.0.tar", last modified: Tue Apr 18 00:49:02 2023, max compression
```

## Comparing `student-repos-handler-2.0.0.tar` & `student-repos-handler-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2023-04-18 00:10:21.395319 student-repos-handler-2.0.0/
--rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2023-04-18 00:10:21.395319 student-repos-handler-2.0.0/PKG-INFO
--rw-r--r--   0 fisa      (1000) fisa      (1000)      256 2020-09-12 01:06:10.000000 student-repos-handler-2.0.0/README.md
--rwxr-xr-x   0 fisa      (1000) fisa      (1000)    17815 2023-04-18 00:07:07.000000 student-repos-handler-2.0.0/repos.py
--rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2023-04-18 00:10:21.395319 student-repos-handler-2.0.0/setup.cfg
--rw-rw-r--   0 fisa      (1000) fisa      (1000)      910 2023-04-18 00:09:34.000000 student-repos-handler-2.0.0/setup.py
-drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2023-04-18 00:10:21.395319 student-repos-handler-2.0.0/student_repos_handler.egg-info/
--rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/PKG-INFO
--rw-rw-r--   0 fisa      (1000) fisa      (1000)      299 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)        1 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/entry_points.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)       19 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/requires.txt
--rw-rw-r--   0 fisa      (1000) fisa      (1000)        6 2023-04-18 00:10:21.000000 student-repos-handler-2.0.0/student_repos_handler.egg-info/top_level.txt
+drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2023-04-18 00:49:02.209112 student-repos-handler-2.1.0/
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2023-04-18 00:49:02.209112 student-repos-handler-2.1.0/PKG-INFO
+-rw-r--r--   0 fisa      (1000) fisa      (1000)      256 2020-09-12 01:06:10.000000 student-repos-handler-2.1.0/README.md
+-rwxr-xr-x   0 fisa      (1000) fisa      (1000)    17960 2023-04-18 00:47:29.000000 student-repos-handler-2.1.0/repos.py
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2023-04-18 00:49:02.209112 student-repos-handler-2.1.0/setup.cfg
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)      910 2023-04-18 00:48:51.000000 student-repos-handler-2.1.0/setup.py
+drwxrwxr-x   0 fisa      (1000) fisa      (1000)        0 2023-04-18 00:49:02.209112 student-repos-handler-2.1.0/student_repos_handler.egg-info/
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)     1009 2023-04-18 00:49:02.000000 student-repos-handler-2.1.0/student_repos_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)      299 2023-04-18 00:49:02.000000 student-repos-handler-2.1.0/student_repos_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)        1 2023-04-18 00:49:02.000000 student-repos-handler-2.1.0/student_repos_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)       38 2023-04-18 00:49:02.000000 student-repos-handler-2.1.0/student_repos_handler.egg-info/entry_points.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)       19 2023-04-18 00:49:02.000000 student-repos-handler-2.1.0/student_repos_handler.egg-info/requires.txt
+-rw-rw-r--   0 fisa      (1000) fisa      (1000)        6 2023-04-18 00:49:02.000000 student-repos-handler-2.1.0/student_repos_handler.egg-info/top_level.txt
```

### Comparing `student-repos-handler-2.0.0/PKG-INFO` & `student-repos-handler-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: student-repos-handler
-Version: 2.0.0
+Version: 2.1.0
 Summary: Simple tool to handle multiple repos at once, oriented to the grading of assignments in UCSE DAR
 Home-page: https://github.com/fisadev/student-repos-handler
 Author: Juan Pedro Fisanotti
 Author-email: fisadev@gmail.com
 License: LICENSE.txt
 Description: # Student-repos-handler
```

### Comparing `student-repos-handler-2.0.0/repos.py` & `student-repos-handler-2.1.0/repos.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,120 +180,133 @@
 
     def long_description(self):
         """
         Repo details described in a human readable string.
         """
         return f"{self.alias}: {self.description} ({self.slug} at {self.service.value})"
 
-    def vcs_update(self, section):
+    def vcs_update_command(self, section):
         """
-        Update the cloned repo, or clone it if not present.
+        Command to update the cloned repo, or clone it if not present.
         """
-        repo_url = self.clone_url(section)
         repo_path = self.path(section)
 
         if repo_path.exists():
             if self.vcs == VCS.HG:
-                pull_command = "hg pull -u"
+                command = "hg pull -u"
             elif self.vcs == VCS.GIT:
-                pull_command = "git pull"
-
-            command = f"(cd {repo_path} && {pull_command})"
+                command = "git pull"
         else:
             if self.vcs == VCS.HG:
                 clone_command = "hg clone"
             elif self.vcs == VCS.GIT:
                 clone_command = "git clone"
 
-            command = f"{clone_command} {repo_url} {repo_path}"
+            command = f"{clone_command} {repo_path}"
 
-        result = system(command)
-        return result == 0
+        return command
 
-    def vcs_clean(self, section):
+    def vcs_clean_command(self, section):
         """
-        Clean changes done to the repo.
+        Command to clean changes done to the repo.
         """
-        repo_path = self.path(section)
-
         if self.vcs == VCS.HG:
-            clean_command = "hg revert --all --no-backup"
+            command = "hg revert --all --no-backup"
         elif self.vcs == VCS.GIT:
-            clean_command = "git checkout -- ."
+            command = "git checkout -- ."
 
-        command = f"(cd {repo_path} && {clean_command})"
-        result = system(command)
-        return result == 0
+        return command
 
-    def vcs_status(self, section):
+    def vcs_status_command(self, section):
         """
-        Show the status of the repo.
+        Command to show the status of the repo.
         """
-        repo_path = self.path(section)
-
         if self.vcs == VCS.HG:
-            status_command = "hg status"
+            command = "hg status"
         elif self.vcs == VCS.GIT:
-            status_command = "git status"
+            command = "git status"
 
-        command = f"(cd {repo_path} && {status_command})"
-        result = system(command)
-        return result == 0
+        return command
 
     def open_vcs_file(self, section, editor, file_, any_extension=False):
         """
         Find and open a specified file from the repo.
         """
-        file_path = self.path(section) / file_
+        repo_path = self.path(section)
+        file_path = repo_path / file_
         possible_files = []
 
         if any_extension:
             parent_dir = file_path.parent
 
             if parent_dir.exists():
                 possible_files = list(parent_dir.glob(f"{file_}.*"))
         else:
             if file_path.exists():
                 possible_files = [file_path]
 
         if len(possible_files) == 1:
-            system(f"{editor} {possible_files[0]}")
-            return True, possible_files
+            winner_relative_path = possible_files[0].relative_to(repo_path)
+            command = f"{editor} {winner_relative_path}"
+            success = self.run(command, section)
+            return success, possible_files
         else:
             return False, possible_files
 
     def navigate_wiki(self, browser, url):
         """
         Open a browser to a specific page of the wiki.
         """
         full_url = f"{self.web_url(Section.WIKI)}/{url}"
-        system(f"{browser} {full_url}")
+        return self.run(f"{browser} {full_url}")
 
     def navigate_server(self, browser):
         """
         Open a browser to the web server running the code.
         """
-        system(f"{browser} {self.server}")
+        return self.run(f"{browser} {self.server}")
 
     def revive_server(self):
         """
         Do a background request to the server running the code, so it wakes up if it was put to
         sleep.
         """
         response = requests.get(self.server)
         response.raise_for_status()
 
-    def run(self, command):
+    def run(self, command, section=Section.CODE):
         """
         Run a command inside the repo.
         """
-        repo_path = self.path(Section.CODE)
+        repo_path = self.path(section)
         putenv("REPO_PATH", repo_path)
+
+        Color.GOOD.print("Run:", command)
+        print()
+
         result = system(f"(cd {repo_path} && {command})")
-        return result
+        success = result == 0
+
+        print()
+        if success:
+            Color.GOOD.print("Done!")
+        else:
+            Color.BAD.print("Error running command")
+        print()
+
+        return success
+
+    def matches(self, filters):
+        """
+        Decide wether a filter applies to this repo.
+        """
+        filters = [f.lower() for f in filters]
+
+        long_description = self.long_description().lower()
+        return any(f in long_description for f in filters)
 
 
 class ReposHandler(object):
     """
     The app itself, exposing a set of actions that you can run over a set of repos.
     """
     def __init__(self, repos):
@@ -303,71 +316,65 @@
         """
         Obtain the list of repos that match a given filter.
         IF no filter is specified, then all repos are returned.
         """
         if not filters:
             filtered = self.repos
         else:
-            filters = [f.lower() for f in filters]
-
             filtered = [repo for repo in self.repos
-                        if any(f in repo.long_description().lower()
-                               for f in filters)]
+                        if repo.matches(filters)]
 
             if filtered:
                 Color.GOOD.print(len(filtered), "repos found")
-                print()
             else:
                 Color.BAD.print("No repos matching the filters")
 
         return filtered
 
     def iterate_filtered_repos(self, filters):
         """
         Iterate over the results of filter_repos, printing the title of the repo on each step.
         """
         repos = self.filter_repos(filters)
         for repo in repos:
+            print()
             Color.GOOD.print("<<<<", repo, ">>>>")
+            print()
             yield repo
 
     def vcs_action_in_repos(self, filters, vcs_action):
         """
         Run a vcs action in a set of filtered repos.
         """
         repos_ok = []
         repos_err = []
 
-        method_name = f"vcs_{vcs_action.value}"
+        method_name = f"vcs_{vcs_action.value}_command"
 
         for repo in self.iterate_filtered_repos(filters):
             code_ok = True
             wiki_ok = True
 
             if Section.CODE in repo.sections:
                 Color.GOOD.print("--- Code ---")
-                code_ok = getattr(repo, method_name)(Section.CODE)
+                code_command = getattr(repo, method_name)(Section.CODE)
 
-                if not code_ok:
-                    Color.BAD.print("Error running command")
+                code_ok = repo.run(code_command)
 
             if Section.WIKI in repo.sections:
                 Color.GOOD.print("--- Wiki ---")
-                wiki_ok = getattr(repo, method_name)(Section.WIKI)
+                wiki_command = getattr(repo, method_name)(Section.WIKI)
 
-                if not wiki_ok:
-                    Color.BAD.print("Error running command")
+                wiki_ok = repo.run(wiki_command)
 
             if code_ok and wiki_ok:
                 repos_ok.append(repo)
             else:
                 repos_err.append(repo)
 
-            print()
-
         self.summary_errors(repos_ok, repos_err)
 
     def update(self, *filters):
         """
         Do a vcs update over a set of filtered repos.
         """
         self.vcs_action_in_repos(filters, VCSAction.UPDATE)
@@ -424,34 +431,28 @@
                 repo.revive_server()
                 repos_ok.append(repo)
                 Color.GOOD.print("Done!")
             except:
                 repos_err.append(repo)
                 Color.BAD.print("Error:")
 
-            print()
-
         self.summary_errors(repos_ok, repos_err)
 
     def run(self, command, *filters):
         """
         Run a command inside the folders of a set of filtered repos.
         """
         repos_ok = []
         repos_err = []
         for repo in self.iterate_filtered_repos(filters):
-            result = repo.run(command)
-            if result == 0:
+            success = repo.run(command)
+            if success:
                 repos_ok.append(repo)
-                Color.GOOD.print("Done!")
             else:
                 repos_err.append(repo)
-                Color.BAD.print("Error running command")
-
-            print()
 
         self.summary_errors(repos_ok, repos_err)
 
     def open_vcs_file(self, section, editor, filters, file_, any_extension=False):
         """
         Open files of a set of filtered repos.
         """
@@ -468,16 +469,14 @@
 
                 if possible_files:
                     Color.BAD.print("Many files on the wiki with that name:")
                     print("\n".join(map(str, possible_files)))
                 else:
                     Color.BAD.print("File does not exists")
 
-            print()
-
         self.summary_errors(repos_ok, repos_err)
 
     def show(self, *filters):
         """
         Just show filtered repos info.
         """
         for repo in self.iterate_filtered_repos(filters):
@@ -488,16 +487,14 @@
             if Section.WIKI in repo.sections:
                 Color.GOOD.print("Wiki:", end=" ")
                 print(repo.web_url(Section.WIKI))
             if repo.server:
                 Color.GOOD.print("Server:", end=" ")
                 print(repo.server)
 
-            print()
-
     @classmethod
     def find_repos_config(cls, start_path):
         """
         Find the closest repos config file, navigating from the current dir backwards.
         """
         current_path = start_path
         while current_path:
@@ -528,65 +525,78 @@
         return ReposHandler(repos)
 
     @classmethod
     def summary_errors(cls, repos_ok, repos_err):
         """
         Show a summary of ok and errors from actions in a set of repos.
         """
+        print()
         if len(repos_ok) + len(repos_err) > 1:
             if repos_ok:
                 Color.GOOD.print("Success:", end=" ")
                 print(*repos_ok, sep=", ")
             if repos_err:
                 Color.BAD.print("Errors:", end=" ")
                 print(*repos_err, sep=", ")
+        print()
 
     @classmethod
-    def show_help(cls):
+    def help(cls):
         """
         Show the help message.
         """
+        print()
         Color.GOOD.print("Usage:")
+        print()
+        print("repos help")
         print("repos show FILTERS")
         print("repos status FILTERS")
         print("repos clean FILTERS")
         print("repos update FILTERS")
         print("repos code EDITOR FILE FILTERS")
         print("repos wiki EDITOR FILE FILTERS")
         print("repos wiki_web BROWSER URL FILTERS")
         print("repos server BROWSER FILTERS")
         print("repos revive_server BROWSER FILTERS")
         print("repos run \"COMMAND\" FILTERS")
+        print()
 
 
 def main():
     """
     When running from the command line, this is executed.
     """
     current_path = Path(".")
     config_path = ReposHandler.find_repos_config(current_path)
     if not config_path:
+        print()
         Color.BAD.print("Unable to find repos.config")
+        print()
         exit(1)
 
     handler = ReposHandler.parse_file(config_path, current_path)
 
     if len(sys.argv) < 2:
-        handler.show_help()
+        handler.help()
         exit()
 
     action = sys.argv[1]
     method = getattr(handler, action, None)
     if method is None:
+        print()
         Color.BAD.print("Unknown action:", action)
-        handler.show_help()
+
+        handler.help()
         exit(1)
 
     if method:
         try:
             method(*sys.argv[2:])
         except KeyboardInterrupt:
+            print()
             Color.BAD.print("Cancelled")
+            print()
+            exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `student-repos-handler-2.0.0/setup.py` & `student-repos-handler-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
     name='student-repos-handler',
-    version='2.0.0',
+    version='2.1.0',
     description='Simple tool to handle multiple repos at once, oriented to the grading of assignments in UCSE DAR',
     long_description=open('README.md').read(),
     author='Juan Pedro Fisanotti',
     author_email='fisadev@gmail.com',
     url='https://github.com/fisadev/student-repos-handler',
     license='LICENSE.txt',
     python_requires='>=3.4',
```

### Comparing `student-repos-handler-2.0.0/student_repos_handler.egg-info/PKG-INFO` & `student-repos-handler-2.1.0/student_repos_handler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: student-repos-handler
-Version: 2.0.0
+Version: 2.1.0
 Summary: Simple tool to handle multiple repos at once, oriented to the grading of assignments in UCSE DAR
 Home-page: https://github.com/fisadev/student-repos-handler
 Author: Juan Pedro Fisanotti
 Author-email: fisadev@gmail.com
 License: LICENSE.txt
 Description: # Student-repos-handler
```

