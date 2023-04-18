# Comparing `tmp/poectrl-0.3.0.tar.gz` & `tmp/poectrl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poectrl-0.3.0.tar", max compression
+gzip compressed data, was "poectrl-0.4.0.tar", max compression
```

## Comparing `poectrl-0.3.0.tar` & `poectrl-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2022-12-13 13:10:09.884351 poectrl-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     5496 2022-12-26 18:52:39.232609 poectrl-0.3.0/README.md
--rw-r--r--   0        0        0        0 2022-12-13 17:24:57.939711 poectrl-0.3.0/poectrl/__init__.py
--rw-r--r--   0        0        0        0 2022-12-26 18:52:39.232609 poectrl-0.3.0/poectrl/api/__init__.py
--rw-r--r--   0        0        0      386 2022-12-26 18:52:39.232609 poectrl-0.3.0/poectrl/api/main.py
--rw-r--r--   0        0        0     2024 2022-12-26 18:52:39.232609 poectrl-0.3.0/poectrl/api/managers/PoE.py
--rw-r--r--   0        0        0        0 2022-12-26 18:52:39.232609 poectrl-0.3.0/poectrl/api/resources/__init__.py
--rw-r--r--   0        0        0      773 2022-12-26 18:52:39.232609 poectrl-0.3.0/poectrl/api/resources/control.py
--rw-r--r--   0        0        0      227 2022-12-26 18:52:39.232609 poectrl-0.3.0/poectrl/api/resources/home.py
--rw-r--r--   0        0        0        0 2022-12-26 18:52:39.232609 poectrl-0.3.0/poectrl/api/schemas/__init__.py
--rw-r--r--   0        0        0      543 2022-12-26 18:52:39.236609 poectrl-0.3.0/poectrl/api/schemas/base.py
--rw-r--r--   0        0        0        0 2022-12-26 18:52:39.236609 poectrl-0.3.0/poectrl/api/schemas/request/__init__.py
--rw-r--r--   0        0        0        0 2022-12-26 18:52:39.236609 poectrl-0.3.0/poectrl/api/schemas/response/__init__.py
--rw-r--r--   0        0        0      295 2022-12-26 18:52:39.236609 poectrl-0.3.0/poectrl/api/schemas/response/poe.py
--rw-r--r--   0        0        0      671 2022-12-26 18:52:39.236609 poectrl-0.3.0/poectrl/api/settings.py
--rw-r--r--   0        0        0     6982 2022-12-26 18:52:39.236609 poectrl-0.3.0/poectrl/base.py
--rw-r--r--   0        0        0     4001 2022-12-26 18:52:39.236609 poectrl-0.3.0/poectrl/cliapp.py
--rw-r--r--   0        0        0      906 2022-12-13 17:24:57.943711 poectrl-0.3.0/poectrl/errors.py
--rwxr-xr-x   0        0        0      725 2022-12-26 18:52:39.236609 poectrl-0.3.0/poectrl/main.py
--rw-r--r--   0        0        0     2629 2022-12-26 18:52:39.236609 poectrl-0.3.0/poectrl/profiles.py
--rw-r--r--   0        0        0     2077 2022-12-13 17:24:57.943711 poectrl-0.3.0/poectrl/sshwrapper.py
--rw-r--r--   0        0        0     1418 2022-12-26 18:52:39.236609 poectrl-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6683 1970-01-01 00:00:00.000000 poectrl-0.3.0/setup.py
--rw-r--r--   0        0        0     6978 1970-01-01 00:00:00.000000 poectrl-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-12-13 13:10:09.884351 poectrl-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     5633 2023-04-18 15:00:31.673931 poectrl-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-13 17:24:57.939711 poectrl-0.4.0/poectrl/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-26 18:52:39.232609 poectrl-0.4.0/poectrl/api/__init__.py
+-rw-r--r--   0        0        0      386 2022-12-26 18:52:39.232609 poectrl-0.4.0/poectrl/api/main.py
+-rw-r--r--   0        0        0     2024 2022-12-26 18:52:39.232609 poectrl-0.4.0/poectrl/api/managers/PoE.py
+-rw-r--r--   0        0        0        0 2022-12-26 18:52:39.232609 poectrl-0.4.0/poectrl/api/resources/__init__.py
+-rw-r--r--   0        0        0      773 2022-12-26 18:52:39.232609 poectrl-0.4.0/poectrl/api/resources/control.py
+-rw-r--r--   0        0        0      227 2022-12-26 18:52:39.232609 poectrl-0.4.0/poectrl/api/resources/home.py
+-rw-r--r--   0        0        0        0 2022-12-26 18:52:39.232609 poectrl-0.4.0/poectrl/api/schemas/__init__.py
+-rw-r--r--   0        0        0      543 2022-12-26 18:52:39.236609 poectrl-0.4.0/poectrl/api/schemas/base.py
+-rw-r--r--   0        0        0        0 2022-12-26 18:52:39.236609 poectrl-0.4.0/poectrl/api/schemas/request/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-26 18:52:39.236609 poectrl-0.4.0/poectrl/api/schemas/response/__init__.py
+-rw-r--r--   0        0        0      295 2022-12-26 18:52:39.236609 poectrl-0.4.0/poectrl/api/schemas/response/poe.py
+-rw-r--r--   0        0        0      671 2022-12-26 18:52:39.236609 poectrl-0.4.0/poectrl/api/settings.py
+-rw-r--r--   0        0        0     6982 2022-12-26 18:52:39.236609 poectrl-0.4.0/poectrl/base.py
+-rw-r--r--   0        0        0     4071 2023-04-18 15:01:12.313659 poectrl-0.4.0/poectrl/cliapp.py
+-rw-r--r--   0        0        0      906 2022-12-13 17:24:57.943711 poectrl-0.4.0/poectrl/errors.py
+-rwxr-xr-x   0        0        0      751 2023-04-18 14:55:55.659772 poectrl-0.4.0/poectrl/main.py
+-rw-r--r--   0        0        0     2629 2022-12-26 18:52:39.236609 poectrl-0.4.0/poectrl/profiles.py
+-rw-r--r--   0        0        0     2077 2022-12-13 17:24:57.943711 poectrl-0.4.0/poectrl/sshwrapper.py
+-rw-r--r--   0        0        0     1432 2023-04-18 15:04:47.388222 poectrl-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 poectrl-0.4.0/setup.py
+-rw-r--r--   0        0        0     7107 1970-01-01 00:00:00.000000 poectrl-0.4.0/PKG-INFO
```

### Comparing `poectrl-0.3.0/LICENSE.txt` & `poectrl-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `poectrl-0.3.0/README.md` & `poectrl-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -147,14 +147,17 @@
 There are a couple of command-line switches you can use :
 
 `---refresh` - This is useful if you are modifiying or troubleshooting the code,
 the API will reload after each source code change.
 
 `--port <int>` - Change the port that the API listens on (default is 8000)
 
+`--host` - binds to all network interfaces on the host, allowing access from
+other machines using the public IP address of this machine
+
 After this, you can access the API on `http://localhost:8000`. Swagger docs are
 available at `http://localhost:8000/docs`
 
 #### API Routes
 
 There are currently 3 routes which correspond to the same command in the CLI.
