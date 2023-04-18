# Comparing `tmp/opensesame-plugin-audio_low_latency-9.1.0.tar.gz` & `tmp/opensesame-plugin-audio_low_latency-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame-plugin-audio_low_latency-9.1.0.tar", last modified: Fri Mar 24 14:48:41 2023, max compression
+gzip compressed data, was "opensesame-plugin-audio_low_latency-9.2.0.tar", last modified: Tue Apr 18 21:41:03 2023, max compression
```

## Comparing `opensesame-plugin-audio_low_latency-9.1.0.tar` & `opensesame-plugin-audio_low_latency-9.2.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.675608 opensesame-plugin-audio_low_latency-9.1.0/
--rw-r--r--   0 bob       (1000) bob       (1000)     2772 2022-07-07 12:11:34.000000 opensesame-plugin-audio_low_latency-9.1.0/.gitignore
--rw-r--r--   0 bob       (1000) bob       (1000)    35147 2017-10-13 14:38:12.000000 opensesame-plugin-audio_low_latency-9.1.0/COPYING
--rw-r--r--   0 bob       (1000) bob       (1000)      349 2022-11-25 14:22:19.000000 opensesame-plugin-audio_low_latency-9.1.0/LICENSE.md
--rw-r--r--   0 bob       (1000) bob       (1000)      106 2017-11-24 23:04:58.000000 opensesame-plugin-audio_low_latency-9.1.0/MANIFEST.in
--rw-r--r--   0 bob       (1000) bob       (1000)     4290 2023-03-24 14:48:41.675608 opensesame-plugin-audio_low_latency-9.1.0/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     3546 2022-11-25 20:20:56.000000 opensesame-plugin-audio_low_latency-9.1.0/README.md
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.667608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugin_audio_low_latency.egg-info/
--rw-r--r--   0 bob       (1000) bob       (1000)     4290 2023-03-24 14:48:41.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugin_audio_low_latency.egg-info/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     5702 2023-03-24 14:48:41.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugin_audio_low_latency.egg-info/SOURCES.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-03-24 14:48:41.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugin_audio_low_latency.egg-info/dependency_links.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-03-24 14:48:41.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugin_audio_low_latency.egg-info/top_level.txt
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.666608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.668608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/
--rw-r--r--   0 bob       (1000) bob       (1000)     1997 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.md
--rw-r--r--   0 bob       (1000) bob       (1000)      645 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.png
--rw-r--r--   0 bob       (1000) bob       (1000)    12844 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1170 2021-04-14 21:43:49.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1547 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.669608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/
--rw-r--r--   0 bob       (1000) bob       (1000)     1966 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.md
--rw-r--r--   0 bob       (1000) bob       (1000)      653 2021-04-14 21:47:07.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.png
--rw-r--r--   0 bob       (1000) bob       (1000)    24904 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1242 2021-04-14 21:43:48.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1675 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.669608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_pause/
--rw-r--r--   0 bob       (1000) bob       (1000)     1594 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1332 2021-04-14 21:47:07.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3062 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.py
--rw-r--r--   0 bob       (1000) bob       (1000)     8301 2021-04-14 21:43:48.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)      461 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_pause/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.670608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_resume/
--rw-r--r--   0 bob       (1000) bob       (1000)     1594 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1341 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3067 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.py
--rw-r--r--   0 bob       (1000) bob       (1000)     8535 2021-04-14 21:43:49.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)      462 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_resume/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.670608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/
--rw-r--r--   0 bob       (1000) bob       (1000)     2039 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1339 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.png
--rw-r--r--   0 bob       (1000) bob       (1000)    13428 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.py
--rw-r--r--   0 bob       (1000) bob       (1000)     8249 2021-04-14 21:43:49.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1579 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.671608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_stop/
--rw-r--r--   0 bob       (1000) bob       (1000)     1593 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1329 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3347 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.py
--rw-r--r--   0 bob       (1000) bob       (1000)     8019 2021-04-14 21:43:49.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)      460 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_stop/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.671608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_wait/
--rw-r--r--   0 bob       (1000) bob       (1000)     1594 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1344 2021-04-14 21:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3110 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.py
--rw-r--r--   0 bob       (1000) bob       (1000)     8229 2021-04-14 21:53:55.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)      479 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_wait/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.672608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/
--rw-r--r--   0 bob       (1000) bob       (1000)     1977 2022-04-29 12:41:51.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1356 2021-04-14 21:47:09.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.png
--rw-r--r--   0 bob       (1000) bob       (1000)    14246 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1829 2021-04-14 21:43:50.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)     2072 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.672608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/
--rw-r--r--   0 bob       (1000) bob       (1000)     1966 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1831 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.png
--rw-r--r--   0 bob       (1000) bob       (1000)    24909 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.py
--rw-r--r--   0 bob       (1000) bob       (1000)     2580 2021-04-14 21:43:49.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1679 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.673608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_pause/
--rw-r--r--   0 bob       (1000) bob       (1000)     1594 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.md
--rw-r--r--   0 bob       (1000) bob       (1000)     2402 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3092 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.py
--rw-r--r--   0 bob       (1000) bob       (1000)     9464 2021-04-14 21:43:50.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)      484 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_pause/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.674608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_resume/
--rw-r--r--   0 bob       (1000) bob       (1000)     1594 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.md
--rw-r--r--   0 bob       (1000) bob       (1000)     2420 2021-04-14 21:47:09.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3115 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.py
--rw-r--r--   0 bob       (1000) bob       (1000)     9798 2021-04-14 21:43:50.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)      467 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_resume/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.674608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/
--rw-r--r--   0 bob       (1000) bob       (1000)     2043 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.md
--rw-r--r--   0 bob       (1000) bob       (1000)     2432 2021-04-14 21:47:09.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.png
--rw-r--r--   0 bob       (1000) bob       (1000)    14889 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.py
--rw-r--r--   0 bob       (1000) bob       (1000)     9465 2021-04-14 21:43:50.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)     2103 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.675608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_stop/
--rw-r--r--   0 bob       (1000) bob       (1000)     1593 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.md
--rw-r--r--   0 bob       (1000) bob       (1000)     2408 2021-04-14 21:47:09.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3382 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.py
--rw-r--r--   0 bob       (1000) bob       (1000)     9133 2021-04-14 21:43:50.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)      464 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_stop/info.yaml
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-03-24 14:48:41.675608 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_wait/
--rw-r--r--   0 bob       (1000) bob       (1000)     1593 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.md
--rw-r--r--   0 bob       (1000) bob       (1000)     2396 2021-04-14 21:54:42.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3232 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.py
--rw-r--r--   0 bob       (1000) bob       (1000)     9619 2021-04-14 21:53:55.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)      484 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_wait/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      121 2023-03-24 14:48:41.676608 opensesame-plugin-audio_low_latency-9.1.0/setup.cfg
--rw-r--r--   0 bob       (1000) bob       (1000)     9764 2023-03-24 14:46:56.000000 opensesame-plugin-audio_low_latency-9.1.0/setup.py
--rw-r--r--   0 bob       (1000) bob       (1000)      292 2023-03-11 22:44:21.000000 opensesame-plugin-audio_low_latency-9.1.0/stdeb.cfg
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.347714 opensesame-plugin-audio_low_latency-9.2.0/
+-rw-r--r--   0 bob       (1000) bob       (1000)     2772 2022-07-07 12:11:34.000000 opensesame-plugin-audio_low_latency-9.2.0/.gitignore
+-rw-r--r--   0 bob       (1000) bob       (1000)    35147 2017-10-13 14:38:12.000000 opensesame-plugin-audio_low_latency-9.2.0/COPYING
+-rw-r--r--   0 bob       (1000) bob       (1000)      349 2022-11-25 14:22:19.000000 opensesame-plugin-audio_low_latency-9.2.0/LICENSE.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      106 2017-11-24 23:04:58.000000 opensesame-plugin-audio_low_latency-9.2.0/MANIFEST.in
+-rw-r--r--   0 bob       (1000) bob       (1000)     4290 2023-04-18 21:41:03.347714 opensesame-plugin-audio_low_latency-9.2.0/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     3546 2022-11-25 20:20:56.000000 opensesame-plugin-audio_low_latency-9.2.0/README.md
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.339713 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugin_audio_low_latency.egg-info/
+-rw-r--r--   0 bob       (1000) bob       (1000)     4290 2023-04-18 21:41:03.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugin_audio_low_latency.egg-info/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     5702 2023-04-18 21:41:03.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugin_audio_low_latency.egg-info/SOURCES.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-04-18 21:41:03.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugin_audio_low_latency.egg-info/dependency_links.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-04-18 21:41:03.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugin_audio_low_latency.egg-info/top_level.txt
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.337713 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.339713 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1997 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      645 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.png
+-rw-r--r--   0 bob       (1000) bob       (1000)    12714 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1170 2021-04-14 21:43:49.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     1547 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.340714 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1966 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      653 2021-04-14 21:47:07.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.png
+-rw-r--r--   0 bob       (1000) bob       (1000)    24988 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1242 2021-04-14 21:43:48.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     1675 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.340714 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_pause/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1594 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1332 2021-04-14 21:47:07.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3062 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     8301 2021-04-14 21:43:48.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      461 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_pause/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.341714 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_resume/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1594 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1341 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3067 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     8535 2021-04-14 21:43:49.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      462 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_resume/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.342713 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/
+-rw-r--r--   0 bob       (1000) bob       (1000)     2039 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1339 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.png
+-rw-r--r--   0 bob       (1000) bob       (1000)    13428 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     8249 2021-04-14 21:43:49.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     1579 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.342713 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_stop/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1593 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1329 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3347 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     8019 2021-04-14 21:43:49.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      460 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_stop/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.343714 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_wait/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1594 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1344 2021-04-14 21:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3110 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     8229 2021-04-14 21:53:55.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      479 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_wait/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.344714 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1977 2022-04-29 12:41:51.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1356 2021-04-14 21:47:09.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.png
+-rw-r--r--   0 bob       (1000) bob       (1000)    14116 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1829 2021-04-14 21:43:50.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     2072 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.344714 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1966 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1831 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.png
+-rw-r--r--   0 bob       (1000) bob       (1000)    24998 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     2580 2021-04-14 21:43:49.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     1679 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.345713 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_pause/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1594 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     2402 2021-04-14 21:47:08.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3092 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     9464 2021-04-14 21:43:50.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      484 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_pause/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.345713 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_resume/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1594 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     2420 2021-04-14 21:47:09.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3115 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     9798 2021-04-14 21:43:50.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      467 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_resume/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.346714 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/
+-rw-r--r--   0 bob       (1000) bob       (1000)     2043 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     2432 2021-04-14 21:47:09.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.png
+-rw-r--r--   0 bob       (1000) bob       (1000)    14889 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     9465 2021-04-14 21:43:50.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     2103 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.346714 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_stop/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1593 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     2408 2021-04-14 21:47:09.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3382 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     9133 2021-04-14 21:43:50.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      464 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_stop/info.yaml
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-04-18 21:41:03.347714 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_wait/
+-rw-r--r--   0 bob       (1000) bob       (1000)     1593 2022-04-29 12:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     2396 2021-04-14 21:54:42.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3232 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     9619 2021-04-14 21:53:55.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      484 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_wait/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      121 2023-04-18 21:41:03.347714 opensesame-plugin-audio_low_latency-9.2.0/setup.cfg
+-rw-r--r--   0 bob       (1000) bob       (1000)     9764 2023-04-18 21:27:33.000000 opensesame-plugin-audio_low_latency-9.2.0/setup.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      292 2023-03-11 22:44:21.000000 opensesame-plugin-audio_low_latency-9.2.0/stdeb.cfg
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/.gitignore` & `opensesame-plugin-audio_low_latency-9.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/COPYING` & `opensesame-plugin-audio_low_latency-9.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/PKG-INFO` & `opensesame-plugin-audio_low_latency-9.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensesame-plugin-audio_low_latency
-Version: 9.1.0
+Version: 9.2.0
 Summary: An OpenSesame Plug-in for playing and recording audio files with low latency on Linux.
 Home-page: https://github.com/dev-jam/opensesame-plugin-audio_low_latency
 Author: Bob Rosbag
 Author-email: debian@bobrosbag.nl
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: MacOS X
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/README.md` & `opensesame-plugin-audio_low_latency-9.2.0/README.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugin_audio_low_latency.egg-info/PKG-INFO` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugin_audio_low_latency.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensesame-plugin-audio-low-latency
-Version: 9.1.0
+Version: 9.2.0
 Summary: An OpenSesame Plug-in for playing and recording audio files with low latency on Linux.
 Home-page: https://github.com/dev-jam/opensesame-plugin-audio_low_latency
 Author: Bob Rosbag
 Author-email: debian@bobrosbag.nl
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: MacOS X
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugin_audio_low_latency.egg-info/SOURCES.txt` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugin_audio_low_latency.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 import wave
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_play(item):
 
     description = u'Low Latency Audio: starts audio playback on the foreground.'
 
     def __init__(self, name, experiment, string=None):
 
