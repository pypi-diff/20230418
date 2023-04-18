# Comparing `tmp/ogsapi-0.2.1.tar.gz` & `tmp/ogsapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogsapi-0.2.1.tar", last modified: Wed Apr  5 01:30:51 2023, max compression
+gzip compressed data, was "ogsapi-0.3.0.tar", last modified: Tue Apr 18 14:50:11 2023, max compression
```

## Comparing `ogsapi-0.2.1.tar` & `ogsapi-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 01:30:51.081236 ogsapi-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)    35082 2023-04-05 01:30:34.000000 ogsapi-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3036 2023-04-05 01:30:51.080237 ogsapi-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2602 2023-04-05 01:30:34.000000 ogsapi-0.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-04-05 01:30:34.000000 ogsapi-0.2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 01:30:51.081236 ogsapi-0.2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 01:30:51.076237 ogsapi-0.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 01:30:51.078237 ogsapi-0.2.1/src/ogsapi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-05 01:30:34.000000 ogsapi-0.2.1/src/ogsapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15947 2023-04-05 01:30:34.000000 ogsapi-0.2.1/src/ogsapi/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 01:30:51.080237 ogsapi-0.2.1/src/ogsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3036 2023-04-05 01:30:51.000000 ogsapi-0.2.1/src/ogsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-04-05 01:30:51.000000 ogsapi-0.2.1/src/ogsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 01:30:51.000000 ogsapi-0.2.1/src/ogsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-04-05 01:30:51.000000 ogsapi-0.2.1/src/ogsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-05 01:30:51.000000 ogsapi-0.2.1/src/ogsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:50:11.998084 ogsapi-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35082 2023-04-18 14:49:55.000000 ogsapi-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3882 2023-04-18 14:50:11.996251 ogsapi-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3448 2023-04-18 14:49:55.000000 ogsapi-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-18 14:49:55.000000 ogsapi-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 14:50:11.998084 ogsapi-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:50:11.992584 ogsapi-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:50:11.994417 ogsapi-0.3.0/src/ogsapi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:49:55.000000 ogsapi-0.3.0/src/ogsapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17976 2023-04-18 14:49:55.000000 ogsapi-0.3.0/src/ogsapi/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 14:50:11.996251 ogsapi-0.3.0/src/ogsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3882 2023-04-18 14:50:11.000000 ogsapi-0.3.0/src/ogsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-04-18 14:50:11.000000 ogsapi-0.3.0/src/ogsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 14:50:11.000000 ogsapi-0.3.0/src/ogsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-18 14:50:11.000000 ogsapi-0.3.0/src/ogsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-18 14:50:11.000000 ogsapi-0.3.0/src/ogsapi.egg-info/top_level.txt
```

### Comparing `ogsapi-0.2.1/LICENSE` & `ogsapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ogsapi-0.2.1/PKG-INFO` & `ogsapi-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: ogsapi
-Version: 0.2.1
-Summary: An API Wrapper for online-go.com, an online Go / Baduk server
-Author-email: Dakota Marshall <me@dakotamarshall.net>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # OGS Python Library
 
 
 [![pipeline status](https://gitlab.com/dakota.marshall/ogs-python/badges/prod/pipeline.svg)](https://gitlab.com/dakota.marshall/ogs-python/-/commits/prod)  [![Latest Release](https://gitlab.com/dakota.marshall/ogs-python/-/badges/release.svg)](https://gitlab.com/dakota.marshall/ogs-python/-/releases) [![PyPI version](https://badge.fury.io/py/ogsapi.svg)](https://badge.fury.io/py/ogsapi) 
 
 ## Summary
 
@@ -53,14 +41,22 @@
 
 ## Implemented API Functions
 *NOTE* All usernames are case sensitive
 ### User Functions
 
 - Get User vitals: `ogs.user_vitals()`
 - Get User Settings: `ogs.user_settings()`
+- Update User Settings: `ogs.update_user_settings()
+  - username: str
+  - first_name: str
+  - last_name: str
+  - country: str
+  - private_name: bool
+  - website: str
+  - about: str
 - Get User Games: `ogs.user_games()`
 - Get User Friends (Optionally search for user): `ogs.user_friends(username)`
 - Send friend request: `ogs.send_friend_request(username)`
 
 ### Player Functions
 
 - Get Player Info: `ogs.get_player(username)`
@@ -72,19 +68,34 @@
 ## Implemented Realtime API Functions
 
 - Get Host Info: `ogs.sock.host_info()`
 - Ping: `ogs.sock.ping()`
 - Connect To Notification Stream: `ogs.sock.notification_connect()`
 - Connect to Chat: `ogs.sock.chat_connect()`
 - Connect to a Game: `ogs.sock.game_connect(gameid: int)`
-  - This creates an object in the `ogs.sock.games` list with the key `game_id`
+  - This returns an object containing all the functions to handle received events from that game
+  - To be able to run code when a move is received, you need to register a callback function you made with: 
+  - `ogs.sock.games[game_id].register_callback(callback)`
 - Disconnect from a Game: `ogs.sock.game_disconnect(game_id)`
 
 ### Implemented Game Functions
 
 - Make a move: `ogs.sock.games[game_id].move('jj')`
+- Pass turn: `ogs.sock.games[game_id].pass_turn()`
+- Request an undo: `ogs.sock.games[game_id].undo()`
+- Resign: `ogs.sock.games[game_id].resign()`
+
+### Implemented Received Events
+
+- Getting gamedata: `ogs.sock.games[game_id].game_data`
+- Getting connection latency: `ogs.sock.games[game_id].latency`
+- Getting a move: `ogs.sock.games[game_id].callback_func['on_move']`
 
 
 ## To Implement
-TODO: Update this list
 
-- Pretty much everything
+- Implement callback function handling for:
+  - The clock
+  - Undo requested
+  - Undo Accepted
+- Implement proper challenge creation
+- Create open challenge
```

### Comparing `ogsapi-0.2.1/README.md` & `ogsapi-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: ogsapi
+Version: 0.3.0
+Summary: An API Wrapper for online-go.com, an online Go / Baduk server
+Author-email: Dakota Marshall <me@dakotamarshall.net>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # OGS Python Library
 
 
 [![pipeline status](https://gitlab.com/dakota.marshall/ogs-python/badges/prod/pipeline.svg)](https://gitlab.com/dakota.marshall/ogs-python/-/commits/prod)  [![Latest Release](https://gitlab.com/dakota.marshall/ogs-python/-/badges/release.svg)](https://gitlab.com/dakota.marshall/ogs-python/-/releases) [![PyPI version](https://badge.fury.io/py/ogsapi.svg)](https://badge.fury.io/py/ogsapi) 
 
 ## Summary
 
@@ -41,14 +53,22 @@
 
 ## Implemented API Functions
 *NOTE* All usernames are case sensitive
 ### User Functions
 
 - Get User vitals: `ogs.user_vitals()`
 - Get User Settings: `ogs.user_settings()`
+- Update User Settings: `ogs.update_user_settings()
+  - username: str
+  - first_name: str
+  - last_name: str
+  - country: str
+  - private_name: bool
+  - website: str
+  - about: str
 - Get User Games: `ogs.user_games()`
 - Get User Friends (Optionally search for user): `ogs.user_friends(username)`
 - Send friend request: `ogs.send_friend_request(username)`
 
 ### Player Functions
 
 - Get Player Info: `ogs.get_player(username)`
@@ -60,19 +80,34 @@
 ## Implemented Realtime API Functions
 
 - Get Host Info: `ogs.sock.host_info()`
 - Ping: `ogs.sock.ping()`
 - Connect To Notification Stream: `ogs.sock.notification_connect()`
 - Connect to Chat: `ogs.sock.chat_connect()`
 - Connect to a Game: `ogs.sock.game_connect(gameid: int)`
-  - This creates an object in the `ogs.sock.games` list with the key `game_id`
+  - This returns an object containing all the functions to handle received events from that game
+  - To be able to run code when a move is received, you need to register a callback function you made with: 
+  - `ogs.sock.games[game_id].register_callback(callback)`
 - Disconnect from a Game: `ogs.sock.game_disconnect(game_id)`
 
 ### Implemented Game Functions
 
 - Make a move: `ogs.sock.games[game_id].move('jj')`
+- Pass turn: `ogs.sock.games[game_id].pass_turn()`
+- Request an undo: `ogs.sock.games[game_id].undo()`
+- Resign: `ogs.sock.games[game_id].resign()`
+
+### Implemented Received Events
+
+- Getting gamedata: `ogs.sock.games[game_id].game_data`
+- Getting connection latency: `ogs.sock.games[game_id].latency`
+- Getting a move: `ogs.sock.games[game_id].callback_func['on_move']`
 
 
 ## To Implement
-TODO: Update this list
 
-- Pretty much everything
+- Implement callback function handling for:
+  - The clock
+  - Undo requested
+  - Undo Accepted
+- Implement proper challenge creation
+- Create open challenge
```

### Comparing `ogsapi-0.2.1/pyproject.toml` & `ogsapi-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,25 @@
   "setuptools>=42",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ogsapi"
-version = "0.2.1"
+version = "0.3.0"
 authors = [
   { name="Dakota Marshall", email="me@dakotamarshall.net" },
 ]
 description = "An API Wrapper for online-go.com, an online Go / Baduk server"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "python-engineio==3.13.2",
   "python-socketio==4.6.0",
+  "websocket-client",
   "requests"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `ogsapi-0.2.1/src/ogsapi/api.py` & `ogsapi-0.3.0/src/ogsapi/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import requests
 import urllib.parse
 import socketio
-import json
+from typing import Callable
 from time import sleep, time
 
 # TODO: This will eventually need to be moved to `termination-api` instead of `/api/v1/`
+# TODO: Should probably implement a user class that contains all user info and functions
 
 class OGSApiException(Exception):
     pass
 
 class OGSClient:
     def __init__(self, client_id, client_secret, username, password):
         self.client_id = client_id
         self.client_secret = client_secret
         self.username = username
         self.password = password
         self.access_token = None
+        # TODO:  Implement refresh token
         self.refresh_token = None
         self.user_id = None
         self.base_url = "https://online-go.com"
         self.api_ver = "v1"
 
         # Attempt authentication once everything is defined
         # TODO: Maybe implement some form of token caching, so we arent making new tokens every time the script runs
@@ -121,20 +123,43 @@
         endpoint = '/me'
         return self.get_rest_endpoint(endpoint)
     
     def user_settings(self):
         endpoint = '/me/settings/'
         return self.get_rest_endpoint(endpoint=endpoint)
     
-    #TODO: Allow for a good way to update settings appropriately.
-    def update_user_settings(self, payload: dict = None):
-        endpoint = '/me/settings/'
-        payload = {
-            'website' : 'https://example.com'
-        }
+    def update_user_settings(
+            self, username: str = None, 
+            first_name: str = None, 
+            last_name: str = None, 
+            private_name: bool = None, 
+            country: str = None, 
+            website: str = None,
+            about: str = None
+        ):
+
+        # This is a bit of a mess, but it works, should be refactored
+        payload = {}
+        if username is not None:
+            payload['username'] = username
+        if first_name is not None:
+            payload['first_name'] = first_name
+        if last_name is not None:
+            payload['last_name'] = last_name
+        if private_name is not None:
+            payload['real_name_is_private'] = private_name
+        if country is not None:
+            payload['country'] = country
+        if website is not None:
+            payload['website'] = website
+        if about is not None:
+            payload['about'] = about
+
+        endpoint = f'/players/{self.user_id}'
+        # Add the inputs to a payload, only if they are not None
         return self.put_rest_endpoint(endpoint=endpoint, payload=payload)
 
     def user_games(self):
         endpoint = '/me/games'
         return self.get_rest_endpoint(endpoint)
 
     def user_friends(self, username: str = None):
@@ -248,75 +273,95 @@
 
     def game_details(self, game_id):
         endpoint = f'/games/{game_id}'
         return self.get_rest_endpoint(endpoint)
 
 class OGSGame:
     # Class for handling each OGSGame connected via the OGSSocket
+    # To receive data from the game, use the callback function to register functions to be called when data is received.
+    # on_move and on_clock are required for the game to function properly, on_undo is only for handling undo requests
+    
     def __init__(self, game_socket, game_id, auth_data, user_data):
         self.socket = game_socket
         self.game_id = game_id
         self.user_data = user_data
         self.auth_data = auth_data
-        self.game_call_backs()
+        self._game_call_backs()
         self.connect()
         self.game_data = {}
         self.latency = 0
-    
+        self.callback_func = {
+            'on_move': None,
+            'on_clock': None,
+            'on_undo': None
+        }
+
     def __del__(self):
         self.disconnect()
 
-    def game_call_backs(self):
+    def register_callback(self, event: str, callback: Callable):
+        self.callback_func[event] = callback
+
+    # Low level socket functions
+    def _game_call_backs(self):
 
         @self.socket.on(f'game/{self.game_id}/move')
-        def on_game_move(data):
-            #TODO: Handle Moves
+        def _on_game_move(data):
             print(f"Got move: {data}")
-
+            self.callback_func['on_move'](data)
+            
         @self.socket.on(f'game/{self.game_id}/gamedata')
-        def on_game_data(data):
+        def _on_game_data(data):
             print(f'Got Gamedata: {data}')
             self.game_data = data
 
         @self.socket.on(f'game/{self.game_id}/clock')
-        def on_game_clock(data):
+        def _on_game_clock(data):
             #TODO: Need to create a game clock and sync clock with this event
             print(f'Got Clock: {data}')
 
         @self.socket.on(f'game/{self.game_id}/latency')
-        def on_game_latency(data):
+        def _on_game_latency(data):
             print(f'Got Latency: {data}')
             self.latency = data['latency']
 
         @self.socket.on(f'game/{self.game_id}/undo_requested')
-        def on_undo_requested(data):
+        def _on_undo_requested(data):
             #TODO: Handle This 
             print(f'Got Undo Request: {data}')
         
         @self.socket.on(f'game/{self.game_id}/undo_accepted')
-        def on_undo_accepted(data):
+        def _on_undo_accepted(data):
             #TODO: Handle This
             print(f'Got Accepted Undo: {data}')
-
+    
+    # Send functions
     def connect(self):
         print(f"Connecting to game {self.game_id}")
         self.socket.emit(event="game/connect", data={'game_id': self.game_id, 'player_id': self.user_data['id'], 'chat': False})
 
     def disconnect(self):
         print(f"Disconnecting game {self.game_id}")
         self.socket.emit(event="game/disconnect", data={'game_id': self.game_id})
 
     def move(self, move):
         print(f"Submitting move {move} to game {self.game_id}")
         self.socket.emit(event="game/move", data={'auth': self.auth_data['chat_auth'], 'player_id': self.user_data['id'], 'game_id': self.game_id, 'move': move})
 
-    #TODO: Needs Testing
     def resign(self):
         print(f"Resigning game {self.game_id}")
         self.socket.emit(event="game/resign", data={'auth': self.auth_data['chat_auth'], 'player_id': self.user_data['id'], 'game_id': self.game_id})  
+    
+    def undo(self):
+        print(f"Requesting undo on game {self.game_id}")
+        self.socket.emit(event="game/undo/request", data={'auth': self.auth_data['chat_auth'], 'player_id': self.user_data['id'], 'game_id': self.game_id})
+    
+    def pass_turn(self):
+        print(f'Submitting move pass to game {self.game_id}')
+        self.socket.emit(event="game/move", data={'auth': self.auth_data['chat_auth'], 'player_id': self.user_data['id'], 'game_id': self.game_id, 'move': '..'})
 
 class OGSSocket:
     def __init__(self, bearer_token: str):
         # Clock Settings
         self.clock_drift = 0.0
         self.clock_latency = 0.0
         self.last_ping = 0
@@ -397,13 +442,15 @@
     
     def chat_connect(self):
         self.socket.emit(event="chat/connect", data={"auth": self.auth_data['chat_auth'], "player_id": self.user_data['id'], "username": self.user_data['username']})
 
     def game_connect(self, game_id: int):
         self.games[game_id] = OGSGame(game_socket=self.socket, game_id=game_id, auth_data=self.auth_data, user_data=self.user_data)
 
+        return self.games[game_id]
+
     def game_disconnect(self, game_id: int):
         del self.games[game_id]
 
     def disconnect(self):
         self.socket.disconnect()
         print("Disconnected from WebSocket")
```

### Comparing `ogsapi-0.2.1/src/ogsapi.egg-info/PKG-INFO` & `ogsapi-0.3.0/src/ogsapi.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogsapi
-Version: 0.2.1
+Version: 0.3.0
 Summary: An API Wrapper for online-go.com, an online Go / Baduk server
 Author-email: Dakota Marshall <me@dakotamarshall.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -53,14 +53,22 @@
 
 ## Implemented API Functions
 *NOTE* All usernames are case sensitive
 ### User Functions
 
 - Get User vitals: `ogs.user_vitals()`
 - Get User Settings: `ogs.user_settings()`
+- Update User Settings: `ogs.update_user_settings()
+  - username: str
+  - first_name: str
+  - last_name: str
+  - country: str
+  - private_name: bool
+  - website: str
+  - about: str
 - Get User Games: `ogs.user_games()`
 - Get User Friends (Optionally search for user): `ogs.user_friends(username)`
 - Send friend request: `ogs.send_friend_request(username)`
 
 ### Player Functions
 
 - Get Player Info: `ogs.get_player(username)`
@@ -72,19 +80,34 @@
 ## Implemented Realtime API Functions
 
 - Get Host Info: `ogs.sock.host_info()`
 - Ping: `ogs.sock.ping()`
 - Connect To Notification Stream: `ogs.sock.notification_connect()`
 - Connect to Chat: `ogs.sock.chat_connect()`
 - Connect to a Game: `ogs.sock.game_connect(gameid: int)`
-  - This creates an object in the `ogs.sock.games` list with the key `game_id`
+  - This returns an object containing all the functions to handle received events from that game
+  - To be able to run code when a move is received, you need to register a callback function you made with: 
+  - `ogs.sock.games[game_id].register_callback(callback)`
 - Disconnect from a Game: `ogs.sock.game_disconnect(game_id)`
 
 ### Implemented Game Functions
 
 - Make a move: `ogs.sock.games[game_id].move('jj')`
+- Pass turn: `ogs.sock.games[game_id].pass_turn()`
+- Request an undo: `ogs.sock.games[game_id].undo()`
+- Resign: `ogs.sock.games[game_id].resign()`
+
+### Implemented Received Events
+
+- Getting gamedata: `ogs.sock.games[game_id].game_data`
+- Getting connection latency: `ogs.sock.games[game_id].latency`
+- Getting a move: `ogs.sock.games[game_id].callback_func['on_move']`
 
 
 ## To Implement
-TODO: Update this list
 
-- Pretty much everything
+- Implement callback function handling for:
+  - The clock
+  - Undo requested
+  - Undo Accepted
+- Implement proper challenge creation
+- Create open challenge
```