```

### Comparing `poectrl-0.3.0/poectrl/api/managers/PoE.py` & `poectrl-0.4.0/poectrl/api/managers/PoE.py`

 * *Files identical despite different names*

### Comparing `poectrl-0.3.0/poectrl/api/resources/control.py` & `poectrl-0.4.0/poectrl/api/resources/control.py`

 * *Files identical despite different names*

### Comparing `poectrl-0.3.0/poectrl/api/schemas/base.py` & `poectrl-0.4.0/poectrl/api/schemas/base.py`

 * *Files identical despite different names*

### Comparing `poectrl-0.3.0/poectrl/api/settings.py` & `poectrl-0.4.0/poectrl/api/settings.py`

 * *Files identical despite different names*

### Comparing `poectrl-0.3.0/poectrl/base.py` & `poectrl-0.4.0/poectrl/base.py`

 * *Files identical despite different names*

### Comparing `poectrl-0.3.0/poectrl/cliapp.py` & `poectrl-0.4.0/poectrl/cliapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,13 +119,15 @@
         """Apply the specified profile.
 
         Turn PoE ports on/off depending on the settings in the Profile.
         """
         this_profile = self.get_profile(profile_name)
         self.activate_profile(this_profile)
 
-    def serve(self, reload: bool, port: int):
-        """Run the API server using 'gunicorn'."""
+    def serve(self, reload: bool, port: int, host: bool):
+        """Run the API server using 'uvicorn'."""
         cmd_line = f"uvicorn poectrl.api.main:app --port={port}"
         if reload:
             cmd_line += " --reload"