@@ -267,19 +267,14 @@
                     break
 
         self.set_stimulus_offset()
 
         if self.ram_cache == u'no':
             wav_file.close()
 
-        if self.module == self.experiment.pyaudio_module_name:
-           self.device.stop_stream()
-
-        self.device.close()
-
         self.show_message(u'Finished audio playback')
 
     def check_keys(self):
 
         key1, time1 = self.kb.get_key()
         self.kb.flush()
         if self.stop != u'':
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/audio_low_latency_play_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play/info.yaml` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play/info.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Low Latency Audio - starts audio playback on the foreground.
-version: 9.1.0
+version: 9.2.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "Audio Low Latency Playback"
 date: "2022"
 controls:
 -
     label: "Audio Filename"
@@ -48,9 +48,9 @@
     type: "text"
 -
     label: |
       <small><b>Note:</b> Audio Low Latency Play Init item at the begin of the experiment is needed for initialization of the audio device</small>
     type: text
 -
     label:  |
-      <small>Audio Low Latency version 9.1.0</small>
+      <small>Audio Low Latency version 9.2.0</small>
     type: text
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 import pygame
 import subprocess
 import re
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_play_init(item):
 
     description = u'Low Latency Audio: initializes the playback audio device.'
     lazy_init = False
 
     def __init__(self, name, experiment, string=None):
@@ -386,15 +386,15 @@
                 self.period_size_time = round(float(self.period_size) / float(self.samplerate) * 1000, 1)
                 self.data_size = self.frame_size * self.period_size // 8
 
                 self.experiment.audio_low_latency_play_period_size = self.period_size
                 self.experiment.audio_low_latency_play_data_size = self.data_size
                 self.experiment.var.audio_low_latency_play_period_size = self.period_size
 
-                print('Overruling period size with hardware buffer for OSS4, using: ' + str(self.period_size) + ' frames or ' + str(self.period_size_time) + 'ms')
+                self.show_message('Overruling period size with hardware buffer for OSS4, using: ' + str(self.period_size) + ' frames or ' + str(self.period_size_time) + 'ms')
 
             self.experiment.audio_low_latency_play_device = self.device
             self.experiment.cleanup_functions.append(self.close)
 
 
         elif self.dummy_mode == u'yes':
             self.show_message(u'Dummy mode enabled, run phase')
@@ -417,20 +417,19 @@
             self.experiment.audio_low_latency_play_device is None:
                 self.show_message(u"no active Audio Device")
                 return
         try:
             self.show_message(u"Closing audio device")
 
             if self.module == self.pyaudio_module_name:
-               self.device.stop_stream()
-               self.device.close()
+               self.experiment.audio_low_latency_play_device.stop_stream()
+               self.experiment.audio_low_latency_play_device.close()
                self.device_init.terminate()
             else:
-               self.device.close()
-            self.device = None
+                self.experiment.audio_low_latency_play_device.close()
             self.experiment.audio_low_latency_play_device = None
             self.show_message(u"Audio device closed")
         except:
             self.show_message(u"failed to close Audio Device")
 
 
 class qtaudio_low_latency_play_init(audio_low_latency_play_init, qtautoplugin):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/audio_low_latency_play_init_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_init/info.yaml` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_init/info.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Low Latency Audio - initializes the playback audio device.
