# Comparing `tmp/update_pip_packages-0.1.1.tar.gz` & `tmp/update_pip_packages-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update_pip_packages-0.1.1.tar", max compression
+gzip compressed data, was "update_pip_packages-0.1.2.tar", max compression
```

## Comparing `update_pip_packages-0.1.1.tar` & `update_pip_packages-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2202 2023-04-17 21:03:45.931791 update_pip_packages-0.1.1/README.md
--rw-r--r--   0        0        0      480 2023-04-17 21:02:27.951809 update_pip_packages-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-15 15:28:02.452473 update_pip_packages-0.1.1/update_project/__init__.py
--rw-r--r--   0        0        0     5154 2023-04-15 15:51:35.400818 update_pip_packages-0.1.1/update_project/update_packages.py
--rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 update_pip_packages-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2202 2023-04-17 22:06:57.790789 update_pip_packages-0.1.2/README.md
+-rw-r--r--   0        0        0      480 2023-04-17 22:07:30.150780 update_pip_packages-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-15 15:28:02.452473 update_pip_packages-0.1.2/update_project/__init__.py
+-rw-r--r--   0        0        0     5394 2023-04-17 21:38:58.551232 update_pip_packages-0.1.2/update_project/update_packages.py
+-rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 update_pip_packages-0.1.2/PKG-INFO
```

### Comparing `update_pip_packages-0.1.1/README.md` & `update_pip_packages-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Update Pip and App Packages
-## v0.1.1
+## v0.1.2
 
 This Python script provides an efficient way to update Pip and app packages on various Linux distributions. The script supports Ubuntu, Debian, Fedora, CentOS, Red Hat, Arch, Manjaro, OpenSUSE, and SUSE distributions. It updates packages using the appropriate package manager for each distribution.
 
 **I know this script may seem useless. Moreover, updating all pip packages can lead to challenges in some projects.
 This script is only a part of my self-education journey.**
 
 ## Features
```

### Comparing `update_pip_packages-0.1.1/update_project/update_packages.py` & `update_pip_packages-0.1.2/update_project/update_packages.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,17 +34,22 @@
     packages_to_update = [pkg["name"] for pkg in json.loads(outdated_packages)]
 
     if not packages_to_update:
         print("All pip packages are up-to-date.")
     else:
         print("Updating pip packages...")
         for package in packages_to_update:
-            subprocess.check_call(
+            update_result = subprocess.run(
                 [sys.executable, "-m", "pip", "install", "--upgrade", package])
-        print("Pip packages updated successfully.")
+            if update_result.returncode == 0:
+                print(f"{package} updated successfully.")
+            else:
+                print(
+                    f"Error updating {package}. Return code: {update_result.returncode}")
+        print("Pip packages update completed.")
 
 
 def update_apt_packages() -> None:
     print("Updating apt packages...")
     apt_update_result = subprocess.run(["sudo", "apt", "update"])
     if apt_update_result.returncode == 0:
         print("Apt update completed successfully.")
```

### Comparing `update_pip_packages-0.1.1/PKG-INFO` & `update_pip_packages-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: update-pip-packages
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: OleksandrMakarov
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: distro (>=1.8.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Update Pip and App Packages
-## v0.1.1
+## v0.1.2
 
 This Python script provides an efficient way to update Pip and app packages on various Linux distributions. The script supports Ubuntu, Debian, Fedora, CentOS, Red Hat, Arch, Manjaro, OpenSUSE, and SUSE distributions. It updates packages using the appropriate package manager for each distribution.
 
 **I know this script may seem useless. Moreover, updating all pip packages can lead to challenges in some projects.
 This script is only a part of my self-education journey.**
 
 ## Features
```

