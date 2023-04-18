# Comparing `tmp/TapisCL-ICICLE-0.0.26.tar.gz` & `tmp/TapisCL-ICICLE-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.26.tar", last modified: Fri Apr 14 18:34:16 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.27.tar", last modified: Tue Apr 18 02:47:00 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.26.tar` & `TapisCL-ICICLE-0.0.27.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 18:34:16.720619 TapisCL-ICICLE-0.0.26/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/LICENSE
--rw-rw-rw-   0        0        0    43880 2023-04-14 18:34:16.720619 TapisCL-ICICLE-0.0.26/PKG-INFO
--rw-rw-rw-   0        0        0     1970 2023-04-14 17:01:05.000000 TapisCL-ICICLE-0.0.26/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 18:34:16.710651 TapisCL-ICICLE-0.0.26/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0     1408 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/args.py
--rw-rw-rw-   0        0        0    10950 2023-04-14 18:32:13.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/cli.py
--rw-rw-rw-   0        0        0     6873 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/decorators.py
--rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/exceptions.py
--rw-rw-rw-   0        0        0     5132 2023-04-14 18:06:28.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/helpers.py
--rw-rw-rw-   0        0        0     1049 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/schemas.py
--rw-rw-rw-   0        0        0    10402 2023-04-14 18:00:07.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/socketOpts.py
--rw-rw-rw-   0        0        0    18763 2023-04-14 18:25:04.000000 TapisCL-ICICLE-0.0.26/TapisCLICICLE/tapisObjectWrappers.py
-drwxrwxrwx   0        0        0        0 2023-04-14 18:34:16.719623 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    43880 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-14 18:34:16.000000 TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2023-04-14 18:31:46.000000 TapisCL-ICICLE-0.0.26/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 18:34:16.721612 TapisCL-ICICLE-0.0.26/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 02:47:00.110382 TapisCL-ICICLE-0.0.27/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.27/LICENSE
+-rw-rw-rw-   0        0        0    43999 2023-04-18 02:47:00.110382 TapisCL-ICICLE-0.0.27/PKG-INFO
+-rw-rw-rw-   0        0        0     2089 2023-04-18 01:25:59.000000 TapisCL-ICICLE-0.0.27/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 02:47:00.100554 TapisCL-ICICLE-0.0.27/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0     1597 2023-04-18 02:12:46.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/args.py
+-rw-rw-rw-   0        0        0    10894 2023-04-18 02:36:57.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/cli.py
+-rw-rw-rw-   0        0        0     9161 2023-04-18 02:36:33.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/decorators.py
+-rw-rw-rw-   0        0        0     1772 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/exceptions.py
+-rw-rw-rw-   0        0        0     5754 2023-04-18 02:23:18.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/helpers.py
+-rw-rw-rw-   0        0        0     2023 2023-04-18 02:17:20.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/schemas.py
+-rw-rw-rw-   0        0        0    10260 2023-04-18 02:42:20.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/server.py
+-rw-rw-rw-   0        0        0     1645 2023-04-18 02:26:10.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/socketOpts.py
+-rw-rw-rw-   0        0        0    18892 2023-04-18 02:20:35.000000 TapisCL-ICICLE-0.0.27/TapisCLICICLE/tapisObjectWrappers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:47:00.108679 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    43999 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-18 02:47:00.000000 TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2023-04-18 02:45:35.000000 TapisCL-ICICLE-0.0.27/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 02:47:00.110382 TapisCL-ICICLE-0.0.27/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.26/LICENSE` & `TapisCL-ICICLE-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.26/PKG-INFO` & `TapisCL-ICICLE-0.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.26
+Version: 0.0.27
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,14 +685,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # TapisCLI
+Please remember to create an issue in this repository if you encounter any bugs, we will do our best to fix it quick!
 ## Overview
 Tapis CLI is designed to provide a simple to use, versatile way to interface with Tapis services hosted on HPC resources. User can either start the app and use it as a traditional command line applications, or pass commands directly from bash.
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
```

### Comparing `TapisCL-ICICLE-0.0.26/README.md` & `TapisCL-ICICLE-0.0.27/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # TapisCLI
+Please remember to create an issue in this repository if you encounter any bugs, we will do our best to fix it quick!
 ## Overview
 Tapis CLI is designed to provide a simple to use, versatile way to interface with Tapis services hosted on HPC resources. User can either start the app and use it as a traditional command line applications, or pass commands directly from bash.
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
```

### Comparing `TapisCL-ICICLE-0.0.26/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.27/TapisCLICICLE/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/python3
-
 import socket
 import argparse
 from argparse import SUPPRESS
 import sys
 import pyfiglet
 from getpass import getpass
 import os
@@ -27,14 +26,17 @@
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(__file__)))
 server_path = os.path.join(__location__, 'server.py')
 
 
 class CLI(SO.SocketOpts, helpers.OperationsHelper, decorators.DecoratorSetup, helpers.Formatters):
+    """
+    Receive user input, either direct from bash environment or from the custom interface, then parse these commands and send them to the server to be executed. 
+    """
     def __init__(self, IP: str, PORT: int):
         self.ip, self.port = IP, PORT
         self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM) 
 
         # sets up connection with the server
         self.username, self.url = self.connect()
 
