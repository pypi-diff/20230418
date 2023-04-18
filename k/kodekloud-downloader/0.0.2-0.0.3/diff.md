# Comparing `tmp/kodekloud-downloader-0.0.2.tar.gz` & `tmp/kodekloud-downloader-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodekloud-downloader-0.0.2.tar", max compression
+gzip compressed data, was "kodekloud-downloader-0.0.3.tar", max compression
```

## Comparing `kodekloud-downloader-0.0.2.tar` & `kodekloud-downloader-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    13313 2023-04-18 14:06:33.784184 kodekloud-downloader-0.0.2/README.md
--rw-r--r--   0        0        0     1007 2023-04-18 14:06:45.532733 kodekloud-downloader-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-18 14:06:33.784184 kodekloud-downloader-0.0.2/src/kodekloud_downloader/__init__.py
--rw-r--r--   0        0        0     1729 2023-04-18 14:06:33.784184 kodekloud-downloader-0.0.2/src/kodekloud_downloader/cli.py
--rw-r--r--   0        0        0      134 2023-04-18 14:06:33.784184 kodekloud-downloader-0.0.2/src/kodekloud_downloader/enums.py
--rw-r--r--   0        0        0     2144 2023-04-18 14:06:33.784184 kodekloud-downloader-0.0.2/src/kodekloud_downloader/helpers.py
--rw-r--r--   0        0        0     2273 2023-04-18 14:06:33.784184 kodekloud-downloader-0.0.2/src/kodekloud_downloader/main.py
--rw-r--r--   0        0        0     1976 2023-04-18 14:06:33.784184 kodekloud-downloader-0.0.2/src/kodekloud_downloader/models.py
--rw-r--r--   0        0        0    14565 2023-04-18 14:06:47.451894 kodekloud-downloader-0.0.2/setup.py
--rw-r--r--   0        0        0    14164 2023-04-18 14:06:47.453371 kodekloud-downloader-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    13313 2023-04-18 14:09:51.666578 kodekloud-downloader-0.0.3/README.md
+-rw-r--r--   0        0        0     1015 2023-04-18 14:10:00.910492 kodekloud-downloader-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-18 14:09:51.666578 kodekloud-downloader-0.0.3/src/kodekloud_downloader/__init__.py
+-rw-r--r--   0        0        0     1729 2023-04-18 14:09:51.666578 kodekloud-downloader-0.0.3/src/kodekloud_downloader/cli.py
+-rw-r--r--   0        0        0      134 2023-04-18 14:09:51.670578 kodekloud-downloader-0.0.3/src/kodekloud_downloader/enums.py
+-rw-r--r--   0        0        0     2144 2023-04-18 14:09:51.670578 kodekloud-downloader-0.0.3/src/kodekloud_downloader/helpers.py
+-rw-r--r--   0        0        0     2273 2023-04-18 14:09:51.670578 kodekloud-downloader-0.0.3/src/kodekloud_downloader/main.py
+-rw-r--r--   0        0        0     1976 2023-04-18 14:09:51.670578 kodekloud-downloader-0.0.3/src/kodekloud_downloader/models.py
+-rw-r--r--   0        0        0    14573 2023-04-18 14:10:02.328929 kodekloud-downloader-0.0.3/setup.py
+-rw-r--r--   0        0        0    14164 2023-04-18 14:10:02.330475 kodekloud-downloader-0.0.3/PKG-INFO
```

### Comparing `kodekloud-downloader-0.0.2/README.md` & `kodekloud-downloader-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kodekloud-downloader-0.0.2/pyproject.toml` & `kodekloud-downloader-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodekloud-downloader"
-version = "v0.0.2"
+version = "v0.0.3"
 description = "Simple downloaded for https://kodekloud.com/"
 readme = "README.md"
 authors = ["Roy, Debakar <debakar.roy@outlook.com>"]
 repository = "https://github.com/debakarr/kodekloud-downloader"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -26,12 +26,12 @@
 pep8-naming = "^0.13.3"
 pytest-cov = "^4.0.0"
 mypy = "^1.0.1"
 black = "^23.1.0"
 types-requests = "^2.28.11.15"
 
 [tool.poetry.scripts]
