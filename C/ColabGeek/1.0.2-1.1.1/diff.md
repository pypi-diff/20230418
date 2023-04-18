# Comparing `tmp/ColabGeek-1.0.2.tar.gz` & `tmp/ColabGeek-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ColabGeek-1.0.2.tar", last modified: Mon Apr 17 11:27:43 2023, max compression
+gzip compressed data, was "ColabGeek-1.1.1.tar", last modified: Tue Apr 18 03:18:11 2023, max compression
```

## Comparing `ColabGeek-1.0.2.tar` & `ColabGeek-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:27:43.284695 ColabGeek-1.0.2/
--rw-rw-r--   0 root         (0) root         (0)     1067 2023-04-17 10:15:07.000000 ColabGeek-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5154 2023-04-17 11:27:43.284695 ColabGeek-1.0.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     4417 2023-04-17 11:20:28.000000 ColabGeek-1.0.2/README.md
--rw-rw-r--   0 root         (0) root         (0)      939 2023-04-17 11:20:28.000000 ColabGeek-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 11:27:43.284695 ColabGeek-1.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:27:43.282695 ColabGeek-1.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:27:43.283695 ColabGeek-1.0.2/src/ColabGeek/
--rw-rw-r--   0 root         (0) root         (0)     6650 2023-04-17 11:20:28.000000 ColabGeek-1.0.2/src/ColabGeek/ColabGeek.py
--rw-rw-r--   0 root         (0) root         (0)       24 2023-04-17 10:15:07.000000 ColabGeek-1.0.2/src/ColabGeek/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:27:43.284695 ColabGeek-1.0.2/src/ColabGeek/shell_scripts/
--rw-rw-r--   0 root         (0) root         (0)      382 2023-04-17 10:15:07.000000 ColabGeek-1.0.2/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
--rw-rw-r--   0 root         (0) root         (0)     1192 2023-04-17 10:15:07.000000 ColabGeek-1.0.2/src/ColabGeek/shell_scripts/Run_code_server.exp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 11:27:43.283695 ColabGeek-1.0.2/src/ColabGeek.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5154 2023-04-17 11:27:43.000000 ColabGeek-1.0.2/src/ColabGeek.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-04-17 11:27:43.000000 ColabGeek-1.0.2/src/ColabGeek.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 11:27:43.000000 ColabGeek-1.0.2/src/ColabGeek.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-17 11:27:43.000000 ColabGeek-1.0.2/src/ColabGeek.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 03:18:11.984721 ColabGeek-1.1.1/
+-rw-rw-r--   0 root         (0) root         (0)     1067 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5602 2023-04-18 03:18:11.984721 ColabGeek-1.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4865 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)      939 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 03:18:11.984721 ColabGeek-1.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 03:18:11.982721 ColabGeek-1.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 03:18:11.983721 ColabGeek-1.1.1/src/ColabGeek/
+-rw-rw-r--   0 root         (0) root         (0)     6993 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/src/ColabGeek/ColabGeek.py
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/src/ColabGeek/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 03:18:11.984721 ColabGeek-1.1.1/src/ColabGeek/shell_scripts/
+-rw-rw-r--   0 root         (0) root         (0)      382 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/src/ColabGeek/shell_scripts/Run_Rstudio_server.sh
+-rw-rw-r--   0 root         (0) root         (0)     1192 2023-04-18 03:15:02.000000 ColabGeek-1.1.1/src/ColabGeek/shell_scripts/Run_code_server.exp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 03:18:11.983721 ColabGeek-1.1.1/src/ColabGeek.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5602 2023-04-18 03:18:11.000000 ColabGeek-1.1.1/src/ColabGeek.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-04-18 03:18:11.000000 ColabGeek-1.1.1/src/ColabGeek.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 03:18:11.000000 ColabGeek-1.1.1/src/ColabGeek.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 03:18:11.000000 ColabGeek-1.1.1/src/ColabGeek.egg-info/top_level.txt
```

### Comparing `ColabGeek-1.0.2/LICENSE` & `ColabGeek-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.0.2/PKG-INFO` & `ColabGeek-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.0.2
+Version: 1.1.1
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -49,14 +49,24 @@
 # - port The port you want to run code server on, set to None to use the default port.
 # - password The code server login password, set to None and use the linux user password by default.
 # - verbose Show the running logs.
 
 main.Run_code_server()
 ```
 
+You can also install code server extension by providing extension id or the path of the VSIX file downloaded from [vscode marketplace](https://marketplace.visualstudio.com/vscode).
+
+```python
+# ColabGeek.Install_code_server_extension has the following parameters:
+# - extension The extension id or the path of the VSIX file.
+# - verbose Show the running logs.
+
+main.Install_code_server_extension(extension='ms-python.anaconda-extension-pack')
+```
+
 ### Run Rstudio server
 
 [Rstudio server](https://posit.co/products/open-source/rstudio-server/) is a web IDE for R programming. With Rstudio server, users can run R scripts, create and manage R projects, develop and test code, and share their work with others. Rstudio server also offers powerful features such as syntax highlighting, code completion, debugging and data visualization.
 
 ```python
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
```

### Comparing `ColabGeek-1.0.2/README.md` & `ColabGeek-1.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,14 +35,24 @@
 # - port The port you want to run code server on, set to None to use the default port.
 # - password The code server login password, set to None and use the linux user password by default.
 # - verbose Show the running logs.
 
 main.Run_code_server()
 ```
 
+You can also install code server extension by providing extension id or the path of the VSIX file downloaded from [vscode marketplace](https://marketplace.visualstudio.com/vscode).
+
+```python
+# ColabGeek.Install_code_server_extension has the following parameters:
+# - extension The extension id or the path of the VSIX file.
+# - verbose Show the running logs.
+
+main.Install_code_server_extension(extension='ms-python.anaconda-extension-pack')
+```
+
 ### Run Rstudio server
 
 [Rstudio server](https://posit.co/products/open-source/rstudio-server/) is a web IDE for R programming. With Rstudio server, users can run R scripts, create and manage R projects, develop and test code, and share their work with others. Rstudio server also offers powerful features such as syntax highlighting, code completion, debugging and data visualization.
 
 ```python
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
```

### Comparing `ColabGeek-1.0.2/pyproject.toml` & `ColabGeek-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 where = ["src"]
 
 [tool.setuptools.package-data]
 "ColabGeek.shell_scripts" = ["*"]
 
 [project]
 name = "ColabGeek"
