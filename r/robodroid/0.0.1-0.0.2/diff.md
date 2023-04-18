# Comparing `tmp/robodroid-0.0.1.tar.gz` & `tmp/robodroid-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robodroid-0.0.1.tar", max compression
+gzip compressed data, was "robodroid-0.0.2.tar", max compression
```

## Comparing `robodroid-0.0.1.tar` & `robodroid-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35149 2023-04-14 13:37:15.254915 robodroid-0.0.1/LICENSE
--rw-r--r--   0        0        0    12421 2023-04-14 13:37:15.254915 robodroid-0.0.1/README.md
--rw-r--r--   0        0        0     1459 2023-04-14 13:37:15.258915 robodroid-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      282 2023-04-14 13:37:15.258915 robodroid-0.0.1/robodroid/__init__.py
--rw-r--r--   0        0        0       33 2023-04-14 13:37:15.258915 robodroid-0.0.1/robodroid/config/metadata.json
--rw-r--r--   0        0        0      560 2023-04-14 13:37:15.258915 robodroid-0.0.1/robodroid/config/template.yaml
--rw-r--r--   0        0        0     1935 2023-04-14 13:37:15.258915 robodroid-0.0.1/robodroid/main.py
--rw-r--r--   0        0        0      133 2023-04-14 13:37:15.258915 robodroid-0.0.1/robodroid/services/__init__.py
--rw-r--r--   0        0        0     4835 2023-04-14 13:37:15.258915 robodroid-0.0.1/robodroid/services/adb.py
--rw-r--r--   0        0        0     6195 2023-04-14 13:37:15.258915 robodroid-0.0.1/robodroid/services/frida.py
--rw-r--r--   0        0        0  3462429 2023-04-14 13:37:15.270915 robodroid-0.0.1/robodroid/tests/assets/InsecureBankv2.apk
--rw-r--r--   0        0        0     2040 2023-04-14 13:37:15.270915 robodroid-0.0.1/robodroid/tests/test_adb.py
--rw-r--r--   0        0        0      304 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/tests/test_config.py
--rw-r--r--   0        0        0      214 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/tests/test_helpers.py
--rw-r--r--   0        0        0       68 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/types/__init__.py
--rw-r--r--   0        0        0     1270 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/types/common.py
--rw-r--r--   0        0        0      855 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/types/enum.py
--rw-r--r--   0        0        0      241 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/utils/__init__.py
--rw-r--r--   0        0        0      790 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/utils/constants.py
--rw-r--r--   0        0        0       44 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/utils/exceptions.py
--rw-r--r--   0        0        0    11355 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/utils/helper.py
--rw-r--r--   0        0        0     2764 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/utils/logger.py
--rw-r--r--   0        0        0     2941 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/utils/schemas.py
--rw-r--r--   0        0        0      179 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/workflow/__init__.py
--rw-r--r--   0        0        0      726 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/workflow/commands.py
--rw-r--r--   0        0        0      285 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/workflow/config.py
--rw-r--r--   0        0        0     4794 2023-04-14 13:37:15.274915 robodroid-0.0.1/robodroid/workflow/manager.py
--rw-r--r--   0        0        0    13520 1970-01-01 00:00:00.000000 robodroid-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-18 16:20:47.927374 robodroid-0.0.2/LICENSE
+-rw-r--r--   0        0        0    16314 2023-04-18 16:20:47.927374 robodroid-0.0.2/README.md
+-rw-r--r--   0        0        0     1459 2023-04-18 16:20:47.935374 robodroid-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-04-18 16:20:47.935374 robodroid-0.0.2/robodroid/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-18 16:20:47.935374 robodroid-0.0.2/robodroid/config/metadata.json
+-rw-r--r--   0        0        0      563 2023-04-18 16:20:47.935374 robodroid-0.0.2/robodroid/config/template.yaml
+-rw-r--r--   0        0        0     4744 2023-04-18 16:20:47.935374 robodroid-0.0.2/robodroid/main.py
+-rw-r--r--   0        0        0      133 2023-04-18 16:20:47.935374 robodroid-0.0.2/robodroid/services/__init__.py
+-rw-r--r--   0        0        0     4992 2023-04-18 16:20:47.935374 robodroid-0.0.2/robodroid/services/adb.py
+-rw-r--r--   0        0        0     6373 2023-04-18 16:20:47.935374 robodroid-0.0.2/robodroid/services/frida.py
+-rw-r--r--   0        0        0  3462429 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/tests/assets/InsecureBankv2.apk
+-rw-r--r--   0        0        0     2040 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/tests/test_adb.py
+-rw-r--r--   0        0        0      434 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/tests/test_config.py
+-rw-r--r--   0        0        0      214 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/tests/test_helpers.py
+-rw-r--r--   0        0        0       68 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/types/__init__.py
+-rw-r--r--   0        0        0     1540 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/types/common.py
+-rw-r--r--   0        0        0     1063 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/types/enum.py
+-rw-r--r--   0        0        0      241 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/utils/__init__.py
+-rw-r--r--   0        0        0     1177 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/utils/constants.py
+-rw-r--r--   0        0        0       44 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/utils/exceptions.py
+-rw-r--r--   0        0        0    14619 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/utils/helper.py
+-rw-r--r--   0        0        0     2764 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/utils/logger.py
+-rw-r--r--   0        0        0     3343 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/utils/schemas.py
+-rw-r--r--   0        0        0      179 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/workflow/__init__.py
+-rw-r--r--   0        0        0      726 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/workflow/commands.py
+-rw-r--r--   0        0        0      285 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/workflow/config.py
+-rw-r--r--   0        0        0     4815 2023-04-18 16:20:47.951374 robodroid-0.0.2/robodroid/workflow/manager.py
+-rw-r--r--   0        0        0    17413 1970-01-01 00:00:00.000000 robodroid-0.0.2/PKG-INFO
```

### Comparing `robodroid-0.0.1/LICENSE` & `robodroid-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robodroid-0.0.1/README.md` & `robodroid-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,16 @@
     <img src="https://raw.githubusercontent.com/cybersecsi/robodroid/main/logo.png" alt= "robodroid" width="200px">
 </h1>
 <p align="center">
     <b>RoboDroid</b>
 <p>
 
 <p align="center">
-    <img src="https://github.com/cybersecsi/robodroid/actions/workflows/release.yml/badge.svg"/>
-    <img src="https://github.com/cybersecsi/robodroid/actions/workflows/publish.yml/badge.svg"/>
+    <img src="https://github.com/cybersecsi/robodroid/actions/workflows/release.yaml/badge.svg"/>
+    <img src="https://github.com/cybersecsi/robodroid/actions/workflows/publish.yaml/badge.svg"/>
   <a href="https://github.com/cybersecsi/robodroid/blob/main/README.md"><img src="https://img.shields.io/badge/Documentation-complete-green.svg?style=flat"></a>
   <a href="https://github.com/cybersecsi/robodroid/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-GPL3-blue.svg"></a>
 </p>
 
 RoboDroid is a cutting-edge software tool designed to simplify the process of managing (and **very soon** also deploying) Android machines for usage in Cyber Range environments. With RoboDroid, users can easily set up and customize pre-defined behaviors for their Android machines, allowing them to create complex cyber attack scenarios and test their defenses against a wide range of threats.
 
 <!-- omit in toc -->
