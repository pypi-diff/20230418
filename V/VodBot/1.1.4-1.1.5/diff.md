# Comparing `tmp/VodBot-1.1.4.tar.gz` & `tmp/VodBot-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VodBot-1.1.4.tar", last modified: Sun Jan 29 02:31:47 2023, max compression
+gzip compressed data, was "VodBot-1.1.5.tar", last modified: Mon Apr 17 22:33:43 2023, max compression
```

## Comparing `VodBot-1.1.4.tar` & `VodBot-1.1.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-01-29 02:31:47.549315 VodBot-1.1.4/
--rw-rw-rw-   0        0        0     1140 2022-12-17 05:25:09.000000 VodBot-1.1.4/LICENSE.md
--rw-rw-rw-   0        0        0     4320 2023-01-29 02:31:47.548809 VodBot-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3800 2023-01-28 02:09:38.000000 VodBot-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-01-29 02:31:47.511870 VodBot-1.1.4/VodBot.egg-info/
--rw-rw-rw-   0        0        0     4320 2023-01-29 02:31:47.000000 VodBot-1.1.4/VodBot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-01-29 02:31:47.000000 VodBot-1.1.4/VodBot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-29 02:31:47.000000 VodBot-1.1.4/VodBot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-01-29 02:31:47.000000 VodBot-1.1.4/VodBot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      198 2023-01-29 02:31:47.000000 VodBot-1.1.4/VodBot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-29 02:31:47.000000 VodBot-1.1.4/VodBot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-29 02:31:47.550322 VodBot-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-01-20 01:23:02.000000 VodBot-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-29 02:31:47.528609 VodBot-1.1.4/vodbot/
--rw-rw-rw-   0        0        0       47 2023-01-29 02:28:58.000000 VodBot-1.1.4/vodbot/__init__.py
--rw-rw-rw-   0        0        0     9038 2023-01-20 21:45:35.000000 VodBot-1.1.4/vodbot/__main__.py
--rw-rw-rw-   0        0        0     3843 2023-01-20 19:40:58.000000 VodBot-1.1.4/vodbot/cache.py
--rw-rw-rw-   0        0        0     7072 2023-01-20 19:40:58.000000 VodBot-1.1.4/vodbot/chatlog.py
-drwxrwxrwx   0        0        0        0 2023-01-29 02:31:47.540720 VodBot-1.1.4/vodbot/commands/
--rw-rw-rw-   0        0        0        0 2022-12-16 02:49:49.000000 VodBot-1.1.4/vodbot/commands/__init__.py
--rw-rw-rw-   0        0        0     3319 2023-01-29 02:26:17.000000 VodBot-1.1.4/vodbot/commands/export.py
--rw-rw-rw-   0        0        0     3433 2023-01-20 20:08:55.000000 VodBot-1.1.4/vodbot/commands/info.py
--rw-rw-rw-   0        0        0     1601 2023-01-21 05:15:39.000000 VodBot-1.1.4/vodbot/commands/init.py
--rw-rw-rw-   0        0        0     7785 2023-01-29 01:43:03.000000 VodBot-1.1.4/vodbot/commands/pull.py
--rw-rw-rw-   0        0        0    21507 2023-01-28 02:09:38.000000 VodBot-1.1.4/vodbot/commands/stage.py
--rw-rw-rw-   0        0        0    11117 2023-01-29 01:41:31.000000 VodBot-1.1.4/vodbot/commands/upload.py
--rw-rw-rw-   0        0        0    16003 2023-01-29 01:41:31.000000 VodBot-1.1.4/vodbot/config.py
-drwxrwxrwx   0        0        0        0 2023-01-29 02:31:47.547246 VodBot-1.1.4/vodbot/itd/
--rw-rw-rw-   0        0        0       68 2022-12-16 02:49:49.000000 VodBot-1.1.4/vodbot/itd/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-01-29 01:43:19.000000 VodBot-1.1.4/vodbot/itd/download.py
--rw-rw-rw-   0        0        0     4388 2022-12-16 02:49:49.000000 VodBot-1.1.4/vodbot/itd/gql.py
--rw-rw-rw-   0        0        0     3229 2023-01-28 02:09:38.000000 VodBot-1.1.4/vodbot/itd/worker.py
--rw-rw-rw-   0        0        0     1213 2023-01-20 01:23:02.000000 VodBot-1.1.4/vodbot/printer.py
--rw-rw-rw-   0        0        0     5060 2023-01-28 02:09:38.000000 VodBot-1.1.4/vodbot/thumbnail.py
--rw-rw-rw-   0        0        0     9810 2022-12-17 05:25:09.000000 VodBot-1.1.4/vodbot/twitch.py
--rw-rw-rw-   0        0        0     4024 2023-01-28 02:09:38.000000 VodBot-1.1.4/vodbot/util.py
--rw-rw-rw-   0        0        0     3243 2023-01-27 05:41:06.000000 VodBot-1.1.4/vodbot/video.py
--rw-rw-rw-   0        0        0     6052 2023-01-20 01:23:02.000000 VodBot-1.1.4/vodbot/webhook.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:33:43.595310 VodBot-1.1.5/
+-rw-rw-rw-   0        0        0     1140 2022-12-17 05:25:09.000000 VodBot-1.1.5/LICENSE.md
+-rw-rw-rw-   0        0        0     4208 2023-04-17 22:33:43.594800 VodBot-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3688 2023-02-01 04:16:24.000000 VodBot-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 22:33:43.551659 VodBot-1.1.5/VodBot.egg-info/
+-rw-rw-rw-   0        0        0     4208 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      198 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-17 22:33:43.000000 VodBot-1.1.5/VodBot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 22:33:43.595310 VodBot-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-01-20 01:23:02.000000 VodBot-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:33:43.568876 VodBot-1.1.5/vodbot/
+-rw-rw-rw-   0        0        0       47 2023-04-17 22:32:08.000000 VodBot-1.1.5/vodbot/__init__.py
+-rw-rw-rw-   0        0        0     9038 2023-01-20 21:45:35.000000 VodBot-1.1.5/vodbot/__main__.py
+-rw-rw-rw-   0        0        0     3843 2023-01-20 19:40:58.000000 VodBot-1.1.5/vodbot/cache.py
+-rw-rw-rw-   0        0        0     7165 2023-01-30 04:24:10.000000 VodBot-1.1.5/vodbot/chatlog.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:33:43.589673 VodBot-1.1.5/vodbot/commands/
+-rw-rw-rw-   0        0        0        0 2022-12-16 02:49:49.000000 VodBot-1.1.5/vodbot/commands/__init__.py
+-rw-rw-rw-   0        0        0     3799 2023-01-29 07:37:06.000000 VodBot-1.1.5/vodbot/commands/export.py
+-rw-rw-rw-   0        0        0     3433 2023-01-20 20:08:55.000000 VodBot-1.1.5/vodbot/commands/info.py
+-rw-rw-rw-   0        0        0     1601 2023-01-21 05:15:39.000000 VodBot-1.1.5/vodbot/commands/init.py
+-rw-rw-rw-   0        0        0     7901 2023-04-17 22:07:30.000000 VodBot-1.1.5/vodbot/commands/pull.py
+-rw-rw-rw-   0        0        0    21509 2023-04-17 22:27:24.000000 VodBot-1.1.5/vodbot/commands/stage.py
+-rw-rw-rw-   0        0        0    12980 2023-04-17 22:18:15.000000 VodBot-1.1.5/vodbot/commands/upload.py
+-rw-rw-rw-   0        0        0    16412 2023-04-17 22:27:35.000000 VodBot-1.1.5/vodbot/config.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:33:43.593791 VodBot-1.1.5/vodbot/itd/
+-rw-rw-rw-   0        0        0       68 2022-12-16 02:49:49.000000 VodBot-1.1.5/vodbot/itd/__init__.py
+-rw-rw-rw-   0        0        0     3359 2023-04-17 22:07:30.000000 VodBot-1.1.5/vodbot/itd/download.py
+-rw-rw-rw-   0        0        0     4374 2023-01-30 04:07:09.000000 VodBot-1.1.5/vodbot/itd/gql.py
+-rw-rw-rw-   0        0        0     3298 2023-04-17 22:07:30.000000 VodBot-1.1.5/vodbot/itd/worker.py
+-rw-rw-rw-   0        0        0     1213 2023-01-20 01:23:02.000000 VodBot-1.1.5/vodbot/printer.py
+-rw-rw-rw-   0        0        0     5060 2023-01-28 02:09:38.000000 VodBot-1.1.5/vodbot/thumbnail.py
+-rw-rw-rw-   0        0        0    10202 2023-01-30 04:19:30.000000 VodBot-1.1.5/vodbot/twitch.py
+-rw-rw-rw-   0        0        0     4024 2023-01-28 02:09:38.000000 VodBot-1.1.5/vodbot/util.py
+-rw-rw-rw-   0        0        0     3248 2023-01-29 07:28:46.000000 VodBot-1.1.5/vodbot/video.py
+-rw-rw-rw-   0        0        0     6052 2023-01-20 01:23:02.000000 VodBot-1.1.5/vodbot/webhook.py
```

### Comparing `VodBot-1.1.4/LICENSE.md` & `VodBot-1.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.4/PKG-INFO` & `VodBot-1.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VodBot
-Version: 1.1.4
+Version: 1.1.5
 Summary: Twitch VOD and Clip manager
 Home-page: https://github.com/FriendTeamInc/VodBot
 Author: Logan "NotQuiteApex" Hickok-Dickson
 Author-email: self@notquiteapex.net
 License: MIT
 Project-URL: Homepage, https://github.com/FriendTeamInc/VodBot
 Project-URL: Bug Tracker, https://github.com/FriendTeamInc/VodBot/issues