-version: 9.1.0
+version: 9.2.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "Audio Low Latency Playback"
 date: "2022"
 controls:
 -
     label: "Dummy Mode"
@@ -59,9 +59,9 @@
     var: "period_size"
 -
     label: |
       <small><b>Note:</b> Audio Low Latency Play Init item at the begin of the experiment is needed for initialization of the audio device</small>
     type: text
 -
     label:  |
-      <small>Audio Low Latency version 9.1.0</small>
+      <small>Audio Low Latency version 9.2.0</small>
     type: text
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_play_pause(item):
 
     description = u'Low Latency Audio: stops the background audio playback.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_pause/audio_low_latency_play_pause_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_play_resume(item):
 
     description = u'Low Latency Audio: stops the background audio playback.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_resume/audio_low_latency_play_resume_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 import threading
 import wave
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_play_start(item):
 
     description = u'Low Latency Audio: starts audio playback in the background.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/audio_low_latency_play_start_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_start/info.yaml` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_start/info.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Low Latency Audio - starts audio playback in the background.
-version: 9.1.0
+version: 9.2.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "Audio Low Latency Playback"
 date: "2022"
 controls:
 -
     label: "Audio Filename"
@@ -48,10 +48,10 @@
     type: "text"
 -
     label: |
       <small><b>Note:</b> Audio Low Latency Play Init item at the begin of the experiment is needed for initialization of the audio device</small>
     type: text
 -
     label:  |