-kodekloud = "kodekloud_dl.cli:kodekloud"
+kodekloud = "kodekloud_downloader.cli:kodekloud"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kodekloud-downloader-0.0.2/src/kodekloud_downloader/cli.py` & `kodekloud-downloader-0.0.3/src/kodekloud_downloader/cli.py`

 * *Files identical despite different names*

### Comparing `kodekloud-downloader-0.0.2/src/kodekloud_downloader/helpers.py` & `kodekloud-downloader-0.0.3/src/kodekloud_downloader/helpers.py`

 * *Files identical despite different names*

### Comparing `kodekloud-downloader-0.0.2/src/kodekloud_downloader/main.py` & `kodekloud-downloader-0.0.3/src/kodekloud_downloader/main.py`

 * *Files identical despite different names*

### Comparing `kodekloud-downloader-0.0.2/src/kodekloud_downloader/models.py` & `kodekloud-downloader-0.0.3/src/kodekloud_downloader/models.py`

 * *Files identical despite different names*

### Comparing `kodekloud-downloader-0.0.2/setup.py` & `kodekloud-downloader-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
  'markdownify>=0.11.6,<0.12.0',
  'prettytable>=3.7.0,<4.0.0',
  'requests>=2.28.2,<3.0.0',
  'validators>=0.20.0,<0.21.0',
  'yt-dlp>=2023.2.17,<2024.0.0']
 
 entry_points = \