@@ -18,15 +18,14 @@
 
 VodBot is command line VOD and Clip manager for Twitch. Vodbot can:
 * Grab info on any public VOD, Clip, or Channel on Twitch.
 * Download any public VOD or Clip from Twitch, along with useful metadata and chatlogs.
 * Slice and splice videos downloaded into instances of staged data.
 * Export staged data, one at a time or all at once, with chat logs as subtitles synced with the video and programmatically generated thumbnails.
 * Upload staged data, one at a time or all at once, to YouTube with chat logs as subtitles synced with the video and programmatically generated thumbnails.
-	* NOTE: Requires approval and credentials from Google, for now just use export and upload the video manually.
 * Bash tab completion, for quickly putting in commands and referencing saved videos or staged data.
     * NOTE: Available through the argcomplete package, see its repo for more details. Requires `eval "$(register-python-argcomplete vodbot)"` to be placed in an appropriate location such as `~/.bashrc` after installation.
 * Send webhooks to Discord to help you keep tabs on what VodBot is up to.
 
 ...with more features to come!
 
 # Installation
```

### Comparing `VodBot-1.1.4/README.md` & `VodBot-1.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 VodBot is command line VOD and Clip manager for Twitch. Vodbot can:
 * Grab info on any public VOD, Clip, or Channel on Twitch.
 * Download any public VOD or Clip from Twitch, along with useful metadata and chatlogs.
 * Slice and splice videos downloaded into instances of staged data.
 * Export staged data, one at a time or all at once, with chat logs as subtitles synced with the video and programmatically generated thumbnails.
 * Upload staged data, one at a time or all at once, to YouTube with chat logs as subtitles synced with the video and programmatically generated thumbnails.
