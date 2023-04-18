# Comparing `tmp/sprocket_carball-0.8.6.tar.gz` & `tmp/sprocket_carball-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocket_carball-0.8.6.tar", last modified: Tue Apr 18 17:41:54 2023, max compression
+gzip compressed data, was "sprocket_carball-0.8.7.tar", last modified: Tue Apr 18 19:44:06 2023, max compression
```

## Comparing `sprocket_carball-0.8.6.tar` & `sprocket_carball-0.8.7.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.224520 sprocket_carball-0.8.6/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11357 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/LICENSE
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      198 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/MANIFEST.in
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      552 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/NOTICE
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6722 2023-04-18 17:41:54.224520 sprocket_carball-0.8.6/PKG-INFO
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6365 2023-04-18 17:27:43.000000 sprocket_carball-0.8.6/README.md
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.160520 sprocket_carball-0.8.6/carball/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      223 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.160520 sprocket_carball-0.8.6/carball/analysis/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        2 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/PROTOBUF_VERSION
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    17254 2023-04-16 06:18:49.000000 sprocket_carball-0.8.6/carball/analysis/analysis_manager.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.160520 sprocket_carball-0.8.6/carball/analysis/cleaner/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/cleaner/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/cleaner/cleaner.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2295 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/cleaner/frame_cleaner.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.164520 sprocket_carball-0.8.6/carball/analysis/constants/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/constants/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      815 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/constants/basic_math.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5721 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/constants/dropshot.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6198 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/constants/field_constants.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1187 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/constants/playlist.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.164520 sprocket_carball-0.8.6/carball/analysis/events/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.164520 sprocket_carball-0.8.6/carball/analysis/events/boost_pad_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/boost_pad_detection/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3707 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/boost_pad_detection/pickup_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.164520 sprocket_carball-0.8.6/carball/analysis/events/bump_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/bump_detection/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1277 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/bump_detection/bump_analysis.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    15129 2023-04-18 17:32:26.000000 sprocket_carball-0.8.6/carball/analysis/events/carry_detection.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.168520 sprocket_carball-0.8.6/carball/analysis/events/dropshot/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/dropshot/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/dropshot/ball.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      935 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/dropshot/damage.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5568 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/event_creator.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.168520 sprocket_carball-0.8.6/carball/analysis/events/fifty_fifty/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/fifty_fifty/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7419 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/fifty_fifty/fifty_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.168520 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11653 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/base_hit.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11223 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hit_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.168520 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    41555 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1662 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/car.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1973 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/hitbox.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.172520 sprocket_carball-0.8.6/carball/analysis/events/hit_pressure/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_pressure/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3373 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/hit_pressure/pressure_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.172520 sprocket_carball-0.8.6/carball/analysis/events/kickoff_detection/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/kickoff_detection/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10002 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/events/kickoff_detection/kickoff_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.172520 sprocket_carball-0.8.6/carball/analysis/saltie_game/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.176520 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      459 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiDemo.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2531 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiGame.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      383 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiGoal.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      479 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiMutators.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1473 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayer.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1406 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3124 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      681 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiTeam.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4703 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/saltie_game/saltie_game.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.176520 sprocket_carball-0.8.6/carball/analysis/simulator/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/simulator/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11609 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/simulator/ball_simulator.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      855 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/simulator/bounce.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      238 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/simulator/map_constants.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.176520 sprocket_carball-0.8.6/carball/analysis/stats/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.176520 sprocket_carball-0.8.6/carball/analysis/stats/ball_forward/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/ball_forward/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1023 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/boost/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/boost/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6918 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/boost/boost.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/controls/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/controls/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2829 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/controls/controls.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/demos/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/demos/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1623 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/demos/demos.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/dribbles/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dribbles/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3342 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dribbles/ball_carry.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/dropshot/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      343 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dropshot/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2082 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dropshot/ball_phase_times.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3902 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dropshot/damage.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2575 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/dropshot/goals.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.180520 sprocket_carball-0.8.6/carball/analysis/stats/kickoffs/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/kickoffs/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2211 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/kickoffs/kickoff_stat.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.184520 sprocket_carball-0.8.6/carball/analysis/stats/possession/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/possession/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3521 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/possession/ball_distances.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10214 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/possession/per_possession.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2982 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/possession/possession.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2243 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/possession/turnovers.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.184520 sprocket_carball-0.8.6/carball/analysis/stats/rumble/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/rumble/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3475 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/rumble/goals.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8977 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/rumble/rumble.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4033 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/stats.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3336 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/stats_list.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3851 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/stats_manager.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.188520 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1330 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/averages.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1583 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/hit_counts.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6969 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/positional_tendencies.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2777 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/relative_position_tendencies.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1962 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/speed_tendencies.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6502 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/tendencies/team_tendencies.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.188520 sprocket_carball-0.8.6/carball/analysis/stats/utils/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/utils/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1708 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/stats/utils/pandas_utils.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.188520 sprocket_carball-0.8.6/carball/analysis/utils/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      316 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/json_encoder.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1974 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/numpy_manager.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2050 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/pandas_manager.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      374 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/proto_manager.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1265 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/analysis/utils/split_location.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2558 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/command_line.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.192520 sprocket_carball-0.8.6/carball/controls/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/controls/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2203 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/controls/controls.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3427 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/controls/rotations.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2586 2023-04-16 23:12:44.000000 sprocket_carball-0.8.6/carball/decompile_replays.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.192520 sprocket_carball-0.8.6/carball/extras/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/extras/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1770 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/extras/per_goal_analysis.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.152520 sprocket_carball-0.8.6/carball/generated/
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.192520 sprocket_carball-0.8.6/carball/generated/api/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/__init__.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     5076 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/game_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.196520 sprocket_carball-0.8.6/carball/generated/api/metadata/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/metadata/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4653 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/metadata/camera_settings_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)    19305 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/metadata/game_metadata_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3635 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/metadata/mutators_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12482 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/metadata/player_loadout_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     2397 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/party_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1793 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/player_id_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     8237 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/player_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.200520 sprocket_carball-0.8.6/carball/generated/api/stats/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/__init__.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     3714 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/ball_stats_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/data_frame_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)    18134 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/dropshot_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)    31534 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/events_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     5766 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/extra_mode_stats_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     6701 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/game_stats_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1837 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/goal_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)    18809 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/kickoff_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7823 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/per_possession_stats_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)    34767 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/player_stats_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7450 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/rumble_pb2.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    21715 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/stats_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     7909 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/stats/team_stats_pb2.py
--rw-------   0 jacbaile  (1000) jacbaile  (1000)     3568 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/api/team_pb2.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.200520 sprocket_carball-0.8.6/carball/generated/binaries/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:40:35.000000 sprocket_carball-0.8.6/carball/generated/binaries/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.204520 sprocket_carball-0.8.6/carball/json_parser/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.208520 sprocket_carball-0.8.6/carball/json_parser/actor/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      435 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1649 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/ball.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1210 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/base.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4316 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/boost.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1053 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/camera.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3497 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/car.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1719 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/dropshot.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1034 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/game_event.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      388 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/game_info.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/jump.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4207 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/player.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1122 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/rumble.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      466 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor/team.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3761 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/actor_parsing.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1374 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/bots.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2021 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/dropshot.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12747 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/frame_parser.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    13147 2023-04-16 06:04:04.000000 sprocket_carball-0.8.6/carball/json_parser/game.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1614 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/game_info.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      932 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/goal.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11640 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/player.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.208520 sprocket_carball-0.8.6/carball/json_parser/sanity_check/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/__init__.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.208520 sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1261 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/base_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      117 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/game_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      298 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/player_check.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.212520 sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      496 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/ball_data_frame_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1037 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/player_attributes_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      813 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/player_data_frame_check.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.212520 sprocket_carball-0.8.6/carball/json_parser/sanity_check/errors/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/errors/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      275 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/errors/errors.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1459 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/sanity_check/sanity_check.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1195 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/json_parser/team.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.212520 sprocket_carball-0.8.6/carball/tests/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3666 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/analysis_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.212520 sprocket_carball-0.8.6/carball/tests/benchmarking/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/benchmarking/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1577 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/benchmarking/benchmarking.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      124 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/conftest.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.216520 sprocket_carball-0.8.6/carball/tests/docs/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/docs/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1610 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/docs/data_frame_docs.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2641 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/export_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2791 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/game_creation_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.216520 sprocket_carball-0.8.6/carball/tests/metadata/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1100 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/camera_settings_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      796 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/command_line_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      668 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/error_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2809 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/leader_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      635 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/metadata/offline_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      819 2023-04-15 17:31:55.000000 sprocket_carball-0.8.6/carball/tests/read_pandas_test.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.220520 sprocket_carball-0.8.6/carball/tests/stats/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6280 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/boost_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      494 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/demo_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    16228 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/dribble_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8308 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/dropshot_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2911 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/fifty_fifty_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6753 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/hit_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5648 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/kickoff_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10956 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/rumble_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      814 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/stats/team_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      574 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/tiles_test.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12330 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/carball/tests/utils.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      375 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/init.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)       62 2023-04-16 23:09:05.000000 sprocket_carball-0.8.6/requirements.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       38 2023-04-18 17:41:54.224520 sprocket_carball-0.8.6/setup.cfg
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1676 2023-04-18 17:41:43.000000 sprocket_carball-0.8.6/setup.py
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.220520 sprocket_carball-0.8.6/sprocket_carball.egg-info/
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6722 2023-04-18 17:41:53.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/PKG-INFO
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8448 2023-04-18 17:41:54.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/SOURCES.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)        1 2023-04-18 17:41:53.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/dependency_links.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       54 2023-04-18 17:41:53.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/entry_points.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       61 2023-04-18 17:41:53.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/requires.txt
--rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       14 2023-04-18 17:41:53.000000 sprocket_carball-0.8.6/sprocket_carball.egg-info/top_level.txt
-drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 17:41:54.224520 sprocket_carball-0.8.6/utils/
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/utils/__init__.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2544 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/utils/create_proto.py
--rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2610 2023-04-15 17:31:56.000000 sprocket_carball-0.8.6/utils/import_fixer.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.728324 sprocket_carball-0.8.7/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11357 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/LICENSE
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      198 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/MANIFEST.in
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      552 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/NOTICE
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6722 2023-04-18 19:44:06.728324 sprocket_carball-0.8.7/PKG-INFO
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6365 2023-04-18 17:27:43.000000 sprocket_carball-0.8.7/README.md
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.656323 sprocket_carball-0.8.7/carball/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      223 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.656323 sprocket_carball-0.8.7/carball/analysis/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        2 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/PROTOBUF_VERSION
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    17254 2023-04-16 06:18:49.000000 sprocket_carball-0.8.7/carball/analysis/analysis_manager.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.660323 sprocket_carball-0.8.7/carball/analysis/cleaner/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/cleaner/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/cleaner/cleaner.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2295 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/cleaner/frame_cleaner.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.660323 sprocket_carball-0.8.7/carball/analysis/constants/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/constants/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      815 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/constants/basic_math.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5721 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/constants/dropshot.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6198 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/constants/field_constants.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1187 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/constants/playlist.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.664323 sprocket_carball-0.8.7/carball/analysis/events/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.664323 sprocket_carball-0.8.7/carball/analysis/events/boost_pad_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/boost_pad_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3707 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/boost_pad_detection/pickup_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.664323 sprocket_carball-0.8.7/carball/analysis/events/bump_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/bump_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1277 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/bump_detection/bump_analysis.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    15129 2023-04-18 17:32:26.000000 sprocket_carball-0.8.7/carball/analysis/events/carry_detection.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.664323 sprocket_carball-0.8.7/carball/analysis/events/dropshot/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/dropshot/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/dropshot/ball.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      935 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/dropshot/damage.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5568 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/event_creator.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.664323 sprocket_carball-0.8.7/carball/analysis/events/fifty_fifty/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/fifty_fifty/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7419 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/fifty_fifty/fifty_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.668323 sprocket_carball-0.8.7/carball/analysis/events/hit_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/hit_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11653 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/hit_detection/base_hit.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11223 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/hit_detection/hit_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.668323 sprocket_carball-0.8.7/carball/analysis/events/hit_detection/hitbox/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    41555 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/hit_detection/hitbox/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1662 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/hit_detection/hitbox/car.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1973 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/hit_detection/hitbox/hitbox.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.668323 sprocket_carball-0.8.7/carball/analysis/events/hit_pressure/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/hit_pressure/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3373 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/hit_pressure/pressure_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.668323 sprocket_carball-0.8.7/carball/analysis/events/kickoff_detection/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/kickoff_detection/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10002 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/events/kickoff_detection/kickoff_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.668323 sprocket_carball-0.8.7/carball/analysis/saltie_game/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.672323 sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      459 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiDemo.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2531 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiGame.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      383 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiGoal.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      479 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiMutators.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1578 2023-04-18 19:41:40.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiPlayer.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1406 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3124 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      681 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiTeam.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4703 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/saltie_game/saltie_game.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.676324 sprocket_carball-0.8.7/carball/analysis/simulator/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/simulator/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11609 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/simulator/ball_simulator.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      855 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/simulator/bounce.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      238 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/simulator/map_constants.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.676324 sprocket_carball-0.8.7/carball/analysis/stats/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.676324 sprocket_carball-0.8.7/carball/analysis/stats/ball_forward/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/ball_forward/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1023 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.676324 sprocket_carball-0.8.7/carball/analysis/stats/boost/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/boost/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6918 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/boost/boost.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.680323 sprocket_carball-0.8.7/carball/analysis/stats/controls/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/controls/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2829 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/controls/controls.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.680323 sprocket_carball-0.8.7/carball/analysis/stats/demos/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/demos/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1623 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/demos/demos.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.680323 sprocket_carball-0.8.7/carball/analysis/stats/dribbles/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/dribbles/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3342 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/dribbles/ball_carry.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.680323 sprocket_carball-0.8.7/carball/analysis/stats/dropshot/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      343 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/dropshot/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2082 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/dropshot/ball_phase_times.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3902 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/dropshot/damage.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2575 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/dropshot/goals.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.680323 sprocket_carball-0.8.7/carball/analysis/stats/kickoffs/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/kickoffs/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2211 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/kickoffs/kickoff_stat.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.684323 sprocket_carball-0.8.7/carball/analysis/stats/possession/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/possession/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3521 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/possession/ball_distances.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10214 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/possession/per_possession.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2982 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/possession/possession.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2243 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/possession/turnovers.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.684323 sprocket_carball-0.8.7/carball/analysis/stats/rumble/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/rumble/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3475 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/rumble/goals.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8977 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/rumble/rumble.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4033 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/stats.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3336 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/stats_list.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3851 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/stats_manager.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.688324 sprocket_carball-0.8.7/carball/analysis/stats/tendencies/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/tendencies/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1330 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/tendencies/averages.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1583 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/tendencies/hit_counts.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6969 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/tendencies/positional_tendencies.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2777 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/tendencies/relative_position_tendencies.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1962 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/tendencies/speed_tendencies.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6502 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/tendencies/team_tendencies.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.688324 sprocket_carball-0.8.7/carball/analysis/stats/utils/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/utils/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1708 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/stats/utils/pandas_utils.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.692324 sprocket_carball-0.8.7/carball/analysis/utils/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/utils/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      316 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/utils/json_encoder.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1974 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/utils/numpy_manager.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2050 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/utils/pandas_manager.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      374 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/utils/proto_manager.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1265 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/analysis/utils/split_location.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2558 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/command_line.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.692324 sprocket_carball-0.8.7/carball/controls/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/controls/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2203 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/controls/controls.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3427 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/controls/rotations.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2586 2023-04-16 23:12:44.000000 sprocket_carball-0.8.7/carball/decompile_replays.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.692324 sprocket_carball-0.8.7/carball/extras/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/extras/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1770 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/extras/per_goal_analysis.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.652323 sprocket_carball-0.8.7/carball/generated/
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.696324 sprocket_carball-0.8.7/carball/generated/api/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/__init__.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     5076 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/game_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.696324 sprocket_carball-0.8.7/carball/generated/api/metadata/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/metadata/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4653 2023-04-18 19:41:45.000000 sprocket_carball-0.8.7/carball/generated/api/metadata/camera_settings_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    19305 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/metadata/game_metadata_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3635 2023-04-18 19:41:45.000000 sprocket_carball-0.8.7/carball/generated/api/metadata/mutators_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12482 2023-04-18 19:41:45.000000 sprocket_carball-0.8.7/carball/generated/api/metadata/player_loadout_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     2397 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/party_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1793 2023-04-18 19:41:45.000000 sprocket_carball-0.8.7/carball/generated/api/player_id_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     8621 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/player_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.700324 sprocket_carball-0.8.7/carball/generated/api/stats/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/__init__.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     3714 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/ball_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     1383 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/data_frame_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    18134 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/dropshot_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    31534 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/events_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     5766 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/extra_mode_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     6701 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/game_stats_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1837 2023-04-18 19:41:45.000000 sprocket_carball-0.8.7/carball/generated/api/stats/goal_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    18809 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/kickoff_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7823 2023-04-18 19:41:45.000000 sprocket_carball-0.8.7/carball/generated/api/stats/per_possession_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)    34767 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/player_stats_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     7450 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/rumble_pb2.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    21715 2023-04-18 19:41:45.000000 sprocket_carball-0.8.7/carball/generated/api/stats/stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     7909 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/stats/team_stats_pb2.py
+-rw-------   0 jacbaile  (1000) jacbaile  (1000)     3568 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/api/team_pb2.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.704324 sprocket_carball-0.8.7/carball/generated/binaries/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:41:46.000000 sprocket_carball-0.8.7/carball/generated/binaries/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.708324 sprocket_carball-0.8.7/carball/json_parser/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.712324 sprocket_carball-0.8.7/carball/json_parser/actor/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      435 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1649 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/ball.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1210 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/base.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4316 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/boost.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1053 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/camera.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3497 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/car.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1719 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/dropshot.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1034 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/game_event.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      388 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/game_info.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1386 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/jump.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     4207 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/player.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1122 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/rumble.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      466 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor/team.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3761 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/actor_parsing.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1374 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/bots.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2021 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/dropshot.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12747 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/frame_parser.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    13147 2023-04-16 06:04:04.000000 sprocket_carball-0.8.7/carball/json_parser/game.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1614 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/game_info.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      932 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/goal.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    11933 2023-04-18 19:43:16.000000 sprocket_carball-0.8.7/carball/json_parser/player.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.712324 sprocket_carball-0.8.7/carball/json_parser/sanity_check/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/__init__.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.712324 sprocket_carball-0.8.7/carball/json_parser/sanity_check/base_checks/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/base_checks/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1261 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/base_checks/base_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      117 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/base_checks/game_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      298 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/base_checks/player_check.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.716324 sprocket_carball-0.8.7/carball/json_parser/sanity_check/checks/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/checks/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      496 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/checks/ball_data_frame_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1037 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/checks/player_attributes_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      813 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/checks/player_data_frame_check.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.716324 sprocket_carball-0.8.7/carball/json_parser/sanity_check/errors/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/errors/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      275 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/errors/errors.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1459 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/sanity_check/sanity_check.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1195 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/json_parser/team.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.716324 sprocket_carball-0.8.7/carball/tests/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     3666 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/analysis_test.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.720324 sprocket_carball-0.8.7/carball/tests/benchmarking/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/benchmarking/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1577 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/benchmarking/benchmarking.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      124 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/conftest.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.720324 sprocket_carball-0.8.7/carball/tests/docs/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/docs/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1610 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/docs/data_frame_docs.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2641 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/export_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2791 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/game_creation_test.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.720324 sprocket_carball-0.8.7/carball/tests/metadata/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/metadata/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1100 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/metadata/camera_settings_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      796 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/metadata/command_line_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      668 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/metadata/error_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2809 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/metadata/leader_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      635 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/metadata/offline_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      819 2023-04-15 17:31:55.000000 sprocket_carball-0.8.7/carball/tests/read_pandas_test.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.724324 sprocket_carball-0.8.7/carball/tests/stats/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/stats/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6280 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/stats/boost_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      494 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/stats/demo_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    16228 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/stats/dribble_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     8308 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/stats/dropshot_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2911 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/stats/fifty_fifty_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     6753 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/stats/hit_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     5648 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/stats/kickoff_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    10956 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/stats/rumble_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      814 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/stats/team_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      574 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/tiles_test.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)    12330 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/carball/tests/utils.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)      375 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/init.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)       62 2023-04-16 23:09:05.000000 sprocket_carball-0.8.7/requirements.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       38 2023-04-18 19:44:06.728324 sprocket_carball-0.8.7/setup.cfg
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     1676 2023-04-18 19:43:59.000000 sprocket_carball-0.8.7/setup.py
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.728324 sprocket_carball-0.8.7/sprocket_carball.egg-info/
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     6722 2023-04-18 19:44:06.000000 sprocket_carball-0.8.7/sprocket_carball.egg-info/PKG-INFO
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)     8448 2023-04-18 19:44:06.000000 sprocket_carball-0.8.7/sprocket_carball.egg-info/SOURCES.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)        1 2023-04-18 19:44:06.000000 sprocket_carball-0.8.7/sprocket_carball.egg-info/dependency_links.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       54 2023-04-18 19:44:06.000000 sprocket_carball-0.8.7/sprocket_carball.egg-info/entry_points.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       61 2023-04-18 19:44:06.000000 sprocket_carball-0.8.7/sprocket_carball.egg-info/requires.txt
+-rw-rw-r--   0 jacbaile  (1000) jacbaile  (1000)       14 2023-04-18 19:44:06.000000 sprocket_carball-0.8.7/sprocket_carball.egg-info/top_level.txt
+drwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-18 19:44:06.728324 sprocket_carball-0.8.7/utils/
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)        0 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/utils/__init__.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2544 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/utils/create_proto.py
+-rwxrwxr-x   0 jacbaile  (1000) jacbaile  (1000)     2610 2023-04-15 17:31:56.000000 sprocket_carball-0.8.7/utils/import_fixer.py
```

### Comparing `sprocket_carball-0.8.6/LICENSE` & `sprocket_carball-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/NOTICE` & `sprocket_carball-0.8.7/NOTICE`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/PKG-INFO` & `sprocket_carball-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocket_carball
-Version: 0.8.6
+Version: 0.8.7
 Summary: Rocket League replay parsing and analysis.
 Home-page: https://github.com/SprocketBot/carball
 Author: Sprocket Dev Team
 Author-email: asaxplayinghorse@gmail.com
 License: Apache 2.0
 Keywords: rocket-league
 Description-Content-Type: text/markdown
```