-      <small>Audio Low Latency version 9.1.0</small>
+      <small>Audio Low Latency version 9.2.0</small>
     type: text
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_play_stop(item):
 
     description = u'Low Latency Audio: stops the background audio playback.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_stop/audio_low_latency_play_stop_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_play_wait(item):
 
     description = u'Low Latency Audio: waits until the background audio playback has finished.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_play_wait/audio_low_latency_play_wait_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 import wave
 import numpy
 import os, re, os.path
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_record(item):
 
     description = u'Low Latency Audio: starts audio recording on the foreground.'
 
     def __init__(self, name, experiment, string=None):
 
@@ -291,19 +291,14 @@
 
         if self.ram_cache == u'yes':
             self.show_message(u'Writing data to wav file')
             wav_file.writeframes(b''.join(frames))
 
         wav_file.close()
 
-
-        if self.module == self.experiment.pyaudio_module_name:
-           self.device.stop_stream()
-
-        self.device.close()
         self.show_message(u'Finished audio recording')
         self.experiment.audio_low_latency_record_locked = 0
 
     def process_data(self, stream, wav_file, chunk, frames):
 
         # Read data from device
         if self.module == self.experiment.pyalsaaudio_module_name:
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/audio_low_latency_record_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record/info.yaml` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record/info.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Low Latency Audio - starts audio recording on the foreground.
-version: 9.1.0
+version: 9.2.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "Audio Low Latency Recording"
 date: "2022"
 controls:
 -
     label: "Audio Filename"
@@ -62,9 +62,9 @@
     type: "text"
 -
     label: |
       <small><b>Note:</b> Audio Low Latency Record Init item at the begin of the experiment is needed for initialization of the audio device</small>
     type: text
 -
     label:  |
-      <small>Audio Low Latency version 9.1.0</small>
+      <small>Audio Low Latency version 9.2.0</small>
     type: text
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 import pygame
 import subprocess
 import re
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_record_init(item):
 
     description = u'Low Latency Audio: initializes the recording audio device.'
     lazy_init = False
 
     def __init__(self, name, experiment, string=None):
@@ -388,15 +388,15 @@
                 self.period_size_time = round(float(self.period_size) / float(self.samplerate) * 1000, 1)
                 self.data_size = self.frame_size * self.period_size // 8
 
                 self.experiment.audio_low_latency_record_period_size = self.period_size
                 self.experiment.audio_low_latency_record_data_size = self.data_size
                 self.experiment.var.audio_low_latency_record_period_size = self.period_size
 
-                print('Overruling period size with hardware buffer for OSS4, using: ' + str(self.period_size) + ' frames or ' + str(self.period_size_time) + 'ms')
+                self.show_message('Overruling period size with hardware buffer for OSS4, using: ' + str(self.period_size) + ' frames or ' + str(self.period_size_time) + 'ms')
 
             self.experiment.audio_low_latency_record_device = self.device
             self.experiment.cleanup_functions.append(self.close)
 
 
         elif self.dummy_mode == u'yes':
             self.show_message(u'Dummy mode enabled, run phase')
@@ -419,20 +419,19 @@
             self.experiment.audio_low_latency_record_device is None:
                 self.show_message(u"no active Audio Device")
                 return
         try:
             self.show_message(u"Closing audio device")
 
             if self.module == self.pyaudio_module_name:
-               self.device.stop_stream()
-               self.device.close()
+               self.experiment.audio_low_latency_record_device.stop_stream()
+               self.experiment.audio_low_latency_record_device.close()
                self.device_init.terminate()
             else:
-               self.device.close()
-            self.device = None
+               self.experiment.audio_low_latency_record_device.close()
             self.experiment.audio_low_latency_record_device = None
             self.show_message(u"Audio device closed")
         except:
             self.show_message(u"failed to close Audio Device")
 
 
 class qtaudio_low_latency_record_init(audio_low_latency_record_init, qtautoplugin):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/audio_low_latency_record_init_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_init/info.yaml` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_init/info.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Low Latency Audio - initializes the recording audio device.