-	* NOTE: Requires approval and credentials from Google, for now just use export and upload the video manually.
 * Bash tab completion, for quickly putting in commands and referencing saved videos or staged data.
     * NOTE: Available through the argcomplete package, see its repo for more details. Requires `eval "$(register-python-argcomplete vodbot)"` to be placed in an appropriate location such as `~/.bashrc` after installation.
 * Send webhooks to Discord to help you keep tabs on what VodBot is up to.
 
 ...with more features to come!
 
 # Installation
```

### Comparing `VodBot-1.1.4/VodBot.egg-info/PKG-INFO` & `VodBot-1.1.5/VodBot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VodBot
-Version: 1.1.4
+Version: 1.1.5
 Summary: Twitch VOD and Clip manager
 Home-page: https://github.com/FriendTeamInc/VodBot
 Author: Logan "NotQuiteApex" Hickok-Dickson
 Author-email: self@notquiteapex.net
 License: MIT
 Project-URL: Homepage, https://github.com/FriendTeamInc/VodBot
 Project-URL: Bug Tracker, https://github.com/FriendTeamInc/VodBot/issues
@@ -18,15 +18,14 @@
 
 VodBot is command line VOD and Clip manager for Twitch. Vodbot can:
 * Grab info on any public VOD, Clip, or Channel on Twitch.
 * Download any public VOD or Clip from Twitch, along with useful metadata and chatlogs.
 * Slice and splice videos downloaded into instances of staged data.
 * Export staged data, one at a time or all at once, with chat logs as subtitles synced with the video and programmatically generated thumbnails.
 * Upload staged data, one at a time or all at once, to YouTube with chat logs as subtitles synced with the video and programmatically generated thumbnails.
-	* NOTE: Requires approval and credentials from Google, for now just use export and upload the video manually.
 * Bash tab completion, for quickly putting in commands and referencing saved videos or staged data.
     * NOTE: Available through the argcomplete package, see its repo for more details. Requires `eval "$(register-python-argcomplete vodbot)"` to be placed in an appropriate location such as `~/.bashrc` after installation.
 * Send webhooks to Discord to help you keep tabs on what VodBot is up to.
 
 ...with more features to come!
 
 # Installation
```

### Comparing `VodBot-1.1.4/VodBot.egg-info/SOURCES.txt` & `VodBot-1.1.5/VodBot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.4/setup.py` & `VodBot-1.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.4/vodbot/__main__.py` & `VodBot-1.1.5/vodbot/__main__.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.4/vodbot/cache.py` & `VodBot-1.1.5/vodbot/cache.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.4/vodbot/chatlog.py` & `VodBot-1.1.5/vodbot/chatlog.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,23 +90,28 @@
 	return userlist, userorder
 
 
 def chat_to_listwithbounds(msgs: List[ChatMessage], vid_duration:int, msg_duration:int) -> List[dict]:
 	# First we run through all the messages and see what needs showing and what doesn't
 	chat_lists = []
 	# this is so cursed
+	# we walk through each second and check if a message should be displayed during its duration on screen
 	last_msgs: List[ChatMessage] = []
 	for t in range(vid_duration):
 		current_msgs: List[ChatMessage] = []
 		for m in msgs:
-			if t <= m.offset < t+msg_duration:
+			if t < m.offset or m.offset+msg_duration < t:
+				# time is before the offset OR
+				# time is after the offset plus its screen duration
+				continue
+			# elif m.offset <= t <= m.offset+msg_duration:
+			else:
 				current_msgs.append(m)
-			elif m.offset >= t+msg_duration:
-				break
 		
+		# check if the messages we need to display has changed
 		if current_msgs != last_msgs:
 			# write line and overwrite last_msgs
 			last_msgs = current_msgs
 			write = {"begin": t, "end": vid_duration, "msgs":[], "break":False}
 			if len(current_msgs) != 0:
 				# write full messages line
 				for m in current_msgs:
@@ -188,15 +193,14 @@
 		# finish up
 		f.write("</body></timedtext>")
 
 
 def process_stage(conf: Config, stage: StageData, mode:str) -> Path:
 	tempdir = Path(conf.directories.temp)
 
-	#cprint(f"#rLoading all chat messages for `#fM{stage.id}#r`.", end="")
 	total_offset = 0
 	chat_list = []
 	for slc in stage.slices:
 		# load up each stagedata's meta to see if chat exists
 		metapath = slc.filepath[:-4] + ".meta"
 		meta = None
 		with open(metapath, "r") as f:
@@ -219,24 +223,21 @@
 			chat_list += msg_list
 		
 		# now take each stage's duration and apply it to the next chat list's
 		total_offset += end_sec - start_sec
 
 	# determine how to export, then return the resultant path
 	if mode != "upload" and mode != "export":