### Comparing `sprocket_carball-0.8.6/README.md` & `sprocket_carball-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/analysis_manager.py` & `sprocket_carball-0.8.7/carball/analysis/analysis_manager.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/cleaner/cleaner.py` & `sprocket_carball-0.8.7/carball/analysis/cleaner/cleaner.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/cleaner/frame_cleaner.py` & `sprocket_carball-0.8.7/carball/analysis/cleaner/frame_cleaner.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/constants/basic_math.py` & `sprocket_carball-0.8.7/carball/analysis/constants/basic_math.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/constants/dropshot.py` & `sprocket_carball-0.8.7/carball/analysis/constants/dropshot.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/constants/field_constants.py` & `sprocket_carball-0.8.7/carball/analysis/constants/field_constants.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/constants/playlist.py` & `sprocket_carball-0.8.7/carball/analysis/constants/playlist.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/boost_pad_detection/pickup_analysis.py` & `sprocket_carball-0.8.7/carball/analysis/events/boost_pad_detection/pickup_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/bump_detection/bump_analysis.py` & `sprocket_carball-0.8.7/carball/analysis/events/bump_detection/bump_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/carry_detection.py` & `sprocket_carball-0.8.7/carball/analysis/events/carry_detection.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/dropshot/ball.py` & `sprocket_carball-0.8.7/carball/analysis/events/dropshot/ball.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/dropshot/damage.py` & `sprocket_carball-0.8.7/carball/analysis/events/dropshot/damage.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/event_creator.py` & `sprocket_carball-0.8.7/carball/analysis/events/event_creator.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/fifty_fifty/fifty_analysis.py` & `sprocket_carball-0.8.7/carball/analysis/events/fifty_fifty/fifty_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/hit_detection/base_hit.py` & `sprocket_carball-0.8.7/carball/analysis/events/hit_detection/base_hit.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hit_analysis.py` & `sprocket_carball-0.8.7/carball/analysis/events/hit_detection/hit_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx` & `sprocket_carball-0.8.7/carball/analysis/events/hit_detection/hitbox/Vehicle Specifications v1.39 - Hitboxes, Handling.xlsx`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/car.py` & `sprocket_carball-0.8.7/carball/analysis/events/hit_detection/hitbox/car.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/hit_detection/hitbox/hitbox.py` & `sprocket_carball-0.8.7/carball/analysis/events/hit_detection/hitbox/hitbox.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/hit_pressure/pressure_analysis.py` & `sprocket_carball-0.8.7/carball/analysis/events/hit_pressure/pressure_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/events/kickoff_detection/kickoff_analysis.py` & `sprocket_carball-0.8.7/carball/analysis/events/kickoff_detection/kickoff_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiGame.py` & `sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiGame.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayer.py` & `sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiPlayer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from .ApiPlayerLoadout import ApiPlayerLoadout
 
 
 class ApiPlayer:
 
     @staticmethod
     def create_from_player(proto_player: player_pb2.Player, player: Player, id_creator: Callable):