@@ -51,108 +53,118 @@
         """
         if 'win' in sys.platform:
             os.system(f"pythonw {server_path}")
         else: # unix based
             os.system(f"python {server_path} &")
 
     @decorators.AnimatedLoading
-    def connection_initialization(self): # patience. This sometimes takes a while
+    def connection_initialization(self):
         """
         start the local server through the client
         """
-        startup_flag = False # flag to tell code not to run multiple server setup threads at once
+        startup_flag = False
         timeout_time = time.time() + 30 # server setup timeout. If expires, there is a problem!
         while True:
             if time.time() > timeout_time: # connection timeout condition
                 sys.stdout.write("\r[-] Connection timeout")
                 os._exit(0)
             try:
-                self.connection.connect((self.ip, self.port)) # try to establish a connection
+                self.connection.connect((self.ip, self.port)) 
                 if startup_flag:
                     startup.kill()
                 break
             except Exception as e:
                 if not startup_flag:
                     startup = helpers.KillableThread(target=self.initialize_server) # run the server setup on a separate thread
                     startup.start() 
                     startup_flag = True # set the flag to true so the thread runs only once
                     continue
 
     def connect(self):
         """
         connect to the local server
         """
-        self.connection_initialization() # connect to the server
-        if __name__ == "__main__":
-            self.connection.connect((self.ip, self.port)) # enable me for debugging. Requires manual server start
+        self.connection_initialization() 
+        #self.connection.connect((self.ip, self.port)) # enable me for debugging. Requires manual server start
         connection_info: schemas.StartupData = self.schema_unpack() # receive info from the server whether it is a first time connection
         if connection_info.initial: # if the server is receiving its first connection for the session\
             while True:
                 try:
                     url = str(input("\nEnter the link for the tapis service you are connecting to: ")).strip()
                 except KeyboardInterrupt:
                     url = " "
                     pass
                 url_data = schemas.StartupData(url=url)
                 self.json_send(url_data.dict())
                 auth_request: schemas.AuthRequest = self.schema_unpack()
                 try:
-                    username = str(input("\nUsername: ")).strip() # take the username
-                    password = getpass("Password: ").strip() # take the password
+                    username = str(input("\nUsername: ")).strip()
+                    password = getpass("Password: ").strip() 
                 except KeyboardInterrupt:
                     username, password = " ", " "
                     pass
                 auth_data = schemas.AuthData(username = username, password = password)
-                self.json_send(auth_data.dict()) # send the username and password to the server to be used
+                self.json_send(auth_data.dict())
 
-                verification: schemas.ResponseData | schemas.StartupData = self.schema_unpack() # server responds saying if the verification succeeded or not
+                verification: schemas.ResponseData | schemas.StartupData = self.schema_unpack() 
                 if verification.schema_type == 'StartupData': # verification success, program moves forward
                     return verification.username, verification.url
                 else: # verification failed. User has 3 tries, afterwards the program will shut down
                     print(f"[-] verification failure, attempt # {verification.response_message[1]}")
                     if verification.response_message[1] == 3:
                         sys.exit(0)
                     continue
 
-        print(f"[+] Connected to the Tapis service at {connection_info.url}")
         return connection_info.username, connection_info.url # return the username and url
 
     def process_command(self, command: str) -> list[str]: 
         """
         split the command string into a list. Not sure why this was even made
         """
         command = command.strip().split(' ') 
         return command
 
-    def expression_input(self) -> str: # for subclients. Pods and apps running through Tapis will have their own inputs. This gives user an interface
-        print("Enter 'exit' to submit") # user must enter exit to submit their input
+    def expression_input(self) -> str: 
+        """
+        Input an expression as requested by the server for something like cypher queries
+        """
+        print("Enter 'exit' to submit") 
         expression = ''
         line = ''
-        while line != 'exit': # handles multiple lines of input. Good for neo4j expressions
+        while line != 'exit': 
             line = str(input("> "))
             if line != 'exit':
                 expression += line
         return expression
 
     def fillout_form(self, form: list) -> dict:
+        """
+        fill out a form as requested by the server for more complicated functions
+        """
         filled_form = dict()
         for field in form:
             value = str(input(f"{field}: "))
             filled_form.update({field:value})
         return filled_form
 
-    def command_operator(self, kwargs: dict | list, exit_: int=0): # parses command input
+    def command_operator(self, kwargs: dict | list, exit_: int=0): 
+        """
+        parse arguments, handling bash and CLI input
+        """
         if isinstance(kwargs, list): # check if the command input is from the CLI, or direct input
-            kwargs = vars(self.parser.parse_args(kwargs)) # parse the arguments
+            kwargs = vars(self.parser.parse_args(kwargs)) 
         if not kwargs['command_group']:
             return False
         command = schemas.CommandData(kwargs = kwargs, exit_status = exit_)
         return command
     
     def special_forms_ops(self):
+        """
+        handle special form requests sent by the server
+        """
         while True:
             response = self.schema_unpack()
             if response.schema_type == 'FormRequest' and not response.arguments_list:
                 form = self.expression_input()
                 filled_form = schemas.FormResponse(arguments_list=form)
             elif response.schema_type == 'FormRequest':
                 form = self.fillout_form(response.arguments_list)
@@ -179,14 +191,17 @@
                         print("Enter valid response")
                 filled_form = schemas.ResponseData(response_message=decision)
             else:
                 return response
             self.json_send(filled_form.dict())
 
     def print_response(self, response_message):
+        """
+        format response messages from the server
+        """
         if type(response_message) == dict:
             self.recursive_dict_print(response_message)
         elif (type(response_message) == list or 
              type(response_message) == tuple or 
              type(response_message) == set):
             for value in response_message:
                 print(value)
```

### Comparing `TapisCL-ICICLE-0.0.26/TapisCLICICLE/decorators.py` & `TapisCL-ICICLE-0.0.27/TapisCLICICLE/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+DECORATORS
+These decorators are used in the tapisObjectWrappers.py file to standardize special functions. Allows for increased code reusability
+"""
 import typing
 import socket
 import sys
 import time
 from functools import update_wrapper, partial
 try:
     from . import helpers