-		util.exit_prog(94, f"Cannot export chat with export mode {mode}")
+		util.exit_prog(94, f"Cannot export chat with export mode {mode}.")
 	
 	export_type = conf.chat.export_format if mode != "upload" else "YTT"
 
 	if len(chat_list) == 0:
-		#cprint(f" No chat found in `#fM{stage.id}#r` stage. Skipping...")
 		return None
 
-	#cprint(f" Exporting as format `#fY{export_type}#r`.")
-
 	returnpath = None
 	if export_type == "raw":
 		# chat to logfile time
 		returnpath = tempdir / f"{stage.id}.chat"
 		chat_to_logfile(chat_list, str(returnpath))
 	elif export_type == "YTT":
 		# load from archive, parse and write to temp
```

### Comparing `VodBot-1.1.4/vodbot/commands/export.py` & `VodBot-1.1.5/vodbot/commands/export.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,39 +15,46 @@
 from pathlib import Path
 from os import remove as os_remove
 from shutil import move as shutil_move
 
 
 DISALLOWED_CHARACTERS = [
 	"/", "\\", "<", ">", ":",
-	"\"", "|", "?", "*"
+	"\"", "\'", "|", "?", "*"
 ]
 
 
 EPOCH = datetime.utcfromtimestamp(0)
 def sort_stagedata(stagedata):
 	date = datetime.strptime(stagedata.datestring, "%Y/%m/%d")
 	return (date - EPOCH).total_seconds()
 
 
 def handle_stage(conf: Config, stage: StageData) -> Path:
+	# handle not having videos to process
+	if not all(Path(x.filepath).is_file() for x in stage.slices):
+		lost_vids = [x.video_id for x in stage.slices if Path(x.filepath).is_file()]
+		cprint(f"#d#fYWARN: Skipping stage video `{stage.id}`, failed to find video(s) with ID(s) of `{lost_vids}`.#r")
+		send_export_error(f'For stage video "{stage.id}", failed to find video(s) with ID(s) "{lost_vids}".')
+		return None
+
 	tmpfile = None
 	try:
 		tmpfile = vbvid.process_stage(conf, stage)
 	except vbvid.FailedToSlice as e:
-		cprint(f"#r#fRSkipping stage `{stage.id}`, failed to slice video with ID of `{e.video_id}`.#r\n")
-		send_export_error(f'For stage "{stage.id}", failed to slice video with ID "{e.video_id}".')
+		cprint(f"#d#fYWARN: Skipping stage video `{stage.id}`, failed to slice video with ID of `{e.video_id}`.#r")
+		send_export_error(f'For stage video "{stage.id}", failed to slice video with ID "{e.video_id}".')
 		return None
 	except vbvid.FailedToConcat:
-		cprint(f"#r#fRSkipping stage `{stage.id}`, failed to concatenate videos.#r\n")
-		send_export_error(f'For stage "{stage.id}", failed to concatenate videos.')
+		cprint(f"#d#fYWARN: Skipping stage video `{stage.id}`, failed to concatenate videos.#r")
+		send_export_error(f'For stage video "{stage.id}", failed to concatenate videos.')
 		return None
 	except vbvid.FailedToCleanUp as e:
-		cprint(f"#r#fRSkipping stage `{stage.id}`, failed to clean up temporary files.#r\n\n{e.vid}")
-		send_export_error(f'For stage "{stage.id}", failed to clean up temporary files.')
+		cprint(f"#d#fYWARN: Skipping stage video `{stage.id}`, failed to clean up temporary files.#r\n{e.video_id}")
+		send_export_error(f'For stage video "{stage.id}", failed to clean up temporary files.')
 		return None
 	
 	return tmpfile
 
 
 def run(args):
 	conf = util.load_conf(args.config)
```

### Comparing `VodBot-1.1.4/vodbot/commands/info.py` & `VodBot-1.1.5/vodbot/commands/info.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.4/vodbot/commands/init.py` & `VodBot-1.1.5/vodbot/commands/init.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.4/vodbot/commands/pull.py` & `VodBot-1.1.5/vodbot/commands/pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,18 +103,20 @@
 		cprint(f"Total #fMvideos#r to pull: #fC#l{totalvods+totalclips}#r")
 	elif atvods:
 		cprint(f"Total #fMVODs#r to pull: #fC#l{totalvods}#r")
 	elif atclips:
 		cprint(f"Total #fMClips#r to pull: #fC#l{totalclips}#r")
 
 	# Download all the videos we need.
-	cprint("#r#dPulling videos...#r", flush=True)
+	if totalvods > 0 or totalclips > 0:
+		cprint("#r#dPulling videos...#r", flush=True)
 	fin_vods = fin_clips = all_vods = all_clips = 0
 	for channel in channels:
-		if len(channel.new_vods) > 0 or len(channel.new_clips) > 0:
+		if ((hasattr(channel, "new_vods") and len(channel.new_vods) > 0) or
+			(hasattr(channel, "new_clips") and len(channel.new_clips) > 0)):
 			cprint(f"Pulling videos for #fY#l{channel.display_name}#r...")
 		else:
 			continue
 
 		voddir = VODS_DIR / channel.login
 		all_vods += len(channel.new_vods)
 		for vod in channel.new_vods:
```

### Comparing `VodBot-1.1.4/vodbot/commands/stage.py` & `VodBot-1.1.5/vodbot/commands/stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 			if len(metas) > 0:
 				vid_id = metas[0] # use first result of matching
 				metajson = None
 				try:
 					with open(folder / f"{vid_id}.meta") as f:
 						metajson = json.load(f)
 					filename = folder / f"{metajson['created_at']}_{metajson['id']}.mkv".replace(":", ";")
-					return (filename, metajson, "VOD" if dir_t[1] == voddir else "Clip")
+					return (filename, metajson) #, "VOD" if dir_t[1] == voddir else "Clip")
 				except FileNotFoundError:
 					pass
 				except ValueError:
 					pass
 	
 	raise CouldntFindVideo()
 
@@ -460,19 +460,18 @@
 			game = ""
 			continue
 	
 	return game
 
 
 def check_thumbnail_text() -> str:
-	text = ""
-
-	while not text:
-		text = input(colorize(f"#fW#lEnter the text you want in the thumbnail#r: "))
-		# TODO: check text?
+	# text = ""
+	# while not text:
+	# 	# TODO: check text?
+	text = input(colorize(f"#fW#lEnter the text you want in the thumbnail#r: "))
 	
 	return text
 
 
 def check_thumbnail_vid_id(possible_slices: List[VideoSlice]) -> int:
 	vid = ""
 
@@ -525,22 +524,22 @@
 	
 	# Get what streamers were involved (usernames), only asked if args is not full
 	if not args.streamer:
 		default_streamers = args.streamer
 		for f in videos:
 			if f["meta"]["user_login"] not in default_streamers:
 				default_streamers.append(f["meta"]["user_login"])
-		args.streamers = check_streamers(default=default_streamers, conf_users=[chan.username for chan in conf.channels])
+		args.streamer = check_streamers(default=default_streamers, conf_users=[chan.username for chan in conf.channels])
 
 	# get title
 	if not args.title:
 		args.title = check_title(default=None)
 
 	# get description
-	formatdict, datestring = create_format_dict(conf, args.streamers, utcdate=metadata["created_at"])
+	formatdict, datestring = create_format_dict(conf, args.streamer, utcdate=metadata["created_at"])
 	args.desc = check_description(formatdict, inputdefault=args.desc)
 
 	# get timestamps for each video through input
 	for x in range(len(videos)):
 		# skip times we dont need because we already have them
 		if x < len(args.ss):
 			# lied we need to check and convert the times
@@ -638,18 +637,18 @@
 			timestamp = testtimestamp
 		else:
 			timestamp = check_thumbnail_timestamp()
 
 		tn = ThumbnailData(heads=heads, game=game, text=text, video_slice_id=vid_id, timestamp=timestamp)
 
 	# make stage object
-	stage = StageData(streamers=args.streamers, title=args.title, desc=args.desc, datestring=datestring, slices=slices, thumbnail=tn)
+	stage = StageData(streamers=args.streamer, title=args.title, desc=args.desc, datestring=datestring, slices=slices, thumbnail=tn)
 	# Check that new "id" does not collide
 	while check_stage_id(stage.id, STAGE_DIR):
-		stage = StageData(streamers=args.streamers, title=args.title, desc=args.desc, datestring=datestring, slices=slices, thumbnail=tn)
+		stage = StageData(streamers=args.streamer, title=args.title, desc=args.desc, datestring=datestring, slices=slices, thumbnail=tn)
 
 	# shorter file name
 	#shortfile = stage.filename.replace(VODS_DIR, "$vods").replace(CLIPS_DIR, "$clips")
 
 	cprint(f"#r`#fC{stage.title}#r` #fM{' '.join(stage.streamers)}#r #d({stage.id})#r")
 	cprint(f"#d#fG{stage.desc}#r")
 	for vid in stage.slices:
```

### Comparing `VodBot-1.1.4/vodbot/commands/upload.py` & `VodBot-1.1.5/vodbot/commands/upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 import vodbot.thumbnail as vbthumbnail
 from vodbot.util import exit_prog, load_conf, format_size
 from vodbot.cache import load_cache, save_cache
 from vodbot.printer import cprint
 from vodbot.config import Config
 from vodbot.webhook import init_webhooks, send_upload_error, send_upload_video, send_upload_job_done
 
+import base64
+import requests
 import json
 from datetime import datetime
 from os import remove as os_remove
 from os.path import exists as os_exists
 from time import sleep
 from typing import List
 
@@ -129,15 +131,15 @@
 	# create media file, upload in chunks
 	media_file = MediaFileUpload(str(tmpfile), chunksize=conf.upload.chunk_size, resumable=True)
 
 	# create upload request and execute
 	response_upload = service.videos().insert(
 		part="snippet,status",
 		body=request_body,
-		notifySubscribers=False,
+		notifySubscribers=Config.upload.notify_subscribers,
 		media_body=media_file
 	)
 
 	filesize = media_file.size()
 
 	cprint(f"#c#fCUploading stage video #r`#fM{stagedata.id}#r`: #fC0#fY%#r #d(0/{format_size(filesize)})...#r", end="\r")
 	uploaded = _upload_artifact(f"stage video #r`#fM{stagedata.id}#r`", response_upload, getting_video=True, filesize=filesize)
@@ -222,14 +224,67 @@
 		os_remove(str(tmpfile))
 	except Exception as e:
 		exit_prog(90, f"Failed to remove temp thumbnail file of stage `{stagedata.id}` after upload. {e}")
 
 	return uploaded
 
 