-        ApiPlayerCameraSettings.create_from_player(proto_player.camera_settings, player)
+        ApiPlayerCameraSettings.create_from_player(
+            proto_player.camera_settings, player)
         ApiPlayerLoadout.create_from_player(proto_player.loadout, player)
 
         id_creator(proto_player.id, player.name)
         if player.name is not None:
             proto_player.name = player.name
         if player.title is not None:
             proto_player.title_id = player.title
@@ -29,9 +30,11 @@
             proto_player.shots = player.shots
         if player.is_orange is not None:
             proto_player.is_orange = player.is_orange
         if player.party_leader is not None:
             proto_player.party_leader.id = player.party_leader
         if player.is_bot is not None:
             proto_player.is_bot = player.is_bot
+        if player.platform is not None:
+            proto_player.platform = player.platform
 
         return proto_player
```

### Comparing `sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py` & `sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiPlayerCameraSettings.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py` & `sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiPlayerLoadout.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/saltie_game/metadata/ApiTeam.py` & `sprocket_carball-0.8.7/carball/analysis/saltie_game/metadata/ApiTeam.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/saltie_game/saltie_game.py` & `sprocket_carball-0.8.7/carball/analysis/saltie_game/saltie_game.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/simulator/ball_simulator.py` & `sprocket_carball-0.8.7/carball/analysis/simulator/ball_simulator.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/simulator/bounce.py` & `sprocket_carball-0.8.7/carball/analysis/simulator/bounce.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py` & `sprocket_carball-0.8.7/carball/analysis/stats/ball_forward/distance_hit_ball_forward.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/boost/boost.py` & `sprocket_carball-0.8.7/carball/analysis/stats/boost/boost.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/controls/controls.py` & `sprocket_carball-0.8.7/carball/analysis/stats/controls/controls.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/demos/demos.py` & `sprocket_carball-0.8.7/carball/analysis/stats/demos/demos.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/dribbles/ball_carry.py` & `sprocket_carball-0.8.7/carball/analysis/stats/dribbles/ball_carry.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/dropshot/ball_phase_times.py` & `sprocket_carball-0.8.7/carball/analysis/stats/dropshot/ball_phase_times.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/dropshot/damage.py` & `sprocket_carball-0.8.7/carball/analysis/stats/dropshot/damage.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/dropshot/goals.py` & `sprocket_carball-0.8.7/carball/analysis/stats/dropshot/goals.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/kickoffs/kickoff_stat.py` & `sprocket_carball-0.8.7/carball/analysis/stats/kickoffs/kickoff_stat.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/possession/ball_distances.py` & `sprocket_carball-0.8.7/carball/analysis/stats/possession/ball_distances.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/possession/per_possession.py` & `sprocket_carball-0.8.7/carball/analysis/stats/possession/per_possession.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/possession/possession.py` & `sprocket_carball-0.8.7/carball/analysis/stats/possession/possession.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/possession/turnovers.py` & `sprocket_carball-0.8.7/carball/analysis/stats/possession/turnovers.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/rumble/goals.py` & `sprocket_carball-0.8.7/carball/analysis/stats/rumble/goals.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/rumble/rumble.py` & `sprocket_carball-0.8.7/carball/analysis/stats/rumble/rumble.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/stats.py` & `sprocket_carball-0.8.7/carball/analysis/stats/stats.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/stats_list.py` & `sprocket_carball-0.8.7/carball/analysis/stats/stats_list.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/stats_manager.py` & `sprocket_carball-0.8.7/carball/analysis/stats/stats_manager.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/averages.py` & `sprocket_carball-0.8.7/carball/analysis/stats/tendencies/averages.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/hit_counts.py` & `sprocket_carball-0.8.7/carball/analysis/stats/tendencies/hit_counts.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/positional_tendencies.py` & `sprocket_carball-0.8.7/carball/analysis/stats/tendencies/positional_tendencies.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/relative_position_tendencies.py` & `sprocket_carball-0.8.7/carball/analysis/stats/tendencies/relative_position_tendencies.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/speed_tendencies.py` & `sprocket_carball-0.8.7/carball/analysis/stats/tendencies/speed_tendencies.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/tendencies/team_tendencies.py` & `sprocket_carball-0.8.7/carball/analysis/stats/tendencies/team_tendencies.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/stats/utils/pandas_utils.py` & `sprocket_carball-0.8.7/carball/analysis/stats/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/utils/numpy_manager.py` & `sprocket_carball-0.8.7/carball/analysis/utils/numpy_manager.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/utils/pandas_manager.py` & `sprocket_carball-0.8.7/carball/analysis/utils/pandas_manager.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/analysis/utils/split_location.py` & `sprocket_carball-0.8.7/carball/analysis/utils/split_location.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/command_line.py` & `sprocket_carball-0.8.7/carball/command_line.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/controls/controls.py` & `sprocket_carball-0.8.7/carball/controls/controls.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/controls/rotations.py` & `sprocket_carball-0.8.7/carball/controls/rotations.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/decompile_replays.py` & `sprocket_carball-0.8.7/carball/decompile_replays.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/extras/per_goal_analysis.py` & `sprocket_carball-0.8.7/carball/extras/per_goal_analysis.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/game_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/game_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/metadata/camera_settings_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/metadata/camera_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/metadata/game_metadata_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/metadata/game_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/metadata/mutators_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/metadata/mutators_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/metadata/player_loadout_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/metadata/player_loadout_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/party_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/party_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/player_id_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/player_id_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/player_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/player_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from ..api.stats import player_stats_pb2
 from ..api import player_id_pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='api/player.proto',
   package='api',