@@ -38,98 +42,128 @@
         return str(self.function)
     
     def __str__(self):
         return str(self.function)
 
 
 class RequiresForm(BaseRequirementDecorator):
-    def __call__(self, obj, *args, **kwargs):
-        fields = list(helpers.get_parameters(self.function))
-        for key, value in kwargs.items():
-            if value or value == False:
-                fields.remove(key)
-        if not fields:
-            raise AttributeError(f"The decorated function {self.function} has no parameters.")
-        form_request = schemas.FormRequest(arguments_list=fields)
-        self.json_send_explicit(BaseRequirementDecorator.connection, form_request.dict())
-        filled_form: schemas.FormResponse = self.schema_unpack_explicit(self.connection).arguments_list
-        for key, value in filled_form.items():
-            kwargs[key] = value
+    """
+    This is for when you want to request separate input for specific command parameters instead of taking directly from the original command input (kwargs)
+    Takes the parameters list of the function in question, filters out the ones that were not received from the original request message, sends another message 
+    to request the unreceived parameters, and receives a message in response from the client to execute the function
+    """
+    def __call__(self, obj, *args, **kwargs):
+        if BaseRequirementDecorator.connection:
+            fields = list(helpers.get_parameters(self.function))
+            for key, value in kwargs.items():
+                if value or value == False:
+                    fields.remove(key)
+            if not fields:
+                raise AttributeError(f"The decorated function {self.function} has no parameters.")
+            form_request = schemas.FormRequest(arguments_list=fields)
+            self.json_send_explicit(BaseRequirementDecorator.connection, form_request.dict())
+            filled_form: schemas.FormResponse = self.schema_unpack_explicit(self.connection).arguments_list
+            for key, value in filled_form.items():
+                kwargs[key] = value
 
         return self.function(obj, **kwargs)
 
 
 class RequiresExpression(BaseRequirementDecorator):
-    def __call__(self, obj, *args, **kwargs):
-        fields = list(helpers.get_parameters(self.function))
-        if 'expression' not in fields:
-            raise AttributeError(f"The function {self.function} does not contain an 'expression' parameter")
-        form_request = schemas.FormRequest(arguments_list=[])
-        self.json_send_explicit(BaseRequirementDecorator.connection, form_request.dict())
-        filled_form: schemas.FormResponse = self.schema_unpack()
-        kwargs['expression'] = filled_form.arguments_list
+    """
+    This is for when you have something like a Neo4j or postgres interface to add to the tapisObjectWrappers file. Writing a Neo4j query directly in a command is cumbersome, its much
+    easier to do if you have a blank, multiline environment to write. This will send a request for an expression, if an expression parameter exists in the decorated function.
+    The client will open a new interface to type the expression. This is then sent back and fed to the function
+    """
+    def __call__(self, obj, *args, **kwargs):
+        if BaseRequirementDecorator.connection:
+            fields = list(helpers.get_parameters(self.function))
+            if 'expression' not in fields:
+                raise AttributeError(f"The function {self.function} does not contain an 'expression' parameter")
+            form_request = schemas.FormRequest(arguments_list=[])
+            self.json_send_explicit(BaseRequirementDecorator.connection, form_request.dict())
+            filled_form: schemas.FormResponse = self.schema_unpack()
+            kwargs['expression'] = filled_form.arguments_list
 
         return self.function(obj, **kwargs)
     
 
 class SecureInput(BaseRequirementDecorator):