+def _download_credentials(conf: Config) -> None:
+	CLIENT_FILE = conf.upload.client_path
+	CLIENT_FILE_URL = conf.upload.client_url
+
+	# download the credentials
+	try:
+		r = requests.get(CLIENT_FILE_URL)
+		r.raise_for_status()
+		decoded = base64.b64decode(r.content, validate=True)
+		with open(CLIENT_FILE, "wb") as f:
+			f.write(decoded)
+	except (requests.HTTPError, requests.ConnectionError, requests.Timeout, requests.TooManyRedirects) as e:
+		exit_prog(13, f"Failed to GET credentials from url `{conf.upload.client_url}`, error: \n{e}")
+	except base64.binascii.Error as e:
+		exit_prog(13, f"Failed to decode downloaded credentials, error: \n{e}")
+	except IOError as e:
+		exit_prog(13, f"Failed to write credentials to path `{conf.upload.client_path}`, error: \n{e}")
+	except Exception as e:
+		exit_prog(13, f"Unknown exception occurred when pulling YouTube credentials, error: \n{e}")
+
+
+def get_credentials(conf:Config, SCOPES:List[str]) -> Credentials:
+	CLIENT_FILE = conf.upload.client_path
+	got_new_creds = False
+
+	if not CLIENT_FILE.is_file():
+		if CLIENT_FILE.exists():
+			exit_prog(12, f"Something that isn't a file exists at `{CLIENT_FILE}` and should be removed.")
+		else:
+			cprint("#dDownloading new credentials...")
+			_download_credentials(conf)
+			got_new_creds = True
+	else:
+		cprint()
+
+	creds = None
+
+	cprint("#dNOTE: If Google gives an error, you will need to exit and check `client_url` in your configuration.")
+	try:
+		flow = InstalledAppFlow.from_client_secrets_file(CLIENT_FILE, SCOPES)
+		creds = flow.run_local_server(port=conf.upload.oauth_port)
+	except KeyboardInterrupt as e:
+		# credentials were trash, we need to reset them
+		if got_new_creds:
+			cprint("#d#fYWARN: Exited during OAuth authentication with brand new credentials, deleting credentials assuming they are bad.")
+			os_remove(CLIENT_FILE)
+		raise e
+
+	# add a check to the above functions for if the credentials are invalid.
+	# should also add a flag for if they were already downloaded so we can shortcut to an error that the new credentials are already bad and delete them
+
+	return creds
+
 def run(args):
 	# load config
 	conf = load_conf(args.config)
 	cache = load_cache(conf, args.cache_toggle)
 	init_webhooks(conf)
 
 	# configure variables
@@ -263,50 +318,45 @@
 		stagedatas = StageData.load_all_stages(STAGE_DIR)
 		stagedatas.sort(key=sort_stagedata)
 	else:
 		cprint("#dLoading stage...", end=" ")
 		# check if stage exists, and prep it for upload
 		stagedatas = [StageData.load_from_id(STAGE_DIR, args.id)]
 
-	# authenticate youtube service
-	if not os_exists(CLIENT_FILE):
-		exit_prog(19, "Missing YouTube Client ID/Secret file.")
-
 	cprint("Authenticating with Google...", end=" ")
 
 	service: Resource = None
 	creds = None
 
 	if os_exists(SESSION_FILE):
 		creds = Credentials.from_authorized_user_file(SESSION_FILE, SCOPES)
 	
 	if not creds or not creds.valid:
 		try:
 			if creds and creds.expired and creds.refresh_token:
 				creds.refresh(Request())
 			else:
-				flow = InstalledAppFlow.from_client_secrets_file(CLIENT_FILE, SCOPES)
-				creds = flow.run_local_server(port=conf.upload.oauth_port)
+				creds = get_credentials(conf, SCOPES)
 		except RefreshError:
-			flow = InstalledAppFlow.from_client_secrets_file(CLIENT_FILE, SCOPES)
-			creds = flow.run_local_server(port=conf.upload.oauth_port)
+			creds = get_credentials(conf, SCOPES)
 		
 		with open(SESSION_FILE, "w") as f:
 			f.write(creds.to_json())
 	
 	try:
 		service = build(API_NAME, API_VERSION, credentials=creds)
 	except Exception as err:
 		exit_prog(50, f"Failed to connect to YouTube API, \"{err}\".")
 	
-	cprint("Authenticated.", end=" ")
+	cprint("done.#r")
 	
 	# begin to upload
 	finished_jobs = 0
-	cprint(f"About to upload {len(stagedatas)} stage(s).#r")
+	cprint(f"#dAbout to upload {len(stagedatas)} stage(s).#r")
+  
 	for stage in stagedatas:
 		video_id = upload_video(conf, service, stage)
 		if video_id is not None:
 			if conf.upload.thumbnail_enable:
 				if not upload_thumbnail(conf, service, stage, video_id):
 					t = f"Failed to upload video thumbnail for stage `{stage.id}`, video ID `{video_id}`."
 					cprint(f"#fY#dWARN: {t} Skipping...#r")
```

### Comparing `VodBot-1.1.4/vodbot/config.py` & `VodBot-1.1.5/vodbot/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 	
 	# https://github.com/arcusmaximus/YTSubConverter/blob/master/ytt.ytt
 	# Caption alignment within its box in the YouTube player.
 	# Possible values are "left", "right", and "center". Defaults to "left".
 	ytt_align: str = field(default="left", metadata=config(mm_field=fields.Str(
 		validate=validate.OneOf(["left", "right", "center"]))))
 	# Caption anchor point, or its origin point. Can be any integer from 0 to 8.