-  serialized_pb=_b('\n\x10\x61pi/player.proto\x12\x03\x61pi\x1a!api/metadata/player_loadout.proto\x1a\"api/metadata/camera_settings.proto\x1a\x1c\x61pi/stats/player_stats.proto\x1a\x13\x61pi/player_id.proto\"\x97\x03\n\x06Player\x12\x19\n\x02id\x18\x01 \x01(\x0b\x32\r.api.PlayerId\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08title_id\x18\x03 \x01(\x05\x12\r\n\x05score\x18\x04 \x01(\x05\x12\r\n\x05goals\x18\x05 \x01(\x05\x12\x0f\n\x07\x61ssists\x18\x06 \x01(\x05\x12\r\n\x05saves\x18\x07 \x01(\x05\x12\r\n\x05shots\x18\x08 \x01(\x05\x12\x35\n\x0f\x63\x61mera_settings\x18\t \x01(\x0b\x32\x1c.api.metadata.CameraSettings\x12,\n\x07loadout\x18\n \x01(\x0b\x32\x1b.api.metadata.PlayerLoadout\x12\x11\n\tis_orange\x18\x0b \x01(\x05\x12%\n\x05stats\x18\x0c \x01(\x0b\x32\x16.api.stats.PlayerStats\x12#\n\x0cparty_leader\x18\r \x01(\x0b\x32\r.api.PlayerId\x12\x0e\n\x06is_bot\x18\x0e \x01(\x08\x12\x14\n\x0ctime_in_game\x18\x0f \x01(\x02\x12\x1b\n\x13\x66irst_frame_in_game\x18\x10 \x01(\x05')
+  serialized_pb=_b('\n\x10\x61pi/player.proto\x12\x03\x61pi\x1a!api/metadata/player_loadout.proto\x1a\"api/metadata/camera_settings.proto\x1a\x1c\x61pi/stats/player_stats.proto\x1a\x13\x61pi/player_id.proto\"\xa9\x03\n\x06Player\x12\x19\n\x02id\x18\x01 \x01(\x0b\x32\r.api.PlayerId\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08title_id\x18\x03 \x01(\x05\x12\r\n\x05score\x18\x04 \x01(\x05\x12\r\n\x05goals\x18\x05 \x01(\x05\x12\x0f\n\x07\x61ssists\x18\x06 \x01(\x05\x12\r\n\x05saves\x18\x07 \x01(\x05\x12\r\n\x05shots\x18\x08 \x01(\x05\x12\x35\n\x0f\x63\x61mera_settings\x18\t \x01(\x0b\x32\x1c.api.metadata.CameraSettings\x12,\n\x07loadout\x18\n \x01(\x0b\x32\x1b.api.metadata.PlayerLoadout\x12\x11\n\tis_orange\x18\x0b \x01(\x05\x12%\n\x05stats\x18\x0c \x01(\x0b\x32\x16.api.stats.PlayerStats\x12#\n\x0cparty_leader\x18\r \x01(\x0b\x32\r.api.PlayerId\x12\x0e\n\x06is_bot\x18\x0e \x01(\x08\x12\x14\n\x0ctime_in_game\x18\x0f \x01(\x02\x12\x1b\n\x13\x66irst_frame_in_game\x18\x10 \x01(\x05\x12\x10\n\x08platform\x18\x11 \x01(\t')
   ,
   dependencies=[player_loadout_pb2.DESCRIPTOR,camera_settings_pb2.DESCRIPTOR,player_stats_pb2.DESCRIPTOR,player_id_pb2.DESCRIPTOR,])
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 
 
 
@@ -145,27 +145,34 @@
     _descriptor.FieldDescriptor(
       name='first_frame_in_game', full_name='api.Player.first_frame_in_game', index=15,
       number=16, type=5, cpp_type=1, label=1,
       has_default_value=False, default_value=0,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       options=None),
