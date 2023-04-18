# Comparing `tmp/botsh-0.1.3.tar.gz` & `tmp/botsh-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botsh-0.1.3.tar", last modified: Mon Apr 10 16:06:21 2023, max compression
+gzip compressed data, was "botsh-0.1.4.tar", last modified: Tue Apr 18 16:17:00 2023, max compression
```

## Comparing `botsh-0.1.3.tar` & `botsh-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 16:06:21.516873 botsh-0.1.3/
--rw-r--r--   0 paulbutler   (501) staff       (20)       54 2023-04-10 14:28:50.000000 botsh-0.1.3/MANIFEST.in
--rw-r--r--   0 paulbutler   (501) staff       (20)     3791 2023-04-10 16:06:21.516674 botsh-0.1.3/PKG-INFO
--rw-r--r--   0 paulbutler   (501) staff       (20)      234 2023-04-10 14:12:58.000000 botsh-0.1.3/Pipfile
--rw-r--r--   0 paulbutler   (501) staff       (20)    64876 2023-04-10 14:13:02.000000 botsh-0.1.3/Pipfile.lock
--rw-r--r--   0 paulbutler   (501) staff       (20)     3152 2023-04-10 16:05:16.000000 botsh-0.1.3/README.md
--rw-r--r--   0 paulbutler   (501) staff       (20)       38 2023-04-10 16:06:21.516914 botsh-0.1.3/setup.cfg
--rw-r--r--   0 paulbutler   (501) staff       (20)     1597 2023-04-10 16:05:22.000000 botsh-0.1.3/setup.py
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 16:06:21.512266 botsh-0.1.3/src/
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 16:06:21.515121 botsh-0.1.3/src/botsh/
--rw-r--r--   0 paulbutler   (501) staff       (20)        0 2023-04-10 09:30:05.000000 botsh-0.1.3/src/botsh/__init__.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     3264 2023-04-10 14:41:08.000000 botsh-0.1.3/src/botsh/docker_exec.py
--rw-r--r--   0 paulbutler   (501) staff       (20)      317 2023-04-10 11:28:56.000000 botsh-0.1.3/src/botsh/history.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     1479 2023-04-10 13:40:08.000000 botsh-0.1.3/src/botsh/llm.py
--rw-r--r--   0 paulbutler   (501) staff       (20)       46 2023-04-10 12:14:03.000000 botsh-0.1.3/src/botsh/logging.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     2718 2023-04-10 14:39:56.000000 botsh-0.1.3/src/botsh/main.py
--rw-r--r--   0 paulbutler   (501) staff       (20)      972 2023-04-10 12:28:06.000000 botsh-0.1.3/src/botsh/prompt.py
--rw-r--r--   0 paulbutler   (501) staff       (20)     2164 2023-04-10 13:51:16.000000 botsh-0.1.3/src/botsh/task_driver.py
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 16:06:21.516315 botsh-0.1.3/src/botsh/templates/
--rw-r--r--   0 paulbutler   (501) staff       (20)     1099 2023-04-10 13:51:54.000000 botsh-0.1.3/src/botsh/templates/prompt.jinja2
-drwxr-xr-x   0 paulbutler   (501) staff       (20)        0 2023-04-10 16:06:21.516125 botsh-0.1.3/src/botsh.egg-info/
--rw-r--r--   0 paulbutler   (501) staff       (20)     3791 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/PKG-INFO
--rw-r--r--   0 paulbutler   (501) staff       (20)      454 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/SOURCES.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)        1 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/dependency_links.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)       42 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/entry_points.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)      881 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/requires.txt
--rw-r--r--   0 paulbutler   (501) staff       (20)        6 2023-04-10 16:06:21.000000 botsh-0.1.3/src/botsh.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:17:00.504965 botsh-0.1.4/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1074 2023-04-18 14:41:00.000000 botsh-0.1.4/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-04-18 14:41:00.000000 botsh-0.1.4/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4562 2023-04-18 16:17:00.504965 botsh-0.1.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      234 2023-04-18 14:41:00.000000 botsh-0.1.4/Pipfile
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    64876 2023-04-18 14:41:00.000000 botsh-0.1.4/Pipfile.lock
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3901 2023-04-18 14:41:00.000000 botsh-0.1.4/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-18 16:17:00.504965 botsh-0.1.4/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1597 2023-04-18 15:23:31.000000 botsh-0.1.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:17:00.500965 botsh-0.1.4/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:17:00.500965 botsh-0.1.4/src/botsh/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-18 14:41:00.000000 botsh-0.1.4/src/botsh/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3601 2023-04-18 15:21:53.000000 botsh-0.1.4/src/botsh/docker_exec.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      317 2023-04-18 14:41:00.000000 botsh-0.1.4/src/botsh/history.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1479 2023-04-18 14:41:00.000000 botsh-0.1.4/src/botsh/llm.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       46 2023-04-18 14:41:00.000000 botsh-0.1.4/src/botsh/logging.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2718 2023-04-18 14:41:00.000000 botsh-0.1.4/src/botsh/main.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1196 2023-04-18 16:16:16.000000 botsh-0.1.4/src/botsh/prompt.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2189 2023-04-18 15:01:04.000000 botsh-0.1.4/src/botsh/task_driver.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:17:00.504965 botsh-0.1.4/src/botsh/templates/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1099 2023-04-18 14:41:00.000000 botsh-0.1.4/src/botsh/templates/prompt.jinja2
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-18 16:17:00.504965 botsh-0.1.4/src/botsh.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4562 2023-04-18 16:17:00.000000 botsh-0.1.4/src/botsh.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      462 2023-04-18 16:17:00.000000 botsh-0.1.4/src/botsh.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-18 16:17:00.000000 botsh-0.1.4/src/botsh.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-04-18 16:17:00.000000 botsh-0.1.4/src/botsh.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      881 2023-04-18 16:17:00.000000 botsh-0.1.4/src/botsh.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-04-18 16:17:00.000000 botsh-0.1.4/src/botsh.egg-info/top_level.txt
```

### Comparing `botsh-0.1.3/PKG-INFO` & `botsh-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,21 @@
-Metadata-Version: 2.1
-Name: botsh
-Version: 0.1.3
-Summary: A task runner powered by OpenAI and Docker.
-Home-page: https://github.com/drifting-in-space/botsh
-Author: Paul Butler
-Author-email: paul@driftingin.space
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # `botsh`
 
 [![PyPI version](https://badge.fury.io/py/botsh.svg)](https://badge.fury.io/py/botsh)
 
-`botsh` is a task runner powered by OpenAI and Docker.
+`botsh` attaches a chat agent to a Docker container running Ubuntu.
 
-Invoke botsh by providing a task as a command line argument.
+This effectively gives the agent access to the entire [Apt](https://wiki.debian.org/Apt)
+universe, while limiting its blast radius to the current directory.
 
-botsh will create a bare Ubuntu Docker container associated with
-the current directory, or create one if one does not exist. botsh
-will then attach the OpenAI API to a shell running in the container
-to attempt to complete the given task.
+## Demo
 
-The AI is explicitly told that it is allowed to install software,
-and will typically install programs as needed to complete its task.
-Installed software remains confined to the container.
+This demo uses the prompt `create a sequence of 100 200x200 images which each contain a different number, and turn them into a 30fps video with ffmpeg`.
+
+https://user-images.githubusercontent.com/46173/230953506-c8545345-c0a1-46b1-b937-458191fc2456.mp4
 
 ## Setup
 
 Install with:
 
     pip install botsh
 
@@ -48,22 +28,37 @@
 
     # botsh "convert cat.jpg into a png file"
 
     # botsh "use a remote service to find my public ip and base64 encode it"
 
     # botsh "run pylint on the codebase in src/"
 
+## Additional details
+
+`botsh` will create a bare Ubuntu Docker container associated with
+the current directory, or create one if one does not exist. botsh
+will then attach the OpenAI API to a shell running in the container
+to attempt to complete the given task.
+
+The AI is explicitly told that it is allowed to install software,
+and will typically install programs as needed to complete its task.
+Installed software remains confined to the container.
+
 ## Observations
 
 These observations relate to the default model, `text-davinci-003`. Using GPT-4 may improve things.
 
 - It works best if you explicitly specify the files/paths you want to work with (use relative references).
   It is not good at figuring out what you mean.
 - It often gets stuck in loops if it can't complete a task rather than giving up, despite the prompt
   telling it not to.
+- It sometimes needs subtle encouragement to break a task down into multiple parts, instead of chaining together
+  a long shell command, particularly when the command it wants to run has a bug. For example, instead of
+  saying “convert foo.png to a gif and compute its md5 sum”, try “convert foo.png into a gif, and then compute
+  its md5 sum”
 
 ## Container re-use
 
 When `botsh` is invoked, the current working directory is mounted
 into the container and can be modified by programs the agent runs.
 The filesystem outside of the current working directory is sealed
 off from the container.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `botsh-0.1.3/Pipfile.lock` & `botsh-0.1.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `botsh-0.1.3/README.md` & `botsh-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,40 @@
+Metadata-Version: 2.1
+Name: botsh
+Version: 0.1.4
+Summary: A task runner powered by OpenAI and Docker.
+Home-page: https://github.com/drifting-in-space/botsh
+Author: Paul Butler
+Author-email: paul@driftingin.space
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # `botsh`
 
 [![PyPI version](https://badge.fury.io/py/botsh.svg)](https://badge.fury.io/py/botsh)
 
-`botsh` is a task runner powered by OpenAI and Docker.
+`botsh` attaches a chat agent to a Docker container running Ubuntu.
 
-Invoke botsh by providing a task as a command line argument.
+This effectively gives the agent access to the entire [Apt](https://wiki.debian.org/Apt)
+universe, while limiting its blast radius to the current directory.
 
-botsh will create a bare Ubuntu Docker container associated with
-the current directory, or create one if one does not exist. botsh
-will then attach the OpenAI API to a shell running in the container
-to attempt to complete the given task.
+## Demo
 
-The AI is explicitly told that it is allowed to install software,
-and will typically install programs as needed to complete its task.
-Installed software remains confined to the container.
+This demo uses the prompt `create a sequence of 100 200x200 images which each contain a different number, and turn them into a 30fps video with ffmpeg`.
+
+https://user-images.githubusercontent.com/46173/230953506-c8545345-c0a1-46b1-b937-458191fc2456.mp4
 
 ## Setup
 
 Install with:
 
     pip install botsh
 
@@ -30,22 +47,37 @@
 
     # botsh "convert cat.jpg into a png file"
 
     # botsh "use a remote service to find my public ip and base64 encode it"
 
     # botsh "run pylint on the codebase in src/"
 
+## Additional details
+
+`botsh` will create a bare Ubuntu Docker container associated with
+the current directory, or create one if one does not exist. botsh
+will then attach the OpenAI API to a shell running in the container
+to attempt to complete the given task.
+
+The AI is explicitly told that it is allowed to install software,
+and will typically install programs as needed to complete its task.
+Installed software remains confined to the container.
+
 ## Observations
 
 These observations relate to the default model, `text-davinci-003`. Using GPT-4 may improve things.
 
 - It works best if you explicitly specify the files/paths you want to work with (use relative references).
   It is not good at figuring out what you mean.
 - It often gets stuck in loops if it can't complete a task rather than giving up, despite the prompt
   telling it not to.
+- It sometimes needs subtle encouragement to break a task down into multiple parts, instead of chaining together
+  a long shell command, particularly when the command it wants to run has a bug. For example, instead of
+  saying “convert foo.png to a gif and compute its md5 sum”, try “convert foo.png into a gif, and then compute
+  its md5 sum”
 
 ## Container re-use
 
 When `botsh` is invoked, the current working directory is mounted
 into the container and can be modified by programs the agent runs.
 The filesystem outside of the current working directory is sealed
 off from the container.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `botsh-0.1.3/setup.py` & `botsh-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         f"{pkg_name}{pkg_info['version']}"
         for pkg_name, pkg_info in pipfile_lock[mode].items()
     ]
 
 
 setup(
     name="botsh",
-    version="0.1.3",
+    version="0.1.4",
     description="A task runner powered by OpenAI and Docker.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Paul Butler",
     author_email="paul@driftingin.space",
     url="https://github.com/drifting-in-space/botsh",
     packages=find_packages("src"),
```

### Comparing `botsh-0.1.3/src/botsh/docker_exec.py` & `botsh-0.1.4/src/botsh/docker_exec.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,24 @@
         self.remove_on_exit = remove_on_exit
         self.current_directory = os.getcwd()
         self.shell_command = shell_command
         dir_hash = hashlib.sha256(self.current_directory.encode("utf-8")).hexdigest()
         container_name = f"botsh-{dir_hash}"
 
         log.info("Connecting to Docker...")
-        self.client = docker.from_env()
+        try:
+           self.client = docker.from_env()
+        except Exception as e:
+           log.error(
+                "Permission error connecting to Docker. "
+                "Is Docker running? "
+                "You may need to follow these instructions: "
+                "https://docs.docker.com/engine/install/linux-postinstall/.",
+           )
+           exit(1)
 
         self._get_container(container_name, image, wipe)
 
     def _get_mounts(self) -> list[Mount]:
         mount = Mount(target="/work", source=self.current_directory, type="bind")
 
         return [mount]
```

### Comparing `botsh-0.1.3/src/botsh/llm.py` & `botsh-0.1.4/src/botsh/llm.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.3/src/botsh/main.py` & `botsh-0.1.4/src/botsh/main.py`

 * *Files identical despite different names*

### Comparing `botsh-0.1.3/src/botsh/task_driver.py` & `botsh-0.1.4/src/botsh/task_driver.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,31 +36,34 @@
         self.history.append(CommandExecution(explanation, command, output, exit_code))
         return output
 
     def step(self):
         response = self.llm.completion(self.task, self.history)
 
         result = parse_response(response)
-        command = result.get("COMMAND", "")
-        explanation = result.get("EXPLANATION", "")
 
-        if command == "":
+        if result.command == "":
             log.info(
-                "Agent indicated that the task is complete.", explanation=explanation
+                "Agent indicated that the task is complete.",
+                explanation=result.explanation,
             )
             return True
         else:
             log.info(
-                "Agent requested a command.", command=command, explanation=explanation
+                "Agent requested a command.",
+                command=result.command,
+                explanation=result.explanation,
             )
 
-        exit_code, output = self.container.run_command(command)
+        exit_code, output = self.container.run_command(result.command)
         lines = output.splitlines()
         if len(lines) > 10:
             truncated = len(lines) - 10
             result = (
                 f"[ {truncated} lines truncated ]"
                 + "\n".join(lines[-10:])
                 + "\n[...]\n"
             )
 
-        self.history.append(CommandExecution(explanation, command, output, exit_code))
+        self.history.append(
+            CommandExecution(result.explanation, result.command, output, exit_code)
+        )
```

### Comparing `botsh-0.1.3/src/botsh/templates/prompt.jinja2` & `botsh-0.1.4/src/botsh/templates/prompt.jinja2`

 * *Files identical despite different names*

### Comparing `botsh-0.1.3/src/botsh.egg-info/PKG-INFO` & `botsh-0.1.4/src/botsh.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: botsh
-Version: 0.1.3
+Version: 0.1.4
 Summary: A task runner powered by OpenAI and Docker.
 Home-page: https://github.com/drifting-in-space/botsh
 Author: Paul Butler
 Author-email: paul@driftingin.space
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
 
 # `botsh`
 
 [![PyPI version](https://badge.fury.io/py/botsh.svg)](https://badge.fury.io/py/botsh)
 
-`botsh` is a task runner powered by OpenAI and Docker.
+`botsh` attaches a chat agent to a Docker container running Ubuntu.
 
-Invoke botsh by providing a task as a command line argument.
+This effectively gives the agent access to the entire [Apt](https://wiki.debian.org/Apt)
+universe, while limiting its blast radius to the current directory.
 
-botsh will create a bare Ubuntu Docker container associated with
-the current directory, or create one if one does not exist. botsh
-will then attach the OpenAI API to a shell running in the container
-to attempt to complete the given task.
+## Demo
 
-The AI is explicitly told that it is allowed to install software,
-and will typically install programs as needed to complete its task.
-Installed software remains confined to the container.
+This demo uses the prompt `create a sequence of 100 200x200 images which each contain a different number, and turn them into a 30fps video with ffmpeg`.
+
+https://user-images.githubusercontent.com/46173/230953506-c8545345-c0a1-46b1-b937-458191fc2456.mp4
 
 ## Setup
 
 Install with:
 
     pip install botsh
 
@@ -48,22 +47,37 @@
 
     # botsh "convert cat.jpg into a png file"
 
     # botsh "use a remote service to find my public ip and base64 encode it"
 
     # botsh "run pylint on the codebase in src/"
 
+## Additional details
+
+`botsh` will create a bare Ubuntu Docker container associated with
+the current directory, or create one if one does not exist. botsh
+will then attach the OpenAI API to a shell running in the container
+to attempt to complete the given task.
+
+The AI is explicitly told that it is allowed to install software,
+and will typically install programs as needed to complete its task.
+Installed software remains confined to the container.
+
 ## Observations
 
 These observations relate to the default model, `text-davinci-003`. Using GPT-4 may improve things.
 
 - It works best if you explicitly specify the files/paths you want to work with (use relative references).
   It is not good at figuring out what you mean.
 - It often gets stuck in loops if it can't complete a task rather than giving up, despite the prompt
   telling it not to.
+- It sometimes needs subtle encouragement to break a task down into multiple parts, instead of chaining together
+  a long shell command, particularly when the command it wants to run has a bug. For example, instead of
+  saying “convert foo.png to a gif and compute its md5 sum”, try “convert foo.png into a gif, and then compute
+  its md5 sum”
 
 ## Container re-use
 
 When `botsh` is invoked, the current working directory is mounted
 into the container and can be modified by programs the agent runs.
 The filesystem outside of the current working directory is sealed
 off from the container.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `botsh-0.1.3/src/botsh.egg-info/requires.txt` & `botsh-0.1.4/src/botsh.egg-info/requires.txt`

 * *Files identical despite different names*