-	# For example, 0 is top left, 4 is dead center, 8 is bottom right. Defaults to 6 (aka bottom left).
+	# For example, 0 is top left, 4 is dead center, 8 is bottom right. Defaults to 6 (bottom left).
 	ytt_anchor: int = field(default=6, metadata=config(mm_field=fields.Int(
 		validate=validate.Range(0, 8))))
 	# Position in the YouTube player that the captions appear, horizontally.
 	# Can be any integer from 0 (left) to 100 (right). Defaults to 0.
 	ytt_position_x: int = field(default=0, metadata=config(mm_field=fields.Int(
 		validate=validate.Range(0, 100))))
 	# Position in the YouTube player that the captions appear, vertically.
@@ -134,14 +134,15 @@
 	# the program directs it to manage video files. "warning" is recommended as it displays very
 	# little unless otherwise necessary.
 	ffmpeg_loglevel: str = field(default="warning", metadata=config(mm_field=fields.Str(
 		validate=validate.OneOf(["warning", "error", "fatal"]))))
 	# This is used to tell FFmpeg where to output the logs. It goes from FFmpeg's stderr to wherever
 	# described with this path. If no path is specified, it will be piped to /dev/null (or whatever
 	# is equivalent on your system).
+	# TODO: change this to a toggle for just silencing the output
 	ffmpeg_stderr: Path = field(default=Path(), metadata=_path_field_config)
 
 	# A simple toggle for managing whether chat is exported with a stage, if available. More
 	# options are available in the chat config section.
 	chat_enable: bool = True
 	# A simple toggle for managing whether video is exported with a stage. Useful for if you
 	# just need the chat logs.
@@ -156,21 +157,26 @@
 class _ConfigUpload:
 	# Toggle for uploading chat logs as closed captions.
 	chat_enable: bool = True
 	# Toggle for uploading generated thumbnails with the videos.
 	thumbnail_enable: bool = True
 	# Path for client JSON, the credentials needed for using the YouTube API.
 	client_path: Path = field(default=DEFAULT_CONFIG_DIRECTORY/"yt-client.json", metadata=_path_field_config)
+	# URL for getting the YouTube credentials for uploading.
+	client_url: str = field(default="https://www.friendteam.biz/assets/vodbot-youtube-credentials")
 	# Path for session JSON, the "cookies" for the logged-in YouTube account to upload videos to.
 	session_path: Path = field(default=DEFAULT_CONFIG_DIRECTORY/"yt-session.json", metadata=_path_field_config)
 	# Size of chunks of uploaded data in bytes, with a minimum of 262144. It's recommended that this
 	# size be a multiple of this minimum value.
 	chunk_size: int = field(default=262144, metadata=config(mm_field=fields.Int(validate=validate.Range(262144))))
 	# Port for the OAuth local server to run on, used for logging into Google's services.
 	oauth_port: int = field(default=8080, metadata=config(mm_field=fields.Int(validate=validate.Range(0, 65535))))
+	# Toggle for if uploaded videos should be pushed to subscription feeds and notify users of new
+	# uploads (if they have the notification bell enabled)
+	notify_subscribers: bool = True
 
 @dataclass_json
 @dataclass
 class _ConfigThumbnailIcon:
 	# Offset/origin position of the image.
 	ox: int
 	oy: int
@@ -209,16 +215,17 @@
 	cover_position: _ConfigThumbnailPosition = field(default_factory=lambda: _ConfigThumbnailPosition())
 	# Path of the "cover art" image. This path is always relative to the thumbnail directory.
 	cover_filepath: Path = field(default_factory=lambda: Path(), metadata=_path_field_config)
 
 	# Position settings of the text.
 	text_position: _ConfigThumbnailPosition = field(default_factory=lambda: _ConfigThumbnailPosition())
 	# The specific font to use when printing text on the thumbnail.
-	# This can be a relative or absolute path. If the path is relative, then locations are checked in this order:
-	# 1. Thumbnail directory, 2. System locations, 3. Path relative to execution (not recommended for use)
+	# This can be a relative or absolute path. If the path is relative, then locations are checked
+	# in this order: 1. Thumbnail directory, 2. System locations, 3. Path relative to execution
+	# (not recommended for use)
 	text_font: str = ""
 	# The font pointsize to use when printing text on the thumbnail.
 	text_size: int = 48
 
 	# A list of positions that heads will be placed at. Extra options such as offset and scale are
 	# accounted for as well.
 	head_positions: List[_ConfigThumbnailPosition] = field(default_factory=lambda: [])
```

### Comparing `VodBot-1.1.4/vodbot/itd/download.py` & `VodBot-1.1.5/vodbot/itd/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 	
 	return playlist_uris
 
 def dl_video(conf: Config, video: Vod, path: str):
 	TEMP_DIR = conf.directories.temp
 	LOG_LEVEL = conf.export.ffmpeg_loglevel
 	REDIRECT = conf.export.ffmpeg_stderr
-	MAX_WORKERS = conf.pull.MAX_WORKERS
 
 	video_id = video.id
 
 	# Grab access token
 	access_token = gql.get_access_token(video_id)
 
 	# Get M3U8 playlist, and parse them