@@ -21,14 +21,17 @@
 - [📱 Context](#-context)
 - [⚡ Overview](#-overview)
 - [📚 How It Works](#-how-it-works)
   - [Interaction with the Frida Agent](#interaction-with-the-frida-agent)
 - [🔌 Install](#-install)
   - [RoboDroid Library](#robodroid-library)
 - [ℹ️ Usage](#ℹ️-usage)
+  - [``run`` command](#run-command)
+  - [ENV Variables](#env-variables)
+  - [Run in Docker](#run-in-docker)
 - [🚀 Demo](#-demo)
 - [🚧 Roadmap](#-roadmap)
 - [📚 Credits](#-credits)
 - [🪪 License](#-license)
 
 ## 📱 Context
 Mobile devices have become ubiquitous in today's world. People use smartphones for almost every aspect of their lives, including banking, shopping, and communication. As a result, mobile devices are now a primary target for cybercriminals.
@@ -44,28 +47,30 @@
 
 RoboDroid leverages [Frida](https://frida.re) technology to run behaviors that are specific to applications, while using ``ADB`` for all other operations. This powerful combination enables users to create workflows of preset behaviors that can simulate a mobile user's actions.
 
 One example of a workflow that can be used in a cyber range environment involves simulating a mobile user receiving a phishing email, clicking on the link contained in the email, and subsequently downloading a malware.
 
 The following picture summarizes it:
 
-![Kill Chain Example](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-chain-example.png)
+![Kill Chain Example](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-chain-example.png#gh-light-mode-only)
+![Kill Chain Example](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-chain-example-dark.png#gh-dark-mode-only)
 
 The workflow can be broken down into the following steps:
 
 1. The user receives a phishing email containing a link that appears legitimate.
 2. The user clicks on the link, which redirects them to a malicious website.
 3. The website prompts the user to download an app, which they do.
 4. The app is installed on the user's device and begins executing malicious code.
 5. The malware gains access to sensitive data on the device, such as passwords, credit card information, and other personal details.
 
 By creating and running workflows like this, users can simulate realistic cyber attack scenarios and test their defenses against a wide range of threats. This helps to ensure that systems and networks are well-protected against potential vulnerabilities, and that users are prepared to respond effectively in the event of an attack.
 
 ## 📚 How It Works
-![How RoboDroid Works](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/how-it-works.png)
+![How RoboDroid Works](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/how-it-works.png#gh-light-mode-only)
+![How RoboDroid Works](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/how-it-works-dark.png#gh-dark-mode-only)
 
 ### Interaction with the Frida Agent
 
 RoboDroid ommunicates with the Frida Agent provided by the RoboDroid Library via messages, providing efficient interaction.
 When the RoboDroid begins a specific behavior, it awaits a message from the Frida Agent. The message could be of either ``FAILURE`` or ``COMPLETED`` type.
 
 If the message type is ``FAILURE`` RoboDroid restarts the current behavior to ensure successful completion. If the message type is ``COMPLETED`` the current step is marked as finished, and RoboDroid moves to the next step.
@@ -89,50 +94,107 @@
 ```
 robodroid --help
 ```
 
 This will display the help for the tool:
 
 ```
-    ███████╗███████╗ ██████╗███████╗██╗
-    ██╔════╝██╔════╝██╔════╝██╔════╝██║
-    ███████╗█████╗  ██║     ███████╗██║
-    ╚════██║██╔══╝  ██║     ╚════██║██║
-    ███████║███████╗╚██████╗███████║██║
-    ╚══════╝╚══════╝ ╚═════╝╚══════╝╚═╝
-    RoboDroid v0.0.1
+              &&&&&&&&&&&
+           &&&&         &&&&
+         &&&               &&&
+      (&&&&   &&&&   &&&&   &&&)&
+      &(&&&&               &&&&)&
+          &&&&           &&&&
+             &&&&&&&&&&&&&
+       &&&  &&&&&&&&&&&&&&&  &&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+              &&&&&&&&&&&
+               &&&& &&&&
+               &&&& &&&&
+            RoboDroid v0.0.2
 
-
- Usage: robodroid [OPTIONS]
+ Usage: robodroid [OPTIONS] COMMAND [ARGS]...
 
  Manage and deploy Android machines with pre-defined behaviors for Cyber Range environments
 
-╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --log-mode          [silent|normal|debug]  Set logging mode [default: normal]                                                   │
-│ --help      -h                             Show this message and exit.                                                          │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ──────────────────────────────────────────────────────────────────────────────────╮
+│ --help  -h        Show this message and exit.                                              │
+╰────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ─────────────────────────────────────────────────────────────────────────────────╮
+│ run               Run RoboDroid.                                                           │
+| update-library    Update the RoboDroid Library to the latest version                       |
+│ version           Print the current version and exit.                                      │
+╰────────────────────────────────────────────────────────────────────────────────────────────╯
+
 ```
 
-Before actually running it you need to provide at least one valid config file that **must** be placed under ``$HOME/.RoboDroid/config`` in ``yaml`` format.
-This config file defines all the steps of the workflow that will be executed, you can take a look at the ``examples`` folder for some valid configurations. The following table provides a description of the fields used in the config file:
-
-| **Key**  | **Required** | **Description**                                      |
-|----------|--------------|------------------------------------------------------|
-| id       | True         | The ID of the workflow                               |
-| init     | False        | The init section, contains the initial setup actions |
-| workflow | True         | The actual workflow to be executed                   |
+### ``run`` command
+You can run ``robodroid`` in two different modes:
+- Interactive (``default``)
+- Managed
+
+```
+              &&&&&&&&&&&
+           &&&&         &&&&
+         &&&               &&&
+      (&&&&   &&&&   &&&&   &&&)&
+      &(&&&&               &&&&)&
+          &&&&           &&&&
+             &&&&&&&&&&&&&
+       &&&  &&&&&&&&&&&&&&&  &&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+              &&&&&&&&&&&
+               &&&& &&&&
+               &&&& &&&&
+            RoboDroid v0.0.2
+
+ Usage: robodroid run [OPTIONS]
+
+ Run RoboDroid.
+
+╭─ Options ───────────────────────────────────────────────────────────────────────────╮
+│ --log-mode          [silent|normal|debug]  Set logging mode [default: normal]       │
+│ --mode      -m      [interactive|managed]  Set run mode [default: interactive]      │
+│ --config    -c      TEXT                   Name of the managed config file to load  │
+│ --help      -h                             Show this message and exit.              │
+╰─────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+In the interactive mode there is a prompt that lets the user select the ``ADB`` host, the port and the device to use while the **managed** mode uses a config file that **MUST BE PLACED** under ``$HOME/.RoboDroid/config`` in ``yaml`` format. The **managed** mode is the perfect mode to use while setting up a lab/environment without the need of user input/configuration.
+The following table provides a description of the fields used in the **config** file:
+| **Key**   | **Required** | **Description**                                      |
+|-----------|--------------|------------------------------------------------------|
+| device    | True         | Info about the device to use                         |
+| workflow  | True         | The workflow to use (name of the file)               |
+
+Before actually running it you need to provide at least one valid workflow file that **must** be placed under ``$HOME/.RoboDroid/workflows`` in ``yaml`` format.
+This config file defines all the steps of the workflow that will be executed, you can take a look at the ``examples`` folder for some valid configurations. The following table provides a description of the fields used in the **workflow** file:
+
+| **Key**   | **Required** | **Description**                                      |
+|-----------|--------------|------------------------------------------------------|
+| id        | True         | The ID of the workflow                               |
+| init      | False        | The init section, contains the initial setup actions |
+| behaviors | True         | The list of behaviors to execute                     |
 
 In the ``init`` section you may set the APKs that must be installed and the packages that must be cleaned up (storage and cache) before running the actual workflow. The structure of this section is the following:
 
 | **Key** | **Required** | **Description**                                  |
 |---------|--------------|--------------------------------------------------|
 | install | True         | List of paths of APKs to install                 |
 | clear   | False        | List of packages to clean up (storage and cache) |
 
-In the ``worfklow`` section there is the actual workflow. It is a **list** of elements that are called **steps** which are meant to be executed **sequentially**. Every *step* has the following structure:
+In the ``behaviors`` section there is the actual workflow. It is a **list** of elements that are called **steps** which are meant to be executed **sequentially**. Every *step* has the following structure:
 
 | **Key** | **Required** | **Description**                                                             |
 |---------|--------------|-----------------------------------------------------------------------------|
 | id      | True         | ID of the step                                                              |
 | name    | True         | The name of the behavior (in the RoboDroid Library or in the commands list) |
 | type    | True         | The type of the behavior ("frida-behavior", "adb")                          |
 | inputs  | False        | The list of inputs                                                          |
@@ -155,14 +217,26 @@
     type: frida
     inputs:
       - id: link
         value: robodroid.outputs.get-link.link
 ...
 ```
 
+### ENV Variables
+
+The CLI options can also be set through env variables (especially useful when running inside Docker); the following table provides a list of the current env variables available:
+| **Key**                       | **Description**                                                           |
+|-------------------------------|---------------------------------------------------------------------------|
+| ROBODROID_LOG_MODE            | Log level of RoboDroid [silent|normal|debug]                              |
+| ROBODROID_RUN_MODE            | Run mode [interactive|managed]                                            |
+| ROBODROID_MANAGED_CONFIG_NAME | The name of the managed config to use (while running in ``managed`` mode) |
+
+### Run in Docker
+TODO
+
 ## 🚀 Demo
 
 We made a brief demo video that shows RoboDroid in action with a template that does the following:
 1. Sets up and email account on the K9 Mail app
 2. Waits indefinitely for a new email and returns the first link inside it
 3. Opens the link with the Firefox Android (Fenix) application, downloads the linked file and installs it
 
@@ -173,19 +247,19 @@
 
 ## 🚧 Roadmap
 *RoboDroid* is a newborn tool and still needs to grow up! Currently these are the features we plan to add very soon:
 - [ ] Automatic deploy of AVD
 - [ ] Automatic deploy of ReDroid instance
 - [ ] Automatic deploy of Genymotion instance
 - [ ] Multi-device support
-- [ ] Interactive mode (without workflow config file)
+- [ ] ~~Interactive~~ Creative mode (without workflow file)
 - [ ] Continuous workflow mode (restart the whole workflow indefinitely until manually stopped)
 
 Of course we plan to add more and more behaviors in the [RoboDroid Library](https://github.com/cybersecsi/robodroid-library) and more and more ``adb`` commands in this repo. We also encourage every user to contribute to this projet and make it better!
 
 ## 📚 Credits
 
 Developed by Angelo Delicato [@SecSI](https://secsi.io)
 
 ## 🪪 License
 
-_robodroid_ is released under the [GPL-3.0 LICENSE](https://github.com/cybersecsi/robodroid/blob/main/LICENSE)
+_RoboDroid_ is released under the [GPL-3.0 LICENSE](https://github.com/cybersecsi/robodroid/blob/main/LICENSE)
```

#### html2text {}

```diff
@@ -1,115 +1,142 @@
                                     ******
                               [robodroid] ******
                                    RoboDroid
-    [https://github.com/cybersecsi/robodroid/actions/workflows/release.yml/
+   [https://github.com/cybersecsi/robodroid/actions/workflows/release.yaml/
     badge.svg] [https://github.com/cybersecsi/robodroid/actions/workflows/
- publish.yml/badge.svg] [https://img.shields.io/badge/Documentation-complete-
+ publish.yaml/badge.svg] [https://img.shields.io/badge/Documentation-complete-
   green.svg?style=flat] [https://img.shields.io/badge/License-GPL3-blue.svg]
 RoboDroid is a cutting-edge software tool designed to simplify the process of
 managing (and **very soon** also deploying) Android machines for usage in Cyber
 Range environments. With RoboDroid, users can easily set up and customize pre-
 defined behaviors for their Android machines, allowing them to create complex
 cyber attack scenarios and test their defenses against a wide range of threats.
 ## ð Table of Contents - [ð± Context](#-context) - [â¡ Overview](#-
 overview) - [ð How It Works](#-how-it-works) - [Interaction with the Frida
 Agent](#interaction-with-the-frida-agent) - [ð Install](#-install) -
-[RoboDroid Library](#robodroid-library) - [â¹ï¸ Usage](#â¹ï¸-usage) - [ð
-Demo](#-demo) - [ð§ Roadmap](#-roadmap) - [ð Credits](#-credits) - [ðªª
-License](#-license) ## ð± Context Mobile devices have become ubiquitous in
-today's world. People use smartphones for almost every aspect of their lives,
-including banking, shopping, and communication. As a result, mobile devices are
-now a primary target for cybercriminals. However, the security of mobile
-devices is often overlooked in cybersecurity training and testing environments.
-This can leave organizations vulnerable to attacks that exploit the weaknesses
-of mobile devices. Therefore, it is important to introduce mobile components in
-next-generation cyber-ranges to adapt to the current world that is more and
-more smartphone-addicted. **RoboDroid** is designed to help fill this gap by
-providing a set of tools that can simulate human-like smartphone behavior. The
-pre-defined behaviors are created using [Frida](https://frida.re) and are
-managed in the [RoboDroid Library](https://github.com/cybersecsi/robodroid-
-library) repository. ## â¡ Overview The goal of **RoboDroid** is to provide a
-simple way to introduce mobile components in Cyber Range environments. Its main
-objective is to provide users with an easy-to-use platform that allows them to
-simulate human-like behaviors and actions on mobile devices. RoboDroid
-leverages [Frida](https://frida.re) technology to run behaviors that are
-specific to applications, while using ``ADB`` for all other operations. This
-powerful combination enables users to create workflows of preset behaviors that
-can simulate a mobile user's actions. One example of a workflow that can be
-used in a cyber range environment involves simulating a mobile user receiving a
-phishing email, clicking on the link contained in the email, and subsequently
-downloading a malware. The following picture summarizes it: ![Kill Chain
-Example](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-
-chain-example.png) The workflow can be broken down into the following steps: 1.
-The user receives a phishing email containing a link that appears legitimate.
-2. The user clicks on the link, which redirects them to a malicious website. 3.
-The website prompts the user to download an app, which they do. 4. The app is
-installed on the user's device and begins executing malicious code. 5. The
-malware gains access to sensitive data on the device, such as passwords, credit
-card information, and other personal details. By creating and running workflows
-like this, users can simulate realistic cyber attack scenarios and test their
-defenses against a wide range of threats. This helps to ensure that systems and
-networks are well-protected against potential vulnerabilities, and that users
-are prepared to respond effectively in the event of an attack. ## ð How It
-Works ![How RoboDroid Works](https://raw.githubusercontent.com/cybersecsi/
-robodroid/main/docs/how-it-works.png) ### Interaction with the Frida Agent
-RoboDroid ommunicates with the Frida Agent provided by the RoboDroid Library
-via messages, providing efficient interaction. When the RoboDroid begins a
-specific behavior, it awaits a message from the Frida Agent. The message could
-be of either ``FAILURE`` or ``COMPLETED`` type. If the message type is
-``FAILURE`` RoboDroid restarts the current behavior to ensure successful
-completion. If the message type is ``COMPLETED`` the current step is marked as
-finished, and RoboDroid moves to the next step. Furthermore, a message of type
-``COMPLETED`` can also contain **outputs** that can be used in subsequent
-steps. This ensures that the tool can optimize its behavior to achieve accurate
-simulation of human-like actions on mobile devices. By providing this robust
-communication process, RoboDroid ensures the seamless integration of the Frida
-Agent into its toolset, and facilitates the creation of complex workflows for
-the simulation of mobile devices in a Cyber Range environment. ## ð Install
-You can easily install it by running: ``` pipx install robodroid ``` We suggest
-you to use ``pipx`` instead of ``pip`` because in future Python versions
-package installation with ``pip`` will be removed outside virtual environments.
-### RoboDroid Library **RoboDroid** has built-in support for automatic
-behaviors download (and **soon** auto-update) from the [RoboDroid Library]
-(https://github.com/cybersecsi/robodroid-library) repository. If you want to
-add a new Frida behavior we suggest you to head over to the specific repository
-and make a Pull Request. ## â¹ï¸ Usage ``` robodroid --help ``` This will
-display the help for the tool: ```
-ââââââââââââââââ
-ââââââââââââââââââ
-âââââââââââââââââââââââââââââââââââ
-ââââââââââââââ âââ
-âââââââââââ ââââââââââââââ
-âââ âââââââââââ
-âââââââââââââââââââââââââââââââââââ
-ââââââââââââââââ
-ââââââââââââââââââ RoboDroid v0.0.1 Usage:
-robodroid [OPTIONS] Manage and deploy Android machines with pre-defined
-behaviors for Cyber Range environments â­â Options
-ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+[RoboDroid Library](#robodroid-library) - [â¹ï¸ Usage](#â¹ï¸-usage) -
+[``run`` command](#run-command) - [ENV Variables](#env-variables) - [Run in
+Docker](#run-in-docker) - [ð Demo](#-demo) - [ð§ Roadmap](#-roadmap) -
+[ð Credits](#-credits) - [ðªª License](#-license) ## ð± Context Mobile
+devices have become ubiquitous in today's world. People use smartphones for
+almost every aspect of their lives, including banking, shopping, and
+communication. As a result, mobile devices are now a primary target for
+cybercriminals. However, the security of mobile devices is often overlooked in
+cybersecurity training and testing environments. This can leave organizations
+vulnerable to attacks that exploit the weaknesses of mobile devices. Therefore,
+it is important to introduce mobile components in next-generation cyber-ranges
+to adapt to the current world that is more and more smartphone-addicted.
+**RoboDroid** is designed to help fill this gap by providing a set of tools
+that can simulate human-like smartphone behavior. The pre-defined behaviors are
+created using [Frida](https://frida.re) and are managed in the [RoboDroid
+Library](https://github.com/cybersecsi/robodroid-library) repository. ## â¡
+Overview The goal of **RoboDroid** is to provide a simple way to introduce
+mobile components in Cyber Range environments. Its main objective is to provide
+users with an easy-to-use platform that allows them to simulate human-like
+behaviors and actions on mobile devices. RoboDroid leverages [Frida](https://
+frida.re) technology to run behaviors that are specific to applications, while
+using ``ADB`` for all other operations. This powerful combination enables users
+to create workflows of preset behaviors that can simulate a mobile user's
+actions. One example of a workflow that can be used in a cyber range
+environment involves simulating a mobile user receiving a phishing email,
+clicking on the link contained in the email, and subsequently downloading a
+malware. The following picture summarizes it: ![Kill Chain Example](https://
+raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-chain-
+example.png#gh-light-mode-only) ![Kill Chain Example](https://
+raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-chain-example-
+dark.png#gh-dark-mode-only) The workflow can be broken down into the following
+steps: 1. The user receives a phishing email containing a link that appears
+legitimate. 2. The user clicks on the link, which redirects them to a malicious
+website. 3. The website prompts the user to download an app, which they do. 4.
+The app is installed on the user's device and begins executing malicious code.
+5. The malware gains access to sensitive data on the device, such as passwords,
+credit card information, and other personal details. By creating and running
+workflows like this, users can simulate realistic cyber attack scenarios and
+test their defenses against a wide range of threats. This helps to ensure that
+systems and networks are well-protected against potential vulnerabilities, and
+that users are prepared to respond effectively in the event of an attack. ##
+ð How It Works ![How RoboDroid Works](https://raw.githubusercontent.com/
+cybersecsi/robodroid/main/docs/how-it-works.png#gh-light-mode-only) ![How
+RoboDroid Works](https://raw.githubusercontent.com/cybersecsi/robodroid/main/
+docs/how-it-works-dark.png#gh-dark-mode-only) ### Interaction with the Frida
+Agent RoboDroid ommunicates with the Frida Agent provided by the RoboDroid
+Library via messages, providing efficient interaction. When the RoboDroid
+begins a specific behavior, it awaits a message from the Frida Agent. The
+message could be of either ``FAILURE`` or ``COMPLETED`` type. If the message
+type is ``FAILURE`` RoboDroid restarts the current behavior to ensure
+successful completion. If the message type is ``COMPLETED`` the current step is
+marked as finished, and RoboDroid moves to the next step. Furthermore, a
+message of type ``COMPLETED`` can also contain **outputs** that can be used in
+subsequent steps. This ensures that the tool can optimize its behavior to
+achieve accurate simulation of human-like actions on mobile devices. By
+providing this robust communication process, RoboDroid ensures the seamless
+integration of the Frida Agent into its toolset, and facilitates the creation
+of complex workflows for the simulation of mobile devices in a Cyber Range
+environment. ## ð Install You can easily install it by running: ``` pipx
+install robodroid ``` We suggest you to use ``pipx`` instead of ``pip`` because
+in future Python versions package installation with ``pip`` will be removed
+outside virtual environments. ### RoboDroid Library **RoboDroid** has built-in
+support for automatic behaviors download (and **soon** auto-update) from the
+[RoboDroid Library](https://github.com/cybersecsi/robodroid-library)
+repository. If you want to add a new Frida behavior we suggest you to head over
+to the specific repository and make a Pull Request. ## â¹ï¸ Usage ```
+robodroid --help ``` This will display the help for the tool: ``` &&&&&&&&&&&
+&&&& &&&& &&& &&& (&&&& &&&& &&&& &&&)& &(&&&& &&&&)& &&&& &&&& &&&&&&&&&&&&&
+&&& &&&&&&&&&&&&&&& &&& &&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&&
+&&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&&
+&&&&&&&&&&& &&&& &&&& &&&& &&&& RoboDroid v0.0.2 Usage: robodroid [OPTIONS]
+COMMAND [ARGS]... Manage and deploy Android machines with pre-defined behaviors
+for Cyber Range environments â­â Options
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --help -h Show this message and exit. â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Commands
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â run Run RoboDroid. â | update-library Update the RoboDroid Library to the
+latest version | â version Print the current version and exit. â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ### ``run`` command You can run ``robodroid`` in two different modes: -
+Interactive (``default``) - Managed ``` &&&&&&&&&&& &&&& &&&& &&& &&& (&&&&
+&&&& &&&& &&&)& &(&&&& &&&&)& &&&& &&&& &&&&&&&&&&&&& &&& &&&&&&&&&&&&&&& &&&
+&&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&&
+&&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&& &&&&&&&&&&& &&&& &&&& &&&&
+&&&& RoboDroid v0.0.2 Usage: robodroid run [OPTIONS] Run RoboDroid. â­â
+Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
 â --log-mode [silent|normal|debug] Set logging mode [default: normal] â â
---help -h Show this message and exit. â
-â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
-``` Before actually running it you need to provide at least one valid config
-file that **must** be placed under ``$HOME/.RoboDroid/config`` in ``yaml``
-format. This config file defines all the steps of the workflow that will be
-executed, you can take a look at the ``examples`` folder for some valid
+--mode -m [interactive|managed] Set run mode [default: interactive] â â --
+config -c TEXT Name of the managed config file to load â â --help -h Show
+this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` In the interactive mode there is a prompt that lets the user select the
+``ADB`` host, the port and the device to use while the **managed** mode uses a
+config file that **MUST BE PLACED** under ``$HOME/.RoboDroid/config`` in
+``yaml`` format. The **managed** mode is the perfect mode to use while setting
+up a lab/environment without the need of user input/configuration. The
+following table provides a description of the fields used in the **config**
+file: | **Key** | **Required** | **Description** | |-----------|--------------
+|------------------------------------------------------| | device | True | Info
+about the device to use | | workflow | True | The workflow to use (name of the
+file) | Before actually running it you need to provide at least one valid
+workflow file that **must** be placed under ``$HOME/.RoboDroid/workflows`` in
+``yaml`` format. This config file defines all the steps of the workflow that
+will be executed, you can take a look at the ``examples`` folder for some valid
 configurations. The following table provides a description of the fields used
-in the config file: | **Key** | **Required** | **Description** | |----------|--
-------------|------------------------------------------------------| | id |
-True | The ID of the workflow | | init | False | The init section, contains the
-initial setup actions | | workflow | True | The actual workflow to be executed
-| In the ``init`` section you may set the APKs that must be installed and the
-packages that must be cleaned up (storage and cache) before running the actual
-workflow. The structure of this section is the following: | **Key** |
-**Required** | **Description** | |---------|--------------|--------------------
-------------------------------| | install | True | List of paths of APKs to
-install | | clear | False | List of packages to clean up (storage and cache) |
-In the ``worfklow`` section there is the actual workflow. It is a **list** of
-elements that are called **steps** which are meant to be executed
+in the **workflow** file: | **Key** | **Required** | **Description** | |-------
+----|--------------|------------------------------------------------------| |
+id | True | The ID of the workflow | | init | False | The init section,
+contains the initial setup actions | | behaviors | True | The list of behaviors
+to execute | In the ``init`` section you may set the APKs that must be
+installed and the packages that must be cleaned up (storage and cache) before
+running the actual workflow. The structure of this section is the following: |
+**Key** | **Required** | **Description** | |---------|--------------|----------
+----------------------------------------| | install | True | List of paths of
+APKs to install | | clear | False | List of packages to clean up (storage and
+cache) | In the ``behaviors`` section there is the actual workflow. It is a
+**list** of elements that are called **steps** which are meant to be executed
 **sequentially**. Every *step* has the following structure: | **Key** |
 **Required** | **Description** | |---------|--------------|--------------------
 ---------------------------------------------------------| | id | True | ID of
 the step | | name | True | The name of the behavior (in the RoboDroid Library
 or in the commands list) | | type | True | The type of the behavior ("frida-
 behavior", "adb") | | inputs | False | The list of inputs | Finally every input
 has the following structure: | **Key** | **Required** | **Description** | |----
@@ -117,28 +144,36 @@
 the input | | value | True | The value to assign to this input | The last thing
 to say is that you can **also use outputs from previous steps as input to the
 next ones**. To do that you can set the value of an input by using the
 **reserved** prefix ``robodroid.outputs`` followed by the ID of the step and
 the ID of the output, for example: ``` ... - id: get-link name: k9-mail-
 refresh-and-get-link type: frida - id: open-and-download name: firefox-android-
 open-link-and-download type: frida inputs: - id: link value:
-robodroid.outputs.get-link.link ... ``` ## ð Demo We made a brief demo video
-that shows RoboDroid in action with a template that does the following: 1. Sets
-up and email account on the K9 Mail app 2. Waits indefinitely for a new email
-and returns the first link inside it 3. Opens the link with the Firefox Android
-(Fenix) application, downloads the linked file and installs it This workflow
-simulates a common phishing attack (although simplified) that can be used in a
-next-generation Cyber Range involving Android Mobile Devices. [![RoboDroid
-Introduction](https://img.youtube.com/vi/jn8OQZyNLD4/maxresdefault.jpg)](http:/
-/www.youtube.com/watch?v=jn8OQZyNLD4 "RoboDroid Introduction") ## ð§ Roadmap
-*RoboDroid* is a newborn tool and still needs to grow up! Currently these are
-the features we plan to add very soon: - [ ] Automatic deploy of AVD - [ ]
-Automatic deploy of ReDroid instance - [ ] Automatic deploy of Genymotion
-instance - [ ] Multi-device support - [ ] Interactive mode (without workflow
-config file) - [ ] Continuous workflow mode (restart the whole workflow
-indefinitely until manually stopped) Of course we plan to add more and more
-behaviors in the [RoboDroid Library](https://github.com/cybersecsi/robodroid-
-library) and more and more ``adb`` commands in this repo. We also encourage
-every user to contribute to this projet and make it better! ## ð Credits
-Developed by Angelo Delicato [@SecSI](https://secsi.io) ## ðªª License
-_robodroid_ is released under the [GPL-3.0 LICENSE](https://github.com/
-cybersecsi/robodroid/blob/main/LICENSE)
+robodroid.outputs.get-link.link ... ``` ### ENV Variables The CLI options can
+also be set through env variables (especially useful when running inside
+Docker); the following table provides a list of the current env variables
+available: | **Key** | **Description** | |-------------------------------|-----
+----------------------------------------------------------------------| |
+ROBODROID_LOG_MODE | Log level of RoboDroid [silent|normal|debug] | |
+ROBODROID_RUN_MODE | Run mode [interactive|managed] | |
+ROBODROID_MANAGED_CONFIG_NAME | The name of the managed config to use (while
+running in ``managed`` mode) | ### Run in Docker TODO ## ð Demo We made a
+brief demo video that shows RoboDroid in action with a template that does the
+following: 1. Sets up and email account on the K9 Mail app 2. Waits
+indefinitely for a new email and returns the first link inside it 3. Opens the
+link with the Firefox Android (Fenix) application, downloads the linked file
+and installs it This workflow simulates a common phishing attack (although
+simplified) that can be used in a next-generation Cyber Range involving Android
+Mobile Devices. [![RoboDroid Introduction](https://img.youtube.com/vi/
+jn8OQZyNLD4/maxresdefault.jpg)](http://www.youtube.com/watch?v=jn8OQZyNLD4
+"RoboDroid Introduction") ## ð§ Roadmap *RoboDroid* is a newborn tool and
+still needs to grow up! Currently these are the features we plan to add very
+soon: - [ ] Automatic deploy of AVD - [ ] Automatic deploy of ReDroid instance
+- [ ] Automatic deploy of Genymotion instance - [ ] Multi-device support - [ ]
+~~Interactive~~ Creative mode (without workflow file) - [ ] Continuous workflow
+mode (restart the whole workflow indefinitely until manually stopped) Of course
+we plan to add more and more behaviors in the [RoboDroid Library](https://
+github.com/cybersecsi/robodroid-library) and more and more ``adb`` commands in
+this repo. We also encourage every user to contribute to this projet and make
+it better! ## ð Credits Developed by Angelo Delicato [@SecSI](https://
+secsi.io) ## ðªª License _RoboDroid_ is released under the [GPL-3.0 LICENSE]
+(https://github.com/cybersecsi/robodroid/blob/main/LICENSE)
```

### Comparing `robodroid-0.0.1/pyproject.toml` & `robodroid-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robodroid"
-version = "0.0.1"
+version = "0.0.2"
 description = "Manage and deploy Android machines with pre-defined behaviors for Cyber Range environments"
 authors = ["Angelo Delicato <thelicato@duck.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 exclude = [
     { path = "tests" }
 ]
```

### Comparing `robodroid-0.0.1/robodroid/config/template.yaml` & `robodroid-0.0.2/robodroid/config/template.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-id: Config ID
+id: Workflow ID
 
 init:
   install:
     - Path to the .apk to install
   clear:
     - Package to clean with "pm clear <package-name>"
 
-workflow:
+behaviors:
   - id: ID of the step in this workflow
     name: ID of the script in the RoboDroid library to execute (.e.g. k9-mail-account-setup)
     type: Type of the step (e.g. 'frida-behavior', 'adb')
     inputs:
       - id: input ID
         value: value for this input (use 'robodroid.outputs.<step_id>.<step_output>' to use the outputs of previous steps)
```

### Comparing `robodroid-0.0.1/robodroid/services/adb.py` & `robodroid-0.0.2/robodroid/services/adb.py`

 * *Files 7% similar despite different names*

```diff
@@ -143,7 +143,12 @@
         try:
             result = self.device.root()
         except RuntimeError as exc:
             if "adbd is already running as root" in str(exc):
                 result = True
         self.device.wait_boot_complete()
         return result
+
+    @validate_connection(None)
+    def forward_frida_port(self) -> None:
+        # Default frida port
+        self.device.forward("tcp:27042", "tcp:27042")
```

### Comparing `robodroid-0.0.1/robodroid/services/frida.py` & `robodroid-0.0.2/robodroid/services/frida.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 class RoboDroidFrida:
     """
     A class for interacting with Android devices using 'frida'
     """
 
     def __init__(self, robodroidAdb: adb.RoboDroidAdb):
         self.adb = robodroidAdb
-        self.device = frida.get_usb_device()
+        frida.get_device_manager().add_remote_device(robodroidAdb.host)  # TODO: Check port usage
+        self.device = frida.get_device_matching(lambda d: d.name == robodroidAdb.host)
         self.queue: queue.Queue = queue.Queue()
 
     def get_download_fname(self, arch: str) -> str:
         """
         Depending upon the arch provided, the function returns the filename of the frida-server file.
         """
         base_filename = "frida-server-{}-android-{}.xz"
@@ -90,14 +91,15 @@
             return True
         return False
 
     def start_frida_server(self) -> None:
         frida_server_bin = self.get_frida_server_bin_path()
         if not self.is_frida_server_bin_available():
             self.download_frida_server()
+        self.adb.forward_frida_port()
         self.adb.push(frida_server_bin, "/data/local/tmp/frida-server", 755)
         self.adb.shell_cmd("killall frida-server", False)
         self.adb.thread_shell_cmd("/data/local/tmp/frida-server")
         self.adb.wait_for_process_up("frida-server")
         logger.success("Frida server correctly started")
 
     @retry(stop=stop_after_attempt(10), wait=wait_fixed(1))
```

### Comparing `robodroid-0.0.1/robodroid/tests/assets/InsecureBankv2.apk` & `robodroid-0.0.2/robodroid/tests/assets/InsecureBankv2.apk`

 * *Files identical despite different names*

### Comparing `robodroid-0.0.1/robodroid/tests/test_adb.py` & `robodroid-0.0.2/robodroid/tests/test_adb.py`

 * *Files identical despite different names*

### Comparing `robodroid-0.0.1/robodroid/types/common.py` & `robodroid-0.0.2/robodroid/types/common.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,38 +30,50 @@
 class LibData(TypedDict):
     id: str
     info: LibInfo
     inputs: List[LibInputs]
     outputs: List[LibOutputs]
 
 
-class ConfigInit(TypedDict):
+class WorkflowInit(TypedDict):
     install: List[str]
     clear: List[str]
 
 
-class ConfigStepInput(TypedDict):
+class WorkflowStepInput(TypedDict):
     id: str
     value: str
 
 
-class ConfigStep(TypedDict):
+class WorkflowStep(TypedDict):
     id: str
     name: str
     type: WorkflowStepTypeValue
-    inputs: List[ConfigStepInput]
+    inputs: List[WorkflowStepInput]
 
 
-class ConfigData(TypedDict):
+class WorkflowData(TypedDict):
     id: str
-    init: NotRequired[ConfigInit]
-    workflow: List[ConfigStep]
+    init: NotRequired[WorkflowInit]
+    behaviors: List[WorkflowStep]
 
 
 class BehaviorResult(TypedDict):
     status: BehaviorResultTypeValue
     msg: str
     outputs: NotRequired[str]
 
 
 class DbMetadata(TypedDict):
+    library_version: str  # Current RoboDroid Library version
     last_library_update: int  # UNIX timestamp of the last library update
+
+
+class ManagedConfigDeviceData(TypedDict):
+    adb_host: str
+    adb_port: int
+    device_name: str
+
+
+class ManagedConfigData(TypedDict):
+    device: ManagedConfigDeviceData
+    workflow: str
```

### Comparing `robodroid-0.0.1/robodroid/types/enum.py` & `robodroid-0.0.2/robodroid/types/enum.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from typing import Literal, get_args
 from enum import Enum
 
 # Define the enums as a class
 
 
+class RunMode(str, Enum):
+    INTERACTIVE = "interactive"
+    MANAGED = "managed"
+
+
 class LoggerMode(str, Enum):
     SILENT = "silent"
     NORMAL = "normal"
     DEBUG = "debug"
 
 
 class WorkflowStepType(str, Enum):
@@ -17,15 +22,17 @@
 
 class BehaviorResultType(str, Enum):
     COMPLETED = "completed"
     FAILED = "failed"
 
 
 # Convert to literal
+RunModeValue = Literal["interactive", "managed"]
 LoggerModeValue = Literal["silent", "normal", "debug"]
 WorkflowStepTypeValue = Literal["frida-behavior", "adb"]
 BehaviorResultTypeValue = Literal["completed", "failed"]
 
 # Assert that the conversion is OK
+assert set(get_args(RunModeValue)) == {member.value for member in RunMode}
 assert set(get_args(LoggerModeValue)) == {member.value for member in LoggerMode}
 assert set(get_args(WorkflowStepTypeValue)) == {member.value for member in WorkflowStepType}
 assert set(get_args(BehaviorResultTypeValue)) == {member.value for member in BehaviorResultType}
```

### Comparing `robodroid-0.0.1/robodroid/utils/logger.py` & `robodroid-0.0.2/robodroid/utils/logger.py`

 * *Files identical despite different names*

### Comparing `robodroid-0.0.1/robodroid/utils/schemas.py` & `robodroid-0.0.2/robodroid/utils/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                     "required": True,
                 },
             },
         },
     },
 }
 
-config_schema = {
+workflow_schema = {
     "id": {
         "type": "string",
         "required": True,
     },
     "init": {
         "type": "dict",
         "required": False,
@@ -78,15 +78,15 @@
             },
             "clear": {
                 "type": "list",
                 "required": True,
             },
         },
     },
-    "workflow": {
+    "behaviors": {
         "type": "list",
         "required": True,
         "schema": {
             "type": "dict",
             "required": True,
             "schema": {
                 "id": {"type": "string", "required": True},
@@ -109,7 +109,23 @@
                         },
                     },
                 },
             },
         },
     },
 }
+
+managed_config_schema = {
+    "device": {
+        "type": "dict",
+        "required": True,
+        "schema": {
+            "adb_host": {"type": "string", "required": True},
+            "adb_port": {"type": "number", "required": True},
+            "device_name": {"type": "string", "required": True},
+        },
+    },
+    "workflow": {
+        "type": "string",
+        "required": True,
+    },
+}
```

### Comparing `robodroid-0.0.1/robodroid/workflow/commands.py` & `robodroid-0.0.2/robodroid/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `robodroid-0.0.1/robodroid/workflow/manager.py` & `robodroid-0.0.2/robodroid/workflow/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,37 +6,37 @@
 
 
 class RoboDroidWorkflowManager:
     """
     A class for managing a workflow
     """
 
-    def __init__(self, config_data: types.common.ConfigData, adb_instance: adb.RoboDroidAdb):
-        self.config_data = config_data
+    def __init__(self, workflow_data: types.common.WorkflowData, adb_instance: adb.RoboDroidAdb):
+        self.workflow_data = workflow_data
         self.adb_instance = adb_instance
         is_root_enabled = self.adb_instance.is_root_enabled()
         if not is_root_enabled:
             logger.error("Root is not enabled, restarting adbd as root (it may take a while)...")
             self.adb_instance.enable_root()
         self.frida_instance = frida.RoboDroidFrida(adb_instance)
         self.outputs: Dict[str, Any] = {}
 
     def _run_init(self) -> None:
         # Install packages
-        if not "init" in self.config_data:
+        if not "init" in self.workflow_data:
             return
 
-        for apk in self.config_data["init"]["install"]:
+        for apk in self.workflow_data["init"]["install"]:
             logger.info(f"Installing app from '{apk}'")
             self.adb_instance.install(apk)
-        for package_name in self.config_data["init"]["clear"]:
+        for package_name in self.workflow_data["init"]["clear"]:
             logger.info(f"Cleaning package '{package_name}'")
             self.adb_instance.shell_cmd(f"pm clear {package_name}", False)
 
-    def _run_frida_behavior(self, behavior: types.common.ConfigStep) -> None:
+    def _run_frida_behavior(self, behavior: types.common.WorkflowStep) -> None:
         while True:
             reserved_output = "robodroid.outputs."
             lib_name = behavior["name"]
             inputs = behavior["inputs"]
             input_values: List[str | int] = [i["value"] for i in inputs]
             input_values = [
                 self.outputs[i.split(".")[2]][i.split(".")[3]]
@@ -63,15 +63,15 @@
                 if "outputs" in behavior_result.keys():
                     logger.info(f"Outputs: {behavior_result['outputs']}")
                     self.outputs[behavior["id"]] = behavior_result["outputs"]
                 break
             else:
                 logger.error("Behavior failed, starting over")
 
-    def _run_command(self, step: types.common.ConfigStep) -> None:
+    def _run_command(self, step: types.common.WorkflowStep) -> None:
         command_name = step["name"]
         command_type = step["type"]
         if not command_name in config.workflow_commands[command_type].keys():
             logger.error(f"Unable to find command with id {command_name}")
             return
 
         logger.info(f"Running command '{command_name}'")
@@ -92,15 +92,15 @@
 
     def _run_workflow(self) -> None:
         # TODO: Move this Frida setup steps in a specific function
         self.frida_instance.start_frida_server()
 
         command_types = [types.enum.WorkflowStepType.ADB.value]
         # Run the actual workflow
-        for step in self.config_data["workflow"]:
+        for step in self.workflow_data["behaviors"]:
             if step["type"] == types.enum.WorkflowStepType.FRIDA:
                 self._run_frida_behavior(step)
             elif step["type"] in command_types:
                 self._run_command(step)
             else:
                 logger.error("Unknown step type in Workflow, skipping")
         logger.success("Workflow completed!")
```

### Comparing `robodroid-0.0.1/PKG-INFO` & `robodroid-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robodroid
-Version: 0.0.1
+Version: 0.0.2
 Summary: Manage and deploy Android machines with pre-defined behaviors for Cyber Range environments
 License: GPL-3.0
 Author: Angelo Delicato
 Author-email: thelicato@duck.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -30,16 +30,16 @@
     <img src="https://raw.githubusercontent.com/cybersecsi/robodroid/main/logo.png" alt= "robodroid" width="200px">
 </h1>
 <p align="center">
     <b>RoboDroid</b>
 <p>
 
 <p align="center">
-    <img src="https://github.com/cybersecsi/robodroid/actions/workflows/release.yml/badge.svg"/>
-    <img src="https://github.com/cybersecsi/robodroid/actions/workflows/publish.yml/badge.svg"/>
+    <img src="https://github.com/cybersecsi/robodroid/actions/workflows/release.yaml/badge.svg"/>
+    <img src="https://github.com/cybersecsi/robodroid/actions/workflows/publish.yaml/badge.svg"/>
   <a href="https://github.com/cybersecsi/robodroid/blob/main/README.md"><img src="https://img.shields.io/badge/Documentation-complete-green.svg?style=flat"></a>
   <a href="https://github.com/cybersecsi/robodroid/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-GPL3-blue.svg"></a>
 </p>
 
 RoboDroid is a cutting-edge software tool designed to simplify the process of managing (and **very soon** also deploying) Android machines for usage in Cyber Range environments. With RoboDroid, users can easily set up and customize pre-defined behaviors for their Android machines, allowing them to create complex cyber attack scenarios and test their defenses against a wide range of threats.
 
 <!-- omit in toc -->
@@ -48,14 +48,17 @@
 - [📱 Context](#-context)
 - [⚡ Overview](#-overview)
 - [📚 How It Works](#-how-it-works)
   - [Interaction with the Frida Agent](#interaction-with-the-frida-agent)
 - [🔌 Install](#-install)
   - [RoboDroid Library](#robodroid-library)
 - [ℹ️ Usage](#ℹ️-usage)
+  - [``run`` command](#run-command)
+  - [ENV Variables](#env-variables)
+  - [Run in Docker](#run-in-docker)
 - [🚀 Demo](#-demo)
 - [🚧 Roadmap](#-roadmap)
 - [📚 Credits](#-credits)
 - [🪪 License](#-license)
 
 ## 📱 Context
 Mobile devices have become ubiquitous in today's world. People use smartphones for almost every aspect of their lives, including banking, shopping, and communication. As a result, mobile devices are now a primary target for cybercriminals.
@@ -71,28 +74,30 @@
 
 RoboDroid leverages [Frida](https://frida.re) technology to run behaviors that are specific to applications, while using ``ADB`` for all other operations. This powerful combination enables users to create workflows of preset behaviors that can simulate a mobile user's actions.
 
 One example of a workflow that can be used in a cyber range environment involves simulating a mobile user receiving a phishing email, clicking on the link contained in the email, and subsequently downloading a malware.
 
 The following picture summarizes it:
 
-![Kill Chain Example](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-chain-example.png)
+![Kill Chain Example](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-chain-example.png#gh-light-mode-only)
+![Kill Chain Example](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-chain-example-dark.png#gh-dark-mode-only)
 
 The workflow can be broken down into the following steps:
 
 1. The user receives a phishing email containing a link that appears legitimate.
 2. The user clicks on the link, which redirects them to a malicious website.
 3. The website prompts the user to download an app, which they do.
 4. The app is installed on the user's device and begins executing malicious code.
 5. The malware gains access to sensitive data on the device, such as passwords, credit card information, and other personal details.
 
 By creating and running workflows like this, users can simulate realistic cyber attack scenarios and test their defenses against a wide range of threats. This helps to ensure that systems and networks are well-protected against potential vulnerabilities, and that users are prepared to respond effectively in the event of an attack.
 
 ## 📚 How It Works
-![How RoboDroid Works](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/how-it-works.png)
+![How RoboDroid Works](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/how-it-works.png#gh-light-mode-only)
+![How RoboDroid Works](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/how-it-works-dark.png#gh-dark-mode-only)
 
 ### Interaction with the Frida Agent
 
 RoboDroid ommunicates with the Frida Agent provided by the RoboDroid Library via messages, providing efficient interaction.
 When the RoboDroid begins a specific behavior, it awaits a message from the Frida Agent. The message could be of either ``FAILURE`` or ``COMPLETED`` type.
 
 If the message type is ``FAILURE`` RoboDroid restarts the current behavior to ensure successful completion. If the message type is ``COMPLETED`` the current step is marked as finished, and RoboDroid moves to the next step.
@@ -116,50 +121,107 @@
 ```
 robodroid --help
 ```
 
 This will display the help for the tool:
 
 ```
-    ███████╗███████╗ ██████╗███████╗██╗
-    ██╔════╝██╔════╝██╔════╝██╔════╝██║
-    ███████╗█████╗  ██║     ███████╗██║
-    ╚════██║██╔══╝  ██║     ╚════██║██║
-    ███████║███████╗╚██████╗███████║██║
-    ╚══════╝╚══════╝ ╚═════╝╚══════╝╚═╝
-    RoboDroid v0.0.1
+              &&&&&&&&&&&
+           &&&&         &&&&
+         &&&               &&&
+      (&&&&   &&&&   &&&&   &&&)&
+      &(&&&&               &&&&)&
+          &&&&           &&&&
+             &&&&&&&&&&&&&
+       &&&  &&&&&&&&&&&&&&&  &&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+              &&&&&&&&&&&
+               &&&& &&&&
+               &&&& &&&&
+            RoboDroid v0.0.2
 
-
- Usage: robodroid [OPTIONS]
+ Usage: robodroid [OPTIONS] COMMAND [ARGS]...
 
  Manage and deploy Android machines with pre-defined behaviors for Cyber Range environments
 
-╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --log-mode          [silent|normal|debug]  Set logging mode [default: normal]                                                   │
-│ --help      -h                             Show this message and exit.                                                          │
-╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Options ──────────────────────────────────────────────────────────────────────────────────╮
+│ --help  -h        Show this message and exit.                                              │
+╰────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ─────────────────────────────────────────────────────────────────────────────────╮
+│ run               Run RoboDroid.                                                           │
+| update-library    Update the RoboDroid Library to the latest version                       |
+│ version           Print the current version and exit.                                      │
+╰────────────────────────────────────────────────────────────────────────────────────────────╯
+
 ```
 
-Before actually running it you need to provide at least one valid config file that **must** be placed under ``$HOME/.RoboDroid/config`` in ``yaml`` format.
-This config file defines all the steps of the workflow that will be executed, you can take a look at the ``examples`` folder for some valid configurations. The following table provides a description of the fields used in the config file:
-
-| **Key**  | **Required** | **Description**                                      |
-|----------|--------------|------------------------------------------------------|
-| id       | True         | The ID of the workflow                               |
-| init     | False        | The init section, contains the initial setup actions |
-| workflow | True         | The actual workflow to be executed                   |
+### ``run`` command
+You can run ``robodroid`` in two different modes:
+- Interactive (``default``)
+- Managed
+
+```
+              &&&&&&&&&&&
+           &&&&         &&&&
+         &&&               &&&
+      (&&&&   &&&&   &&&&   &&&)&
+      &(&&&&               &&&&)&
+          &&&&           &&&&
+             &&&&&&&&&&&&&
+       &&&  &&&&&&&&&&&&&&&  &&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+      &&&&  &&&&&&&&&&&&&&&  &&&&
+              &&&&&&&&&&&
+               &&&& &&&&
+               &&&& &&&&
+            RoboDroid v0.0.2
+
+ Usage: robodroid run [OPTIONS]
+
+ Run RoboDroid.
+
+╭─ Options ───────────────────────────────────────────────────────────────────────────╮
+│ --log-mode          [silent|normal|debug]  Set logging mode [default: normal]       │
+│ --mode      -m      [interactive|managed]  Set run mode [default: interactive]      │
+│ --config    -c      TEXT                   Name of the managed config file to load  │
+│ --help      -h                             Show this message and exit.              │
+╰─────────────────────────────────────────────────────────────────────────────────────╯
+```
+
+In the interactive mode there is a prompt that lets the user select the ``ADB`` host, the port and the device to use while the **managed** mode uses a config file that **MUST BE PLACED** under ``$HOME/.RoboDroid/config`` in ``yaml`` format. The **managed** mode is the perfect mode to use while setting up a lab/environment without the need of user input/configuration.
+The following table provides a description of the fields used in the **config** file:
+| **Key**   | **Required** | **Description**                                      |
+|-----------|--------------|------------------------------------------------------|
+| device    | True         | Info about the device to use                         |
+| workflow  | True         | The workflow to use (name of the file)               |
+
+Before actually running it you need to provide at least one valid workflow file that **must** be placed under ``$HOME/.RoboDroid/workflows`` in ``yaml`` format.
+This config file defines all the steps of the workflow that will be executed, you can take a look at the ``examples`` folder for some valid configurations. The following table provides a description of the fields used in the **workflow** file:
+
+| **Key**   | **Required** | **Description**                                      |
+|-----------|--------------|------------------------------------------------------|
+| id        | True         | The ID of the workflow                               |
+| init      | False        | The init section, contains the initial setup actions |
+| behaviors | True         | The list of behaviors to execute                     |
 
 In the ``init`` section you may set the APKs that must be installed and the packages that must be cleaned up (storage and cache) before running the actual workflow. The structure of this section is the following:
 
 | **Key** | **Required** | **Description**                                  |
 |---------|--------------|--------------------------------------------------|
 | install | True         | List of paths of APKs to install                 |
 | clear   | False        | List of packages to clean up (storage and cache) |
 
-In the ``worfklow`` section there is the actual workflow. It is a **list** of elements that are called **steps** which are meant to be executed **sequentially**. Every *step* has the following structure:
+In the ``behaviors`` section there is the actual workflow. It is a **list** of elements that are called **steps** which are meant to be executed **sequentially**. Every *step* has the following structure:
 
 | **Key** | **Required** | **Description**                                                             |
 |---------|--------------|-----------------------------------------------------------------------------|
 | id      | True         | ID of the step                                                              |
 | name    | True         | The name of the behavior (in the RoboDroid Library or in the commands list) |
 | type    | True         | The type of the behavior ("frida-behavior", "adb")                          |
 | inputs  | False        | The list of inputs                                                          |
@@ -182,14 +244,26 @@
     type: frida
     inputs:
       - id: link
         value: robodroid.outputs.get-link.link
 ...
 ```
 
+### ENV Variables
+
+The CLI options can also be set through env variables (especially useful when running inside Docker); the following table provides a list of the current env variables available:
+| **Key**                       | **Description**                                                           |
+|-------------------------------|---------------------------------------------------------------------------|
+| ROBODROID_LOG_MODE            | Log level of RoboDroid [silent|normal|debug]                              |
+| ROBODROID_RUN_MODE            | Run mode [interactive|managed]                                            |
+| ROBODROID_MANAGED_CONFIG_NAME | The name of the managed config to use (while running in ``managed`` mode) |
+
+### Run in Docker
+TODO
+
 ## 🚀 Demo
 
 We made a brief demo video that shows RoboDroid in action with a template that does the following:
 1. Sets up and email account on the K9 Mail app
 2. Waits indefinitely for a new email and returns the first link inside it
 3. Opens the link with the Firefox Android (Fenix) application, downloads the linked file and installs it
 
@@ -200,20 +274,20 @@
 
 ## 🚧 Roadmap
 *RoboDroid* is a newborn tool and still needs to grow up! Currently these are the features we plan to add very soon:
 - [ ] Automatic deploy of AVD
 - [ ] Automatic deploy of ReDroid instance
 - [ ] Automatic deploy of Genymotion instance
 - [ ] Multi-device support
-- [ ] Interactive mode (without workflow config file)
+- [ ] ~~Interactive~~ Creative mode (without workflow file)
 - [ ] Continuous workflow mode (restart the whole workflow indefinitely until manually stopped)
 
 Of course we plan to add more and more behaviors in the [RoboDroid Library](https://github.com/cybersecsi/robodroid-library) and more and more ``adb`` commands in this repo. We also encourage every user to contribute to this projet and make it better!
 
 ## 📚 Credits
 
 Developed by Angelo Delicato [@SecSI](https://secsi.io)
 
 ## 🪪 License
 
-_robodroid_ is released under the [GPL-3.0 LICENSE](https://github.com/cybersecsi/robodroid/blob/main/LICENSE)
+_RoboDroid_ is released under the [GPL-3.0 LICENSE](https://github.com/cybersecsi/robodroid/blob/main/LICENSE)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: robodroid Version: 0.0.1 Summary: Manage and deploy
+Metadata-Version: 2.1 Name: robodroid Version: 0.0.2 Summary: Manage and deploy
 Android machines with pre-defined behaviors for Cyber Range environments
 License: GPL-3.0 Author: Angelo Delicato Author-email: thelicato@duck.com
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cerberus (>=1.3.4,<2.0.0) Requires-Dist: frida
@@ -12,119 +12,146 @@
 Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: tenacity
 (>=8.2.2,<9.0.0) Requires-Dist: typer[all] (>=0.7.0,<0.8.0) Requires-Dist:
 typing-extensions (>=4.5.0,<5.0.0) Requires-Dist: wrapt-timeout-decorator
 (>=1.3.12.2,<2.0.0.0) Description-Content-Type: text/markdown
                                     ******
                               [robodroid] ******
                                    RoboDroid
-    [https://github.com/cybersecsi/robodroid/actions/workflows/release.yml/
+   [https://github.com/cybersecsi/robodroid/actions/workflows/release.yaml/
     badge.svg] [https://github.com/cybersecsi/robodroid/actions/workflows/
- publish.yml/badge.svg] [https://img.shields.io/badge/Documentation-complete-
+ publish.yaml/badge.svg] [https://img.shields.io/badge/Documentation-complete-
   green.svg?style=flat] [https://img.shields.io/badge/License-GPL3-blue.svg]
 RoboDroid is a cutting-edge software tool designed to simplify the process of
 managing (and **very soon** also deploying) Android machines for usage in Cyber
 Range environments. With RoboDroid, users can easily set up and customize pre-
 defined behaviors for their Android machines, allowing them to create complex
 cyber attack scenarios and test their defenses against a wide range of threats.
 ## ð Table of Contents - [ð± Context](#-context) - [â¡ Overview](#-
 overview) - [ð How It Works](#-how-it-works) - [Interaction with the Frida
 Agent](#interaction-with-the-frida-agent) - [ð Install](#-install) -
-[RoboDroid Library](#robodroid-library) - [â¹ï¸ Usage](#â¹ï¸-usage) - [ð
-Demo](#-demo) - [ð§ Roadmap](#-roadmap) - [ð Credits](#-credits) - [ðªª
-License](#-license) ## ð± Context Mobile devices have become ubiquitous in
-today's world. People use smartphones for almost every aspect of their lives,
-including banking, shopping, and communication. As a result, mobile devices are
-now a primary target for cybercriminals. However, the security of mobile
-devices is often overlooked in cybersecurity training and testing environments.
-This can leave organizations vulnerable to attacks that exploit the weaknesses
-of mobile devices. Therefore, it is important to introduce mobile components in
-next-generation cyber-ranges to adapt to the current world that is more and
-more smartphone-addicted. **RoboDroid** is designed to help fill this gap by
-providing a set of tools that can simulate human-like smartphone behavior. The
-pre-defined behaviors are created using [Frida](https://frida.re) and are
-managed in the [RoboDroid Library](https://github.com/cybersecsi/robodroid-
-library) repository. ## â¡ Overview The goal of **RoboDroid** is to provide a
-simple way to introduce mobile components in Cyber Range environments. Its main
-objective is to provide users with an easy-to-use platform that allows them to
-simulate human-like behaviors and actions on mobile devices. RoboDroid
-leverages [Frida](https://frida.re) technology to run behaviors that are
-specific to applications, while using ``ADB`` for all other operations. This
-powerful combination enables users to create workflows of preset behaviors that
-can simulate a mobile user's actions. One example of a workflow that can be
-used in a cyber range environment involves simulating a mobile user receiving a
-phishing email, clicking on the link contained in the email, and subsequently
-downloading a malware. The following picture summarizes it: ![Kill Chain
-Example](https://raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-
-chain-example.png) The workflow can be broken down into the following steps: 1.
-The user receives a phishing email containing a link that appears legitimate.
-2. The user clicks on the link, which redirects them to a malicious website. 3.
-The website prompts the user to download an app, which they do. 4. The app is
-installed on the user's device and begins executing malicious code. 5. The
-malware gains access to sensitive data on the device, such as passwords, credit
-card information, and other personal details. By creating and running workflows
-like this, users can simulate realistic cyber attack scenarios and test their
-defenses against a wide range of threats. This helps to ensure that systems and
-networks are well-protected against potential vulnerabilities, and that users
-are prepared to respond effectively in the event of an attack. ## ð How It
-Works ![How RoboDroid Works](https://raw.githubusercontent.com/cybersecsi/
-robodroid/main/docs/how-it-works.png) ### Interaction with the Frida Agent
-RoboDroid ommunicates with the Frida Agent provided by the RoboDroid Library
-via messages, providing efficient interaction. When the RoboDroid begins a
-specific behavior, it awaits a message from the Frida Agent. The message could
-be of either ``FAILURE`` or ``COMPLETED`` type. If the message type is
-``FAILURE`` RoboDroid restarts the current behavior to ensure successful
-completion. If the message type is ``COMPLETED`` the current step is marked as
-finished, and RoboDroid moves to the next step. Furthermore, a message of type
-``COMPLETED`` can also contain **outputs** that can be used in subsequent
-steps. This ensures that the tool can optimize its behavior to achieve accurate
-simulation of human-like actions on mobile devices. By providing this robust
-communication process, RoboDroid ensures the seamless integration of the Frida
-Agent into its toolset, and facilitates the creation of complex workflows for
-the simulation of mobile devices in a Cyber Range environment. ## ð Install
-You can easily install it by running: ``` pipx install robodroid ``` We suggest
-you to use ``pipx`` instead of ``pip`` because in future Python versions
-package installation with ``pip`` will be removed outside virtual environments.
-### RoboDroid Library **RoboDroid** has built-in support for automatic
-behaviors download (and **soon** auto-update) from the [RoboDroid Library]
-(https://github.com/cybersecsi/robodroid-library) repository. If you want to
-add a new Frida behavior we suggest you to head over to the specific repository
-and make a Pull Request. ## â¹ï¸ Usage ``` robodroid --help ``` This will
-display the help for the tool: ```
-ââââââââââââââââ
-ââââââââââââââââââ
-âââââââââââââââââââââââââââââââââââ
-ââââââââââââââ âââ
-âââââââââââ ââââââââââââââ
-âââ âââââââââââ
-âââââââââââââââââââââââââââââââââââ
-ââââââââââââââââ
-ââââââââââââââââââ RoboDroid v0.0.1 Usage:
-robodroid [OPTIONS] Manage and deploy Android machines with pre-defined
-behaviors for Cyber Range environments â­â Options
-ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+[RoboDroid Library](#robodroid-library) - [â¹ï¸ Usage](#â¹ï¸-usage) -
+[``run`` command](#run-command) - [ENV Variables](#env-variables) - [Run in
+Docker](#run-in-docker) - [ð Demo](#-demo) - [ð§ Roadmap](#-roadmap) -
+[ð Credits](#-credits) - [ðªª License](#-license) ## ð± Context Mobile
+devices have become ubiquitous in today's world. People use smartphones for
+almost every aspect of their lives, including banking, shopping, and
+communication. As a result, mobile devices are now a primary target for
+cybercriminals. However, the security of mobile devices is often overlooked in
+cybersecurity training and testing environments. This can leave organizations
+vulnerable to attacks that exploit the weaknesses of mobile devices. Therefore,
+it is important to introduce mobile components in next-generation cyber-ranges
+to adapt to the current world that is more and more smartphone-addicted.
+**RoboDroid** is designed to help fill this gap by providing a set of tools
+that can simulate human-like smartphone behavior. The pre-defined behaviors are
+created using [Frida](https://frida.re) and are managed in the [RoboDroid
+Library](https://github.com/cybersecsi/robodroid-library) repository. ## â¡
+Overview The goal of **RoboDroid** is to provide a simple way to introduce
+mobile components in Cyber Range environments. Its main objective is to provide
+users with an easy-to-use platform that allows them to simulate human-like
+behaviors and actions on mobile devices. RoboDroid leverages [Frida](https://
+frida.re) technology to run behaviors that are specific to applications, while
+using ``ADB`` for all other operations. This powerful combination enables users
+to create workflows of preset behaviors that can simulate a mobile user's
+actions. One example of a workflow that can be used in a cyber range
+environment involves simulating a mobile user receiving a phishing email,
+clicking on the link contained in the email, and subsequently downloading a
+malware. The following picture summarizes it: ![Kill Chain Example](https://
+raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-chain-
+example.png#gh-light-mode-only) ![Kill Chain Example](https://
+raw.githubusercontent.com/cybersecsi/robodroid/main/docs/kill-chain-example-
+dark.png#gh-dark-mode-only) The workflow can be broken down into the following
+steps: 1. The user receives a phishing email containing a link that appears
+legitimate. 2. The user clicks on the link, which redirects them to a malicious
+website. 3. The website prompts the user to download an app, which they do. 4.
+The app is installed on the user's device and begins executing malicious code.
+5. The malware gains access to sensitive data on the device, such as passwords,
+credit card information, and other personal details. By creating and running
+workflows like this, users can simulate realistic cyber attack scenarios and
+test their defenses against a wide range of threats. This helps to ensure that
+systems and networks are well-protected against potential vulnerabilities, and
+that users are prepared to respond effectively in the event of an attack. ##
+ð How It Works ![How RoboDroid Works](https://raw.githubusercontent.com/
+cybersecsi/robodroid/main/docs/how-it-works.png#gh-light-mode-only) ![How
+RoboDroid Works](https://raw.githubusercontent.com/cybersecsi/robodroid/main/
+docs/how-it-works-dark.png#gh-dark-mode-only) ### Interaction with the Frida
+Agent RoboDroid ommunicates with the Frida Agent provided by the RoboDroid
+Library via messages, providing efficient interaction. When the RoboDroid
+begins a specific behavior, it awaits a message from the Frida Agent. The
+message could be of either ``FAILURE`` or ``COMPLETED`` type. If the message
+type is ``FAILURE`` RoboDroid restarts the current behavior to ensure
+successful completion. If the message type is ``COMPLETED`` the current step is
+marked as finished, and RoboDroid moves to the next step. Furthermore, a
+message of type ``COMPLETED`` can also contain **outputs** that can be used in
+subsequent steps. This ensures that the tool can optimize its behavior to
+achieve accurate simulation of human-like actions on mobile devices. By
+providing this robust communication process, RoboDroid ensures the seamless
+integration of the Frida Agent into its toolset, and facilitates the creation
+of complex workflows for the simulation of mobile devices in a Cyber Range
+environment. ## ð Install You can easily install it by running: ``` pipx
+install robodroid ``` We suggest you to use ``pipx`` instead of ``pip`` because
+in future Python versions package installation with ``pip`` will be removed
+outside virtual environments. ### RoboDroid Library **RoboDroid** has built-in
+support for automatic behaviors download (and **soon** auto-update) from the
+[RoboDroid Library](https://github.com/cybersecsi/robodroid-library)
+repository. If you want to add a new Frida behavior we suggest you to head over
+to the specific repository and make a Pull Request. ## â¹ï¸ Usage ```
+robodroid --help ``` This will display the help for the tool: ``` &&&&&&&&&&&
+&&&& &&&& &&& &&& (&&&& &&&& &&&& &&&)& &(&&&& &&&&)& &&&& &&&& &&&&&&&&&&&&&
+&&& &&&&&&&&&&&&&&& &&& &&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&&
+&&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&&
+&&&&&&&&&&& &&&& &&&& &&&& &&&& RoboDroid v0.0.2 Usage: robodroid [OPTIONS]
+COMMAND [ARGS]... Manage and deploy Android machines with pre-defined behaviors
+for Cyber Range environments â­â Options
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â --help -h Show this message and exit. â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+â­â Commands
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
+â run Run RoboDroid. â | update-library Update the RoboDroid Library to the
+latest version | â version Print the current version and exit. â
+â°âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` ### ``run`` command You can run ``robodroid`` in two different modes: -
+Interactive (``default``) - Managed ``` &&&&&&&&&&& &&&& &&&& &&& &&& (&&&&
+&&&& &&&& &&&)& &(&&&& &&&&)& &&&& &&&& &&&&&&&&&&&&& &&& &&&&&&&&&&&&&&& &&&
+&&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&&
+&&&& &&&&&&&&&&&&&&& &&&& &&&& &&&&&&&&&&&&&&& &&&& &&&&&&&&&&& &&&& &&&& &&&&
+&&&& RoboDroid v0.0.2 Usage: robodroid run [OPTIONS] Run RoboDroid. â­â
+Options
+ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
 â --log-mode [silent|normal|debug] Set logging mode [default: normal] â â
---help -h Show this message and exit. â
-â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
-``` Before actually running it you need to provide at least one valid config
-file that **must** be placed under ``$HOME/.RoboDroid/config`` in ``yaml``
-format. This config file defines all the steps of the workflow that will be
-executed, you can take a look at the ``examples`` folder for some valid
+--mode -m [interactive|managed] Set run mode [default: interactive] â â --
+config -c TEXT Name of the managed config file to load â â --help -h Show
+this message and exit. â
+â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
+``` In the interactive mode there is a prompt that lets the user select the
+``ADB`` host, the port and the device to use while the **managed** mode uses a
+config file that **MUST BE PLACED** under ``$HOME/.RoboDroid/config`` in
+``yaml`` format. The **managed** mode is the perfect mode to use while setting
+up a lab/environment without the need of user input/configuration. The
+following table provides a description of the fields used in the **config**
+file: | **Key** | **Required** | **Description** | |-----------|--------------
+|------------------------------------------------------| | device | True | Info
+about the device to use | | workflow | True | The workflow to use (name of the
+file) | Before actually running it you need to provide at least one valid
+workflow file that **must** be placed under ``$HOME/.RoboDroid/workflows`` in
+``yaml`` format. This config file defines all the steps of the workflow that
+will be executed, you can take a look at the ``examples`` folder for some valid
 configurations. The following table provides a description of the fields used
-in the config file: | **Key** | **Required** | **Description** | |----------|--
-------------|------------------------------------------------------| | id |
-True | The ID of the workflow | | init | False | The init section, contains the
-initial setup actions | | workflow | True | The actual workflow to be executed
-| In the ``init`` section you may set the APKs that must be installed and the
-packages that must be cleaned up (storage and cache) before running the actual
-workflow. The structure of this section is the following: | **Key** |
-**Required** | **Description** | |---------|--------------|--------------------
-------------------------------| | install | True | List of paths of APKs to
-install | | clear | False | List of packages to clean up (storage and cache) |
-In the ``worfklow`` section there is the actual workflow. It is a **list** of
-elements that are called **steps** which are meant to be executed
+in the **workflow** file: | **Key** | **Required** | **Description** | |-------
+----|--------------|------------------------------------------------------| |
+id | True | The ID of the workflow | | init | False | The init section,
+contains the initial setup actions | | behaviors | True | The list of behaviors
+to execute | In the ``init`` section you may set the APKs that must be
+installed and the packages that must be cleaned up (storage and cache) before
+running the actual workflow. The structure of this section is the following: |
+**Key** | **Required** | **Description** | |---------|--------------|----------
+----------------------------------------| | install | True | List of paths of
+APKs to install | | clear | False | List of packages to clean up (storage and
+cache) | In the ``behaviors`` section there is the actual workflow. It is a
+**list** of elements that are called **steps** which are meant to be executed
 **sequentially**. Every *step* has the following structure: | **Key** |
 **Required** | **Description** | |---------|--------------|--------------------
 ---------------------------------------------------------| | id | True | ID of
 the step | | name | True | The name of the behavior (in the RoboDroid Library
 or in the commands list) | | type | True | The type of the behavior ("frida-
 behavior", "adb") | | inputs | False | The list of inputs | Finally every input
 has the following structure: | **Key** | **Required** | **Description** | |----
@@ -132,28 +159,36 @@
 the input | | value | True | The value to assign to this input | The last thing
 to say is that you can **also use outputs from previous steps as input to the
 next ones**. To do that you can set the value of an input by using the
 **reserved** prefix ``robodroid.outputs`` followed by the ID of the step and
 the ID of the output, for example: ``` ... - id: get-link name: k9-mail-
 refresh-and-get-link type: frida - id: open-and-download name: firefox-android-
 open-link-and-download type: frida inputs: - id: link value:
-robodroid.outputs.get-link.link ... ``` ## ð Demo We made a brief demo video
-that shows RoboDroid in action with a template that does the following: 1. Sets
-up and email account on the K9 Mail app 2. Waits indefinitely for a new email
-and returns the first link inside it 3. Opens the link with the Firefox Android
-(Fenix) application, downloads the linked file and installs it This workflow
-simulates a common phishing attack (although simplified) that can be used in a
-next-generation Cyber Range involving Android Mobile Devices. [![RoboDroid
-Introduction](https://img.youtube.com/vi/jn8OQZyNLD4/maxresdefault.jpg)](http:/
-/www.youtube.com/watch?v=jn8OQZyNLD4 "RoboDroid Introduction") ## ð§ Roadmap
-*RoboDroid* is a newborn tool and still needs to grow up! Currently these are
-the features we plan to add very soon: - [ ] Automatic deploy of AVD - [ ]
-Automatic deploy of ReDroid instance - [ ] Automatic deploy of Genymotion
-instance - [ ] Multi-device support - [ ] Interactive mode (without workflow
-config file) - [ ] Continuous workflow mode (restart the whole workflow
-indefinitely until manually stopped) Of course we plan to add more and more
-behaviors in the [RoboDroid Library](https://github.com/cybersecsi/robodroid-
-library) and more and more ``adb`` commands in this repo. We also encourage
-every user to contribute to this projet and make it better! ## ð Credits
-Developed by Angelo Delicato [@SecSI](https://secsi.io) ## ðªª License
-_robodroid_ is released under the [GPL-3.0 LICENSE](https://github.com/
-cybersecsi/robodroid/blob/main/LICENSE)
+robodroid.outputs.get-link.link ... ``` ### ENV Variables The CLI options can
+also be set through env variables (especially useful when running inside
+Docker); the following table provides a list of the current env variables
+available: | **Key** | **Description** | |-------------------------------|-----
+----------------------------------------------------------------------| |
+ROBODROID_LOG_MODE | Log level of RoboDroid [silent|normal|debug] | |
+ROBODROID_RUN_MODE | Run mode [interactive|managed] | |
+ROBODROID_MANAGED_CONFIG_NAME | The name of the managed config to use (while
+running in ``managed`` mode) | ### Run in Docker TODO ## ð Demo We made a
+brief demo video that shows RoboDroid in action with a template that does the
+following: 1. Sets up and email account on the K9 Mail app 2. Waits
+indefinitely for a new email and returns the first link inside it 3. Opens the
+link with the Firefox Android (Fenix) application, downloads the linked file
+and installs it This workflow simulates a common phishing attack (although
+simplified) that can be used in a next-generation Cyber Range involving Android
+Mobile Devices. [![RoboDroid Introduction](https://img.youtube.com/vi/
+jn8OQZyNLD4/maxresdefault.jpg)](http://www.youtube.com/watch?v=jn8OQZyNLD4
+"RoboDroid Introduction") ## ð§ Roadmap *RoboDroid* is a newborn tool and
+still needs to grow up! Currently these are the features we plan to add very
+soon: - [ ] Automatic deploy of AVD - [ ] Automatic deploy of ReDroid instance
+- [ ] Automatic deploy of Genymotion instance - [ ] Multi-device support - [ ]
+~~Interactive~~ Creative mode (without workflow file) - [ ] Continuous workflow
+mode (restart the whole workflow indefinitely until manually stopped) Of course
+we plan to add more and more behaviors in the [RoboDroid Library](https://
+github.com/cybersecsi/robodroid-library) and more and more ``adb`` commands in
+this repo. We also encourage every user to contribute to this projet and make
+it better! ## ð Credits Developed by Angelo Delicato [@SecSI](https://
+secsi.io) ## ðªª License _RoboDroid_ is released under the [GPL-3.0 LICENSE]
+(https://github.com/cybersecsi/robodroid/blob/main/LICENSE)
```