-    def __call__(self, obj, *args, **kwargs):
-        fields = list(helpers.get_parameters(self.function))
-        if 'password' in fields:
-            secure_input_request = schemas.AuthRequest(secure_input=True)
-            self.json_send_explicit(BaseRequirementDecorator.connection, secure_input_request.dict())
-            secure_input_data: schemas.AuthData = self.schema_unpack_explicit(self.connection)
-            kwargs['password'] = secure_input_data.password
-            return self.function(obj, **kwargs)
-        raise AttributeError(f"The function {self.function} does not contain a 'password' parameter")
+    """
+    Use this for functions where you need to hide input while typing into the cli. For instance, if you want to add a password to a service, as a user, but you dont actually
+    want to authenticate. Checks if the decorated function has a password parameter, then requests secure input of a new password from the client
+    """
+    def __call__(self, obj, *args, **kwargs):
+        if BaseRequirementDecorator.connection:
+            fields = list(helpers.get_parameters(self.function))
+            if 'password' in fields:
+                secure_input_request = schemas.AuthRequest(secure_input=True)
+                self.json_send_explicit(BaseRequirementDecorator.connection, secure_input_request.dict())
+                secure_input_data: schemas.AuthData = self.schema_unpack_explicit(self.connection)
+                kwargs['password'] = secure_input_data.password
+                return self.function(obj, **kwargs)
+            raise AttributeError(f"The function {self.function} does not contain a 'password' parameter to securely input")
+        return self.function(obj, **kwargs)
 
 
 class Auth(BaseRequirementDecorator):
-    def __call__(self, obj, *args, **kwargs):
-        if self.function.__name__ == 'tapis_init' and kwargs['username'] and kwargs['password']:
-            return self.function(obj, **kwargs)
-        fields = list(helpers.get_parameters(self.function))
-        auth_request = schemas.AuthRequest()
-        self.json_send_explicit(BaseRequirementDecorator.connection, auth_request.dict())
-        auth_data: schemas.AuthData = self.schema_unpack_explicit(self.connection)
-        if 'username' in fields and 'password' in fields:
-            kwargs['username'], kwargs['password'] = auth_data.username, auth_data.password
-            return self.function(obj, **kwargs)
-        username, password = auth_data.username, auth_data.password
-        if username != BaseRequirementDecorator.username:
-            raise exceptions.InvalidCredentialsReceived(self.function, 'username')
-        elif password != BaseRequirementDecorator.password:    
-            raise exceptions.InvalidCredentialsReceived(self.function, 'password')
+    """
+    used for secure authentication from the client. Requires that the function has a username and password parameter for credentials. sends request for credentials from 
+    the client, and checks those credentials against the stored credentials in the server.
+    """
+    def __call__(self, obj, *args, **kwargs):
+        if BaseRequirementDecorator.connection:
+            if self.function.__name__ == 'tapis_init' and kwargs['username'] and kwargs['password']:
+                return self.function(obj, **kwargs)
+            fields = list(helpers.get_parameters(self.function))
+            auth_request = schemas.AuthRequest()
+            self.json_send_explicit(BaseRequirementDecorator.connection, auth_request.dict())
+            auth_data: schemas.AuthData = self.schema_unpack_explicit(self.connection)
+            if 'username' in fields and 'password' in fields:
+                kwargs['username'], kwargs['password'] = auth_data.username, auth_data.password
+                return self.function(obj, **kwargs)
+            username, password = auth_data.username, auth_data.password
+            if username != BaseRequirementDecorator.username:
+                raise exceptions.InvalidCredentialsReceived(self.function, 'username')
+            elif password != BaseRequirementDecorator.password:    
+                raise exceptions.InvalidCredentialsReceived(self.function, 'password')
 
         return self.function(obj, **kwargs)
 
 
 class NeedsConfirmation(BaseRequirementDecorator):
-    def __call__(self, obj, *args, **kwargs):
-        confirmation_request = schemas.ConfirmationRequest(message=f"You requested to {self.function.__name__}. Please confirm (y/n)")
-        self.json_send_explicit(BaseRequirementDecorator.connection, confirmation_request.dict())
-        confirmation_reply: schemas.ResponseData = self.schema_unpack_explicit(self.connection)
-        confirmed = confirmation_reply.response_message
-        if not confirmed:
-            raise exceptions.NoConfirmationError(self.function)
-        return self.function(obj, **kwargs)
-    
-class TestDecorator(BaseRequirementDecorator):
-    def __call__(self, obj, *args, **kwargs):
-        print(BaseRequirementDecorator.connection)
+    """
+    add to functions that you want user confirmation to exit. If you accidentally enter a command to delete a pod, this will not let you until you confirm
+    """
+    def __call__(self, obj, *args, **kwargs):
+        if BaseRequirementDecorator.connection:
+            confirmation_request = schemas.ConfirmationRequest(message=f"YOU REQUESTED TO {self.function.__name__}. THIS MIGHT CAUSE DATA LOSS! Please confirm (y/n)")
+            self.json_send_explicit(BaseRequirementDecorator.connection, confirmation_request.dict())
+            confirmation_reply: schemas.ResponseData = self.schema_unpack_explicit(self.connection)
+            confirmed = confirmation_reply.response_message
+            if not confirmed:
+                raise exceptions.NoConfirmationError(self.function)
         return self.function(obj, **kwargs)
+
     
 class DecoratorSetup:
+    """
+    for instantiation of the tapis wrappers, and the server, to set up decorators with user credentials and the socket connection. If you want to use the decorators in your class
+    YOU WILL NEED TO USE THIS!
+    """
     def configure_decorators(self):
         BaseRequirementDecorator.connection = self.connection
         BaseRequirementDecorator.username = self.username
         BaseRequirementDecorator.password = self.password
     
 
 class AnimatedLoading:
+    """
+    Add this if you want to print a loading animation while a function is executing
+    """
     def __init__(self, func: typing.Callable):
         update_wrapper(self, func)
         self.function = func
         self.__code__ = func.__code__
         self.animation_frames = ['|','/','-','\\']
 
     def __get__(self, obj, objtype):
@@ -146,28 +180,15 @@
         while True:
             for frame in self.animation_frames:
                 sys.stdout.write(f'\rloading ' + frame)
                 sys.stdout.flush()
                 time.sleep(0.5)
     
     def __call__(self, obj, *args, **kwargs):
-        animation_thread = helpers.KillableThread(target=self.animation)
-        animation_thread.start()
-        result = self.function(obj, *args, **kwargs)
-        animation_thread.kill()
-        return result
-
-
-if __name__ == "__main__":
-    class Silly(DecoratorSetup):
-        def __init__(self):
-            self.connection = "x"
-            self.username = "y"
-            self.password = "v"
-            self.configure_decorators()
-
-        @TestDecorator
-        def sillify(self, x):
-            return "THIS WORKED"
-        
-    zeugmizer = Silly()
-    print(zeugmizer.sillify(x="zed"))
+        if BaseRequirementDecorator.username:
+            animation_thread = helpers.KillableThread(target=self.animation)
+            animation_thread.start()
+            result = self.function(obj, *args, **kwargs)
+            animation_thread.kill()
+        else:
+            result = self.function(obj, *args, **kwargs)
+        return result
```

### Comparing `TapisCL-ICICLE-0.0.26/TapisCLICICLE/exceptions.py` & `TapisCL-ICICLE-0.0.27/TapisCLICICLE/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.26/TapisCLICICLE/helpers.py` & `TapisCL-ICICLE-0.0.27/TapisCLICICLE/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+HELPERS
+Aggregation of helper functions and classes
+"""
 import typing
 import sys
 import threading
 import re
 try:
     from . import exceptions
     from . import args
@@ -16,14 +20,17 @@
 def get_parameters(func):
     args = list(func.__code__.co_varnames[:func.__code__.co_argcount])
     if args[0] == "self":
         args = args[1:]
     return args
 
 class OperationsHelper:
+    """
+    filters the kwargs received by the server to prevent an error from happening
+    """
     def filter_kwargs(self, func: typing.Callable, kwargs: dict) -> dict:
         filtered = dict()
         variables = list(get_parameters(func))
         for arg in variables:
             if arg != "password" and arg != "expression": filtered.update({arg:kwargs[arg]})
             elif arg == "password": filtered.update({'password':None})
             elif arg == "expression": filtered.update({'expression':None})
@@ -36,26 +43,32 @@
 
 class DynamicHelpUtility:
     """
     dynamically generate the help menu based on the doc  string and function arguments using .__doc__ and .__code__
     to generate helps for each command, iterate over the command map of the selected tapis wrapper object, and generate separate help menu for each
     """
     def __locate_docstring_help(self, func: typing.Callable | object, command_name: str) -> str:
+        """
+        extract @help from the docstring
+        """
         docstring_components = func.__doc__
         if docstring_components:
             docstring_components = docstring_components.split("@")
         else:
             raise exceptions.HelpDoesNotExist(command_name)
         for docstring_component in docstring_components:
             if re.match(r'^[^:]+', docstring_component).group(0) == "help":
                 return docstring_component.split("help: ")[1]
         else:
             raise exceptions.HelpDoesNotExist(command_name)
 
     def __tapis_service_commands_help_gen(self, map) -> dict:
+        """
+        generate help menu based on the parameters of the function and the docstring
+        """
         help_menu = dict()
         for command_name, command in map.items():
             command_help = dict()
             command_help['command_name'] = command_name
             command_help['description'] = self.__locate_docstring_help(command, command_name)
             arguments = None
             if self.__class__.__name__ != 'Server': 
@@ -73,21 +86,27 @@
                         argument_help += f" {command_parameters[argument]['args'][1]} <{argument}>"
 
             command_help['syntax'] = argument_help
             help_menu[command_name] = command_help
         return help_menu
             
     def help_generation(self) -> dict:
+        """
+        generate different help menu based on the classname
+        """
         if self.__class__.__name__ != 'Server': 
             return self.__tapis_service_commands_help_gen(map=self.command_map)
         else:
             return self.__tapis_service_commands_help_gen(map=self.command_group_map), self.__tapis_service_commands_help_gen(map=self.command_map)
     
 
 class KillableThread(threading.Thread):
+    """
+    Extends the threading.Thread class from python threading library. Used for the loading animation
+    """
     def __init__(self, *args, **keywords):
         threading.Thread.__init__(self, *args, **keywords)
         self.killed = False
 
     def start(self):
         self.__run_backup = self.run
         self.run = self.__run     
@@ -111,14 +130,17 @@
         return self.localtrace
 
     def kill(self):
         self.killed = True
 
 
 class Formatters:
+    """
+    Format received dictionaries in the client code
+    """
     def recursive_dict_print(self, input_data: dict, depth: int=0):
         for key, value in input_data.items():
             if isinstance(value, dict):
                 print(("  " * depth) + f"{key}:")
                 self.recursive_dict_print(value, depth=depth + 1)
             elif isinstance(value, (list, tuple, set)):
                 print(("  " * depth) + f"{key}:")
```

### Comparing `TapisCL-ICICLE-0.0.26/TapisCLICICLE/server.py` & `TapisCL-ICICLE-0.0.27/TapisCLICICLE/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     import exceptions
     import socketOpts as SO
     import helpers
     import schemas
     import decorators
 
 class Server(SO.SocketOpts, helpers.OperationsHelper, decorators.DecoratorSetup, helpers.DynamicHelpUtility):
+    """
+    Receives commands from the client and executes Tapis operations
+    """
     def __init__(self, IP: str, PORT: int):
         # logger setup
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(logging.INFO)
         stream_handler = logging.StreamHandler(stream=sys.stdout)
 
         file_handler = logging.FileHandler(
@@ -123,61 +126,58 @@
             r'(?<=access_token: )(.*)', str(authenticator))[0]
         
         if 'win' in sys.platform:
             os.system(f"set JWT={access_token}")
         else: # unix based
             os.system(f"export JWT={access_token}")
 
-        self.pods = Pods(t, username, password, self.connection)
-        self.systems = Systems(t, username, password, self.connection)
-        self.files = Files(t, username, password, self.connection)
-        self.apps = Apps(t, username, password, self.connection)
-        self.neo4j = Neo4jCLI(t, username, password, self.connection)
+        self.pods = Pods(t, username, password, connection=self.connection)
+        self.systems = Systems(t, username, password, connection=self.connection)
+        self.files = Files(t, username, password, connection=self.connection)
+        self.apps = Apps(t, username, password, connection=self.connection)
+        self.neo4j = Neo4jCLI(t, username, password, connection=self.connection)
 
         self.t = t
         self.url = url
         self.access_token = access_token
 
         self.logger.info(f"initiated in {time.time()-start}")
 
         return f"Successfully initialized tapis service on {self.url}"
 
-    def accept(self, initial: bool=False):  # function to accept CLI connection to the server
-        self.connection, ip_port = self.sock.accept()  # connection request is accepted
+    def accept(self, initial: bool=False):
+        """
+        accept connection request and initialize communication with the client
+        """  
+        self.connection, ip_port = self.sock.accept() 
         self.logger.info("Received connection request")
 
         if initial:  # if this is the first time in the session that the cli is connecting
             startup_data = schemas.StartupData(initial = initial)
             self.json_send(startup_data.dict())
             self.logger.info("send the initial status update")
 
-            # give the cli 3 attempts to provide authentication
             for attempt in range(1, 4):
-                  # receive the username and password
                 url: schemas.StartupData = self.schema_unpack().url
                 try:
-                # try intializing tapis with the supplied credentials
                     auth_request = schemas.AuthRequest()
                     self.json_send(auth_request.dict())
                     auth_data: schemas.AuthData = self.schema_unpack()
                     username, password = auth_data.username, auth_data.password
-
                     self.tapis_init(link=url, username=username, password=password)
-                    # send to confirm to the CLI that authentication succeeded
                     self.logger.info("Verification success")
                     break
                 except Exception as e:
-                    # send failure message to CLI
                     login_failure_data = schemas.ResponseData(response_message = (str(e), attempt))
                     self.json_send(login_failure_data.dict())
                     self.logger.warning(f"Verification failure, {e}")
-                    if attempt == 3:  # If there have been 3 login attempts
+                    if attempt == 3:  
                         self.logger.error(
                             "Attempted verification too many times. Exiting")
-                        os._exit(0)  # shutdown the server
+                        os._exit(0)  
                     continue
         else:
             self.configure_decorators()
         startup_result = schemas.StartupData(initial = initial, username = self.username, url = self.url)
         self.logger.info("Connection success")
         self.json_send(startup_result.dict())
         self.logger.info("Final connection data sent")
@@ -191,69 +191,76 @@
     def __shutdown(self):
         """
         @help: exit the CLI and shutdown the service
         """
         self.logger.info("Shutdown initiated")
         raise exceptions.Shutdown
 
-    def timeout_handler(self):  # handle timeouts
-        if time.time() > self.end_time:  # if the time exceeds the timeout time
+    def timeout_handler(self):  
+        """
+        checks if the timeout has been exceeded
+        """
+        if time.time() > self.end_time: 
             raise exceptions.TimeoutError
-    
-    def format_help(self, command: dict):
-        return f"Command: {command['command_name']}\nDescription:{command['description']}\n{command['syntax']}\n"
-
 
     def help(self, command: str):
         """
         @help: returns help information. To get specific help information for tapis services, you can run <service> -c help
         """
         if command in self.help:
             return self.help[command]
         return self.help
 
-    def run_command(self, command_data: dict):  # process and run commands
+    def run_command(self, command_data: dict):
+        """
+        process and run command based on received kwargs
+        """
         command_group = command_data['command_group']
         if command_group in self.command_group_map:
             command_group = self.command_group_map[command_group]
             return command_group(**command_data)
         elif command_group in self.command_map:
             command = self.command_map[command_group]
             command_data = self.filter_kwargs(command, command_data)
             if command_data:
                 return command(**command_data)
             return command()
         else:
             raise exceptions.CommandNotFoundError(command_group)
 
     def main(self):
+        """
+        receive and process commands
+        """
         while True: 
             try:
                 message = self.schema_unpack()  
                 self.timeout_handler()  
                 kwargs, exit_status = message.kwargs, message.exit_status
                 result = self.run_command(kwargs)
                 response = schemas.ResponseData(response_message = result)
                 self.end_time = time.time() + 300 
                 self.json_send(response.dict()) 
                 self.logger.info(message)
                 if exit_status == 1:
                     self.__exit()
-            except (exceptions.CommandNotFoundError, exceptions.NoConfirmationError, exceptions.InvalidCredentialsReceived) as e:
-                error_response = schemas.ResponseData(response_message = str(e))
-                self.json_send(error_response.dict())
             except (exceptions.TimeoutError, exceptions.Shutdown) as e:
                 error_response = schemas.ResponseData(response_message = str(e), exit_status=1)
                 self.json_send(error_response.dict())
+                self.logger.warning(str(e))
                 sys.exit(0)
             except exceptions.Exit as e:
                 self.logger.info("user exit initiated")
                 error_response = schemas.ResponseData(response_message = str(e), exit_status=1)
                 self.json_send(error_response.dict())
                 self.connection.close()  # close the connection
                 self.accept()  # wait for CLI to reconnect
+            except (exceptions.CommandNotFoundError, exceptions.NoConfirmationError, exceptions.InvalidCredentialsReceived, Exception) as e:
+                error_response = schemas.ResponseData(response_message = str(e))
+                self.json_send(error_response.dict())
+                self.logger.warning(str(e))
 
 
 
 if __name__ == '__main__':
     server = Server(socket.gethostbyname(socket.gethostname()), 30000)
     server.main()
```

### Comparing `TapisCL-ICICLE-0.0.26/TapisCLICICLE/socketOpts.py` & `TapisCL-ICICLE-0.0.27/TapisCLICICLE/socketOpts.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,23 @@
         'FormResponse':schemas.FormResponse,
         'AuthRequest':schemas.AuthRequest,
         'ConfirmationRequest':schemas.ConfirmationRequest
     }
 
 
 class SocketOpts:
+    """
+    behind the scenes, low level functions to handle the socket operations of the client-server model
+    """
     def json_receive_explicit(self, connection):
         json_data = ""
         while True:
-            try: #to handle long files, so that it continues to receive data and create a complete file
-                json_data = json_data + connection.recv(1024).decode('utf-8') #formulate a full file. Combine sequential data streams to unpack
-                return json.loads(json_data) #this is necessary whenever transporting any large amount of data over TCP streams
+            try: 
+                json_data = json_data + connection.recv(1024).decode('utf-8') 
+                return json.loads(json_data) 
             except ValueError:
                 continue
     
     def json_send_explicit(self, connection, data):
         json_data = json.dumps(data)
         connection.send(json_data.encode())
```

### Comparing `TapisCL-ICICLE-0.0.26/TapisCLICICLE/tapisObjectWrappers.py` & `TapisCL-ICICLE-0.0.27/TapisCLICICLE/tapisObjectWrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(__file__)))
 server_path = os.path.join(__location__, 'server.py')
 
 
 class tapisObject(helpers.OperationsHelper, decorators.DecoratorSetup, helpers.DynamicHelpUtility):
-    def __init__(self, tapis_instance, username, password, connection, command_map=None):
+    def __init__(self, tapis_instance, username, password, connection=None, command_map=None):
         self.t = tapis_instance
         self.username = username
         self.password = password
         self.connection = connection
 
         self.command_map = command_map
         
@@ -49,16 +49,16 @@
         """
         if name:
             return self.help[name]
         return self.help
     
 
 class TapisQuery(tapisObject):