@@ -68,15 +67,15 @@
 
 	# Get all the necessary vod paths for the uri
 	base_uri = "/".join(source_uri.split("/")[:-1]) + "/"
 	vod_paths = [segment.uri for segment in playlist.segments]
 	
 	# Download VOD chunks to the temp folder
 	path_map = worker.download_files(conf, video_id, base_uri, tempdir, vod_paths)
-	cprint("#dDone, now to FFmpeg join...#r")
+	# cprint("\t#dDone, now to FFmpeg join...#r")
 
 	# join the vods using FFmpeg at specified path
 	cwd = os.getcwd()
 	os.chdir(str(tempdir))
 	cmd = [
 		"ffmpeg", "-i", str(playlist_path),
 		"-c", "copy", path, "-y",
```

### Comparing `VodBot-1.1.4/vodbot/itd/gql.py` & `VodBot-1.1.5/vodbot/itd/gql.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 	return resp
 
 
 # GQL Query forms
 # Channel VODs query
 GET_CHANNEL_VIDEOS_QUERY = """
 {{  user(login: "{channel_id}") {{
-		videos( first: {first}, type: {type}, sort: {sort}, after: "{after}" ) {{
+		videos( first: {first}, sort: {sort}, after: "{after}" ) {{
 			totalCount
 			edges {{ cursor
 				node {{ id title
 					publishedAt broadcastType status
 					lengthSeconds thumbnailURLs
 					game {{ id name }}
 					creator {{ id login displayName }}
```

### Comparing `VodBot-1.1.4/vodbot/itd/worker.py` & `VodBot-1.1.5/vodbot/itd/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,16 @@
 			cprint(f"#c\r{msg}", end="")
 	except KeyboardInterrupt:
 		_, not_done = wait(futures, timeout=0)
 		for future in not_done:
 			future.cancel()
 		wait(not_done, timeout=None)
 		raise DownloadCancelled()
-
+	
+	cprint() # to go to the next line after all the printing is done.
 
 def download_files(conf:Config, video_id:str, base_url:str, target_dir:Path, vod_paths:List[str]) -> OrderedDict[str, str]:
 	urls = [base_url + path for path in vod_paths]
 	targets = [str(target_dir / path) for path in vod_paths]
 	retries = conf.pull.connection_retries
 	timeout = conf.pull.connection_timeout
 	chunk_size = conf.pull.chunk_size
```

### Comparing `VodBot-1.1.4/vodbot/printer.py` & `VodBot-1.1.5/vodbot/printer.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.4/vodbot/thumbnail.py` & `VodBot-1.1.5/vodbot/thumbnail.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.4/vodbot/twitch.py` & `VodBot-1.1.5/vodbot/twitch.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,32 +194,38 @@
 	:param channel: A Channel object.
 	:returns: A list of VOD objects.
 	"""
 
 	vods = []
 	pagination = ""
 	while True:
+		# get videos of multiple types
+		# past streams = ARCHIVE, segment of stream = HIGHLIGHT, upload = UPLOAD, premiere = PAST_PREMIERE
 		query = gql.GET_CHANNEL_VIDEOS_QUERY.format(
 			channel_id=channel.login,
 			after=pagination, first=100,
-			type="ARCHIVE", sort="TIME"
+			sort="TIME"
 		)
 		resp = gql.gql_query(query=query).json()["data"]["user"]["videos"]
 
 		if not resp or not resp["edges"]:
 			break
 
 		pagination = resp["edges"][-1]["cursor"]
 		
 		for vod in resp["edges"]:
 			v = vod["node"]
 			c, g, b, s = v["creator"], v["game"], v["broadcastType"], v["status"]
 
-			if b == "ARCHIVE" and s == "RECORDING":
-				# This broadcast is currently live, we need to skip it.
+			# check broadcast type
+			if not any(b==t for t in ["ARCHIVE", "HIGHLIGHT", "UPLOAD", "PAST_PREMIERE"]):
+				continue
+			# This video is still be processed (or is live) and it must be skipped.
+			# if b == "ARCHIVE" and s == "RECORDING":
+			if s != "RECORDED":
 				continue
 
 			game_id = game_name = ""
 	  
 			if g:
 				game_id, game_name = g["id"], g["name"]
 			
@@ -241,14 +247,15 @@
 				for chap in resp["edges"]:
 					n = chap["node"]
 					chapters.append(
 						VodChapter(
 							type=n["type"], description=n["description"],
 							position=int(n["positionMilliseconds"]/1000),
 							duration=int(n["durationMilliseconds"]/1000)
+							# its fine to do the above because twitch's precision of message timings isnt greater than seconds
 						)
 					)
 				
 				if chapter_page == "" or chapter_page == None:
 					break
 
 			vods.append(
```

### Comparing `VodBot-1.1.4/vodbot/util.py` & `VodBot-1.1.5/vodbot/util.py`

 * *Files identical despite different names*

### Comparing `VodBot-1.1.4/vodbot/video.py` & `VodBot-1.1.5/vodbot/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 from typing import List
 
 
 class VideoFailure(Exception):
 	def __init__(self, video_id:str="unknown") -> None:
 		self.video_id = video_id
-		super().__init__(self.vid)
+		super().__init__(self.video_id)
 
 class FailedToSlice(VideoFailure):
 	pass
 
 class FailedToConcat(VideoFailure):
 	pass
```

### Comparing `VodBot-1.1.4/vodbot/webhook.py` & `VodBot-1.1.5/vodbot/webhook.py`

 * *Files identical despite different names*

