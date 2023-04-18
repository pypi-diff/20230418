# Comparing `tmp/autocog-0.0.1.tar.gz` & `tmp/autocog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocog-0.0.1.tar", last modified: Tue Apr 18 20:00:03 2023, max compression
+gzip compressed data, was "autocog-0.0.2.tar", last modified: Tue Apr 18 20:04:19 2023, max compression
```

## Comparing `autocog-0.0.1.tar` & `autocog-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:00:03.593343 autocog-0.0.1/
--rw-r--r--   0 andreas    (501) staff       (20)       24 2023-04-18 15:13:54.000000 autocog-0.0.1/.gitignore
--rw-r--r--   0 andreas    (501) staff       (20)     1176 2023-04-18 20:00:03.593204 autocog-0.0.1/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)     1084 2023-04-18 16:19:54.000000 autocog-0.0.1/README.md
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:00:03.570783 autocog-0.0.1/autocog/
--rw-r--r--   0 andreas    (501) staff       (20)    17526 2023-04-18 15:13:54.000000 autocog-0.0.1/autocog/autocog.py
-drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:00:03.593029 autocog-0.0.1/autocog.egg-info/
--rw-r--r--   0 andreas    (501) staff       (20)     1176 2023-04-18 20:00:03.000000 autocog-0.0.1/autocog.egg-info/PKG-INFO
--rw-r--r--   0 andreas    (501) staff       (20)      236 2023-04-18 20:00:03.000000 autocog-0.0.1/autocog.egg-info/SOURCES.txt
--rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-18 20:00:03.000000 autocog-0.0.1/autocog.egg-info/dependency_links.txt
--rw-r--r--   0 andreas    (501) staff       (20)       52 2023-04-18 20:00:03.000000 autocog-0.0.1/autocog.egg-info/entry_points.txt
--rw-r--r--   0 andreas    (501) staff       (20)       20 2023-04-18 20:00:03.000000 autocog-0.0.1/autocog.egg-info/requires.txt
--rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-18 20:00:03.000000 autocog-0.0.1/autocog.egg-info/top_level.txt
--rw-r--r--   0 andreas    (501) staff       (20)       38 2023-04-18 20:00:03.593382 autocog-0.0.1/setup.cfg
--rw-r--r--   0 andreas    (501) staff       (20)      540 2023-04-18 19:59:14.000000 autocog-0.0.1/setup.py
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:04:19.795281 autocog-0.0.2/
+-rw-r--r--   0 andreas    (501) staff       (20)       24 2023-04-18 15:13:54.000000 autocog-0.0.2/.gitignore
+-rw-r--r--   0 andreas    (501) staff       (20)     1227 2023-04-18 20:04:19.795093 autocog-0.0.2/PKG-INFO
+-rw-r--r--   0 andreas    (501) staff       (20)     1135 2023-04-18 20:03:23.000000 autocog-0.0.2/README.md
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:04:19.753303 autocog-0.0.2/autocog/
+-rw-r--r--   0 andreas    (501) staff       (20)    17478 2023-04-18 20:03:31.000000 autocog-0.0.2/autocog/autocog.py
+drwxr-xr-x   0 andreas    (501) staff       (20)        0 2023-04-18 20:04:19.794854 autocog-0.0.2/autocog.egg-info/
+-rw-r--r--   0 andreas    (501) staff       (20)     1227 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/PKG-INFO
+-rw-r--r--   0 andreas    (501) staff       (20)      236 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       52 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/entry_points.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       20 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/requires.txt
+-rw-r--r--   0 andreas    (501) staff       (20)        1 2023-04-18 20:04:19.000000 autocog-0.0.2/autocog.egg-info/top_level.txt
+-rw-r--r--   0 andreas    (501) staff       (20)       38 2023-04-18 20:04:19.795328 autocog-0.0.2/setup.cfg
+-rw-r--r--   0 andreas    (501) staff       (20)      540 2023-04-18 20:03:37.000000 autocog-0.0.2/setup.py
```

### Comparing `autocog-0.0.1/PKG-INFO` & `autocog-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: autocog
-Version: 0.0.1
+Version: 0.0.2
 Description-Content-Type: text/markdown
 
 # AutoCog
 
 _Generate [predict.py and cog.yaml](https://github.com/replicate/cog) automatically using GPT4_
 
-![Screen recording](assets/screen-recording.gif)
+![Screen recording](https://github.com/andreasjansson/AutoCog/raw/main/assets/screen-recording.gif)
 
 ## Usage
 
 First, set your OpenAI API key in an environment variable
 
 ```
 OPENAI_API_KEY=sk-...
```

### Comparing `autocog-0.0.1/README.md` & `autocog-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AutoCog
 
 _Generate [predict.py and cog.yaml](https://github.com/replicate/cog) automatically using GPT4_
 
-![Screen recording](assets/screen-recording.gif)
+![Screen recording](https://github.com/andreasjansson/AutoCog/raw/main/assets/screen-recording.gif)
 
 ## Usage
 
 First, set your OpenAI API key in an environment variable
 
 ```
 OPENAI_API_KEY=sk-...
```

### Comparing `autocog-0.0.1/autocog/autocog.py` & `autocog-0.0.2/autocog/autocog.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,46 +493,44 @@
     default=5,
     type=int,
     help="Number of attempts to try to fix issues before giving up",
 )
 @click.option(
     "-p",
     "--predict-command",
-    "initial_predict_command",
     help="Initial predict command. If not specified, AutoCog will generate one",
 )
 @click.option(
     "-c",
     "--continue",
     "continue_from_existing",
     is_flag=True,
     help="Continue to try to fix an existing predict.py and cog.yaml instead of generating them from scratch. AutoCog isn't perfect and having a human in the loop is often necessary.",
 )
 def autocog(
-    repo, openai_api_key, attempts, initial_predict_command, continue_from_existing
+    repo, openai_api_key, attempts, predict_command, continue_from_existing
 ):
     openai.api_key = openai_api_key
 
     repo_path = repo or os.getcwd()
 
     if continue_from_existing:
         files = {}
         for filename in ["cog.yaml", "predict.py"]:
             with open(os.path.join(repo_path, filename)) as f:
                 files[filename] = f.read()
     else:
         paths = order_paths(repo_path)
         files = generate_files(repo_path, paths)
         write_files(repo_path, files)
+
+    if not predict_command:
+        predict_command = generate_predict_command(files["predict.py"])
+    predict_command = create_files_for_predict_command(predict_command, repo_path)
     for attempt in range(attempts):
-        if attempt == 0 and initial_predict_command:
-            predict_command = initial_predict_command
-        else:
-            predict_command = generate_predict_command(files["predict.py"])
-        predict_command = create_files_for_predict_command(predict_command, repo_path)
         success, stderr = run_cog_predict(predict_command, repo_path)
         if success:
             return
 
         if attempt == attempts - 1:
             print(f"Failed after {attempts} attempts, giving up :'(")
             sys.exit(1)
@@ -550,11 +548,12 @@
         elif error_source == ERROR_COG_YAML:
             files["cog.yaml"] = fix_cog_yaml(
                 files["cog.yaml"], files["predict.py"], error, attempt=attempt
             )
             write_files(repo_path, files)
         elif error_source == ERROR_COG_PREDICT:
             predict_command = generate_predict_command(files["predict.py"])
+            predict_command = create_files_for_predict_command(predict_command, repo_path)
 
 
 if __name__ == "__main__":
     autocog()
```

### Comparing `autocog-0.0.1/autocog.egg-info/PKG-INFO` & `autocog-0.0.2/autocog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: autocog
-Version: 0.0.1
+Version: 0.0.2
 Description-Content-Type: text/markdown
 
 # AutoCog
 
 _Generate [predict.py and cog.yaml](https://github.com/replicate/cog) automatically using GPT4_
 
-![Screen recording](assets/screen-recording.gif)
+![Screen recording](https://github.com/andreasjansson/AutoCog/raw/main/assets/screen-recording.gif)
 
 ## Usage
 
 First, set your OpenAI API key in an environment variable
 
 ```
 OPENAI_API_KEY=sk-...
```

### Comparing `autocog-0.0.1/setup.py` & `autocog-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="autocog",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(),
     install_requires=[
         "openai",
         "click",
         "Pillow",
     ],
     entry_points={
```