+    _descriptor.FieldDescriptor(
+      name='platform', full_name='api.Player.platform', index=16,
+      number=17, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=_b("").decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      options=None),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   options=None,
   is_extendable=False,
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=148,
-  serialized_end=555,
+  serialized_end=573,
 )
 
 _PLAYER.fields_by_name['id'].message_type = player_id_pb2._PLAYERID
 _PLAYER.fields_by_name['camera_settings'].message_type = camera_settings_pb2._CAMERASETTINGS
 _PLAYER.fields_by_name['loadout'].message_type = player_loadout_pb2._PLAYERLOADOUT
 _PLAYER.fields_by_name['stats'].message_type = player_stats_pb2._PLAYERSTATS
 _PLAYER.fields_by_name['party_leader'].message_type = player_id_pb2._PLAYERID
```

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/ball_stats_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/ball_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/data_frame_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/dropshot_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/dropshot_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/events_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/events_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/extra_mode_stats_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/extra_mode_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/game_stats_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/game_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/goal_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/goal_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/kickoff_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/kickoff_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/per_possession_stats_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/per_possession_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/player_stats_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/player_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/rumble_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/rumble_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/stats_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/stats/team_stats_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/stats/team_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/generated/api/team_pb2.py` & `sprocket_carball-0.8.7/carball/generated/api/team_pb2.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor/ball.py` & `sprocket_carball-0.8.7/carball/json_parser/actor/ball.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor/base.py` & `sprocket_carball-0.8.7/carball/json_parser/actor/base.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor/boost.py` & `sprocket_carball-0.8.7/carball/json_parser/actor/boost.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor/camera.py` & `sprocket_carball-0.8.7/carball/json_parser/actor/camera.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor/car.py` & `sprocket_carball-0.8.7/carball/json_parser/actor/car.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor/dropshot.py` & `sprocket_carball-0.8.7/carball/json_parser/actor/dropshot.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor/game_event.py` & `sprocket_carball-0.8.7/carball/json_parser/actor/game_event.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor/jump.py` & `sprocket_carball-0.8.7/carball/json_parser/actor/jump.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor/player.py` & `sprocket_carball-0.8.7/carball/json_parser/actor/player.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor/rumble.py` & `sprocket_carball-0.8.7/carball/json_parser/actor/rumble.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/actor_parsing.py` & `sprocket_carball-0.8.7/carball/json_parser/actor_parsing.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/bots.py` & `sprocket_carball-0.8.7/carball/json_parser/bots.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/dropshot.py` & `sprocket_carball-0.8.7/carball/json_parser/dropshot.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/frame_parser.py` & `sprocket_carball-0.8.7/carball/json_parser/frame_parser.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/game.py` & `sprocket_carball-0.8.7/carball/json_parser/game.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/game_info.py` & `sprocket_carball-0.8.7/carball/json_parser/game_info.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/goal.py` & `sprocket_carball-0.8.7/carball/json_parser/goal.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/player.py` & `sprocket_carball-0.8.7/carball/json_parser/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 class Player:
 
     def __init__(self):
         self.name = None
         self.online_id = None
+        self.platform = None
         self.team = None  # using team class. set later.
         self.is_orange = None
         self.score = None
         self.goals = None
         self.assists = None
         self.saves = None
         self.shots = None
@@ -57,15 +58,16 @@
     def create_from_actor_data(self, actor_data: dict, teams: List['Team'], objects: List[str]):
         self.name = actor_data['name']
         if 'Engine.PlayerReplicationInfo:bBot' in actor_data and actor_data['Engine.PlayerReplicationInfo:bBot']:
             self.is_bot = True
             self.online_id = get_online_id_for_bot(bot_map, self)
 
         else:
-            actor_type = list(actor_data["Engine.PlayerReplicationInfo:UniqueId"]['remote_id'].keys())[0]
+            actor_type = list(
+                actor_data["Engine.PlayerReplicationInfo:UniqueId"]['remote_id'].keys())[0]
             self.online_id = self._get_player_id(actor_data["Engine.PlayerReplicationInfo:UniqueId"]
                                                  ['remote_id'][actor_type])
         try:
             self.score = actor_data["TAGame.PRI_TA:MatchScore"]
         except KeyError:
             logger.warning('Score is not found for player')
         team_actor_id = actor_data["Engine.PlayerReplicationInfo:Team"]['actor']
@@ -93,61 +95,68 @@
         self.is_orange = bool(player_stats["Team"])
         self.score = player_stats["Score"]
         self.goals = player_stats["Goals"]
         self.assists = player_stats["Assists"]
         self.saves = player_stats["Saves"]
         self.shots = player_stats["Shots"]
         self.is_bot = player_stats["bBot"]
+        self.platform = player_stats["Platform"]["value"]
 
         logger.debug('Created Player from stats: %s', self)
         if self.is_bot or self.online_id == '0' or self.online_id == 0:
             self.online_id = get_online_id_for_bot(bot_map, self)
 
         return self
 
     def get_camera_settings(self, camera_data: dict):
         self.camera_settings['field_of_view'] = camera_data.get('fov', None)
         self.camera_settings['height'] = camera_data.get('height', None)
         self.camera_settings['pitch'] = camera_data.get('angle', None)
         self.camera_settings['distance'] = camera_data.get('distance', None)
         self.camera_settings['stiffness'] = camera_data.get('stiffness', None)
         self.camera_settings['swivel_speed'] = camera_data.get('swivel', None)
-        self.camera_settings['transition_speed'] = camera_data.get('transition', None)
+        self.camera_settings['transition_speed'] = camera_data.get(
+            'transition', None)
 
         for key, value in self.camera_settings.items():
             if value is None:
-                logger.warning('Could not find ' + key + ' in camera settings for ' + self.name)
-        logger.debug('Camera settings for %s: %s', self.name, self.camera_settings)
+                logger.warning('Could not find ' + key +
+                               ' in camera settings for ' + self.name)
+        logger.debug('Camera settings for %s: %s',
+                     self.name, self.camera_settings)
 
     def parse_actor_data(self, actor_data: dict, objects: List[str]):
         """
         Adds stuff not found in PlayerStats metadata.
         PlayerStats is a better source of truth - as actor_data might not have been updated (e.g. for last assist)
 
         :param actor_data:
         :param objects:
         :return:
         """
         self.get_loadout(actor_data, objects)
         self.party_leader = actor_data.get('TAGame.PRI_TA:PartyLeader', None)
         try:
             if self.party_leader is not None and 'remote_id' in self.party_leader:
-                self.party_leader = str(list(self.party_leader['remote_id'].values())[0])
+                self.party_leader = str(
+                    list(self.party_leader['remote_id'].values())[0])
             else:
                 self.party_leader = None
         except KeyError:
             logger.warning('Could not set player party leader for:', self.name)
             self.party_leader = None
         self.title = actor_data.get('TAGame.PRI_TA:Title', None)
         self.total_xp = actor_data.get('TAGame.PRI_TA:TotalXP', None)
-        self.steering_sensitivity = actor_data.get('TAGame.PRI_TA:SteeringSensitivity', None)
+        self.steering_sensitivity = actor_data.get(
+            'TAGame.PRI_TA:SteeringSensitivity', None)
         return self
 
     def get_loadout(self, actor_data: dict, objects: List[str]):
-        if "TAGame.PRI_TA:ClientLoadouts" in actor_data:  # new version (2 loadouts)
+        # new version (2 loadouts)
+        if "TAGame.PRI_TA:ClientLoadouts" in actor_data:
             loadout_data = actor_data["TAGame.PRI_TA:ClientLoadouts"]
         else:
             try:
                 loadout_data = {'0': actor_data["TAGame.PRI_TA:ClientLoadout"]}
             except KeyError:
                 loadout_data = {'0': {}}
         for loadout_name, _loadout in loadout_data.items():
@@ -175,15 +184,16 @@
                 items = [
                     'car', 'skin', 'wheels', 'boost', 'antenna', 'topper',
                     #  8 unknown items O.o
                     'Unknown', 'Unknown', 'Unknown', 'Unknown', 'Unknown', 'Unknown', 'Unknown', 'Unknown',
                     'trail', 'goal_explosion', 'banner',
                     'Unknown', 'Unknown', 'Unknown', 'avatar_border'
                 ]
-                for item_name, corresponding_item in zip(items, team_loadout):  # order is based on menu
+                # order is based on menu
+                for item_name, corresponding_item in zip(items, team_loadout):
                     for attribute in corresponding_item:
                         object_name = objects[attribute['object_ind']]
                         if object_name == 'TAGame.ProductAttribute_Painted_TA':
                             if 'OldPaint' in attribute['value']:
                                 paint[item_name] = attribute['value']['OldPaint']
                             else:
                                 paint[item_name] = attribute['value']['NewPaint']
@@ -252,11 +262,15 @@
 
         for i in range(2):
             try:
                 loadout = self.loadout[i]
             except IndexError:
                 continue
             # default blue primary = 35, default orange primary = 33, default accent = 0, default glossy = 270
-            loadout['primary_color'] = car_data['team_paint'].get(i, {}).get('primary_color', 35 if i == 0 else 33)
-            loadout['accent_color'] = car_data['team_paint'].get(i, {}).get('accent_color', 0)
-            loadout['primary_finish'] = car_data['team_paint'].get(i, {}).get('primary_finish', 270)
-            loadout['accent_finish'] = car_data['team_paint'].get(i, {}).get('accent_finish', 270)
+            loadout['primary_color'] = car_data['team_paint'].get(
+                i, {}).get('primary_color', 35 if i == 0 else 33)
+            loadout['accent_color'] = car_data['team_paint'].get(
+                i, {}).get('accent_color', 0)
+            loadout['primary_finish'] = car_data['team_paint'].get(
+                i, {}).get('primary_finish', 270)
+            loadout['accent_finish'] = car_data['team_paint'].get(
+                i, {}).get('accent_finish', 270)
```