-version: 9.1.0
+version: 9.2.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "Audio Low Latency Recording"
 date: "2022"
 controls:
 -
     label: "Dummy Mode"
@@ -59,9 +59,9 @@
     var: "period_size"
 -
     label: |
       <small><b>Note:</b> Audio Low Latency Record Init item at the begin of the experiment is needed for initialization of the audio device</small>
     type: text
 -
     label:  |
-      <small>Audio Low Latency version 9.1.0</small>
+      <small>Audio Low Latency version 9.2.0</small>
     type: text
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_record_pause(item):
 
     description = u'Low Latency Audio: pauses the background audio recording.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_pause/audio_low_latency_record_pause_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_record_resume(item):
 
     description = u'Low Latency Audio: waits until the background audio recording has finished.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_resume/audio_low_latency_record_resume_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 import threading
 import wave
 import numpy
 import os, re, os.path
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_record_start(item):
 
     description = u'Low Latency Audio: starts audio recording in the background.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/audio_low_latency_record_start_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_start/info.yaml` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_start/info.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Low Latency Audio - starts audio recording in the background.
-version: 9.1.0
+version: 9.2.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "Audio Low Latency Recording"
 date: "2022"
 controls:
 -
     label: "Audio Filename"
@@ -62,9 +62,9 @@
     type: "text"
 -
     label: |
       <small><b>Note:</b> Audio Low Latency Record Init item at the begin of the experiment is needed for initialization of the audio device</small>
     type: text
 -
     label:  |
