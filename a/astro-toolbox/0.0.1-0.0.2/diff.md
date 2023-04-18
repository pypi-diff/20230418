# Comparing `tmp/astro-toolbox-0.0.1.tar.gz` & `tmp/astro-toolbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-toolbox-0.0.1.tar", last modified: Wed Mar 15 10:34:24 2023, max compression
+gzip compressed data, was "astro-toolbox-0.0.2.tar", last modified: Tue Apr 18 16:57:39 2023, max compression
```

## Comparing `astro-toolbox-0.0.1.tar` & `astro-toolbox-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,72 @@
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.079744 astro-toolbox-0.0.1/
--rw-r--r--   0 romain     (501) staff       (20)    35160 2023-02-26 19:51:45.000000 astro-toolbox-0.0.1/LICENSE
--rw-r--r--   0 romain     (501) staff       (20)     4348 2023-03-15 10:34:24.079865 astro-toolbox-0.0.1/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)     3526 2023-03-15 10:24:58.000000 astro-toolbox-0.0.1/README.md
--rw-r--r--   0 romain     (501) staff       (20)     1411 2023-03-15 10:34:24.080243 astro-toolbox-0.0.1/setup.cfg
--rw-r--r--   0 romain     (501) staff       (20)       68 2023-01-06 19:50:39.000000 astro-toolbox-0.0.1/setup.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.069568 astro-toolbox-0.0.1/src/
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.072366 astro-toolbox-0.0.1/src/astro_toolbox/
--rw-r--r--   0 romain     (501) staff       (20)      901 2023-03-15 10:28:04.000000 astro-toolbox-0.0.1/src/astro_toolbox/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)       88 2023-02-07 20:30:19.000000 astro-toolbox-0.0.1/src/astro_toolbox/__main__.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.074967 astro-toolbox-0.0.1/src/astro_toolbox/angle/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.0.1/src/astro_toolbox/angle/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     2170 2023-03-10 13:03:07.000000 astro-toolbox-0.0.1/src/astro_toolbox/angle/degrees.py
--rw-r--r--   0 romain     (501) staff       (20)     1665 2023-03-10 13:01:21.000000 astro-toolbox-0.0.1/src/astro_toolbox/angle/dms.py
--rw-r--r--   0 romain     (501) staff       (20)     1579 2023-03-10 13:04:29.000000 astro-toolbox-0.0.1/src/astro_toolbox/angle/hms.py
--rw-r--r--   0 romain     (501) staff       (20)     2230 2023-03-10 13:06:25.000000 astro-toolbox-0.0.1/src/astro_toolbox/angle/radians.py
--rw-r--r--   0 romain     (501) staff       (20)    10792 2023-02-21 10:01:05.000000 astro-toolbox-0.0.1/src/astro_toolbox/command_line.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.076413 astro-toolbox-0.0.1/src/astro_toolbox/coordinates/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.0.1/src/astro_toolbox/coordinates/__init__.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.077030 astro-toolbox-0.0.1/src/astro_toolbox/coordinates/data/
--rw-r--r--   0 romain     (501) staff       (20)     2451 2023-02-02 19:46:48.000000 astro-toolbox-0.0.1/src/astro_toolbox/coordinates/data/orbital_elements.json
--rw-r--r--   0 romain     (501) staff       (20)      419 2023-02-02 17:33:55.000000 astro-toolbox-0.0.1/src/astro_toolbox/coordinates/data/sites.json
--rw-r--r--   0 romain     (501) staff       (20)     8253 2023-03-10 13:34:41.000000 astro-toolbox-0.0.1/src/astro_toolbox/coordinates/equatorial.py
--rw-r--r--   0 romain     (501) staff       (20)     3299 2023-03-10 13:34:22.000000 astro-toolbox-0.0.1/src/astro_toolbox/coordinates/horizontal.py
--rw-r--r--   0 romain     (501) staff       (20)     6648 2023-03-10 13:36:16.000000 astro-toolbox-0.0.1/src/astro_toolbox/coordinates/location.py
--rw-r--r--   0 romain     (501) staff       (20)    11831 2023-03-10 13:22:52.000000 astro-toolbox-0.0.1/src/astro_toolbox/coordinates/solar_system.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.077681 astro-toolbox-0.0.1/src/astro_toolbox/query/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-08 12:07:57.000000 astro-toolbox-0.0.1/src/astro_toolbox/query/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     2415 2023-03-10 13:41:22.000000 astro-toolbox-0.0.1/src/astro_toolbox/query/catalogs.py
--rw-r--r--   0 romain     (501) staff       (20)     3924 2023-03-10 13:42:49.000000 astro-toolbox-0.0.1/src/astro_toolbox/query/ephemeris.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.078446 astro-toolbox-0.0.1/src/astro_toolbox/scripts/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-17 20:03:46.000000 astro-toolbox-0.0.1/src/astro_toolbox/scripts/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     1780 2023-02-08 13:53:17.000000 astro-toolbox-0.0.1/src/astro_toolbox/scripts/planning.py
--rw-r--r--   0 romain     (501) staff       (20)    10857 2023-02-08 13:53:23.000000 astro-toolbox-0.0.1/src/astro_toolbox/scripts/plots.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.078880 astro-toolbox-0.0.1/src/astro_toolbox/time/
--rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:53:46.000000 astro-toolbox-0.0.1/src/astro_toolbox/time/__init__.py
--rw-r--r--   0 romain     (501) staff       (20)     4585 2023-03-10 13:27:09.000000 astro-toolbox-0.0.1/src/astro_toolbox/time/core.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.079475 astro-toolbox-0.0.1/src/astro_toolbox/utils/
--rw-r--r--   0 romain     (501) staff       (20)      441 2023-02-08 13:53:35.000000 astro-toolbox-0.0.1/src/astro_toolbox/utils/python_functions.py
--rw-r--r--   0 romain     (501) staff       (20)      658 2023-02-08 13:53:46.000000 astro-toolbox-0.0.1/src/astro_toolbox/utils/strparser.py
-drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-03-15 10:34:24.073846 astro-toolbox-0.0.1/src/astro_toolbox.egg-info/
--rw-r--r--   0 romain     (501) staff       (20)     4348 2023-03-15 10:34:24.000000 astro-toolbox-0.0.1/src/astro_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 romain     (501) staff       (20)     1274 2023-03-15 10:34:24.000000 astro-toolbox-0.0.1/src/astro_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-03-15 10:34:24.000000 astro-toolbox-0.0.1/src/astro_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 romain     (501) staff       (20)       62 2023-03-15 10:34:24.000000 astro-toolbox-0.0.1/src/astro_toolbox.egg-info/entry_points.txt
--rw-r--r--   0 romain     (501) staff       (20)        1 2023-01-18 11:00:43.000000 astro-toolbox-0.0.1/src/astro_toolbox.egg-info/not-zip-safe
--rw-r--r--   0 romain     (501) staff       (20)      152 2023-03-15 10:34:24.000000 astro-toolbox-0.0.1/src/astro_toolbox.egg-info/requires.txt
--rw-r--r--   0 romain     (501) staff       (20)       14 2023-03-15 10:34:24.000000 astro-toolbox-0.0.1/src/astro_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.075724 astro-toolbox-0.0.2/
+-rw-r--r--   0 romain     (501) staff       (20)    35160 2023-02-26 19:51:45.000000 astro-toolbox-0.0.2/LICENSE
+-rw-r--r--   0 romain     (501) staff       (20)     4669 2023-04-18 16:57:39.075835 astro-toolbox-0.0.2/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)     3847 2023-04-18 16:51:39.000000 astro-toolbox-0.0.2/README.md
+-rw-r--r--   0 romain     (501) staff       (20)     1422 2023-04-18 16:57:39.076168 astro-toolbox-0.0.2/setup.cfg
+-rw-r--r--   0 romain     (501) staff       (20)       68 2023-01-06 19:50:39.000000 astro-toolbox-0.0.2/setup.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.060951 astro-toolbox-0.0.2/src/
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.063473 astro-toolbox-0.0.2/src/astro_toolbox/
+-rw-r--r--   0 romain     (501) staff       (20)      968 2023-04-18 16:57:18.000000 astro-toolbox-0.0.2/src/astro_toolbox/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)       88 2023-02-07 20:30:19.000000 astro-toolbox-0.0.2/src/astro_toolbox/__main__.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.065686 astro-toolbox-0.0.2/src/astro_toolbox/angle/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.0.2/src/astro_toolbox/angle/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     2170 2023-03-10 13:03:07.000000 astro-toolbox-0.0.2/src/astro_toolbox/angle/degrees.py
+-rw-r--r--   0 romain     (501) staff       (20)     1665 2023-03-10 13:01:21.000000 astro-toolbox-0.0.2/src/astro_toolbox/angle/dms.py
+-rw-r--r--   0 romain     (501) staff       (20)     1579 2023-03-10 13:04:29.000000 astro-toolbox-0.0.2/src/astro_toolbox/angle/hms.py
+-rw-r--r--   0 romain     (501) staff       (20)     2230 2023-03-10 13:06:25.000000 astro-toolbox-0.0.2/src/astro_toolbox/angle/radians.py
+-rw-r--r--   0 romain     (501) staff       (20)    12495 2023-04-18 16:44:14.000000 astro-toolbox-0.0.2/src/astro_toolbox/command_line.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.066494 astro-toolbox-0.0.2/src/astro_toolbox/coordinates/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:50:39.000000 astro-toolbox-0.0.2/src/astro_toolbox/coordinates/__init__.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.066964 astro-toolbox-0.0.2/src/astro_toolbox/coordinates/data/
+-rw-r--r--   0 romain     (501) staff       (20)     2451 2023-02-02 19:46:48.000000 astro-toolbox-0.0.2/src/astro_toolbox/coordinates/data/orbital_elements.json
+-rw-r--r--   0 romain     (501) staff       (20)      419 2023-04-17 18:44:34.000000 astro-toolbox-0.0.2/src/astro_toolbox/coordinates/data/sites.json
+-rw-r--r--   0 romain     (501) staff       (20)     8253 2023-03-10 13:34:41.000000 astro-toolbox-0.0.2/src/astro_toolbox/coordinates/equatorial.py
+-rw-r--r--   0 romain     (501) staff       (20)     3299 2023-03-10 13:34:22.000000 astro-toolbox-0.0.2/src/astro_toolbox/coordinates/horizontal.py
+-rw-r--r--   0 romain     (501) staff       (20)     6648 2023-03-10 13:36:16.000000 astro-toolbox-0.0.2/src/astro_toolbox/coordinates/location.py
+-rw-r--r--   0 romain     (501) staff       (20)    11831 2023-03-10 13:22:52.000000 astro-toolbox-0.0.2/src/astro_toolbox/coordinates/solar_system.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.067669 astro-toolbox-0.0.2/src/astro_toolbox/query/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-08 12:07:57.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     2415 2023-03-10 13:41:22.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/catalogs.py
+-rw-r--r--   0 romain     (501) staff       (20)     3925 2023-04-17 19:20:22.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/ephemeris.py
+-rw-r--r--   0 romain     (501) staff       (20)     9672 2023-04-18 15:59:36.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.073918 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/
+-rw-r--r--   0 romain     (501) staff       (20)      457 2023-04-17 20:13:59.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/cloudy.png
+-rw-r--r--   0 romain     (501) staff       (20)      200 2023-04-17 18:29:15.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/direction_down.png
+-rw-r--r--   0 romain     (501) staff       (20)      193 2023-04-17 18:29:15.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/direction_down_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      220 2023-04-17 18:29:15.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/direction_down_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      256 2023-04-17 18:29:15.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/direction_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      215 2023-04-17 18:29:15.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/direction_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      270 2023-04-17 18:29:15.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/direction_up.png
+-rw-r--r--   0 romain     (501) staff       (20)      243 2023-04-17 18:29:15.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/direction_up_left.png
+-rw-r--r--   0 romain     (501) staff       (20)      228 2023-04-17 18:29:15.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/direction_up_right.png
+-rw-r--r--   0 romain     (501) staff       (20)      519 2023-04-17 20:23:18.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/drizzle.png
+-rw-r--r--   0 romain     (501) staff       (20)      388 2023-04-17 20:22:30.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/fog.png
+-rw-r--r--   0 romain     (501) staff       (20)      470 2023-04-17 21:01:44.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/haze.png
+-rw-r--r--   0 romain     (501) staff       (20)      613 2023-04-18 05:58:24.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/mainly_clear.png
+-rw-r--r--   0 romain     (501) staff       (20)      329 2023-04-17 20:17:22.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/na.png
+-rw-r--r--   0 romain     (501) staff       (20)      467 2023-04-17 21:07:00.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/partly_cloudy.png
+-rw-r--r--   0 romain     (501) staff       (20)      555 2023-04-17 20:23:54.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/rain.png
+-rw-r--r--   0 romain     (501) staff       (20)      545 2023-04-17 21:14:52.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/rain_mix.png
+-rw-r--r--   0 romain     (501) staff       (20)      410 2023-04-17 20:21:39.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/sandstorm.png
+-rw-r--r--   0 romain     (501) staff       (20)      525 2023-04-17 20:25:57.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/showers.png
+-rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 20:24:39.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/snow.png
+-rw-r--r--   0 romain     (501) staff       (20)      504 2023-04-17 15:03:01.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/sunny.png
+-rw-r--r--   0 romain     (501) staff       (20)      576 2023-04-17 21:16:48.000000 astro-toolbox-0.0.2/src/astro_toolbox/query/weather_icons/thunderstorm.png
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.074574 astro-toolbox-0.0.2/src/astro_toolbox/scripts/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-17 20:03:46.000000 astro-toolbox-0.0.2/src/astro_toolbox/scripts/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     1780 2023-02-08 13:53:17.000000 astro-toolbox-0.0.2/src/astro_toolbox/scripts/planning.py
+-rw-r--r--   0 romain     (501) staff       (20)    17118 2023-04-18 14:18:07.000000 astro-toolbox-0.0.2/src/astro_toolbox/scripts/plots.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.075081 astro-toolbox-0.0.2/src/astro_toolbox/time/
+-rw-r--r--   0 romain     (501) staff       (20)        0 2023-01-06 19:53:46.000000 astro-toolbox-0.0.2/src/astro_toolbox/time/__init__.py
+-rw-r--r--   0 romain     (501) staff       (20)     6330 2023-04-17 16:55:55.000000 astro-toolbox-0.0.2/src/astro_toolbox/time/core.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.075453 astro-toolbox-0.0.2/src/astro_toolbox/utils/
+-rw-r--r--   0 romain     (501) staff       (20)      441 2023-02-08 13:53:35.000000 astro-toolbox-0.0.2/src/astro_toolbox/utils/python_functions.py
+-rw-r--r--   0 romain     (501) staff       (20)      659 2023-04-17 16:11:48.000000 astro-toolbox-0.0.2/src/astro_toolbox/utils/strparser.py
+drwxr-xr-x   0 romain     (501) staff       (20)        0 2023-04-18 16:57:39.064917 astro-toolbox-0.0.2/src/astro_toolbox.egg-info/
+-rw-r--r--   0 romain     (501) staff       (20)     4669 2023-04-18 16:57:39.000000 astro-toolbox-0.0.2/src/astro_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 romain     (501) staff       (20)     2480 2023-04-18 16:57:39.000000 astro-toolbox-0.0.2/src/astro_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-04-18 16:57:39.000000 astro-toolbox-0.0.2/src/astro_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 romain     (501) staff       (20)       62 2023-04-18 16:57:39.000000 astro-toolbox-0.0.2/src/astro_toolbox.egg-info/entry_points.txt
+-rw-r--r--   0 romain     (501) staff       (20)        1 2023-01-18 11:00:43.000000 astro-toolbox-0.0.2/src/astro_toolbox.egg-info/not-zip-safe
+-rw-r--r--   0 romain     (501) staff       (20)      152 2023-04-18 16:57:39.000000 astro-toolbox-0.0.2/src/astro_toolbox.egg-info/requires.txt
+-rw-r--r--   0 romain     (501) staff       (20)       14 2023-04-18 16:57:39.000000 astro-toolbox-0.0.2/src/astro_toolbox.egg-info/top_level.txt
```

### Comparing `astro-toolbox-0.0.1/LICENSE` & `astro-toolbox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/PKG-INFO` & `astro-toolbox-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-toolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolbox for observationnal astronomy
 Home-page: https://github.com/rloustalet/astro_toolbox
 Author: Romain Loustalet Palengat
 Project-URL: Source, https://github.com/rloustalet/astro_toolbox
 Project-URL: Documentation, https://astro-toolbox.readthedocs.io/en/latest/
 Keywords: astro,toolbox,astro_toolbox,observationnal
 Platform: unix