### Comparing `sprocket_carball-0.8.6/carball/json_parser/sanity_check/base_checks/base_check.py` & `sprocket_carball-0.8.7/carball/json_parser/sanity_check/base_checks/base_check.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/player_attributes_check.py` & `sprocket_carball-0.8.7/carball/json_parser/sanity_check/checks/player_attributes_check.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/sanity_check/checks/player_data_frame_check.py` & `sprocket_carball-0.8.7/carball/json_parser/sanity_check/checks/player_data_frame_check.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/sanity_check/sanity_check.py` & `sprocket_carball-0.8.7/carball/json_parser/sanity_check/sanity_check.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/json_parser/team.py` & `sprocket_carball-0.8.7/carball/json_parser/team.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/analysis_test.py` & `sprocket_carball-0.8.7/carball/tests/analysis_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/benchmarking/benchmarking.py` & `sprocket_carball-0.8.7/carball/tests/benchmarking/benchmarking.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/docs/data_frame_docs.py` & `sprocket_carball-0.8.7/carball/tests/docs/data_frame_docs.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/export_test.py` & `sprocket_carball-0.8.7/carball/tests/export_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/game_creation_test.py` & `sprocket_carball-0.8.7/carball/tests/game_creation_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/metadata/camera_settings_test.py` & `sprocket_carball-0.8.7/carball/tests/metadata/camera_settings_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/metadata/command_line_test.py` & `sprocket_carball-0.8.7/carball/tests/metadata/command_line_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/metadata/error_test.py` & `sprocket_carball-0.8.7/carball/tests/metadata/error_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/metadata/leader_test.py` & `sprocket_carball-0.8.7/carball/tests/metadata/leader_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/metadata/offline_test.py` & `sprocket_carball-0.8.7/carball/tests/metadata/offline_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/read_pandas_test.py` & `sprocket_carball-0.8.7/carball/tests/read_pandas_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/stats/boost_test.py` & `sprocket_carball-0.8.7/carball/tests/stats/boost_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/stats/dribble_test.py` & `sprocket_carball-0.8.7/carball/tests/stats/dribble_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/stats/dropshot_test.py` & `sprocket_carball-0.8.7/carball/tests/stats/dropshot_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/stats/fifty_fifty_test.py` & `sprocket_carball-0.8.7/carball/tests/stats/fifty_fifty_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/stats/hit_test.py` & `sprocket_carball-0.8.7/carball/tests/stats/hit_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/stats/kickoff_test.py` & `sprocket_carball-0.8.7/carball/tests/stats/kickoff_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/stats/rumble_test.py` & `sprocket_carball-0.8.7/carball/tests/stats/rumble_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/stats/team_test.py` & `sprocket_carball-0.8.7/carball/tests/stats/team_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/tiles_test.py` & `sprocket_carball-0.8.7/carball/tests/tiles_test.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/carball/tests/utils.py` & `sprocket_carball-0.8.7/carball/tests/utils.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/setup.py` & `sprocket_carball-0.8.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         initialize_project()
         # this needs to be last
         install.run(self)
 
 
 setup(
     name='sprocket_carball',
-    version='0.8.6',
+    version='0.8.7',
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=['pandas', 'protobuf==3.6.1',
                       'xlrd==1.1.0', 'numpy', 'sprocket-boxcars-py'],
     url='https://github.com/SprocketBot/carball',
     keywords=['rocket-league'],
     license='Apache 2.0',
```

### Comparing `sprocket_carball-0.8.6/sprocket_carball.egg-info/PKG-INFO` & `sprocket_carball-0.8.7/sprocket_carball.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocket-carball
-Version: 0.8.6
+Version: 0.8.7
 Summary: Rocket League replay parsing and analysis.
 Home-page: https://github.com/SprocketBot/carball
 Author: Sprocket Dev Team
 Author-email: asaxplayinghorse@gmail.com
 License: Apache 2.0
 Keywords: rocket-league
 Description-Content-Type: text/markdown
```

### Comparing `sprocket_carball-0.8.6/sprocket_carball.egg-info/SOURCES.txt` & `sprocket_carball-0.8.7/sprocket_carball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/utils/create_proto.py` & `sprocket_carball-0.8.7/utils/create_proto.py`

 * *Files identical despite different names*

### Comparing `sprocket_carball-0.8.6/utils/import_fixer.py` & `sprocket_carball-0.8.7/utils/import_fixer.py`

 * *Files identical despite different names*

