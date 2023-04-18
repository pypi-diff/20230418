# Comparing `tmp/update_pip_packages-0.1.2.tar.gz` & `tmp/update_pip_packages-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update_pip_packages-0.1.2.tar", max compression
+gzip compressed data, was "update_pip_packages-0.1.3.tar", max compression
```

## Comparing `update_pip_packages-0.1.2.tar` & `update_pip_packages-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2202 2023-04-17 22:06:57.790789 update_pip_packages-0.1.2/README.md
--rw-r--r--   0        0        0      480 2023-04-17 22:07:30.150780 update_pip_packages-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-15 15:28:02.452473 update_pip_packages-0.1.2/update_project/__init__.py
--rw-r--r--   0        0        0     5394 2023-04-17 21:38:58.551232 update_pip_packages-0.1.2/update_project/update_packages.py
--rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 update_pip_packages-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2232 2023-04-18 00:04:56.539638 update_pip_packages-0.1.3/README.md
+-rw-r--r--   0        0        0      480 2023-04-18 00:03:24.315494 update_pip_packages-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-15 15:28:02.452473 update_pip_packages-0.1.3/update_project/__init__.py
+-rw-r--r--   0        0        0     5650 2023-04-18 00:03:29.017160 update_pip_packages-0.1.3/update_project/update_packages.py
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 update_pip_packages-0.1.3/PKG-INFO
```

### Comparing `update_pip_packages-0.1.2/README.md` & `update_pip_packages-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Update Pip and App Packages
-## v0.1.2
+## v0.1.3
 
 This Python script provides an efficient way to update Pip and app packages on various Linux distributions. The script supports Ubuntu, Debian, Fedora, CentOS, Red Hat, Arch, Manjaro, OpenSUSE, and SUSE distributions. It updates packages using the appropriate package manager for each distribution.
 
 **I know this script may seem useless. Moreover, updating all pip packages can lead to challenges in some projects.
 This script is only a part of my self-education journey.**
 
 ## Features
@@ -18,14 +18,15 @@
 
 ```bash
 update-pip-packages [--pip] [--app]
 ```
 - -h, --help: Show this help message and exit
 - --pip: Update Pip packages.
 - --app: Update app packages.
+- -v, --version: Display the version of the package
 - If no options are provided, the script will display help information.
 
 ## Tests
 The tests cover various aspects of the script, including the following:
 
 - Getting the Linux distribution.
 - Updating Pip packages.
@@ -46,12 +47,12 @@
 ```
 or
 ```
 python3 -m pip install update-pip-packages
 ```
 
 ## GitHub Repository
-For more information, source code, and installation instructions, please visit the GitHub repository: [GitHub: update_packages](https://github.com/OleksandrMakarov/Scripts/tree/main/update-pip-project)
+For more information, source code, and installation instructions, please visit the GitHub repository: [GitHub: update-pip-packages](https://github.com/OleksandrMakarov/update-pip-project)
 
 ## Remarks
-There is also a [bash script](https://github.com/OleksandrMakarov/Scripts/tree/main/update-pip-project/update_packages.sh), I started with it and developed it into this Python project. 
+There is also a [bash script](https://github.com/OleksandrMakarov/update-pip-project/blob/main/update_packages.sh), I started with it and developed it into this Python project. 
 It does not support Linux distribution detection, but you can use it for the same purposes as the main(python) application in a Debian or Ubuntu environment.
```

### Comparing `update_pip_packages-0.1.2/update_project/update_packages.py` & `update_pip_packages-0.1.3/update_project/update_packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -133,20 +133,27 @@
 
 def main() -> None:
     parser = argparse.ArgumentParser(description="Update pip and app packages")
     parser.add_argument('--pip', action='store_true',
                         help='Update pip packages')
     parser.add_argument('--app', action='store_true',
                         help='Update app packages')
+    parser.add_argument('-v', '--version', action='store_true',
+                        help='Display the version of the package')
     args = parser.parse_args()
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
+    if args.version:
+        version = "0.1.3"
+        print(f"update-pip-packages version: {version}")
+        sys.exit(0)
+
     if args.pip:
         update_pip_packages()
     if args.app:
         update_app_packages()
 
 
 if __name__ == "__main__":
```

### Comparing `update_pip_packages-0.1.2/PKG-INFO` & `update_pip_packages-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: update-pip-packages
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: OleksandrMakarov
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: distro (>=1.8.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Update Pip and App Packages
-## v0.1.2
+## v0.1.3
 
 This Python script provides an efficient way to update Pip and app packages on various Linux distributions. The script supports Ubuntu, Debian, Fedora, CentOS, Red Hat, Arch, Manjaro, OpenSUSE, and SUSE distributions. It updates packages using the appropriate package manager for each distribution.
 
 **I know this script may seem useless. Moreover, updating all pip packages can lead to challenges in some projects.
 This script is only a part of my self-education journey.**
 
 ## Features
@@ -30,14 +30,15 @@
 
 ```bash
 update-pip-packages [--pip] [--app]
 ```
 - -h, --help: Show this help message and exit
 - --pip: Update Pip packages.
 - --app: Update app packages.
+- -v, --version: Display the version of the package
 - If no options are provided, the script will display help information.
 
 ## Tests
 The tests cover various aspects of the script, including the following:
 
 - Getting the Linux distribution.
 - Updating Pip packages.
@@ -58,13 +59,13 @@
 ```
 or
 ```
 python3 -m pip install update-pip-packages
 ```
 
 ## GitHub Repository
-For more information, source code, and installation instructions, please visit the GitHub repository: [GitHub: update_packages](https://github.com/OleksandrMakarov/Scripts/tree/main/update-pip-project)
+For more information, source code, and installation instructions, please visit the GitHub repository: [GitHub: update-pip-packages](https://github.com/OleksandrMakarov/update-pip-project)
 
 ## Remarks
-There is also a [bash script](https://github.com/OleksandrMakarov/Scripts/tree/main/update-pip-project/update_packages.sh), I started with it and developed it into this Python project. 
+There is also a [bash script](https://github.com/OleksandrMakarov/update-pip-project/blob/main/update_packages.sh), I started with it and developed it into this Python project. 
 It does not support Linux distribution detection, but you can use it for the same purposes as the main(python) application in a Debian or Ubuntu environment.
```