@@ -36,15 +36,15 @@
 
 ### Synopsis
 
 astro-toolbox \[options1\] \<command\> \<argument\> \[options2\]
 
 # Options 1
 
-**-v, \--verbose** Program verbosity
+**-v, \--verbose** Program verbosity.
 
 # Commands
 
 # airmass
 
 This command allows you to plot airmass map of one or multiple objects.
 
@@ -126,14 +126,27 @@
 
 **-d, \--datetime** Option to inform a different date and time
 `-d 2022-12-18:20:35:55`, default is None (today date).
 
 **-l, \--location** Option to inform a location name `-l Greenwich`,
 default is None (last location used).
 
+# weather
+
+This command allows you to display forecasts of a given location.
+This command doesn\'t need any argument.
+
+# *options*
+
+**-l, \--location** Option to inform a location name `-l Greenwich`,
+default is None (last location used).
+
+**-d, \--days** Counter to inform the number of days to display,
+default is 1.
+
 ## Documentation
 
 The documentation is availale on [readthedocs.io](https://astro-toolbox.readthedocs.io/en/latest/)
 
 ## License
 
 Astropy is licensed under a GNU GPL license - see the [LICENSE](https://github.com/rloustalet/astro_toolbox/blob/main/LICENSE) file.
```

### Comparing `astro-toolbox-0.0.1/README.md` & `astro-toolbox-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ### Synopsis
 
 astro-toolbox \[options1\] \<command\> \<argument\> \[options2\]
 
 # Options 1
 
-**-v, \--verbose** Program verbosity
+**-v, \--verbose** Program verbosity.
 
 # Commands
 
 # airmass
 
 This command allows you to plot airmass map of one or multiple objects.
 
@@ -102,14 +102,27 @@
 
 **-d, \--datetime** Option to inform a different date and time
 `-d 2022-12-18:20:35:55`, default is None (today date).
 
 **-l, \--location** Option to inform a location name `-l Greenwich`,
 default is None (last location used).
 
+# weather
+
+This command allows you to display forecasts of a given location.
+This command doesn\'t need any argument.
+
+# *options*
+
+**-l, \--location** Option to inform a location name `-l Greenwich`,
+default is None (last location used).
+
+**-d, \--days** Counter to inform the number of days to display,
+default is 1.
+
 ## Documentation
 
 The documentation is availale on [readthedocs.io](https://astro-toolbox.readthedocs.io/en/latest/)
 
 ## License
 
 Astropy is licensed under a GNU GPL license - see the [LICENSE](https://github.com/rloustalet/astro_toolbox/blob/main/LICENSE) file.
```

### Comparing `astro-toolbox-0.0.1/setup.cfg` & `astro-toolbox-0.0.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 install_requires = numpy>=1.20
 	rich>=12.6.0
 	xmltodict>=0.13.0
 	click>=8.1.3
 	matplotlib>=3.5.0
 
 [options.package_data]
-astro_toolbox.coordinates = data/sites.json, data/orbital_elements.json
+astro_toolbox.coordinates = data/*.json,
+astro_toolbox.query = weather_icons/*.png
 
 [options.entry_points]
 console_scripts = 
 	astro-toolbox=astro_toolbox.__main__:main
 
 [options.extras_require]
 test = pytest
```

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/__init__.py` & `astro-toolbox-0.0.2/src/astro_toolbox/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from astro_toolbox.angle.hms import AngleHMS
 from astro_toolbox.coordinates.equatorial import Equatorial
 from astro_toolbox.coordinates.horizontal import Horizontal
 from astro_toolbox.coordinates.location import Location
 from astro_toolbox.coordinates.solar_system import Ephemeris
 from astro_toolbox.query.ephemeris import Horizons
 from astro_toolbox.query.catalogs import Simbad
+from astro_toolbox.query.weather import OpenMeteo
 
 from astro_toolbox.query.ephemeris import DICT_OBJECTS
 
 __all__ = [
     "AstroDateTime",
     "AngleDeg",
     "AngleRad",
@@ -23,10 +24,11 @@
     "AngleHMS",
     "Equatorial",
     "Horizontal",
     "Location",
     "Ephemeris",
     "Simbad",
     "Horizons",
+    "OpenMeteo",
 ]
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/angle/degrees.py` & `astro-toolbox-0.0.2/src/astro_toolbox/angle/degrees.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/angle/dms.py` & `astro-toolbox-0.0.2/src/astro_toolbox/angle/dms.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/angle/hms.py` & `astro-toolbox-0.0.2/src/astro_toolbox/angle/hms.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/angle/radians.py` & `astro-toolbox-0.0.2/src/astro_toolbox/angle/radians.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/command_line.py` & `astro-toolbox-0.0.2/src/astro_toolbox/command_line.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,25 @@
 from astro_toolbox.angle.degrees import AngleDeg
 from astro_toolbox.angle.hms import AngleHMS
 from astro_toolbox.time.core import AstroDateTime
 from astro_toolbox.coordinates.location import Location
 from astro_toolbox.coordinates.equatorial import Equatorial
 from astro_toolbox.query.ephemeris import Horizons
 from astro_toolbox.query.catalogs import Simbad
+from astro_toolbox.query.weather import OpenMeteo
 from astro_toolbox.scripts.planning import read_observatory_program
 from astro_toolbox.scripts.planning import get_multiple_informations
 from astro_toolbox.scripts.plots import airmas_map
 from astro_toolbox.scripts.plots import polarstar_plt_northern
 from astro_toolbox.scripts.plots import polarstar_plt_southern
 
 from astro_toolbox.query.ephemeris import DICT_OBJECTS
 
 PATH = pkg_resources.resource_filename('astro_toolbox', 'coordinates/data/')
+PATH_2 = pkg_resources.resource_filename('astro_toolbox', 'query/weather_icons/')
 
 @click.group()
 @click.option(
     "-v",
     "--verbose",
     count=True,
     default=0,
@@ -285,10 +287,52 @@
     """
     location = Location(location)
     if location.latitude.dmstodeg() > 0:
         polarstar_plt_northern(location, time)
     elif location.latitude.dmstodeg() < 0:
         polarstar_plt_southern(location, time)
 
+@cli.command('weather')
+@click.option("-l", "--location",
+            type=click.STRING,
+            default=None,
+            help='-l --location the site name default is None if None last site used')
+@click.option(
+    "-d",
+    "--days",
+    count=True,
+    default=1)
+def weather_command(location, days):
+    """Weather forecasts displayed from Open-Meteo
+
+    Parameters
+    ----------
+    location : str
+        Saved site name.
+    days : int
+        Number of days displayed.
+    """
+    last_time = '0000-00-00T00:00:00'
+    print(f'weather_forecasts @ {Location(location)}')
+    weather_forecasts = OpenMeteo(Location(location))
+    for time in weather_forecasts.data['hourly']['time'][:24*days]:
+        time += ':00'
+        if int(time[8:10]) != int(last_time[8:10]):
+            print('=' * 152)
+            print(f"|{'time':^25}|{'Temperature (°C)':^20}|" +
+                f"{'Humidity (%)':^20}|{'Precipitation (mm)':^20}|" +
+                f"{'Wind Speed (km/h)':^20}|{'Wind Direction (°)':^20}|" +
+                f"{'WMO':^20}|")
+            print('=' * 152)
+        else:
+            print('-' * 152)
+        print(f'|{time:^25}|{weather_forecasts.get_temperature(time):^20}|' +
+              f'{weather_forecasts.get_humidity(time):^20}|' +
+              f'{weather_forecasts.get_precipitation(time):^20}|' +
+              f'{weather_forecasts.get_wind_speed(time):^20}|' +
+              f'{weather_forecasts.get_wind_direction(time):^20}|' +
+              f'{weather_forecasts.get_wmo(time):^20}|')
+        last_time = time
+    print('-' * 152)
 
 if __name__ == '__main__':
     cli(False)
```

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/coordinates/data/orbital_elements.json` & `astro-toolbox-0.0.2/src/astro_toolbox/coordinates/data/orbital_elements.json`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/coordinates/equatorial.py` & `astro-toolbox-0.0.2/src/astro_toolbox/coordinates/equatorial.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/coordinates/horizontal.py` & `astro-toolbox-0.0.2/src/astro_toolbox/coordinates/horizontal.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/coordinates/location.py` & `astro-toolbox-0.0.2/src/astro_toolbox/coordinates/location.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/coordinates/solar_system.py` & `astro-toolbox-0.0.2/src/astro_toolbox/coordinates/solar_system.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/query/catalogs.py` & `astro-toolbox-0.0.2/src/astro_toolbox/query/catalogs.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/query/ephemeris.py` & `astro-toolbox-0.0.2/src/astro_toolbox/query/ephemeris.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         Parameters
         ----------
         object_name : str | int
             The object name or integer reference according to JPL Horizons.
         datetime : tuple | str
             Date and time as tuple or str (``dd:dd:dd.dd`` or ``ddhddmdd.dds``).
         location : Location
-            Observer location as Location class
+            Observer location as Location class.
         """
         self.name = object_name
         self.datetime = AstroDateTime(datetime)
         self.location = location
         self.object_data = self._get_data()
 
     def _get_data(self):
```

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/scripts/planning.py` & `astro-toolbox-0.0.2/src/astro_toolbox/scripts/planning.py`

 * *Files identical despite different names*

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/time/core.py` & `astro-toolbox-0.0.2/src/astro_toolbox/time/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,31 +18,35 @@
         Parameters
         ----------
         ut_time : tuple
             Tuple of the date and time in format (year,month,day,hour,minute,second)
         """
         if ut_time is None:
             ut_time = datetime.datetime.now(datetime.timezone.utc).timetuple()
-        elif isinstance(ut_time, str):
+        if ut_time is not None and isinstance(ut_time, str):
             ut_time = angle_parser(ut_time)
         if ut_time is not None and len(ut_time) == 3:
             ut_time += (12, 0, 0)
         self.date = (ut_time[0], ut_time[1], ut_time[2])
-        self.time = (ut_time[3], ut_time[4], ut_time[5])
+        self.time = (ut_time[3]%24, ut_time[4], ut_time[5])
+        if ut_time is not None and ut_time[3] > 23:
+            ut_time = self.get_gregorian(0) + ut_time[3:6]
+        self.date = (int(ut_time[0]), int(ut_time[1]), int(ut_time[2]))
+        self.time = (int(ut_time[3])%24, int(ut_time[4]),int(ut_time[5]))
 
     def __repr__(self):
         """Representative method.
 
         Returns
         -------
         string
             Return a class representative string.
         """
-        return (f'{self.date[0]:02d}-{self.date[1]:02d}-{self.date[2]:02d} '+
-                f'{self.time[0]:02d}:{self.time[1]:02d}:{self.time[2]:02d}')
+        return (f'{self.date[0]:02d}-{self.date[1]:02d}-{self.date[2]:02d}'+
+                f'T{self.time[0]:02d}:{self.time[1]:02d}:{self.time[2]:02d}')
 
     def get_year(self):
         """Get year
 
         Returns
         -------
         int
@@ -76,34 +80,76 @@
         Returns
         -------
         tuple
             Time in format (hour,minute,second).
         """
         return self.time
 
-    def get_jd(self):
-        """Get julian day with USNO formula.
+    def get_jd(self, delta: int = 0):
+        """Get julian day with possibility of delta days from USNO formula.
 
         .. math:: JD=367year-\\frac{7(year+\\frac{month+9}{12})}{4}>+\\frac{275month}{9}+
                 day+1721013.5+\\frac{UT}{24}-\n
         .. math:: 0.5sign(100year+month-190002.5)+0.5
 
+        Parameters
+        ----------
+        delta : int
+            Delta in days.
+
         Returns
         -------
         float
             Julian day.
         """
         julian_day = (367 * self.date[0] -
         int((7 * (self.date[0] +
         int((self.date[1] + 9) / 12.0))) / 4.0) +
         int((275 * self.date[1]) / 9.0) +
         self.date[2] + 1721013.5 +
         (self.time[0] + self.time[1] / 60.0 + self.time[2] / 3600) / 24.0 -
         0.5 * math.copysign(1, 100 * self.date[0] + self.date[1] - 190002.5) + 0.5)
-        return julian_day
+        return julian_day + delta
+
+    def get_gregorian(self, delta: int = 0):
+        """Get gregorian date with possibility of delta days from USNO formulas.
+
+        .. math:: g_1 = julian_day + 68569
+        .. math:: g_2 = <\\frac{4g_1}{146097}>
+        .. math:: g_1 = g_1 - <\\frac{146087g_2 + 3}{4}>
+        .. math:: g_3 = <\\frac{4000(g_1 + 1)}{1461001}>
+        .. math:: g_1 = g_1 - <\\frac{1461g_3}{4}> + 31
+        .. math:: g_4 = <\\frac{80g_3}{2447}>
+        .. math:: day = g_1 - <\\frac{2447g_4}{80}>
+        .. math:: g_1 = <\\frac{g_4}{11}
+        .. math:: month = g_4 + 2 - 12g_1
+        .. math:: year = 100(g_2 - 49) + g_3 + g_1
+
+        Parameters
+        ----------
+        delta : int, optional
+            Delta days, by default 0.
+
+        Returns
+        -------
+        tuple
+            Tuple of int containing year month and month day.
+        """
+        julian_day = int(self.get_jd(delta) + 0.5)
+        g_1 = julian_day + 68569
+        g_2 = int(4 * g_1 / 146097)
+        g_1 = g_1 - int((146097 * g_2 + 3) / 4)
+        g_3 = int(4000 * (g_1 + 1) / 1461001)
+        g_1 = g_1 - int(1461 * g_3 / 4) + 31
+        g_4 = int(80 * g_1 / 2447)
+        day = g_1 - int(2447 * g_4 / 80)
+        g_1 = int(g_4 / 11)
+        month = g_4 + 2 - 12 * g_1
+        year = 100 * (g_2 - 49) + g_3 + g_1
+        return year, month, day
 
     def get_year_day(self):
         """Get day of year.
 
         .. math:: N1 = floor(275 * month / 9)
         .. math:: N2 = floor((month + 9) / 12)
         .. math:: N3 = (1 + floor((year - 4 * floor(year / 4) + 2) / 3))
```

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox/utils/strparser.py` & `astro-toolbox-0.0.2/src/astro_toolbox/utils/strparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
         The angle value as str in format (`dd:dd:dd.dd` `dd°dd'dd.dd"` `ddhddmdd.dds` or `dd.dd`)
 
     Returns
     -------
     tuple | float
         the angle in correct format depending on its unity
     """
-    angle_list =  re.split(r"[\-:°'\"hms]",str_angle)
+    angle_list =  re.split(r"[\-:°'\"hmsT]",str_angle)
     if len(angle_list) == 1 and "." in angle_list[0]:
         return float(angle_list[0])
     angle = [int(val) for val in angle_list]
     if len(angle) == 3:
         angle[-1] = float(angle_list[-1])
     return tuple(angle)
```

### Comparing `astro-toolbox-0.0.1/src/astro_toolbox.egg-info/PKG-INFO` & `astro-toolbox-0.0.2/src/astro_toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-toolbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolbox for observationnal astronomy
 Home-page: https://github.com/rloustalet/astro_toolbox
 Author: Romain Loustalet Palengat
 Project-URL: Source, https://github.com/rloustalet/astro_toolbox
 Project-URL: Documentation, https://astro-toolbox.readthedocs.io/en/latest/
 Keywords: astro,toolbox,astro_toolbox,observationnal
 Platform: unix
@@ -36,15 +36,15 @@
 
 ### Synopsis
 
 astro-toolbox \[options1\] \<command\> \<argument\> \[options2\]
 
 # Options 1
 
-**-v, \--verbose** Program verbosity
+**-v, \--verbose** Program verbosity.
 
 # Commands
 
 # airmass
 
 This command allows you to plot airmass map of one or multiple objects.
 
@@ -126,14 +126,27 @@
 
 **-d, \--datetime** Option to inform a different date and time
 `-d 2022-12-18:20:35:55`, default is None (today date).
 
 **-l, \--location** Option to inform a location name `-l Greenwich`,
 default is None (last location used).
 
+# weather
+
+This command allows you to display forecasts of a given location.
+This command doesn\'t need any argument.
+
+# *options*
+
+**-l, \--location** Option to inform a location name `-l Greenwich`,
+default is None (last location used).
+
+**-d, \--days** Counter to inform the number of days to display,
+default is 1.
+
 ## Documentation
 
 The documentation is availale on [readthedocs.io](https://astro-toolbox.readthedocs.io/en/latest/)
 
 ## License
 
 Astropy is licensed under a GNU GPL license - see the [LICENSE](https://github.com/rloustalet/astro_toolbox/blob/main/LICENSE) file.
```