-{'console_scripts': ['kodekloud = kodekloud_dl.cli:kodekloud']}
+{'console_scripts': ['kodekloud = kodekloud_downloader.cli:kodekloud']}
 
 setup_kwargs = {
     'name': 'kodekloud-downloader',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Simple downloaded for https://kodekloud.com/',
     'long_description': '# KodeKloud Downloader\n\n## Disclaimer\nPlease use this only to keep your local copy. Please don\'t distribute the courses illegally. You will be responsible for the legal consequences. \n\n---\n\n## Features\n\n- Download video lessons in selected quality\n- Download resources (PDFs, etc.) alongside video lessons\n- Organizes downloaded content in a structured folder hierarchy\n\n---\n\n## Prerequisites\n\n- Python 3.8 or higher\n- ffmpeg\n\n<details>\n    <summary>How to Install FFmpeg on Linux, Mac, and Windows</summary>\n\n# How to Install FFmpeg on Linux, Mac, and Windows\n\nFFmpeg is a powerful and flexible multimedia processing tool that can handle a wide range of tasks, such as video and audio conversion, streaming, and recording. In this guide, we will show you how to install FFmpeg on Linux, Mac, and Windows operating systems.\n\n## Linux\n\n### Ubuntu and Debian-based distributions\n\n1.  Update the package lists for upgrades and new package installations.\n\n`sudo apt update`\n\n1.  Install FFmpeg using the following command:\n\n`sudo apt install ffmpeg`\n\n### Fedora\n\n1.  Install FFmpeg using the following command:\n\n`sudo dnf install ffmpeg`\n\n### Arch Linux and Manjaro\n\n1.  Install FFmpeg using the following command:\n\n`sudo pacman -S ffmpeg`\n\n## Mac\n\n### Using Homebrew\n\nIf you don\'t have Homebrew installed, you can install it by following the instructions on the [official Homebrew website](https://brew.sh/).\n\nUpdate Homebrew to ensure you have the latest package information:\n\n`brew update`\n\n1.  Install FFmpeg using the following command:\n\n`brew install ffmpeg`\n\n### Using MacPorts\n\nIf you don\'t have MacPorts installed, you can install it by following the instructions on the [official MacPorts website](https://www.macports.org/install.php).\n\nUpdate MacPorts to ensure you have the latest package information:\n\n`sudo port selfupdate`\n\n1.  Install FFmpeg using the following command:\n\n`sudo port install ffmpeg`\n\n## Windows\n\n### Using Chocolatey\n\nIf you don\'t have Chocolatey installed, you can install it by following the instructions on the [official Chocolatey website](https://chocolatey.org/install).\n\nOpen an elevated Command Prompt (run as Administrator) and install FFmpeg using the following command:\n\n`choco install ffmpeg`\n\n### Using Scoop\n\nIf you don\'t have Scoop installed, you can install it by following the instructions on the [official Scoop website](https://scoop.sh/).\n\nOpen a PowerShell terminal and install FFmpeg using the following command:\n\n`scoop install ffmpeg`\n\nAfter following these steps, FFmpeg should be installed on your system. You can check the installation by running the following command in your terminal or command prompt:\n\n`ffmpeg -version`\n\nThis will display the FFmpeg version and build information, confirming that the installation was successful.\n\n</details>\n\n\n\n## How to get cookie\n- Sign in to kodekloud.com\n- Right Click -> Inspect -> Go to Network Tab -> Reload -> Select the first resource and copy the cookie:\n\n![](https://i.imgur.com/MwkR9u6.png)\n\n## 💻 Installation\n\nTo install kodekloud-downloader, simply run the following command:\n\n```css\npip install -U kodekloud-downloader\n```\n\n## 📚 Usage\n\nAfter installing the package, you can use the `kodekloud dl` command to download shows from the command line.\n\n```css\nkisskh dl --help\nUsage: kodekloud dl [OPTIONS] [COURSE_URL]\n\nOptions:\n  -q, --quality [360p|480p|540p|720p|1080p]\n                                  Quality of the video to be downloaded.\n  -o, --output-dir TEXT           Output directory where downloaded files will\n                                  be store.\n  -c, --cookie TEXT               Cookie to download the courses.  [required]\n  --help                          Show this message and exit.\n```\n\nHere are some examples:\n\n### 🔗 Direct download entire course in highest quality available in current folder\n\n```css\nkodekloud dl "https://kodekloud.com/courses/amazon-elastic-container-service-aws-ecs/" -o . -c <YOUR COOKIE HERE INSIDE DOUBLE QUOTES>\n```\n\n### 🔍 Download entire course from list of available course in current folder\n\n```css\nkodekloud dl -o . -c <YOUR COOKIE HERE INSIDE DOUBLE QUOTES>\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\n| No. | Name                                                                        | Type    | Categories                                                 |\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\n| 1   | Ultimate Certified Kubernetes Application Developer (CKAD) Mock Exam Series | Premium | Challenges, Containers, Kubernetes                         |\n| 2   | GCP DevOps Project                                                          | Premium | Cloud, GCP                                                 |\n| 3   | 12 Factor App                                                               | Premium | Productivity                                               |\n| 4   | AZ-305: Microsoft Azure Solutions Architect Expert                          | Premium | Certification, Cloud, Devops                               |\n| 5   | Ultimate Certified Kubernetes Administrator (CKA) Mock Exam Series          | Free    | Container Orchestration, Kubernetes, Devops, Certification |\n| 6   | AWS Lambda                                                                  | Premium | AWS, Cloud                                                 |\n| 7   | Linux Professional Institute LPIC-1 Exam 101                                | Premium | Certification, Linux                                       |\n| 8   | Advanced Golang                                                             | Premium | Programming                                                |\n| 9   | Prometheus Certified Associate (PCA)                                        | Premium | Certification, Kubernetes, Monitoring                      |\n| 10  | GCP Cloud Digital Leader Certification                                      | Premium | Cloud, GCP, Certification                                  |\n| 11  | OpenShift 4                                                                 | Premium | Container Orchestration, Devops, Red Hat                   |\n| 12  | HashiCorp : Terraform Cloud                                                 | Premium | Cloud, Devops, HashiCorp                                   |\n| 13  | ArgoCD                                                                      | Premium | CI/CD, Devops, Kubernetes                                  |\n| 14  | Amazon Elastic Container Service (AWS ECS)                                  | Free    | AWS, Devops                                                |\n| 15  | Red Hat Certified System Administrator(RHCSA)                               | Premium | Devops, Linux, Red Hat, Certification                      |\n| 16  | Open Source for Beginners                                                   | Premium | Productivity                                               |\n| 17  | Kustomize                                                                   | Premium | Devops, Kubernetes                                         |\n| 18  | DevSecOps – Kubernetes DevOps & Security                                    | Premium | Devops, DevSecOps, Kubernetes                              |\n| 19  | AZ-104: Microsoft Azure Administrator                                       | Premium | Cloud, Devops, Certification                               |\n| 20  | DevOps Interview Preparation Course                                         | Premium | Devops                                                     |\n| 21  | Terraform Challenges                                                        | Free    | Challenges, Devops, IAC                                    |\n| 22  | HashiCorp Certified: Consul Associate Certification                         | Premium | Devops, HashiCorp                                          |\n| 23  | HashiCorp Certified: Vault Associate Certification                          | Premium | Devops, HashiCorp                                          |\n| 24  | Kubernetes Challenges                                                       | Free    | Challenges, Devops                                         |\n| 25  | Linux Challenges                                                            | Free    | Challenges, Devops, Linux                                  |\n| 26  | HashiCorp Certified: Vault Operations Professional 2022                     | Premium | Container Orchestration, Containers, Devops, HashiCorp     |\n| 27  | CKS – Challenges                                                            | Free    | Challenges, Container Orchestration, Containers, Devops    |\n| 28  | Linux Foundation Certified System Administrator (LFCS)                      | Premium | Devops, Linux, Certification                               |\n| 29  | Jenkins                                                                     | Premium | Automation, CI/CD, Devops                                  |\n| 30  | Golang                                                                      | Premium | Devops, Programming                                        |\n| 31  | Terraform Associate Certification: HashiCorp Certified                      | Premium | Container Orchestration, Devops, IAC, Certification        |\n| 32  | Helm for Beginners                                                          | Premium | Container Orchestration, Containers, Devops                |\n| 33  | PCAP – Python Certification Course                                          | Premium | Devops, Programming, Python, Certification                 |\n| 34  | Istio Service Mesh                                                          | Premium | Devops                                                     |\n| 35  | Jinja2 Basics (Mini Course)                                                 | Free    | Devops                                                     |\n| 36  | Certified Kubernetes Security Specialist (CKS)                              | Premium | Container Orchestration, Kubernetes, Devops, Certification |\n| 37  | Certified Python Entry-Level Programmer: PCEP-30-02                         | Premium | Devops, Programming, Python, Certification                 |\n| 38  | JSON Path Test – Free Course                                                | Free    | Devops                                                     |\n| 39  | Docker Certified Associate Exam Course                                      | Premium | Containers, Devops, Certification                          |\n| 40  | Terraform Basics Training Course                                            | Premium | Automation, Devops, IAC                                    |\n| 41  | CKA Certification Course – Certified Kubernetes Administrator               | Premium | Container Orchestration, Containers, Devops                |\n| 42  | Certified Kubernetes Application Developer (CKAD)                           | Premium | Container Orchestration, Kubernetes, Devops, Certification |\n| 43  | Kubernetes for the Absolute Beginners – Hands-on Tutorial                   | Premium | Container Orchestration, Containers, Kubernetes, Devops    |\n| 44  | Docker Training Course for the Absolute Beginner                            | Premium | Containers, Devops                                         |\n| 45  | Chef for the Absolute Beginners                                             | Premium | Automation, Devops                                         |\n| 46  | OpenShift 3 for the Absolute Beginners                                      | Premium | Container Orchestration, Containers, Devops                |\n| 47  | Ansible Advanced Course                                                     | Premium | Automation, Devops, IAC                                    |\n| 48  | Learn Ansible Basics – Beginners Course                                     | Premium | Automation, Devops, IAC                                    |\n| 49  | Docker – SWARM | SERVICES | STACKS – Hands-on                               | Premium | Containers, Devops                                         |\n| 50  | DevOps Pre-Requisite Course                                                 | Premium | Automation, Devops, IAC                                    |\n| 51  | Learning Linux Basics Course & Labs                                         | Premium | Devops, Linux                                              |\n| 52  | Shell Scripts for Beginners                                                 | Premium | Devops                                                     |\n| 53  | Puppet for the Absolute Beginners Course                                    | Premium | Automation, Devops, IAC                                    |\n| 54  | GIT for Beginners                                                           | Premium | Devops, Programming                                        |\n+-----+-----------------------------------------------------------------------------+---------+------------------------------------------------------------+\nEnter the number of the course you want to select: 35\n```',
     'author': 'Roy, Debakar',
     'author_email': 'debakar.roy@outlook.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/debakarr/kodekloud-downloader',
```

### Comparing `kodekloud-downloader-0.0.2/PKG-INFO` & `kodekloud-downloader-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodekloud-downloader
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple downloaded for https://kodekloud.com/
 Home-page: https://github.com/debakarr/kodekloud-downloader
 Author: Roy, Debakar
 Author-email: debakar.roy@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