-      <small>Audio Low Latency version 9.1.0</small>
+      <small>Audio Low Latency version 9.2.0</small>
     type: text
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_record_stop(item):
 
     description = u'Low Latency Audio: stops the background audio recording.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_stop/audio_low_latency_record_stop_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.md` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.md`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.py` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from libopensesame.py3compat import *
 from libopensesame import debug
 from libopensesame.item import item
 from libqtopensesame.items.qtautoplugin import qtautoplugin
 from libopensesame.exceptions import osexception
 from openexp.keyboard import keyboard
 
-VERSION = u'9.1.0'
+VERSION = u'9.2.0'
 
 class audio_low_latency_record_wait(item):
 
     description = u'Low Latency Audio: waits until the background audio recording has finished.'
 
     def __init__(self, name, experiment, string=None):
```

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait_large.png` & `opensesame-plugin-audio_low_latency-9.2.0/opensesame_plugins/audio_low_latency_record_wait/audio_low_latency_record_wait_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-audio_low_latency-9.1.0/setup.py` & `opensesame-plugin-audio_low_latency-9.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         with open('README.md') as fd:
             return fd.read()
     return 'No readme information'
 
 
 setup(
     name='opensesame-plugin-audio_low_latency',
-    version='9.1.0',
+    version='9.2.0',
     description='An OpenSesame Plug-in for playing and recording audio files with low latency on Linux.',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     author='Bob Rosbag',
     author_email='debian@bobrosbag.nl',
     url='https://github.com/dev-jam/opensesame-plugin-audio_low_latency',
     # Classifiers used by PyPi if you upload the plugin there
```