+        if host:
+            cmd_line += " --host 0.0.0.0"
         subprocess.call(cmd_line, shell=True)
```

### Comparing `poectrl-0.3.0/poectrl/errors.py` & `poectrl-0.4.0/poectrl/errors.py`

 * *Files identical despite different names*

### Comparing `poectrl-0.3.0/poectrl/main.py` & `poectrl-0.4.0/poectrl/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,14 @@
 @app.command()
 def list():
     """List all profiles."""
     cliapp.list()
 
 
 @app.command()
-def serve(reload: bool = False, port: int = 8000):
+def serve(reload: bool = False, port: int = 8000, host: bool = False):
     """Run a server to provide API access."""
-    cliapp.serve(reload, port)
+    cliapp.serve(reload, port, host)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `poectrl-0.3.0/poectrl/profiles.py` & `poectrl-0.4.0/poectrl/profiles.py`

 * *Files identical despite different names*

### Comparing `poectrl-0.3.0/poectrl/sshwrapper.py` & `poectrl-0.4.0/poectrl/sshwrapper.py`

 * *Files identical despite different names*

### Comparing `poectrl-0.3.0/pyproject.toml` & `poectrl-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poectrl"
-version = "0.3.0"
+version = "0.4.0"
 description = "Control PoE status on select Ubiquiti switches"
 license = "MIT"
 authors = ["Grant Ramsay <seapagan@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/seapagan/ts-8-pro-control"
 homepage = "https://github.com/seapagan/ts-8-pro-control"
 classifiers = [
@@ -27,22 +27,22 @@
 
 
 [tool.poetry.scripts]
 poectrl = "poectrl.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.7.2,<4.0"
-paramiko = "^2.12.0"
+paramiko = ">=2.12,<4.0"
 typer = { extras = ["all"], version = "^0.7.0" }
-fastapi = {extras = ["all"], version = "^0.88.0"}
+fastapi = {extras = ["all"], version = ">=0.88,<0.96"}
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^5.0.4"
-black = "^22.10.0"
+black = ">=22.10,<24.0"
 flake8-docstrings = "^1.6.0"
 pydocstyle = "^6.1.1"
 pep8-naming = "^0.13.2"
 pylint = "^2.15.5"
 
 
 [build-system]
```

### Comparing `poectrl-0.3.0/setup.py` & `poectrl-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,24 @@
  'poectrl.api.schemas.request',
  'poectrl.api.schemas.response']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi[all]>=0.88.0,<0.89.0',
- 'paramiko>=2.12.0,<3.0.0',
- 'typer[all]>=0.7.0,<0.8.0']
+['fastapi[all]>=0.88,<0.96', 'paramiko>=2.12,<4.0', 'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['poectrl = poectrl.main:app']}
 
 setup_kwargs = {
     'name': 'poectrl',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Control PoE status on select Ubiquiti switches',
-    'long_description': '# Control PoE status on a Ubiquiti TS-8-Pro Switch <!-- omit in toc -->\n\n[![PyPI version](https://badge.fury.io/py/poectrl.svg)](https://badge.fury.io/py/poectrl)\n\n**Development work** for a system to remotely and automatically control the PoE\nstatus of individual ports on multiple Ubiquiti TS-8-Pro Switch, using\npredefined profiles.\n\nThis has currently only been tested on the TS-8-PRO ToughSwitch routers,\nthough others will be added soon.\n\n**IMPORTANT: This library DOES NOT (and CAN NOT) ensure that any device attached\nto a port is compatible with the voltage selected. BE VERY CAREFUL that you\nchoose the correct voltage for your devices or you can DAMAGE THEM. No\nresponsibility is taken for equipment damaged using this library.**\n\n- [Status](#status)\n- [Use Cases](#use-cases)\n- [Installation](#installation)\n- [Configuration](#configuration)\n- [Usage](#usage)\n  - [As a command-line program](#as-a-command-line-program)\n  - [As an API](#as-an-api)\n    - [API Routes](#api-routes)\n- [Development Plans](#development-plans)\n- [Contributing](#contributing)\n\n## Status\n\nThis project is in no way ready to be used, and documentation is non-existent.\nSee the Development Plans below. Until I have a stable useful interface, check\nthe source code if you are interested 😃\n\n## Use Cases\n\n- Control a set of PoE-powered IP cameras, switches and access points to allow\ndisabling when not needed or quick enabling if required.\n\n## Installation\n\nThe latest version is uploaded to [pypi.org](https://pypi.org) so you can\ninstall this the same as any other package:\n\n```console\npip install poectrl\n```\n\n## Configuration\n\n**IMPORTANT : The configuration layout has CHANGED from version 1.2.0. If you\nare using config files from previous versions you will need to update the\n"devices" section to fit the below schema and change the profile to point to the\nname instead of IP address.**\n\nThe program is configured using a `poectrl.json` file either in the current\nworking directory (first priority) or the user\'s home directory. This is a\nsimple file that describes all devices and profiles. There is an example in\n[poectrl-example.json](poectrl-example.json) :\n\n```json\n{\n  "devices": {\n    "switch_1": {"ip": "192.168.0.187", "user": "ubnt", "password": "ubnt"},\n    "switch_2": {"ip": "192.168.0.190", "user": "ubnt", "password": "ubnt"}\n  },\n  "profiles": {\n    "cctv_on": {\n      "switch_1": {"4": 24, "5": 24, "8": 48},\n      "switch_2": {"5": 24, "6": 24, "7": 48}\n    },\n    "cctv_off": {\n      "switch_1": {"4": 0, "5": 0, "8": 0},\n      "switch_2": {"5": 0, "6": 0, "7": 0}\n    }\n  }\n}\n\n```\n\n## Usage\n\n### As a command-line program\n\nApply a predefined profile, setting the PoE port voltages.\n\n```console\n$ poectrl apply cctv_off\nUsing configuration from /home/seapagan/data/work/own/poectrl/poectrl.json\nConncting to switch_1 (192.168.0.187):\n  Setting port 4 to 0V\n  Setting port 5 to 0V\n  Setting port 8 to 0V\nConncting to switch_2 (192.168.0.190):\n  Setting port 5 to 0V\n  Setting port 6 to 0V\n  Setting port 7 to 0V\n\n```\n\nList all defined profiles:\n\n```console\n$ poectrl list\nUsing configuration from /home/seapagan/data/work/own/ts-8-pro-control/poectrl.json\n\nValid profiles are :\n - cctv_on\n - cctv_off\n```\n\nShow settings for a profile :\n\n```console\n$ poectrl show cctv_off\nUsing configuration from /home/seapagan/data/work/own/ts-8-pro-control/poectrl.json\n{\n    "switch_1": {\n        "4": 0,\n        "5": 0,\n        "8": 0\n    },\n    "switch_2": {\n        "5": 0,\n        "6": 0,\n        "7": 0\n    }\n}\n```\n\n### As an API\n\nIt is also possible to run this locally as an API, which can then allow easier\ncontrol using a web browser.\n\n**Important**: This is only designed for local network use, not over the\ninternet since there is NO access control set up. If you open this to the\ninternet then ANYONE can control your PoE!\n\n```console\n$ poectrl serve\nINFO:     Started server process [49922]\nINFO:     Waiting for application startup.\nINFO:     Application startup complete.\nINFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)\n```\n\nThere are a couple of command-line switches you can use :\n\n`---refresh` - This is useful if you are modifiying or troubleshooting the code,\nthe API will reload after each source code change.\n\n`--port <int>` - Change the port that the API listens on (default is 8000)\n\nAfter this, you can access the API on `http://localhost:8000`. Swagger docs are\navailable at `http://localhost:8000/docs`\n\n#### API Routes\n\nThere are currently 3 routes which correspond to the same command in the CLI.\n\n`/list/` - Lists all the defined profiles\\\n`/show/{profile_name}` - Shows details for the specific profile\\\n`/apply/{profile_name}` - Apply the specific profile\n\n## Development Plans\n\nCurrent proposed project plan.\n\n- [x] Write proof-of-concept code to control ports.\n- [x] Refactor and tidy the above code into a Library Class.\n- [x] Create a basic CLI using this Library\n- [x] Continue the CLI to use a config file, show current values, list profiles\n  etc.\n- [x] Publish on PyPi as a standalone package.\n- [x] Wrap this into an API (using FastAPI) for local use only.\n- [ ] Create a Web App to interface with the above API.\n\n## Contributing\n\nAt this time, the project is barely in it\'s planning stage but I do have a firm\nidea where it\'s going and how to structure it. As such, other contributions are\nnot looked for at this time. Hopefully, within a few days this project will be\nat a much more advanced stage and that will change 😃.\n',
+    'long_description': '# Control PoE status on a Ubiquiti TS-8-Pro Switch <!-- omit in toc -->\n\n[![PyPI version](https://badge.fury.io/py/poectrl.svg)](https://badge.fury.io/py/poectrl)\n\n**Development work** for a system to remotely and automatically control the PoE\nstatus of individual ports on multiple Ubiquiti TS-8-Pro Switch, using\npredefined profiles.\n\nThis has currently only been tested on the TS-8-PRO ToughSwitch routers,\nthough others will be added soon.\n\n**IMPORTANT: This library DOES NOT (and CAN NOT) ensure that any device attached\nto a port is compatible with the voltage selected. BE VERY CAREFUL that you\nchoose the correct voltage for your devices or you can DAMAGE THEM. No\nresponsibility is taken for equipment damaged using this library.**\n\n- [Status](#status)\n- [Use Cases](#use-cases)\n- [Installation](#installation)\n- [Configuration](#configuration)\n- [Usage](#usage)\n  - [As a command-line program](#as-a-command-line-program)\n  - [As an API](#as-an-api)\n    - [API Routes](#api-routes)\n- [Development Plans](#development-plans)\n- [Contributing](#contributing)\n\n## Status\n\nThis project is in no way ready to be used, and documentation is non-existent.\nSee the Development Plans below. Until I have a stable useful interface, check\nthe source code if you are interested 😃\n\n## Use Cases\n\n- Control a set of PoE-powered IP cameras, switches and access points to allow\ndisabling when not needed or quick enabling if required.\n\n## Installation\n\nThe latest version is uploaded to [pypi.org](https://pypi.org) so you can\ninstall this the same as any other package:\n\n```console\npip install poectrl\n```\n\n## Configuration\n\n**IMPORTANT : The configuration layout has CHANGED from version 1.2.0. If you\nare using config files from previous versions you will need to update the\n"devices" section to fit the below schema and change the profile to point to the\nname instead of IP address.**\n\nThe program is configured using a `poectrl.json` file either in the current\nworking directory (first priority) or the user\'s home directory. This is a\nsimple file that describes all devices and profiles. There is an example in\n[poectrl-example.json](poectrl-example.json) :\n\n```json\n{\n  "devices": {\n    "switch_1": {"ip": "192.168.0.187", "user": "ubnt", "password": "ubnt"},\n    "switch_2": {"ip": "192.168.0.190", "user": "ubnt", "password": "ubnt"}\n  },\n  "profiles": {\n    "cctv_on": {\n      "switch_1": {"4": 24, "5": 24, "8": 48},\n      "switch_2": {"5": 24, "6": 24, "7": 48}\n    },\n    "cctv_off": {\n      "switch_1": {"4": 0, "5": 0, "8": 0},\n      "switch_2": {"5": 0, "6": 0, "7": 0}\n    }\n  }\n}\n\n```\n\n## Usage\n\n### As a command-line program\n\nApply a predefined profile, setting the PoE port voltages.\n\n```console\n$ poectrl apply cctv_off\nUsing configuration from /home/seapagan/data/work/own/poectrl/poectrl.json\nConncting to switch_1 (192.168.0.187):\n  Setting port 4 to 0V\n  Setting port 5 to 0V\n  Setting port 8 to 0V\nConncting to switch_2 (192.168.0.190):\n  Setting port 5 to 0V\n  Setting port 6 to 0V\n  Setting port 7 to 0V\n\n```\n\nList all defined profiles:\n\n```console\n$ poectrl list\nUsing configuration from /home/seapagan/data/work/own/ts-8-pro-control/poectrl.json\n\nValid profiles are :\n - cctv_on\n - cctv_off\n```\n\nShow settings for a profile :\n\n```console\n$ poectrl show cctv_off\nUsing configuration from /home/seapagan/data/work/own/ts-8-pro-control/poectrl.json\n{\n    "switch_1": {\n        "4": 0,\n        "5": 0,\n        "8": 0\n    },\n    "switch_2": {\n        "5": 0,\n        "6": 0,\n        "7": 0\n    }\n}\n```\n\n### As an API\n\nIt is also possible to run this locally as an API, which can then allow easier\ncontrol using a web browser.\n\n**Important**: This is only designed for local network use, not over the\ninternet since there is NO access control set up. If you open this to the\ninternet then ANYONE can control your PoE!\n\n```console\n$ poectrl serve\nINFO:     Started server process [49922]\nINFO:     Waiting for application startup.\nINFO:     Application startup complete.\nINFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)\n```\n\nThere are a couple of command-line switches you can use :\n\n`---refresh` - This is useful if you are modifiying or troubleshooting the code,\nthe API will reload after each source code change.\n\n`--port <int>` - Change the port that the API listens on (default is 8000)\n\n`--host` - binds to all network interfaces on the host, allowing access from\nother machines using the public IP address of this machine\n\nAfter this, you can access the API on `http://localhost:8000`. Swagger docs are\navailable at `http://localhost:8000/docs`\n\n#### API Routes\n\nThere are currently 3 routes which correspond to the same command in the CLI.\n\n`/list/` - Lists all the defined profiles\\\n`/show/{profile_name}` - Shows details for the specific profile\\\n`/apply/{profile_name}` - Apply the specific profile\n\n## Development Plans\n\nCurrent proposed project plan.\n\n- [x] Write proof-of-concept code to control ports.\n- [x] Refactor and tidy the above code into a Library Class.\n- [x] Create a basic CLI using this Library\n- [x] Continue the CLI to use a config file, show current values, list profiles\n  etc.\n- [x] Publish on PyPi as a standalone package.\n- [x] Wrap this into an API (using FastAPI) for local use only.\n- [ ] Create a Web App to interface with the above API.\n\n## Contributing\n\nAt this time, the project is barely in it\'s planning stage but I do have a firm\nidea where it\'s going and how to structure it. As such, other contributions are\nnot looked for at this time. Hopefully, within a few days this project will be\nat a much more advanced stage and that will change 😃.\n',
     'author': 'Grant Ramsay',
     'author_email': 'seapagan@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seapagan/ts-8-pro-control',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `poectrl-0.3.0/PKG-INFO` & `poectrl-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poectrl
-Version: 0.3.0
+Version: 0.4.0
 Summary: Control PoE status on select Ubiquiti switches
 Home-page: https://github.com/seapagan/ts-8-pro-control
 License: MIT
 Author: Grant Ramsay
 Author-email: seapagan@gmail.com
 Requires-Python: >=3.7.2,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -20,16 +20,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: fastapi[all] (>=0.88.0,<0.89.0)
-Requires-Dist: paramiko (>=2.12.0,<3.0.0)
+Requires-Dist: fastapi[all] (>=0.88,<0.96)
+Requires-Dist: paramiko (>=2.12,<4.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: Bug Tracker, https://github.com/seapagan/openapi-readme/issues
 Project-URL: Pull Requests, https://github.com/seapagan/openapi-readme/pulls
 Project-URL: Repository, https://github.com/seapagan/ts-8-pro-control
 Description-Content-Type: text/markdown
 
 # Control PoE status on a Ubiquiti TS-8-Pro Switch <!-- omit in toc -->
@@ -181,14 +181,17 @@
 There are a couple of command-line switches you can use :
 
 `---refresh` - This is useful if you are modifiying or troubleshooting the code,
 the API will reload after each source code change.
 
 `--port <int>` - Change the port that the API listens on (default is 8000)
 
+`--host` - binds to all network interfaces on the host, allowing access from
+other machines using the public IP address of this machine
+
 After this, you can access the API on `http://localhost:8000`. Swagger docs are
 available at `http://localhost:8000/docs`
 
 #### API Routes
 
 There are currently 3 routes which correspond to the same command in the CLI.
```

