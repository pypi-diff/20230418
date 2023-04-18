# Comparing `tmp/spotify_to_ytmusic-0.1.2.tar.gz` & `tmp/spotify_to_ytmusic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_to_ytmusic-0.1.2.tar", last modified: Sun Apr  9 19:29:00 2023, max compression
+gzip compressed data, was "spotify_to_ytmusic-0.1.3.tar", last modified: Tue Apr 18 21:04:33 2023, max compression
```

## Comparing `spotify_to_ytmusic-0.1.2.tar` & `spotify_to_ytmusic-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.662665 spotify_to_ytmusic-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.658666 spotify_to_ytmusic-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.658666 spotify_to_ytmusic-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-09 19:29:00.662665 spotify_to_ytmusic-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 19:29:00.662665 spotify_to_ytmusic-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.658666 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/match.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/settings.ini.example
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.662665 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-09 19:29:00.000000 spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 19:29:00.662665 spotify_to_ytmusic-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/tests/test_spotipy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 19:28:50.000000 spotify_to_ytmusic-0.1.2/tests/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.254796 spotify_to_ytmusic-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.246796 spotify_to_ytmusic-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.250796 spotify_to_ytmusic-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-18 21:04:33.254796 spotify_to_ytmusic-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:04:33.254796 spotify_to_ytmusic-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.250796 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/settings.ini.example
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.254796 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 21:04:33.000000 spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:33.254796 spotify_to_ytmusic-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/tests/test_spotipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:04:22.000000 spotify_to_ytmusic-0.1.3/tests/test_youtube.py
```

### Comparing `spotify_to_ytmusic-0.1.2/.github/workflows/coverage.yml` & `spotify_to_ytmusic-0.1.3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.2/.github/workflows/pythonpublish.yml` & `spotify_to_ytmusic-0.1.3/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.2/.gitignore` & `spotify_to_ytmusic-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.2/LICENSE` & `spotify_to_ytmusic-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.2/PKG-INFO` & `spotify_to_ytmusic-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_to_ytmusic
-Version: 0.1.2
+Version: 0.1.3
 Summary: Transfer Spotify playlists to YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spotify_to_ytmusic-0.1.2/README.rst` & `spotify_to_ytmusic-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.2/pyproject.toml` & `spotify_to_ytmusic-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/controllers.py` & `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/controllers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from datetime import datetime
 
 from spotify_to_ytmusic.setup import setup as setup_func
 from spotify_to_ytmusic.spotify import Spotify
 from spotify_to_ytmusic.ytmusic import YTMusicTransfer
 
 
@@ -64,14 +65,15 @@
 def update(args):
     spotify, ytmusic = _init()
     playlist = _get_spotify_playlist(spotify, args.playlist)
     playlistId = ytmusic.get_playlist_id(args.name)
     videoIds = ytmusic.search_songs(playlist["tracks"])
     if not args.append:
         ytmusic.remove_songs(playlistId)
+    time.sleep(2)
     ytmusic.add_playlist_items(playlistId, videoIds)
 
 
 def remove(args):
     ytmusic = YTMusicTransfer()
     ytmusic.remove_playlists(args.pattern)
```

### Comparing `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/main.py` & `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/main.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/match.py` & `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/match.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/settings.py` & `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/settings.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/setup.py` & `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 
 def setup(file: Optional[Path] = None):
     if file:
         setup_file(file)
         return
 
+    if not Settings.filepath.is_file():
+        shutil.copy(Settings.filepath.with_suffix(".ini.example"), Settings.filepath)
     choice = input("Choose which API to set up\n" "(1) Spotify\n" "(2) YouTube\n" "(3) both\n")
     choices = ["1", "2", "3"]
     if choice not in choices:
         sys.exit("Invalid choice")
 
     if choice == choices[0]:
         setup_spotify()
```

### Comparing `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/spotify.py` & `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/spotify.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 import html
+import string
 from urllib.parse import urlparse
 
 import spotipy
 from spotipy.oauth2 import SpotifyClientCredentials
 
 from spotify_to_ytmusic.settings import Settings
 
 
 class Spotify:
     def __init__(self):
         settings = Settings()
         conf = settings["spotify"]
+        client_id = conf["client_id"]
+
+        assert set(client_id).issubset(
+            string.hexdigits
+        ), f"Spotify client_id not set or invalid: {client_id}"
+        client_secret = conf["client_secret"]
+        assert set(client_secret).issubset(
+            string.hexdigits
+        ), f"Spotify client_secret not set or invalid: {client_secret}"
+
         client_credentials_manager = SpotifyClientCredentials(
-            client_id=conf["client_id"], client_secret=conf["client_secret"]
+            client_id=client_id, client_secret=client_secret
         )
         self.api = spotipy.Spotify(client_credentials_manager=client_credentials_manager)
 
     def getSpotifyPlaylist(self, url):
         playlistId = get_id_from_url(url)
         if len(playlistId) != 22:
             raise Exception(f"Bad playlist id: {playlistId}")
```

### Comparing `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic/ytmusic.py` & `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic/ytmusic.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 path = os.path.dirname(os.path.realpath(__file__)) + os.sep
 
 
 class YTMusicTransfer:
     def __init__(self):
         settings = Settings()
-        self.api = YTMusic(settings["youtube"]["headers"], settings["youtube"]["user_id"])
+        headers = settings["youtube"]["headers"]
+        assert headers.startswith("{"), "ytmusicapi headers not set or invalid"
+        self.api = YTMusic(headers, settings["youtube"]["user_id"])
 
     def create_playlist(self, name, info, privacy="PRIVATE", tracks=None):
         return self.api.create_playlist(name, info, privacy, video_ids=tracks)
 
     def search_songs(self, tracks):
         videoIds = []
         songs = list(tracks)
```

### Comparing `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/PKG-INFO` & `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-to-ytmusic
-Version: 0.1.2
+Version: 0.1.3
 Summary: Transfer Spotify playlists to YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `spotify_to_ytmusic-0.1.2/spotify_to_ytmusic.egg-info/SOURCES.txt` & `spotify_to_ytmusic-0.1.3/spotify_to_ytmusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.2/tests/test_cli.py` & `spotify_to_ytmusic-0.1.3/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,17 +44,15 @@
                 int(fakeOutput.getvalue().splitlines()[-1][0]) >= 2
             )  # assert number of lines deleted
 
     def test_setup(self):
         tmp_path = Path(__file__).parent.joinpath("settings.tmp")
         example_path = Settings.filepath.parent.joinpath("settings.ini.example")
         shutil.copy(example_path, tmp_path)
-        with mock.patch("sys.argv", ["", "setup"]), mock.patch(
-            "builtins.input", return_value="3"
-        ), mock.patch("spotify_to_ytmusic.settings.Settings.filepath", tmp_path):
+        with mock.patch("sys.argv", ["", "setup"]), mock.patch("builtins.input", return_value="3"):
             main()
             assert tmp_path.is_file()
             tmp_path.unlink()
 
         with mock.patch("sys.argv", ["", "setup", "--file", example_path.as_posix()]), mock.patch(
             "spotify_to_ytmusic.settings.Settings.filepath", tmp_path
         ):
```

### Comparing `spotify_to_ytmusic-0.1.2/tests/test_spotipy.py` & `spotify_to_ytmusic-0.1.3/tests/test_spotipy.py`

 * *Files identical despite different names*