-    def __init__(self, tapis_object, uname, pword, connection):
-        super().__init__(tapis_object, uname, pword, connection)
+    def __init__(self, tapis_object, uname, pword, connection=None):
+        super().__init__(tapis_object, uname, pword, connection=connection)
         self.t = tapis_object
         self.__code__ = self.query.__code__
 
     def __call__(self, **kwargs):
         try:
             kwargs = self.filter_kwargs(self.query, kwargs)
             result = self.query(**kwargs)
@@ -66,26 +66,27 @@
         except (tapipy.errors.NotFoundError, tapipy.errors.BadRequestError, tapipy.errors.BaseTapyException) as e:
             return str(e)
 
 
 class Systems(tapisObject):
     """
     @help: Access Tapis systems through the connected service
+    @doc: provides a CLI interface to the Tapis Systems service
     """
-    def __init__(self, tapis_instance, username, password, connection):
+    def __init__(self, tapis_instance, username, password, connection=None):
         command_map = {
             'get_systems':self.get_systems,
             'get_system_info':self.get_system_info,
             'create_system':self.create_system,
             'set_credentials':self.system_credential_upload,
             'set_password':self.system_password_set,
             'delete_system':self.delete_system,
             'help':self.help
         }
-        super().__init__(tapis_instance, username, password, connection, command_map=command_map)
+        super().__init__(tapis_instance, username, password, connection=connection, command_map=command_map)
 
     def return_formatter(self, info):
         return f"id: {info.id}\nhost: {info.host}\n\n"
 
     def __keygen(self):
         local_files = os.listdir(__location__)
         if "id_rsa" not in local_files or "id_rsa.pub" not in local_files:
@@ -198,37 +199,36 @@
             return str(e)
 
 
 class Pods(tapisObject):
     """
     @help: Access Tapis pods through the connected service
     """
-    def __init__(self, tapis_instance, username, password, connection):
+    def __init__(self, tapis_instance, username, password, connection=None):
         command_map = {
                 'get_pods':self.get_pods,
                 'create_pod':self.create_pod,
                 'restart_pod':self.restart_pod,
                 'delete_pod':self.delete_pod,
                 'set_pod_perms':self.set_pod_perms,
                 'stop_pod':self.stop_pod,
                 'delete_pod_perms':self.delete_pod_perms,
                 'get_perms':self.get_perms,
                 'copy_pod_password':self.copy_pod_password,
                 'get_logs':self.get_pod_logs,
                 'help':self.help
             }
-        super().__init__(tapis_instance, username, password, connection, command_map=command_map)
+        super().__init__(tapis_instance, username, password, connection=connection, command_map=command_map)
 
     def return_formatter(self, info):
         return f"Pod ID: {info.pod_id}\nPod Template: {info.pod_template}\nStatus: {info.status_requested}\n\n"
 
     def get_pods(self, verbose: bool) -> str: 
         """
         @help: return a list of pods the current tapis instance has access to
-        @doc: notes
         """
         pods_list = self.t.pods.get_pods()
         if verbose:
             return str(pods_list)
         pods_list = [self.return_formatter(pod) for pod in pods_list]
         pods_string = ""
         for pod in pods_list:
@@ -326,22 +326,22 @@
         return logs
 
 
 class Files(tapisObject):
     """
     @help: Access Tapis files through the connected service
     """
-    def __init__(self, tapis_instance, username, password, connection):
+    def __init__(self, tapis_instance, username, password, connection=None):
         command_map = {
             'list_files':self.list_files,
             'upload':self.upload,
             'download':self.download,
             'help':self.help
         }
-        super().__init__(tapis_instance, username, password, connection, command_map=command_map)
+        super().__init__(tapis_instance, username, password, connection=connection, command_map=command_map)
 
     def return_formatter(self, info):
         return f"name: {info.name}\ngroup: {info.group}\npath: {info.path}\n"
 
     def list_files(self, verbose: bool, id: str, file: str) -> str: # lists files available on a tapis account
         """
         @help: list the files on a system 
@@ -380,26 +380,26 @@
         return f'successfully downloaded {source} to {destination}'
 
 
 class Apps(tapisObject):
     """
     @help: Access Tapis systems through the connected service
     """
-    def __init__(self, tapis_instance, username, password, connection):
+    def __init__(self, tapis_instance, username, password, connection=None):
         command_map = {
             'create_app':self.create_app,
             'get_apps':self.get_apps,
             'delete_app':self.delete_app,
             'get_app_info':self.get_app,
             'run_app':self.run_job,
             'get_app_status':self.get_job_status,
             'download_app_results':self.download_job_output,
             'help':self.help,
         }
-        super().__init__(tapis_instance, username, password, connection, command_map=command_map)
+        super().__init__(tapis_instance, username, password, connection=connection, command_map=command_map)
 
     def create_app(self, file: str) -> str: # create a tapis app taking a json descriptor file path
         """
         @help: create an app. You must have a properly configured app config file. 
         See a template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/app-config.json
         """
         with open(file, 'r') as f:
```

### Comparing `TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.26
+Version: 0.0.27
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,14 +685,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # TapisCLI
+Please remember to create an issue in this repository if you encounter any bugs, we will do our best to fix it quick!
 ## Overview
 Tapis CLI is designed to provide a simple to use, versatile way to interface with Tapis services hosted on HPC resources. User can either start the app and use it as a traditional command line applications, or pass commands directly from bash.
 Allows you to work with all major Tapis services: Pods, Systems, Files, and Apps in one place. It can also interface directly with services being hosted on Tapis pods, like Neo4j. Although currently Neo4j is the only 3rd party application it can work with, adding support for Postgres and the like will not be difficult.
 
 ### Dependencies
 * Dependencies are listed [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_03_2023/CLI/TapisCL-ICICLE/requirements.txt)
```

### Comparing `TapisCL-ICICLE-0.0.26/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.27/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.26/pyproject.toml` & `TapisCL-ICICLE-0.0.27/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.26"
+version = "0.0.27"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