-version = "1.0.2"
+version = "1.1.1"
 authors = [
     {name = "Yiming Sun",email = "yiming.sun12138@gmail.com"},
 ]
 description = "ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ColabGeek-1.0.2/src/ColabGeek/ColabGeek.py` & `ColabGeek-1.1.1/src/ColabGeek/ColabGeek.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,21 @@
 
         # run code server
         char_cmd = "expect" + " " + str(script_path) + " " + str(self.user) + " " + str(self.password) + " " + str(port) + " " + str(password) + " " + str(self.path)
         exec_logging = os.popen(char_cmd)
         if verbose:
             exec_logging = ''.join(exec_logging.readlines())
             print(exec_logging)
+
+    def Install_code_server_extension(self,extension,verbose = True):
+        char_cmd = "sudo -u" + " " + str(self.user) + " " + "code-server --install-extension" + " " + str(extension)
+        exec_logging = os.popen(char_cmd)
+        if verbose:
+            exec_logging = ''.join(exec_logging.readlines())
+            print(exec_logging)
             
     '''
     proxy method
     '''
     # run shadowsocks
     def Run_shadowsocks(self,port = None,password = None,encrypt = 'aes-256-gcm'):
         # check param
```

### Comparing `ColabGeek-1.0.2/src/ColabGeek/shell_scripts/Run_code_server.exp` & `ColabGeek-1.1.1/src/ColabGeek/shell_scripts/Run_code_server.exp`

 * *Files identical despite different names*

### Comparing `ColabGeek-1.0.2/src/ColabGeek.egg-info/PKG-INFO` & `ColabGeek-1.1.1/src/ColabGeek.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColabGeek
-Version: 1.0.2
+Version: 1.1.1
 Summary: ColabGeek is designed to help run useful tools on Google Colab, including port forwarding, web IDE and so on. It is worth noting that this package is also compatible with other Ubuntu operating system servers, so try on other platforms as well.
 Author-email: Yiming Sun <yiming.sun12138@gmail.com>
 Project-URL: Homepage, https://github.com/yimingsun12138/ColabGeek
 Project-URL: Bug Tracker, https://github.com/yimingsun12138/ColabGeek/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -49,14 +49,24 @@
 # - port The port you want to run code server on, set to None to use the default port.
 # - password The code server login password, set to None and use the linux user password by default.
 # - verbose Show the running logs.
 
 main.Run_code_server()
 ```
 
+You can also install code server extension by providing extension id or the path of the VSIX file downloaded from [vscode marketplace](https://marketplace.visualstudio.com/vscode).
+
+```python
+# ColabGeek.Install_code_server_extension has the following parameters:
+# - extension The extension id or the path of the VSIX file.
+# - verbose Show the running logs.
+
+main.Install_code_server_extension(extension='ms-python.anaconda-extension-pack')
+```
+
 ### Run Rstudio server
 
 [Rstudio server](https://posit.co/products/open-source/rstudio-server/) is a web IDE for R programming. With Rstudio server, users can run R scripts, create and manage R projects, develop and test code, and share their work with others. Rstudio server also offers powerful features such as syntax highlighting, code completion, debugging and data visualization.
 
 ```python
 # ColabGeek.Run_Rstudio_server has the following parameters:
 # - port The port you want to run Rstudio on, set to None to use the default port.
```

