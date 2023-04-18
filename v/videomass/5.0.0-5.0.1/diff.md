# Comparing `tmp/videomass-5.0.0.tar.gz` & `tmp/videomass-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "videomass-5.0.0.tar", last modified: Tue Apr 11 14:58:09 2023, max compression
+gzip compressed data, was "videomass-5.0.1.tar", last modified: Tue Apr 18 19:51:19 2023, max compression
```

## Comparing `videomass-5.0.0.tar` & `videomass-5.0.1.tar`

### file list

```diff
@@ -1,478 +1,479 @@
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.492029 videomass-5.0.0/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      616 2023-03-21 19:08:04.000000 videomass-5.0.0/AUTHORS
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      156 2023-01-13 00:08:29.000000 videomass-5.0.0/BUGS
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    73042 2023-04-11 12:41:12.000000 videomass-5.0.0/CHANGELOG
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2352 2023-03-31 16:50:16.000000 videomass-5.0.0/INSTALL
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35122 2023-01-13 00:08:29.000000 videomass-5.0.0/LICENSE
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      311 2023-01-13 00:08:29.000000 videomass-5.0.0/MANIFEST.in
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6040 2023-04-11 14:58:09.492029 videomass-5.0.0/PKG-INFO
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4509 2023-03-31 16:50:16.000000 videomass-5.0.0/README.md
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1188 2023-04-11 12:42:54.000000 videomass-5.0.0/TODO
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.424029 videomass-5.0.0/debian/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    39421 2023-04-11 12:41:44.000000 videomass-5.0.0/debian/changelog
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        3 2023-01-19 08:32:08.000000 videomass-5.0.0/debian/compat
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      882 2023-03-31 16:50:16.000000 videomass-5.0.0/debian/control
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1595 2023-01-19 08:32:08.000000 videomass-5.0.0/debian/copyright
--rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)      339 2023-01-19 08:32:08.000000 videomass-5.0.0/debian/rules
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.424029 videomass-5.0.0/debian/source/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)       12 2023-01-19 08:32:08.000000 videomass-5.0.0/debian/source/format
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)       32 2023-01-19 08:32:08.000000 videomass-5.0.0/debian/source/options
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.424029 videomass-5.0.0/develop/
--rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)     3077 2023-04-08 10:09:16.000000 videomass-5.0.0/develop/make_pot.sh
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.424029 videomass-5.0.0/develop/tools/
--rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)     2953 2023-03-22 12:03:23.000000 videomass-5.0.0/develop/tools/AppImage_Update_Tool.sh
--rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)     5841 2023-04-01 11:49:37.000000 videomass-5.0.0/develop/tools/AppImage_build.sh
--rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)     1779 2023-04-01 11:50:08.000000 videomass-5.0.0/develop/tools/AppRun
--rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)      982 2023-01-12 23:34:28.000000 videomass-5.0.0/develop/tools/create_ICNS.sh
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5742 2023-01-12 23:34:28.000000 videomass-5.0.0/develop/tools/generate_INNO_setup.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7661 2023-01-13 14:43:59.000000 videomass-5.0.0/develop/tools/inkscape2png.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    15762 2023-03-22 12:06:11.000000 videomass-5.0.0/develop/tools/pyinstaller_setup.py
--rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)     7173 2023-03-17 21:56:33.000000 videomass-5.0.0/develop/tools/rsvg2png.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.428029 videomass-5.0.0/docs/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      125 2023-01-19 08:32:08.000000 videomass-5.0.0/docs/EBU_resources.md
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      646 2023-01-19 08:32:08.000000 videomass-5.0.0/docs/localization_guidelines.md
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.416029 videomass-5.0.0/docs/man/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.428029 videomass-5.0.0/docs/man/man1/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1162 2023-01-19 08:32:08.000000 videomass-5.0.0/docs/man/man1/videomass.1.gz
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3787 2023-03-21 19:07:04.000000 videomass-5.0.0/docs/pyinstaller_setup.md
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1717 2023-03-31 16:50:16.000000 videomass-5.0.0/io.github.jeanslack.videomass.appdata.xml
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1069 2023-01-13 14:43:59.000000 videomass-5.0.0/launcher
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)       38 2023-04-11 14:58:09.492029 videomass-5.0.0/setup.cfg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5881 2023-03-21 19:07:04.000000 videomass-5.0.0/setup.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.428029 videomass-5.0.0/tests/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1527 2023-01-13 00:08:29.000000 videomass-5.0.0/tests/test_check_bin.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1691 2023-01-13 00:08:29.000000 videomass-5.0.0/tests/test_display_GUI.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1675 2023-01-13 00:08:29.000000 videomass-5.0.0/tests/test_ffprobe.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2782 2023-01-13 00:08:29.000000 videomass-5.0.0/tests/test_utils.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.428029 videomass-5.0.0/videomass/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.428029 videomass-5.0.0/videomass/FFMPEG/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2411 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/FFMPEG/NOTICE.rtf
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3108 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/FFMPEG/README
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/__init__.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.432029 videomass-5.0.0/videomass/art/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.432029 videomass-5.0.0/videomass/art/icons/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.432029 videomass-5.0.0/videomass/art/icons/Sign_Icons/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.432029 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1965 2023-04-01 21:58:04.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_concat.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12070 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_concat.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1236 2023-04-01 21:58:04.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_prst_mng.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7788 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_prst_mng.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1526 2023-04-01 21:58:04.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_slideshow.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    20798 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_slideshow.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1657 2023-04-01 21:58:04.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_videoconversions.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10445 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_videoconversions.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2166 2023-04-01 21:58:04.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_videopictures.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    40040 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_videopictures.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1096 2023-04-01 22:30:31.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/youtube.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13650 2023-04-01 22:30:31.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/youtube.svg
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.436029 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1885 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_concat.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12236 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_concat.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1239 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_prst_mng.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2687 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_prst_mng.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1630 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_slideshow.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    20707 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_slideshow.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1662 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_videoconversions.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10172 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_videoconversions.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1551 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_videopictures.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    76564 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_videopictures.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1009 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/youtube.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13701 2023-03-29 10:32:04.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/youtube.svg
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.436029 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1956 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_concat.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12236 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_concat.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1324 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_prst_mng.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2687 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_prst_mng.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1688 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_slideshow.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    20708 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_slideshow.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1720 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_videoconversions.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10173 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_videoconversions.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1551 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_videopictures.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    76564 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_videopictures.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1081 2023-03-29 10:33:03.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/youtube.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13702 2023-03-29 10:31:41.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/youtube.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35957 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Sign_Icons/COPYING-ICONS.txt
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.436029 videomass-5.0.0/videomass/art/icons/Videomass-Colours/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.444029 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      420 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/addtoprst.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5635 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/addtoprst.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      315 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/audiotrack.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4354 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/audiotrack.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      451 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/coloreq.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    25312 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/coloreq.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      591 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/configure.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4937 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/configure.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      480 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/copyprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7022 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/copyprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      168 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/deinterlace.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3058 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/deinterlace.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      252 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/delprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6077 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/delprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      606 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/denoise.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7573 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/denoise.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      281 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/edit-clear.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2241 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/edit-clear.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      489 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/editprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4757 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/editprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      361 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/newprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5049 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/newprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      344 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/playback.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2992 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/playback.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      519 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/player-volume.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5159 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/player-volume.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      275 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/playlist.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3153 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/playlist.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      752 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/preview.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5285 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/preview.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      521 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/preview_audio.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4039 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/preview_audio.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      273 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/stabilizer.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3092 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/stabilizer.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      569 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/timer.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2835 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/timer.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      261 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/transform-crop.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2737 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/transform-crop.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      517 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/transform-rotate.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2742 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/transform-rotate.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      441 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/transform-scale.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3829 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/transform-scale.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      266 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/volanalyze.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3216 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/volanalyze.svg
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.448029 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1079 2023-03-28 09:49:44.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/cleanup.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3460 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/cleanup.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      764 2023-03-28 09:49:44.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/convert.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4246 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/convert.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      663 2023-03-28 09:49:44.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/download.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    14879 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/download.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      696 2023-03-28 09:49:44.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/go-next.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3914 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/go-next.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      711 2023-03-28 09:49:44.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/go-previous.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3949 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/go-previous.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      742 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/home.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3081 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/home.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      669 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/play.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-28 09:23:48.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/play.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      731 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/properties.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4779 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/properties.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      525 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/statistics.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/statistics.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      517 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/stop.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2922 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/stop.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35929 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Colours/COPYING-ICONS.txt
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.448029 videomass-5.0.0/videomass/art/icons/Videomass-Dark/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.456029 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      425 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/addtoprst.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5628 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/addtoprst.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      308 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/audiotrack.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4396 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/audiotrack.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      438 2023-03-20 11:01:01.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/coloreq.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    25205 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/coloreq.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      568 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/configure.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4937 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/configure.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      442 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/copyprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7038 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/copyprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      165 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/deinterlace.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3058 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/deinterlace.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      252 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/delprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6077 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/delprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      622 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/denoise.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7573 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/denoise.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      281 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/edit-clear.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2241 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/edit-clear.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      428 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/editprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4768 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/editprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      394 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/newprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5049 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/newprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      321 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/playback.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2991 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/playback.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      497 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/player-volume.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5157 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/player-volume.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      273 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/playlist.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3180 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/playlist.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      776 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/preview.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5262 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/preview.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      464 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/preview_audio.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4075 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/preview_audio.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      262 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/stabilizer.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3085 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/stabilizer.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      547 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/timer.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2895 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/timer.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      289 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/transform-crop.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2738 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/transform-crop.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      467 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/transform-rotate.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2742 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/transform-rotate.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      509 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/transform-scale.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3829 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/transform-scale.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      273 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/volanalyze.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3215 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/volanalyze.svg
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.460029 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1003 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/cleanup.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3505 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/cleanup.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      705 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/convert.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3960 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/convert.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      599 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/download.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13215 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/download.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      713 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/go-next.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3913 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/go-next.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      716 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/go-previous.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3947 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/go-previous.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      701 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/home.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3081 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/home.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      638 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/play.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-28 09:46:52.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/play.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      748 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/properties.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4770 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/properties.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      525 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/statistics.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/statistics.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      478 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/stop.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2922 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/stop.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35926 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Dark/COPYING-ICONS.txt
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.460029 videomass-5.0.0/videomass/art/icons/Videomass-Light/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.464029 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      433 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/addtoprst.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5628 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/addtoprst.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      304 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/audiotrack.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4396 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/audiotrack.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      435 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/coloreq.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    25205 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/coloreq.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      513 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/configure.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4946 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/configure.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      399 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/copyprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7038 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/copyprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      165 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/deinterlace.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3058 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/deinterlace.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      252 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/delprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6077 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/delprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      682 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/denoise.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7573 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/denoise.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      281 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/edit-clear.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2241 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/edit-clear.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      473 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/editprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4768 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/editprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      390 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/newprf.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5047 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/newprf.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      342 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/playback.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2992 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/playback.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      493 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/player-volume.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5166 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/player-volume.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      275 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/playlist.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3180 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/playlist.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      780 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/preview.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5261 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/preview.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      461 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/preview_audio.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4079 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/preview_audio.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      259 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/stabilizer.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3093 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/stabilizer.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      616 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/timer.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2895 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/timer.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      298 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/transform-crop.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2745 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/transform-crop.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      502 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/transform-rotate.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2742 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/transform-rotate.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      513 2023-03-20 11:01:02.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/transform-scale.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3828 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/transform-scale.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      265 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/volanalyze.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3215 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/volanalyze.svg
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.468029 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1035 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/cleanup.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3505 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/cleanup.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      718 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/convert.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3960 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/convert.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      604 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/download.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13215 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/download.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      726 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/go-next.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3913 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/go-next.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      753 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/go-previous.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3947 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/go-previous.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      710 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/home.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3081 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/home.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      646 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/play.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-28 09:47:34.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/play.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      749 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/properties.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4770 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/properties.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      539 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/statistics.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/statistics.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      501 2023-03-28 09:49:45.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/stop.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2922 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/stop.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35926 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/Videomass-Light/COPYING-ICONS.txt
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.468029 videomass-5.0.0/videomass/art/icons/hicolor/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.416029 videomass-5.0.0/videomass/art/icons/hicolor/256x256/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.472029 videomass-5.0.0/videomass/art/icons/hicolor/256x256/apps/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    52997 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/hicolor/256x256/apps/videomass.png
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.416029 videomass-5.0.0/videomass/art/icons/hicolor/48x48/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.472029 videomass-5.0.0/videomass/art/icons/hicolor/48x48/apps/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5196 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/hicolor/48x48/apps/videomass.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    22362 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/hicolor/48x48/apps/videomass.xpm
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35225 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/hicolor/COPYING-ICONS.txt
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.416029 videomass-5.0.0/videomass/art/icons/hicolor/scalable/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.472029 videomass-5.0.0/videomass/art/icons/hicolor/scalable/apps/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    23218 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/hicolor/scalable/apps/videomass.svg
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    20866 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/icons/videomass.png
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      220 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/io.github.jeanslack.videomass.desktop
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)  1154230 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/videomass.icns
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   154088 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/art/videomass.ico
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     9778 2023-04-01 17:16:01.000000 videomass-5.0.0/videomass/gui_app.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.472029 videomass-5.0.0/videomass/locale/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      565 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/locale/README
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.416029 videomass-5.0.0/videomass/locale/en_US/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.472029 videomass-5.0.0/videomass/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      335 2023-04-10 12:33:37.000000 videomass-5.0.0/videomass/locale/en_US/LC_MESSAGES/videomass.mo
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    92486 2023-04-10 12:33:37.000000 videomass-5.0.0/videomass/locale/en_US/LC_MESSAGES/videomass.po
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.420029 videomass-5.0.0/videomass/locale/es_CU/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.472029 videomass-5.0.0/videomass/locale/es_CU/LC_MESSAGES/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    67413 2023-04-10 12:33:53.000000 videomass-5.0.0/videomass/locale/es_CU/LC_MESSAGES/videomass.mo
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   152612 2023-04-10 12:33:53.000000 videomass-5.0.0/videomass/locale/es_CU/LC_MESSAGES/videomass.po
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.420029 videomass-5.0.0/videomass/locale/es_ES/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.472029 videomass-5.0.0/videomass/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    67413 2023-04-10 12:34:11.000000 videomass-5.0.0/videomass/locale/es_ES/LC_MESSAGES/videomass.mo
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   152612 2023-04-10 12:34:11.000000 videomass-5.0.0/videomass/locale/es_ES/LC_MESSAGES/videomass.po
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.420029 videomass-5.0.0/videomass/locale/es_MX/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.472029 videomass-5.0.0/videomass/locale/es_MX/LC_MESSAGES/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    67413 2023-04-10 12:34:27.000000 videomass-5.0.0/videomass/locale/es_MX/LC_MESSAGES/videomass.mo
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   152612 2023-04-10 12:34:27.000000 videomass-5.0.0/videomass/locale/es_MX/LC_MESSAGES/videomass.po
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.420029 videomass-5.0.0/videomass/locale/fr_FR/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.472029 videomass-5.0.0/videomass/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    70835 2023-04-10 12:34:44.000000 videomass-5.0.0/videomass/locale/fr_FR/LC_MESSAGES/videomass.mo
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   154491 2023-04-10 12:34:44.000000 videomass-5.0.0/videomass/locale/fr_FR/LC_MESSAGES/videomass.po
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.420029 videomass-5.0.0/videomass/locale/it_IT/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.476029 videomass-5.0.0/videomass/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    96595 2023-04-10 12:33:10.000000 videomass-5.0.0/videomass/locale/it_IT/LC_MESSAGES/videomass.mo
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   179594 2023-04-10 12:33:10.000000 videomass-5.0.0/videomass/locale/it_IT/LC_MESSAGES/videomass.po
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.420029 videomass-5.0.0/videomass/locale/nl_NL/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.476029 videomass-5.0.0/videomass/locale/nl_NL/LC_MESSAGES/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    60147 2023-04-10 12:35:01.000000 videomass-5.0.0/videomass/locale/nl_NL/LC_MESSAGES/videomass.mo
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   162093 2023-04-10 12:35:01.000000 videomass-5.0.0/videomass/locale/nl_NL/LC_MESSAGES/videomass.po
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.420029 videomass-5.0.0/videomass/locale/pt_BR/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.476029 videomass-5.0.0/videomass/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    52777 2023-04-10 12:35:16.000000 videomass-5.0.0/videomass/locale/pt_BR/LC_MESSAGES/videomass.mo
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   164019 2023-04-10 12:35:16.000000 videomass-5.0.0/videomass/locale/pt_BR/LC_MESSAGES/videomass.po
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.420029 videomass-5.0.0/videomass/locale/ru_RU/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.476029 videomass-5.0.0/videomass/locale/ru_RU/LC_MESSAGES/
--rw-rw-rw-   0 jeanslack  (1000) jeanslack  (1000)   127777 2023-04-11 12:33:00.000000 videomass-5.0.0/videomass/locale/ru_RU/LC_MESSAGES/videomass.mo
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   220241 2023-04-11 12:33:00.000000 videomass-5.0.0/videomass/locale/ru_RU/LC_MESSAGES/videomass.po
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    92494 2023-04-10 12:19:42.000000 videomass-5.0.0/videomass/locale/videomass.pot
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.420029 videomass-5.0.0/videomass/locale/zh_CN/
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.476029 videomass-5.0.0/videomass/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    30134 2023-04-10 12:35:50.000000 videomass-5.0.0/videomass/locale/zh_CN/LC_MESSAGES/videomass.mo
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   144453 2023-04-10 12:35:50.000000 videomass-5.0.0/videomass/locale/zh_CN/LC_MESSAGES/videomass.po
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.476029 videomass-5.0.0/videomass/share/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      187 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/README
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.480029 videomass-5.0.0/videomass/share/presets/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2619 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Audio_Conversions.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      711 2023-02-18 00:17:17.000000 videomass-5.0.0/videomass/share/presets/Audio_removing_from_video.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5989 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Coding to DVD by GMJCZP.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    14966 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Coding-to-DVD-by-GMJCZP.md
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1228 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Create animated GIFs.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1812 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Embed_Subtitles_to_Video.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1355 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Encoding_for_Devices.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2904 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Extract_audio_from_Videos.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1027 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/For_Archive_Collection.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      814 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Merging_audio_and_video.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        3 2023-02-18 00:17:17.000000 videomass-5.0.0/videomass/share/presets/My_Profiles.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1169 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Utilities.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3935 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Video Encoding AV1.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3481 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Video Encoding VP9-WebM.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1774 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Video effects.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1930 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Video-Repair.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1862 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Video_Stabilizer.prst
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4409 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/Video_Streaming.prst
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.480029 videomass-5.0.0/videomass/share/presets/version/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        5 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/share/presets/version/version.txt
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.484029 videomass-5.0.0/videomass/vdms_dialogs/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/vdms_dialogs/__init__.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2992 2023-03-31 16:50:16.000000 videomass-5.0.0/videomass/vdms_dialogs/about.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    19377 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_dialogs/audiodialogs.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5966 2023-04-03 10:27:52.000000 videomass-5.0.0/videomass/vdms_dialogs/epilogue.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     9774 2023-03-27 08:43:50.000000 videomass-5.0.0/videomass/vdms_dialogs/ffmpeg_codecs.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     9329 2023-03-27 08:47:51.000000 videomass-5.0.0/videomass/vdms_dialogs/ffmpeg_conf.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7128 2023-03-27 08:47:49.000000 videomass-5.0.0/videomass/vdms_dialogs/ffmpeg_formats.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    17894 2023-03-29 21:58:26.000000 videomass-5.0.0/videomass/vdms_dialogs/ffmpeg_help.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    21187 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_dialogs/filter_colorcorrection.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    24148 2023-04-11 14:52:21.000000 videomass-5.0.0/videomass/vdms_dialogs/filter_crop.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    23619 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_dialogs/filter_deinterlace.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12450 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_dialogs/filter_denoisers.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    22029 2023-04-03 10:30:42.000000 videomass-5.0.0/videomass/vdms_dialogs/filter_scale.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    37831 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_dialogs/filter_stab.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12093 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_dialogs/filter_transpose.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    14985 2023-03-28 18:28:35.000000 videomass-5.0.0/videomass/vdms_dialogs/mediainfo.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    44117 2023-04-01 22:30:31.000000 videomass-5.0.0/videomass/vdms_dialogs/preferences.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    14066 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_dialogs/presets_addnew.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7279 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_dialogs/renamer.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10460 2023-01-13 14:43:59.000000 videomass-5.0.0/videomass/vdms_dialogs/set_timestamp.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     8207 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/vdms_dialogs/showlogs.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    11846 2023-03-27 08:46:43.000000 videomass-5.0.0/videomass/vdms_dialogs/shownormlist.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5371 2023-01-13 14:43:59.000000 videomass-5.0.0/videomass/vdms_dialogs/videomass_check_version.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5243 2023-03-27 08:47:46.000000 videomass-5.0.0/videomass/vdms_dialogs/while_playing.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4975 2023-03-04 13:42:00.000000 videomass-5.0.0/videomass/vdms_dialogs/widget_utils.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    25435 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/vdms_dialogs/wizard_dlg.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.484029 videomass-5.0.0/videomass/vdms_io/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/vdms_io/__init__.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3823 2023-02-24 17:41:33.000000 videomass-5.0.0/videomass/vdms_io/checkup.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6994 2023-04-07 15:37:26.000000 videomass-5.0.0/videomass/vdms_io/io_tools.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1952 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_io/make_filelog.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6445 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_io/presets_manager_prop.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.484029 videomass-5.0.0/videomass/vdms_main/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/vdms_main/__init__.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    69172 2023-04-08 12:34:49.000000 videomass-5.0.0/videomass/vdms_main/main_frame.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.484029 videomass-5.0.0/videomass/vdms_miniframes/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/vdms_miniframes/__init__.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    23063 2023-04-11 14:13:15.000000 videomass-5.0.0/videomass/vdms_miniframes/timeline.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.488029 videomass-5.0.0/videomass/vdms_panels/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/vdms_panels/__init__.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   112280 2023-04-07 21:08:30.000000 videomass-5.0.0/videomass/vdms_panels/av_conversions.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10290 2023-04-01 22:30:31.000000 videomass-5.0.0/videomass/vdms_panels/choose_topic.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    14156 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_panels/concatenate.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    22775 2023-04-08 12:38:04.000000 videomass-5.0.0/videomass/vdms_panels/filedrop.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10929 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_panels/hevc_avc.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6484 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_panels/libaom.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    17078 2023-04-01 22:30:31.000000 videomass-5.0.0/videomass/vdms_panels/long_processing_task.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    42324 2023-04-07 15:47:12.000000 videomass-5.0.0/videomass/vdms_panels/presets_manager.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    30075 2023-04-08 11:14:37.000000 videomass-5.0.0/videomass/vdms_panels/sequence_to_video.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    26706 2023-04-08 11:18:18.000000 videomass-5.0.0/videomass/vdms_panels/video_to_sequence.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6436 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_panels/webm.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.488029 videomass-5.0.0/videomass/vdms_sys/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/vdms_sys/__init__.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1111 2023-01-16 11:12:25.000000 videomass-5.0.0/videomass/vdms_sys/app_const.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4716 2023-03-22 11:00:27.000000 videomass-5.0.0/videomass/vdms_sys/argparser.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    24119 2023-04-01 22:30:31.000000 videomass-5.0.0/videomass/vdms_sys/configurator.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3753 2023-04-08 12:38:59.000000 videomass-5.0.0/videomass/vdms_sys/msg_info.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     8405 2023-04-01 22:30:31.000000 videomass-5.0.0/videomass/vdms_sys/settings_manager.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.488029 videomass-5.0.0/videomass/vdms_threads/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/vdms_threads/__init__.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6517 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/check_bin.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6069 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/concat_demuxer.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5379 2023-01-13 14:43:59.000000 videomass-5.0.0/videomass/vdms_threads/ffplay_file.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3229 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/ffprobe.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3754 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/generic_downloads.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4289 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/generic_task.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6938 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/one_pass.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5997 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/picture_exporting.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13725 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/slideshow.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10173 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/two_pass.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    11175 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/two_pass_ebu.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13996 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_threads/video_stabilization.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5365 2023-04-07 15:36:59.000000 videomass-5.0.0/videomass/vdms_threads/volumedetect.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.488029 videomass-5.0.0/videomass/vdms_utils/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.0/videomass/vdms_utils/__init__.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1275 2023-01-13 14:43:59.000000 videomass-5.0.0/videomass/vdms_utils/get_bmpfromsvg.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    19274 2023-03-17 21:56:33.000000 videomass-5.0.0/videomass/vdms_utils/utils.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.492029 videomass-5.0.0/videomass/vdms_ytdlp/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/vdms_ytdlp/__init__.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12549 2023-03-31 16:50:16.000000 videomass-5.0.0/videomass/vdms_ytdlp/formatcode.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    11029 2023-03-28 12:11:17.000000 videomass-5.0.0/videomass/vdms_ytdlp/long_task_ytdlp.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    26223 2023-04-03 10:18:01.000000 videomass-5.0.0/videomass/vdms_ytdlp/main_ytdlp.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10889 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/vdms_ytdlp/playlist_indexing.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10253 2023-04-01 22:30:31.000000 videomass-5.0.0/videomass/vdms_ytdlp/textdrop.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     8151 2023-04-04 16:01:07.000000 videomass-5.0.0/videomass/vdms_ytdlp/ydl_downloader.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3337 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/vdms_ytdlp/ydl_extractinfo.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6358 2023-03-21 19:07:04.000000 videomass-5.0.0/videomass/vdms_ytdlp/ydl_mediainfo.py
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    33217 2023-03-31 16:50:16.000000 videomass-5.0.0/videomass/vdms_ytdlp/youtubedl_ui.py
-drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 14:58:09.428029 videomass-5.0.0/videomass.egg-info/
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6040 2023-04-11 14:58:09.000000 videomass-5.0.0/videomass.egg-info/PKG-INFO
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    19529 2023-04-11 14:58:09.000000 videomass-5.0.0/videomass.egg-info/SOURCES.txt
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        1 2023-04-11 14:58:09.000000 videomass-5.0.0/videomass.egg-info/dependency_links.txt
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)       49 2023-04-11 14:58:09.000000 videomass-5.0.0/videomass.egg-info/entry_points.txt
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        1 2023-04-11 14:58:09.000000 videomass-5.0.0/videomass.egg-info/not-zip-safe
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      130 2023-04-11 14:58:09.000000 videomass-5.0.0/videomass.egg-info/requires.txt
--rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)       10 2023-04-11 14:58:09.000000 videomass-5.0.0/videomass.egg-info/top_level.txt
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.612019 videomass-5.0.1/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      669 2023-04-17 21:02:09.000000 videomass-5.0.1/AUTHORS
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      156 2023-01-13 00:08:29.000000 videomass-5.0.1/BUGS
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    73660 2023-04-18 19:50:28.000000 videomass-5.0.1/CHANGELOG
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2352 2023-03-31 16:50:16.000000 videomass-5.0.1/INSTALL
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35122 2023-01-13 00:08:29.000000 videomass-5.0.1/LICENSE
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      311 2023-01-13 00:08:29.000000 videomass-5.0.1/MANIFEST.in
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6040 2023-04-18 19:51:19.612019 videomass-5.0.1/PKG-INFO
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4509 2023-03-31 16:50:16.000000 videomass-5.0.1/README.md
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1188 2023-04-11 17:55:13.000000 videomass-5.0.1/TODO
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.552019 videomass-5.0.1/debian/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    40103 2023-04-18 19:50:28.000000 videomass-5.0.1/debian/changelog
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        3 2023-01-19 08:32:08.000000 videomass-5.0.1/debian/compat
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      882 2023-03-31 16:50:16.000000 videomass-5.0.1/debian/control
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1595 2023-01-19 08:32:08.000000 videomass-5.0.1/debian/copyright
+-rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)      339 2023-01-19 08:32:08.000000 videomass-5.0.1/debian/rules
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.552019 videomass-5.0.1/debian/source/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)       12 2023-01-19 08:32:08.000000 videomass-5.0.1/debian/source/format
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)       32 2023-01-19 08:32:08.000000 videomass-5.0.1/debian/source/options
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.552019 videomass-5.0.1/develop/
+-rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)     3113 2023-04-17 21:02:09.000000 videomass-5.0.1/develop/make_pot.sh
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.552019 videomass-5.0.1/develop/tools/
+-rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)     2953 2023-03-22 12:03:23.000000 videomass-5.0.1/develop/tools/AppImage_Update_Tool.sh
+-rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)     5841 2023-04-01 11:49:37.000000 videomass-5.0.1/develop/tools/AppImage_build.sh
+-rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)     1779 2023-04-01 11:50:08.000000 videomass-5.0.1/develop/tools/AppRun
+-rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)      982 2023-01-12 23:34:28.000000 videomass-5.0.1/develop/tools/create_ICNS.sh
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5742 2023-01-12 23:34:28.000000 videomass-5.0.1/develop/tools/generate_INNO_setup.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7661 2023-01-13 14:43:59.000000 videomass-5.0.1/develop/tools/inkscape2png.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    15762 2023-03-22 12:06:11.000000 videomass-5.0.1/develop/tools/pyinstaller_setup.py
+-rwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)     7173 2023-03-17 21:56:33.000000 videomass-5.0.1/develop/tools/rsvg2png.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.556019 videomass-5.0.1/docs/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      125 2023-01-19 08:32:08.000000 videomass-5.0.1/docs/EBU_resources.md
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      646 2023-01-19 08:32:08.000000 videomass-5.0.1/docs/localization_guidelines.md
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.544019 videomass-5.0.1/docs/man/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.556019 videomass-5.0.1/docs/man/man1/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1162 2023-01-19 08:32:08.000000 videomass-5.0.1/docs/man/man1/videomass.1.gz
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3787 2023-03-21 19:07:04.000000 videomass-5.0.1/docs/pyinstaller_setup.md
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1717 2023-03-31 16:50:16.000000 videomass-5.0.1/io.github.jeanslack.videomass.appdata.xml
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1069 2023-01-13 14:43:59.000000 videomass-5.0.1/launcher
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)       38 2023-04-18 19:51:19.612019 videomass-5.0.1/setup.cfg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5881 2023-03-21 19:07:04.000000 videomass-5.0.1/setup.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.556019 videomass-5.0.1/tests/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1527 2023-01-13 00:08:29.000000 videomass-5.0.1/tests/test_check_bin.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1691 2023-01-13 00:08:29.000000 videomass-5.0.1/tests/test_display_GUI.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1675 2023-01-13 00:08:29.000000 videomass-5.0.1/tests/test_ffprobe.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2782 2023-01-13 00:08:29.000000 videomass-5.0.1/tests/test_utils.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.556019 videomass-5.0.1/videomass/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.556019 videomass-5.0.1/videomass/FFMPEG/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2411 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/FFMPEG/NOTICE.rtf
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3108 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/FFMPEG/README
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/__init__.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.556019 videomass-5.0.1/videomass/art/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.560019 videomass-5.0.1/videomass/art/icons/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.560019 videomass-5.0.1/videomass/art/icons/Sign_Icons/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.560019 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1965 2023-04-01 21:58:04.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_concat.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12070 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_concat.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1236 2023-04-01 21:58:04.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_prst_mng.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7788 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_prst_mng.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1526 2023-04-01 21:58:04.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_slideshow.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    20798 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_slideshow.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1657 2023-04-01 21:58:04.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_videoconversions.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10445 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_videoconversions.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2166 2023-04-01 21:58:04.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_videopictures.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    40040 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_videopictures.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1096 2023-04-01 22:30:31.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/youtube.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13650 2023-04-01 22:30:31.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/youtube.svg
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.560019 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1885 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_concat.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12236 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_concat.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1239 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_prst_mng.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2687 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_prst_mng.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1630 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_slideshow.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    20707 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_slideshow.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1662 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_videoconversions.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10172 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_videoconversions.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1551 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_videopictures.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    76564 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_videopictures.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1009 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/youtube.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13701 2023-03-29 10:32:04.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/youtube.svg
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.564019 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1956 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_concat.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12236 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_concat.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1324 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_prst_mng.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2687 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_prst_mng.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1688 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_slideshow.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    20708 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_slideshow.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1720 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_videoconversions.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10173 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_videoconversions.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1551 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_videopictures.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    76564 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_videopictures.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1081 2023-03-29 10:33:03.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/youtube.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13702 2023-03-29 10:31:41.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/youtube.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35957 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Sign_Icons/COPYING-ICONS.txt
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.564019 videomass-5.0.1/videomass/art/icons/Videomass-Colours/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.572018 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      420 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/addtoprst.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5635 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/addtoprst.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      315 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/audiotrack.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4354 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/audiotrack.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      451 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/coloreq.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    25312 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/coloreq.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      591 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/configure.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4937 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/configure.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      480 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/copyprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7022 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/copyprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      168 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/deinterlace.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3058 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/deinterlace.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      252 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/delprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6077 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/delprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      606 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/denoise.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7573 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/denoise.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      281 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/edit-clear.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2241 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/edit-clear.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      489 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/editprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4757 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/editprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      361 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/newprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5049 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/newprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      344 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/playback.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2992 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/playback.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      519 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/player-volume.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5159 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/player-volume.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      275 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/playlist.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3153 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/playlist.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      752 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/preview.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5285 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/preview.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      521 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/preview_audio.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4039 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/preview_audio.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      273 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/stabilizer.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3092 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/stabilizer.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      569 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/timer.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2835 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/timer.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      261 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/transform-crop.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2737 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/transform-crop.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      517 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/transform-rotate.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2742 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/transform-rotate.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      441 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/transform-scale.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3829 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/transform-scale.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      266 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/volanalyze.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3216 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/volanalyze.svg
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.576019 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1079 2023-03-28 09:49:44.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/cleanup.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3460 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/cleanup.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      764 2023-03-28 09:49:44.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/convert.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4246 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/convert.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      663 2023-03-28 09:49:44.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/download.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    14879 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/download.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      696 2023-03-28 09:49:44.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/go-next.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3914 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/go-next.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      711 2023-03-28 09:49:44.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/go-previous.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3949 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/go-previous.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      742 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/home.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3081 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/home.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      669 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/play.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-28 09:23:48.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/play.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      731 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/properties.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4779 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/properties.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      525 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/statistics.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/statistics.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      517 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/stop.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2922 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/stop.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35929 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Colours/COPYING-ICONS.txt
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.576019 videomass-5.0.1/videomass/art/icons/Videomass-Dark/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.580019 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      425 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/addtoprst.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5628 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/addtoprst.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      308 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/audiotrack.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4396 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/audiotrack.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      438 2023-03-20 11:01:01.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/coloreq.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    25205 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/coloreq.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      568 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/configure.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4937 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/configure.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      442 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/copyprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7038 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/copyprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      165 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/deinterlace.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3058 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/deinterlace.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      252 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/delprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6077 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/delprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      622 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/denoise.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7573 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/denoise.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      281 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/edit-clear.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2241 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/edit-clear.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      428 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/editprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4768 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/editprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      394 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/newprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5049 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/newprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      321 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/playback.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2991 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/playback.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      497 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/player-volume.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5157 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/player-volume.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      273 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/playlist.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3180 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/playlist.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      776 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/preview.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5262 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/preview.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      464 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/preview_audio.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4075 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/preview_audio.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      262 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/stabilizer.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3085 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/stabilizer.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      547 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/timer.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2895 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/timer.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      289 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/transform-crop.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2738 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/transform-crop.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      467 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/transform-rotate.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2742 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/transform-rotate.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      509 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/transform-scale.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3829 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/transform-scale.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      273 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/volanalyze.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3215 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/volanalyze.svg
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.584019 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1003 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/cleanup.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3505 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/cleanup.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      705 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/convert.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3960 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/convert.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      599 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/download.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13215 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/download.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      713 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/go-next.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3913 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/go-next.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      716 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/go-previous.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3947 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/go-previous.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      701 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/home.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3081 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/home.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      638 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/play.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-28 09:46:52.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/play.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      748 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/properties.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4770 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/properties.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      525 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/statistics.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/statistics.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      478 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/stop.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2922 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/stop.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35926 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Dark/COPYING-ICONS.txt
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.584019 videomass-5.0.1/videomass/art/icons/Videomass-Light/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.592019 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      433 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/addtoprst.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5628 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/addtoprst.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      304 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/audiotrack.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4396 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/audiotrack.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      435 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/coloreq.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    25205 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/coloreq.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      513 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/configure.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4946 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/configure.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      399 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/copyprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7038 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/copyprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      165 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/deinterlace.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3058 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/deinterlace.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      252 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/delprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6077 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/delprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      682 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/denoise.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7573 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/denoise.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      281 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/edit-clear.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2241 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/edit-clear.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      473 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/editprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4768 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/editprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      390 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/newprf.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5047 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/newprf.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      342 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/playback.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2992 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/playback.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      493 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/player-volume.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5166 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/player-volume.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      275 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/playlist.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3180 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/playlist.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      780 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/preview.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5261 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/preview.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      461 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/preview_audio.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4079 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/preview_audio.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      259 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/stabilizer.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3093 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/stabilizer.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      616 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/timer.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2895 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/timer.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      298 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/transform-crop.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2745 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/transform-crop.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      502 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/transform-rotate.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2742 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/transform-rotate.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      513 2023-03-20 11:01:02.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/transform-scale.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3828 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/transform-scale.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      265 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/volanalyze.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3215 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/volanalyze.svg
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.592019 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1035 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/cleanup.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3505 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/cleanup.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      718 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/convert.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3960 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/convert.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      604 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/download.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13215 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/download.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      726 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/go-next.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3913 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/go-next.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      753 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/go-previous.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3947 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/go-previous.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      710 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/home.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3081 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/home.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      646 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/play.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-28 09:47:34.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/play.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      749 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/properties.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4770 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/properties.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      539 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/statistics.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3372 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/statistics.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      501 2023-03-28 09:49:45.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/stop.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2922 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/stop.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35926 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/Videomass-Light/COPYING-ICONS.txt
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.592019 videomass-5.0.1/videomass/art/icons/hicolor/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/art/icons/hicolor/256x256/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.592019 videomass-5.0.1/videomass/art/icons/hicolor/256x256/apps/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    52997 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/hicolor/256x256/apps/videomass.png
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/art/icons/hicolor/48x48/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.592019 videomass-5.0.1/videomass/art/icons/hicolor/48x48/apps/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5196 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/hicolor/48x48/apps/videomass.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    22362 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/hicolor/48x48/apps/videomass.xpm
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    35225 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/hicolor/COPYING-ICONS.txt
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/art/icons/hicolor/scalable/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.596019 videomass-5.0.1/videomass/art/icons/hicolor/scalable/apps/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    23218 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/hicolor/scalable/apps/videomass.svg
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    20866 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/icons/videomass.png
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      220 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/io.github.jeanslack.videomass.desktop
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)  1154230 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/videomass.icns
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   154088 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/art/videomass.ico
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     9778 2023-04-01 17:16:01.000000 videomass-5.0.1/videomass/gui_app.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.596019 videomass-5.0.1/videomass/locale/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      565 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/locale/README
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/locale/en_US/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.596019 videomass-5.0.1/videomass/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      335 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/en_US/LC_MESSAGES/videomass.mo
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    93831 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/en_US/LC_MESSAGES/videomass.po
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/locale/es_CU/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.596019 videomass-5.0.1/videomass/locale/es_CU/LC_MESSAGES/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    67014 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/es_CU/LC_MESSAGES/videomass.mo
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   154383 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/es_CU/LC_MESSAGES/videomass.po
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/locale/es_ES/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.596019 videomass-5.0.1/videomass/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    67014 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/es_ES/LC_MESSAGES/videomass.mo
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   154383 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/es_ES/LC_MESSAGES/videomass.po
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/locale/es_MX/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.596019 videomass-5.0.1/videomass/locale/es_MX/LC_MESSAGES/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    67014 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/es_MX/LC_MESSAGES/videomass.mo
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   154383 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/es_MX/LC_MESSAGES/videomass.po
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/locale/fr_FR/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.596019 videomass-5.0.1/videomass/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    70407 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/fr_FR/LC_MESSAGES/videomass.mo
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   156269 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/fr_FR/LC_MESSAGES/videomass.po
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/locale/it_IT/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.596019 videomass-5.0.1/videomass/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    98213 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/it_IT/LC_MESSAGES/videomass.mo
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   181678 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/it_IT/LC_MESSAGES/videomass.po
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/locale/nl_NL/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.596019 videomass-5.0.1/videomass/locale/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    59745 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/nl_NL/LC_MESSAGES/videomass.mo
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   163865 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/nl_NL/LC_MESSAGES/videomass.po
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/locale/pt_BR/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.596019 videomass-5.0.1/videomass/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    52714 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/pt_BR/LC_MESSAGES/videomass.mo
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   165721 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/pt_BR/LC_MESSAGES/videomass.po
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/locale/ru_RU/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.600019 videomass-5.0.1/videomass/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   128496 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/ru_RU/LC_MESSAGES/videomass.mo
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   221768 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/ru_RU/LC_MESSAGES/videomass.po
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    93839 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/videomass.pot
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.548019 videomass-5.0.1/videomass/locale/zh_CN/
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.600019 videomass-5.0.1/videomass/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    30218 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/zh_CN/LC_MESSAGES/videomass.mo
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   146091 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/locale/zh_CN/LC_MESSAGES/videomass.po
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.600019 videomass-5.0.1/videomass/share/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      187 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/share/README
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.600019 videomass-5.0.1/videomass/share/presets/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2619 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Audio_Conversions.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      711 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Audio_removing_from_video.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5989 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Coding to DVD by GMJCZP.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    14966 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Coding-to-DVD-by-GMJCZP.md
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1228 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Create animated GIFs.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1812 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Embed_Subtitles_to_Video.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1355 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Encoding_for_Devices.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2904 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Extract_audio_from_Videos.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1027 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/For_Archive_Collection.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      814 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Merging_audio_and_video.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        3 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/My_Profiles.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1169 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Utilities.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3935 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Video Encoding AV1.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3481 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Video Encoding VP9-WebM.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1774 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Video effects.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1930 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Video-Repair.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1862 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Video_Stabilizer.prst
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4409 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/Video_Streaming.prst
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.600019 videomass-5.0.1/videomass/share/presets/version/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        5 2023-04-17 11:00:42.000000 videomass-5.0.1/videomass/share/presets/version/version.txt
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.604019 videomass-5.0.1/videomass/vdms_dialogs/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/vdms_dialogs/__init__.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     2992 2023-03-31 16:50:16.000000 videomass-5.0.1/videomass/vdms_dialogs/about.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    19377 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_dialogs/audiodialogs.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5966 2023-04-03 10:27:52.000000 videomass-5.0.1/videomass/vdms_dialogs/epilogue.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     9774 2023-03-27 08:43:50.000000 videomass-5.0.1/videomass/vdms_dialogs/ffmpeg_codecs.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     9329 2023-03-27 08:47:51.000000 videomass-5.0.1/videomass/vdms_dialogs/ffmpeg_conf.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7128 2023-03-27 08:47:49.000000 videomass-5.0.1/videomass/vdms_dialogs/ffmpeg_formats.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    17894 2023-03-29 21:58:26.000000 videomass-5.0.1/videomass/vdms_dialogs/ffmpeg_help.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    21187 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_dialogs/filter_colorcorrection.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    24306 2023-04-17 21:02:09.000000 videomass-5.0.1/videomass/vdms_dialogs/filter_crop.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    23619 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_dialogs/filter_deinterlace.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12450 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_dialogs/filter_denoisers.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    22029 2023-04-03 10:30:42.000000 videomass-5.0.1/videomass/vdms_dialogs/filter_scale.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    37832 2023-04-17 21:02:09.000000 videomass-5.0.1/videomass/vdms_dialogs/filter_stab.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12093 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_dialogs/filter_transpose.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6046 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_dialogs/list_warning.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    14985 2023-03-28 18:28:35.000000 videomass-5.0.1/videomass/vdms_dialogs/mediainfo.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    47268 2023-04-17 21:02:09.000000 videomass-5.0.1/videomass/vdms_dialogs/preferences.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    14066 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_dialogs/presets_addnew.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     7279 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_dialogs/renamer.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10460 2023-01-13 14:43:59.000000 videomass-5.0.1/videomass/vdms_dialogs/set_timestamp.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     8220 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_dialogs/showlogs.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    11846 2023-03-27 08:46:43.000000 videomass-5.0.1/videomass/vdms_dialogs/shownormlist.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5371 2023-01-13 14:43:59.000000 videomass-5.0.1/videomass/vdms_dialogs/videomass_check_version.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5243 2023-03-27 08:47:46.000000 videomass-5.0.1/videomass/vdms_dialogs/while_playing.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4975 2023-03-04 13:42:00.000000 videomass-5.0.1/videomass/vdms_dialogs/widget_utils.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    25448 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_dialogs/wizard_dlg.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.608018 videomass-5.0.1/videomass/vdms_io/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/vdms_io/__init__.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4277 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_io/checkup.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6994 2023-04-11 17:55:13.000000 videomass-5.0.1/videomass/vdms_io/io_tools.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1952 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_io/make_filelog.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6445 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_io/presets_manager_prop.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.608018 videomass-5.0.1/videomass/vdms_main/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/vdms_main/__init__.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    69265 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_main/main_frame.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.608018 videomass-5.0.1/videomass/vdms_miniframes/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-11 17:55:13.000000 videomass-5.0.1/videomass/vdms_miniframes/__init__.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    23063 2023-04-11 17:55:13.000000 videomass-5.0.1/videomass/vdms_miniframes/timeline.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.608018 videomass-5.0.1/videomass/vdms_panels/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/vdms_panels/__init__.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)   112293 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_panels/av_conversions.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10282 2023-04-17 21:02:09.000000 videomass-5.0.1/videomass/vdms_panels/choose_topic.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    14156 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_panels/concatenate.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    22586 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_panels/filedrop.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10929 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_panels/hevc_avc.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6484 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_panels/libaom.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    17078 2023-04-01 22:30:31.000000 videomass-5.0.1/videomass/vdms_panels/long_processing_task.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    42445 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_panels/presets_manager.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    30076 2023-04-17 21:02:09.000000 videomass-5.0.1/videomass/vdms_panels/sequence_to_video.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    26706 2023-04-17 21:02:09.000000 videomass-5.0.1/videomass/vdms_panels/video_to_sequence.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6436 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_panels/webm.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.608018 videomass-5.0.1/videomass/vdms_sys/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/vdms_sys/__init__.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1111 2023-01-16 11:12:25.000000 videomass-5.0.1/videomass/vdms_sys/app_const.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4716 2023-03-22 11:00:27.000000 videomass-5.0.1/videomass/vdms_sys/argparser.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    24119 2023-04-01 22:30:31.000000 videomass-5.0.1/videomass/vdms_sys/configurator.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3753 2023-04-17 21:02:09.000000 videomass-5.0.1/videomass/vdms_sys/msg_info.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     8788 2023-04-13 22:32:49.000000 videomass-5.0.1/videomass/vdms_sys/settings_manager.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.612019 videomass-5.0.1/videomass/vdms_threads/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/vdms_threads/__init__.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6517 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/check_bin.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6069 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/concat_demuxer.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5379 2023-01-13 14:43:59.000000 videomass-5.0.1/videomass/vdms_threads/ffplay_file.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3229 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/ffprobe.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3754 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/generic_downloads.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     4289 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/generic_task.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6938 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/one_pass.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5997 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/picture_exporting.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13725 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/slideshow.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10173 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/two_pass.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    11175 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/two_pass_ebu.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    13996 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_threads/video_stabilization.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     5365 2023-04-11 17:55:13.000000 videomass-5.0.1/videomass/vdms_threads/volumedetect.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.612019 videomass-5.0.1/videomass/vdms_utils/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-01-13 00:08:29.000000 videomass-5.0.1/videomass/vdms_utils/__init__.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     1275 2023-01-13 14:43:59.000000 videomass-5.0.1/videomass/vdms_utils/get_bmpfromsvg.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    19274 2023-03-17 21:56:33.000000 videomass-5.0.1/videomass/vdms_utils/utils.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.612019 videomass-5.0.1/videomass/vdms_ytdlp/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        0 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/vdms_ytdlp/__init__.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    12549 2023-03-31 16:50:16.000000 videomass-5.0.1/videomass/vdms_ytdlp/formatcode.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    11029 2023-03-28 12:11:17.000000 videomass-5.0.1/videomass/vdms_ytdlp/long_task_ytdlp.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    26236 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_ytdlp/main_ytdlp.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10889 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/vdms_ytdlp/playlist_indexing.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    10171 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_ytdlp/textdrop.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     8328 2023-04-13 22:32:49.000000 videomass-5.0.1/videomass/vdms_ytdlp/ydl_downloader.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     3337 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/vdms_ytdlp/ydl_extractinfo.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6358 2023-03-21 19:07:04.000000 videomass-5.0.1/videomass/vdms_ytdlp/ydl_mediainfo.py
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    33243 2023-04-18 19:50:28.000000 videomass-5.0.1/videomass/vdms_ytdlp/youtubedl_ui.py
+drwxr-xr-x   0 jeanslack  (1000) jeanslack  (1000)        0 2023-04-18 19:51:19.556019 videomass-5.0.1/videomass.egg-info/
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)     6040 2023-04-18 19:51:19.000000 videomass-5.0.1/videomass.egg-info/PKG-INFO
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)    19568 2023-04-18 19:51:19.000000 videomass-5.0.1/videomass.egg-info/SOURCES.txt
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        1 2023-04-18 19:51:19.000000 videomass-5.0.1/videomass.egg-info/dependency_links.txt
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)       49 2023-04-18 19:51:19.000000 videomass-5.0.1/videomass.egg-info/entry_points.txt
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)        1 2023-04-18 19:51:19.000000 videomass-5.0.1/videomass.egg-info/not-zip-safe
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)      130 2023-04-18 19:51:19.000000 videomass-5.0.1/videomass.egg-info/requires.txt
+-rw-r--r--   0 jeanslack  (1000) jeanslack  (1000)       10 2023-04-18 19:51:19.000000 videomass-5.0.1/videomass.egg-info/top_level.txt
```

### Comparing `videomass-5.0.0/AUTHORS` & `videomass-5.0.1/AUTHORS`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 Author:
 Gianluca (jeanslack) Pernigotto <jeanlucperni@gmail.com>
 
 Contributors:
 @SwampRabbit (https://mxlinux.org/)
 @CComparon (https://github.com/CComparon)
+@samarthshrivas (https://github.com/samarthshrivas)
+
 
 Translators:
 - Gianluca Pernigotto <jeanlucperni@gmail.com> (Italian)
 - ChourS <chours2008@yandex.ru> (Russian)
 - Roelof Berkepeis <roelof@imoma.eu> (Dutch)
 - @johannesdedoper <https://github.com/johannesdedoper> (Dutch)
 - Samuel (Brazilian Portuguese)
```

### Comparing `videomass-5.0.0/CHANGELOG` & `videomass-5.0.1/CHANGELOG`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,28 @@
 Author: Gianluca (jeanslack) Pernigotto
 Copyright: (c) Gianluca Pernigotto 2014-2022
 License: GPL3
 
 Change Log:
 
 +------------------------------------+
+Tue, 18 April 2023 V.5.0.1
+
+  * Update ru_RU translation
+  * [YouTube Downloader] Added external downloader support #222,
+    thanks to @samarthshrivas .
+  * [A/V Conversions] Improved mouse crop area accuracy.
+  * Improved display of rejected files and URLs with a dialog that pops up when
+    files or URLs aren't imported correctly. This allows you to have a clear
+    overview of rejected files and URLs with their associated error messages,
+    see #224 .
+  * New dialog for file overwrite confirmation and missing file notification.
+  * Improved all confirmation dialogs.
+
++------------------------------------+
 Tue, 11 April 2023 V.5.0.0
 
   * [Confirm Settings] checking "Move files to trash" the "clean up files list"
     checkbox must be selected and disabled.
   * [A/V Conversions] Fix filter scrolled panel: preview/reset buttons always
     visibles on scrolling.
   * [Drag files panel] added more informations referring to a specific
```

### Comparing `videomass-5.0.0/INSTALL` & `videomass-5.0.1/INSTALL`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/LICENSE` & `videomass-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/PKG-INFO` & `videomass-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videomass
-Version: 5.0.0
+Version: 5.0.1
 Summary: Videomass is a cross-platform GUI for FFmpeg and yt-dlp
 Home-page: http://jeanslack.github.io/Videomass/
 Author: Gianluca Pernigotto
 Author-email: jeanlucperni@gmail.com
 License: GPL3 (Gnu Public License)
 Platform: All
 Classifier: Environment :: X11 Applications :: GTK
```

### Comparing `videomass-5.0.0/README.md` & `videomass-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/TODO` & `videomass-5.0.1/TODO`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/debian/changelog` & `videomass-5.0.1/debian/changelog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+videomass (5.0.1-1) UNRELEASED; urgency=medium
+
+  * Update ru_RU translation
+  * [YouTube Downloader] Added external downloader support #222,
+    thanks to @samarthshrivas .
+  * [A/V Conversions] Improved mouse crop area accuracy.
+  * Improved display of rejected files and URLs with a dialog that pops up when
+    files or URLs aren't imported correctly. This allows you to have a clear
+    overview of rejected files and URLs with their associated error messages,
+    see #224 .
+  * New dialog for file overwrite confirmation and missing file notification.
+  * Improved all confirmation dialogs.
+
+ -- Gianluca Pernigotto <jeanlucperni@gmail.com>  Tue, 18 Apr 2023 17:00:00 +0200
+
 videomass (5.0.0-1) UNRELEASED; urgency=medium
 
   * [Confirm Settings] checking "Move files to trash" the "clean up files list"
     checkbox must be selected and disabled.
   * [A/V Conversions] Fix filter scrolled panel: preview/reset buttons always
     visibles on scrolling.
   * [Drag files panel] added more informations referring to a specific
```

### Comparing `videomass-5.0.0/debian/control` & `videomass-5.0.1/debian/control`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/debian/copyright` & `videomass-5.0.1/debian/copyright`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/develop/make_pot.sh` & `videomass-5.0.1/develop/make_pot.sh`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 "../vdms_dialogs/epilogue.py" \
 "../vdms_dialogs/filter_crop.py" \
 "../vdms_dialogs/filter_deinterlace.py" \
 "../vdms_dialogs/filter_denoisers.py" \
 "../vdms_dialogs/filter_scale.py" \
 "../vdms_dialogs/filter_stab.py" \
 "../vdms_dialogs/filter_transpose.py" \
+"../vdms_dialogs/list_warning.py" \
 "../vdms_dialogs/wizard_dlg.py" \
 "../vdms_dialogs/about.py" \
 "../vdms_dialogs/presets_addnew.py" \
 "../vdms_dialogs/set_timestamp.py" \
 "../vdms_dialogs/preferences.py" \
 "../vdms_dialogs/videomass_check_version.py" \
 "../vdms_dialogs/mediainfo.py" \
```

### Comparing `videomass-5.0.0/develop/tools/AppImage_Update_Tool.sh` & `videomass-5.0.1/develop/tools/AppImage_Update_Tool.sh`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/develop/tools/AppImage_build.sh` & `videomass-5.0.1/develop/tools/AppImage_build.sh`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/develop/tools/AppRun` & `videomass-5.0.1/develop/tools/AppRun`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/develop/tools/create_ICNS.sh` & `videomass-5.0.1/develop/tools/create_ICNS.sh`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/develop/tools/generate_INNO_setup.py` & `videomass-5.0.1/develop/tools/generate_INNO_setup.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/develop/tools/inkscape2png.py` & `videomass-5.0.1/develop/tools/inkscape2png.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/develop/tools/pyinstaller_setup.py` & `videomass-5.0.1/develop/tools/pyinstaller_setup.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/develop/tools/rsvg2png.py` & `videomass-5.0.1/develop/tools/rsvg2png.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/docs/localization_guidelines.md` & `videomass-5.0.1/docs/localization_guidelines.md`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/docs/man/man1/videomass.1.gz` & `videomass-5.0.1/docs/man/man1/videomass.1.gz`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/docs/pyinstaller_setup.md` & `videomass-5.0.1/docs/pyinstaller_setup.md`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/io.github.jeanslack.videomass.appdata.xml` & `videomass-5.0.1/io.github.jeanslack.videomass.appdata.xml`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/launcher` & `videomass-5.0.1/launcher`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/setup.py` & `videomass-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/tests/test_check_bin.py` & `videomass-5.0.1/tests/test_check_bin.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/tests/test_display_GUI.py` & `videomass-5.0.1/tests/test_display_GUI.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/tests/test_ffprobe.py` & `videomass-5.0.1/tests/test_ffprobe.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/tests/test_utils.py` & `videomass-5.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/FFMPEG/NOTICE.rtf` & `videomass-5.0.1/videomass/FFMPEG/NOTICE.rtf`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/FFMPEG/README` & `videomass-5.0.1/videomass/FFMPEG/README`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_concat.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_concat.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_concat.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_concat.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_prst_mng.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_prst_mng.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_prst_mng.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_prst_mng.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_slideshow.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_slideshow.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_slideshow.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_slideshow.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_videoconversions.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_videoconversions.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_videoconversions.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_videoconversions.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_videopictures.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_videopictures.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/icon_videopictures.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/icon_videopictures.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/youtube.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/youtube.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48/youtube.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48/youtube.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_concat.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_concat.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_concat.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_concat.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_prst_mng.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_prst_mng.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_prst_mng.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_prst_mng.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_slideshow.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_slideshow.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_slideshow.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_slideshow.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_videoconversions.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_videoconversions.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_videoconversions.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_videoconversions.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_videopictures.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_videopictures.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/icon_videopictures.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/icon_videopictures.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/youtube.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/youtube.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_dark/youtube.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_dark/youtube.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_concat.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_concat.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_concat.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_concat.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_prst_mng.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_prst_mng.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_prst_mng.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_prst_mng.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_slideshow.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_slideshow.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_slideshow.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_slideshow.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_videoconversions.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_videoconversions.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_videoconversions.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_videoconversions.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_videopictures.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_videopictures.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/icon_videopictures.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/icon_videopictures.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/youtube.png` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/youtube.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/48x48_light/youtube.svg` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/48x48_light/youtube.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Sign_Icons/COPYING-ICONS.txt` & `videomass-5.0.1/videomass/art/icons/Sign_Icons/COPYING-ICONS.txt`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/addtoprst.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/addtoprst.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/audiotrack.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/audiotrack.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/coloreq.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/coloreq.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/configure.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/configure.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/configure.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/configure.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/copyprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/copyprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/deinterlace.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/deinterlace.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/delprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/delprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/denoise.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/denoise.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/denoise.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/denoise.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/edit-clear.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/editprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/editprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/newprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/newprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/playback.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/playback.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/player-volume.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/player-volume.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/player-volume.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/player-volume.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/playlist.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/playlist.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/preview.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/preview.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/preview.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/preview.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/preview_audio.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/preview_audio.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/preview_audio.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/preview_audio.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/stabilizer.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/stabilizer.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/timer.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/timer.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/timer.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/timer.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/transform-crop.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/transform-crop.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/transform-rotate.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/transform-rotate.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/transform-rotate.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/transform-rotate.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/transform-scale.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/transform-scale.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/16x16/volanalyze.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/16x16/volanalyze.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/cleanup.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/cleanup.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/cleanup.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/cleanup.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/convert.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/convert.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/convert.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/convert.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/download.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/download.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/download.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/download.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/go-next.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/go-next.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/go-next.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/go-next.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/go-previous.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/go-previous.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/go-previous.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/go-previous.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/home.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/home.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/home.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/home.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/play.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/play.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/play.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/play.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/properties.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/properties.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/properties.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/properties.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/statistics.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/statistics.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/statistics.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/statistics.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/stop.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/stop.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/24x24/stop.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/24x24/stop.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Colours/COPYING-ICONS.txt` & `videomass-5.0.1/videomass/art/icons/Videomass-Colours/COPYING-ICONS.txt`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/addtoprst.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/addtoprst.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/audiotrack.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/audiotrack.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/coloreq.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/coloreq.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/configure.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/configure.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/configure.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/configure.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/copyprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/copyprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/deinterlace.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/deinterlace.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/delprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/delprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/denoise.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/denoise.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/denoise.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/denoise.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/edit-clear.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/editprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/editprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/newprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/newprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/playback.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/playback.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/player-volume.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/player-volume.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/playlist.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/playlist.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/preview.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/preview.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/preview.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/preview.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/preview_audio.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/preview_audio.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/stabilizer.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/stabilizer.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/timer.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/timer.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/timer.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/timer.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/transform-crop.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/transform-crop.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/transform-rotate.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/transform-rotate.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/transform-scale.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/transform-scale.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/16x16/volanalyze.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/16x16/volanalyze.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/cleanup.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/cleanup.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/cleanup.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/cleanup.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/convert.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/convert.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/convert.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/convert.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/download.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/download.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/download.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/download.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/go-next.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/go-next.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/go-next.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/go-next.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/go-previous.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/go-previous.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/go-previous.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/go-previous.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/home.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/home.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/home.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/home.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/play.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/play.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/play.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/play.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/properties.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/properties.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/properties.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/properties.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/statistics.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/statistics.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/statistics.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/statistics.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/24x24/stop.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/24x24/stop.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Dark/COPYING-ICONS.txt` & `videomass-5.0.1/videomass/art/icons/Videomass-Dark/COPYING-ICONS.txt`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/addtoprst.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/addtoprst.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/audiotrack.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/audiotrack.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/coloreq.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/coloreq.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/configure.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/configure.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/configure.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/configure.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/copyprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/copyprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/deinterlace.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/deinterlace.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/delprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/delprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/denoise.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/denoise.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/denoise.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/denoise.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/edit-clear.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/editprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/editprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/newprf.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/newprf.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/playback.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/playback.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/player-volume.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/player-volume.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/playlist.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/playlist.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/preview.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/preview.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/preview.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/preview.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/preview_audio.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/preview_audio.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/stabilizer.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/stabilizer.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/timer.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/timer.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/timer.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/timer.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/transform-crop.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/transform-crop.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/transform-rotate.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/transform-rotate.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/transform-scale.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/transform-scale.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/transform-scale.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/transform-scale.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/16x16/volanalyze.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/16x16/volanalyze.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/cleanup.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/cleanup.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/cleanup.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/cleanup.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/convert.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/convert.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/convert.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/convert.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/download.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/download.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/download.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/download.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/go-next.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/go-next.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/go-next.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/go-next.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/go-previous.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/go-previous.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/go-previous.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/go-previous.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/home.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/home.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/home.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/home.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/play.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/play.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/play.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/play.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/properties.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/properties.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/properties.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/properties.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/statistics.png` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/statistics.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/statistics.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/statistics.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/24x24/stop.svg` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/24x24/stop.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/Videomass-Light/COPYING-ICONS.txt` & `videomass-5.0.1/videomass/art/icons/Videomass-Light/COPYING-ICONS.txt`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/hicolor/256x256/apps/videomass.png` & `videomass-5.0.1/videomass/art/icons/hicolor/256x256/apps/videomass.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/hicolor/48x48/apps/videomass.png` & `videomass-5.0.1/videomass/art/icons/hicolor/48x48/apps/videomass.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/hicolor/48x48/apps/videomass.xpm` & `videomass-5.0.1/videomass/art/icons/hicolor/48x48/apps/videomass.xpm`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/hicolor/COPYING-ICONS.txt` & `videomass-5.0.1/videomass/art/icons/hicolor/COPYING-ICONS.txt`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/hicolor/scalable/apps/videomass.svg` & `videomass-5.0.1/videomass/art/icons/hicolor/scalable/apps/videomass.svg`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/icons/videomass.png` & `videomass-5.0.1/videomass/art/icons/videomass.png`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/videomass.icns` & `videomass-5.0.1/videomass/art/videomass.icns`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/art/videomass.ico` & `videomass-5.0.1/videomass/art/videomass.ico`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/gui_app.py` & `videomass-5.0.1/videomass/gui_app.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/locale/README` & `videomass-5.0.1/videomass/locale/README`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/locale/en_US/LC_MESSAGES/videomass.po` & `videomass-5.0.1/videomass/locale/en_US/LC_MESSAGES/videomass.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # English translation for Videomass.
 # Copyleft -  2023 Gianluca Pernigotto
 # This file is distributed under the same license as the Videomass package
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
-"PO-Revision-Date: 2023-04-10 14:33+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
+"PO-Revision-Date: 2023-04-18 21:42+0200\n"
 "Last-Translator: \n"
 "Language-Team: English (US)\n"
 "Language: en_US\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "X-Generator: Poedit 2.4.2\n"
@@ -34,20 +34,20 @@
 #, python-brace-format
 msgid ""
 "Unexpected error while deleting file contents:\n"
 "\n"
 "{0}"
 msgstr ""
 
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr ""
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -89,71 +89,71 @@
 "imported files"
 msgstr ""
 
 #: ../vdms_dialogs/epilogue.py:100
 msgid "Confirm Settings"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 msgid "Search for a specific frame"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr ""
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr ""
 
@@ -269,16 +269,16 @@
 "This is a high precision/quality 3d denoise filter. It aims to reduce image "
 "noise, producing smooth images and making still images really still. It "
 "should enhance compressibility."
 msgstr ""
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 msgid "Read me"
 msgstr ""
 
 #: ../vdms_dialogs/filter_scale.py:80
 msgid "View result"
@@ -363,14 +363,18 @@
 msgid "Create a snapshot"
 msgstr ""
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr ""
 
+#: ../vdms_dialogs/filter_stab.py:110
+msgid "Duration seconds:"
+msgstr ""
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr ""
 
 #: ../vdms_dialogs/filter_stab.py:177
 msgid "[TRIPOD] Enable tripod mode if checked"
 msgstr ""
@@ -658,16 +662,16 @@
 #: ../vdms_dialogs/wizard_dlg.py:263
 msgid ""
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr ""
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 msgid "Videomass has a simple graphical interface for yt-dlp\n"
 msgstr ""
 
@@ -869,153 +873,179 @@
 msgid "Miscellanea"
 msgstr ""
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 msgid "Save each file in the same folder as input file"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 msgid "Auto-create subfolders when downloading playlists"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:288
+msgid "Enable/Disable yt-dlp"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 msgid "Place the toolbar"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:349
-msgid "Shows the text in the toolbar buttons"
+#: ../vdms_dialogs/preferences.py:378
+msgid "Shows text in the toolbar buttons"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 msgid "Appearance"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 msgid "Set a persistent location to save exported files"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 msgid "Choose a new destination for the files to be trashed"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 msgid "Set a persistent location to save the file downloads"
 msgstr ""
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 msgid "Get Latest Version"
 msgstr ""
 
@@ -1061,15 +1091,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr ""
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 msgid "Properties"
 msgstr ""
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
 msgid "Values"
 msgstr ""
@@ -1534,56 +1564,56 @@
 msgid "Seconds"
 msgstr ""
 
 #: ../vdms_miniframes/timeline.py:108
 msgid "Milliseconds"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 msgid "Start adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:320
+#: ../vdms_miniframes/timeline.py:322
 msgid "Source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 msgid "Start"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 msgid "End"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1596,40 +1626,43 @@
 "duration of a selected source file (see status bar messages).\n"
 "\n"
 "The \"Start\"/\"End\" duration values always refer to the initial position "
 "of the timeline: 00:00:00.000. For other informations as the segment "
 "duration and warnings, please refer to the status bar messages."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:559
+#: ../vdms_miniframes/timeline.py:566
 msgid "Timeline Editor Usage"
 msgstr ""
 
-#: ../vdms_io/checkup.py:45
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
+#: ../vdms_io/checkup.py:47
+msgid "Files already exist, do you want to overwrite them?"
 msgstr ""
 
-#: ../vdms_io/checkup.py:48
-msgid "Please Confirm"
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
 msgstr ""
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
+#: ../vdms_io/checkup.py:50
+msgid "Please Confirm"
 msgstr ""
 
 #: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
+msgstr ""
+
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr ""
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr ""
+
+#: ../vdms_io/checkup.py:75
 msgid ""
 "Output folder does not exist:\n"
 "\n"
 "\"{}\"\n"
 msgstr ""
 
 #: ../vdms_io/io_tools.py:58
@@ -1676,38 +1709,38 @@
 msgid ""
 "No presets found.\n"
 "\n"
 "Possible solution: open the Presets Manager panel, go to the presets column "
 "and try to click the \"Restore all...\" button"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 msgid ""
 "There are still processes running. if you want to stop them, use the \"Abort"
 "\" button."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:350
 msgid "Are you sure you want to exit the application?"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -1882,15 +1915,15 @@
 msgid "View"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:520
 msgid "Home panel\tCtrl+Shift+H"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 msgid "Go to the 'Home' panel"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:524
 msgid "Presets Manager\tCtrl+Shift+P"
 msgstr ""
 
@@ -1946,15 +1979,15 @@
 msgid "Keeps track of the output for debugging errors"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr ""
 
@@ -2049,172 +2082,172 @@
 msgid "Help"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:677
 msgid "Open the selected files"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 msgid "No such folder '{}'"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 msgid "Are you sure to empty trash folder?"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 msgid "No files to delete"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr ""
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 msgid "Default destination folders successfully restored"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 msgid "Changes will take effect once the program has been restarted."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, python-brace-format
 msgid "A new release is available - v.{0}\n"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 msgid "Next"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 msgid "Play the selected file in the list"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 msgid "Get informative data about imported media streams"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 msgid "Start rendering"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 msgid "Videomass - Queued Files"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 msgid "Videomass - Concatenate Demuxer"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 msgid "Videomass - From Movie to Pictures"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 msgid "Videomass - Still Image Maker"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 msgid "Videomass - FFmpeg message monitor"
 msgstr ""
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
 msgstr ""
 
@@ -2513,20 +2546,20 @@
 msgid "{} file in queue"
 msgstr ""
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr ""
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr ""
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr ""
 
 #: ../vdms_panels/av_conversions.py:2261
 msgid ""
 "Queued File\n"
@@ -2670,15 +2703,15 @@
 msgstr ""
 
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 
 #: ../vdms_panels/choose_topic.py:223
-msgid "The downloader is disabled. Check your preferences."
+msgid "yt-dlp is disabled. Check your preferences."
 msgstr ""
 
 #: ../vdms_panels/concatenate.py:78
 msgid ""
 "\n"
 "- The concatenation function is performed only with Audio files or only with "
 "Video files.\n"
@@ -2750,108 +2783,116 @@
 "File to concatenate\n"
 "Output filename\n"
 "Destination\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 msgid "Invalid path name. Contains double or single quotes"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 msgid "Directories are not allowed, just add files, please."
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 msgid "Output file name"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:207
-msgid "Duplicate files are rejected: > {}"
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:209
+msgid "Rejected Files"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 msgid "Destination folder"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 msgid "Drag the images below"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 msgid "Drag one or more video below"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 msgid "No file selected"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 msgid "File renaming..."
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 msgid "Rename the selected file to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 msgid "New Name #"
 msgstr ""
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
 msgid "[Videomass]: SUCCESS !"
 msgstr ""
@@ -3230,19 +3271,19 @@
 
 #: ../vdms_panels/presets_manager.py:833
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 msgid "Don't show this dialog again"
 msgstr ""
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 msgid ""
 "Queued File\n"
 "Pass Encoding\n"
 "Profile Used\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
@@ -3254,26 +3295,28 @@
 #: ../vdms_panels/sequence_to_video.py:74
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 
 #: ../vdms_panels/sequence_to_video.py:129
 msgid "Enable a single still image"
 msgstr ""
 
 #: ../vdms_panels/sequence_to_video.py:161
@@ -3324,14 +3367,22 @@
 msgstr ""
 
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 msgid "Unsupported format '{}'"
 msgstr ""
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+
 #: ../vdms_panels/sequence_to_video.py:719
 msgid ""
 "File to process\n"
 "Output filename\n"
 "Destination Folder\n"
 "Output Format\n"
 "Additional arguments\n"
@@ -3411,24 +3462,24 @@
 
 #: ../vdms_panels/video_to_sequence.py:49
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 
 #: ../vdms_panels/video_to_sequence.py:84
 msgid "Create thumbnails"
 msgstr ""
 
 #: ../vdms_panels/video_to_sequence.py:85
@@ -3496,15 +3547,15 @@
 "At least one \"Format Code\" must be checked for each URL selected in green."
 msgstr ""
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr ""
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr ""
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr ""
 
@@ -3579,25 +3630,25 @@
 msgid "Hide YouTube Downloader"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 msgid "Quit YouTube Downloader"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 msgid "Paste\tCtrl+V"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 msgid "Remove the selected URL from the list"
 msgstr ""
 
@@ -3613,15 +3664,15 @@
 msgid "Latest version of yt-dlp"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 msgid "Check the latest version available on github.com"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr ""
 
@@ -3719,19 +3770,27 @@
 
 #: ../vdms_ytdlp/playlist_indexing.py:256
 msgid ""
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr ""
 
-#: ../vdms_ytdlp/textdrop.py:74
-msgid "Invalid URL:"
+#: ../vdms_ytdlp/textdrop.py:68
+msgid "Invalid URL"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:84
+msgid "List of rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:87
+msgid "Rejected URLs"
 msgstr ""
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr ""
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 msgid "Statistics viewer"
 msgstr ""
```

### Comparing `videomass-5.0.0/videomass/locale/es_CU/LC_MESSAGES/videomass.mo` & `videomass-5.0.1/videomass/locale/es_CU/LC_MESSAGES/videomass.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-10 14:33+0200\n"
+"PO-Revision-Date: 2023-04-18 21:42+0200\n"
 "Last-Translator: José Alberto Valle Cid j.alberto.vc@gmail.com\n"
 "Language-Team: Spanish <>\n"
 "Language: es_CU\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -187,27 +187,14 @@
 
 msgid "All default presets have been successfully recovered"
 msgstr "Se han recuperado todos los presets con éxito"
 
 msgid "All presets have been exported successfully"
 msgstr "Todos los presets exportados con exito"
 
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
-msgstr ""
-"Ya existe: \n"
-"\n"
-"{}\n"
-"\n"
-"¿Quiere reescribirlo? "
-
 msgid "Appearance"
 msgstr "Apariencia"
 
 msgid "Application preferences"
 msgstr "Preferencias de la aplicación"
 
 msgid "Apply"
@@ -654,17 +641,14 @@
 
 msgid "Drag one or more files below"
 msgstr "Arrastre uno o más archivos abajo"
 
 msgid "Duplicate"
 msgstr "Duplicado"
 
-msgid "Duplicate files are rejected: > {}"
-msgstr "Se desechan archivos duplicados: > {}"
-
 msgid "Duration"
 msgstr "Duración"
 
 msgid "Duration:"
 msgstr "Duración:"
 
 msgid "ERROR"
@@ -1256,14 +1240,17 @@
 
 msgid "Normalization"
 msgstr "Normalización"
 
 msgid "Not everything was successful."
 msgstr "No todo fue exitoso."
 
+msgid "Not found"
+msgstr "No encontrado"
+
 msgid "Numerator"
 msgstr "Numerador"
 
 msgid "OK: Indexes to download"
 msgstr "Indices de video a descargar de la Lista"
 
 msgid "Off"
@@ -1842,17 +1829,14 @@
 
 msgid "Shows available decoders for FFmpeg"
 msgstr "Muestra los decodificadores disponible en FFmpeg"
 
 msgid "Shows available encoders for FFmpeg"
 msgstr "Muestra los codificadores disponible en FFmpeg"
 
-msgid "Shows the text in the toolbar buttons"
-msgstr "Mostrar texto en los botones de la barra de herramientas"
-
 msgid "Shows the version in use"
 msgstr "Mostrar versión en uso"
 
 msgid "Simple interlacing filter from progressive contents."
 msgstr "Filtro de entrelazado simple proveniente de contenidos progresivos."
 
 msgid "Size"
@@ -1981,17 +1965,14 @@
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "El tema de iconos solo cambia los iconos,\n"
 "fondo y primer plano de algunos campos de texto."
 
-msgid "The downloader is disabled. Check your preferences."
-msgstr "Gestor de descargas esta desactivado. Revise sus configuraciones."
-
 msgid "The file is not a frame or a video file"
 msgstr "El archivo no es un cuadro o archivo de video"
 
 msgid ""
 "The files do not have the same \"codec_types\", same \"sample_rate\" or same "
 "\"width\" or \"height\". Unable to proceed."
 msgstr ""
```

### Comparing `videomass-5.0.0/videomass/locale/es_CU/LC_MESSAGES/videomass.po` & `videomass-5.0.1/videomass/locale/es_CU/LC_MESSAGES/videomass.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Spanish translation for Videomass.
 # Copyleft -  2023 Gianluca Pernigotto
 # This file is distributed under the same license as the Videomass package
 # FIRST AUTHOR Gianluca Pernigotto <jeanlucperni@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
-"PO-Revision-Date: 2023-04-10 14:33+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
+"PO-Revision-Date: 2023-04-18 21:42+0200\n"
 "Last-Translator: José Alberto Valle Cid j.alberto.vc@gmail.com\n"
 "Language-Team: Spanish <>\n"
 "Language: es_CU\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -41,20 +41,20 @@
 "\n"
 "{0}"
 msgstr ""
 "Error inesperado al borrar contenido de archivo:\n"
 "\n"
 "{0}"
 
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr "Reiniciar"
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -116,71 +116,71 @@
 
 #: ../vdms_dialogs/epilogue.py:100
 #, fuzzy
 #| msgid "Settings"
 msgid "Confirm Settings"
 msgstr "Configuraciones"
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr "Tamaño de la fuente: {0} x {1} pixeles"
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 msgid "Search for a specific frame"
 msgstr "Buscar un cuadro especifico"
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr "Cargar"
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr "Recortar area seleccionada "
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr "Altura"
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr "Centro"
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr "Ancho"
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr "Aplicar"
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr "Filtro de Recorte"
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr "Recortar ancho"
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr "Mover verticalmente - ponga -1 para centrar en el eje vertical"
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr "Mover horizontalmente - ponga -1 para centrar en el eje horizontal"
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr "Recortar altura"
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr "Opciones Avanzadas"
 
@@ -317,16 +317,16 @@
 "hqdn3d:\n"
 "Estes es un filtro reductor de alta precisión/calidad 3d . Su objetivo es "
 "reducir el ruido de la imagen, produciendo imágenes suaves y hacer que las "
 "imágenes fijas sean realmente fijas. Debe mejorar la compresibilidad."
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 #, fuzzy
 #| msgid "Ready"
 msgid "Read me"
 msgstr "Listo"
 
@@ -423,14 +423,20 @@
 msgid "Create a snapshot"
 msgstr "Crear nuevo preset"
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr "Previsualizar"
 
+#: ../vdms_dialogs/filter_stab.py:110
+#, fuzzy
+#| msgid "Duration"
+msgid "Duration seconds:"
+msgstr "Duración"
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr "Detectar Video"
 
 #: ../vdms_dialogs/filter_stab.py:177
 msgid "[TRIPOD] Enable tripod mode if checked"
 msgstr "[TRIPOD] Al marcar se habilita el modo tripie"
@@ -789,16 +795,16 @@
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 "Se requiere \"ffmpeg\", \"ffprobe\" y \"ffplay\". Complete todas\n"
 "las cajas de texto presionando en los botones respectivos."
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr "Elija el  ejecutable de {}"
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 #, fuzzy
 #| msgid ""
 #| "Videomass has a simple graphical\n"
@@ -1020,164 +1026,192 @@
 msgid "Miscellanea"
 msgstr "Miscelánea"
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr "¿Donde prefiere guardar sus resultados?"
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 msgid "Save each file in the same folder as input file"
 msgstr "Guardar en la carpeta del archivo de entrada"
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr "Asignar un sufijo opcional a los archivos de salida:"
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 #, fuzzy
 #| msgid ""
 #| "Move source file to the Videomass trash folder after successful encoding"
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 "Después de conversión exitosa mover archivo fuente a la papelera de Videomass"
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr "¿Donde prefiere guardar sus descargas?"
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 msgid "Auto-create subfolders when downloading playlists"
 msgstr "Crear sub carpetas al descargar listas de reproducción"
 
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr "Preferencias de Archivo"
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr "Trayectoria de los ejecutables"
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr "Habilitar otra localización para FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr "Habilitar otra localización para FFprobe"
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr "Habilitar otra localización para FFplay"
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr "Otras opciones"
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr "Hilos usados para transcodificar(de 0 a 32):"
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:288
+msgid "Enable/Disable yt-dlp"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr "Temas de iconos"
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "El tema de iconos solo cambia los iconos,\n"
 "fondo y primer plano de algunos campos de texto."
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr "Personalizar barra de Herramientas"
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr "Parte superior de la ventana (predeterminado)"
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr "Parte inferior de la ventana"
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr "A la derecha de la ventana"
 
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr "A la izquierda de la ventana"
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 msgid "Place the toolbar"
 msgstr "Situar la barra de herramientas"
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr "Tamaño de icono:"
 
-#: ../vdms_dialogs/preferences.py:349
-msgid "Shows the text in the toolbar buttons"
+#: ../vdms_dialogs/preferences.py:378
+#, fuzzy
+#| msgid "Shows the text in the toolbar buttons"
+msgid "Shows text in the toolbar buttons"
 msgstr "Mostrar texto en los botones de la barra de herramientas"
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 msgid "Appearance"
 msgstr "Apariencia"
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 "Las siguientes configuraciones afectan los mensajes de salida\n"
 "y del registro durante los procesos de transcodificación.\n"
 "Cámbielas solo si sabe lo que esta haciendo.\n"
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr "Nivel de registro de FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr "Configuraciones"
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr "Asignar un sufijo adicional evita la reescritura de archivos"
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 msgid "Set a persistent location to save exported files"
 msgstr "Elija una localización permanente para guardar los archivos exportados"
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 "Teclee solo caracteres alfanuméricos. Puede utilizar el guion (\"-\") y el "
 "guion bajo (\"_\"). No se permiten espacios."
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 msgid "Choose a new destination for the files to be trashed"
 msgstr "Elija un destino para la papelera"
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 msgid "Set a persistent location to save the file downloads"
 msgstr "Elija una localización permanente para guardar las descargas"
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 msgid "Get Latest Version"
 msgstr "Obtenga la Ultima Version"
 
@@ -1234,15 +1268,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr "SELECCIÓN DE ARCHIVO"
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 #, fuzzy
 #| msgid "Audio Properties"
 msgid "Properties"
 msgstr "Propiedades de Audio"
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
@@ -1808,64 +1842,64 @@
 msgid "Seconds"
 msgstr ""
 
 #: ../vdms_miniframes/timeline.py:108
 msgid "Milliseconds"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 #, fuzzy
 #| msgid "Starts"
 msgid "Start adjustment"
 msgstr "Iniciar"
 
-#: ../vdms_miniframes/timeline.py:320
+#: ../vdms_miniframes/timeline.py:322
 #, fuzzy
 #| msgid "Duration:"
 msgid "Source duration:"
 msgstr "Duración:"
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 #, fuzzy
 #| msgid "Starts"
 msgid "Start"
 msgstr "Iniciar"
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 #, fuzzy
 #| msgid "Enabled"
 msgid "End"
 msgstr "Habilitado"
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1878,50 +1912,47 @@
 "duration of a selected source file (see status bar messages).\n"
 "\n"
 "The \"Start\"/\"End\" duration values always refer to the initial position "
 "of the timeline: 00:00:00.000. For other informations as the segment "
 "duration and warnings, please refer to the status bar messages."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:559
+#: ../vdms_miniframes/timeline.py:566
 #, fuzzy
 #| msgid "Show timeline\tCtrl+T"
 msgid "Timeline Editor Usage"
 msgstr "Mostrar linea de tiempo\tCtrl+T"
 
-#: ../vdms_io/checkup.py:45
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
+#: ../vdms_io/checkup.py:47
+#, fuzzy
+#| msgid "A file with this name already exists, do you want to overwrite it?"
+msgid "Files already exist, do you want to overwrite them?"
+msgstr "Ya existe archivo con ese nombres, ¿quiere sobreecribirlo?"
+
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
 msgstr ""
-"Ya existe: \n"
-"\n"
-"{}\n"
-"\n"
-"¿Quiere reescribirlo? "
 
-#: ../vdms_io/checkup.py:48
+#: ../vdms_io/checkup.py:50
 msgid "Please Confirm"
 msgstr "Por favor Confirme"
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
+#: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
 msgstr ""
-"Archivo no existe:\n"
-"\n"
-"\"{}\"\n"
 
-#: ../vdms_io/checkup.py:62
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr "No encontrado"
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr ""
+
+#: ../vdms_io/checkup.py:75
 msgid ""
 "Output folder does not exist:\n"
 "\n"
 "\"{}\"\n"
 msgstr ""
 "Carpeta destino no existente:\n"
 "\n"
@@ -1990,18 +2021,18 @@
 "and try to click the \"Restore all...\" button"
 msgstr ""
 "No se encontraron presets.\n"
 "\n"
 "Posible solución: abra el panel del Administrador de Presets, ir a la "
 "columna presets y presionar el botón \"Restaurar todo...\""
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr "Listo"
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 #, fuzzy
 #| msgid ""
 #| "There are still processes running.. if you want to stop them, use the "
@@ -2013,27 +2044,27 @@
 "\" button."
 msgstr ""
 "Aun hay procesos ejecutandose. si desea pararlos, use el bnotón \"Abortar"
 "\" .\n"
 "\n"
 "¿Desea terminar la aplicación?"
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr "Videomass"
 
 #: ../vdms_main/main_frame.py:350
 #, fuzzy
 #| msgid "Are you sure you want to exit?"
 msgid "Are you sure you want to exit the application?"
 msgstr "¿Seguro que desea salir?"
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr "Salir"
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -2233,15 +2264,15 @@
 
 #: ../vdms_main/main_frame.py:520
 #, fuzzy
 #| msgid "Home panel\tShift+H"
 msgid "Home panel\tCtrl+Shift+H"
 msgstr "Panel principal\tShift+H"
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 msgid "Go to the 'Home' panel"
 msgstr "Ir al panel Principal"
 
 #: ../vdms_main/main_frame.py:524
 #, fuzzy
 #| msgid "Presets Manager\tShift+P"
 msgid "Presets Manager\tCtrl+Shift+P"
@@ -2313,15 +2344,15 @@
 msgid "Keeps track of the output for debugging errors"
 msgstr "Mantener rastro de la salida para depuración de errores"
 
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr "Ir a"
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr "Fijar carpeta temporal para conversiones"
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr "Utiliza una carpeta temporal para guardar conversiones"
 
@@ -2433,189 +2464,189 @@
 msgid "Help"
 msgstr "Ayuda"
 
 #: ../vdms_main/main_frame.py:677
 msgid "Open the selected files"
 msgstr "Abrir archivo seleccionado"
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 msgid "No such folder '{}'"
 msgstr "No existe carpeta '{}'"
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 msgid "Are you sure to empty trash folder?"
 msgstr "¿Seguro que desea vaciar la papelera?"
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 msgid "No files to delete"
 msgstr "No hay archivos a borrar"
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr "Elija una carpeta de descarga"
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 "Espere....\n"
 "El archivo esta siendo descargado"
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr "Descargado exitosamente en \"{0}\""
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr "Elija un destino temporal para las conversiones"
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 msgid "Default destination folders successfully restored"
 msgstr "Carpetas destino predeterminadas restablecidas con éxito"
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 #, fuzzy
 #| msgid ""
 #| "Changes will take effect once the program has been restarted.\n"
 #| "\n"
 #| "Do you want to exit the application now?"
 msgid "Changes will take effect once the program has been restarted."
 msgstr ""
 "Los cambios tendrán efecto al reiniciar el programa.\n"
 "\n"
 "¿Quiere salir ahora?"
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr ""
 "Los cambios tendrán efecto al reiniciar el programa.\n"
 "\n"
 "¿Quiere salir ahora?"
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, python-brace-format
 msgid "A new release is available - v.{0}\n"
 msgstr "Una nueva versión esta disponible . {0}\n"
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr "¡Esta utilizando una versión de desarrollo!\n"
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr "¡Felicitaciones! Ya esta utilizando la ultima versión versión.\n"
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr "Ir al panel anterior"
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr "Regresar"
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr "Ir al proximo panel"
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 msgid "Next"
 msgstr "Siguiente"
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 msgid "Play the selected file in the list"
 msgstr "Reproducir archivo seleccionado en la lista"
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr "Reproducir"
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 #, fuzzy
 #| msgid "Gathers information of multimedia streams"
 msgid "Get informative data about imported media streams"
 msgstr "Obtiene información de flujos Multimedia"
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 #, fuzzy
 #| msgid "Starts"
 msgid "Start rendering"
 msgstr "Iniciar"
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr "Detener proceso actual"
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr "Abortar"
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr "Borrar todo de la lista"
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 msgid "Videomass - Queued Files"
 msgstr "Videomass - Archivos Pendientes"
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr "Videomass - Conversiones AV"
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr "Videomass - Administrador de Presets"
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 msgid "Videomass - Concatenate Demuxer"
 msgstr "Videomass - Encadenar Dezmezcladores"
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 msgid "Videomass - From Movie to Pictures"
 msgstr "Videomass -De Película a Imágenes"
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 msgid "Videomass - Still Image Maker"
 msgstr "Videomass -Productor de Imágenes Fijas"
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr "Ver ultimo mensaje de registro"
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr "Procesando..."
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 #, fuzzy
 #| msgid "Videomass - Output Monitor"
 msgid "Videomass - FFmpeg message monitor"
 msgstr "Videomass - Monitor de Salida"
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
@@ -2977,20 +3008,20 @@
 msgid "{} file in queue"
 msgstr "{} archivo en espera"
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr "Apagado"
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr "No fijado"
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr "inicio  {} | duración  {}"
 
 #: ../vdms_panels/av_conversions.py:2261
 msgid ""
 "Queued File\n"
@@ -3235,15 +3266,17 @@
 
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 "Extraer cuadros desde películas  a imágenes  en formatos JPG, PNG, BMP, GIF ."
 
 #: ../vdms_panels/choose_topic.py:223
-msgid "The downloader is disabled. Check your preferences."
+#, fuzzy
+#| msgid "The downloader is disabled. Check your preferences."
+msgid "yt-dlp is disabled. Check your preferences."
 msgstr "Gestor de descargas esta desactivado. Revise sus configuraciones."
 
 #: ../vdms_panels/concatenate.py:78
 #, fuzzy
 #| msgid ""
 #| "NOTE:\n"
 #| "\n"
@@ -3360,122 +3393,132 @@
 msgstr ""
 "Archivo a encadenar\n"
 "Archivo de Salda\n"
 "Destino\n"
 "Formato de Salida\n"
 "Periodo de Tiempo"
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 #, fuzzy
 #| msgid "Invalid filename. Contains double or single quotes"
 msgid "Invalid path name. Contains double or single quotes"
 msgstr "Nombre de archivo invalido, Contiene comillas dobles o sencillas"
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 msgid "Directories are not allowed, just add files, please."
 msgstr "No se permiten Carpetas, por favor solo añada archivos."
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 "Archivo sin extensión de formato: ponga una extensión apropiada al archivo, "
 "ejemplo '.mkv', '.avi','.mp3', etc."
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr "Nombre de Archivo"
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr "Duración"
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr "Tipo de Medio"
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr "Tamaño"
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 #, fuzzy
 #| msgid "Output index:"
 msgid "Output file name"
 msgstr "Indice de Salida:"
 
-#: ../vdms_panels/filedrop.py:207
-msgid "Duplicate files are rejected: > {}"
-msgstr "Se desechan archivos duplicados: > {}"
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr ""
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:209
+#, fuzzy
+#| msgid "Add Files"
+msgid "Rejected Files"
+msgstr "Añadir Archivos"
+
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr "Arrastre uno o más archivos abajo"
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 msgid "Destination folder"
 msgstr "Carpeta destino"
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag the images below"
 msgstr "Arrastre uno o más archivos abajo"
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag one or more video below"
 msgstr "Arrastre uno o más archivos abajo"
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 msgid "No file selected"
 msgstr "No se ha seleccionado archivo"
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 #, fuzzy
 #| msgid "File name"
 msgid "File renaming..."
 msgstr "Nombre de archivo"
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 #, fuzzy
 #| msgid "Open the selected files"
 msgid "Rename the selected file to:"
 msgstr "Abrir archivo seleccionado"
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr "Añadir Archivos"
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 #, fuzzy
 #| msgid "File Name"
 msgid "New Name #"
 msgstr "Nombre de Archivo"
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
@@ -3891,19 +3934,19 @@
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 "El comando del perfil seleccionado se cambio manualmente.\n"
 "¿Desea aplicarlo durante el proceso de conversión?"
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 msgid "Don't show this dialog again"
 msgstr "No mostrar nuevamente este dialogo"
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 msgid ""
 "Queued File\n"
 "Pass Encoding\n"
 "Profile Used\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
@@ -3939,26 +3982,28 @@
 #| "with a progressive digit, in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 "\n"
 "1. Importar uno o más archivos de imágenes en formato JPG, PNG y BMP , y "
 "seleccione uno.\n"
 "\n"
 "2. Usé la función Redimensionar en las imágenes que tengan altura y anchura "
 "diferentes. En otros casos es opcional.\n"
@@ -4029,14 +4074,25 @@
 msgstr "Archivo invalido: \"{}\""
 
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 msgid "Unsupported format '{}'"
 msgstr "Formato no soportado '{}'"
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+"Archivo no existe:\n"
+"\n"
+"\"{}\"\n"
+
 #: ../vdms_panels/sequence_to_video.py:719
 msgid ""
 "File to process\n"
 "Output filename\n"
 "Destination Folder\n"
 "Output Format\n"
 "Additional arguments\n"
@@ -4163,24 +4219,24 @@
 #| "with a progressive digit, \n"
 #| "in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 "\n"
 "1. Importar uno o más archivos de video , y seleccione uno.\n"
 "\n"
 "2. Usé el editor de linea de Tiempo  (CTRL+T) para fijar el intervalo de "
 "tiempo moviendo los deslizantes DURATION y SEEK.\n"
 "\n"
@@ -4276,15 +4332,15 @@
 msgstr ""
 "Al menos un \"Código de Formato\" debe seleccionarse en las URL en verde."
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr "Código de Formato"
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr "Url"
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr "Titulo"
 
@@ -4373,27 +4429,27 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 #, fuzzy
 #| msgid "YouTube Downloader"
 msgid "Quit YouTube Downloader"
 msgstr "YouTube Downloader"
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 #, fuzzy
 #| msgid "Exit\tCtrl+Q"
 msgid "Paste\tCtrl+V"
 msgstr "Salir\tCtrl+Q"
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 #, fuzzy
 #| msgid "Remove the selected files from the list"
 msgid "Remove the selected URL from the list"
@@ -4415,15 +4471,15 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 #, fuzzy
 #| msgid "Shows the latest version available on github.com"
 msgid "Check the latest version available on github.com"
 msgstr "Mostrar ultima versión disponible en github.com"
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr "Fijar carpeta temporal para descargas"
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr "Guardar todas las descargas en esta carpeta temporal"
 
@@ -4541,21 +4597,29 @@
 msgid ""
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr ""
 "ADVERTENCIA: La URL no es una lista de reproducción. Solo las lineas "
 "marcadas en verde pueden indexarse."
 
-#: ../vdms_ytdlp/textdrop.py:74
+#: ../vdms_ytdlp/textdrop.py:68
 #, fuzzy
 #| msgid "ERROR: Invalid URL: \"{}\""
-msgid "Invalid URL:"
+msgid "Invalid URL"
 msgstr "ERROR: URL invalida: \"{}\""
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:84
+msgid "List of rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:87
+msgid "Rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr ""
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 msgid "Statistics viewer"
 msgstr "Visualizado de Estadisticas"
 
@@ -4665,14 +4729,30 @@
 msgstr ""
 "Las URLs contienen listas de reproducción. ¿Seguro que desea continuar?"
 
 #: ../vdms_ytdlp/youtubedl_ui.py:659
 msgid "The URLs contain channels. Are you sure you want to continue?"
 msgstr "Las URLs contienen canales. ¿Seguro que desea continuar?"
 
+#~ msgid ""
+#~ "Already exist: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Do you want to overwrite? "
+#~ msgstr ""
+#~ "Ya existe: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "¿Quiere reescribirlo? "
+
+#~ msgid "Duplicate files are rejected: > {}"
+#~ msgstr "Se desechan archivos duplicados: > {}"
+
 #~ msgid "File list changed, please check the settings again."
 #~ msgstr "Cambio en lista de archivos, revise las configuraciones de nuevo."
 
 #~ msgid ""
 #~ "Cannot continue: The duration in the timeline exceeds the duration of "
 #~ "some queued files."
 #~ msgstr ""
@@ -4829,17 +4909,14 @@
 #~ msgid ""
 #~ "Make sure you are using the latest available version of\n"
 #~ "'{}'. This allows you to avoid download problems.\n"
 #~ msgstr ""
 #~ "Asegúrese de utilizar la ultima versión de\n"
 #~ "'{}'. Esto le evita problemas con las descargas.\n"
 
-#~ msgid "Not found"
-#~ msgstr "No encontrado"
-
 #~ msgid "Not Installed"
 #~ msgstr "No instalado"
 
 #~ msgid "Downloader"
 #~ msgstr "Gestor"
 
 #~ msgid "Topic List..."
@@ -4981,19 +5058,14 @@
 
 #, fuzzy
 #~| msgid "Duration"
 #~ msgid "Duration minutes"
 #~ msgstr "Duración"
 
 #, fuzzy
-#~| msgid "Duration"
-#~ msgid "Duration seconds"
-#~ msgstr "Duración"
-
-#, fuzzy
 #~| msgid "Starts"
 #~ msgid "Start hours"
 #~ msgstr "Iniciar"
 
 #~ msgid "Show panel for editing timeline (seek/duration)"
 #~ msgstr "Mostrar panel para editar linea de tiempo (buscar/duración)"
```

### Comparing `videomass-5.0.0/videomass/locale/es_ES/LC_MESSAGES/videomass.mo` & `videomass-5.0.1/videomass/locale/es_ES/LC_MESSAGES/videomass.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-10 14:34+0200\n"
+"PO-Revision-Date: 2023-04-18 21:43+0200\n"
 "Last-Translator: José Alberto Valle Cid j.alberto.vc@gmail.com\n"
 "Language-Team: Spanish <>\n"
 "Language: es_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -187,27 +187,14 @@
 
 msgid "All default presets have been successfully recovered"
 msgstr "Se han recuperado todos los presets con éxito"
 
 msgid "All presets have been exported successfully"
 msgstr "Todos los presets exportados con exito"
 
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
-msgstr ""
-"Ya existe: \n"
-"\n"
-"{}\n"
-"\n"
-"¿Quiere reescribirlo? "
-
 msgid "Appearance"
 msgstr "Apariencia"
 
 msgid "Application preferences"
 msgstr "Preferencias de la aplicación"
 
 msgid "Apply"
@@ -654,17 +641,14 @@
 
 msgid "Drag one or more files below"
 msgstr "Arrastre uno o más archivos abajo"
 
 msgid "Duplicate"
 msgstr "Duplicado"
 
-msgid "Duplicate files are rejected: > {}"
-msgstr "Se desechan archivos duplicados: > {}"
-
 msgid "Duration"
 msgstr "Duración"
 
 msgid "Duration:"
 msgstr "Duración:"
 
 msgid "ERROR"
@@ -1256,14 +1240,17 @@
 
 msgid "Normalization"
 msgstr "Normalización"
 
 msgid "Not everything was successful."
 msgstr "No todo fue exitoso."
 
+msgid "Not found"
+msgstr "No encontrado"
+
 msgid "Numerator"
 msgstr "Numerador"
 
 msgid "OK: Indexes to download"
 msgstr "Indices de video a descargar de la Lista"
 
 msgid "Off"
@@ -1842,17 +1829,14 @@
 
 msgid "Shows available decoders for FFmpeg"
 msgstr "Muestra los decodificadores disponible en FFmpeg"
 
 msgid "Shows available encoders for FFmpeg"
 msgstr "Muestra los codificadores disponible en FFmpeg"
 
-msgid "Shows the text in the toolbar buttons"
-msgstr "Mostrar texto en los botones de la barra de herramientas"
-
 msgid "Shows the version in use"
 msgstr "Mostrar versión en uso"
 
 msgid "Simple interlacing filter from progressive contents."
 msgstr "Filtro de entrelazado simple proveniente de contenidos progresivos."
 
 msgid "Size"
@@ -1981,17 +1965,14 @@
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "El tema de iconos solo cambia los iconos,\n"
 "fondo y primer plano de algunos campos de texto."
 
-msgid "The downloader is disabled. Check your preferences."
-msgstr "Gestor de descargas esta desactivado. Revise sus configuraciones."
-
 msgid "The file is not a frame or a video file"
 msgstr "El archivo no es un cuadro o archivo de video"
 
 msgid ""
 "The files do not have the same \"codec_types\", same \"sample_rate\" or same "
 "\"width\" or \"height\". Unable to proceed."
 msgstr ""
```

### Comparing `videomass-5.0.0/videomass/locale/es_ES/LC_MESSAGES/videomass.po` & `videomass-5.0.1/videomass/locale/es_ES/LC_MESSAGES/videomass.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Spanish translation for Videomass.
 # Copyleft -  2023 Gianluca Pernigotto
 # This file is distributed under the same license as the Videomass package
 # FIRST AUTHOR Gianluca Pernigotto <jeanlucperni@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
-"PO-Revision-Date: 2023-04-10 14:34+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
+"PO-Revision-Date: 2023-04-18 21:43+0200\n"
 "Last-Translator: José Alberto Valle Cid j.alberto.vc@gmail.com\n"
 "Language-Team: Spanish <>\n"
 "Language: es_ES\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -41,20 +41,20 @@
 "\n"
 "{0}"
 msgstr ""
 "Error inesperado al borrar contenido de archivo:\n"
 "\n"
 "{0}"
 
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr "Reiniciar"
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -116,71 +116,71 @@
 
 #: ../vdms_dialogs/epilogue.py:100
 #, fuzzy
 #| msgid "Settings"
 msgid "Confirm Settings"
 msgstr "Configuraciones"
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr "Tamaño de la fuente: {0} x {1} pixeles"
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 msgid "Search for a specific frame"
 msgstr "Buscar un cuadro especifico"
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr "Cargar"
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr "Recortar area seleccionada "
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr "Altura"
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr "Centro"
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr "Ancho"
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr "Aplicar"
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr "Filtro de Recorte"
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr "Recortar ancho"
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr "Mover verticalmente - ponga -1 para centrar en el eje vertical"
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr "Mover horizontalmente - ponga -1 para centrar en el eje horizontal"
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr "Recortar altura"
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr "Opciones Avanzadas"
 
@@ -317,16 +317,16 @@
 "hqdn3d:\n"
 "Estes es un filtro reductor de alta precisión/calidad 3d . Su objetivo es "
 "reducir el ruido de la imagen, produciendo imágenes suaves y hacer que las "
 "imágenes fijas sean realmente fijas. Debe mejorar la compresibilidad."
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 #, fuzzy
 #| msgid "Ready"
 msgid "Read me"
 msgstr "Listo"
 
@@ -423,14 +423,20 @@
 msgid "Create a snapshot"
 msgstr "Crear nuevo preset"
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr "Previsualizar"
 
+#: ../vdms_dialogs/filter_stab.py:110
+#, fuzzy
+#| msgid "Duration"
+msgid "Duration seconds:"
+msgstr "Duración"
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr "Detectar Video"
 
 #: ../vdms_dialogs/filter_stab.py:177
 msgid "[TRIPOD] Enable tripod mode if checked"
 msgstr "[TRIPOD] Al marcar se habilita el modo tripie"
@@ -789,16 +795,16 @@
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 "Se requiere \"ffmpeg\", \"ffprobe\" y \"ffplay\". Complete todas\n"
 "las cajas de texto presionando en los botones respectivos."
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr "Elija el  ejecutable de {}"
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 #, fuzzy
 #| msgid ""
 #| "Videomass has a simple graphical\n"
@@ -1020,164 +1026,192 @@
 msgid "Miscellanea"
 msgstr "Miscelánea"
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr "¿Donde prefiere guardar sus resultados?"
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 msgid "Save each file in the same folder as input file"
 msgstr "Guardar en la carpeta del archivo de entrada"
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr "Asignar un sufijo opcional a los archivos de salida:"
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 #, fuzzy
 #| msgid ""
 #| "Move source file to the Videomass trash folder after successful encoding"
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 "Después de conversión exitosa mover archivo fuente a la papelera de Videomass"
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr "¿Donde prefiere guardar sus descargas?"
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 msgid "Auto-create subfolders when downloading playlists"
 msgstr "Crear sub carpetas al descargar listas de reproducción"
 
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr "Preferencias de Archivo"
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr "Trayectoria de los ejecutables"
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr "Habilitar otra localización para FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr "Habilitar otra localización para FFprobe"
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr "Habilitar otra localización para FFplay"
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr "Otras opciones"
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr "Hilos usados para transcodificar(de 0 a 32):"
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:288
+msgid "Enable/Disable yt-dlp"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr "Temas de iconos"
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "El tema de iconos solo cambia los iconos,\n"
 "fondo y primer plano de algunos campos de texto."
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr "Personalizar barra de Herramientas"
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr "Parte superior de la ventana (predeterminado)"
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr "Parte inferior de la ventana"
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr "A la derecha de la ventana"
 
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr "A la izquierda de la ventana"
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 msgid "Place the toolbar"
 msgstr "Situar la barra de herramientas"
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr "Tamaño de icono:"
 
-#: ../vdms_dialogs/preferences.py:349
-msgid "Shows the text in the toolbar buttons"
+#: ../vdms_dialogs/preferences.py:378
+#, fuzzy
+#| msgid "Shows the text in the toolbar buttons"
+msgid "Shows text in the toolbar buttons"
 msgstr "Mostrar texto en los botones de la barra de herramientas"
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 msgid "Appearance"
 msgstr "Apariencia"
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 "Las siguientes configuraciones afectan los mensajes de salida\n"
 "y del registro durante los procesos de transcodificación.\n"
 "Cámbielas solo si sabe lo que esta haciendo.\n"
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr "Nivel de registro de FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr "Configuraciones"
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr "Asignar un sufijo adicional evita la reescritura de archivos"
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 msgid "Set a persistent location to save exported files"
 msgstr "Elija una localización permanente para guardar los archivos exportados"
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 "Teclee solo caracteres alfanuméricos. Puede utilizar el guion (\"-\") y el "
 "guion bajo (\"_\"). No se permiten espacios."
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 msgid "Choose a new destination for the files to be trashed"
 msgstr "Elija un destino para la papelera"
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 msgid "Set a persistent location to save the file downloads"
 msgstr "Elija una localización permanente para guardar las descargas"
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 msgid "Get Latest Version"
 msgstr "Obtenga la Ultima Version"
 
@@ -1234,15 +1268,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr "SELECCIÓN DE ARCHIVO"
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 #, fuzzy
 #| msgid "Audio Properties"
 msgid "Properties"
 msgstr "Propiedades de Audio"
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
@@ -1808,64 +1842,64 @@
 msgid "Seconds"
 msgstr ""
 
 #: ../vdms_miniframes/timeline.py:108
 msgid "Milliseconds"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 #, fuzzy
 #| msgid "Starts"
 msgid "Start adjustment"
 msgstr "Iniciar"
 
-#: ../vdms_miniframes/timeline.py:320
+#: ../vdms_miniframes/timeline.py:322
 #, fuzzy
 #| msgid "Duration:"
 msgid "Source duration:"
 msgstr "Duración:"
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 #, fuzzy
 #| msgid "Starts"
 msgid "Start"
 msgstr "Iniciar"
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 #, fuzzy
 #| msgid "Enabled"
 msgid "End"
 msgstr "Habilitado"
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1878,50 +1912,47 @@
 "duration of a selected source file (see status bar messages).\n"
 "\n"
 "The \"Start\"/\"End\" duration values always refer to the initial position "
 "of the timeline: 00:00:00.000. For other informations as the segment "
 "duration and warnings, please refer to the status bar messages."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:559
+#: ../vdms_miniframes/timeline.py:566
 #, fuzzy
 #| msgid "Show timeline\tCtrl+T"
 msgid "Timeline Editor Usage"
 msgstr "Mostrar linea de tiempo\tCtrl+T"
 
-#: ../vdms_io/checkup.py:45
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
+#: ../vdms_io/checkup.py:47
+#, fuzzy
+#| msgid "A file with this name already exists, do you want to overwrite it?"
+msgid "Files already exist, do you want to overwrite them?"
+msgstr "Ya existe archivo con ese nombres, ¿quiere sobreecribirlo?"
+
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
 msgstr ""
-"Ya existe: \n"
-"\n"
-"{}\n"
-"\n"
-"¿Quiere reescribirlo? "
 
-#: ../vdms_io/checkup.py:48
+#: ../vdms_io/checkup.py:50
 msgid "Please Confirm"
 msgstr "Por favor Confirme"
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
+#: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
 msgstr ""
-"Archivo no existe:\n"
-"\n"
-"\"{}\"\n"
 
-#: ../vdms_io/checkup.py:62
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr "No encontrado"
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr ""
+
+#: ../vdms_io/checkup.py:75
 msgid ""
 "Output folder does not exist:\n"
 "\n"
 "\"{}\"\n"
 msgstr ""
 "Carpeta destino no existente:\n"
 "\n"
@@ -1990,18 +2021,18 @@
 "and try to click the \"Restore all...\" button"
 msgstr ""
 "No se encontraron presets.\n"
 "\n"
 "Posible solución: abra el panel del Administrador de Presets, ir a la "
 "columna presets y presionar el botón \"Restaurar todo...\""
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr "Listo"
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 #, fuzzy
 #| msgid ""
 #| "There are still processes running.. if you want to stop them, use the "
@@ -2013,27 +2044,27 @@
 "\" button."
 msgstr ""
 "Aun hay procesos ejecutandose. si desea pararlos, use el bnotón \"Abortar"
 "\" .\n"
 "\n"
 "¿Desea terminar la aplicación?"
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr "Videomass"
 
 #: ../vdms_main/main_frame.py:350
 #, fuzzy
 #| msgid "Are you sure you want to exit?"
 msgid "Are you sure you want to exit the application?"
 msgstr "¿Seguro que desea salir?"
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr "Salir"
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -2233,15 +2264,15 @@
 
 #: ../vdms_main/main_frame.py:520
 #, fuzzy
 #| msgid "Home panel\tShift+H"
 msgid "Home panel\tCtrl+Shift+H"
 msgstr "Panel principal\tShift+H"
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 msgid "Go to the 'Home' panel"
 msgstr "Ir al panel Principal"
 
 #: ../vdms_main/main_frame.py:524
 #, fuzzy
 #| msgid "Presets Manager\tShift+P"
 msgid "Presets Manager\tCtrl+Shift+P"
@@ -2313,15 +2344,15 @@
 msgid "Keeps track of the output for debugging errors"
 msgstr "Mantener rastro de la salida para depuración de errores"
 
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr "Ir a"
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr "Fijar carpeta temporal para conversiones"
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr "Utiliza una carpeta temporal para guardar conversiones"
 
@@ -2433,189 +2464,189 @@
 msgid "Help"
 msgstr "Ayuda"
 
 #: ../vdms_main/main_frame.py:677
 msgid "Open the selected files"
 msgstr "Abrir archivo seleccionado"
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 msgid "No such folder '{}'"
 msgstr "No existe carpeta '{}'"
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 msgid "Are you sure to empty trash folder?"
 msgstr "¿Seguro que desea vaciar la papelera?"
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 msgid "No files to delete"
 msgstr "No hay archivos a borrar"
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr "Elija una carpeta de descarga"
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 "Espere....\n"
 "El archivo esta siendo descargado"
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr "Descargado exitosamente en \"{0}\""
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr "Elija un destino temporal para las conversiones"
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 msgid "Default destination folders successfully restored"
 msgstr "Carpetas destino predeterminadas restablecidas con éxito"
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 #, fuzzy
 #| msgid ""
 #| "Changes will take effect once the program has been restarted.\n"
 #| "\n"
 #| "Do you want to exit the application now?"
 msgid "Changes will take effect once the program has been restarted."
 msgstr ""
 "Los cambios tendrán efecto al reiniciar el programa.\n"
 "\n"
 "¿Quiere salir ahora?"
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr ""
 "Los cambios tendrán efecto al reiniciar el programa.\n"
 "\n"
 "¿Quiere salir ahora?"
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, python-brace-format
 msgid "A new release is available - v.{0}\n"
 msgstr "Una nueva versión esta disponible . {0}\n"
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr "¡Esta utilizando una versión de desarrollo!\n"
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr "¡Felicitaciones! Ya esta utilizando la ultima versión versión.\n"
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr "Ir al panel anterior"
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr "Regresar"
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr "Ir al proximo panel"
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 msgid "Next"
 msgstr "Siguiente"
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 msgid "Play the selected file in the list"
 msgstr "Reproducir archivo seleccionado en la lista"
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr "Reproducir"
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 #, fuzzy
 #| msgid "Gathers information of multimedia streams"
 msgid "Get informative data about imported media streams"
 msgstr "Obtiene información de flujos Multimedia"
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 #, fuzzy
 #| msgid "Starts"
 msgid "Start rendering"
 msgstr "Iniciar"
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr "Detener proceso actual"
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr "Abortar"
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr "Borrar todo de la lista"
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 msgid "Videomass - Queued Files"
 msgstr "Videomass - Archivos Pendientes"
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr "Videomass - Conversiones AV"
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr "Videomass - Administrador de Presets"
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 msgid "Videomass - Concatenate Demuxer"
 msgstr "Videomass - Encadenar Dezmezcladores"
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 msgid "Videomass - From Movie to Pictures"
 msgstr "Videomass -De Película a Imágenes"
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 msgid "Videomass - Still Image Maker"
 msgstr "Videomass -Productor de Imágenes Fijas"
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr "Ver ultimo mensaje de registro"
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr "Procesando..."
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 #, fuzzy
 #| msgid "Videomass - Output Monitor"
 msgid "Videomass - FFmpeg message monitor"
 msgstr "Videomass - Monitor de Salida"
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
@@ -2977,20 +3008,20 @@
 msgid "{} file in queue"
 msgstr "{} archivo en espera"
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr "Apagado"
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr "No fijado"
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr "inicio  {} | duración  {}"
 
 #: ../vdms_panels/av_conversions.py:2261
 msgid ""
 "Queued File\n"
@@ -3235,15 +3266,17 @@
 
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 "Extraer cuadros desde películas  a imágenes  en formatos JPG, PNG, BMP, GIF ."
 
 #: ../vdms_panels/choose_topic.py:223
-msgid "The downloader is disabled. Check your preferences."
+#, fuzzy
+#| msgid "The downloader is disabled. Check your preferences."
+msgid "yt-dlp is disabled. Check your preferences."
 msgstr "Gestor de descargas esta desactivado. Revise sus configuraciones."
 
 #: ../vdms_panels/concatenate.py:78
 #, fuzzy
 #| msgid ""
 #| "NOTE:\n"
 #| "\n"
@@ -3360,122 +3393,132 @@
 msgstr ""
 "Archivo a encadenar\n"
 "Archivo de Salda\n"
 "Destino\n"
 "Formato de Salida\n"
 "Periodo de Tiempo"
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 #, fuzzy
 #| msgid "Invalid filename. Contains double or single quotes"
 msgid "Invalid path name. Contains double or single quotes"
 msgstr "Nombre de archivo invalido, Contiene comillas dobles o sencillas"
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 msgid "Directories are not allowed, just add files, please."
 msgstr "No se permiten Carpetas, por favor solo añada archivos."
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 "Archivo sin extensión de formato: ponga una extensión apropiada al archivo, "
 "ejemplo '.mkv', '.avi','.mp3', etc."
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr "Nombre de Archivo"
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr "Duración"
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr "Tipo de Medio"
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr "Tamaño"
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 #, fuzzy
 #| msgid "Output index:"
 msgid "Output file name"
 msgstr "Indice de Salida:"
 
-#: ../vdms_panels/filedrop.py:207
-msgid "Duplicate files are rejected: > {}"
-msgstr "Se desechan archivos duplicados: > {}"
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr ""
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:209
+#, fuzzy
+#| msgid "Add Files"
+msgid "Rejected Files"
+msgstr "Añadir Archivos"
+
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr "Arrastre uno o más archivos abajo"
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 msgid "Destination folder"
 msgstr "Carpeta destino"
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag the images below"
 msgstr "Arrastre uno o más archivos abajo"
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag one or more video below"
 msgstr "Arrastre uno o más archivos abajo"
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 msgid "No file selected"
 msgstr "No se ha seleccionado archivo"
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 #, fuzzy
 #| msgid "File name"
 msgid "File renaming..."
 msgstr "Nombre de archivo"
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 #, fuzzy
 #| msgid "Open the selected files"
 msgid "Rename the selected file to:"
 msgstr "Abrir archivo seleccionado"
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr "Añadir Archivos"
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 #, fuzzy
 #| msgid "File Name"
 msgid "New Name #"
 msgstr "Nombre de Archivo"
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
@@ -3891,19 +3934,19 @@
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 "El comando del perfil seleccionado se cambio manualmente.\n"
 "¿Desea aplicarlo durante el proceso de conversión?"
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 msgid "Don't show this dialog again"
 msgstr "No mostrar nuevamente este dialogo"
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 msgid ""
 "Queued File\n"
 "Pass Encoding\n"
 "Profile Used\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
@@ -3939,26 +3982,28 @@
 #| "with a progressive digit, in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 "\n"
 "1. Importar uno o más archivos de imágenes en formato JPG, PNG y BMP , y "
 "seleccione uno.\n"
 "\n"
 "2. Usé la función Redimensionar en las imágenes que tengan altura y anchura "
 "diferentes. En otros casos es opcional.\n"
@@ -4029,14 +4074,25 @@
 msgstr "Archivo invalido: \"{}\""
 
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 msgid "Unsupported format '{}'"
 msgstr "Formato no soportado '{}'"
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+"Archivo no existe:\n"
+"\n"
+"\"{}\"\n"
+
 #: ../vdms_panels/sequence_to_video.py:719
 msgid ""
 "File to process\n"
 "Output filename\n"
 "Destination Folder\n"
 "Output Format\n"
 "Additional arguments\n"
@@ -4163,24 +4219,24 @@
 #| "with a progressive digit, \n"
 #| "in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 "\n"
 "1. Importar uno o más archivos de video , y seleccione uno.\n"
 "\n"
 "2. Usé el editor de linea de Tiempo  (CTRL+T) para fijar el intervalo de "
 "tiempo moviendo los deslizantes DURATION y SEEK.\n"
 "\n"
@@ -4276,15 +4332,15 @@
 msgstr ""
 "Al menos un \"Código de Formato\" debe seleccionarse en las URL en verde."
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr "Código de Formato"
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr "Url"
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr "Titulo"
 
@@ -4373,27 +4429,27 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 #, fuzzy
 #| msgid "YouTube Downloader"
 msgid "Quit YouTube Downloader"
 msgstr "YouTube Downloader"
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 #, fuzzy
 #| msgid "Exit\tCtrl+Q"
 msgid "Paste\tCtrl+V"
 msgstr "Salir\tCtrl+Q"
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 #, fuzzy
 #| msgid "Remove the selected files from the list"
 msgid "Remove the selected URL from the list"
@@ -4415,15 +4471,15 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 #, fuzzy
 #| msgid "Shows the latest version available on github.com"
 msgid "Check the latest version available on github.com"
 msgstr "Mostrar ultima versión disponible en github.com"
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr "Fijar carpeta temporal para descargas"
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr "Guardar todas las descargas en esta carpeta temporal"
 
@@ -4541,21 +4597,29 @@
 msgid ""
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr ""
 "ADVERTENCIA: La URL no es una lista de reproducción. Solo las lineas "
 "marcadas en verde pueden indexarse."
 
-#: ../vdms_ytdlp/textdrop.py:74
+#: ../vdms_ytdlp/textdrop.py:68
 #, fuzzy
 #| msgid "ERROR: Invalid URL: \"{}\""
-msgid "Invalid URL:"
+msgid "Invalid URL"
 msgstr "ERROR: URL invalida: \"{}\""
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:84
+msgid "List of rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:87
+msgid "Rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr ""
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 msgid "Statistics viewer"
 msgstr "Visualizado de Estadisticas"
 
@@ -4665,14 +4729,30 @@
 msgstr ""
 "Las URLs contienen listas de reproducción. ¿Seguro que desea continuar?"
 
 #: ../vdms_ytdlp/youtubedl_ui.py:659
 msgid "The URLs contain channels. Are you sure you want to continue?"
 msgstr "Las URLs contienen canales. ¿Seguro que desea continuar?"
 
+#~ msgid ""
+#~ "Already exist: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Do you want to overwrite? "
+#~ msgstr ""
+#~ "Ya existe: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "¿Quiere reescribirlo? "
+
+#~ msgid "Duplicate files are rejected: > {}"
+#~ msgstr "Se desechan archivos duplicados: > {}"
+
 #~ msgid "File list changed, please check the settings again."
 #~ msgstr "Cambio en lista de archivos, revise las configuraciones de nuevo."
 
 #~ msgid ""
 #~ "Cannot continue: The duration in the timeline exceeds the duration of "
 #~ "some queued files."
 #~ msgstr ""
@@ -4829,17 +4909,14 @@
 #~ msgid ""
 #~ "Make sure you are using the latest available version of\n"
 #~ "'{}'. This allows you to avoid download problems.\n"
 #~ msgstr ""
 #~ "Asegúrese de utilizar la ultima versión de\n"
 #~ "'{}'. Esto le evita problemas con las descargas.\n"
 
-#~ msgid "Not found"
-#~ msgstr "No encontrado"
-
 #~ msgid "Not Installed"
 #~ msgstr "No instalado"
 
 #~ msgid "Downloader"
 #~ msgstr "Gestor"
 
 #~ msgid "Topic List..."
@@ -4981,19 +5058,14 @@
 
 #, fuzzy
 #~| msgid "Duration"
 #~ msgid "Duration minutes"
 #~ msgstr "Duración"
 
 #, fuzzy
-#~| msgid "Duration"
-#~ msgid "Duration seconds"
-#~ msgstr "Duración"
-
-#, fuzzy
 #~| msgid "Starts"
 #~ msgid "Start hours"
 #~ msgstr "Iniciar"
 
 #~ msgid "Show panel for editing timeline (seek/duration)"
 #~ msgstr "Mostrar panel para editar linea de tiempo (buscar/duración)"
```

### Comparing `videomass-5.0.0/videomass/locale/es_MX/LC_MESSAGES/videomass.mo` & `videomass-5.0.1/videomass/locale/es_MX/LC_MESSAGES/videomass.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-10 14:34+0200\n"
+"PO-Revision-Date: 2023-04-18 21:43+0200\n"
 "Last-Translator: José Alberto Valle Cid j.alberto.vc@gmail.com\n"
 "Language-Team: Spanish <>\n"
 "Language: es_MX\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -187,27 +187,14 @@
 
 msgid "All default presets have been successfully recovered"
 msgstr "Se han recuperado todos los presets con éxito"
 
 msgid "All presets have been exported successfully"
 msgstr "Todos los presets exportados con exito"
 
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
-msgstr ""
-"Ya existe: \n"
-"\n"
-"{}\n"
-"\n"
-"¿Quiere reescribirlo? "
-
 msgid "Appearance"
 msgstr "Apariencia"
 
 msgid "Application preferences"
 msgstr "Preferencias de la aplicación"
 
 msgid "Apply"
@@ -654,17 +641,14 @@
 
 msgid "Drag one or more files below"
 msgstr "Arrastre uno o más archivos abajo"
 
 msgid "Duplicate"
 msgstr "Duplicado"
 
-msgid "Duplicate files are rejected: > {}"
-msgstr "Se desechan archivos duplicados: > {}"
-
 msgid "Duration"
 msgstr "Duración"
 
 msgid "Duration:"
 msgstr "Duración:"
 
 msgid "ERROR"
@@ -1256,14 +1240,17 @@
 
 msgid "Normalization"
 msgstr "Normalización"
 
 msgid "Not everything was successful."
 msgstr "No todo fue exitoso."
 
+msgid "Not found"
+msgstr "No encontrado"
+
 msgid "Numerator"
 msgstr "Numerador"
 
 msgid "OK: Indexes to download"
 msgstr "Indices de video a descargar de la Lista"
 
 msgid "Off"
@@ -1842,17 +1829,14 @@
 
 msgid "Shows available decoders for FFmpeg"
 msgstr "Muestra los decodificadores disponible en FFmpeg"
 
 msgid "Shows available encoders for FFmpeg"
 msgstr "Muestra los codificadores disponible en FFmpeg"
 
-msgid "Shows the text in the toolbar buttons"
-msgstr "Mostrar texto en los botones de la barra de herramientas"
-
 msgid "Shows the version in use"
 msgstr "Mostrar versión en uso"
 
 msgid "Simple interlacing filter from progressive contents."
 msgstr "Filtro de entrelazado simple proveniente de contenidos progresivos."
 
 msgid "Size"
@@ -1981,17 +1965,14 @@
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "El tema de iconos solo cambia los iconos,\n"
 "fondo y primer plano de algunos campos de texto."
 
-msgid "The downloader is disabled. Check your preferences."
-msgstr "Gestor de descargas esta desactivado. Revise sus configuraciones."
-
 msgid "The file is not a frame or a video file"
 msgstr "El archivo no es un cuadro o archivo de video"
 
 msgid ""
 "The files do not have the same \"codec_types\", same \"sample_rate\" or same "
 "\"width\" or \"height\". Unable to proceed."
 msgstr ""
```

### Comparing `videomass-5.0.0/videomass/locale/es_MX/LC_MESSAGES/videomass.po` & `videomass-5.0.1/videomass/locale/es_MX/LC_MESSAGES/videomass.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Spanish translation for Videomass.
 # Copyleft -  2023 Gianluca Pernigotto
 # This file is distributed under the same license as the Videomass package
 # FIRST AUTHOR Gianluca Pernigotto <jeanlucperni@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
-"PO-Revision-Date: 2023-04-10 14:34+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
+"PO-Revision-Date: 2023-04-18 21:43+0200\n"
 "Last-Translator: José Alberto Valle Cid j.alberto.vc@gmail.com\n"
 "Language-Team: Spanish <>\n"
 "Language: es_MX\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -41,20 +41,20 @@
 "\n"
 "{0}"
 msgstr ""
 "Error inesperado al borrar contenido de archivo:\n"
 "\n"
 "{0}"
 
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr "Reiniciar"
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -116,71 +116,71 @@
 
 #: ../vdms_dialogs/epilogue.py:100
 #, fuzzy
 #| msgid "Settings"
 msgid "Confirm Settings"
 msgstr "Configuraciones"
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr "Tamaño de la fuente: {0} x {1} pixeles"
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 msgid "Search for a specific frame"
 msgstr "Buscar un cuadro especifico"
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr "Cargar"
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr "Recortar area seleccionada "
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr "Altura"
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr "Centro"
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr "Ancho"
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr "Aplicar"
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr "Filtro de Recorte"
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr "Recortar ancho"
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr "Mover verticalmente - ponga -1 para centrar en el eje vertical"
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr "Mover horizontalmente - ponga -1 para centrar en el eje horizontal"
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr "Recortar altura"
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr "Opciones Avanzadas"
 
@@ -317,16 +317,16 @@
 "hqdn3d:\n"
 "Estes es un filtro reductor de alta precisión/calidad 3d . Su objetivo es "
 "reducir el ruido de la imagen, produciendo imágenes suaves y hacer que las "
 "imágenes fijas sean realmente fijas. Debe mejorar la compresibilidad."
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 #, fuzzy
 #| msgid "Ready"
 msgid "Read me"
 msgstr "Listo"
 
@@ -423,14 +423,20 @@
 msgid "Create a snapshot"
 msgstr "Crear nuevo preset"
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr "Previsualizar"
 
+#: ../vdms_dialogs/filter_stab.py:110
+#, fuzzy
+#| msgid "Duration"
+msgid "Duration seconds:"
+msgstr "Duración"
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr "Detectar Video"
 
 #: ../vdms_dialogs/filter_stab.py:177
 msgid "[TRIPOD] Enable tripod mode if checked"
 msgstr "[TRIPOD] Al marcar se habilita el modo tripie"
@@ -789,16 +795,16 @@
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 "Se requiere \"ffmpeg\", \"ffprobe\" y \"ffplay\". Complete todas\n"
 "las cajas de texto presionando en los botones respectivos."
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr "Elija el  ejecutable de {}"
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 #, fuzzy
 #| msgid ""
 #| "Videomass has a simple graphical\n"
@@ -1020,164 +1026,192 @@
 msgid "Miscellanea"
 msgstr "Miscelánea"
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr "¿Donde prefiere guardar sus resultados?"
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 msgid "Save each file in the same folder as input file"
 msgstr "Guardar en la carpeta del archivo de entrada"
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr "Asignar un sufijo opcional a los archivos de salida:"
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 #, fuzzy
 #| msgid ""
 #| "Move source file to the Videomass trash folder after successful encoding"
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 "Después de conversión exitosa mover archivo fuente a la papelera de Videomass"
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr "¿Donde prefiere guardar sus descargas?"
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 msgid "Auto-create subfolders when downloading playlists"
 msgstr "Crear sub carpetas al descargar listas de reproducción"
 
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr "Preferencias de Archivo"
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr "Trayectoria de los ejecutables"
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr "Habilitar otra localización para FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr "Habilitar otra localización para FFprobe"
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr "Habilitar otra localización para FFplay"
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr "Otras opciones"
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr "Hilos usados para transcodificar(de 0 a 32):"
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:288
+msgid "Enable/Disable yt-dlp"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr "Temas de iconos"
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "El tema de iconos solo cambia los iconos,\n"
 "fondo y primer plano de algunos campos de texto."
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr "Personalizar barra de Herramientas"
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr "Parte superior de la ventana (predeterminado)"
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr "Parte inferior de la ventana"
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr "A la derecha de la ventana"
 
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr "A la izquierda de la ventana"
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 msgid "Place the toolbar"
 msgstr "Situar la barra de herramientas"
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr "Tamaño de icono:"
 
-#: ../vdms_dialogs/preferences.py:349
-msgid "Shows the text in the toolbar buttons"
+#: ../vdms_dialogs/preferences.py:378
+#, fuzzy
+#| msgid "Shows the text in the toolbar buttons"
+msgid "Shows text in the toolbar buttons"
 msgstr "Mostrar texto en los botones de la barra de herramientas"
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 msgid "Appearance"
 msgstr "Apariencia"
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 "Las siguientes configuraciones afectan los mensajes de salida\n"
 "y del registro durante los procesos de transcodificación.\n"
 "Cámbielas solo si sabe lo que esta haciendo.\n"
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr "Nivel de registro de FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr "Configuraciones"
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr "Asignar un sufijo adicional evita la reescritura de archivos"
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 msgid "Set a persistent location to save exported files"
 msgstr "Elija una localización permanente para guardar los archivos exportados"
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 "Teclee solo caracteres alfanuméricos. Puede utilizar el guion (\"-\") y el "
 "guion bajo (\"_\"). No se permiten espacios."
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 msgid "Choose a new destination for the files to be trashed"
 msgstr "Elija un destino para la papelera"
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 msgid "Set a persistent location to save the file downloads"
 msgstr "Elija una localización permanente para guardar las descargas"
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 msgid "Get Latest Version"
 msgstr "Obtenga la Ultima Version"
 
@@ -1234,15 +1268,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr "SELECCIÓN DE ARCHIVO"
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 #, fuzzy
 #| msgid "Audio Properties"
 msgid "Properties"
 msgstr "Propiedades de Audio"
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
@@ -1808,64 +1842,64 @@
 msgid "Seconds"
 msgstr ""
 
 #: ../vdms_miniframes/timeline.py:108
 msgid "Milliseconds"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 #, fuzzy
 #| msgid "Starts"
 msgid "Start adjustment"
 msgstr "Iniciar"
 
-#: ../vdms_miniframes/timeline.py:320
+#: ../vdms_miniframes/timeline.py:322
 #, fuzzy
 #| msgid "Duration:"
 msgid "Source duration:"
 msgstr "Duración:"
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 #, fuzzy
 #| msgid "Starts"
 msgid "Start"
 msgstr "Iniciar"
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 #, fuzzy
 #| msgid "Enabled"
 msgid "End"
 msgstr "Habilitado"
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1878,50 +1912,47 @@
 "duration of a selected source file (see status bar messages).\n"
 "\n"
 "The \"Start\"/\"End\" duration values always refer to the initial position "
 "of the timeline: 00:00:00.000. For other informations as the segment "
 "duration and warnings, please refer to the status bar messages."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:559
+#: ../vdms_miniframes/timeline.py:566
 #, fuzzy
 #| msgid "Show timeline\tCtrl+T"
 msgid "Timeline Editor Usage"
 msgstr "Mostrar linea de tiempo\tCtrl+T"
 
-#: ../vdms_io/checkup.py:45
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
+#: ../vdms_io/checkup.py:47
+#, fuzzy
+#| msgid "A file with this name already exists, do you want to overwrite it?"
+msgid "Files already exist, do you want to overwrite them?"
+msgstr "Ya existe archivo con ese nombres, ¿quiere sobreecribirlo?"
+
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
 msgstr ""
-"Ya existe: \n"
-"\n"
-"{}\n"
-"\n"
-"¿Quiere reescribirlo? "
 
-#: ../vdms_io/checkup.py:48
+#: ../vdms_io/checkup.py:50
 msgid "Please Confirm"
 msgstr "Por favor Confirme"
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
+#: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
 msgstr ""
-"Archivo no existe:\n"
-"\n"
-"\"{}\"\n"
 
-#: ../vdms_io/checkup.py:62
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr "No encontrado"
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr ""
+
+#: ../vdms_io/checkup.py:75
 msgid ""
 "Output folder does not exist:\n"
 "\n"
 "\"{}\"\n"
 msgstr ""
 "Carpeta destino no existente:\n"
 "\n"
@@ -1990,18 +2021,18 @@
 "and try to click the \"Restore all...\" button"
 msgstr ""
 "No se encontraron presets.\n"
 "\n"
 "Posible solución: abra el panel del Administrador de Presets, ir a la "
 "columna presets y presionar el botón \"Restaurar todo...\""
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr "Listo"
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 #, fuzzy
 #| msgid ""
 #| "There are still processes running.. if you want to stop them, use the "
@@ -2013,27 +2044,27 @@
 "\" button."
 msgstr ""
 "Aun hay procesos ejecutandose. si desea pararlos, use el bnotón \"Abortar"
 "\" .\n"
 "\n"
 "¿Desea terminar la aplicación?"
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr "Videomass"
 
 #: ../vdms_main/main_frame.py:350
 #, fuzzy
 #| msgid "Are you sure you want to exit?"
 msgid "Are you sure you want to exit the application?"
 msgstr "¿Seguro que desea salir?"
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr "Salir"
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -2233,15 +2264,15 @@
 
 #: ../vdms_main/main_frame.py:520
 #, fuzzy
 #| msgid "Home panel\tShift+H"
 msgid "Home panel\tCtrl+Shift+H"
 msgstr "Panel principal\tShift+H"
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 msgid "Go to the 'Home' panel"
 msgstr "Ir al panel Principal"
 
 #: ../vdms_main/main_frame.py:524
 #, fuzzy
 #| msgid "Presets Manager\tShift+P"
 msgid "Presets Manager\tCtrl+Shift+P"
@@ -2313,15 +2344,15 @@
 msgid "Keeps track of the output for debugging errors"
 msgstr "Mantener rastro de la salida para depuración de errores"
 
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr "Ir a"
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr "Fijar carpeta temporal para conversiones"
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr "Utiliza una carpeta temporal para guardar conversiones"
 
@@ -2433,189 +2464,189 @@
 msgid "Help"
 msgstr "Ayuda"
 
 #: ../vdms_main/main_frame.py:677
 msgid "Open the selected files"
 msgstr "Abrir archivo seleccionado"
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 msgid "No such folder '{}'"
 msgstr "No existe carpeta '{}'"
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 msgid "Are you sure to empty trash folder?"
 msgstr "¿Seguro que desea vaciar la papelera?"
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 msgid "No files to delete"
 msgstr "No hay archivos a borrar"
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr "Elija una carpeta de descarga"
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 "Espere....\n"
 "El archivo esta siendo descargado"
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr "Descargado exitosamente en \"{0}\""
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr "Elija un destino temporal para las conversiones"
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 msgid "Default destination folders successfully restored"
 msgstr "Carpetas destino predeterminadas restablecidas con éxito"
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 #, fuzzy
 #| msgid ""
 #| "Changes will take effect once the program has been restarted.\n"
 #| "\n"
 #| "Do you want to exit the application now?"
 msgid "Changes will take effect once the program has been restarted."
 msgstr ""
 "Los cambios tendrán efecto al reiniciar el programa.\n"
 "\n"
 "¿Quiere salir ahora?"
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr ""
 "Los cambios tendrán efecto al reiniciar el programa.\n"
 "\n"
 "¿Quiere salir ahora?"
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, python-brace-format
 msgid "A new release is available - v.{0}\n"
 msgstr "Una nueva versión esta disponible . {0}\n"
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr "¡Esta utilizando una versión de desarrollo!\n"
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr "¡Felicitaciones! Ya esta utilizando la ultima versión versión.\n"
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr "Ir al panel anterior"
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr "Regresar"
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr "Ir al proximo panel"
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 msgid "Next"
 msgstr "Siguiente"
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 msgid "Play the selected file in the list"
 msgstr "Reproducir archivo seleccionado en la lista"
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr "Reproducir"
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 #, fuzzy
 #| msgid "Gathers information of multimedia streams"
 msgid "Get informative data about imported media streams"
 msgstr "Obtiene información de flujos Multimedia"
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 #, fuzzy
 #| msgid "Starts"
 msgid "Start rendering"
 msgstr "Iniciar"
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr "Detener proceso actual"
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr "Abortar"
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr "Borrar todo de la lista"
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 msgid "Videomass - Queued Files"
 msgstr "Videomass - Archivos Pendientes"
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr "Videomass - Conversiones AV"
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr "Videomass - Administrador de Presets"
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 msgid "Videomass - Concatenate Demuxer"
 msgstr "Videomass - Encadenar Dezmezcladores"
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 msgid "Videomass - From Movie to Pictures"
 msgstr "Videomass -De Película a Imágenes"
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 msgid "Videomass - Still Image Maker"
 msgstr "Videomass -Productor de Imágenes Fijas"
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr "Ver ultimo mensaje de registro"
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr "Procesando..."
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 #, fuzzy
 #| msgid "Videomass - Output Monitor"
 msgid "Videomass - FFmpeg message monitor"
 msgstr "Videomass - Monitor de Salida"
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
@@ -2977,20 +3008,20 @@
 msgid "{} file in queue"
 msgstr "{} archivo en espera"
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr "Apagado"
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr "No fijado"
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr "inicio  {} | duración  {}"
 
 #: ../vdms_panels/av_conversions.py:2261
 msgid ""
 "Queued File\n"
@@ -3235,15 +3266,17 @@
 
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 "Extraer cuadros desde películas  a imágenes  en formatos JPG, PNG, BMP, GIF ."
 
 #: ../vdms_panels/choose_topic.py:223
-msgid "The downloader is disabled. Check your preferences."
+#, fuzzy
+#| msgid "The downloader is disabled. Check your preferences."
+msgid "yt-dlp is disabled. Check your preferences."
 msgstr "Gestor de descargas esta desactivado. Revise sus configuraciones."
 
 #: ../vdms_panels/concatenate.py:78
 #, fuzzy
 #| msgid ""
 #| "NOTE:\n"
 #| "\n"
@@ -3360,122 +3393,132 @@
 msgstr ""
 "Archivo a encadenar\n"
 "Archivo de Salda\n"
 "Destino\n"
 "Formato de Salida\n"
 "Periodo de Tiempo"
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 #, fuzzy
 #| msgid "Invalid filename. Contains double or single quotes"
 msgid "Invalid path name. Contains double or single quotes"
 msgstr "Nombre de archivo invalido, Contiene comillas dobles o sencillas"
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 msgid "Directories are not allowed, just add files, please."
 msgstr "No se permiten Carpetas, por favor solo añada archivos."
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 "Archivo sin extensión de formato: ponga una extensión apropiada al archivo, "
 "ejemplo '.mkv', '.avi','.mp3', etc."
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr "Nombre de Archivo"
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr "Duración"
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr "Tipo de Medio"
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr "Tamaño"
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 #, fuzzy
 #| msgid "Output index:"
 msgid "Output file name"
 msgstr "Indice de Salida:"
 
-#: ../vdms_panels/filedrop.py:207
-msgid "Duplicate files are rejected: > {}"
-msgstr "Se desechan archivos duplicados: > {}"
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr ""
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:209
+#, fuzzy
+#| msgid "Add Files"
+msgid "Rejected Files"
+msgstr "Añadir Archivos"
+
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr "Arrastre uno o más archivos abajo"
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 msgid "Destination folder"
 msgstr "Carpeta destino"
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag the images below"
 msgstr "Arrastre uno o más archivos abajo"
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag one or more video below"
 msgstr "Arrastre uno o más archivos abajo"
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 msgid "No file selected"
 msgstr "No se ha seleccionado archivo"
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 #, fuzzy
 #| msgid "File name"
 msgid "File renaming..."
 msgstr "Nombre de archivo"
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 #, fuzzy
 #| msgid "Open the selected files"
 msgid "Rename the selected file to:"
 msgstr "Abrir archivo seleccionado"
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr "Añadir Archivos"
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 #, fuzzy
 #| msgid "File Name"
 msgid "New Name #"
 msgstr "Nombre de Archivo"
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
@@ -3891,19 +3934,19 @@
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 "El comando del perfil seleccionado se cambio manualmente.\n"
 "¿Desea aplicarlo durante el proceso de conversión?"
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 msgid "Don't show this dialog again"
 msgstr "No mostrar nuevamente este dialogo"
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 msgid ""
 "Queued File\n"
 "Pass Encoding\n"
 "Profile Used\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
@@ -3939,26 +3982,28 @@
 #| "with a progressive digit, in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 "\n"
 "1. Importar uno o más archivos de imágenes en formato JPG, PNG y BMP , y "
 "seleccione uno.\n"
 "\n"
 "2. Usé la función Redimensionar en las imágenes que tengan altura y anchura "
 "diferentes. En otros casos es opcional.\n"
@@ -4029,14 +4074,25 @@
 msgstr "Archivo invalido: \"{}\""
 
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 msgid "Unsupported format '{}'"
 msgstr "Formato no soportado '{}'"
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+"Archivo no existe:\n"
+"\n"
+"\"{}\"\n"
+
 #: ../vdms_panels/sequence_to_video.py:719
 msgid ""
 "File to process\n"
 "Output filename\n"
 "Destination Folder\n"
 "Output Format\n"
 "Additional arguments\n"
@@ -4163,24 +4219,24 @@
 #| "with a progressive digit, \n"
 #| "in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 "\n"
 "1. Importar uno o más archivos de video , y seleccione uno.\n"
 "\n"
 "2. Usé el editor de linea de Tiempo  (CTRL+T) para fijar el intervalo de "
 "tiempo moviendo los deslizantes DURATION y SEEK.\n"
 "\n"
@@ -4276,15 +4332,15 @@
 msgstr ""
 "Al menos un \"Código de Formato\" debe seleccionarse en las URL en verde."
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr "Código de Formato"
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr "Url"
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr "Titulo"
 
@@ -4373,27 +4429,27 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 #, fuzzy
 #| msgid "YouTube Downloader"
 msgid "Quit YouTube Downloader"
 msgstr "YouTube Downloader"
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 #, fuzzy
 #| msgid "Exit\tCtrl+Q"
 msgid "Paste\tCtrl+V"
 msgstr "Salir\tCtrl+Q"
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 #, fuzzy
 #| msgid "Remove the selected files from the list"
 msgid "Remove the selected URL from the list"
@@ -4415,15 +4471,15 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 #, fuzzy
 #| msgid "Shows the latest version available on github.com"
 msgid "Check the latest version available on github.com"
 msgstr "Mostrar ultima versión disponible en github.com"
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr "Fijar carpeta temporal para descargas"
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr "Guardar todas las descargas en esta carpeta temporal"
 
@@ -4541,21 +4597,29 @@
 msgid ""
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr ""
 "ADVERTENCIA: La URL no es una lista de reproducción. Solo las lineas "
 "marcadas en verde pueden indexarse."
 
-#: ../vdms_ytdlp/textdrop.py:74
+#: ../vdms_ytdlp/textdrop.py:68
 #, fuzzy
 #| msgid "ERROR: Invalid URL: \"{}\""
-msgid "Invalid URL:"
+msgid "Invalid URL"
 msgstr "ERROR: URL invalida: \"{}\""
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:84
+msgid "List of rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:87
+msgid "Rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr ""
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 msgid "Statistics viewer"
 msgstr "Visualizado de Estadisticas"
 
@@ -4665,14 +4729,30 @@
 msgstr ""
 "Las URLs contienen listas de reproducción. ¿Seguro que desea continuar?"
 
 #: ../vdms_ytdlp/youtubedl_ui.py:659
 msgid "The URLs contain channels. Are you sure you want to continue?"
 msgstr "Las URLs contienen canales. ¿Seguro que desea continuar?"
 
+#~ msgid ""
+#~ "Already exist: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Do you want to overwrite? "
+#~ msgstr ""
+#~ "Ya existe: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "¿Quiere reescribirlo? "
+
+#~ msgid "Duplicate files are rejected: > {}"
+#~ msgstr "Se desechan archivos duplicados: > {}"
+
 #~ msgid "File list changed, please check the settings again."
 #~ msgstr "Cambio en lista de archivos, revise las configuraciones de nuevo."
 
 #~ msgid ""
 #~ "Cannot continue: The duration in the timeline exceeds the duration of "
 #~ "some queued files."
 #~ msgstr ""
@@ -4829,17 +4909,14 @@
 #~ msgid ""
 #~ "Make sure you are using the latest available version of\n"
 #~ "'{}'. This allows you to avoid download problems.\n"
 #~ msgstr ""
 #~ "Asegúrese de utilizar la ultima versión de\n"
 #~ "'{}'. Esto le evita problemas con las descargas.\n"
 
-#~ msgid "Not found"
-#~ msgstr "No encontrado"
-
 #~ msgid "Not Installed"
 #~ msgstr "No instalado"
 
 #~ msgid "Downloader"
 #~ msgstr "Gestor"
 
 #~ msgid "Topic List..."
@@ -4981,19 +5058,14 @@
 
 #, fuzzy
 #~| msgid "Duration"
 #~ msgid "Duration minutes"
 #~ msgstr "Duración"
 
 #, fuzzy
-#~| msgid "Duration"
-#~ msgid "Duration seconds"
-#~ msgstr "Duración"
-
-#, fuzzy
 #~| msgid "Starts"
 #~ msgid "Start hours"
 #~ msgstr "Iniciar"
 
 #~ msgid "Show panel for editing timeline (seek/duration)"
 #~ msgstr "Mostrar panel para editar linea de tiempo (buscar/duración)"
```

### Comparing `videomass-5.0.0/videomass/locale/fr_FR/LC_MESSAGES/videomass.mo` & `videomass-5.0.1/videomass/locale/fr_FR/LC_MESSAGES/videomass.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-10 14:34+0200\n"
+"PO-Revision-Date: 2023-04-18 21:43+0200\n"
 "Last-Translator: Phil Aug <philiaug@live.fr>\n"
 "Language-Team: French (FR)\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -192,27 +192,14 @@
 
 msgid "All default presets have been successfully recovered"
 msgstr "Tous les pré-réglages par défaut ont été restaurés avec succès"
 
 msgid "All presets have been exported successfully"
 msgstr "Tous les pré-réglages ont été exportés avec succès"
 
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
-msgstr ""
-"Existe déjà: \n"
-"\n"
-"{}\n"
-"\n"
-"Voulez-vous écraser le fichier? "
-
 msgid "Appearance"
 msgstr "Apparence"
 
 msgid "Application Language"
 msgstr "Langue de l'Application"
 
 msgid "Application preferences"
@@ -677,17 +664,14 @@
 
 msgid "Drag one or more files below"
 msgstr "Faites glisser un ou plusieurs fichiers ci-dessous"
 
 msgid "Duplicate"
 msgstr "Dupliquer"
 
-msgid "Duplicate files are rejected: > {}"
-msgstr "Les fichiers en double sont refusés: > {}"
-
 msgid "Duration"
 msgstr "Durée"
 
 msgid "Duration:"
 msgstr "Durée:"
 
 msgid "ERROR"
@@ -1292,14 +1276,17 @@
 
 msgid "Normalization"
 msgstr "Normalisation"
 
 msgid "Not everything was successful."
 msgstr "Tout n'a pas réussi."
 
+msgid "Not found"
+msgstr "Introuvable"
+
 msgid "Numerator"
 msgstr "Numérateur"
 
 msgid "OK: Indexes to download"
 msgstr "OK: numéros à télécharger"
 
 msgid "Off"
@@ -1890,17 +1877,14 @@
 
 msgid "Shows available decoders for FFmpeg"
 msgstr "Aficher les décodeurs disponibles pour FFmpeg"
 
 msgid "Shows available encoders for FFmpeg"
 msgstr "Afficher les encodeurs disponibles pour FFmpeg"
 
-msgid "Shows the text in the toolbar buttons"
-msgstr "Afficher le texte avec les boutons de la barre d'outils"
-
 msgid "Shows the version in use"
 msgstr "Afficher la version actuelle"
 
 msgid "Simple interlacing filter from progressive contents."
 msgstr "Filtre simple d'entrelacement à partir d'un contenu progressif."
 
 msgid "Size"
@@ -2035,17 +2019,14 @@
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "Le thème d'icônes choisi ne modifiera que les icônes,\n"
 "quelques champs de texte d'arrière et de premier plan ."
 
-msgid "The downloader is disabled. Check your preferences."
-msgstr "L'appli de téléchargement  est désactivé. Vérifiez les préférences."
-
 msgid "The file is not a frame or a video file"
 msgstr "Le fichier n'est pas une image ou un fichier vidéo"
 
 msgid ""
 "The files do not have the same \"codec_types\", same \"sample_rate\" or same "
 "\"width\" or \"height\". Unable to proceed."
 msgstr ""
```

### Comparing `videomass-5.0.0/videomass/locale/fr_FR/LC_MESSAGES/videomass.po` & `videomass-5.0.1/videomass/locale/fr_FR/LC_MESSAGES/videomass.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # French translation for Videomass.
 # Copyleft -  2023 Gianluca Pernigotto
 # This file is distributed under the same license as the Videomass package
 # FIRST AUTHOR <philiaug@live.fr>, 2022.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
-"PO-Revision-Date: 2023-04-10 14:34+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
+"PO-Revision-Date: 2023-04-18 21:43+0200\n"
 "Last-Translator: Phil Aug <philiaug@live.fr>\n"
 "Language-Team: French (FR)\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -41,20 +41,20 @@
 "\n"
 "{0}"
 msgstr ""
 "Erreur inattendue en supprimant le contenu:\n"
 "\n"
 "{0}"
 
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr "Mise à zéro"
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -118,71 +118,71 @@
 
 #: ../vdms_dialogs/epilogue.py:100
 #, fuzzy
 #| msgid "Settings"
 msgid "Confirm Settings"
 msgstr "Réglages"
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr "Taille originale: {0} x {1} pixels"
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 msgid "Search for a specific frame"
 msgstr "Chercher une trame spécifique"
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr "Charger"
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr "Zone de recadrage "
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr "Hauteur"
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr "Centre"
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr "Largeur"
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr "Appliquer"
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr "Filtre Recadrage"
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr "Recadrer sur la largeur"
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr "Déplacement vertical - réglé sur -1 pour centrer l'axe vertical"
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr "Déplacerment horizontal- réglé sur -1 pour centrer l'axe horizontal"
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr "Recadrer sur la hauteur"
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr "Options Avancées"
 
@@ -320,16 +320,16 @@
 "Est un filtre de débruitage 3D de haute précision / qualité.Il vise à "
 "réduire le bruit de l'image, à produire des images plus lissées et à rendre  "
 "réellement les images fixes .Il  améliore  potentiellement la "
 "compressibilité."
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 #, fuzzy
 #| msgid "Ready"
 msgid "Read me"
 msgstr "Prêt"
 
@@ -425,14 +425,20 @@
 msgid "Create a snapshot"
 msgstr "Créer un nouveau pré-réglage"
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr "Aperçu"
 
+#: ../vdms_dialogs/filter_stab.py:110
+#, fuzzy
+#| msgid "Duration"
+msgid "Duration seconds:"
+msgstr "Durée"
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr "Détection Vidéo"
 
 #: ../vdms_dialogs/filter_stab.py:177
 msgid "[TRIPOD] Enable tripod mode if checked"
 msgstr "[TRÉPIED] Active le mode trépied si coché"
@@ -800,16 +806,16 @@
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 "\"ffmpeg\", \"ffprobe\" et \"ffplay\" sont requis.Ciquez sur toutes\n"
 "sur chacun de leurs boutons respectifs."
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr "Choisir l' {} l'éxécutable"
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 #, fuzzy
 #| msgid ""
 #| "Videomass has a simple graphical\n"
@@ -1034,172 +1040,200 @@
 msgid "Miscellanea"
 msgstr "Divers"
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr "Où souhaitez-vous enregistrer les fichiers transcodés ?"
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 msgid "Save each file in the same folder as input file"
 msgstr ""
 "Enregistrez les fichiers dans le même répertoire que les fichiers d'entrée"
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr "Attribuer un suffixe facultatif aux  fichiers de sortie:"
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 #, fuzzy
 #| msgid ""
 #| "Move source file to the Videomass trash folder after successful encoding"
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 "Déplacez le fichier source dans la corbeille Videomass après un encodage "
 "réussi"
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr "Où souhaitez-vous sauvegarder vos fichiers téléchargés ?"
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 msgid "Auto-create subfolders when downloading playlists"
 msgstr ""
 "Créer automatiquement des sous-dossiers lors du téléchargement de listes de "
 "lecture (playlists)"
 
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr "Préférences Fichier"
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr "Chemin vers les éxécutables"
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr "Définir un autre chemin pour utiliser FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr "Définir un autre chemin pour utiliser FFprobe"
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr "Définir un autre chemin pour utiliser FFplay"
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr "Autres options"
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr "Threads utilisés pour le transcodage (de 0 à 32):"
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:288
+msgid "Enable/Disable yt-dlp"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr "Thème d'icônes"
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "Le thème d'icônes choisi ne modifiera que les icônes,\n"
 "quelques champs de texte d'arrière et de premier plan ."
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr "Personnalisation de la barre d'outils"
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr "En haut de la fenêtre (par défaut)"
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr "En bas de la fenêtre"
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr "À droite de la fenêtre"
 
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr "À gauche de la fenêtre"
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 msgid "Place the toolbar"
 msgstr "Position de la barre d'outils"
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr "Taille d'icône:"
 
-#: ../vdms_dialogs/preferences.py:349
-msgid "Shows the text in the toolbar buttons"
+#: ../vdms_dialogs/preferences.py:378
+#, fuzzy
+#| msgid "Shows the text in the toolbar buttons"
+msgid "Shows text in the toolbar buttons"
 msgstr "Afficher le texte avec les boutons de la barre d'outils"
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 msgid "Appearance"
 msgstr "Apparence"
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 "Les paramètres suivants modifient les messages de sortie et\n"
 "les messages de log pendant le processus de transcodage.\n"
 "Ne modifier que si vous savez ce que vous faites..\n"
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr "Niveaux de journalisation FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr "Réglages"
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr ""
 "En attribuant un suffixe additionnel, vous  éviterez d'écraser vos fichiers"
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 msgid "Set a persistent location to save exported files"
 msgstr ""
 "Définir un emplacement spécifique pour enregistrer vos fichiers exportés"
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 "Nentrez que des caractères alphanumériques.Vous pouvez également utiliser le "
 "trait d'union (\"-\") et le trait de soulignement (\"_\").Les espaces ne "
 "sont pas autorisés."
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 msgid "Choose a new destination for the files to be trashed"
 msgstr ""
 "Choisissez une nouvelle destination pour que les fichiers soient supprimés"
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 msgid "Set a persistent location to save the file downloads"
 msgstr ""
 "Définit un emplacement spécifique pour enregistrer vos fichiers téléchargés"
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 msgid "Get Latest Version"
 msgstr "Télécharger la Dernière Version"
@@ -1258,15 +1292,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr "SELECTION FICHIER"
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 #, fuzzy
 #| msgid "Audio Properties"
 msgid "Properties"
 msgstr "Propriétés Audio"
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
@@ -1841,64 +1875,64 @@
 msgid "Seconds"
 msgstr ""
 
 #: ../vdms_miniframes/timeline.py:108
 msgid "Milliseconds"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 #, fuzzy
 #| msgid "Starts"
 msgid "Start adjustment"
 msgstr "Démarre"
 
-#: ../vdms_miniframes/timeline.py:320
+#: ../vdms_miniframes/timeline.py:322
 #, fuzzy
 #| msgid "Duration:"
 msgid "Source duration:"
 msgstr "Durée:"
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 #, fuzzy
 #| msgid "Starts"
 msgid "Start"
 msgstr "Démarre"
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 #, fuzzy
 #| msgid "Enabled"
 msgid "End"
 msgstr "Activé"
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1911,50 +1945,47 @@
 "duration of a selected source file (see status bar messages).\n"
 "\n"
 "The \"Start\"/\"End\" duration values always refer to the initial position "
 "of the timeline: 00:00:00.000. For other informations as the segment "
 "duration and warnings, please refer to the status bar messages."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:559
+#: ../vdms_miniframes/timeline.py:566
 #, fuzzy
 #| msgid "Show timeline\tCtrl+T"
 msgid "Timeline Editor Usage"
 msgstr "Afficher la timeline\tCtrl+T"
 
-#: ../vdms_io/checkup.py:45
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
+#: ../vdms_io/checkup.py:47
+#, fuzzy
+#| msgid "A file with this name already exists, do you want to overwrite it?"
+msgid "Files already exist, do you want to overwrite them?"
+msgstr "Un fichier avec ce nom existe déjà, voulez-vous l'écraser ?"
+
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
 msgstr ""
-"Existe déjà: \n"
-"\n"
-"{}\n"
-"\n"
-"Voulez-vous écraser le fichier? "
 
-#: ../vdms_io/checkup.py:48
+#: ../vdms_io/checkup.py:50
 msgid "Please Confirm"
 msgstr "Confirmer SVP"
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
+#: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
 msgstr ""
-"Fiichier non existant\n"
-"\n"
-"\"{}\"\n"
 
-#: ../vdms_io/checkup.py:62
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr "Introuvable"
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr ""
+
+#: ../vdms_io/checkup.py:75
 msgid ""
 "Output folder does not exist:\n"
 "\n"
 "\"{}\"\n"
 msgstr ""
 "Le dossier de sortie n'existe pas:\n"
 "\n"
@@ -2024,18 +2055,18 @@
 msgstr ""
 "Aucun pré-réglage trouvé.\n"
 "\n"
 "Solution possible: ouvrir le panneau du Gestionnaire de Pré-réglages, "
 "accédez à la colonne Pré-réglages et essayez de cliquer sur le bouton "
 "\"Restaurer tout ...\""
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr "Prêt"
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 #, fuzzy
 #| msgid ""
 #| "There are still processes running.. if you want to stop them, use the "
@@ -2047,27 +2078,27 @@
 "\" button."
 msgstr ""
 "Il y a encore des processus en cours d'exécution. Si vous voulez les "
 "arrêter, utilisez le bouton \"Annuler\".\n"
 "\n"
 "Voulez-vous tuer l'application?"
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr "Videomass"
 
 #: ../vdms_main/main_frame.py:350
 #, fuzzy
 #| msgid "Are you sure you want to exit?"
 msgid "Are you sure you want to exit the application?"
 msgstr "Voulez vous quitter ?"
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr "Quitter"
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -2273,15 +2304,15 @@
 
 #: ../vdms_main/main_frame.py:520
 #, fuzzy
 #| msgid "Home panel\tShift+H"
 msgid "Home panel\tCtrl+Shift+H"
 msgstr "Écran d'Accueil\tShift+H"
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 msgid "Go to the 'Home' panel"
 msgstr "Aller à  \"Ecran d'Accueil\""
 
 #: ../vdms_main/main_frame.py:524
 #, fuzzy
 #| msgid "Presets Manager\tShift+P"
 msgid "Presets Manager\tCtrl+Shift+P"
@@ -2353,15 +2384,15 @@
 msgid "Keeps track of the output for debugging errors"
 msgstr "Garde une trace de la sortie pour débogage d'erreurs"
 
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr "Aller à"
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr "Définir un dossier temporaire pour les conversions"
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr "Utilisez un emplacement temporaire pour enregistrer les conversions"
 
@@ -2476,182 +2507,182 @@
 msgid "Help"
 msgstr "Aide"
 
 #: ../vdms_main/main_frame.py:677
 msgid "Open the selected files"
 msgstr "Ouvrir les fichiers sélectionnés"
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 msgid "No such folder '{}'"
 msgstr "Dossier introuvable '{}'"
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 msgid "Are you sure to empty trash folder?"
 msgstr "Etes vous sûr de vouloir vider la corbeille ?"
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 msgid "No files to delete"
 msgstr "Aucun fichier à supprimer"
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr "Choisir un dossier de destination"
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 "En attente...\n"
 "L'archive est en cours de téléchargement"
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr "Téléchargé avec succès dans\"{0}\""
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr "Choisissez une destination temporaire pour les conversions"
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 msgid "Default destination folders successfully restored"
 msgstr "Les dossiers de destination par défaut ont été restaurés avec succès"
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 msgid "Changes will take effect once the program has been restarted."
 msgstr "Les modifications prendront effet une fois le programme redémarré."
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr ""
 "Les modifications prendront effet une fois le programme redémarré.\n"
 "\n"
 "Voulez-vous quitter l'application maintenant?"
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, python-brace-format
 msgid "A new release is available - v.{0}\n"
 msgstr "Une nouvelle version est disponible - v.{0}\n"
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr ""
 "Vous utilisez une version de développement qui n'a pas encore été finalisée\n"
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr "Félicitations! Vous utilisez déjà la dernière version\n"
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr "Revenir au panneau précédent"
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr "Retour"
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr "Panneau suivant"
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 msgid "Next"
 msgstr "Suivant"
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 msgid "Play the selected file in the list"
 msgstr "Lire le fichier sélectionné dans la liste"
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr "Lire"
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 #, fuzzy
 #| msgid "Gathers information of multimedia streams"
 msgid "Get informative data about imported media streams"
 msgstr "Rassemble  les informations de flux multimédias"
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 #, fuzzy
 #| msgid "Starts"
 msgid "Start rendering"
 msgstr "Démarre"
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr "Arrête le traitement en cours"
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr "Interrompre"
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr "Supprimer tous les fichiers de la liste"
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 msgid "Videomass - Queued Files"
 msgstr "Videomass - Fichiers en file d'attente"
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr "Videomass - Conversion Audio/Vidéo"
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr "Videomass - Gestion des Pré-Réglages"
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 msgid "Videomass - Concatenate Demuxer"
 msgstr "Videomass - Assemblage Fichiers Multimedia"
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 msgid "Videomass - From Movie to Pictures"
 msgstr "Videomass -  Image(s) à partir d'un film"
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 msgid "Videomass - Still Image Maker"
 msgstr "Videomass - Extraire image(s) à partir d'un film"
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr "Visualiser le dernier log"
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr "Traitement en cours..."
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 #, fuzzy
 #| msgid "Videomass - Output Monitor"
 msgid "Videomass - FFmpeg message monitor"
 msgstr "Videomass - Moniteur de sortie"
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
@@ -3019,20 +3050,20 @@
 msgid "{} file in queue"
 msgstr "{} filchier en file d'attente"
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr "Off"
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr "Désactivé"
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr "début  {} | durée  {}"
 
 #: ../vdms_panels/av_conversions.py:2261
 msgid ""
 "Queued File\n"
@@ -3277,15 +3308,17 @@
 
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 "Extraire des images de vos films aux formats JPG, PNG, BMP et GIF animé."
 
 #: ../vdms_panels/choose_topic.py:223
-msgid "The downloader is disabled. Check your preferences."
+#, fuzzy
+#| msgid "The downloader is disabled. Check your preferences."
+msgid "yt-dlp is disabled. Check your preferences."
 msgstr "L'appli de téléchargement  est désactivé. Vérifiez les préférences."
 
 #: ../vdms_panels/concatenate.py:78
 #, fuzzy
 #| msgid ""
 #| "NOTE:\n"
 #| "\n"
@@ -3408,123 +3441,133 @@
 msgstr ""
 "Filchier à assembler\n"
 "Nom de sortie du fichier\n"
 "Destination\n"
 "Format de sortie\n"
 "Durée"
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 #, fuzzy
 #| msgid "Invalid filename. Contains double or single quotes"
 msgid "Invalid path name. Contains double or single quotes"
 msgstr "Nom de fichier non valide.Contient des apostrophes doubles ou simples"
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 msgid "Directories are not allowed, just add files, please."
 msgstr ""
 "Les répertoires ne sont pas autorisés, ajouter uniquement des fichiers svp."
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 "Fichier sans extension veuillez donner une extension appropriée au nom du "
 "fichier, exemple '.mkv', '.avi', '.mp3', etc."
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr "Nom du fichier"
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr "Durée"
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr "Type de média"
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr "Taille"
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 #, fuzzy
 #| msgid "Restrict file names"
 msgid "Output file name"
 msgstr "Réduire les noms de fichiers"
 
-#: ../vdms_panels/filedrop.py:207
-msgid "Duplicate files are rejected: > {}"
-msgstr "Les fichiers en double sont refusés: > {}"
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr ""
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:209
+#, fuzzy
+#| msgid "Add Files"
+msgid "Rejected Files"
+msgstr "Ajouter des Fichiers"
+
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr "Faites glisser un ou plusieurs fichiers ci-dessous"
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 msgid "Destination folder"
 msgstr "Dossier de destination"
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag the images below"
 msgstr "Faites glisser un ou plusieurs fichiers ci-dessous"
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag one or more video below"
 msgstr "Faites glisser un ou plusieurs fichiers ci-dessous"
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 msgid "No file selected"
 msgstr "Aucun fichier sélectionné"
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 #, fuzzy
 #| msgid "File name"
 msgid "File renaming..."
 msgstr "Nom du fichier"
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 #, fuzzy
 #| msgid "Open the selected files"
 msgid "Rename the selected file to:"
 msgstr "Ouvrir les fichiers sélectionnés"
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr "Ajouter des Fichiers"
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 #, fuzzy
 #| msgid "File Name"
 msgid "New Name #"
 msgstr "Nom du fichier"
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
@@ -3947,19 +3990,19 @@
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 "La commande de profil sélectionnée a été modifiée manuellement..\n"
 "Voulez-vous l'appliquer pendant le processus de conversion?"
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 msgid "Don't show this dialog again"
 msgstr "Ne plus afficher cette boîte de dialogue"
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 msgid ""
 "Queued File\n"
 "Pass Encoding\n"
 "Profile Used\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
@@ -3996,26 +4039,28 @@
 #| "with a progressive digit, in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 "\n"
 "1. Importez un ou plusieurs fichiers d'image tels que les formats JPG, PNG "
 "et BMP, puis en sélectionnez un..\n"
 "\n"
 "2. Utilisez la fonction de Redimensionnement pour redimensionner des images "
 "qui ont différentes tailles telles que la largeur et la hauteur.Cette option "
@@ -4087,14 +4132,25 @@
 msgstr "Fichier non valide '{}'"
 
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 msgid "Unsupported format '{}'"
 msgstr "Format non supporté '{}'"
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+"Fiichier non existant\n"
+"\n"
+"\"{}\"\n"
+
 #: ../vdms_panels/sequence_to_video.py:719
 msgid ""
 "File to process\n"
 "Output filename\n"
 "Destination Folder\n"
 "Output Format\n"
 "Additional arguments\n"
@@ -4223,24 +4279,24 @@
 #| "with a progressive digit, \n"
 #| "in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 "\n"
 "1. Importez un ou plusieurs fichiers vidéo, puis en sélectionnez un.\n"
 "\n"
 "2. Pour sélectionner une portion de temps, utilisez l'éditeur de Timeline "
 "(CTRL + T) en faisant défiler la DUREE et les curseurs de RECHERCHE.\n"
 "\n"
@@ -4337,15 +4393,15 @@
 "Au moins un \"code format\" doit être sélectionné pour chaque URL "
 "sélectionnée en vert."
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr "Code de format"
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr "Url"
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr "Titre"
 
@@ -4434,27 +4490,27 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 #, fuzzy
 #| msgid "YouTube Downloader"
 msgid "Quit YouTube Downloader"
 msgstr "Télécharger sur YouTube"
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 #, fuzzy
 #| msgid "Exit\tCtrl+Q"
 msgid "Paste\tCtrl+V"
 msgstr "Quitter\tCtrl+Q"
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 #, fuzzy
 #| msgid "Remove the selected files from the list"
 msgid "Remove the selected URL from the list"
@@ -4476,15 +4532,15 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 #, fuzzy
 #| msgid "Shows the latest version available on github.com"
 msgid "Check the latest version available on github.com"
 msgstr "Affiche la dernière version disponible sur github.com"
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr "Définir un dossier temporaire pour les téléchargements"
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr "Enregistrer tous les téléchargements dans cet emplacement temporaire"
 
@@ -4605,21 +4661,29 @@
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr ""
 "AVERTISSEMENT: L'URL sélectionnée ne fait pas référence à une liste de "
 "lecture (playlist).Seules les lignes de couleur verte peuvent être "
 "numérotées."
 
-#: ../vdms_ytdlp/textdrop.py:74
+#: ../vdms_ytdlp/textdrop.py:68
 #, fuzzy
 #| msgid "ERROR: Invalid URL: \"{}\""
-msgid "Invalid URL:"
+msgid "Invalid URL"
 msgstr "ERREUR:  URL: invalide \"{}\""
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:84
+msgid "List of rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:87
+msgid "Rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr ""
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 msgid "Statistics viewer"
 msgstr "Visionner les statistiques"
 
@@ -4730,14 +4794,30 @@
 "Les URL contiennent des listes de lecture.Êtes-vous  sûr de vouloir "
 "continuer?"
 
 #: ../vdms_ytdlp/youtubedl_ui.py:659
 msgid "The URLs contain channels. Are you sure you want to continue?"
 msgstr "Les URL contiennent des canaux.Êtes vous sûr de vouloir continuer?"
 
+#~ msgid ""
+#~ "Already exist: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Do you want to overwrite? "
+#~ msgstr ""
+#~ "Existe déjà: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Voulez-vous écraser le fichier? "
+
+#~ msgid "Duplicate files are rejected: > {}"
+#~ msgstr "Les fichiers en double sont refusés: > {}"
+
 #~ msgid "File list changed, please check the settings again."
 #~ msgstr ""
 #~ "La liste des fichiers a été modifiée, veuillez revérifier les paramètres."
 
 #~ msgid ""
 #~ "Cannot continue: The duration in the timeline exceeds the duration of "
 #~ "some queued files."
@@ -4897,17 +4977,14 @@
 #~ msgid ""
 #~ "Make sure you are using the latest available version of\n"
 #~ "'{}'. This allows you to avoid download problems.\n"
 #~ msgstr ""
 #~ "Assurez-vous d'utiliser la dernière version disponible de\n"
 #~ "'{}'.Cela vous  évitera des problèmes de téléchargement.\n"
 
-#~ msgid "Not found"
-#~ msgstr "Introuvable"
-
 #~ msgid "Not Installed"
 #~ msgstr "Non installé"
 
 #~ msgid "Downloader"
 #~ msgstr "Télécharger"
 
 #~ msgid "Topic List..."
@@ -5053,19 +5130,14 @@
 
 #, fuzzy
 #~| msgid "Duration"
 #~ msgid "Duration minutes"
 #~ msgstr "Durée"
 
 #, fuzzy
-#~| msgid "Duration"
-#~ msgid "Duration seconds"
-#~ msgstr "Durée"
-
-#, fuzzy
 #~| msgid "Starts"
 #~ msgid "Start hours"
 #~ msgstr "Démarre"
 
 #~ msgid "Show panel for editing timeline (seek/duration)"
 #~ msgstr "Afficher le panneau pour éditer la timeline (recherche / durée)"
```

### Comparing `videomass-5.0.0/videomass/locale/it_IT/LC_MESSAGES/videomass.mo` & `videomass-5.0.1/videomass/locale/it_IT/LC_MESSAGES/videomass.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-10 14:33+0200\n"
+"PO-Revision-Date: 2023-04-18 21:42+0200\n"
 "Last-Translator: Gianluca (jeanslack) Pernigotto <jeanlucperni@gmail.com>\n"
 "Language-Team: Italian <>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
@@ -90,77 +90,81 @@
 
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 "\n"
 "1. Importa uno o più file immagine nei formati JPG, PNG e BMP, quindi "
 "selezionane uno.\n"
 "\n"
 "2. Utilizzare la funzione Ridimensionamento per ridimensionare le immagini "
-"che hanno dimensioni diverse come larghezza e\n"
-"altezza. Negli altri casi è opzionale.\n"
+"che hanno \n"
+"dimensioni diverse come larghezza e altezza. Negli altri casi è opzionale.\n"
 "\n"
 "3. Per impostare la DURATA tra le immagini usa l'editor Timeline (CTRL+T) e "
-"regolare solo il valore \"Fine\",\n"
-"lasciando il valore \"Inizio\" a 00:00:00.000.\n"
+"regolare solo il\n"
+"valore \"Fine\", lasciando il valore \"Inizio\" a 00:00:00.000.\n"
 "\n"
 "4. Avvia la conversione.\n"
 "\n"
 "\n"
 "Il video prodotto avrà il nome del file selezionato nell'elenco 'File in "
-"coda', il quale verrà salvato in una cartella denominata 'Still_Images'\n"
-"con l'aggiunta di una cifra progressiva, nel percorso da te specificato."
+"coda', il quale verrà salvato\n"
+"in una cartella denominata 'Still_Images' con l'aggiunta di una cifra "
+"progressiva, nel percorso\n"
+"da te specificato."
 
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 "\n"
 "1. Importa uno o più file video, quindi selezionane uno.\n"
 "\n"
 "2. Per selezionare un intervallo di tempo utilizzare l'editor Timeline "
-"(CTRL+T), e regolare i valori di durata\n"
-"di \"Inizio\" e \"Fine\" come desiderato.\n"
+"(CTRL+T), e \n"
+"regolare i valori di durata di \"Inizio\" e \"Fine\" come desiderato.\n"
 "\n"
 "3. Selezionare un formato di output (jpg, png, bmp o gif).\n"
 "\n"
 "4. Avvia la conversione.\n"
 "\n"
 "\n"
 "Le immagini prodotte verranno salvate in una cartella denominata "
-"'Movie_to_Pictures' con l'aggiunta \n"
-"di una cifra progressiva, nel percorso da te specificato."
+"'Movie_to_Pictures'\n"
+"con l'aggiunta  di una cifra progressiva, nel percorso da te specificato."
 
 msgid " Do you want to enable this feature?"
 msgstr " Vuoi abilitare questa funzione?"
 
 msgid ""
 "\"Auto\" keeps all audio stream but processes only the one of the selected "
 "index; \"All\" keeps all audio streams and processes them all with the "
@@ -392,26 +396,16 @@
 
 msgid "All default presets have been successfully recovered"
 msgstr "Tutti i preset predefiniti sono stati ripristinati con successo"
 
 msgid "All presets have been exported successfully"
 msgstr "Tutti i preset sono stati esportati correttamente"
 
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
-msgstr ""
-"File già esistenti: \n"
-"\n"
-"{}\n"
-"\n"
-"Vuoi sovrascrivere? "
+msgid "Already exist"
+msgstr "Già esistente"
 
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 "Spostare sempre i file di origine sul cestino di\n"
 "Videomass dopo una corretta codifica"
@@ -1026,16 +1020,16 @@
 "page"
 msgstr ""
 "Scarica l'intera collezione degli ultimi preset disponibili dalla home page"
 
 msgid "Download videos by resolution"
 msgstr "Scarica video in base alla risoluzione"
 
-msgid "Download videos from YouTube.com and other video sites "
-msgstr "Scarica video da YouTube.com e altri siti di video "
+msgid "Download videos from YouTube.com and other video sites"
+msgstr "Scarica video da YouTube.com e altri siti di video"
 
 msgid "Downloads folder\tCtrl+D"
 msgstr "Cartella dei download\tCtrl+D"
 
 msgid "Drag one or more files below"
 msgstr "Trascina uno o più file qui sotto"
 
@@ -1047,20 +1041,23 @@
 
 msgid "Drag the images below"
 msgstr "Trascina le immagini qui sotto"
 
 msgid "Duplicate"
 msgstr "Duplica"
 
-msgid "Duplicate files are rejected: > {}"
-msgstr "I files duplicati sono rifiutati: > {}"
+msgid "Duplicate file, it has already been added to the list."
+msgstr "File duplicato, è già stato aggiunto all'elenco."
 
 msgid "Duration"
 msgstr "Durata"
 
+msgid "Duration seconds:"
+msgstr "Durata in secondi:"
+
 msgid "Duration:"
 msgstr "Durata:"
 
 msgid "ERROR"
 msgstr "ERRORE"
 
 msgid "ERROR: Invalid option"
@@ -1144,14 +1141,17 @@
 "Enable virtual tripod mode if checked, which is equivalent to relative=0:"
 "smoothing=0. Default is unchecked. Use also tripod option of vidstabdetect."
 msgstr ""
 "Abilita la modalità treppiede virtuale se selezionata, che è equivalente a "
 "relative=abilitato: smoothing=0. Per impostazione predefinita è "
 "disabilitato. Usa anche l'opzione treppiede di vidstabdetect."
 
+msgid "Enable/Disable yt-dlp"
+msgstr "Abilita/Disabilita yt-dlp"
+
 msgid "Enabled"
 msgstr "Abilitato"
 
 msgid "Encoders"
 msgstr "Codificatori"
 
 msgid "End"
@@ -1193,14 +1193,23 @@
 
 msgid "Export selected preset as copy"
 msgstr "Esporta il preset selezionato come copia"
 
 msgid "Extension"
 msgstr "Estensione"
 
+msgid "External Downloader Preferences"
+msgstr "Preferenze del downloader esterno"
+
+msgid "External downloader arguments"
+msgstr "Argomenti del downloader esterno"
+
+msgid "External downloader executable path"
+msgstr "Percorso eseguibile del downloader esterno"
+
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 "Estrai immagini (frame) dai tuoi filmati nei formati JPG, PNG, BMP, GIF."
 
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
@@ -1316,14 +1325,17 @@
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 "File senza estensione di formato: fornire un'estensione appropriata al nome "
 "del file, ad esempio '.mkv', '.avi', '.mp3', ecc."
 
+msgid "Files already exist, do you want to overwrite them?"
+msgstr "File già esistenti, vuoi sovrascriverli?"
+
 msgid "Find FFmpeg topics and options"
 msgstr "Trova argomenti e opzioni di FFmpeg"
 
 msgid "Finish"
 msgstr "Fine"
 
 msgid "First pass of the selected profile"
@@ -1492,18 +1504,18 @@
 "If you want to keep the aspect ratio, select \"Constrain proportions\" below "
 "and\n"
 "specify only one dimension, either width or height, and set the other "
 "dimension\n"
 "to -1 or -2 (some codecs require -2, so you should do some testing first)."
 msgstr ""
 "Se desideri mantenere le proporzioni, seleziona \"Vincola proporzioni\" di "
-"seguito \n"
+"seguito\n"
 "e specifica solo una dimensione, larghezza o altezza, e imposta l'altra "
-"dimensione \n"
-"su -1 o -2 (alcuni codec richiedono -2, quindi dovresti prima fare qualche "
+"dimensione\n"
+"a -1 o -2 (alcuni codec richiedono -2, quindi prima dovresti fare qualche "
 "test)."
 
 msgid ""
 "If you want to use a version of FFmpeg located on your\n"
 "filesystem but not installed on your operating system,\n"
 "click the \"Locate\" button."
 msgstr ""
@@ -1539,14 +1551,29 @@
 
 msgid "Import group"
 msgstr "Importa gruppo"
 
 msgid "Import preset"
 msgstr "Importa preset"
 
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+"Oltre a quello predefinito (nativo), yt-dlp attualmente\n"
+"supporta i seguenti downloader esterni:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Tieni presente che se abiliti un downloader esterno, non\n"
+"sarai in grado di visualizzare la barra di avanzamento durante\n"
+"le operazioni di download."
+
 msgid "Include audio file"
 msgstr "Includi file audio"
 
 msgid ""
 "Include the video ID\n"
 "in the file names"
 msgstr ""
@@ -1574,16 +1601,16 @@
 
 msgid "Interlaces with interlace filter"
 msgstr "Interlaccia con il filtro interlace"
 
 msgid "Interrupted Process !"
 msgstr "Processo Interrotto !"
 
-msgid "Invalid URL:"
-msgstr "URL non valido:"
+msgid "Invalid URL"
+msgstr "URL non valido"
 
 msgid "Invalid file: '{}'"
 msgstr "File non valido: '{}'"
 
 msgid ""
 "Invalid file: '{}'\n"
 "\n"
@@ -1654,14 +1681,17 @@
 
 msgid "List basic options"
 msgstr "Elenca le opzioni basilari"
 
 msgid "List more options"
 msgstr "Elenca più opzioni"
 
+msgid "List of rejected URLs"
+msgstr "Lista degli URL rifiutati"
+
 msgid "List sinks of the output device"
 msgstr "Elenca i sink del dispositivo di output"
 
 msgid "List sources of the input device"
 msgstr "Elenca le fonti del dispositivo di input"
 
 msgid "Listening"
@@ -1777,23 +1807,32 @@
 "\n"
 "Possibile soluzione: apri il pannello Gestionale Predefiniti, vai alla "
 "colonna Presets e prova a cliccare sul pulsante \"Ripristina tutto ...\""
 
 msgid "No source duration:"
 msgstr "Nessuna durata sorgente:"
 
+msgid "No source files found in the specified path"
+msgstr "Nessun file sorgente trovato nel percorso specificato"
+
 msgid "No such folder '{}'"
 msgstr "Nessuna cartella denominata '{}'"
 
+msgid "Non-existent source files"
+msgstr "File sorgente inesistenti"
+
 msgid "Normalization"
 msgstr "Normalizzazione"
 
 msgid "Not everything was successful."
 msgstr "Non tutto ha avuto successo."
 
+msgid "Not found"
+msgstr "Non trovato"
+
 msgid "Numerator"
 msgstr "Numeratore"
 
 msgid "OK: Indexes to download"
 msgstr "OK: Indici da scaricare"
 
 msgid "Off"
@@ -2188,14 +2227,20 @@
 
 msgid "Ready"
 msgstr "Pronto"
 
 msgid "Refresh all log files"
 msgstr "Aggiorna tutti i registri"
 
+msgid "Rejected Files"
+msgstr "File Rifiutati"
+
+msgid "Rejected URLs"
+msgstr "URL Rifiutati"
+
 msgid "Reload"
 msgstr "Ricarica"
 
 msgid ""
 "Remember that you can always change these settings later, through the Setup "
 "dialog."
 msgstr ""
@@ -2334,14 +2379,17 @@
 
 msgid "Second pass of the selected profile"
 msgstr "Secondo passaggio del profilo selezionato"
 
 msgid "Seconds"
 msgstr "Secondi"
 
+msgid "See the error message next to each path name"
+msgstr "Vedere il messaggio di errore accanto a ciascun nome di percorso"
+
 msgid "Seek to a position on the video."
 msgstr "Ricerca una posizione nel video."
 
 msgid "Select a log file"
 msgstr "Seleziona un file di registro"
 
 msgid ""
@@ -2619,15 +2667,15 @@
 
 msgid "Shows available encoders for FFmpeg"
 msgstr "Mostra i codificatori disponibili su FFmpeg"
 
 msgid "Shows statistics and information"
 msgstr "Mostra le statistiche e informazioni"
 
-msgid "Shows the text in the toolbar buttons"
+msgid "Shows text in the toolbar buttons"
 msgstr "Mostra il testo nei pulsanti della barra degli strumenti"
 
 msgid "Shows the version in use"
 msgstr "Mostra la versione in uso"
 
 msgid "Simple interlacing filter from progressive contents."
 msgstr "Filtro interlacciamento semplice dai contenuti progressivi."
@@ -2835,17 +2883,14 @@
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "Il tema delle icone scelto cambierà solo le icone,\n"
 "lo sfondo e il primo piano di alcuni campi di testo."
 
-msgid "The downloader is disabled. Check your preferences."
-msgstr "Il downloader è disabilitato. Controlla le tue preferenze."
-
 msgid "The file is not a frame or a video file"
 msgstr "Il file non è un frame o un file video"
 
 msgid ""
 "The files do not have the same \"codec_types\", same \"sample_rate\" or same "
 "\"width\" or \"height\". Unable to proceed."
 msgstr ""
@@ -3523,14 +3568,17 @@
 
 msgid "supported encoders"
 msgstr "codificatori supportati"
 
 msgid "supported formats"
 msgstr "formati supportati"
 
+msgid "yt-dlp is disabled. Check your preferences."
+msgstr "yt-dlp è disabilitato. Controlla le tue preferenze."
+
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr "{0} {1}  |  Durata Segmento: {2}"
 
 msgid ""
 "{}\n"
 "\n"
 "Sorry, removal failed, cannot continue.."
```

### Comparing `videomass-5.0.0/videomass/locale/it_IT/LC_MESSAGES/videomass.po` & `videomass-5.0.1/videomass/locale/it_IT/LC_MESSAGES/videomass.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Italian translation for Videomass.
 # Copyleft -  2023 Gianluca Pernigotto
 # This file is distributed under the same license as the Videomass package
 # FIRST AUTHOR Gianluca Pernigotto <jeanlucperni@gmail.com>, 2020
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
-"PO-Revision-Date: 2023-04-10 14:33+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
+"PO-Revision-Date: 2023-04-18 21:42+0200\n"
 "Last-Translator: Gianluca (jeanslack) Pernigotto <jeanlucperni@gmail.com>\n"
 "Language-Team: Italian <>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: pygettext.py 1.5\n"
@@ -45,20 +45,20 @@
 "\n"
 "{0}"
 msgstr ""
 "Errore imprevisto durante l'eliminazione del contenuto del file:\n"
 "\n"
 "{0}"
 
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr "Azzera"
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -118,71 +118,71 @@
 "Cancella l'elenco\n"
 "dei file importati"
 
 #: ../vdms_dialogs/epilogue.py:100
 msgid "Confirm Settings"
 msgstr "Conferma Impostazioni"
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr "Dimensione origine: {0} x {1} pixel"
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 msgid "Search for a specific frame"
 msgstr "Cerca un fotogramma specifico"
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr "Carica"
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr "Selezione area di ritaglio "
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr "Altezza"
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr "Centro"
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr "Larghezza"
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr "Applica"
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr "Filtro Ritaglia"
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr "Ritaglia in larghezza"
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr "Spostati verticalmente - imposta su -1 per centrare l'asse verticale"
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr "Sposta orizzontalmente - imposta su -1 per centrare l'asse orizzontale"
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr "Ritagliare all'altezza"
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr "Opzioni Avanzate"
 
@@ -322,16 +322,16 @@
 " Questo è un filtro per il denoise 3d di alta precisione e qualità. Mira a "
 "ridurre il rumore dell'immagine, a produrre immagini uniformi e a rendere "
 "ferme le immagini statiche. Dovrebbe migliorare comprensibilmente la qualità "
 "visiva."
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 msgid "Read me"
 msgstr "Leggimi"
 
 #: ../vdms_dialogs/filter_scale.py:80
 msgid "View result"
@@ -404,18 +404,18 @@
 "If you want to keep the aspect ratio, select \"Constrain proportions\" below "
 "and\n"
 "specify only one dimension, either width or height, and set the other "
 "dimension\n"
 "to -1 or -2 (some codecs require -2, so you should do some testing first)."
 msgstr ""
 "Se desideri mantenere le proporzioni, seleziona \"Vincola proporzioni\" di "
-"seguito \n"
+"seguito\n"
 "e specifica solo una dimensione, larghezza o altezza, e imposta l'altra "
-"dimensione \n"
-"su -1 o -2 (alcuni codec richiedono -2, quindi dovresti prima fare qualche "
+"dimensione\n"
+"a -1 o -2 (alcuni codec richiedono -2, quindi prima dovresti fare qualche "
 "test)."
 
 #: ../vdms_dialogs/filter_stab.py:82
 msgid "Enable stabilizer"
 msgstr "Abilita lo stabilizzatore"
 
 #: ../vdms_dialogs/filter_stab.py:84
@@ -426,14 +426,18 @@
 msgid "Create a snapshot"
 msgstr "Crea un'istantanea"
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr "Anteprima"
 
+#: ../vdms_dialogs/filter_stab.py:110
+msgid "Duration seconds:"
+msgstr "Durata in secondi:"
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr "Rilevamento"
 
 #: ../vdms_dialogs/filter_stab.py:177
 msgid "[TRIPOD] Enable tripod mode if checked"
 msgstr "[TRIPOD] Abilita la modalità treppiede"
@@ -805,16 +809,16 @@
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 "Sono richiesti \"ffmpeg\", \"ffprobe\" ed \" ffplay\". Completa tutti\n"
 "i campi di testo sottostanti cliccando sui rispettivi pulsanti."
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr "Scegli l'eseguibile {}"
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 msgid "Videomass has a simple graphical interface for yt-dlp\n"
 msgstr ""
 "Videomass dispone di una semplice interfaccia grafica\n"
@@ -1031,164 +1035,196 @@
 msgid "Miscellanea"
 msgstr "Varie"
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr "Dove preferisci salvare le tue transcodifiche?"
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 msgid "Save each file in the same folder as input file"
 msgstr "Salva ogni file nella stessa cartella del file di input"
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr "Assegna un suffisso aggiuntivo ai nomi dei file in uscita:"
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 "Spostare sempre i file di origine sul cestino di\n"
 "Videomass dopo una corretta codifica"
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr "Dove desideri salvare i tuoi download?"
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 msgid "Auto-create subfolders when downloading playlists"
 msgstr ""
 "Crea automaticamente le sottocartelle durante il download delle playlist"
 
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr "Preferenze file"
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr "Percorso degli eseguibili"
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr "Abilita un'altra posizione per eseguire FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr "Abilita un'altra posizione per eseguire FFprobe"
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr "Abilita un'altra posizione per eseguire FFplay"
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr "Altre opzioni"
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr "Thread utilizzati per la transcodifica (da 0 a 32):"
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
-msgstr "Scarica video da YouTube.com e altri siti di video "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr "Scarica video da YouTube.com e altri siti di video"
+
+#: ../vdms_dialogs/preferences.py:288
+msgid "Enable/Disable yt-dlp"
+msgstr "Abilita/Disabilita yt-dlp"
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr "Preferenze del downloader esterno"
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+"Oltre a quello predefinito (nativo), yt-dlp attualmente\n"
+"supporta i seguenti downloader esterni:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Tieni presente che se abiliti un downloader esterno, non\n"
+"sarai in grado di visualizzare la barra di avanzamento durante\n"
+"le operazioni di download."
+
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
+msgstr "Percorso eseguibile del downloader esterno"
+
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
+msgstr "Argomenti del downloader esterno"
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr "Temi icona"
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "Il tema delle icone scelto cambierà solo le icone,\n"
 "lo sfondo e il primo piano di alcuni campi di testo."
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr "Personalizzazione barra degli strumenti"
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr "Sopra alla finestra (default)"
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr "Sotto alla finestra"
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr "A destra della finestra"
 
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr "A sinistra della finestra"
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 msgid "Place the toolbar"
 msgstr "Posiziona la barra degli strumenti"
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr "Dimensioni icona:"
 
-#: ../vdms_dialogs/preferences.py:349
-msgid "Shows the text in the toolbar buttons"
+#: ../vdms_dialogs/preferences.py:378
+msgid "Shows text in the toolbar buttons"
 msgstr "Mostra il testo nei pulsanti della barra degli strumenti"
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 msgid "Appearance"
 msgstr "Aspetto"
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 "Le seguenti impostazioni influenzano i messaggi di output\n"
 "e i messaggi di registro durante i processi di transcodifica.\n"
 "Modificale solo se sai cosa stai facendo.\n"
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr "Livelli logs FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr "Impostazioni"
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr ""
 "Assegnando un suffisso aggiuntivo è possibile evitare di sovrascrivere i file"
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 msgid "Set a persistent location to save exported files"
 msgstr "Imposta una posizione persistente per salvare i file esportati"
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 "Immettere solo caratteri alfanumerici. È inoltre possibile utilizzare il "
 "trattino (\"-\") e il trattino basso (\"_\"). Non sono ammessi spazi vuoti."
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 msgid "Choose a new destination for the files to be trashed"
 msgstr "Scegli una nuova cartella di destinazione per i file da cestinare"
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 msgid "Set a persistent location to save the file downloads"
 msgstr "Imposta una posizione persistente per salvare i download dei file"
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 msgid "Get Latest Version"
 msgstr "Ottieni l'ultima versione"
 
@@ -1241,15 +1277,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr "SELEZIONE FILE"
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 msgid "Properties"
 msgstr "Proprietà"
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
 msgid "Values"
 msgstr "Valori"
@@ -1772,58 +1808,58 @@
 msgid "Seconds"
 msgstr "Secondi"
 
 #: ../vdms_miniframes/timeline.py:108
 msgid "Milliseconds"
 msgstr "Millisecondi"
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr "Nessuna durata sorgente:"
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr "{0} {1}  |  Durata Segmento: {2}"
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr "Regola Fine"
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 msgid "Start adjustment"
 msgstr "Regola Inizio"
 
-#: ../vdms_miniframes/timeline.py:320
+#: ../vdms_miniframes/timeline.py:322
 msgid "Source duration:"
 msgstr "Durata sorgente:"
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr "ATTENZIONE: Selezione non valida, fuori intervallo."
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 "Inizia trascinando la maniglia in basso a sinistra o fai clic\n"
 "con il pulsante destro del mouse per le opzioni."
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 msgid "Start"
 msgstr "Inizio"
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 msgid "End"
 msgstr "Fine"
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1856,48 +1892,43 @@
 "della barra di stato).\n"
 "\n"
 "I valori di durata \"Inizio\"/\"Fine\" fanno sempre riferimento alla "
 "posizione iniziale della timeline: 00:00:00.000. Le altre informazioni come "
 "la durata del segmento e gli avvisi, saranno visualizzati sui messaggi della "
 "barra di stato."
 
-#: ../vdms_miniframes/timeline.py:559
+#: ../vdms_miniframes/timeline.py:566
 msgid "Timeline Editor Usage"
 msgstr "Note sull'utilizzo dell'editor Timeline"
 
-#: ../vdms_io/checkup.py:45
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
-msgstr ""
-"File già esistenti: \n"
-"\n"
-"{}\n"
-"\n"
-"Vuoi sovrascrivere? "
+#: ../vdms_io/checkup.py:47
+msgid "Files already exist, do you want to overwrite them?"
+msgstr "File già esistenti, vuoi sovrascriverli?"
+
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
+msgstr "Già esistente"
 
-#: ../vdms_io/checkup.py:48
+#: ../vdms_io/checkup.py:50
 msgid "Please Confirm"
 msgstr "Prego confermare"
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
-msgstr ""
-"File inesistente:\n"
-"\n"
-"\"{}\"\n"
-
 #: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
+msgstr "Nessun file sorgente trovato nel percorso specificato"
+
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr "Non trovato"
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr "File sorgente inesistenti"
+
+#: ../vdms_io/checkup.py:75
 msgid ""
 "Output folder does not exist:\n"
 "\n"
 "\"{}\"\n"
 msgstr ""
 "Cartella di output inesistente:\n"
 "\n"
@@ -1965,40 +1996,40 @@
 "and try to click the \"Restore all...\" button"
 msgstr ""
 "Nessun preset trovato.\n"
 "\n"
 "Possibile soluzione: apri il pannello Gestionale Predefiniti, vai alla "
 "colonna Presets e prova a cliccare sul pulsante \"Ripristina tutto ...\""
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr "Pronto"
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 msgid ""
 "There are still processes running. if you want to stop them, use the \"Abort"
 "\" button."
 msgstr ""
 "Ci sono ancora processi avviati... Se vuoi interromperli clicca sul pulsante "
 "\"Interrompi\"."
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr "Videomass"
 
 #: ../vdms_main/main_frame.py:350
 msgid "Are you sure you want to exit the application?"
 msgstr "Sei sicuro di voler uscire dall'applicazione?"
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr "Esci"
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -2179,15 +2210,15 @@
 msgid "View"
 msgstr "Visualizza"
 
 #: ../vdms_main/main_frame.py:520
 msgid "Home panel\tCtrl+Shift+H"
 msgstr "Pannello iniziale\tCtrl+Shift+H"
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 msgid "Go to the 'Home' panel"
 msgstr "Vai al pannello 'Home'"
 
 #: ../vdms_main/main_frame.py:524
 msgid "Presets Manager\tCtrl+Shift+P"
 msgstr "Gestionale Predefiniti\tCtrl+Shift+P"
 
@@ -2243,15 +2274,15 @@
 msgid "Keeps track of the output for debugging errors"
 msgstr "Tiene traccia dell'output per gli errori di debug"
 
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr "Vai"
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr "Imposta una cartella temporanea per le conversioni"
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr "Utilizza una posizione temporanea per salvare le conversioni"
 
@@ -2355,180 +2386,180 @@
 msgid "Help"
 msgstr "Aiuto"
 
 #: ../vdms_main/main_frame.py:677
 msgid "Open the selected files"
 msgstr "Apri i file selezionati"
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 msgid "No such folder '{}'"
 msgstr "Nessuna cartella denominata '{}'"
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 msgid "Are you sure to empty trash folder?"
 msgstr "Sei sicuro di voler svuotare la cartella cestino?"
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 msgid "No files to delete"
 msgstr "Nessun file da eliminare"
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr ""
 "Versione installata v{0}. È disponibile una nuova versione dei preset {1}"
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr "Versione installata v{0}. Nessun nuovo aggiornamento trovato."
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr "Scegli una cartella per il download"
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 "Attendi....\n"
 "L'archivio è in fase di download"
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr "Scaricato correttamente in \"{0}\""
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr "Scegli una destinazione temporanea per le conversioni"
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 msgid "Default destination folders successfully restored"
 msgstr "Cartelle di destinazione predefinite ripristinate correttamente"
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 msgid "Changes will take effect once the program has been restarted."
 msgstr "Le modifiche avranno effetto una volta riavviato il programma."
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr ""
 "Le modifiche avranno effetto una volta riavviato il programma\n"
 "\n"
 "Vuoi uscire dall'applicazione ora?"
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, python-brace-format
 msgid "A new release is available - v.{0}\n"
 msgstr "È disponibile un nuovo rilascio - v.{0}\n"
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr ""
 "Stai utilizzando una versione di sviluppo che non è ancora stata "
 "rilasciata!\n"
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr "Congratulazioni! Stai già usando l'ultima versione.\n"
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr "Vai al pannello precedente"
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr "Indietro"
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr "Vai al prossimo pannello"
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 msgid "Next"
 msgstr "Avanti"
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr "Casa"
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 msgid "Play the selected file in the list"
 msgstr "Riproduci il file selezionato nell'elenco"
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr "Riproduci"
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 msgid "Get informative data about imported media streams"
 msgstr "Ottieni dati informativi sui flussi dei media importati"
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 msgid "Start rendering"
 msgstr "Avvia il rendering"
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr "Avvia"
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr "Interrompi il processo corrente"
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr "Interrompi"
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr "Elimina tutti i file dall'elenco"
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr "Cancella"
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 msgid "Videomass - Queued Files"
 msgstr "Videomass - File in Coda"
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr "Videomass - Conversioni AV"
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr "Videomass - Gestionale Predefiniti"
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 msgid "Videomass - Concatenate Demuxer"
 msgstr "Videomass - Concatenate Demuxer"
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 msgid "Videomass - From Movie to Pictures"
 msgstr "Videomass - Dal Filmato alle Immagini"
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 msgid "Videomass - Still Image Maker"
 msgstr "Videomass - Creatore di Presentazioni"
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr "Visualizzazione ultimo log"
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr "In lavorazione..."
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 msgid "Videomass - FFmpeg message monitor"
 msgstr "Videomass - Monitor messaggi FFmpeg"
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
 msgstr "Media:"
 
@@ -2869,20 +2900,20 @@
 msgid "{} file in queue"
 msgstr "{} file in coda"
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr "Spento"
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr "Non settato"
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr "inizio  {} | durata  {}"
 
 #: ../vdms_panels/av_conversions.py:2261
 msgid ""
 "Queued File\n"
@@ -3095,16 +3126,16 @@
 
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 "Estrai immagini (frame) dai tuoi filmati nei formati JPG, PNG, BMP, GIF."
 
 #: ../vdms_panels/choose_topic.py:223
-msgid "The downloader is disabled. Check your preferences."
-msgstr "Il downloader è disabilitato. Controlla le tue preferenze."
+msgid "yt-dlp is disabled. Check your preferences."
+msgstr "yt-dlp è disabilitato. Controlla le tue preferenze."
 
 #: ../vdms_panels/concatenate.py:78
 msgid ""
 "\n"
 "- The concatenation function is performed only with Audio files or only with "
 "Video files.\n"
 "\n"
@@ -3206,110 +3237,118 @@
 msgstr ""
 "File da concatenare\n"
 "Nome file in uscita\n"
 "Destinazione\n"
 "Formato in Uscita\n"
 "Segmento Tempo"
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr "Il file ha caratteri non validi come:"
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 msgid "Invalid path name. Contains double or single quotes"
 msgstr "Nome del file non valido. Contiene virgolette doppie o singole"
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 msgid "Directories are not allowed, just add files, please."
 msgstr "Le directory non sono ammesse, aggiungi solo file."
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 "File senza estensione di formato: fornire un'estensione appropriata al nome "
 "del file, ad esempio '.mkv', '.avi', '.mp3', ecc."
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr "Il nome ha caratteri non validi come: {0}"
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr "Nome già in uso:"
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr "Nome File"
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr "Durata"
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr "Tipo di media"
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr "Dimensione"
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 msgid "Output file name"
 msgstr "Nome del file in uscita"
 
-#: ../vdms_panels/filedrop.py:207
-msgid "Duplicate files are rejected: > {}"
-msgstr "I files duplicati sono rifiutati: > {}"
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr "File duplicato, è già stato aggiunto all'elenco."
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr "Vedere il messaggio di errore accanto a ciascun nome di percorso"
+
+#: ../vdms_panels/filedrop.py:209
+msgid "Rejected Files"
+msgstr "File Rifiutati"
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr "Trascina uno o più file qui sotto"
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 msgid "Destination folder"
 msgstr "Cartella di destinazione"
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 msgid "Drag the images below"
 msgstr "Trascina le immagini qui sotto"
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 msgid "Drag one or more video below"
 msgstr "Trascina uno o più video qui sotto"
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 msgid "No file selected"
 msgstr "Nessun file selezionato"
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 msgid "File renaming..."
 msgstr "Ridenominazione file..."
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 msgid "Rename the selected file to:"
 msgstr "Rinomina il file selezionato in:"
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr "Aggiungi Files"
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr "Rinomina elementi"
 
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr "Rinominare i {0} elementi in:"
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 msgid "New Name #"
 msgstr "Nuovo Nome #"
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
 msgid "[Videomass]: SUCCESS !"
 msgstr "[Videomass]: SUCCESSO !"
@@ -3734,19 +3773,19 @@
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 "Il comando del profilo selezionato è stato cambiato manualmente.\n"
 "Vuoi applicarlo durante il processo di conversione?"
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 msgid "Don't show this dialog again"
 msgstr "Non mostrare ancora questo dialogo"
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 msgid ""
 "Queued File\n"
 "Pass Encoding\n"
 "Profile Used\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
@@ -3765,45 +3804,49 @@
 #: ../vdms_panels/sequence_to_video.py:74
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 "\n"
 "1. Importa uno o più file immagine nei formati JPG, PNG e BMP, quindi "
 "selezionane uno.\n"
 "\n"
 "2. Utilizzare la funzione Ridimensionamento per ridimensionare le immagini "
-"che hanno dimensioni diverse come larghezza e\n"
-"altezza. Negli altri casi è opzionale.\n"
+"che hanno \n"
+"dimensioni diverse come larghezza e altezza. Negli altri casi è opzionale.\n"
 "\n"
 "3. Per impostare la DURATA tra le immagini usa l'editor Timeline (CTRL+T) e "
-"regolare solo il valore \"Fine\",\n"
-"lasciando il valore \"Inizio\" a 00:00:00.000.\n"
+"regolare solo il\n"
+"valore \"Fine\", lasciando il valore \"Inizio\" a 00:00:00.000.\n"
 "\n"
 "4. Avvia la conversione.\n"
 "\n"
 "\n"
 "Il video prodotto avrà il nome del file selezionato nell'elenco 'File in "
-"coda', il quale verrà salvato in una cartella denominata 'Still_Images'\n"
-"con l'aggiunta di una cifra progressiva, nel percorso da te specificato."
+"coda', il quale verrà salvato\n"
+"in una cartella denominata 'Still_Images' con l'aggiunta di una cifra "
+"progressiva, nel percorso\n"
+"da te specificato."
 
 #: ../vdms_panels/sequence_to_video.py:129
 msgid "Enable a single still image"
 msgstr "Abilita un fermo immagine singolo"
 
 #: ../vdms_panels/sequence_to_video.py:161
 msgid ""
@@ -3861,14 +3904,25 @@
 msgstr "File non valido: '{}'"
 
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 msgid "Unsupported format '{}'"
 msgstr "Formato non supportato '{}'"
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+"File inesistente:\n"
+"\n"
+"\"{}\"\n"
+
 #: ../vdms_panels/sequence_to_video.py:719
 msgid ""
 "File to process\n"
 "Output filename\n"
 "Destination Folder\n"
 "Output Format\n"
 "Additional arguments\n"
@@ -3980,40 +4034,40 @@
 
 #: ../vdms_panels/video_to_sequence.py:49
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 "\n"
 "1. Importa uno o più file video, quindi selezionane uno.\n"
 "\n"
 "2. Per selezionare un intervallo di tempo utilizzare l'editor Timeline (CTRL"
-"+T), e regolare i valori di durata\n"
-"di \"Inizio\" e \"Fine\" come desiderato.\n"
+"+T), e \n"
+"regolare i valori di durata di \"Inizio\" e \"Fine\" come desiderato.\n"
 "\n"
 "3. Selezionare un formato di output (jpg, png, bmp o gif).\n"
 "\n"
 "4. Avvia la conversione.\n"
 "\n"
 "\n"
 "Le immagini prodotte verranno salvate in una cartella denominata "
-"'Movie_to_Pictures' con l'aggiunta \n"
-"di una cifra progressiva, nel percorso da te specificato."
+"'Movie_to_Pictures'\n"
+"con l'aggiunta  di una cifra progressiva, nel percorso da te specificato."
 
 #: ../vdms_panels/video_to_sequence.py:84
 msgid "Create thumbnails"
 msgstr "Crea miniature"
 
 #: ../vdms_panels/video_to_sequence.py:85
 msgid "Create tiled mosaics"
@@ -4095,15 +4149,15 @@
 "È necessario spuntare almeno un \"Codice Formato\" per ciascun URL "
 "selezionato in verde."
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr "Codice Formato"
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr "Url"
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr "Titolo"
 
@@ -4184,25 +4238,25 @@
 msgid "Hide YouTube Downloader"
 msgstr "Nascondi YouTube Downloader"
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 msgid "Quit YouTube Downloader"
 msgstr "Esci da YouTube Downloader"
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 msgid "Paste\tCtrl+V"
 msgstr "Incolla\tCtrl+V"
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr "Incolla gli URL copiati negli appunti"
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr "Rimuovi l'URL selezionato\tDEL"
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 msgid "Remove the selected URL from the list"
 msgstr "Rimuove l'URL selezionato dall'elenco"
 
@@ -4218,15 +4272,15 @@
 msgid "Latest version of yt-dlp"
 msgstr "Ultima versione di yt-dlp"
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 msgid "Check the latest version available on github.com"
 msgstr "Mostra l'ultima versione disponibile su github.com"
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr "Imposta una cartella temporanea per i download"
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr "Salva tutti i download in questa posizione temporanea"
 
@@ -4332,19 +4386,27 @@
 msgid ""
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr ""
 "ATTENZIONE: L'URL selezionato non fa riferimento a una playlist. È possibile "
 "indicizzare solo le righe contrassegnate in verde."
 
-#: ../vdms_ytdlp/textdrop.py:74
-msgid "Invalid URL:"
-msgstr "URL non valido:"
+#: ../vdms_ytdlp/textdrop.py:68
+msgid "Invalid URL"
+msgstr "URL non valido"
+
+#: ../vdms_ytdlp/textdrop.py:84
+msgid "List of rejected URLs"
+msgstr "Lista degli URL rifiutati"
+
+#: ../vdms_ytdlp/textdrop.py:87
+msgid "Rejected URLs"
+msgstr "URL Rifiutati"
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr "Trascina o incolla qui gli URL"
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 msgid "Statistics viewer"
 msgstr "Visualizzatore di statistiche"
 
@@ -4457,14 +4519,33 @@
 msgid "The URLs contain playlists. Are you sure you want to continue?"
 msgstr "Gli URL contengono playlist. Sei sicuro di voler continuare?"
 
 #: ../vdms_ytdlp/youtubedl_ui.py:659
 msgid "The URLs contain channels. Are you sure you want to continue?"
 msgstr "Gli URL contengono canali. Sei sicuro di voler continuare?"
 
+#~ msgid "URLs that have been rejected:"
+#~ msgstr "URL che sono stati rifiutati:"
+
+#~ msgid ""
+#~ "Already exist: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Do you want to overwrite? "
+#~ msgstr ""
+#~ "File già esistenti: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Vuoi sovrascrivere? "
+
+#~ msgid "Duplicate files are rejected: > {}"
+#~ msgstr "I files duplicati sono rifiutati: > {}"
+
 #~ msgid "Contextual help to the Timeline Editor"
 #~ msgstr "Aiuto contestuale all'editor timeline"
 
 #~ msgid "Segment Start   (HH:MM:SS.ms)"
 #~ msgstr "Inizio Segmento   (HH:MM:SS.ms)"
 
 #~ msgid "Segment Duration   (HH:MM:SS.ms)"
@@ -4763,17 +4844,14 @@
 #~ msgid ""
 #~ "Make sure you are using the latest available version of\n"
 #~ "'{}'. This allows you to avoid download problems.\n"
 #~ msgstr ""
 #~ "Assicurati di utilizzare l'ultima versione disponibile di '{}'\n"
 #~ "Ciò ti consente di evitare problemi di download.\n"
 
-#~ msgid "Not found"
-#~ msgstr "Non trovato"
-
 #~ msgid "Not Installed"
 #~ msgstr "Non installato"
 
 #~ msgid "Downloader"
 #~ msgstr "Downloader"
 
 #~ msgid "Topic List..."
@@ -4919,17 +4997,14 @@
 
 #~ msgid "Duration hours"
 #~ msgstr "Durata in ore"
 
 #~ msgid "Duration minutes"
 #~ msgstr "Durata in minuti"
 
-#~ msgid "Duration seconds"
-#~ msgstr "Durata in secondi"
-
 #~ msgid "Duration milliseconds"
 #~ msgstr "Durata in millisecondi"
 
 #~ msgid "Start hours"
 #~ msgstr "Inizio in ore"
 
 #~ msgid "Show panel for editing timeline (seek/duration)"
@@ -5457,17 +5532,14 @@
 
 #~ msgid "Disable all"
 #~ msgstr "Disabilita tutto"
 
 #~ msgid "Successful! {} is up-to-date"
 #~ msgstr "Riuscito! {} è aggiornato"
 
-#~ msgid "Disable youtube-dl"
-#~ msgstr "Disabilita youtube-dl"
-
 #~ msgid "Enable youtube-dl"
 #~ msgstr "Abilita youtube-dl"
 
 #~ msgid "youtube-dl"
 #~ msgstr "youtube-dl"
 
 #~ msgid "Update youtube-dl"
@@ -5864,17 +5936,14 @@
 
 #~ msgid "Import a group of Videomass presets"
 #~ msgstr "Importa un gruppo di preset Videomass"
 
 #~ msgid "A new group of presets was successfully imported"
 #~ msgstr "Un nuovo gruppo di preset è stato importato con successo"
 
-#~ msgid "This preset already exists, do you want to overwrite it?"
-#~ msgstr "Questo preset esiste già, vuoi sovrascriverlo?"
-
 #, fuzzy
 #~| msgid "You just added new files. Please check your settings again."
 #~ msgid "You just changed the queued files. Please check your settings again."
 #~ msgstr ""
 #~ "Hai appena aggiunto nuovi file. Controlla nuovamente le tue impostazioni."
 
 #~ msgid "Customize..."
```

### Comparing `videomass-5.0.0/videomass/locale/nl_NL/LC_MESSAGES/videomass.mo` & `videomass-5.0.1/videomass/locale/nl_NL/LC_MESSAGES/videomass.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-10 14:35+0200\n"
+"PO-Revision-Date: 2023-04-18 21:44+0200\n"
 "Last-Translator: johannesdedoper <https://github.com/johannesdedoper>\n"
 "Language-Team: Dutch <>\n"
 "Language: nl_NL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -184,27 +184,14 @@
 
 msgid "All default presets have been successfully recovered"
 msgstr "Alle standaard presets zijn met succes hersteld"
 
 msgid "All presets have been exported successfully"
 msgstr "Alle presets zijn succesvol geëxporteerd"
 
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
-msgstr ""
-"Bestaat reeds: \n"
-"\n"
-"{}\n"
-"\n"
-"Overschrijven? "
-
 msgid "Appearance"
 msgstr "Uiterlijk"
 
 msgid "Application preferences"
 msgstr "Applicatie voorkeuren"
 
 msgid "Apply"
@@ -632,17 +619,14 @@
 
 msgid "Drag one or more files below"
 msgstr "Sleep een of meer bestanden hieronder"
 
 msgid "Duplicate"
 msgstr "Kopieer"
 
-msgid "Duplicate files are rejected: > {}"
-msgstr "Gelijke bestanden zijn overgeslagen: > {}"
-
 msgid "Duration"
 msgstr "Duur"
 
 msgid "Duration:"
 msgstr "Duur:"
 
 msgid "ERROR"
@@ -1159,14 +1143,17 @@
 
 msgid "Normalization"
 msgstr "Normalisatie"
 
 msgid "Not everything was successful."
 msgstr "Niet alles was succesvol."
 
+msgid "Not found"
+msgstr "Niet gevonden"
+
 msgid "Numerator"
 msgstr "Teller"
 
 msgid "OK: Indexes to download"
 msgstr "OK: Index om te downloaden"
 
 msgid "Off"
@@ -1665,17 +1652,14 @@
 
 msgid "Shows available decoders for FFmpeg"
 msgstr "Toont beschikbare decoders voor FFmpeg"
 
 msgid "Shows available encoders for FFmpeg"
 msgstr "Toont beschikbare encoders voor FFmpeg"
 
-msgid "Shows the text in the toolbar buttons"
-msgstr "Toont de tekst in de knoppenbalk knoppen"
-
 msgid "Shows the version in use"
 msgstr "Toont de gebruikte versie"
 
 msgid "Simple interlacing filter from progressive contents."
 msgstr "Simpel interlacing filter voor progressieve beelden."
 
 msgid "Size"
@@ -1769,17 +1753,14 @@
 msgid ""
 "The audio bitrate affects the file compression and thus the quality of "
 "listening. The higher the value, the higher the quality."
 msgstr ""
 "De audio bitrate beïnvloedt de bestandscompressie en daarom de "
 "geluidskwaliteit. Hoe hoger de waarde, hoe hoger de kwaliteit."
 
-msgid "The downloader is disabled. Check your preferences."
-msgstr "De youtube-dl is uitgezet. Controleer uw voorkeuren."
-
 msgid "The file is not a frame or a video file"
 msgstr "Het bestand is geen frame en geen video bestand"
 
 msgid ""
 "The files do not have the same \"codec_types\", same \"sample_rate\" or same "
 "\"width\" or \"height\". Unable to proceed."
 msgstr ""
```

### Comparing `videomass-5.0.0/videomass/locale/nl_NL/LC_MESSAGES/videomass.po` & `videomass-5.0.1/videomass/locale/nl_NL/LC_MESSAGES/videomass.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Dutch translation for Videomass.
 # Copyleft -  2023 Gianluca Pernigotto
 # This file is distributed under the same license as the Videomass package
 # FIRST AUTHOR Gianluca Pernigotto <jeanlucperni@gmail.com>, 2021
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
-"PO-Revision-Date: 2023-04-10 14:35+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
+"PO-Revision-Date: 2023-04-18 21:44+0200\n"
 "Last-Translator: johannesdedoper <https://github.com/johannesdedoper>\n"
 "Language-Team: Dutch <>\n"
 "Language: nl_NL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -41,20 +41,20 @@
 "\n"
 "{0}"
 msgstr ""
 "Onverwachte fout bij het verwijderen van bestands inhoud:\n"
 "\n"
 "{0}"
 
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr "Reset"
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -116,71 +116,71 @@
 
 #: ../vdms_dialogs/epilogue.py:100
 #, fuzzy
 #| msgid "Cache Settings"
 msgid "Confirm Settings"
 msgstr "Cache Instellingen"
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr "Bron grootte: {0} x {1} pixels"
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 msgid "Search for a specific frame"
 msgstr "Zoek naar een specifiek frame"
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr "Laad"
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr "Gebied-selectie bijsnijden "
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr "Hoogte"
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr "Centrum"
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr "Breedte"
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr "Toepassen"
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr "Bijsnij Filter"
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr "Snij breedte bij"
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr "Verplaats verticaal - zet op -1 om de verticale as te centreren"
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr "Verplaats horizontaal - zet op -1 om de horizontale as te centreren"
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr "Snij hoogte bij"
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr "Geavanceerde Opties"
 
@@ -317,16 +317,16 @@
 "hqdn3d:\n"
 "Dit is een 3d denoise filter met hoge nauwkeurigheid / kwaliteit. Het beoogt "
 "beeldruis te verminderen, wat resulteert in vloeiende beelden, waarbij "
 "stilstaande beelden echt stil staan. Compressie zal hierdoor verbeteren."
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 #, fuzzy
 #| msgid "Ready"
 msgid "Read me"
 msgstr "Gereed"
 
@@ -422,14 +422,20 @@
 msgid "Create a snapshot"
 msgstr "Maak een nieuwe preset"
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr "Voorvertoning"
 
+#: ../vdms_dialogs/filter_stab.py:110
+#, fuzzy
+#| msgid "Duration"
+msgid "Duration seconds:"
+msgstr "Duur"
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr "Video Detecteren"
 
 #: ../vdms_dialogs/filter_stab.py:177
 msgid "[TRIPOD] Enable tripod mode if checked"
 msgstr "[TRIPOD] Activeer tripod modus wanneer geselecteerd"
@@ -812,16 +818,16 @@
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 "\"ffmpeg\", \"ffprobe\" en \"ffplay\" zijn vereist. Vul alle onderstaande\n"
 "tekstkaders in, door op de betreffende knoppen te drukken."
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr "Kies het {} programmabestand"
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 #, fuzzy
 #| msgid ""
 #| "Videomass has a simple graphical\n"
@@ -1050,171 +1056,201 @@
 msgid "Miscellanea"
 msgstr "Diversen"
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr "Waar wilt u transcoderingen bewaren?"
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 msgid "Save each file in the same folder as input file"
 msgstr "Bewaar elk bestand in dezelfde map als input bestand"
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr "Ken optioneel achtervoegsel toe aan output-bestandsnamen:"
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 #, fuzzy
 #| msgid ""
 #| "Move source file to the Videomass trash folder after successful encoding"
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 "Verplaats de orginele file naar de Videomass Prullenbak na een succesvolle "
 "encoding"
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr "Waar wilt u gedownloade bestanden bewaren?"
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 msgid "Auto-create subfolders when downloading playlists"
 msgstr "Maak automatisch sub-mappen bij downloaden van afspeellijsten"
 
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr "Bestands Voorkeuren"
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr "Pad naar de programmabestanden"
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr "Activeer een andere lokatie om FFmpeg uit te voeren"
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr "Activeer een andere lokatie om FFprobe uit te voeren"
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr "Activeer een andere lokatie om FFplay uit te voeren"
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr "Andere opties"
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr "Aantal threads voor transcoden (van 0 tot 32)"
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:288
+#, fuzzy
+#| msgid "Disable youtube-dl"
+msgid "Enable/Disable yt-dlp"
+msgstr "Deactiveer youtube-dl"
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr "Icoon thema's"
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 #, fuzzy
 #| msgid ""
 #| "setting the icons will also change the background\n"
 #| "and foreground of some text fields."
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "instellen van iconen zal ook de achtergrond\n"
 "en voorgrond wijzigen van bepaalde tekstvelden."
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr "Knoppenbalk aanpassing"
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr "Bovenaan venster (standaard)"
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr "Onderaan venster"
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr "Rechts van venster"
 
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr "Links van venster"
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 msgid "Place the toolbar"
 msgstr "Plaats de knoppenbalk"
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr "Icoon grootte:"
 
-#: ../vdms_dialogs/preferences.py:349
-msgid "Shows the text in the toolbar buttons"
+#: ../vdms_dialogs/preferences.py:378
+#, fuzzy
+#| msgid "Shows the text in the toolbar buttons"
+msgid "Shows text in the toolbar buttons"
 msgstr "Toont de tekst in de knoppenbalk knoppen"
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 msgid "Appearance"
 msgstr "Uiterlijk"
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 "De volgende instellingen bepalen output-berichten\n"
 "en log-berichten tijdens transcode-processen.\n"
 "Wijzig alleen als u weet wat u doet.\n"
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr "FFmpeg log niveau's"
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr "Instellingen"
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr ""
 "Door toewijzing van een achtervoegsel kunt u overschrijven van bestanden "
 "voorkomen"
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 msgid "Set a persistent location to save exported files"
 msgstr "Geef een vaste lokatie waar u export-bestanden wilt bewaren"
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 "Gebruik alleen alpha-numerieke tekens 0-9 A-Z. Het streepje (\"-\") en de "
 "underscore (\"_\") kunt u ook gebruiken. Spaties zijn niet toegestaan."
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 msgid "Choose a new destination for the files to be trashed"
 msgstr "Kies een bestemming voor de bestanden om te deleten"
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 msgid "Set a persistent location to save the file downloads"
 msgstr "Geef een vaste lokatie waar u de download-bestanden wilt bewaren"
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 msgid "Get Latest Version"
 msgstr "Download laatste versie"
 
@@ -1271,15 +1307,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr "BESTAND SELECTIE"
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 #, fuzzy
 #| msgid "Audio Properties"
 msgid "Properties"
 msgstr "Audio Eigenschappen"
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
@@ -1850,64 +1886,64 @@
 msgid "Seconds"
 msgstr ""
 
 #: ../vdms_miniframes/timeline.py:108
 msgid "Milliseconds"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 #, fuzzy
 #| msgid "Starts"
 msgid "Start adjustment"
 msgstr "Start"
 
-#: ../vdms_miniframes/timeline.py:320
+#: ../vdms_miniframes/timeline.py:322
 #, fuzzy
 #| msgid "Duration:"
 msgid "Source duration:"
 msgstr "Duur:"
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 #, fuzzy
 #| msgid "Starts"
 msgid "Start"
 msgstr "Start"
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 #, fuzzy
 #| msgid "Enabled"
 msgid "End"
 msgstr "Geactiveerd"
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1920,50 +1956,47 @@
 "duration of a selected source file (see status bar messages).\n"
 "\n"
 "The \"Start\"/\"End\" duration values always refer to the initial position "
 "of the timeline: 00:00:00.000. For other informations as the segment "
 "duration and warnings, please refer to the status bar messages."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:559
+#: ../vdms_miniframes/timeline.py:566
 #, fuzzy
 #| msgid "Show timeline\tCtrl+T"
 msgid "Timeline Editor Usage"
 msgstr "Toon tijdslijn\tCtrl+T"
 
-#: ../vdms_io/checkup.py:45
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
+#: ../vdms_io/checkup.py:47
+#, fuzzy
+#| msgid "A file with this name already exists, do you want to overwrite it?"
+msgid "Files already exist, do you want to overwrite them?"
+msgstr "Een bestand met deze naam bestaat al, wilt u het overschrijven?"
+
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
 msgstr ""
-"Bestaat reeds: \n"
-"\n"
-"{}\n"
-"\n"
-"Overschrijven? "
 
-#: ../vdms_io/checkup.py:48
+#: ../vdms_io/checkup.py:50
 msgid "Please Confirm"
 msgstr "Bevestig aub"
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
+#: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
 msgstr ""
-"Bestand bestaat niet:\n"
-"\n"
-"\"{}\"\n"
 
-#: ../vdms_io/checkup.py:62
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr "Niet gevonden"
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr ""
+
+#: ../vdms_io/checkup.py:75
 msgid ""
 "Output folder does not exist:\n"
 "\n"
 "\"{}\"\n"
 msgstr ""
 "Output map bestaat niet:\n"
 "\n"
@@ -2032,18 +2065,18 @@
 "and try to click the \"Restore all...\" button"
 msgstr ""
 "Geen presets gevonden.\n"
 "\n"
 "Mogelijke oplossing: open het Presets Manager paneel, ga naar de presets "
 "kolom en probeer de \"Herstel allen...\" knop te drukken"
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr "Gereed"
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 #, fuzzy
 #| msgid ""
 #| "There are still processes running.. if you want to stop them, use the "
@@ -2054,27 +2087,27 @@
 "There are still processes running. if you want to stop them, use the \"Abort"
 "\" button."
 msgstr ""
 "Er zijn nog processen bezig.. druk de knop \"Afbreken\" om deze te stoppen.\n"
 "\n"
 "Wilt u de applicatie afbreken?"
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr "Videomass"
 
 #: ../vdms_main/main_frame.py:350
 #, fuzzy
 #| msgid "Are you sure you want to exit?"
 msgid "Are you sure you want to exit the application?"
 msgstr "Afsluiten : bent u zeker?"
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr "Afsluiten"
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -2276,15 +2309,15 @@
 
 #: ../vdms_main/main_frame.py:520
 #, fuzzy
 #| msgid "Home panel\tShift+H"
 msgid "Home panel\tCtrl+Shift+H"
 msgstr "Home panel\tShift+H"
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 #, fuzzy
 #| msgid "Go to the next panel"
 msgid "Go to the 'Home' panel"
 msgstr "Ga naar volgende panel"
 
 #: ../vdms_main/main_frame.py:524
 #, fuzzy
@@ -2366,15 +2399,15 @@
 msgid "Keeps track of the output for debugging errors"
 msgstr "Inspecteert output voor debug-fouten"
 
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr "Ga naar"
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr "Stel een tijdelijke folder in voor conversies"
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr "Gebruik een tijdelijke locatie om conversies te bewaren"
 
@@ -2488,187 +2521,187 @@
 
 #: ../vdms_main/main_frame.py:677
 #, fuzzy
 #| msgid "Delete the selected profile"
 msgid "Open the selected files"
 msgstr "Verwijder het geselecteerde profiel"
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 msgid "No such folder '{}'"
 msgstr "Er is geen folder '{}'"
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 msgid "Are you sure to empty trash folder?"
 msgstr "Weet u zeker dat u de Videomass Prullenbak wilt legen?"
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 msgid "No files to delete"
 msgstr "Geen bestanden om te deleten"
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr "Kies een download folder"
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 "Wacht....\n"
 "Het archief wordt gedownload"
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr "Succesvol gedownload naar \"{0}\""
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr "Kies een tijdelijke bestemming voor de conversies"
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 msgid "Default destination folders successfully restored"
 msgstr "Standaard bestemming-folders succesvol hersteld"
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 msgid "Changes will take effect once the program has been restarted."
 msgstr "Wijzigingen worden pas doorgevoerd na herstart van dit programma."
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr ""
 "Wijzigingen worden pas doorgevoerd na herstart van dit programma.\n"
 "\n"
 "Wil je het programma nu sluiten?"
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, python-brace-format
 msgid "A new release is available - v.{0}\n"
 msgstr "Er is een nieuwe versie beschikbaar - v.{0}\n"
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr "U gebruikt een ontwikkelaars versie die nog niet is vrijgegeven!\n"
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr "Gefeliciteerd! U gebruikt al de laatste versie.\n"
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr "Ga naar vorig panel"
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr "Terug"
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr "Ga naar volgende panel"
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 msgid "Next"
 msgstr "Volgende"
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 #, fuzzy
 #| msgid "Play the selected files in the list"
 msgid "Play the selected file in the list"
 msgstr "Speel de geselecteerde bestanden in de lijst af"
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr "Speel"
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 #, fuzzy
 #| msgid "Gathers information of multimedia streams"
 msgid "Get informative data about imported media streams"
 msgstr "Wint informatie in over multimedia streams"
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 #, fuzzy
 #| msgid "Starts"
 msgid "Start rendering"
 msgstr "Start"
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr "Stopt huidige proces"
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr "Afbreken"
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr "Verwijder alle bestanden uit de lijst"
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 msgid "Videomass - Queued Files"
 msgstr "Videomass - Wachtrij Bestanden"
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr "Videomass - AV Conversies"
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr "Videomass - Presets Manager"
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 msgid "Videomass - Concatenate Demuxer"
 msgstr "Videomass - Samenvoeg Demuxer"
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 #, fuzzy
 #| msgid "From an image sequence to a video file"
 msgid "Videomass - From Movie to Pictures"
 msgstr "Van afbeelingen serie naar een video file"
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 #, fuzzy
 #| msgid "Videomass - Presets Manager"
 msgid "Videomass - Still Image Maker"
 msgstr "Videomass - Presets Manager"
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr "Laatste log-berichten bekijken"
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr "Bezig..."
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 #, fuzzy
 #| msgid "Videomass - Output Monitor"
 msgid "Videomass - FFmpeg message monitor"
 msgstr "Videomass - Output Monitor"
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
@@ -3033,20 +3066,20 @@
 msgid "{} file in queue"
 msgstr "{} bestand in wachtrij"
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr "Uit"
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr "Uitgezet"
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr "start  {} | duur  {}"
 
 #: ../vdms_panels/av_conversions.py:2261
 msgid ""
 "Queued File\n"
@@ -3290,15 +3323,17 @@
 msgstr ""
 
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 
 #: ../vdms_panels/choose_topic.py:223
-msgid "The downloader is disabled. Check your preferences."
+#, fuzzy
+#| msgid "The downloader is disabled. Check your preferences."
+msgid "yt-dlp is disabled. Check your preferences."
 msgstr "De youtube-dl is uitgezet. Controleer uw voorkeuren."
 
 #: ../vdms_panels/concatenate.py:78
 #, fuzzy
 #| msgid ""
 #| "NOTE:\n"
 #| "\n"
@@ -3420,122 +3455,132 @@
 msgstr ""
 "Bestand om aaneen te schakelen\n"
 "Output bestandsnaam\n"
 "Bestemming\n"
 "Output Formaat\n"
 "Tijd Periode"
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 #, fuzzy
 #| msgid "Invalid filename. Contains double or single quotes"
 msgid "Invalid path name. Contains double or single quotes"
 msgstr "Ongeldige bestandsnaam. Bevat dubbele of enkele aanhalingstekens"
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 msgid "Directories are not allowed, just add files, please."
 msgstr "Folders zijn niet toegestaan, voeg alleen bestanden toe."
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 "Bestand zonder formaat extensie: u dient een treffende extensie te geven aan "
 "de bestandsnaam, bijv. '.mkv', '.avi', '.mp3', etc."
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr "Bestandsnaam"
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr "Duur"
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr "Media type"
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr "Grootte"
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 #, fuzzy
 #| msgid "Output index:"
 msgid "Output file name"
 msgstr "Output index:"
 
-#: ../vdms_panels/filedrop.py:207
-msgid "Duplicate files are rejected: > {}"
-msgstr "Gelijke bestanden zijn overgeslagen: > {}"
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr ""
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:209
+#, fuzzy
+#| msgid "Add Files"
+msgid "Rejected Files"
+msgstr "Voeg bestanden toe"
+
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr "Sleep een of meer bestanden hieronder"
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 msgid "Destination folder"
 msgstr "Bestemming folder"
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag the images below"
 msgstr "Sleep een of meer bestanden hieronder"
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag one or more video below"
 msgstr "Sleep een of meer bestanden hieronder"
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 msgid "No file selected"
 msgstr "Geen bestand geselecteerd"
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 #, fuzzy
 #| msgid "File name"
 msgid "File renaming..."
 msgstr "Bestandsnaam"
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 #, fuzzy
 #| msgid "Delete the selected profile"
 msgid "Rename the selected file to:"
 msgstr "Verwijder het geselecteerde profiel"
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr "Voeg bestanden toe"
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 #, fuzzy
 #| msgid "File Name"
 msgid "New Name #"
 msgstr "Bestandsnaam"
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
@@ -3950,19 +3995,19 @@
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 "Het geselecteerde profiel commando is handmatig gewijzigd.\n"
 "Wilt u dit toepassen voor het conversie proces?"
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 msgid "Don't show this dialog again"
 msgstr "Toon dit dialoogscherm niet meer"
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 msgid ""
 "Queued File\n"
 "Pass Encoding\n"
 "Profile Used\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
@@ -3979,26 +4024,28 @@
 #: ../vdms_panels/sequence_to_video.py:74
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 
 #: ../vdms_panels/sequence_to_video.py:129
 msgid "Enable a single still image"
 msgstr ""
 
 #: ../vdms_panels/sequence_to_video.py:161
@@ -4057,14 +4104,25 @@
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 #, fuzzy
 #| msgid "Supported Format List"
 msgid "Unsupported format '{}'"
 msgstr "Lijst Ondersteunde Formaten"
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+"Bestand bestaat niet:\n"
+"\n"
+"\"{}\"\n"
+
 #: ../vdms_panels/sequence_to_video.py:719
 msgid ""
 "File to process\n"
 "Output filename\n"
 "Destination Folder\n"
 "Output Format\n"
 "Additional arguments\n"
@@ -4163,24 +4221,24 @@
 
 #: ../vdms_panels/video_to_sequence.py:49
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 
 #: ../vdms_panels/video_to_sequence.py:84
 msgid "Create thumbnails"
 msgstr ""
 
 #: ../vdms_panels/video_to_sequence.py:85
@@ -4250,15 +4308,15 @@
 "Minstens een \"Formaat Code\" moet gezet zijn voor elke URL, groen "
 "geselecteerd."
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr "Formaat Code"
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr "Url"
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr "Titel"
 
@@ -4347,27 +4405,27 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 #, fuzzy
 #| msgid "YouTube Downloader"
 msgid "Quit YouTube Downloader"
 msgstr "YouTube Downloader"
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 #, fuzzy
 #| msgid "Exit\tCtrl+Q"
 msgid "Paste\tCtrl+V"
 msgstr "Afsluiten\tCtrl+Q"
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 #, fuzzy
 #| msgid "Remove the selected file from the list"
 msgid "Remove the selected URL from the list"
@@ -4389,15 +4447,15 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 #, fuzzy
 #| msgid "Shows the latest version available on github.com"
 msgid "Check the latest version available on github.com"
 msgstr "Toont de laatst beschikbare versie op github.com"
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr "Stel een tijdelijke folder in voor downloads"
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr "Bewaar alle downloads in deze tijdelijke locatie"
 
@@ -4515,21 +4573,29 @@
 msgid ""
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr ""
 "PAS OP: De gekozen URL verwijst NIET naar een afspeellijst. Alleen de groen "
 "gemarkeerde kunnen worden geindexeerd."
 
-#: ../vdms_ytdlp/textdrop.py:74
+#: ../vdms_ytdlp/textdrop.py:68
 #, fuzzy
 #| msgid "Invalid URL: \"{}\""
-msgid "Invalid URL:"
+msgid "Invalid URL"
 msgstr "Ongeldige URL: \"{}\""
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:84
+msgid "List of rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:87
+msgid "Rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr ""
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 msgid "Statistics viewer"
 msgstr "Statistieken viewer"
 
@@ -4638,14 +4704,30 @@
 msgid "The URLs contain playlists. Are you sure you want to continue?"
 msgstr "De URLs bevatten playlists. Wilt u toch doorgaan?"
 
 #: ../vdms_ytdlp/youtubedl_ui.py:659
 msgid "The URLs contain channels. Are you sure you want to continue?"
 msgstr "De URLs bevatten kanalen. Wilt u toch doorgaan?"
 
+#~ msgid ""
+#~ "Already exist: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Do you want to overwrite? "
+#~ msgstr ""
+#~ "Bestaat reeds: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Overschrijven? "
+
+#~ msgid "Duplicate files are rejected: > {}"
+#~ msgstr "Gelijke bestanden zijn overgeslagen: > {}"
+
 #~ msgid "File list changed, please check the settings again."
 #~ msgstr "Bestanden-lijst gewijzigd, ga a.u.b. de instellingen na."
 
 #~ msgid ""
 #~ "Cannot continue: The duration in the timeline exceeds the duration of "
 #~ "some queued files."
 #~ msgstr ""
@@ -4786,17 +4868,14 @@
 #~ msgid ""
 #~ "Make sure you are using the latest available version of\n"
 #~ "'{}'. This allows you to avoid download problems.\n"
 #~ msgstr ""
 #~ "Ga na of u de nieuwste '{}' versie gebruikt.\n"
 #~ "Dit voorkomt download problemen.\n"
 
-#~ msgid "Not found"
-#~ msgstr "Niet gevonden"
-
 #~ msgid "Not Installed"
 #~ msgstr "Niet geïnstalleerd"
 
 #~ msgid "Downloader"
 #~ msgstr "Downloader"
 
 #~ msgid "Topic List..."
@@ -4943,19 +5022,14 @@
 
 #, fuzzy
 #~| msgid "Duration"
 #~ msgid "Duration minutes"
 #~ msgstr "Duur"
 
 #, fuzzy
-#~| msgid "Duration"
-#~ msgid "Duration seconds"
-#~ msgstr "Duur"
-
-#, fuzzy
 #~| msgid "Starts"
 #~ msgid "Start hours"
 #~ msgstr "Start"
 
 #~ msgid "Show panel for editing timeline (seek/duration)"
 #~ msgstr "Toon panel voor tijdslijn edit (zoek/duur)"
 
@@ -5369,17 +5443,14 @@
 #~ msgstr "Uitgezet"
 
 #, fuzzy
 #~| msgid "Successful! youtube-dl is up-to-date"
 #~ msgid "Successful! {} is up-to-date"
 #~ msgstr "Succesvol! youtube-dl is up-to-date"
 
-#~ msgid "Disable youtube-dl"
-#~ msgstr "Deactiveer youtube-dl"
-
 #~ msgid "Enable youtube-dl"
 #~ msgstr "Activeer youtube-dl"
 
 #~ msgid "youtube-dl"
 #~ msgstr "youtube-dl"
 
 #~ msgid "Update youtube-dl"
```

### Comparing `videomass-5.0.0/videomass/locale/pt_BR/LC_MESSAGES/videomass.mo` & `videomass-5.0.1/videomass/locale/pt_BR/LC_MESSAGES/videomass.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-10 14:35+0200\n"
+"PO-Revision-Date: 2023-04-18 21:44+0200\n"
 "Last-Translator: Samuel / http://littlesvr.ca/ostd/\n"
 "Language-Team: Portuguese (Brasilian)\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "X-Generator: Poedit 2.4.2\n"
@@ -951,14 +951,17 @@
 
 msgid "Normalization"
 msgstr "Normalização"
 
 msgid "Not everything was successful."
 msgstr "Nem tudo foi bem-sucedido."
 
+msgid "Not found"
+msgstr "Não encontrado"
+
 msgid "Numerator"
 msgstr "Numerador"
 
 msgid "Off"
 msgstr "Desligado"
 
 msgid "Offset dBFS"
@@ -1332,17 +1335,14 @@
 
 msgid "Shows available decoders for FFmpeg"
 msgstr "Mostra os decodificadores disponíveis para FFmpeg"
 
 msgid "Shows available encoders for FFmpeg"
 msgstr "Mostra os codificadores disponíveis para FFmpeg"
 
-msgid "Shows the text in the toolbar buttons"
-msgstr "Mostra o texto nos botões da barra de ferramentas"
-
 msgid "Shows the version in use"
 msgstr "Mostrar a versão em uso"
 
 msgid "Simple interlacing filter from progressive contents."
 msgstr "Filtro de entrelaçamento simples de conteúdos progressivos."
 
 msgid "Size"
```

### Comparing `videomass-5.0.0/videomass/locale/pt_BR/LC_MESSAGES/videomass.po` & `videomass-5.0.1/videomass/locale/pt_BR/LC_MESSAGES/videomass.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Portuguese (Brazil) (pt_BR) translation of videomass.pot
 # Generated 2021-03-31 23:51 using the Open Source Translation Database
 # http://littlesvr.ca/ostd/
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
-"PO-Revision-Date: 2023-04-10 14:35+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
+"PO-Revision-Date: 2023-04-18 21:44+0200\n"
 "Last-Translator: Samuel / http://littlesvr.ca/ostd/\n"
 "Language-Team: Portuguese (Brasilian)\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "X-Generator: Poedit 2.4.2\n"
@@ -36,20 +36,20 @@
 #, python-brace-format
 msgid ""
 "Unexpected error while deleting file contents:\n"
 "\n"
 "{0}"
 msgstr ""
 
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr "Resetar"
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -107,72 +107,72 @@
 
 #: ../vdms_dialogs/epilogue.py:100
 #, fuzzy
 #| msgid "Cache Settings"
 msgid "Confirm Settings"
 msgstr "Configurações de cache"
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr "Tamanho da fonte: {0} x {1} pixels"
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 msgid "Search for a specific frame"
 msgstr "Procure por um quadro específico"
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr "Carregar"
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr "Seleção da área de corte "
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr "Altura"
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr "Centralizar"
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr "Largura"
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr "Aplicar"
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr "Filtro de corte"
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr "Cortar na largura"
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr "Mover verticalmente - defina como -1 para centralizar o eixo vertical"
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr ""
 "Mova horizontalmente - defina como -1 para centralizar o eixo horizontal"
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr "Cortar na altura"
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr "Opções Avançadas"
 
@@ -310,16 +310,16 @@
 "Este é um filtro de redução de ruído 3D, de alta precisão / qualidade. Seu "
 "objetivo é reduzir o ruído da imagem, produzindo imagens suaves e tornando "
 "as imagens estáticas realmente estáticas. Isso deve aumentar a "
 "compressibilidade."
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 #, fuzzy
 #| msgid "Ready"
 msgid "Read me"
 msgstr "Pronto"
 
@@ -416,14 +416,20 @@
 msgid "Create a snapshot"
 msgstr "Crie uma nova predefinição"
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr "Pré-visualizar"
 
+#: ../vdms_dialogs/filter_stab.py:110
+#, fuzzy
+#| msgid "Duration"
+msgid "Duration seconds:"
+msgstr "Duração"
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr "Detecção de vídeo"
 
 #: ../vdms_dialogs/filter_stab.py:177
 msgid "[TRIPOD] Enable tripod mode if checked"
 msgstr "[TRIPÉ] Ative o modo tripé se estiver marcado"
@@ -801,16 +807,16 @@
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 "\"ffmpeg\", \"ffprobe\" e \"ffplay\" são obrigatórios. Complete tudo\n"
 "nas caixas de texto abaixo clicando nos respectivos botões."
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr "Escolha o {} executável"
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 #, fuzzy
 #| msgid ""
 #| "Videomass has a simple graphical\n"
@@ -1039,179 +1045,209 @@
 msgid "Miscellanea"
 msgstr ""
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr "Onde você prefere salvar suas transcodificações?"
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 #, fuzzy
 #| msgid ""
 #| "Save each file in the same\n"
 #| "folder as input file"
 msgid "Save each file in the same folder as input file"
 msgstr ""
 "Salve cada arquivo na mesmo\n"
 "pasta como um arquivo de entrada"
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr "Atribua um sufixo opcional para nomes de arquivo de saída:"
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr "Onde você prefere salvar seus Downloads?"
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 #, fuzzy
 #| msgid ""
 #| "Auto-create subfolders\n"
 #| "when downloading playlists"
 msgid "Auto-create subfolders when downloading playlists"
 msgstr ""
 "Criar subpastas automaticamente\n"
 "ao baixar listas de reprodução"
 
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr "Preferências de arquivo"
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr "Caminho para os executáveis"
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr "Habilite outro local para executar o FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr "Habilite outro local para executar o FFprobe"
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr "Habilite outro local para executar o FFplay"
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr "Outras opções"
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr "Tópicos usados para transcodificação (de 0 a 32):"
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:288
+#, fuzzy
+#| msgid "Disable youtube-dl"
+msgid "Enable/Disable yt-dlp"
+msgstr "Desativar youtube-dl"
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr "Tema de ícones"
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 #, fuzzy
 #| msgid ""
 #| "setting the icons will also change the background\n"
 #| "and foreground of some text fields."
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "definir os ícones também mudará o fundo\n"
 "e primeiro plano de alguns campos de texto."
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr "Personalização da barra de ferramentas"
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr "No topo da janela (padrão)"
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr "Na parte inferior da janela"
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr "À direita da janela"
 
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr "À esquerda da janela"
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 msgid "Place the toolbar"
 msgstr "Coloque a barra de ferramentas"
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr "Tamanho dos ícones:"
 
-#: ../vdms_dialogs/preferences.py:349
-msgid "Shows the text in the toolbar buttons"
+#: ../vdms_dialogs/preferences.py:378
+#, fuzzy
+#| msgid "Shows the text in the toolbar buttons"
+msgid "Shows text in the toolbar buttons"
 msgstr "Mostra o texto nos botões da barra de ferramentas"
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 msgid "Appearance"
 msgstr "Aparência"
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 "As configurações a seguir afetam as mensagens de saída e\n"
 "as mensagens de log durante os processos de transcodificação.\n"
 "Mude apenas se você souber o que está fazendo.\n"
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr "Níveis de registro FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr "Configurações"
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr ""
 "Ao atribuir um sufixo adicional, você pode evitar a substituição de arquivos"
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 msgid "Set a persistent location to save exported files"
 msgstr "Defina um local persistente para salvar os arquivos exportados"
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 "Insira apenas caracteres alfanuméricos. Você também pode usar o hífen (\"-"
 "\") e o sublinhado (\"_\"). Espaços em branco não são permitidos."
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 #, fuzzy
 #| msgid "Choose a temporary destination for downloads"
 msgid "Choose a new destination for the files to be trashed"
 msgstr "Escolha um destino temporário para downloads"
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 msgid "Set a persistent location to save the file downloads"
 msgstr "Defina um local persistente para salvar os downloads de arquivos"
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 #, fuzzy
 #| msgid "Show the latest version..."
 msgid "Get Latest Version"
@@ -1263,15 +1299,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr "SELEÇÃO DE ARQUIVOS"
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 #, fuzzy
 #| msgid "Audio Properties"
 msgid "Properties"
 msgstr "Propriedades do Áudio"
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
@@ -1836,64 +1872,64 @@
 msgid "Seconds"
 msgstr ""
 
 #: ../vdms_miniframes/timeline.py:108
 msgid "Milliseconds"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 #, fuzzy
 #| msgid "Starts"
 msgid "Start adjustment"
 msgstr "Inicia"
 
-#: ../vdms_miniframes/timeline.py:320
+#: ../vdms_miniframes/timeline.py:322
 #, fuzzy
 #| msgid "Duration"
 msgid "Source duration:"
 msgstr "Duração"
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 #, fuzzy
 #| msgid "Starts"
 msgid "Start"
 msgstr "Inicia"
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 #, fuzzy
 #| msgid "Enabled"
 msgid "End"
 msgstr "Ativado"
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1906,62 +1942,47 @@
 "duration of a selected source file (see status bar messages).\n"
 "\n"
 "The \"Start\"/\"End\" duration values always refer to the initial position "
 "of the timeline: 00:00:00.000. For other informations as the segment "
 "duration and warnings, please refer to the status bar messages."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:559
+#: ../vdms_miniframes/timeline.py:566
 #, fuzzy
 #| msgid "Show timeline\tCtrl+T"
 msgid "Timeline Editor Usage"
 msgstr "Mostrar linha do tempo\tCtrl+T"
 
-#: ../vdms_io/checkup.py:45
+#: ../vdms_io/checkup.py:47
 #, fuzzy
-#| msgid ""
-#| "Already exist: \n"
-#| "\n"
-#| "%s\n"
-#| "\n"
-#| "Do you want to overwrite? "
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
+#| msgid "A file with this name already exists, do you want to overwrite it?"
+msgid "Files already exist, do you want to overwrite them?"
+msgstr "Já existe um arquivo com este nome, deseja substituí-lo?"
+
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
 msgstr ""
-"Já existe:\n"
-"\n"
-"% s\n"
-"\n"
-"Você deseja substituir? "
 
-#: ../vdms_io/checkup.py:48
+#: ../vdms_io/checkup.py:50
 msgid "Please Confirm"
 msgstr "Por favor confirme"
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-#, fuzzy
-#| msgid ""
-#| "File does not exist:\n"
-#| "\n"
-#| "\"%s\"\n"
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
+#: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
 msgstr ""
-"Arquivo não existe:\n"
-"\n"
-"\"% s\"\n"
 
-#: ../vdms_io/checkup.py:62
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr "Não encontrado"
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr ""
+
+#: ../vdms_io/checkup.py:75
 #, fuzzy
 #| msgid ""
 #| "Output folder does not exist:\n"
 #| "\n"
 #| "\"%s\"\n"
 msgid ""
 "Output folder does not exist:\n"
@@ -2046,18 +2067,18 @@
 "and try to click the \"Restore all...\" button"
 msgstr ""
 "Nenhuma predefinição encontrada.\n"
 "\n"
 "Solução possível: abra o painel Gerenciador de predefinições, vá para a "
 "coluna de predefinições e tente clicar no botão \"Restaurar tudo ...\""
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr "Pronto"
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 #, fuzzy
 #| msgid ""
 #| "There are still processes running.. if you want to stop them, use the "
@@ -2069,27 +2090,27 @@
 "\" button."
 msgstr ""
 "Ainda há processos em execução .. se quiser pará-los, use o botão \"Encerrar"
 "\".\n"
 "\n"
 "Você quer encerrar o aplicativo?"
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr "Videomass"
 
 #: ../vdms_main/main_frame.py:350
 #, fuzzy
 #| msgid "Are you sure you want to exit?"
 msgid "Are you sure you want to exit the application?"
 msgstr "Você tem certeza que deseja sair?"
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr "Sair"
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -2300,15 +2321,15 @@
 
 #: ../vdms_main/main_frame.py:520
 #, fuzzy
 #| msgid "Home panel\tShift+H"
 msgid "Home panel\tCtrl+Shift+H"
 msgstr "Painel inicial\tShift+H"
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 #, fuzzy
 #| msgid "Go to the next panel"
 msgid "Go to the 'Home' panel"
 msgstr "Vá para o próximo painel"
 
 #: ../vdms_main/main_frame.py:524
 #, fuzzy
@@ -2390,15 +2411,15 @@
 msgid "Keeps track of the output for debugging errors"
 msgstr "Mantém o controle da saída para erros de depuração"
 
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr "Ir para"
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr "Configure uma pasta temporária para conversões"
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr "Use um local temporário para salvar conversões"
 
@@ -2514,203 +2535,203 @@
 
 #: ../vdms_main/main_frame.py:677
 #, fuzzy
 #| msgid "Delete the selected profile"
 msgid "Open the selected files"
 msgstr "Exclua o perfil selecionado"
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 #, fuzzy
 #| msgid "Log folder"
 msgid "No such folder '{}'"
 msgstr "Pasta de log"
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 #, fuzzy
 #| msgid "Are you sure you want to exit?"
 msgid "Are you sure to empty trash folder?"
 msgstr "Você tem certeza que deseja sair?"
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 #, fuzzy
 #| msgid "No file selected"
 msgid "No files to delete"
 msgstr "Nenhum arquivo selecionado"
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr "Escolha uma pasta de download"
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 #, fuzzy
 #| msgid ""
 #| "\n"
 #| "Wait....\n"
 #| "The archive is being downloaded\n"
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 "\n"
 "Aguarde....\n"
 "O arquivo está sendo baixado\n"
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr "Download com sucesso para \"{0}\""
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr "Escolha um destino temporário para conversões"
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 msgid "Default destination folders successfully restored"
 msgstr "Pastas de destino padrão restauradas com sucesso"
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 #, fuzzy
 #| msgid "Changes will take effect once the program has been restarted"
 msgid "Changes will take effect once the program has been restarted."
 msgstr "As alterações entrarão em vigor assim que o programa for reiniciado"
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 #, fuzzy
 #| msgid "Changes will take effect once the program has been restarted"
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr "As alterações entrarão em vigor assim que o programa for reiniciado"
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, fuzzy, python-brace-format
 #| msgid "There is a new version available {0}"
 msgid "A new release is available - v.{0}\n"
 msgstr "Há uma nova versão disponível {0}"
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 #, fuzzy
 #| msgid "You are using youtube-dl version {}"
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr "Você está usando a versão youtube-dl {}"
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr "Vá para o painel anterior"
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr "Voltar"
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr "Vá para o próximo painel"
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 msgid "Next"
 msgstr "Avançar"
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 #, fuzzy
 #| msgid "Play the selected files in the list"
 msgid "Play the selected file in the list"
 msgstr "Reproduza os arquivos selecionados na lista"
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr "Reproduzir"
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 #, fuzzy
 #| msgid "Gathers information of multimedia streams"
 msgid "Get informative data about imported media streams"
 msgstr "Reúne informações de fluxos de multimídia"
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 #, fuzzy
 #| msgid "Starts"
 msgid "Start rendering"
 msgstr "Inicia"
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr "Para o processo atual"
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr "Cancelar"
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr "Exclua todos os arquivos da lista"
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 msgid "Videomass - Queued Files"
 msgstr "Videomass - arquivos enfileirados"
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr "Videomass - Conversões AV"
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr "Videomass - Gerenciador de predefinições"
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 msgid "Videomass - Concatenate Demuxer"
 msgstr "Videomass - Concatenate Demuxer"
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 #, fuzzy
 #| msgid "Videomass - Output Monitor"
 msgid "Videomass - From Movie to Pictures"
 msgstr "Videomass - Monitor de Saída"
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 #, fuzzy
 #| msgid "Videomass - Presets Manager"
 msgid "Videomass - Still Image Maker"
 msgstr "Videomass - Gerenciador de predefinições"
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr "Visualizando o último log"
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr "Processando..."
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 #, fuzzy
 #| msgid "Videomass - Output Monitor"
 msgid "Videomass - FFmpeg message monitor"
 msgstr "Videomass - Monitor de Saída"
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
@@ -3067,20 +3088,20 @@
 msgid "{} file in queue"
 msgstr "% s arquivo na fila"
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr "Desligado"
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr "Não definido"
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr "iniciar {} | duração {}"
 
 #: ../vdms_panels/av_conversions.py:2261
 #, fuzzy
 #| msgid ""
@@ -3366,15 +3387,15 @@
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 
 #: ../vdms_panels/choose_topic.py:223
 #, fuzzy
 #| msgid "youtube-dl is disabled. Check your preferences."
-msgid "The downloader is disabled. Check your preferences."
+msgid "yt-dlp is disabled. Check your preferences."
 msgstr "youtube-dl está desativado. Verifique suas preferências."
 
 #: ../vdms_panels/concatenate.py:78
 #, fuzzy
 #| msgid ""
 #| "NOTE:\n"
 #| "\n"
@@ -3502,124 +3523,132 @@
 "\n"
 "Arquivo para unir\n"
 "Nome do arquivo de saída\n"
 "Destino\n"
 "Formato de saída\n"
 "Período de tempo"
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 #, fuzzy
 #| msgid "Invalid filename. Contains double quotes"
 msgid "Invalid path name. Contains double or single quotes"
 msgstr "Nome de arquivo inválido. Contém aspas duplas"
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 msgid "Directories are not allowed, just add files, please."
 msgstr "Diretórios não são permitidos, apenas adicione arquivos, por favor."
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 "Arquivo sem extensão de formato: forneça uma extensão apropriada para o nome "
 "do arquivo, por exemplo '.mkv', '.avi', '.mp3', etc."
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr "Nome do arquivo"
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr "Duração"
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr "Tipo de mídia"
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr "Tamanho"
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 #, fuzzy
 #| msgid "Output index:"
 msgid "Output file name"
 msgstr "Índice de saída:"
 
-#: ../vdms_panels/filedrop.py:207
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:209
 #, fuzzy
-#| msgid "Duplicate files are rejected: > '%s'"
-msgid "Duplicate files are rejected: > {}"
-msgstr "Arquivos duplicados são rejeitados:> '% s'"
+#| msgid "Add Files"
+msgid "Rejected Files"
+msgstr "Adicionar arquivos"
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr "Arraste um ou mais arquivos abaixo"
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 msgid "Destination folder"
 msgstr "Diretório de destino"
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag the images below"
 msgstr "Arraste um ou mais arquivos abaixo"
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag one or more video below"
 msgstr "Arraste um ou mais arquivos abaixo"
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 msgid "No file selected"
 msgstr "Nenhum arquivo selecionado"
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 #, fuzzy
 #| msgid "File name"
 msgid "File renaming..."
 msgstr "Nome do Arquivo"
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 #, fuzzy
 #| msgid "Delete the selected profile"
 msgid "Rename the selected file to:"
 msgstr "Exclua o perfil selecionado"
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr "Adicionar arquivos"
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 #, fuzzy
 #| msgid "File Name"
 msgid "New Name #"
 msgstr "Nome do arquivo"
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
@@ -4042,19 +4071,19 @@
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 "O comando de perfil selecionado foi alterado manualmente.\n"
 "Quer aplicá-lo durante o processo de conversão?"
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 msgid "Don't show this dialog again"
 msgstr "Não mostrar esta caixa de diálogo novamente"
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 #, fuzzy
 #| msgid ""
 #| "SUMMARY\n"
 #| "\n"
 #| "Queued File\n"
 #| "Pass Encoding                     \n"
 #| "Profile Used\n"
@@ -4082,26 +4111,28 @@
 #: ../vdms_panels/sequence_to_video.py:74
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 
 #: ../vdms_panels/sequence_to_video.py:129
 msgid "Enable a single still image"
 msgstr ""
 
 #: ../vdms_panels/sequence_to_video.py:161
@@ -4160,14 +4191,30 @@
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 #, fuzzy
 #| msgid "Supported Format List"
 msgid "Unsupported format '{}'"
 msgstr "Lista de formatos suportados"
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+#, fuzzy
+#| msgid ""
+#| "File does not exist:\n"
+#| "\n"
+#| "\"%s\"\n"
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+"Arquivo não existe:\n"
+"\n"
+"\"% s\"\n"
+
 #: ../vdms_panels/sequence_to_video.py:719
 #, fuzzy
 #| msgid ""
 #| "SUMMARY\n"
 #| "\n"
 #| "Queued File\n"
 #| "Output Format                        \n"
@@ -4294,24 +4341,24 @@
 
 #: ../vdms_panels/video_to_sequence.py:49
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 
 #: ../vdms_panels/video_to_sequence.py:84
 msgid "Create thumbnails"
 msgstr ""
 
 #: ../vdms_panels/video_to_sequence.py:85
@@ -4381,15 +4428,15 @@
 "Pelo menos um \"Código de formato\" deve ser verificado para cada URL "
 "selecionado em verde."
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr "Código de Formato"
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr "Url"
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr "Título"
 
@@ -4474,25 +4521,25 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 #, fuzzy
 #| msgid "YouTube Downloader"
 msgid "Quit YouTube Downloader"
 msgstr "Baixar vídeos"
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 msgid "Paste\tCtrl+V"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 #, fuzzy
 #| msgid "Remove the selected file from the list"
 msgid "Remove the selected URL from the list"
@@ -4514,15 +4561,15 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 #, fuzzy
 #| msgid "Shows the latest version available on github.com"
 msgid "Check the latest version available on github.com"
 msgstr "Mostra a versão mais recente disponível em github.com"
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr "Configure uma pasta temporária para downloads"
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr "Salve todos os downloads neste local temporário"
 
@@ -4634,21 +4681,29 @@
 
 #: ../vdms_ytdlp/playlist_indexing.py:256
 msgid ""
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr ""
 
-#: ../vdms_ytdlp/textdrop.py:74
+#: ../vdms_ytdlp/textdrop.py:68
 #, fuzzy
 #| msgid "Invalid URL: \"{}\""
-msgid "Invalid URL:"
+msgid "Invalid URL"
 msgstr "URL inválido: \"{}\""
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:84
+msgid "List of rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:87
+msgid "Rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr ""
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 msgid "Statistics viewer"
 msgstr "Visualizador de estatísticas"
 
@@ -4762,14 +4817,39 @@
 msgstr ""
 "Os URLs contêm listas de reprodução. Você tem certeza que quer continuar?"
 
 #: ../vdms_ytdlp/youtubedl_ui.py:659
 msgid "The URLs contain channels. Are you sure you want to continue?"
 msgstr "Os URLs contêm canais . Você tem certeza que quer continuar?"
 
+#, fuzzy
+#~| msgid ""
+#~| "Already exist: \n"
+#~| "\n"
+#~| "%s\n"
+#~| "\n"
+#~| "Do you want to overwrite? "
+#~ msgid ""
+#~ "Already exist: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Do you want to overwrite? "
+#~ msgstr ""
+#~ "Já existe:\n"
+#~ "\n"
+#~ "% s\n"
+#~ "\n"
+#~ "Você deseja substituir? "
+
+#, fuzzy
+#~| msgid "Duplicate files are rejected: > '%s'"
+#~ msgid "Duplicate files are rejected: > {}"
+#~ msgstr "Arquivos duplicados são rejeitados:> '% s'"
+
 #~ msgid "File list changed, please check the settings again."
 #~ msgstr "Lista de arquivos alterada, verifique as configurações novamente."
 
 #~ msgid ""
 #~ "Cannot continue: The duration in the timeline exceeds the duration of "
 #~ "some queued files."
 #~ msgstr ""
@@ -4902,17 +4982,14 @@
 #~ msgid ""
 #~ "Make sure you are using the latest available version of\n"
 #~ "'{}'. This allows you to avoid download problems.\n"
 #~ msgstr ""
 #~ "Certifique-se de que está usando a versão mais recente disponível do\n"
 #~ "youtube-dl. Isso permite evitar problemas de download.\n"
 
-#~ msgid "Not found"
-#~ msgstr "Não encontrado"
-
 #~ msgid "Not Installed"
 #~ msgstr "Não Instalado"
 
 #, fuzzy
 #~| msgid "Download"
 #~ msgid "Downloader"
 #~ msgstr "Download"
@@ -5051,19 +5128,14 @@
 
 #, fuzzy
 #~| msgid "Duration"
 #~ msgid "Duration minutes"
 #~ msgstr "Duração"
 
 #, fuzzy
-#~| msgid "Duration"
-#~ msgid "Duration seconds"
-#~ msgstr "Duração"
-
-#, fuzzy
 #~| msgid "Starts"
 #~ msgid "Start hours"
 #~ msgstr "Inicia"
 
 #~ msgid "Show panel for editing timeline (seek/duration)"
 #~ msgstr "Mostrar painel para edição da linha do tempo (busca / duração)"
 
@@ -5480,17 +5552,14 @@
 #~ msgstr "Desabilitado"
 
 #, fuzzy
 #~| msgid "Successful! youtube-dl is up-to-date"
 #~ msgid "Successful! {} is up-to-date"
 #~ msgstr "Bem sucedido! youtube-dl está atualizado"
 
-#~ msgid "Disable youtube-dl"
-#~ msgstr "Desativar youtube-dl"
-
 #~ msgid "Enable youtube-dl"
 #~ msgstr "Habilitar youtube-dl"
 
 #~ msgid "youtube-dl"
 #~ msgstr "youtube-dl"
 
 #~ msgid "Update youtube-dl"
```

### Comparing `videomass-5.0.0/videomass/locale/ru_RU/LC_MESSAGES/videomass.mo` & `videomass-5.0.1/videomass/locale/ru_RU/LC_MESSAGES/videomass.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-11 14:33+0200\n"
+"PO-Revision-Date: 2023-04-18 21:44+0200\n"
 "Last-Translator: ChourS <ChourS2008@yandex.ru>\n"
 "Language-Team: Russian (RU)\n"
 "Language: ru_RU\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -75,86 +75,90 @@
 "- Имя выходного файла будет таким же, как у первого добавленного файла\n"
 " (также зависит от настроек, сделанных в диалоговом окне настроек,\n"
 "  или от используемых функций переименования).\n"
 "\n"
 "- Видеофайлы должны иметь одинаковые потоки, одинаковые кодеки и одинаковые\n"
 "  ширину/высоту, но может быть упакован в разные форматы контейнеров.\n"
 "\n"
-"- Аудиофайлы должны иметь одинаковые форматы, одинаковые кодеки с одинаковой "
-"частотой дискретизации."
+"- Аудиофайлы должны иметь одинаковые форматы, одинаковые кодеки \n"
+"  с одинаковой частотой дискретизации."
 
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 "\n"
-"1. Импортируйте один или несколько файлов изображений, таких как форматы "
-"JPG, PNG и BMP, затем выберите один из них.\n"
+"1. Импортируйте один или несколько файлов изображений, \n"
+"  таких как форматы JPG, PNG и BMP, затем выберите один.\n"
+"\n"
+"2. Используйте функцию изменения размера, чтобы изменить \n"
+"  размер изображений, которые имеют разные размеры, такие \n"
+"  как ширина и высота. В других случаях это необязательно.\n"
 "\n"
-"2. Используйте функцию изменения размера, чтобы изменить размер изображений, "
-"которые имеют разные размеры, такие как ширина и высота. В других случаях "
-"это необязательно.\n"
-"\n"
-"3. Используйте редактор Timeline (CTRL+T), чтобы установить временной "
-"интервал между изображениями, отрегулировав значение продолжительности "
-"«Конец» \n"
-"и оставив значение «Начало» равным 00:00:00.000.\n"
+"3. Используйте редактор временной шкалы (CTRL+T), чтобы установить \n"
+"  временной интервал между изображениями, регулируя значение \n"
+"  времени «Конец» и оставить значение «Начало» равным 00:00:00.000.\n"
 "\n"
 "4. Запустите преобразование.\n"
 "\n"
 "\n"
-"Созданное видео будет иметь имя выбранного файла в списке «Файл в очереди», "
-"который будет сохранен в папке с именем «Still_Images» \n"
+"Созданное видео будет иметь имя выбранного файла в списке «Файл в "
+"очереди», \n"
+"которые будут сохранены в папке с именем «Still_Images» \n"
 "с прогрессивной цифрой по указанному вами пути."
 
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 "\n"
-"1. Импортируйте один или несколько видеофайлов, затем выберите один.\n"
+"1. Импортируйте один или несколько видеофайлов, \n"
+"    затем выберите один.\n"
 "\n"
-"2. Чтобы выбрать отрезок времени, используйте редактор временной шкалы "
-"(CTRL+T), настроив значения длительности «Конец» и «Начало».\n"
+"2. Чтобы выбрать отрезок времени, используйте редактор \n"
+"    Timeline (CTRL+T), отрегулировав\n"
+"    Значения длительности «Конец» и «Начало».\n"
 "\n"
 "3. Выберите выходной формат (jpg, png, bmp).\n"
 "\n"
 "4. Запустите преобразование.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"Созданные изображения будут сохранены в папке \n"
+"с именем 'Movie_to_Pictures'\n"
+"с прогрессивной цифрой по указанному вами пути."
 
 msgid " Do you want to enable this feature?"
 msgstr " Вы хотите включить эту функцию?"
 
 msgid ""
 "\"Auto\" keeps all audio stream but processes only the one of the selected "
 "index; \"All\" keeps all audio streams and processes them all with the "
@@ -390,27 +394,14 @@
 msgid "All default presets have been successfully recovered"
 msgstr "Все пресеты по умолчанию были успешно восстановлены"
 
 msgid "All presets have been exported successfully"
 msgstr "Все пресеты успешно экспортированы"
 
 msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
-msgstr ""
-"Уже существующие файлы: \n"
-"\n"
-"{}\n"
-"\n"
-"Вы хотите перезаписать? "
-
-msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 "Всегда перемещать исходные файлы в корзину Videomass \n"
 "после успешного преобразования"
 
 msgid "Appearance"
@@ -1016,16 +1007,16 @@
 "page"
 msgstr ""
 "Загрузите всю коллекцию последних пресетов, доступных на главной странице"
 
 msgid "Download videos by resolution"
 msgstr "Загрузка видео по разрешению"
 
-msgid "Download videos from YouTube.com and other video sites "
-msgstr "Скачивайте видео с YouTube.com и других видеосайтов "
+msgid "Download videos from YouTube.com and other video sites"
+msgstr "Скачивайте видео с YouTube.com и других видеосайтов"
 
 msgid "Downloads folder\tCtrl+D"
 msgstr "Папка загрузок\tCtrl+D"
 
 msgid "Drag one or more files below"
 msgstr "Перетащите один или несколько файлов ниже"
 
@@ -1037,20 +1028,20 @@
 
 msgid "Drag the images below"
 msgstr "Перетащите изображения ниже"
 
 msgid "Duplicate"
 msgstr "Дублировать"
 
-msgid "Duplicate files are rejected: > {}"
-msgstr "Дубликаты файлов отклоняются: > {}"
-
 msgid "Duration"
 msgstr "Длина"
 
+msgid "Duration seconds:"
+msgstr "Продолжительность секунд:"
+
 msgid "Duration:"
 msgstr "Продолжительность:"
 
 msgid "ERROR"
 msgstr "ОШИБКА"
 
 msgid "ERROR: Invalid option"
@@ -1183,14 +1174,23 @@
 
 msgid "Export selected preset as copy"
 msgstr "Экспорт выбранного пресета как копии"
 
 msgid "Extension"
 msgstr "Расширение"
 
+msgid "External Downloader Preferences"
+msgstr "Настройки внешнего загрузчика"
+
+msgid "External downloader arguments"
+msgstr "Аргументы внешнего загрузчика"
+
+msgid "External downloader executable path"
+msgstr "Исполняемый путь внешнего загрузчика"
+
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 "Извлекайте изображения (кадры) из ваших фильмов в форматы JPG, PNG, BMP, GIF."
 
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
@@ -1480,20 +1480,19 @@
 msgid ""
 "If you want to keep the aspect ratio, select \"Constrain proportions\" below "
 "and\n"
 "specify only one dimension, either width or height, and set the other "
 "dimension\n"
 "to -1 or -2 (some codecs require -2, so you should do some testing first)."
 msgstr ""
-"Если вы хотите сохранить соотношение сторон, выберите «Сохранить пропорции» "
-"ниже и укажите только одно измерение,\n"
-"ширину или высоту, и установите для другого измерения значение -1 или -2 "
-"(для некоторых \n"
-"кодеков требуется -2, так что сначала вы должны провести некоторое "
-"тестирование)"
+"Если вы хотите сохранить соотношение сторон, выберите \n"
+"«Сохранить пропорции» ниже и укажите только одно измерение,\n"
+"ширину или высоту, и установите для другого измерения \n"
+"значение -1 или -2 (для некоторых кодеков требуется -2, \n"
+"так что сначала вы должны провести некоторое тестирование)"
 
 msgid ""
 "If you want to use a version of FFmpeg located on your\n"
 "filesystem but not installed on your operating system,\n"
 "click the \"Locate\" button."
 msgstr ""
 "Если вы хотите использовать версию FFmpeg, которая\n"
@@ -1527,14 +1526,29 @@
 
 msgid "Import group"
 msgstr "Импорт группы"
 
 msgid "Import preset"
 msgstr "Импортировать пресет"
 
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+"В дополнение к стандартному (собственному) yt-dlp \n"
+"в настоящее время поддерживаются следующие внешние загрузчики: \n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Обратите внимание, что если вы включите внешний загрузчик, \n"
+"вы не сможете просматривать индикатор выполнения во время \n"
+"операций загрузки."
+
 msgid "Include audio file"
 msgstr "Включить аудиофайл"
 
 msgid ""
 "Include the video ID\n"
 "in the file names"
 msgstr ""
@@ -1566,17 +1580,14 @@
 
 msgid "Interlaces with interlace filter"
 msgstr "Чересстрочная с фильтром 'interlace'"
 
 msgid "Interrupted Process !"
 msgstr "Процесс прерван !"
 
-msgid "Invalid URL:"
-msgstr "Неверный URL:"
-
 msgid "Invalid file: '{}'"
 msgstr "Недопустимый файл: '{}'"
 
 msgid ""
 "Invalid file: '{}'\n"
 "\n"
 "It doesn't appear to be an audio file."
@@ -1623,15 +1634,15 @@
 msgid "Issue tracker"
 msgstr "Сообщить о проблеме"
 
 msgid "It can reduce the file size, but takes longer."
 msgstr "Это может уменьшить размер файла, но занимает больше времени."
 
 msgid "Keeps track of the output for debugging errors"
-msgstr "Отслеживает вывод для ошибок отладки"
+msgstr "Отслеживает вывод для отладки ошибок"
 
 msgid "Latest version of yt-dlp"
 msgstr "Последняя версия yt-dlp"
 
 msgid ""
 "Limiter for the maximum peak level or the mean level (when switch to RMS) in "
 "dBFS. From -99.0 to +0.0; default for PEAK level is -1.0; default for RMS is "
@@ -1784,14 +1795,17 @@
 
 msgid "Normalization"
 msgstr "Нормализация"
 
 msgid "Not everything was successful."
 msgstr "Завершено, но не все прошло хорошо."
 
+msgid "Not found"
+msgstr "Не найдено"
+
 msgid "Numerator"
 msgstr "Числитель"
 
 msgid "OK: Indexes to download"
 msgstr "ОК: индексы для загрузки"
 
 msgid "Off"
@@ -2613,17 +2627,14 @@
 
 msgid "Shows available encoders for FFmpeg"
 msgstr "Показывает доступные кодировщики для FFmpeg"
 
 msgid "Shows statistics and information"
 msgstr "Показать статистику и информацию"
 
-msgid "Shows the text in the toolbar buttons"
-msgstr "Показывает текст на кнопках панели инструментов"
-
 msgid "Shows the version in use"
 msgstr "Показывает используемую версию"
 
 msgid "Simple interlacing filter from progressive contents."
 msgstr ""
 "Простой фильтр с чересстрочной разверткой из прогрессивного содержимого."
 
@@ -2831,17 +2842,14 @@
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "Выбранная тема значка изменит только значки, фон\n"
 "и передний план некоторых текстовых полей."
 
-msgid "The downloader is disabled. Check your preferences."
-msgstr "Загрузчик отключен. Проверьте свои настройки."
-
 msgid "The file is not a frame or a video file"
 msgstr "Файл не является кадром или видеофайлом"
 
 msgid ""
 "The files do not have the same \"codec_types\", same \"sample_rate\" or same "
 "\"width\" or \"height\". Unable to proceed."
 msgstr ""
@@ -3379,15 +3387,15 @@
 msgid "fps"
 msgstr "fps"
 
 msgid "help topic list"
 msgstr "список тем справки"
 
 msgid "hqdn3d options"
-msgstr "параметры фильтра hqdn3d"
+msgstr "Параметры фильтра hqdn3d"
 
 msgid ""
 "hqdn3d:\n"
 "This is a high precision/quality 3d denoise filter. It aims to reduce image "
 "noise, producing smooth images and making still images really still. It "
 "should enhance compressibility."
 msgstr ""
@@ -3408,19 +3416,19 @@
 "чтобы избежать чересстрочной развертки твиттера и уменьшить муаровые узоры.\n"
 "По умолчанию настройка отсутствует."
 
 msgid ""
 "mode\n"
 "The interlacing mode to adopt."
 msgstr ""
-"режим\n"
+"mode\n"
 "Используемый режим чересстрочной развертки."
 
 msgid "nlmeans options"
-msgstr "параметры фильтра nlmeans"
+msgstr "Параметры фильтра nlmeans"
 
 msgid ""
 "nlmeans:\n"
 "Denoise frames using Non-Local Means algorithm is capable of restoring video "
 "sequences, even with strong noise. It is ideal for enhancing the quality of "
 "old VHS tapes."
 msgstr ""
@@ -3484,15 +3492,15 @@
 "двойной щелчок левой кнопкой мыши"
 
 msgid ""
 "scan:\n"
 "determines whether the interlaced frame is taken from the even (tff - "
 "default) or odd (bff) lines of the progressive frame."
 msgstr ""
-"развертка:\n"
+"scan:\n"
 "определяет, взят ли чересстрочный кадр из четных (tff - по умолчанию) или "
 "нечетных (bff) строк прогрессивного кадра."
 
 msgid ""
 "specifies the target (average) bit rate for the encoder to use. Higher value "
 "= higher quality. Set -1 to disable this control."
 msgstr ""
```

### Comparing `videomass-5.0.0/videomass/locale/ru_RU/LC_MESSAGES/videomass.po` & `videomass-5.0.1/videomass/locale/ru_RU/LC_MESSAGES/videomass.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Russian translation for Videomass.
 # Copyleft -  2023 Gianluca Pernigotto
 # This file is distributed under the same license as the Videomass package
 # FIRST AUTHOR ChourS <chours2008@yandex.ru>, 2020.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
-"PO-Revision-Date: 2023-04-11 14:33+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
+"PO-Revision-Date: 2023-04-18 21:44+0200\n"
 "Last-Translator: ChourS <ChourS2008@yandex.ru>\n"
 "Language-Team: Russian (RU)\n"
 "Language: ru_RU\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
@@ -46,20 +46,20 @@
 "{0}"
 msgstr ""
 "Непредвиденная ошибка при удалении содержимого файла:\n"
 "\n"
 "{0}"
 
 # Перевод всех отмеченных изменений на значение по умолчанию
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr "Сброс"
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -119,71 +119,71 @@
 "Очистить список \n"
 "импортированных файлов"
 
 #: ../vdms_dialogs/epilogue.py:100
 msgid "Confirm Settings"
 msgstr "Подтвердить настройки"
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr "Размер источника: {0} x {1} пикселей"
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 msgid "Search for a specific frame"
 msgstr "Поиск определенного кадра"
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr "Загрузить"
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr "Выбор области обрезки "
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr "Высота"
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr "Центр"
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr "Ширина"
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr "Применить"
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr "Фильтр Обрезка"
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr "Обрезать по ширине"
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr "Вертикальное положение верхнего левого угла"
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr "Горизонтальное положение верхнего левого угла"
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr "Обрезать по высоте"
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr "Расширенные настройки"
 
@@ -233,15 +233,15 @@
 "это лучший и самый быстрый выбор"
 
 #: ../vdms_dialogs/filter_deinterlace.py:208
 msgid ""
 "mode\n"
 "The interlacing mode to adopt."
 msgstr ""
-"режим\n"
+"mode\n"
 "Используемый режим чересстрочной развертки."
 
 #: ../vdms_dialogs/filter_deinterlace.py:210
 msgid ""
 "parity\n"
 "The picture field parity assumed for the input interlaced video."
 msgstr ""
@@ -255,15 +255,15 @@
 
 #: ../vdms_dialogs/filter_deinterlace.py:217
 msgid ""
 "scan:\n"
 "determines whether the interlaced frame is taken from the even (tff - "
 "default) or odd (bff) lines of the progressive frame."
 msgstr ""
-"развертка:\n"
+"scan:\n"
 "определяет, взят ли чересстрочный кадр из четных (tff - по умолчанию) или "
 "нечетных (bff) строк прогрессивного кадра."
 
 #: ../vdms_dialogs/filter_deinterlace.py:221
 msgid ""
 "lowpass:\n"
 "Enable (default) or disable the vertical lowpass filter to avoid twitter "
@@ -279,25 +279,27 @@
 msgid "Apply Denoisers Filters"
 msgstr "Применить фильтры шумоподавления"
 
 #: ../vdms_dialogs/filter_denoisers.py:59
 msgid "Enable nlmeans denoiser"
 msgstr "Включить фильтр nlmeans"
 
+# Особенности русской фразы
 #: ../vdms_dialogs/filter_denoisers.py:66
 msgid "nlmeans options"
-msgstr "параметры фильтра nlmeans"
+msgstr "Параметры фильтра nlmeans"
 
 #: ../vdms_dialogs/filter_denoisers.py:71
 msgid "Enable hqdn3d denoiser"
 msgstr "Включить фильтр hqdn3d"
 
+# Особенности русской фразы
 #: ../vdms_dialogs/filter_denoisers.py:76
 msgid "hqdn3d options"
-msgstr "параметры фильтра hqdn3d"
+msgstr "Параметры фильтра hqdn3d"
 
 #: ../vdms_dialogs/filter_denoisers.py:123
 msgid "Denoiser filters"
 msgstr "Фильтры шумоподавления"
 
 #: ../vdms_dialogs/filter_denoisers.py:124
 msgid ""
@@ -322,16 +324,16 @@
 " Это высокоточный и качественный трехмерный шумоподавляющий фильтр. "
 "Стремится уменьшить шум изображения, создать плавные изображения и сделать "
 "статическиеизображения неподвижными. Понятно, что это должно улучшить "
 "визуальное качество."
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 msgid "Read me"
 msgstr "Прочти меня"
 
 #: ../vdms_dialogs/filter_scale.py:80
 msgid "View result"
@@ -401,20 +403,19 @@
 msgid ""
 "If you want to keep the aspect ratio, select \"Constrain proportions\" below "
 "and\n"
 "specify only one dimension, either width or height, and set the other "
 "dimension\n"
 "to -1 or -2 (some codecs require -2, so you should do some testing first)."
 msgstr ""
-"Если вы хотите сохранить соотношение сторон, выберите «Сохранить пропорции» "
-"ниже и укажите только одно измерение,\n"
-"ширину или высоту, и установите для другого измерения значение -1 или -2 "
-"(для некоторых \n"
-"кодеков требуется -2, так что сначала вы должны провести некоторое "
-"тестирование)"
+"Если вы хотите сохранить соотношение сторон, выберите \n"
+"«Сохранить пропорции» ниже и укажите только одно измерение,\n"
+"ширину или высоту, и установите для другого измерения \n"
+"значение -1 или -2 (для некоторых кодеков требуется -2, \n"
+"так что сначала вы должны провести некоторое тестирование)"
 
 #: ../vdms_dialogs/filter_stab.py:82
 msgid "Enable stabilizer"
 msgstr "Включить stabilizer"
 
 #: ../vdms_dialogs/filter_stab.py:84
 msgid "Create a side-by-side comparison video"
@@ -424,14 +425,18 @@
 msgid "Create a snapshot"
 msgstr "Создать снимок"
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr "Предпросмотр"
 
+#: ../vdms_dialogs/filter_stab.py:110
+msgid "Duration seconds:"
+msgstr "Продолжительность секунд:"
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr "Обнаружение видео"
 
 #: ../vdms_dialogs/filter_stab.py:177
 msgid "[TRIPOD] Enable tripod mode if checked"
 msgstr "[ШТАТИВ] Включите режим штатива, если установлен флажок"
@@ -795,16 +800,16 @@
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 "\"ffmpeg\", \"ffprobe\" и \"ffplay\" обязательны. Заполните все\n"
 "текстовые поля ниже, нажав соответствующие кнопки."
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr "Выберите исполняемый файл {}"
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 msgid "Videomass has a simple graphical interface for yt-dlp\n"
 msgstr "Videomass имеет простой графический интерфейс для yt-dlp\n"
 
@@ -1027,164 +1032,200 @@
 msgid "Miscellanea"
 msgstr "Разное"
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr "Где вы предпочитаете сохранять перекодировки?"
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 msgid "Save each file in the same folder as input file"
 msgstr "Сохраняет каждый файл в той же папке, что и входной файл"
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr "Добавить необязательный суффикс к именам выходных файлов:"
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 "Всегда перемещать исходные файлы в корзину Videomass \n"
 "после успешного преобразования"
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr "Где вы предпочитаете сохранять загрузки?"
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 msgid "Auto-create subfolders when downloading playlists"
 msgstr "Автоматически создавать подпапки при загрузке плейлистов"
 
 # Изменил 14-5-2021
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr "Файл"
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr "Путь к исполняемым файлам"
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr "Включить другое место для запуска FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr "Включить другое место для запуска FFprobe"
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr "Включить другое место для запуска FFplay"
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr "Другие опции"
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr "Потоки, используемые для перекодирования (от 0 до 32):"
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
-msgstr "Скачивайте видео с YouTube.com и других видеосайтов "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr "Скачивайте видео с YouTube.com и других видеосайтов"
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:288
+#, fuzzy
+#| msgid "Disable youtube-dl"
+msgid "Enable/Disable yt-dlp"
+msgstr "Отключить youtube-dl"
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr "Настройки внешнего загрузчика"
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+"В дополнение к стандартному (собственному) yt-dlp \n"
+"в настоящее время поддерживаются следующие внешние загрузчики: \n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Обратите внимание, что если вы включите внешний загрузчик, \n"
+"вы не сможете просматривать индикатор выполнения во время \n"
+"операций загрузки."
+
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
+msgstr "Исполняемый путь внешнего загрузчика"
+
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
+msgstr "Аргументы внешнего загрузчика"
+
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr "Темы значков"
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "Выбранная тема значка изменит только значки, фон\n"
 "и передний план некоторых текстовых полей."
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr "Настройка панели инструментов"
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr "Вверху (по умолчанию)"
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr "Внизу"
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr "Справа"
 
 # слева от окна или в левой части окна?
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr "Слева"
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 msgid "Place the toolbar"
 msgstr "Разместите панель инструментов"
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr "Размер значка:"
 
-#: ../vdms_dialogs/preferences.py:349
-msgid "Shows the text in the toolbar buttons"
-msgstr "Показывает текст на кнопках панели инструментов"
+#: ../vdms_dialogs/preferences.py:378
+#, fuzzy
+#| msgid "Shows the text in the toolbar buttons"
+msgid "Shows text in the toolbar buttons"
+msgstr "Показывать текст на кнопках панели инструментов"
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 msgid "Appearance"
 msgstr "Вид"
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 "Следующие настройки влияют на выходные сообщения и\n"
 "сообщения журнала во время процессов перекодирования.\n"
 "Изменяйте, только если знаете, что делаете.\n"
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr "Комплект log-журналов FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr "Настройки"
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr "Назначив дополнительный суффикс, вы можете избежать перезаписи файлов"
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 msgid "Set a persistent location to save exported files"
 msgstr "Установите постоянное место для сохранения экспортированных файлов"
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 "Вводите только буквенно-цифровые символы. Вы также можете использовать дефис "
 "(\"-\") и подчеркивание (\"_\"). Пробелы не допускаются."
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 msgid "Choose a new destination for the files to be trashed"
 msgstr "Выберите новое место для файлов, которые нужно удалить"
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 msgid "Set a persistent location to save the file downloads"
 msgstr "Установите постоянное место для сохранения скачанных файлов"
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 msgid "Get Latest Version"
 msgstr "Получить последнюю версию"
 
@@ -1237,15 +1278,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr "ВЫБОР ФАЙЛА"
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 msgid "Properties"
 msgstr "Характеристики"
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
 msgid "Values"
 msgstr "Значения"
@@ -1744,15 +1785,14 @@
 "двойной щелчок левой кнопкой мыши"
 
 #: ../vdms_dialogs/while_playing.py:92
 msgid "Shortcut keys while playing with FFplay"
 msgstr "Сочетания клавиш во время проигрывания с FFplay"
 
 #: ../vdms_miniframes/timeline.py:46
-#| msgid "Start minutes"
 msgid "Start point adjustment"
 msgstr "Регулировка точки \"Начало\""
 
 #: ../vdms_miniframes/timeline.py:48
 msgid "End point adjustment"
 msgstr "Регулировка точки \"Конец\""
 
@@ -1765,64 +1805,61 @@
 msgstr "Минуты"
 
 #: ../vdms_miniframes/timeline.py:107
 msgid "Seconds"
 msgstr "Секунды"
 
 #: ../vdms_miniframes/timeline.py:108
-#| msgid "Start milliseconds"
 msgid "Milliseconds"
 msgstr "Миллисекунды"
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr "Нет длительности источника:"
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr "{0} {1}  |  Продолжительность сегмента: {2}"
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr "Регулировка \"Конец\""
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
-#| msgid "Start minutes"
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 msgid "Start adjustment"
 msgstr "Регулировка \"Начало\""
 
-#: ../vdms_miniframes/timeline.py:320
-#| msgid "Saturation:"
+#: ../vdms_miniframes/timeline.py:322
 msgid "Source duration:"
 msgstr "Длительность источника:"
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr "WARNING: Неверный выбор, вне допустимого диапазона."
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 "Начните с перетаскивания нижнего левого маркера \n"
 "или щелкните правой кнопкой мыши для выбора параметров."
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 msgid "Start"
 msgstr "Начало"
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 msgid "End"
 msgstr "Конец"
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1855,49 +1892,45 @@
 "длительность выбранного исходного файла (см. сообщения в строке состояния).\n"
 "\n"
 "Значения продолжительности «Начало»/«Конец» всегда относятся к начальной "
 "позиции временной шкалы: 00:00:00.000. Для получения другой информации, "
 "такой как продолжительность сегмента и Warnings, см. сообщения в строке "
 "состояния."
 
-#: ../vdms_miniframes/timeline.py:559
-#| msgid "Show timeline\tCtrl+T"
+#: ../vdms_miniframes/timeline.py:566
 msgid "Timeline Editor Usage"
 msgstr "Использование редактора Timeline"
 
-#: ../vdms_io/checkup.py:45
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
+#: ../vdms_io/checkup.py:47
+#, fuzzy
+#| msgid "This preset already exists, do you want to overwrite it?"
+msgid "Files already exist, do you want to overwrite them?"
+msgstr "Этот пресет уже существует, вы хотите его перезаписать?"
+
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
 msgstr ""
-"Уже существующие файлы: \n"
-"\n"
-"{}\n"
-"\n"
-"Вы хотите перезаписать? "
 
-#: ../vdms_io/checkup.py:48
+#: ../vdms_io/checkup.py:50
 msgid "Please Confirm"
 msgstr "Пожалуйста подтвердите"
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
+#: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
 msgstr ""
-"Файл не существует:\n"
-"\n"
-"\"{}\"\n"
 
-#: ../vdms_io/checkup.py:62
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr "Не найдено"
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr ""
+
+#: ../vdms_io/checkup.py:75
 msgid ""
 "Output folder does not exist:\n"
 "\n"
 "\"{}\"\n"
 msgstr ""
 "Выходная папка не существует:\n"
 "\n"
@@ -1965,40 +1998,40 @@
 "and try to click the \"Restore all...\" button"
 msgstr ""
 "Пресеты не найдены.\n"
 "\n"
 "Возможное решение: откройте панель Менеджер Пресетов, перейдите в столбец "
 "пресеты и попробуйте нажать кнопку «Восстановить всё ...»"
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr "Готово"
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 msgid ""
 "There are still processes running. if you want to stop them, use the \"Abort"
 "\" button."
 msgstr ""
 "Есть еще запущенные процессы... если вы хотите остановить их, используйте "
 "кнопку «Прервать»."
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr "Videomass"
 
 #: ../vdms_main/main_frame.py:350
 msgid "Are you sure you want to exit the application?"
 msgstr "Вы уверены, что хотите выйти из приложения?"
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr "Выход"
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -2172,27 +2205,26 @@
 msgstr "Просмотр сообщений log-журнала"
 
 #: ../vdms_main/main_frame.py:511
 msgid "Show timeline\tCtrl+T"
 msgstr "Показать шкалу времени\tCtrl+T"
 
 #: ../vdms_main/main_frame.py:512
-#| msgid "Show timeline\tCtrl+T"
 msgid "Show timeline editor"
 msgstr "Показать редактор Timeline"
 
 #: ../vdms_main/main_frame.py:515 ../vdms_ytdlp/main_ytdlp.py:284
 msgid "View"
 msgstr "Посмотр"
 
 #: ../vdms_main/main_frame.py:520
 msgid "Home panel\tCtrl+Shift+H"
 msgstr "Начальная панель\tCtrl+Shift+H"
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 msgid "Go to the 'Home' panel"
 msgstr "Перейдите к 'Начальной панели'"
 
 #: ../vdms_main/main_frame.py:524
 msgid "Presets Manager\tCtrl+Shift+P"
 msgstr "Менеджер Пресетов\tCtrl+Shift+P"
 
@@ -2242,22 +2274,22 @@
 
 #: ../vdms_main/main_frame.py:544
 msgid "Output Monitor\tCtrl+Shift+O"
 msgstr "Выходной экран\tCtrl+Shift+O"
 
 #: ../vdms_main/main_frame.py:545
 msgid "Keeps track of the output for debugging errors"
-msgstr "Отслеживает вывод для ошибок отладки"
+msgstr "Отслеживает вывод для отладки ошибок"
 
 # посмотреть в программе
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr "Перейти"
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr "Настройте временную папку для конверсий"
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr "Используйте временное местоположение для сохранения конверсий"
 
@@ -2357,177 +2389,177 @@
 msgid "Help"
 msgstr "Помощь"
 
 #: ../vdms_main/main_frame.py:677
 msgid "Open the selected files"
 msgstr "Открыть выбранные файлы"
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 msgid "No such folder '{}'"
 msgstr "Нет такой папки '{}'"
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 msgid "Are you sure to empty trash folder?"
 msgstr "Вы уверены, что очистили папку \"Корзина\"?"
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 msgid "No files to delete"
 msgstr "Нет файлов для удаления"
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr "Installed release v{0}. A new presets release is available {1}"
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr "Установленная версия {0}. Новых обновлений не обнаружено."
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr "Выберите папку для загрузки"
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 "Подождите...\n"
 "Архив скачивается"
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr "Успешно загружено в \"{0}\""
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr "Выберите временное место назначения для конверсий"
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 msgid "Default destination folders successfully restored"
 msgstr "Папки назначения по умолчанию успешно восстановлены"
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 msgid "Changes will take effect once the program has been restarted."
 msgstr "Изменения вступят в силу после перезапуска программы."
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr ""
 "Изменения вступят в силу после перезапуска программы\n"
 "\n"
 "Вы хотите выйти из приложения сейчас?"
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, python-brace-format
 msgid "A new release is available - v.{0}\n"
 msgstr "Доступна новая версия - v.{0}\n"
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr "Вы используете версию для разработки, которая еще не выпущена!\n"
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr "Поздравляю! Вы уже используете последнюю версию.\n"
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr "Перейти к предыдущей панели"
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr "Назад"
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr "Перейти к следующей панели"
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 msgid "Next"
 msgstr "Вперед"
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr "Начальная панель"
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 msgid "Play the selected file in the list"
 msgstr "Воспроизведение выбранного в списке файла"
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr "Воспроизведение"
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 msgid "Get informative data about imported media streams"
 msgstr "Получайте информативные данные об импортированных медиапотоках"
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 msgid "Start rendering"
 msgstr "Начать преобразование"
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr "Запуск"
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr "Останавливает текущий процесс"
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr "Прервать"
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr "Удалить все файлы из списка"
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr "Очистить"
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 msgid "Videomass - Queued Files"
 msgstr "Videomass - Файлы в очереди"
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr "Videomass - AV-конвертация"
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr "Videomass - Менеджер Пресетов"
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 msgid "Videomass - Concatenate Demuxer"
 msgstr "Videomass - Concatenate Demuxer"
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 msgid "Videomass - From Movie to Pictures"
 msgstr "Videomass - Картинки из фильма"
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 msgid "Videomass - Still Image Maker"
 msgstr "Videomass - Still Image Maker"
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr "Просмотр последнего log-журнала"
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr "Обработка ..."
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 msgid "Videomass - FFmpeg message monitor"
 msgstr "Videomass - монитор сообщений FFmpeg"
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
 msgstr "Медиа:"
 
@@ -2873,20 +2905,20 @@
 msgid "{} file in queue"
 msgstr "{} файл в очереди"
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr "Выключено"
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr "Не установлено"
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr "начало  {} | продолжительность  {}"
 
 #: ../vdms_panels/av_conversions.py:2261
 msgid ""
 "Queued File\n"
@@ -3098,15 +3130,17 @@
 
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 "Извлекайте изображения (кадры) из ваших фильмов в форматы JPG, PNG, BMP, GIF."
 
 #: ../vdms_panels/choose_topic.py:223
-msgid "The downloader is disabled. Check your preferences."
+#, fuzzy
+#| msgid "The downloader is disabled. Check your preferences."
+msgid "yt-dlp is disabled. Check your preferences."
 msgstr "Загрузчик отключен. Проверьте свои настройки."
 
 #: ../vdms_panels/concatenate.py:78
 msgid ""
 "\n"
 "- The concatenation function is performed only with Audio files or only with "
 "Video files.\n"
@@ -3133,16 +3167,16 @@
 "- Имя выходного файла будет таким же, как у первого добавленного файла\n"
 " (также зависит от настроек, сделанных в диалоговом окне настроек,\n"
 "  или от используемых функций переименования).\n"
 "\n"
 "- Видеофайлы должны иметь одинаковые потоки, одинаковые кодеки и одинаковые\n"
 "  ширину/высоту, но может быть упакован в разные форматы контейнеров.\n"
 "\n"
-"- Аудиофайлы должны иметь одинаковые форматы, одинаковые кодеки с одинаковой "
-"частотой дискретизации."
+"- Аудиофайлы должны иметь одинаковые форматы, одинаковые кодеки \n"
+"  с одинаковой частотой дискретизации."
 
 #: ../vdms_panels/concatenate.py:122
 msgid "From an image sequence to a video file"
 msgstr "Из последовательности изображений в видеофайл"
 
 #: ../vdms_panels/concatenate.py:127
 msgid "Duration:"
@@ -3204,111 +3238,121 @@
 msgstr ""
 "Файл для объединения\n"
 "Имя выходного файла\n"
 "Папка назначения\n"
 "Выходной формат\n"
 "Временной период"
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr "Файл содержит недопустимые символы, такие как:"
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 msgid "Invalid path name. Contains double or single quotes"
 msgstr "Недопустимое имя пути. Содержит двойные или одинарные кавычки"
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 msgid "Directories are not allowed, just add files, please."
 msgstr "Каталоги не разрешены, добавьте просто файлы."
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 "Файл без расширения формата: укажите соответствующее расширение имени файла, "
 "например «.mkv», «.avi», «.mp3» и т.д."
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr "Имя содержит недопустимые символы, такие как: {0}"
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr "Имя уже используется:"
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr "Имя Файла"
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr "Длина"
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr "Тип медиа"
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr "Размер"
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 msgid "Output file name"
 msgstr "Имя выходного файла"
 
-#: ../vdms_panels/filedrop.py:207
-msgid "Duplicate files are rejected: > {}"
-msgstr "Дубликаты файлов отклоняются: > {}"
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr ""
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:209
+#, fuzzy
+#| msgid "Add Files"
+msgid "Rejected Files"
+msgstr "Добавить файлы"
+
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr "Перетащите один или несколько файлов ниже"
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 msgid "Destination folder"
 msgstr "Папка назначения"
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 msgid "Drag the images below"
 msgstr "Перетащите изображения ниже"
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 msgid "Drag one or more video below"
 msgstr "Перетащите одно или несколько видео ниже"
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 msgid "No file selected"
 msgstr "Файл не выбран"
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 msgid "File renaming..."
 msgstr "Переименование файла..."
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 msgid "Rename the selected file to:"
 msgstr "Переименуйте выбранный файл в:"
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr "Добавить файлы"
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr "Переименовать элементы"
 
 # Здесь изменил фразу исходника для правильного использования в русском языке
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr "Файлов для переименования: {0}"
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 msgid "New Name #"
 msgstr "Новое имя #"
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
 msgid "[Videomass]: SUCCESS !"
 msgstr "[Videomass]: УСПЕШНО !"
@@ -3732,19 +3776,19 @@
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 "Управление выбранным профилем изменено вручную.\n"
 "Вы хотите применить его в процессе конвертации?"
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 msgid "Don't show this dialog again"
 msgstr "Больше не показывать этот диалог"
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 msgid ""
 "Queued File\n"
 "Pass Encoding\n"
 "Profile Used\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
@@ -3757,68 +3801,53 @@
 #: ../vdms_panels/sequence_to_video.py:55
 msgid "Images need to be resized, please use Resizing function."
 msgstr ""
 "Изображения должны быть изменены, пожалуйста, используйте функцию изменения "
 "размера."
 
 #: ../vdms_panels/sequence_to_video.py:74
-#| msgid ""
-#| "\n"
-#| "1. Import one or more image files such as JPG, PNG and BMP formats, then "
-#| "select one.\n"
-#| "\n"
-#| "2. Use the \"Resizing\" filter to resize images which have different "
-#| "sizes such as width and height. It is optional in other cases.\n"
-#| "\n"
-#| "3. To set the DURATION between images use the \"End\" control on the Trim "
-#| "bar.\n"
-#| "\n"
-#| "4. Start the conversion.\n"
-#| "\n"
-#| "\n"
-#| "The produced video will have the name of the selected file in the 'Queued "
-#| "File' list, which will be saved in a folder named 'Still_Images'\n"
-#| "with a progressive digit, in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 "\n"
-"1. Импортируйте один или несколько файлов изображений, таких как форматы "
-"JPG, PNG и BMP, затем выберите один из них.\n"
+"1. Импортируйте один или несколько файлов изображений, \n"
+"  таких как форматы JPG, PNG и BMP, затем выберите один.\n"
+"\n"
+"2. Используйте функцию изменения размера, чтобы изменить \n"
+"  размер изображений, которые имеют разные размеры, такие \n"
+"  как ширина и высота. В других случаях это необязательно.\n"
 "\n"
-"2. Используйте функцию изменения размера, чтобы изменить размер изображений, "
-"которые имеют разные размеры, такие как ширина и высота. В других случаях "
-"это необязательно.\n"
-"\n"
-"3. Используйте редактор Timeline (CTRL+T), чтобы установить временной "
-"интервал между изображениями, отрегулировав значение продолжительности "
-"«Конец» \n"
-"и оставив значение «Начало» равным 00:00:00.000.\n"
+"3. Используйте редактор временной шкалы (CTRL+T), чтобы установить \n"
+"  временной интервал между изображениями, регулируя значение \n"
+"  времени «Конец» и оставить значение «Начало» равным 00:00:00.000.\n"
 "\n"
 "4. Запустите преобразование.\n"
 "\n"
 "\n"
-"Созданное видео будет иметь имя выбранного файла в списке «Файл в очереди», "
-"который будет сохранен в папке с именем «Still_Images» \n"
+"Созданное видео будет иметь имя выбранного файла в списке «Файл в "
+"очереди», \n"
+"которые будут сохранены в папке с именем «Still_Images» \n"
 "с прогрессивной цифрой по указанному вами пути."
 
 #: ../vdms_panels/sequence_to_video.py:129
 msgid "Enable a single still image"
 msgstr "Включить одно неподвижное изображение"
 
 #: ../vdms_panels/sequence_to_video.py:161
@@ -3877,14 +3906,25 @@
 msgstr "Недопустимый файл: '{}'"
 
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 msgid "Unsupported format '{}'"
 msgstr "Неподдерживаемый формат '{}'"
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+"Файл не существует:\n"
+"\n"
+"\"{}\"\n"
+
 #: ../vdms_panels/sequence_to_video.py:719
 msgid ""
 "File to process\n"
 "Output filename\n"
 "Destination Folder\n"
 "Output Format\n"
 "Additional arguments\n"
@@ -3991,59 +4031,46 @@
 "\"cpu-used\" sets how efficient the compression will be. The meaning depends "
 "on the Quality and Compression mode above."
 msgstr ""
 "«Cpu-used» устанавливает, насколько эффективным будет сжатие. Значение "
 "зависит от режима качества и сжатия, указанного выше."
 
 #: ../vdms_panels/video_to_sequence.py:49
-#| msgid ""
-#| "\n"
-#| "1. Import one or more video files, then select one.\n"
-#| "\n"
-#| "2. To select a slice of time use the \"Start\" \"End\" controls on the "
-#| "Trim bar.\n"
-#| "\n"
-#| "3. Select an output format (jpg, png, bmp).\n"
-#| "\n"
-#| "4. Start the conversion.\n"
-#| "\n"
-#| "\n"
-#| "The images produced will be saved in a folder named \"Movie_to_Pictures\" "
-#| "with a progressive digit, \n"
-#| "in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 "\n"
-"1. Импортируйте один или несколько видеофайлов, затем выберите один.\n"
+"1. Импортируйте один или несколько видеофайлов, \n"
+"    затем выберите один.\n"
 "\n"
-"2. Чтобы выбрать отрезок времени, используйте редактор временной шкалы (CTRL"
-"+T), настроив значения длительности «Конец» и «Начало».\n"
+"2. Чтобы выбрать отрезок времени, используйте редактор \n"
+"    Timeline (CTRL+T), отрегулировав\n"
+"    Значения длительности «Конец» и «Начало».\n"
 "\n"
 "3. Выберите выходной формат (jpg, png, bmp).\n"
 "\n"
 "4. Запустите преобразование.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"Созданные изображения будут сохранены в папке \n"
+"с именем 'Movie_to_Pictures'\n"
+"с прогрессивной цифрой по указанному вами пути."
 
 #: ../vdms_panels/video_to_sequence.py:84
 msgid "Create thumbnails"
 msgstr "Создание эскизов"
 
 #: ../vdms_panels/video_to_sequence.py:85
 msgid "Create tiled mosaics"
@@ -4125,15 +4152,15 @@
 "По крайней мере один \" Код формата \" должен быть проверен для каждого URL, "
 "выделенного зеленым цветом."
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr "Код формата"
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr "Url"
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr "Заглавие"
 
@@ -4214,25 +4241,25 @@
 msgid "Hide YouTube Downloader"
 msgstr "Скрыть загрузчик YouTube"
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 msgid "Quit YouTube Downloader"
 msgstr "Выйти из загрузчика YouTube"
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 msgid "Paste\tCtrl+V"
 msgstr "Вставить\tCtrl+V"
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr "Вставьте скопированные URL-адреса в буфер обмена"
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr "Удалить выбранный URL\tDEL"
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 msgid "Remove the selected URL from the list"
 msgstr "Удалить выбранный URL из списка"
 
@@ -4248,15 +4275,15 @@
 msgid "Latest version of yt-dlp"
 msgstr "Последняя версия yt-dlp"
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 msgid "Check the latest version available on github.com"
 msgstr "Проверьте последнюю версию, доступную на github.com"
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr "Настройте временную папку для загрузок"
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr "Сохраните все загрузки во временной папке"
 
@@ -4363,19 +4390,33 @@
 msgid ""
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr ""
 "ВНИМАНИЕ! Выбранный URL-адрес не относится к списку воспроизведения. "
 "Индексировать можно только строки, отмеченные зелёным."
 
-#: ../vdms_ytdlp/textdrop.py:74
-msgid "Invalid URL:"
+#: ../vdms_ytdlp/textdrop.py:68
+#, fuzzy
+#| msgid "Invalid URL:"
+msgid "Invalid URL"
 msgstr "Неверный URL:"
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:84
+#, fuzzy
+#| msgid "Remove selected URL\tDEL"
+msgid "List of rejected URLs"
+msgstr "Удалить выбранный URL\tDEL"
+
+#: ../vdms_ytdlp/textdrop.py:87
+#, fuzzy
+#| msgid "Remove selected URL\tDEL"
+msgid "Rejected URLs"
+msgstr "Удалить выбранный URL\tDEL"
+
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr "Перетащите или вставьте URL-адреса сюда"
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 msgid "Statistics viewer"
 msgstr "Просмотр статистики"
 
@@ -4490,14 +4531,30 @@
 "URL-адреса содержат списки воспроизведения. Вы уверены, что хотите "
 "продолжить?"
 
 #: ../vdms_ytdlp/youtubedl_ui.py:659
 msgid "The URLs contain channels. Are you sure you want to continue?"
 msgstr "URL-адреса содержат видеоканалы. Вы уверены, что хотите продолжить?"
 
+#~ msgid ""
+#~ "Already exist: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Do you want to overwrite? "
+#~ msgstr ""
+#~ "Уже существующие файлы: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Вы хотите перезаписать? "
+
+#~ msgid "Duplicate files are rejected: > {}"
+#~ msgstr "Дубликаты файлов отклоняются: > {}"
+
 #~ msgid "File list changed, please check the settings again."
 #~ msgstr "Список файлов изменен, проверьте настройки еще раз."
 
 #~ msgid ""
 #~ "Cannot continue: The duration in the timeline exceeds the duration of "
 #~ "some queued files."
 #~ msgstr ""
@@ -4758,17 +4815,14 @@
 #~ msgid ""
 #~ "Make sure you are using the latest available version of\n"
 #~ "'{}'. This allows you to avoid download problems.\n"
 #~ msgstr ""
 #~ "Убедитесь, что вы используете последнюю доступную версию '{}'.\n"
 #~ "Это позволяет избежать проблем с загрузкой.\n"
 
-#~ msgid "Not found"
-#~ msgstr "Не найдено"
-
 #~ msgid "Not Installed"
 #~ msgstr "Не установлено"
 
 #~ msgid "Downloader"
 #~ msgstr "Загрузчик"
 
 #~ msgid "Topic List..."
@@ -4878,17 +4932,14 @@
 
 #~ msgid "Duration hours"
 #~ msgstr "Часы"
 
 #~ msgid "Duration minutes"
 #~ msgstr "Минуты"
 
-#~ msgid "Duration seconds"
-#~ msgstr "Секунды"
-
 #~ msgid "Duration milliseconds"
 #~ msgstr "Миллисекунды"
 
 #~ msgid "Start hours"
 #~ msgstr "Часы"
 
 #~ msgid "Show panel for editing timeline (seek/duration)"
@@ -5377,17 +5428,14 @@
 #~ msgstr "Отключено"
 
 #, fuzzy
 #~| msgid "Successful! youtube-dl is up-to-date"
 #~ msgid "Successful! {} is up-to-date"
 #~ msgstr "Успешно! youtube-dl обновлен"
 
-#~ msgid "Disable youtube-dl"
-#~ msgstr "Отключить youtube-dl"
-
 #~ msgid "Enable youtube-dl"
 #~ msgstr "Включить youtube-dl"
 
 #~ msgid "youtube-dl"
 #~ msgstr "youtube-dl"
 
 #~ msgid "Update youtube-dl"
@@ -5849,15 +5897,12 @@
 
 #~ msgid "Filters"
 #~ msgstr "Фильтры"
 
 #~ msgid "Open a preset to store the new profile"
 #~ msgstr "Откройте пресет, чтобы сохранить новый профиль"
 
-#~ msgid "This preset already exists, do you want to overwrite it?"
-#~ msgstr "Этот пресет уже существует, вы хотите его перезаписать?"
-
 #~ msgid "Import a group of Videomass presets"
 #~ msgstr "Импортируйте группу пресетов Videomass"
 
 #~ msgid "A new group of presets was successfully imported"
 #~ msgstr "Новая группа пресетов была успешно импортирована"
```

### Comparing `videomass-5.0.0/videomass/locale/videomass.pot` & `videomass-5.0.1/videomass/locale/videomass.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -34,20 +34,20 @@
 #, python-brace-format
 msgid ""
 "Unexpected error while deleting file contents:\n"
 "\n"
 "{0}"
 msgstr ""
 
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr ""
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -89,71 +89,71 @@
 "imported files"
 msgstr ""
 
 #: ../vdms_dialogs/epilogue.py:100
 msgid "Confirm Settings"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 msgid "Search for a specific frame"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr ""
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr ""
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr ""
 
@@ -269,16 +269,16 @@
 "This is a high precision/quality 3d denoise filter. It aims to reduce image "
 "noise, producing smooth images and making still images really still. It "
 "should enhance compressibility."
 msgstr ""
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 msgid "Read me"
 msgstr ""
 
 #: ../vdms_dialogs/filter_scale.py:80
 msgid "View result"
@@ -363,14 +363,18 @@
 msgid "Create a snapshot"
 msgstr ""
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr ""
 
+#: ../vdms_dialogs/filter_stab.py:110
+msgid "Duration seconds:"
+msgstr ""
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr ""
 
 #: ../vdms_dialogs/filter_stab.py:177
 msgid "[TRIPOD] Enable tripod mode if checked"
 msgstr ""
@@ -658,16 +662,16 @@
 #: ../vdms_dialogs/wizard_dlg.py:263
 msgid ""
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr ""
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 msgid "Videomass has a simple graphical interface for yt-dlp\n"
 msgstr ""
 
@@ -869,153 +873,179 @@
 msgid "Miscellanea"
 msgstr ""
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 msgid "Save each file in the same folder as input file"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 msgid "Auto-create subfolders when downloading playlists"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:288
+msgid "Enable/Disable yt-dlp"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 msgid "Place the toolbar"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:349
-msgid "Shows the text in the toolbar buttons"
+#: ../vdms_dialogs/preferences.py:378
+msgid "Shows text in the toolbar buttons"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 msgid "Appearance"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 msgid "Set a persistent location to save exported files"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 msgid "Choose a new destination for the files to be trashed"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 msgid "Set a persistent location to save the file downloads"
 msgstr ""
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 msgid "Get Latest Version"
 msgstr ""
 
@@ -1061,15 +1091,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr ""
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 msgid "Properties"
 msgstr ""
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
 msgid "Values"
 msgstr ""
@@ -1534,56 +1564,56 @@
 msgid "Seconds"
 msgstr ""
 
 #: ../vdms_miniframes/timeline.py:108
 msgid "Milliseconds"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 msgid "Start adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:320
+#: ../vdms_miniframes/timeline.py:322
 msgid "Source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 msgid "Start"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 msgid "End"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1596,40 +1626,43 @@
 "duration of a selected source file (see status bar messages).\n"
 "\n"
 "The \"Start\"/\"End\" duration values always refer to the initial position "
 "of the timeline: 00:00:00.000. For other informations as the segment "
 "duration and warnings, please refer to the status bar messages."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:559
+#: ../vdms_miniframes/timeline.py:566
 msgid "Timeline Editor Usage"
 msgstr ""
 
-#: ../vdms_io/checkup.py:45
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
+#: ../vdms_io/checkup.py:47
+msgid "Files already exist, do you want to overwrite them?"
 msgstr ""
 
-#: ../vdms_io/checkup.py:48
-msgid "Please Confirm"
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
 msgstr ""
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
+#: ../vdms_io/checkup.py:50
+msgid "Please Confirm"
 msgstr ""
 
 #: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
+msgstr ""
+
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr ""
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr ""
+
+#: ../vdms_io/checkup.py:75
 msgid ""
 "Output folder does not exist:\n"
 "\n"
 "\"{}\"\n"
 msgstr ""
 
 #: ../vdms_io/io_tools.py:58
@@ -1676,38 +1709,38 @@
 msgid ""
 "No presets found.\n"
 "\n"
 "Possible solution: open the Presets Manager panel, go to the presets column "
 "and try to click the \"Restore all...\" button"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 msgid ""
 "There are still processes running. if you want to stop them, use the \"Abort"
 "\" button."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:350
 msgid "Are you sure you want to exit the application?"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -1882,15 +1915,15 @@
 msgid "View"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:520
 msgid "Home panel\tCtrl+Shift+H"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 msgid "Go to the 'Home' panel"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:524
 msgid "Presets Manager\tCtrl+Shift+P"
 msgstr ""
 
@@ -1946,15 +1979,15 @@
 msgid "Keeps track of the output for debugging errors"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr ""
 
@@ -2049,172 +2082,172 @@
 msgid "Help"
 msgstr ""
 
 #: ../vdms_main/main_frame.py:677
 msgid "Open the selected files"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 msgid "No such folder '{}'"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 msgid "Are you sure to empty trash folder?"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 msgid "No files to delete"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr ""
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 msgid "Default destination folders successfully restored"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 msgid "Changes will take effect once the program has been restarted."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, python-brace-format
 msgid "A new release is available - v.{0}\n"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 msgid "Next"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 msgid "Play the selected file in the list"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 msgid "Get informative data about imported media streams"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 msgid "Start rendering"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 msgid "Videomass - Queued Files"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 msgid "Videomass - Concatenate Demuxer"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 msgid "Videomass - From Movie to Pictures"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 msgid "Videomass - Still Image Maker"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 msgid "Videomass - FFmpeg message monitor"
 msgstr ""
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
 msgstr ""
 
@@ -2513,20 +2546,20 @@
 msgid "{} file in queue"
 msgstr ""
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr ""
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr ""
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr ""
 
 #: ../vdms_panels/av_conversions.py:2261
 msgid ""
 "Queued File\n"
@@ -2670,15 +2703,15 @@
 msgstr ""
 
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr ""
 
 #: ../vdms_panels/choose_topic.py:223
-msgid "The downloader is disabled. Check your preferences."
+msgid "yt-dlp is disabled. Check your preferences."
 msgstr ""
 
 #: ../vdms_panels/concatenate.py:78
 msgid ""
 "\n"
 "- The concatenation function is performed only with Audio files or only with "
 "Video files.\n"
@@ -2750,108 +2783,116 @@
 "File to concatenate\n"
 "Output filename\n"
 "Destination\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 msgid "Invalid path name. Contains double or single quotes"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 msgid "Directories are not allowed, just add files, please."
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 msgid "Output file name"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:207
-msgid "Duplicate files are rejected: > {}"
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:209
+msgid "Rejected Files"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 msgid "Destination folder"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 msgid "Drag the images below"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 msgid "Drag one or more video below"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 msgid "No file selected"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 msgid "File renaming..."
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 msgid "Rename the selected file to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 msgid "New Name #"
 msgstr ""
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
 msgid "[Videomass]: SUCCESS !"
 msgstr ""
@@ -3230,19 +3271,19 @@
 
 #: ../vdms_panels/presets_manager.py:833
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 msgid "Don't show this dialog again"
 msgstr ""
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 msgid ""
 "Queued File\n"
 "Pass Encoding\n"
 "Profile Used\n"
 "Output Format\n"
 "Time Period"
 msgstr ""
@@ -3254,26 +3295,28 @@
 #: ../vdms_panels/sequence_to_video.py:74
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 
 #: ../vdms_panels/sequence_to_video.py:129
 msgid "Enable a single still image"
 msgstr ""
 
 #: ../vdms_panels/sequence_to_video.py:161
@@ -3324,14 +3367,22 @@
 msgstr ""
 
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 msgid "Unsupported format '{}'"
 msgstr ""
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+
 #: ../vdms_panels/sequence_to_video.py:719
 msgid ""
 "File to process\n"
 "Output filename\n"
 "Destination Folder\n"
 "Output Format\n"
 "Additional arguments\n"
@@ -3411,24 +3462,24 @@
 
 #: ../vdms_panels/video_to_sequence.py:49
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 
 #: ../vdms_panels/video_to_sequence.py:84
 msgid "Create thumbnails"
 msgstr ""
 
 #: ../vdms_panels/video_to_sequence.py:85
@@ -3496,15 +3547,15 @@
 "At least one \"Format Code\" must be checked for each URL selected in green."
 msgstr ""
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr ""
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr ""
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr ""
 
@@ -3579,25 +3630,25 @@
 msgid "Hide YouTube Downloader"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 msgid "Quit YouTube Downloader"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 msgid "Paste\tCtrl+V"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 msgid "Remove the selected URL from the list"
 msgstr ""
 
@@ -3613,15 +3664,15 @@
 msgid "Latest version of yt-dlp"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 msgid "Check the latest version available on github.com"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr ""
 
@@ -3719,19 +3770,27 @@
 
 #: ../vdms_ytdlp/playlist_indexing.py:256
 msgid ""
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr ""
 
-#: ../vdms_ytdlp/textdrop.py:74
-msgid "Invalid URL:"
+#: ../vdms_ytdlp/textdrop.py:68
+msgid "Invalid URL"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:84
+msgid "List of rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:87
+msgid "Rejected URLs"
 msgstr ""
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr ""
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 msgid "Statistics viewer"
 msgstr ""
```

### Comparing `videomass-5.0.0/videomass/locale/zh_CN/LC_MESSAGES/videomass.mo` & `videomass-5.0.1/videomass/locale/zh_CN/LC_MESSAGES/videomass.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2023-04-10 14:35+0200\n"
+"PO-Revision-Date: 2023-04-18 21:44+0200\n"
 "Last-Translator: MaiJZ https://github.com/maijz128\n"
 "Language-Team: simplified Chinese (CN)\n"
 "Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
@@ -754,14 +754,17 @@
 
 msgid "New"
 msgstr "创建"
 
 msgid "No Audio"
 msgstr "没有音频"
 
+msgid "Not found"
+msgstr "未找到"
+
 msgid "Off"
 msgstr "关闭"
 
 msgid "Open an audio file"
 msgstr "打开一个音频文件"
 
 msgid "Open audio file"
```

### Comparing `videomass-5.0.0/videomass/locale/zh_CN/LC_MESSAGES/videomass.po` & `videomass-5.0.1/videomass/locale/zh_CN/LC_MESSAGES/videomass.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: Videomass 5.0.0\n"
+"Project-Id-Version: Videomass 5.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-10 14:19+0200\n"
-"PO-Revision-Date: 2023-04-10 14:35+0200\n"
+"POT-Creation-Date: 2023-04-18 21:40+0200\n"
+"PO-Revision-Date: 2023-04-18 21:44+0200\n"
 "Last-Translator: MaiJZ https://github.com/maijz128\n"
 "Language-Team: simplified Chinese (CN)\n"
 "Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
@@ -41,20 +41,20 @@
 "\n"
 "{0}"
 msgstr ""
 "Unexpected error while deleting file contents:\n"
 "\n"
 "{0}"
 
-#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:318
+#: ../vdms_dialogs/audiodialogs.py:109 ../vdms_dialogs/filter_crop.py:310
 #: ../vdms_dialogs/filter_deinterlace.py:121
 #: ../vdms_dialogs/filter_denoisers.py:84 ../vdms_dialogs/filter_scale.py:209
 #: ../vdms_dialogs/filter_stab.py:317 ../vdms_dialogs/filter_transpose.py:105
 #: ../vdms_dialogs/filter_colorcorrection.py:187
-#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:278
+#: ../vdms_miniframes/timeline.py:261 ../vdms_miniframes/timeline.py:280
 #: ../vdms_panels/av_conversions.py:389 ../vdms_ytdlp/playlist_indexing.py:128
 msgid "Reset"
 msgstr "复位"
 
 #: ../vdms_dialogs/audiodialogs.py:230
 msgid ""
 "Videomass supports mono and stereo audio channels. If you are not sure set "
@@ -108,74 +108,74 @@
 
 #: ../vdms_dialogs/epilogue.py:100
 #, fuzzy
 #| msgid "Settings"
 msgid "Confirm Settings"
 msgstr "设置"
 
-#: ../vdms_dialogs/filter_crop.py:243 ../vdms_dialogs/filter_scale.py:108
+#: ../vdms_dialogs/filter_crop.py:235 ../vdms_dialogs/filter_scale.py:108
 #, python-brace-format
 msgid "Source size: {0} x {1} pixels"
 msgstr "源尺寸：{0}×{1}像素"
 
-#: ../vdms_dialogs/filter_crop.py:251
+#: ../vdms_dialogs/filter_crop.py:243
 #: ../vdms_dialogs/filter_colorcorrection.py:103
 #, fuzzy
 msgid "Search for a specific frame"
 msgstr "搜索一个特定的框架"
 
-#: ../vdms_dialogs/filter_crop.py:265
+#: ../vdms_dialogs/filter_crop.py:257
 #: ../vdms_dialogs/filter_colorcorrection.py:117
 msgid "Load"
 msgstr "加载"
 
-#: ../vdms_dialogs/filter_crop.py:268
+#: ../vdms_dialogs/filter_crop.py:260
 msgid "Cropping area selection "
 msgstr "裁剪区的选择 "
 
-#: ../vdms_dialogs/filter_crop.py:273 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:265 ../vdms_dialogs/filter_scale.py:120
 msgid "Height"
 msgstr "高度"
 
-#: ../vdms_dialogs/filter_crop.py:293
+#: ../vdms_dialogs/filter_crop.py:285
 msgid "Center"
 msgstr "中心"
 
-#: ../vdms_dialogs/filter_crop.py:304 ../vdms_dialogs/filter_scale.py:120
+#: ../vdms_dialogs/filter_crop.py:296 ../vdms_dialogs/filter_scale.py:120
 msgid "Width"
 msgstr "宽度"
 
-#: ../vdms_dialogs/filter_crop.py:323 ../vdms_dialogs/filter_deinterlace.py:120
+#: ../vdms_dialogs/filter_crop.py:315 ../vdms_dialogs/filter_deinterlace.py:120
 #: ../vdms_dialogs/filter_denoisers.py:83 ../vdms_dialogs/filter_scale.py:207
 #: ../vdms_dialogs/filter_stab.py:315 ../vdms_dialogs/filter_transpose.py:110
 #: ../vdms_dialogs/set_timestamp.py:148
 #: ../vdms_dialogs/filter_colorcorrection.py:192
 #: ../vdms_ytdlp/playlist_indexing.py:132
 msgid "Apply"
 msgstr "应用"
 
-#: ../vdms_dialogs/filter_crop.py:338
+#: ../vdms_dialogs/filter_crop.py:330
 msgid "Crop Filter"
 msgstr "裁剪过滤器"
 
-#: ../vdms_dialogs/filter_crop.py:339
+#: ../vdms_dialogs/filter_crop.py:331
 msgid "Crop to width"
 msgstr "裁剪的宽度"
 
-#: ../vdms_dialogs/filter_crop.py:340
+#: ../vdms_dialogs/filter_crop.py:332
 #, fuzzy
 msgid "Move vertically - set to -1 to center the vertical axis"
 msgstr "纵向移动--设置为-1以使纵轴居中"
 
-#: ../vdms_dialogs/filter_crop.py:342
+#: ../vdms_dialogs/filter_crop.py:334
 #, fuzzy
 msgid "Move horizontally - set to -1 to center the horizontal axis"
 msgstr "水平移动--设置为-1，使水平轴居中。"
 
-#: ../vdms_dialogs/filter_crop.py:344
+#: ../vdms_dialogs/filter_crop.py:336
 msgid "Crop to height"
 msgstr "裁剪的高度"
 
 #: ../vdms_dialogs/filter_deinterlace.py:56
 msgid "Advanced Options"
 msgstr "高级选项"
 
@@ -327,16 +327,16 @@
 msgstr ""
 "hqdn3d:n\n"
 "这是一个高精度/高质量的三维去噪滤波器。它的目的是减少图像噪音，产生平滑的图"
 "像，使静止的图像真正静止。它应该增强可压缩性。"
 
 #: ../vdms_dialogs/filter_scale.py:75 ../vdms_dialogs/ffmpeg_help.py:117
 #: ../vdms_dialogs/shownormlist.py:98 ../vdms_dialogs/shownormlist.py:107
-#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:260
-#: ../vdms_miniframes/timeline.py:280 ../vdms_panels/concatenate.py:109
+#: ../vdms_dialogs/shownormlist.py:116 ../vdms_miniframes/timeline.py:262
+#: ../vdms_miniframes/timeline.py:282 ../vdms_panels/concatenate.py:109
 #: ../vdms_panels/sequence_to_video.py:117
 #: ../vdms_panels/video_to_sequence.py:79
 #, fuzzy
 #| msgid "Ready"
 msgid "Read me"
 msgstr "准备就绪"
 
@@ -440,14 +440,20 @@
 msgid "Create a snapshot"
 msgstr "创建一个新的预设"
 
 #: ../vdms_dialogs/filter_stab.py:107 ../vdms_panels/av_conversions.py:383
 msgid "Preview"
 msgstr "预览"
 
+#: ../vdms_dialogs/filter_stab.py:110
+#, fuzzy
+#| msgid "Duration"
+msgid "Duration seconds:"
+msgstr "持续时间"
+
 #: ../vdms_dialogs/filter_stab.py:119
 msgid "Video Detect"
 msgstr "视频检测"
 
 #: ../vdms_dialogs/filter_stab.py:177
 #, fuzzy
 msgid "[TRIPOD] Enable tripod mode if checked"
@@ -806,16 +812,16 @@
 "\"ffmpeg\", \"ffprobe\" and \"ffplay\" are required. Complete all\n"
 "the text boxes below by clicking on the respective buttons."
 msgstr ""
 "\"ffmpeg\"、\"ffprobe \"和 \"ffplay \"是必需的。完成所有\n"
 "下面的文本框，点击相应的按钮。"
 
 #: ../vdms_dialogs/wizard_dlg.py:345 ../vdms_dialogs/wizard_dlg.py:362
-#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:734
-#: ../vdms_dialogs/preferences.py:776 ../vdms_dialogs/preferences.py:819
+#: ../vdms_dialogs/wizard_dlg.py:380 ../vdms_dialogs/preferences.py:789
+#: ../vdms_dialogs/preferences.py:831 ../vdms_dialogs/preferences.py:874
 msgid "Choose the {} executable"
 msgstr "选择{}可执行文件"
 
 #: ../vdms_dialogs/wizard_dlg.py:403
 #, fuzzy
 #| msgid ""
 #| "Videomass has a simple graphical\n"
@@ -1052,174 +1058,200 @@
 msgid "Miscellanea"
 msgstr "杂项"
 
 #: ../vdms_dialogs/preferences.py:157
 msgid "Where do you prefer to save your transcodes?"
 msgstr "你喜欢在哪里保存你的转码？"
 
-#: ../vdms_dialogs/preferences.py:171
+#: ../vdms_dialogs/preferences.py:170
 msgid "Save each file in the same folder as input file"
 msgstr "将每个文件保存在与输入文件相同的文件夹中"
 
-#: ../vdms_dialogs/preferences.py:176
+#: ../vdms_dialogs/preferences.py:175
 msgid "Assign optional suffix to output file names:"
 msgstr "为输出文件名指定可选的后缀："
 
-#: ../vdms_dialogs/preferences.py:181
+#: ../vdms_dialogs/preferences.py:180
 #, fuzzy
 #| msgid ""
 #| "Move source file to the Videomass trash folder after successful encoding"
 msgid ""
 "Always move source files to the Videomass\n"
 "trash folder after successful encoding"
 msgstr "编码成功后将源文件移至Videomass垃圾文件夹"
 
-#: ../vdms_dialogs/preferences.py:201
+#: ../vdms_dialogs/preferences.py:200
 msgid "Where do you prefer to save your downloads?"
 msgstr "你喜欢在哪里保存你的下载？"
 
-#: ../vdms_dialogs/preferences.py:213
+#: ../vdms_dialogs/preferences.py:212
 msgid "Auto-create subfolders when downloading playlists"
 msgstr "下载播放列表时自动创建子文件夹"
 
-#: ../vdms_dialogs/preferences.py:217
+#: ../vdms_dialogs/preferences.py:216
 msgid "File Preferences"
 msgstr "文件首选项"
 
-#: ../vdms_dialogs/preferences.py:224
+#: ../vdms_dialogs/preferences.py:223
 msgid "Path to the executables"
 msgstr "可执行文件的路径"
 
-#: ../vdms_dialogs/preferences.py:227
+#: ../vdms_dialogs/preferences.py:226
 msgid "Enable another location to run FFmpeg"
 msgstr "启用另一个位置来运行FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:240
+#: ../vdms_dialogs/preferences.py:239
 msgid "Enable another location to run FFprobe"
 msgstr "启用另一个位置来运行FFprobe"
 
-#: ../vdms_dialogs/preferences.py:253
+#: ../vdms_dialogs/preferences.py:252
 msgid "Enable another location to run FFplay"
 msgstr "启用另一个位置来运行FFplay"
 
-#: ../vdms_dialogs/preferences.py:265
+#: ../vdms_dialogs/preferences.py:264
 msgid "Other options"
 msgstr "其他选择"
 
-#: ../vdms_dialogs/preferences.py:269
+#: ../vdms_dialogs/preferences.py:268
 msgid "Threads used for transcoding (from 0 to 32):"
 msgstr "用于转码的线程（从0到32）："
 
-#: ../vdms_dialogs/preferences.py:280
+#: ../vdms_dialogs/preferences.py:279
 msgid "FFmpeg"
 msgstr "FFmpeg"
 
-#: ../vdms_dialogs/preferences.py:286
-msgid "Download videos from YouTube.com and other video sites "
+#: ../vdms_dialogs/preferences.py:285
+msgid "Download videos from YouTube.com and other video sites"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:288
+msgid "Enable/Disable yt-dlp"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:293
+msgid "External Downloader Preferences"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:295
+msgid ""
+"In addition to the default (native) one, yt-dlp currently\n"
+"supports the following external downloaders:\n"
+"aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+"Please note that if you enable an external downloader, you\n"
+"will not be able to view the progress bar during download\n"
+"operations."
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:303
+msgid "External downloader executable path"
 msgstr ""
 
-#: ../vdms_dialogs/preferences.py:297
+#: ../vdms_dialogs/preferences.py:311
+msgid "External downloader arguments"
+msgstr ""
+
+#: ../vdms_dialogs/preferences.py:326
 msgid "Icon themes"
 msgstr "图标主题"
 
-#: ../vdms_dialogs/preferences.py:299
+#: ../vdms_dialogs/preferences.py:328
 #, fuzzy
 msgid ""
 "The chosen icon theme will only change the icons,\n"
 "background and foreground of some text fields."
 msgstr ""
 "所选择的图标主题将只改变图标，以及一些文本字段的背景和前景。\n"
 "一些文本字段的背景和前景。"
 
-#: ../vdms_dialogs/preferences.py:319
+#: ../vdms_dialogs/preferences.py:348
 msgid "Toolbar customization"
 msgstr "工具栏定制"
 
-#: ../vdms_dialogs/preferences.py:321
+#: ../vdms_dialogs/preferences.py:350
 msgid "At the top of window (default)"
 msgstr "在窗口的顶部（默认）"
 
-#: ../vdms_dialogs/preferences.py:322
+#: ../vdms_dialogs/preferences.py:351
 msgid "At the bottom of window"
 msgstr "在窗口的底部"
 
-#: ../vdms_dialogs/preferences.py:323
+#: ../vdms_dialogs/preferences.py:352
 msgid "At the right of window"
 msgstr "在窗口的右边"
 
-#: ../vdms_dialogs/preferences.py:324
+#: ../vdms_dialogs/preferences.py:353
 msgid "At the left of window"
 msgstr "在窗口的左边"
 
-#: ../vdms_dialogs/preferences.py:326
+#: ../vdms_dialogs/preferences.py:355
 #, fuzzy
 msgid "Place the toolbar"
 msgstr "放置工具栏"
 
-#: ../vdms_dialogs/preferences.py:336
+#: ../vdms_dialogs/preferences.py:365
 msgid "Icon size:"
 msgstr "图标大小："
 
-#: ../vdms_dialogs/preferences.py:349
+#: ../vdms_dialogs/preferences.py:378
 #, fuzzy
-msgid "Shows the text in the toolbar buttons"
+msgid "Shows text in the toolbar buttons"
 msgstr "显示工具条按钮中的文字"
 
-#: ../vdms_dialogs/preferences.py:354
+#: ../vdms_dialogs/preferences.py:383
 #, fuzzy
 msgid "Appearance"
 msgstr "外观"
 
-#: ../vdms_dialogs/preferences.py:361
+#: ../vdms_dialogs/preferences.py:390
 #, fuzzy
 msgid ""
 "The following settings affect output messages and\n"
 "the log messages during transcoding processes.\n"
 "Change only if you know what you are doing.\n"
 msgstr ""
 "以下设置会影响输出信息和\n"
 "转码过程中的日志信息。\n"
 "Only change if you know what you are doing.（只有在你知道你在做什么的情况下才"
 "可以更改。\n"
 "\n"
 
-#: ../vdms_dialogs/preferences.py:382
+#: ../vdms_dialogs/preferences.py:411
 msgid "FFmpeg logging levels"
 msgstr "FFmpeg日志级别"
 
-#: ../vdms_dialogs/preferences.py:402 ../vdms_main/main_frame.py:580
+#: ../vdms_dialogs/preferences.py:431 ../vdms_main/main_frame.py:580
 #: ../vdms_panels/av_conversions.py:471 ../vdms_ytdlp/main_ytdlp.py:298
 msgid "Settings"
 msgstr "设置"
 
-#: ../vdms_dialogs/preferences.py:432
+#: ../vdms_dialogs/preferences.py:467
 #, fuzzy
 msgid "By assigning an additional suffix you could avoid overwriting files"
 msgstr "通过指定一个额外的后缀，你可以避免重写文件"
 
-#: ../vdms_dialogs/preferences.py:586
+#: ../vdms_dialogs/preferences.py:623
 #, fuzzy
 msgid "Set a persistent location to save exported files"
 msgstr "设置一个持久的位置来保存导出的文件"
 
-#: ../vdms_dialogs/preferences.py:618
+#: ../vdms_dialogs/preferences.py:655
 #, fuzzy
 msgid ""
 "Enter only alphanumeric characters. You can also use the hyphen (\"-\") and "
 "the underscore (\"_\"). Spaces are not allowed."
 msgstr ""
 "只输入字母数字字符。你也可以使用连字符（\"-\"）和下划线（\"_\"）。不允许有空"
 "格。"
 
-#: ../vdms_dialogs/preferences.py:666
+#: ../vdms_dialogs/preferences.py:703
 #, fuzzy
 msgid "Choose a new destination for the files to be trashed"
 msgstr "为要销毁的文件选择一个新的目的地"
 
-#: ../vdms_dialogs/preferences.py:683
+#: ../vdms_dialogs/preferences.py:720
 #, fuzzy
 msgid "Set a persistent location to save the file downloads"
 msgstr "设置一个持久的位置来保存文件下载"
 
 #: ../vdms_dialogs/videomass_check_version.py:63
 msgid "Get Latest Version"
 msgstr "获取最新版本"
@@ -1277,15 +1309,15 @@
 
 #: ../vdms_dialogs/mediainfo.py:133
 msgid "FILE SELECTION"
 msgstr "文件选择"
 
 #: ../vdms_dialogs/mediainfo.py:135 ../vdms_dialogs/mediainfo.py:138
 #: ../vdms_dialogs/mediainfo.py:141 ../vdms_dialogs/mediainfo.py:144
-#: ../vdms_main/main_frame.py:1274
+#: ../vdms_main/main_frame.py:1275
 #, fuzzy
 #| msgid "Audio Properties"
 msgid "Properties"
 msgstr "音频属性"
 
 #: ../vdms_dialogs/mediainfo.py:136 ../vdms_dialogs/mediainfo.py:139
 #: ../vdms_dialogs/mediainfo.py:142 ../vdms_dialogs/mediainfo.py:145
@@ -1868,64 +1900,64 @@
 msgid "Seconds"
 msgstr ""
 
 #: ../vdms_miniframes/timeline.py:108
 msgid "Milliseconds"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:189 ../vdms_miniframes/timeline.py:309
+#: ../vdms_miniframes/timeline.py:188 ../vdms_miniframes/timeline.py:311
 msgid "No source duration:"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:210 ../vdms_miniframes/timeline.py:295
-#: ../vdms_miniframes/timeline.py:335 ../vdms_miniframes/timeline.py:340
-#: ../vdms_miniframes/timeline.py:439
+#: ../vdms_miniframes/timeline.py:208 ../vdms_miniframes/timeline.py:297
+#: ../vdms_miniframes/timeline.py:337 ../vdms_miniframes/timeline.py:342
+#: ../vdms_miniframes/timeline.py:445
 #, python-brace-format
 msgid "{0} {1}  |  Segment Duration: {2}"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:257 ../vdms_miniframes/timeline.py:274
+#: ../vdms_miniframes/timeline.py:259 ../vdms_miniframes/timeline.py:276
 msgid "End adjustment"
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:258 ../vdms_miniframes/timeline.py:276
+#: ../vdms_miniframes/timeline.py:260 ../vdms_miniframes/timeline.py:278
 #, fuzzy
 #| msgid "Starts"
 msgid "Start adjustment"
 msgstr "开始"
 
-#: ../vdms_miniframes/timeline.py:320
+#: ../vdms_miniframes/timeline.py:322
 #, fuzzy
 #| msgid "Duration:"
 msgid "Source duration:"
 msgstr "持续时间："
 
-#: ../vdms_miniframes/timeline.py:388
+#: ../vdms_miniframes/timeline.py:391
 msgid "WARNING: Invalid selection, out of range."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:459
+#: ../vdms_miniframes/timeline.py:465
 msgid ""
 "Start by dragging the bottom left handle,\n"
 "or right-click for options."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:493
+#: ../vdms_miniframes/timeline.py:500
 #, fuzzy
 #| msgid "Starts"
 msgid "Start"
 msgstr "开始"
 
-#: ../vdms_miniframes/timeline.py:494
+#: ../vdms_miniframes/timeline.py:501
 #, fuzzy
 #| msgid "Enabled"
 msgid "End"
 msgstr "已启用"
 
-#: ../vdms_miniframes/timeline.py:542
+#: ../vdms_miniframes/timeline.py:549
 msgid ""
 "The timeline editor is a tool that allows you to trim slices of time on "
 "selected imported media (see Queued Files panel).\n"
 "\n"
 "The \"time format\" used to report durations is expressed in hours, minutes, "
 "seconds and milliseconds (HH:MM:SS.ms).\n"
 "\n"
@@ -1938,51 +1970,47 @@
 "duration of a selected source file (see status bar messages).\n"
 "\n"
 "The \"Start\"/\"End\" duration values always refer to the initial position "
 "of the timeline: 00:00:00.000. For other informations as the segment "
 "duration and warnings, please refer to the status bar messages."
 msgstr ""
 
-#: ../vdms_miniframes/timeline.py:559
+#: ../vdms_miniframes/timeline.py:566
 #, fuzzy
 #| msgid "Show timeline\tCtrl+T"
 msgid "Timeline Editor Usage"
 msgstr "显示时间线\tCtrl+T"
 
-#: ../vdms_io/checkup.py:45
+#: ../vdms_io/checkup.py:47
 #, fuzzy
-msgid ""
-"Already exist: \n"
-"\n"
-"{}\n"
-"\n"
-"Do you want to overwrite? "
+#| msgid "A file with this name already exists, do you want to overwrite it?"
+msgid "Files already exist, do you want to overwrite them?"
+msgstr "已经有一个以此为名的文件，你想覆盖它吗？"
+
+#: ../vdms_io/checkup.py:49
+msgid "Already exist"
 msgstr ""
-"Already exist: \n"
-"\n"
-"\n"
-"\n"
-"你想覆盖吗？"
 
-#: ../vdms_io/checkup.py:48
+#: ../vdms_io/checkup.py:50
 msgid "Please Confirm"
 msgstr "请确认"
 
-#: ../vdms_io/checkup.py:54 ../vdms_panels/sequence_to_video.py:581
-#: ../vdms_panels/sequence_to_video.py:605
-msgid ""
-"File does not exist:\n"
-"\n"
-"\"{}\"\n"
+#: ../vdms_io/checkup.py:62
+msgid "No source files found in the specified path"
 msgstr ""
-"文件不存在：\n"
-"\n"
-"\"{}\"\n"
 
-#: ../vdms_io/checkup.py:62
+#: ../vdms_io/checkup.py:64
+msgid "Not found"
+msgstr "未找到"
+
+#: ../vdms_io/checkup.py:65
+msgid "Non-existent source files"
+msgstr ""
+
+#: ../vdms_io/checkup.py:75
 msgid ""
 "Output folder does not exist:\n"
 "\n"
 "\"{}\"\n"
 msgstr ""
 "输出文件夹不存在：\n"
 "\n"
@@ -2052,44 +2080,44 @@
 "Possible solution: open the Presets Manager panel, go to the presets column "
 "and try to click the \"Restore all...\" button"
 msgstr ""
 "No presets found.\n"
 "\n"
 "可能的解决方案：打开预设管理器面板，进入预设栏，尝试点击 \"恢复所有... \"按钮"
 
-#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1372
-#: ../vdms_main/main_frame.py:1402 ../vdms_ytdlp/main_ytdlp.py:99
+#: ../vdms_main/main_frame.py:193 ../vdms_main/main_frame.py:1373
+#: ../vdms_main/main_frame.py:1403 ../vdms_ytdlp/main_ytdlp.py:99
 #: ../vdms_ytdlp/main_ytdlp.py:148 ../vdms_ytdlp/main_ytdlp.py:566
-#: ../vdms_ytdlp/textdrop.py:219 ../vdms_ytdlp/youtubedl_ui.py:451
+#: ../vdms_ytdlp/textdrop.py:224 ../vdms_ytdlp/youtubedl_ui.py:451
 msgid "Ready"
 msgstr "准备就绪"
 
 #: ../vdms_main/main_frame.py:344 ../vdms_ytdlp/main_ytdlp.py:204
 #, fuzzy
 msgid ""
 "There are still processes running. if you want to stop them, use the \"Abort"
 "\" button."
 msgstr ""
 "仍有一些进程在运行。如果你想停止它们，请使用 \"中止 \"按钮。\n"
 "\n"
 "你想杀死应用程序吗？"
 
-#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1075
-#: ../vdms_main/main_frame.py:1371 ../vdms_ytdlp/main_ytdlp.py:147
+#: ../vdms_main/main_frame.py:346 ../vdms_main/main_frame.py:1076
+#: ../vdms_main/main_frame.py:1372 ../vdms_ytdlp/main_ytdlp.py:147
 #: ../vdms_ytdlp/main_ytdlp.py:206
 msgid "Videomass"
 msgstr "Videomass"
 
 #: ../vdms_main/main_frame.py:350
 #, fuzzy
 #| msgid "Are you sure you want to exit?"
 msgid "Are you sure you want to exit the application?"
 msgstr "你确定你要退出吗？"
 
-#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1080
+#: ../vdms_main/main_frame.py:352 ../vdms_main/main_frame.py:1081
 #: ../vdms_ytdlp/main_ytdlp.py:212
 msgid "Exit"
 msgstr "退出"
 
 #: ../vdms_main/main_frame.py:358 ../vdms_main/main_frame.py:383
 msgid ""
 "There are still active windows with running processes, make sure you finish "
@@ -2290,15 +2318,15 @@
 
 #: ../vdms_main/main_frame.py:520
 #, fuzzy
 #| msgid "Home panel\tShift+H"
 msgid "Home panel\tCtrl+Shift+H"
 msgstr "主界面\tShift+H"
 
-#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1263
+#: ../vdms_main/main_frame.py:521 ../vdms_main/main_frame.py:1264
 msgid "Go to the 'Home' panel"
 msgstr "转到 \"主页 \"面板"
 
 #: ../vdms_main/main_frame.py:524
 #, fuzzy
 #| msgid "Presets Manager\tShift+P"
 msgid "Presets Manager\tCtrl+Shift+P"
@@ -2372,15 +2400,15 @@
 msgid "Keeps track of the output for debugging errors"
 msgstr "为调试错误保持输出跟踪"
 
 #: ../vdms_main/main_frame.py:547
 msgid "Goto"
 msgstr "转到"
 
-#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:305
+#: ../vdms_main/main_frame.py:551 ../vdms_panels/filedrop.py:310
 msgid "Set up a temporary folder for conversions"
 msgstr "设置一个临时文件夹用于转换"
 
 #: ../vdms_main/main_frame.py:552
 msgid "Use a temporary location to save conversions"
 msgstr "使用一个临时位置来保存转换结果"
 
@@ -2488,197 +2516,197 @@
 msgid "Help"
 msgstr "帮助"
 
 #: ../vdms_main/main_frame.py:677
 msgid "Open the selected files"
 msgstr "打开选定的文件"
 
-#: ../vdms_main/main_frame.py:729 ../vdms_main/main_frame.py:752
+#: ../vdms_main/main_frame.py:730 ../vdms_main/main_frame.py:753
 #, fuzzy
 msgid "No such folder '{}'"
 msgstr "没有这样的文件夹'{}'"
 
-#: ../vdms_main/main_frame.py:741
+#: ../vdms_main/main_frame.py:742
 msgid "Are you sure to empty trash folder?"
 msgstr "你确定清空垃圾文件夹吗?"
 
-#: ../vdms_main/main_frame.py:749
+#: ../vdms_main/main_frame.py:750
 #, fuzzy
 msgid "No files to delete"
 msgstr "没有要删除的文件"
 
-#: ../vdms_main/main_frame.py:804
+#: ../vdms_main/main_frame.py:805
 #, python-brace-format
 msgid "Installed release v{0}. A new presets release is available {1}"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:808
+#: ../vdms_main/main_frame.py:809
 #, python-brace-format
 msgid "Installed release v{0}. No new updates found."
 msgstr ""
 
-#: ../vdms_main/main_frame.py:821
+#: ../vdms_main/main_frame.py:822
 msgid "Choose a download folder"
 msgstr "选择一个下载文件夹"
 
-#: ../vdms_main/main_frame.py:838
+#: ../vdms_main/main_frame.py:839
 #, fuzzy
 msgid ""
 "Wait....\n"
 "The archive is being downloaded"
 msgstr ""
 "Wait....\n"
 "档案正在下载中"
 
-#: ../vdms_main/main_frame.py:849
+#: ../vdms_main/main_frame.py:850
 #, python-brace-format
 msgid "Successfully downloaded to \"{0}\""
 msgstr "成功下载到\"{0}\"。"
 
-#: ../vdms_main/main_frame.py:999
+#: ../vdms_main/main_frame.py:1000
 msgid "Choose a temporary destination for conversions"
 msgstr "为转换选择一个临时目的地"
 
-#: ../vdms_main/main_frame.py:1024
+#: ../vdms_main/main_frame.py:1025
 #, fuzzy
 msgid "Default destination folders successfully restored"
 msgstr "成功恢复了默认的目标文件夹"
 
-#: ../vdms_main/main_frame.py:1073
+#: ../vdms_main/main_frame.py:1074
 msgid "Changes will take effect once the program has been restarted."
 msgstr "一旦程序被重新启动，更改就会生效"
 
-#: ../vdms_main/main_frame.py:1077
+#: ../vdms_main/main_frame.py:1078
 msgid ""
 "Changes will take effect once the program has been restarted.\n"
 "\n"
 "Do you want to exit the application now?"
 msgstr ""
 "一旦程序被重新启动，更改就会生效。\n"
 "\n"
 "你想现在退出程序吗？"
 
-#: ../vdms_main/main_frame.py:1150
+#: ../vdms_main/main_frame.py:1151
 #, python-brace-format
 msgid "A new release is available - v.{0}\n"
 msgstr ""
 "一个新的版本已经推出--v.{0}/n\n"
 "\n"
 
-#: ../vdms_main/main_frame.py:1153
+#: ../vdms_main/main_frame.py:1154
 msgid "You are using a development version that has not yet been released!\n"
 msgstr ""
 "您正在使用一个开发版本尚未发布！\n"
 "\n"
 
-#: ../vdms_main/main_frame.py:1156
+#: ../vdms_main/main_frame.py:1157
 #, fuzzy
 msgid "Congratulation! You are already using the latest version.\n"
 msgstr ""
 "祝贺你! You are already using the latest version./n\n"
 "\n"
 
-#: ../vdms_main/main_frame.py:1253 ../vdms_ytdlp/main_ytdlp.py:486
+#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:486
 msgid "Go to the previous panel"
 msgstr "转到上一个面板"
 
-#: ../vdms_main/main_frame.py:1254 ../vdms_ytdlp/main_ytdlp.py:487
+#: ../vdms_main/main_frame.py:1255 ../vdms_ytdlp/main_ytdlp.py:487
 msgid "Back"
 msgstr "Back"
 
-#: ../vdms_main/main_frame.py:1258 ../vdms_ytdlp/main_ytdlp.py:491
+#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:491
 msgid "Go to the next panel"
 msgstr "转到下一个面板"
 
-#: ../vdms_main/main_frame.py:1259 ../vdms_ytdlp/main_ytdlp.py:492
+#: ../vdms_main/main_frame.py:1260 ../vdms_ytdlp/main_ytdlp.py:492
 #, fuzzy
 msgid "Next"
 msgstr "下一页"
 
-#: ../vdms_main/main_frame.py:1264
+#: ../vdms_main/main_frame.py:1265
 msgid "Home"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1268
+#: ../vdms_main/main_frame.py:1269
 msgid "Play the selected file in the list"
 msgstr "播放列表中选定的文件"
 
-#: ../vdms_main/main_frame.py:1269
+#: ../vdms_main/main_frame.py:1270
 msgid "Play"
 msgstr "播放"
 
-#: ../vdms_main/main_frame.py:1273
+#: ../vdms_main/main_frame.py:1274
 #, fuzzy
 #| msgid "Gathers information of multimedia streams"
 msgid "Get informative data about imported media streams"
 msgstr "收集多媒体流的信息"
 
-#: ../vdms_main/main_frame.py:1278
+#: ../vdms_main/main_frame.py:1279
 #, fuzzy
 #| msgid "Starts"
 msgid "Start rendering"
 msgstr "开始"
 
-#: ../vdms_main/main_frame.py:1279
+#: ../vdms_main/main_frame.py:1280
 msgid "Run"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1283 ../vdms_ytdlp/main_ytdlp.py:506
+#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:506
 msgid "Stops current process"
 msgstr "停止当前过程"
 
-#: ../vdms_main/main_frame.py:1284 ../vdms_ytdlp/main_ytdlp.py:507
+#: ../vdms_main/main_frame.py:1285 ../vdms_ytdlp/main_ytdlp.py:507
 msgid "Abort"
 msgstr "中止"
 
-#: ../vdms_main/main_frame.py:1288
+#: ../vdms_main/main_frame.py:1289
 msgid "Delete all files from the list"
 msgstr "删除列表中的所有文件"
 
-#: ../vdms_main/main_frame.py:1289 ../vdms_ytdlp/main_ytdlp.py:511
+#: ../vdms_main/main_frame.py:1290 ../vdms_ytdlp/main_ytdlp.py:511
 msgid "Clear"
 msgstr ""
 
-#: ../vdms_main/main_frame.py:1403
+#: ../vdms_main/main_frame.py:1404
 #, fuzzy
 msgid "Videomass - Queued Files"
 msgstr "Videomass - 排队的文件"
 
-#: ../vdms_main/main_frame.py:1420
+#: ../vdms_main/main_frame.py:1421
 msgid "Videomass - AV Conversions"
 msgstr "Videomass - AV转换"
 
-#: ../vdms_main/main_frame.py:1444
+#: ../vdms_main/main_frame.py:1445
 msgid "Videomass - Presets Manager"
 msgstr "Videomass - 预设管理器"
 
-#: ../vdms_main/main_frame.py:1469
+#: ../vdms_main/main_frame.py:1470
 #, fuzzy
 msgid "Videomass - Concatenate Demuxer"
 msgstr "Videomass - Concatenate Demuxer"
 
-#: ../vdms_main/main_frame.py:1493
+#: ../vdms_main/main_frame.py:1494
 #, fuzzy
 msgid "Videomass - From Movie to Pictures"
 msgstr "Videomass - 从电影到图片"
 
-#: ../vdms_main/main_frame.py:1517
+#: ../vdms_main/main_frame.py:1518
 #, fuzzy
 msgid "Videomass - Still Image Maker"
 msgstr "Videomass - 静态图像制作"
 
-#: ../vdms_main/main_frame.py:1534 ../vdms_ytdlp/main_ytdlp.py:589
+#: ../vdms_main/main_frame.py:1535 ../vdms_ytdlp/main_ytdlp.py:589
 msgid "Viewing last log"
 msgstr "查看最后的日志"
 
-#: ../vdms_main/main_frame.py:1542
+#: ../vdms_main/main_frame.py:1543
 msgid "Processing..."
 msgstr "处理..."
 
-#: ../vdms_main/main_frame.py:1546
+#: ../vdms_main/main_frame.py:1547
 #, fuzzy
 msgid "Videomass - FFmpeg message monitor"
 msgstr "Videomass - 输出监控"
 
 #: ../vdms_panels/av_conversions.py:221
 msgid "Media:"
 msgstr "媒体："
@@ -3034,20 +3062,20 @@
 msgid "{} file in queue"
 msgstr "{}队列中的文件"
 
 #: ../vdms_panels/av_conversions.py:2246
 msgid "Off"
 msgstr "关闭"
 
-#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:932
+#: ../vdms_panels/av_conversions.py:2252 ../vdms_panels/presets_manager.py:933
 #: ../vdms_panels/video_to_sequence.py:587
 msgid "Unset"
 msgstr "未设置"
 
-#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:935
+#: ../vdms_panels/av_conversions.py:2255 ../vdms_panels/presets_manager.py:936
 #: ../vdms_panels/video_to_sequence.py:590
 msgid "start  {} | duration  {}"
 msgstr "start  {} | duration  {}"
 
 #: ../vdms_panels/av_conversions.py:2261
 #, fuzzy
 msgid ""
@@ -3267,15 +3295,15 @@
 
 #: ../vdms_panels/choose_topic.py:137
 msgid "Extract images (frames) from your movies in JPG, PNG, BMP, GIF formats."
 msgstr "从你的电影中提取JPG、PNG、BMP、GIF格式的图像（帧）。"
 
 #: ../vdms_panels/choose_topic.py:223
 #, fuzzy
-msgid "The downloader is disabled. Check your preferences."
+msgid "yt-dlp is disabled. Check your preferences."
 msgstr "下载器被禁用。检查你的偏好。"
 
 #: ../vdms_panels/concatenate.py:78
 #, fuzzy
 msgid ""
 "\n"
 "- The concatenation function is performed only with Audio files or only with "
@@ -3377,126 +3405,135 @@
 "\n"
 "File to concatenate\n"
 "Output filename （输出文件名）。\n"
 "Destination （目的地）。\n"
 "Output Format\n"
 "Time Period"
 
-#: ../vdms_panels/filedrop.py:44
+#: ../vdms_panels/filedrop.py:45
 msgid "File has illegal characters like:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:45
+#: ../vdms_panels/filedrop.py:46
 #, fuzzy
 #| msgid "Invalid filename. Contains double or single quotes"
 msgid "Invalid path name. Contains double or single quotes"
 msgstr "无效的文件名。含有双引号或单引号"
 
-#: ../vdms_panels/filedrop.py:46
+#: ../vdms_panels/filedrop.py:47
 #, fuzzy
 msgid "Directories are not allowed, just add files, please."
 msgstr "不允许有目录，只允许添加文件，谢谢。"
 
-#: ../vdms_panels/filedrop.py:47
+#: ../vdms_panels/filedrop.py:48
 msgid ""
 "File without format extension: please give an appropriate extension to the "
 "file name, example '.mkv', '.avi', '.mp3', etc."
 msgstr ""
 "没有格式扩展名的文件：请给文件名加上适当的扩展名，例如\".mkv\"、\".avi\"、\"."
 "mp3 \"等。"
 
-#: ../vdms_panels/filedrop.py:83
+#: ../vdms_panels/filedrop.py:84
 #, python-brace-format
 msgid "Name has illegal characters like: {0}"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:84
+#: ../vdms_panels/filedrop.py:85
 msgid "Name already in use:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:139
+#: ../vdms_panels/filedrop.py:132
 msgid "File Name"
 msgstr "文件名称"
 
-#: ../vdms_panels/filedrop.py:140
+#: ../vdms_panels/filedrop.py:133
 msgid "Duration"
 msgstr "持续时间"
 
-#: ../vdms_panels/filedrop.py:141
+#: ../vdms_panels/filedrop.py:134
 msgid "Media type"
 msgstr "媒体类型"
 
-#: ../vdms_panels/filedrop.py:142 ../vdms_ytdlp/formatcode.py:135
+#: ../vdms_panels/filedrop.py:135 ../vdms_ytdlp/formatcode.py:135
 msgid "Size"
 msgstr "大小"
 
-#: ../vdms_panels/filedrop.py:143
+#: ../vdms_panels/filedrop.py:136
 #, fuzzy
 #| msgid "Restrict file names"
 msgid "Output file name"
 msgstr "限制文件名"
 
-#: ../vdms_panels/filedrop.py:207
+#: ../vdms_panels/filedrop.py:197
+msgid "Duplicate file, it has already been added to the list."
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:206
+msgid "See the error message next to each path name"
+msgstr ""
+
+#: ../vdms_panels/filedrop.py:209
 #, fuzzy
-msgid "Duplicate files are rejected: > {}"
-msgstr "重复的文件被拒绝。> {}"
+#| msgid "Add Files"
+msgid "Rejected Files"
+msgstr "添加文件"
 
-#: ../vdms_panels/filedrop.py:273 ../vdms_panels/filedrop.py:325
+#: ../vdms_panels/filedrop.py:278 ../vdms_panels/filedrop.py:330
 msgid "Drag one or more files below"
 msgstr "拖动下面的一个或多个文件"
 
-#: ../vdms_panels/filedrop.py:307 ../vdms_ytdlp/textdrop.py:163
+#: ../vdms_panels/filedrop.py:312 ../vdms_ytdlp/textdrop.py:168
 #, fuzzy
 msgid "Destination folder"
 msgstr "目的地文件夹"
 
-#: ../vdms_panels/filedrop.py:328
+#: ../vdms_panels/filedrop.py:333
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag the images below"
 msgstr "拖动下面的一个或多个文件"
 
-#: ../vdms_panels/filedrop.py:331
+#: ../vdms_panels/filedrop.py:336
 #, fuzzy
 #| msgid "Drag one or more files below"
 msgid "Drag one or more video below"
 msgstr "拖动下面的一个或多个文件"
 
-#: ../vdms_panels/filedrop.py:413
+#: ../vdms_panels/filedrop.py:418
 #, fuzzy
 msgid "No file selected"
 msgstr "没有选择文件"
 
-#: ../vdms_panels/filedrop.py:531
+#: ../vdms_panels/filedrop.py:528
 #, fuzzy
 #| msgid "File name"
 msgid "File renaming..."
 msgstr "文件名称"
 
-#: ../vdms_panels/filedrop.py:532
+#: ../vdms_panels/filedrop.py:529
 #, fuzzy
 #| msgid "Open the selected files"
 msgid "Rename the selected file to:"
 msgstr "打开选定的文件"
 
-#: ../vdms_panels/filedrop.py:546 ../vdms_panels/filedrop.py:556
-#: ../vdms_panels/filedrop.py:587
+#: ../vdms_panels/filedrop.py:543 ../vdms_panels/filedrop.py:553
+#: ../vdms_panels/filedrop.py:584
 msgid "Add Files"
 msgstr "添加文件"
 
-#: ../vdms_panels/filedrop.py:563
+#: ../vdms_panels/filedrop.py:560
 msgid "Rename items"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:564
+#: ../vdms_panels/filedrop.py:561
 #, python-brace-format
 msgid "Rename the {0} items to:"
 msgstr ""
 
-#: ../vdms_panels/filedrop.py:566
+#: ../vdms_panels/filedrop.py:563
 #, fuzzy
 #| msgid "File Name"
 msgid "New Name #"
 msgstr "文件名称"
 
 #: ../vdms_panels/long_processing_task.py:107
 #: ../vdms_ytdlp/long_task_ytdlp.py:43
@@ -3924,20 +3961,20 @@
 msgid ""
 "The selected profile command has been changed manually.\n"
 "Do you want to apply it during the conversion process?"
 msgstr ""
 "所选的配置文件命令已被手动更改。\n"
 "你想在转换过程中应用它吗？"
 
-#: ../vdms_panels/presets_manager.py:842
+#: ../vdms_panels/presets_manager.py:843
 #, fuzzy
 msgid "Don't show this dialog again"
 msgstr "不要再显示这个对话框"
 
-#: ../vdms_panels/presets_manager.py:939
+#: ../vdms_panels/presets_manager.py:940
 #, fuzzy
 msgid ""
 "Queued File\n"
 "Pass Encoding\n"
 "Profile Used\n"
 "Output Format\n"
 "Time Period"
@@ -3975,26 +4012,28 @@
 #| "with a progressive digit, in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more image files such as JPG, PNG and BMP formats, then "
 "select one.\n"
 "\n"
 "2. Use the Resizing function to resize images which have different sizes "
-"such as width and height. It is optional in other cases.\n"
+"such as width and\n"
+"height. It is optional in other cases.\n"
 "\n"
 "3. Use the Timeline editor (CTRL+T) to set the time interval between images "
-"by adjusting the \"End\" duration value and\n"
-"leaving the \"Start\" value at 00:00:00.000.\n"
+"by adjusting\n"
+"the \"End\" duration value and leaving the \"Start\" value at 00:00:00.000.\n"
 "\n"
 "4. Run the conversion.\n"
 "\n"
 "\n"
 "The produced video will have the name of the selected file in the 'Queued "
-"File' list, which will be saved in a folder named 'Still_Images'\n"
-"with a progressive digit, in the path you specify."
+"File' list, which\n"
+"will be saved in a folder named 'Still_Images' with a progressive digit, in "
+"the path you specify."
 msgstr ""
 "\n"
 "1. 导入一个或多个图像文件，如JPG、PNG和BMP格式，然后选择一个。\n"
 "\n"
 "2. 使用调整大小功能来调整具有不同尺寸的图像，如宽度和高度。在其他情况下，它是"
 "可选的。\n"
 "\n"
@@ -4067,14 +4106,25 @@
 msgstr "无效文件：'{}'"
 
 #: ../vdms_panels/sequence_to_video.py:575
 #: ../vdms_panels/sequence_to_video.py:600
 msgid "Unsupported format '{}'"
 msgstr "不支持的格式'{}'"
 
+#: ../vdms_panels/sequence_to_video.py:581
+#: ../vdms_panels/sequence_to_video.py:605
+msgid ""
+"File does not exist:\n"
+"\n"
+"\"{}\"\n"
+msgstr ""
+"文件不存在：\n"
+"\n"
+"\"{}\"\n"
+
 #: ../vdms_panels/sequence_to_video.py:719
 #, fuzzy
 msgid ""
 "File to process\n"
 "Output filename\n"
 "Destination Folder\n"
 "Output Format\n"
@@ -4197,24 +4247,24 @@
 #| "with a progressive digit, \n"
 #| "in the path you specify."
 msgid ""
 "\n"
 "1. Import one or more video files, then select one.\n"
 "\n"
 "2. To select a slice of time use the Timeline editor (CTRL+T) by adjusting "
-"the \"End\" and the \"Start\" duration values.\n"
+"the\n"
+"\"End\" and the \"Start\" duration values.\n"
 "\n"
 "3. Select an output format (jpg, png, bmp).\n"
 "\n"
 "4. Start the conversion.\n"
 "\n"
 "\n"
-"The images produced will be saved in a folder named 'Movie_to_Pictures' with "
-"a progressive digit, \n"
-"in the path you specify."
+"The images produced will be saved in a folder named 'Movie_to_Pictures'\n"
+"with a progressive digit, in the path you specify."
 msgstr ""
 "\n"
 "1. 导入一个或多个视频文件，然后选择一个。\n"
 "\n"
 "2. 使用时间线编辑器（CTRL+T）滚动DURATION和SEEK滑块来选择一个时间片段。\n"
 "\n"
 "3. 选择一个输出格式（jpg、png、bmp）。\n"
@@ -4314,15 +4364,15 @@
 "At least one \"Format Code\" must be checked for each URL selected in green."
 msgstr "对于每个以绿色选择的URL，必须至少勾选一个 \"格式代码\"。"
 
 #: ../vdms_ytdlp/formatcode.py:127
 msgid "Format Code"
 msgstr "格式代码"
 
-#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:63
+#: ../vdms_ytdlp/formatcode.py:128 ../vdms_ytdlp/textdrop.py:59
 msgid "Url"
 msgstr "网址"
 
 #: ../vdms_ytdlp/formatcode.py:129
 msgid "Title"
 msgstr "标题"
 
@@ -4411,27 +4461,27 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:263
 #, fuzzy
 #| msgid "YouTube Downloader"
 msgid "Quit YouTube Downloader"
 msgstr "YouTube下载器"
 
-#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:179
-#: ../vdms_ytdlp/textdrop.py:195
+#: ../vdms_ytdlp/main_ytdlp.py:268 ../vdms_ytdlp/textdrop.py:184
+#: ../vdms_ytdlp/textdrop.py:200
 #, fuzzy
 #| msgid "Exit\tCtrl+Q"
 msgid "Paste\tCtrl+V"
 msgstr "退出\tCtrl+Q"
 
 #: ../vdms_ytdlp/main_ytdlp.py:269
 msgid "Paste the copied URLs to clipboard"
 msgstr ""
 
-#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:180
-#: ../vdms_ytdlp/textdrop.py:198
+#: ../vdms_ytdlp/main_ytdlp.py:271 ../vdms_ytdlp/textdrop.py:185
+#: ../vdms_ytdlp/textdrop.py:203
 msgid "Remove selected URL\tDEL"
 msgstr ""
 
 #: ../vdms_ytdlp/main_ytdlp.py:272
 #, fuzzy
 #| msgid "Remove the selected files from the list"
 msgid "Remove the selected URL from the list"
@@ -4453,15 +4503,15 @@
 
 #: ../vdms_ytdlp/main_ytdlp.py:282
 #, fuzzy
 #| msgid "Shows the latest version available on github.com"
 msgid "Check the latest version available on github.com"
 msgstr "显示github.com上的最新版本"
 
-#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:161
+#: ../vdms_ytdlp/main_ytdlp.py:289 ../vdms_ytdlp/textdrop.py:166
 msgid "Set up a temporary folder for downloads"
 msgstr "设置一个临时文件夹用于下载"
 
 #: ../vdms_ytdlp/main_ytdlp.py:290
 msgid "Save all downloads to this temporary location"
 msgstr "将所有的下载保存到这个临时位置"
 
@@ -4582,21 +4632,29 @@
 #: ../vdms_ytdlp/playlist_indexing.py:256
 #, fuzzy
 msgid ""
 "WARNING: The selected URL does not refer to a playlist. Only lines marked "
 "green can be indexed."
 msgstr "警告：所选的URL并不是指一个播放列表。只有标记为绿色的行可以被索引。"
 
-#: ../vdms_ytdlp/textdrop.py:74
+#: ../vdms_ytdlp/textdrop.py:68
 #, fuzzy
 #| msgid "ERROR: Invalid URL: \"{}\""
-msgid "Invalid URL:"
+msgid "Invalid URL"
 msgstr "ERROR: 无效的URL。\"{}\""
 
-#: ../vdms_ytdlp/textdrop.py:130
+#: ../vdms_ytdlp/textdrop.py:84
+msgid "List of rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:87
+msgid "Rejected URLs"
+msgstr ""
+
+#: ../vdms_ytdlp/textdrop.py:135
 msgid "Drag or paste URLs here"
 msgstr ""
 
 #: ../vdms_ytdlp/ydl_mediainfo.py:67
 #, fuzzy
 msgid "Statistics viewer"
 msgstr "统计数据查看器"
@@ -4713,14 +4771,32 @@
 msgstr "这些URL包含播放列表。你确定要继续吗？"
 
 #: ../vdms_ytdlp/youtubedl_ui.py:659
 #, fuzzy
 msgid "The URLs contain channels. Are you sure you want to continue?"
 msgstr "URL包含通道。你确定要继续吗？"
 
+#, fuzzy
+#~ msgid ""
+#~ "Already exist: \n"
+#~ "\n"
+#~ "{}\n"
+#~ "\n"
+#~ "Do you want to overwrite? "
+#~ msgstr ""
+#~ "Already exist: \n"
+#~ "\n"
+#~ "\n"
+#~ "\n"
+#~ "你想覆盖吗？"
+
+#, fuzzy
+#~ msgid "Duplicate files are rejected: > {}"
+#~ msgstr "重复的文件被拒绝。> {}"
+
 #~ msgid "File list changed, please check the settings again."
 #~ msgstr "文件列表改变了，请再次检查设置。"
 
 #~ msgid ""
 #~ "Cannot continue: The duration in the timeline exceeds the duration of "
 #~ "some queued files."
 #~ msgstr "不能继续。时间线中的持续时间超过了某些排队文件的持续时间。"
@@ -4870,17 +4946,14 @@
 #~ "Make sure you are using the latest available version of\n"
 #~ "'{}'. This allows you to avoid download problems.\n"
 #~ msgstr ""
 #~ "请确保你使用的是最新的可用版本的\n"
 #~ "'{}'. 这可以让你避免下载问题。\n"
 #~ "\n"
 
-#~ msgid "Not found"
-#~ msgstr "未找到"
-
 #~ msgid "Not Installed"
 #~ msgstr "未安装"
 
 #~ msgid "Downloader"
 #~ msgstr "下载器"
 
 #~ msgid "Topic List..."
@@ -5031,19 +5104,14 @@
 
 #, fuzzy
 #~| msgid "Duration"
 #~ msgid "Duration minutes"
 #~ msgstr "持续时间"
 
 #, fuzzy
-#~| msgid "Duration"
-#~ msgid "Duration seconds"
-#~ msgstr "持续时间"
-
-#, fuzzy
 #~| msgid "Starts"
 #~ msgid "Start hours"
 #~ msgstr "开始"
 
 #, fuzzy
 #~ msgid "Show panel for editing timeline (seek/duration)"
 #~ msgstr "显示编辑时间线的面板（寻路/时间）。"
```

### Comparing `videomass-5.0.0/videomass/share/presets/Audio_Conversions.prst` & `videomass-5.0.1/videomass/share/presets/Audio_Conversions.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Audio_removing_from_video.prst` & `videomass-5.0.1/videomass/share/presets/Audio_removing_from_video.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Coding to DVD by GMJCZP.prst` & `videomass-5.0.1/videomass/share/presets/Coding to DVD by GMJCZP.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Coding-to-DVD-by-GMJCZP.md` & `videomass-5.0.1/videomass/share/presets/Coding-to-DVD-by-GMJCZP.md`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Create animated GIFs.prst` & `videomass-5.0.1/videomass/share/presets/Create animated GIFs.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Embed_Subtitles_to_Video.prst` & `videomass-5.0.1/videomass/share/presets/Embed_Subtitles_to_Video.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Encoding_for_Devices.prst` & `videomass-5.0.1/videomass/share/presets/Encoding_for_Devices.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Extract_audio_from_Videos.prst` & `videomass-5.0.1/videomass/share/presets/Extract_audio_from_Videos.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/For_Archive_Collection.prst` & `videomass-5.0.1/videomass/share/presets/For_Archive_Collection.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Merging_audio_and_video.prst` & `videomass-5.0.1/videomass/share/presets/Merging_audio_and_video.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Utilities.prst` & `videomass-5.0.1/videomass/share/presets/Utilities.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Video Encoding AV1.prst` & `videomass-5.0.1/videomass/share/presets/Video Encoding AV1.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Video Encoding VP9-WebM.prst` & `videomass-5.0.1/videomass/share/presets/Video Encoding VP9-WebM.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Video effects.prst` & `videomass-5.0.1/videomass/share/presets/Video effects.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Video-Repair.prst` & `videomass-5.0.1/videomass/share/presets/Video-Repair.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Video_Stabilizer.prst` & `videomass-5.0.1/videomass/share/presets/Video_Stabilizer.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/share/presets/Video_Streaming.prst` & `videomass-5.0.1/videomass/share/presets/Video_Streaming.prst`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/about.py` & `videomass-5.0.1/videomass/vdms_dialogs/about.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/audiodialogs.py` & `videomass-5.0.1/videomass/vdms_dialogs/audiodialogs.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/epilogue.py` & `videomass-5.0.1/videomass/vdms_dialogs/epilogue.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/ffmpeg_codecs.py` & `videomass-5.0.1/videomass/vdms_dialogs/ffmpeg_codecs.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/ffmpeg_conf.py` & `videomass-5.0.1/videomass/vdms_dialogs/ffmpeg_conf.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/ffmpeg_formats.py` & `videomass-5.0.1/videomass/vdms_dialogs/ffmpeg_formats.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/ffmpeg_help.py` & `videomass-5.0.1/videomass/vdms_dialogs/ffmpeg_help.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/filter_colorcorrection.py` & `videomass-5.0.1/videomass/vdms_dialogs/filter_colorcorrection.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/filter_crop.py` & `videomass-5.0.1/videomass/vdms_dialogs/filter_crop.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,83 +71,83 @@
         a parent and a current_bmp. First make sure you scale the
         image to fit on parent, e.g. a panel.
         """
         self.h = 0  # rectangle height
         self.w = 0  # rectangle width
         self.x = 0  # rectangle x axis
         self.y = 0  # rectangle y axis
-        self.horiz = 0
-        self.vert = 0
+        self.start_x = 0  # start x axis clicked
+        self.start_y = 0  # start y axis clicked
 
         wx.lib.statbmp.GenStaticBitmap.__init__(self, parent, -1,
                                                 bitmap, **kwargs)
         self.current_bmp = bitmap
 
         self.Bind(wx.EVT_PAINT, self.OnPaint)
         self.Bind(wx.EVT_MOTION, self.on_move)
         self.Bind(wx.EVT_LEFT_DOWN, self.on_leftdown)
         self.Bind(wx.EVT_LEFT_UP, self.on_leftup)
     # ------------------------------------------------------------------#
 
     def on_move(self, event):
         """
-        On mouse Dragging on area, only send
-        coordinates for rectangle drawing.
+        Dragging-mouse over the cropping area, it sends
+        the coordinates for drawing the rectangle.
         """
         self.SetCursor(wx.Cursor(wx.CURSOR_CROSS))
-        if event.Dragging():
+        if event.Dragging() and event.LeftIsDown():
             pos = event.GetPosition()
             x, y = pos[0], pos[1]
-            w, h = self.horiz - x, self.vert - y
+            w, h = self.start_x - x, self.start_y - y  # opposite to mouse dir.
             self.onRedraw(x, y, w, h)
     # ------------------------------------------------------------------#
 
     def on_leftdown(self, event):
         """
-        Event on clicking the left mouse button
-        (start position clicked)
+        Left-click event. On mouse click stores the initial
+        positions in pixels for the x/y axis points.
         """
         pos = event.GetPosition()
-        self.horiz = pos[0]
-        self.vert = pos[1]
-        x, y = pos[0], pos[1]
-        w = self.horiz - x
-        h = self.vert - y
-        self.onRedraw(x, y, w, h)
+        self.start_x = pos[0]
+        self.start_y = pos[1]
+        w, h = 0, 0
+        self.onRedraw(self.start_x, self.start_y, w, h)
     # ------------------------------------------------------------------#
 
     def on_leftup(self, event):
         """
         Event on releasing the left mouse button.
         Note: seeking x, y minimum values as dc x
         even to top left and y to bottom left.
         (end position click released)
         """
         self.SetCursor(wx.Cursor(wx.CURSOR_ARROW))
         pos = event.GetPosition()
-        x, y = min(self.horiz, pos[0]), min(self.vert, pos[1])
+        x, y = min(self.start_x, pos[0]), min(self.start_y, pos[1])
         w, h = abs(self.w), abs(self.h)
+        self.start_x, self.start_y = 0, 0
+        self.onRedraw(x, y, w, h)
         pub.sendMessage("TO_REAL_SCALE", msg=[x, y, w, h])
     # ------------------------------------------------------------------#
 
     def OnPaint(self, event=None):
         """
         When instantiating the Actor class, this event is
         executed last. This method is needed to set initial
         image on panel and/or to set crop area previously
         drawn on reopen this dialog.
         """
         dc = wx.PaintDC(self)  # draw window boundary
         dc.DrawBitmap(self.current_bmp, 0, 0, True)
         dc.SetPen(wx.Pen('red', 2, wx.PENSTYLE_SOLID))
         dc.SetBrush(wx.Brush('green', wx.BRUSHSTYLE_TRANSPARENT))
-        dc.DrawRectangle(round(self.x),
-                         round(self.y),
-                         round(self.w),
-                         round(self.h),
+        dc.DrawRectangle(round(self.x + 1),
+                         round(self.y + 1),
+                         round(self.w + 1),
+                         round(self.h + 1),
                          )
     # ------------------------------------------------------------------#
 
     def onRedraw(self, x, y, w, h):
         """
         Update Drawing: A transparent background rectangle in a
         bitmap object.
@@ -157,18 +157,18 @@
         """
         self.h, self.w, self.x, self.y = h, w, x, y
         dc = wx.ClientDC(self)
         dc.Clear()  # needed if image has trasparences
         dc.DrawBitmap(self.current_bmp, 0, 0, True)
         dc.SetPen(wx.Pen('red', 2, wx.PENSTYLE_SOLID))
         dc.SetBrush(wx.Brush('green', wx.BRUSHSTYLE_TRANSPARENT))
-        dc.DrawRectangle(round(self.x),
-                         round(self.y),
-                         round(self.w),
-                         round(self.h),
+        dc.DrawRectangle(round(self.x + 1),
+                         round(self.y + 1),
+                         round(self.w + 1),
+                         round(self.h + 1),
                          )
 
 
 class Crop(wx.Dialog):
     """
     A dialog tool to get video crop values based on FFmpeg syntax.
     See ``av_conversions.py`` -> ``on_Set_crop`` method for
@@ -205,18 +205,16 @@
         self.y_dc = 0
         self.x_dc = 0
         # current video size
         self.v_width = kwa['width']
         self.v_height = kwa['height']
         # resizing values preserving aspect ratio for monitor
         self.toscale = 220 if self.v_height >= self.v_width else 350
-        self.h_ratio = round((self.v_height
-                             / self.v_width) * self.toscale)  # height
-        self.w_ratio = round((self.v_width
-                             / self.v_height) * self.h_ratio)  # width
+        self.h_ratio = round((self.v_height / self.v_width) * self.toscale)
+        self.w_ratio = round((self.v_width / self.v_height) * self.h_ratio)
         self.filename = kwa['filename']  # selected filename on queued list
         name = os.path.splitext(os.path.basename(self.filename))[0]
         self.frame = os.path.join(f'{Crop.TMPSRC}', f'{name}.png')  # image
         self.fileclock = os.path.join(Crop.TMPROOT, f'{name}.clock')
         tcheck = clockset(kwa['duration'], self.fileclock)
         self.clock = tcheck['duration']
         self.mills = tcheck['millis']
```

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/filter_deinterlace.py` & `videomass-5.0.1/videomass/vdms_dialogs/filter_deinterlace.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/filter_denoisers.py` & `videomass-5.0.1/videomass/vdms_dialogs/filter_denoisers.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/filter_scale.py` & `videomass-5.0.1/videomass/vdms_dialogs/filter_scale.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/filter_stab.py` & `videomass-5.0.1/videomass/vdms_dialogs/filter_stab.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                                   )
         boxtime.Add(self.sld_time, 0, wx.CENTER, 0)
         self.lab_time = wx.StaticText(self, wx.ID_ANY, self.clock)
         boxtime.Add(self.lab_time, 0, wx.LEFT | wx.CENTER, 20)
         self.btn_snap = wx.Button(self, wx.ID_ANY, _("Preview"))
         self.btn_snap.Disable()
         boxtime.Add(self.btn_snap, 0, wx.LEFT | wx.CENTER, 20)
-        self.lab_dur = wx.StaticText(self, wx.ID_ANY, ("Duration seconds:"))
+        self.lab_dur = wx.StaticText(self, wx.ID_ANY, _("Duration seconds:"))
         boxtime.Add(self.lab_dur, 0, wx.LEFT | wx.CENTER, 20)
         self.spin_dur = wx.SpinCtrl(self, wx.ID_ANY, "5",
                                     min=3, max=15,
                                     style=wx.TE_PROCESS_ENTER
                                     | wx.SP_ARROW_KEYS,
                                     )
         boxtime.Add(self.spin_dur, 0, wx.LEFT | wx.CENTER, 2)
```

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/filter_transpose.py` & `videomass-5.0.1/videomass/vdms_dialogs/filter_transpose.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/mediainfo.py` & `videomass-5.0.1/videomass/vdms_dialogs/mediainfo.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/preferences.py` & `videomass-5.0.1/videomass/vdms_dialogs/preferences.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,16 +44,16 @@
                      ("error (Show all errors)"),
                      ("warning (Show all warnings and errors)"),
                      ("info (Show informative messages during processing)")
                      ]
     FFMPEG_LOGLEV = [("error (Show all errors)"),
                      ("warning (Show all warnings and errors)"),
                      ("info (Show informative messages during processing)"),
-                     ("verbose (Same as `info`, except more verbose.)"),
-                     ("debug (Show everything, including debugging info.)")
+                     ("verbose (Same as `info`, except more verbose)"),
+                     ("debug (Show everything, including debugging info)")
                      ]
     # -----------------------------------------------------------------
 
     def __init__(self, parent):
         """
         self.appdata: (dict) default settings already loaded.
         self.confmanager: instance to ConfigManager class
@@ -160,15 +160,14 @@
         sizeFFdirdest = wx.BoxSizer(wx.HORIZONTAL)
         sizerFiles.Add(sizeFFdirdest, 0, wx.EXPAND)
         self.txtctrl_FFpath = wx.TextCtrl(tabTwo, wx.ID_ANY, "",
                                           style=wx.TE_READONLY
                                           )
         sizeFFdirdest.Add(self.txtctrl_FFpath, 1, wx.ALL, 5)
         self.txtctrl_FFpath.AppendText(self.appdata['outputfile'])
-
         self.btn_fsave = wx.Button(tabTwo, wx.ID_ANY, "...", size=(35, -1))
         sizeFFdirdest.Add(self.btn_fsave, 0, wx.RIGHT | wx.ALIGN_CENTER, 5)
         sizerFiles.Add((0, 15))
         descr = _("Save each file in the same folder as input file")
         self.ckbx_dir = wx.CheckBox(tabTwo, wx.ID_ANY, (descr))
         sizerFiles.Add(self.ckbx_dir, 0, wx.ALL, 5)
         sizeSamedest = wx.BoxSizer(wx.HORIZONTAL)
@@ -279,17 +278,47 @@
         tabThree.SetSizer(sizerFFmpeg)
         notebook.AddPage(tabThree, _("FFmpeg"))
 
         # -----tab 4
         tabFour = wx.Panel(notebook, wx.ID_ANY)
         sizerytdlp = wx.BoxSizer(wx.VERTICAL)
         sizerytdlp.Add((0, 30))
-        msg = _("Download videos from YouTube.com and other video sites ")
+        msg = _('Download videos from YouTube.com and other video sites')
+        labytdlp = wx.StaticText(tabFour, wx.ID_ANY, msg)
+        sizerytdlp.Add(labytdlp, 0, wx.ALL | wx.EXPAND, 5)
+        msg = _("Enable/Disable yt-dlp")
         self.checkbox_ytdlp = wx.CheckBox(tabFour, wx.ID_ANY, (msg))
         sizerytdlp.Add(self.checkbox_ytdlp, 0, wx.ALL, 5)
+        sizerytdlp.Add((0, 15))
+        labdw = wx.StaticText(tabFour, wx.ID_ANY,
+                              _('External Downloader Preferences'))
+        sizerytdlp.Add(labdw, 0, wx.ALL | wx.EXPAND, 5)
+        msg = _("In addition to the default (native) one, yt-dlp currently\n"
+                "supports the following external downloaders:\n"
+                "aria2c, avconv, axel, curl, ffmpeg, httpie, wget.\n"
+                "Please note that if you enable an external downloader, you\n"
+                "will not be able to view the progress bar during download\n"
+                "operations.")
+        labdwmsg = wx.StaticText(tabFour, wx.ID_ANY, (msg))
+        sizerytdlp.Add(labdwmsg, 0, wx.ALL | wx.ALIGN_CENTER_HORIZONTAL, 5)
+        msg = _("External downloader executable path")
+        labextdw = wx.StaticText(tabFour, wx.ID_ANY, msg)
+        sizerytdlp.Add(labextdw, 0, wx.LEFT | wx.TOP | wx.BOTTOM, 5)
+        exedw = str(self.appdata["external_downloader"])
+        self.txtctrl_extdw = wx.TextCtrl(tabFour, wx.ID_ANY, exedw)
+        sizerytdlp.Add(self.txtctrl_extdw, 0, wx.EXPAND | wx.LEFT | wx.RIGHT
+                       | wx.BOTTOM, 5)
+        labextdwargs = wx.StaticText(tabFour, wx.ID_ANY,
+                                     _("External downloader arguments"))
+        sizerytdlp.Add(labextdwargs, 0, wx.LEFT | wx.TOP | wx.BOTTOM, 5)
+        val = self.appdata["external_downloader_args"]
+        args = " ".join(val) if isinstance(val, list) else 'None'
+        self.txtctrl_extdw_args = wx.TextCtrl(tabFour, wx.ID_ANY, args)
+        sizerytdlp.Add(self.txtctrl_extdw_args, 0, wx.EXPAND | wx.LEFT
+                       | wx.RIGHT | wx.BOTTOM, 5)
         # ----
         tabFour.SetSizer(sizerytdlp)
         notebook.AddPage(tabFour, "yt-dlp")
 
         # -----tab 5
         tabFive = wx.Panel(notebook, wx.ID_ANY)
         sizerAppearance = wx.BoxSizer(wx.VERTICAL)
@@ -342,15 +371,15 @@
                                           style=wx.CB_DROPDOWN | wx.CB_READONLY
                                           )
         gridTBsize.Add(self.cmbx_iconsSize, 0, wx.ALIGN_CENTER_VERTICAL, 0)
 
         if 'wx.svg' not in sys.modules:  # only in wx version 4.1 to up
             self.cmbx_iconsSize.Disable()
             lab1_appearance.Disable()
-        msg = _("Shows the text in the toolbar buttons")
+        msg = _("Shows text in the toolbar buttons")
         self.checkbox_tbtext = wx.CheckBox(tabFive, wx.ID_ANY, (msg))
         sizerAppearance.Add(self.checkbox_tbtext, 0, wx.ALL, 5)
 
         tabFive.SetSizer(sizerAppearance)  # aggiungo il sizer su tab 4
         notebook.AddPage(tabFive, _("Appearance"))
 
         # -----tab 6
@@ -406,27 +435,33 @@
             labconf.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             lablog.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labcache.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labfile.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labdown.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labFFexec.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labFFopt.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
+            labytdlp.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
+            labdw.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
+            labdwmsg.SetFont(wx.Font(11, wx.SWISS, wx.NORMAL, wx.NORMAL))
             labTheme.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labIcons.SetFont(wx.Font(11, wx.SWISS, wx.NORMAL, wx.NORMAL))
             labTB.SetFont(wx.Font(12, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labLog.SetFont(wx.Font(11, wx.SWISS, wx.NORMAL, wx.NORMAL))
         else:
             lablang.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labconf.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             lablog.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labcache.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labfile.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labdown.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labFFexec.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labFFopt.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
+            labytdlp.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
+            labdw.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
+            labdwmsg.SetFont(wx.Font(8, wx.SWISS, wx.NORMAL, wx.NORMAL))
             labTheme.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labIcons.SetFont(wx.Font(8, wx.SWISS, wx.NORMAL, wx.NORMAL))
             labTB.SetFont(wx.Font(9, wx.DEFAULT, wx.NORMAL, wx.BOLD))
             labLog.SetFont(wx.Font(8, wx.SWISS, wx.NORMAL, wx.NORMAL))
 
         #  tooltips
         tip = (_("By assigning an additional suffix you could avoid "
@@ -461,14 +496,16 @@
         self.Bind(wx.EVT_CHECKBOX, self.on_toolbarText, self.checkbox_tbtext)
         self.Bind(wx.EVT_CHECKBOX, self.exit_warn, self.checkbox_exit)
         self.Bind(wx.EVT_CHECKBOX, self.clear_Cache, self.checkbox_cacheclr)
         self.Bind(wx.EVT_CHECKBOX, self.clear_logs, self.checkbox_logclr)
         self.Bind(wx.EVT_BUTTON, self.on_help, btn_help)
         self.Bind(wx.EVT_BUTTON, self.on_cancel, btn_close)
         self.Bind(wx.EVT_BUTTON, self.on_ok, btn_ok)
+        self.Bind(wx.EVT_TEXT, self.on_ext_downl, self.txtctrl_extdw)
+        self.Bind(wx.EVT_TEXT, self.on_ext_downl_args, self.txtctrl_extdw_args)
         # --------------------------------------------#
         self.current_settings()  # call function for initialize setting layout
 
     def current_settings(self):
         """
         Setting enable/disable in according to the configuration file
         """
@@ -688,14 +725,32 @@
             self.txtctrl_YDLpath.Clear()
             getpath = self.appdata['getpath'](dlg.GetPath())
             self.txtctrl_YDLpath.AppendText(getpath)
             self.settings['dirdownload'] = getpath
             dlg.Destroy()
     # ---------------------------------------------------------------------#
 
+    def on_ext_downl(self, event):
+        """
+        Event on entering executable path of external downloader
+        """
+        val = str(self.txtctrl_extdw.GetValue()).strip()
+        downloader = None if val in ("", "None", "none") else val
+        self.settings["external_downloader"] = downloader
+    # -------------------------------------------------------------------#
+
+    def on_ext_downl_args(self, event):
+        """
+        Event on entering arguments for external downloader
+        """
+        val = str(self.txtctrl_extdw_args.GetValue()).strip()
+        args = None if val in ("", "None", "none") else val.split()
+        self.settings["external_downloader_args"] = args
+    # -------------------------------------------------------------------#
+
     def logging_ffplay(self, event):
         """specifies loglevel type for ffplay."""
         strn = self.rdbFFplay.GetStringSelection().split()[0]
         self.settings['ffplayloglev'] = f'-loglevel {strn}'
     # --------------------------------------------------------------------#
 
     def logging_ffmpeg(self, event):
@@ -925,12 +980,11 @@
         Close event
         """
         event.Skip()
     # --------------------------------------------------------------------#
 
     def on_ok(self, event):
         """
-        Applies all changes writing the new entries on
-        `settings.json` file aka file configuration.
+        Writes the new changes to configuration file aka `settings.json`
         """
         self.confmanager.write_options(**self.settings)
         event.Skip()
```

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/presets_addnew.py` & `videomass-5.0.1/videomass/vdms_dialogs/presets_addnew.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/renamer.py` & `videomass-5.0.1/videomass/vdms_dialogs/renamer.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/set_timestamp.py` & `videomass-5.0.1/videomass/vdms_dialogs/set_timestamp.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/showlogs.py` & `videomass-5.0.1/videomass/vdms_dialogs/showlogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,16 +149,16 @@
                           'Videomass', wx.ICON_INFORMATION)
             return
 
         index = self.log_select.GetFocusedItem()
         name = self.log_select.GetItemText(index, 0)
 
         if wx.MessageBox(_('Are you sure you want to clear the selected '
-                           'log file?'), "Videomass",
-                         wx.ICON_QUESTION | wx.YES_NO, self) == wx.NO:
+                           'log file?'), "Videomass", wx.ICON_QUESTION
+                         | wx.CANCEL | wx.YES_NO, self) != wx.YES:
             return
 
         with open(os.path.join(self.dirlog, name),
                   'w', encoding='utf8') as log:
             log.write('')
 
         self.on_update(self)
```

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/shownormlist.py` & `videomass-5.0.1/videomass/vdms_dialogs/shownormlist.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/videomass_check_version.py` & `videomass-5.0.1/videomass/vdms_dialogs/videomass_check_version.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/while_playing.py` & `videomass-5.0.1/videomass/vdms_dialogs/while_playing.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/widget_utils.py` & `videomass-5.0.1/videomass/vdms_dialogs/widget_utils.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_dialogs/wizard_dlg.py` & `videomass-5.0.1/videomass/vdms_dialogs/wizard_dlg.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,16 +230,16 @@
 
             elif not status[0]:
                 path.append(status[1])
 
         if exiting == 'provided':
             if wx.MessageBox(_("Videomass already seems to include "
                                "FFmpeg.\n\nDo you want to use that?"),
-                             _('Videomass: Please Confirm'),
-                             wx.ICON_QUESTION | wx.YES_NO, None) == wx.NO:
+                             _('Videomass: Please Confirm'), wx.ICON_QUESTION
+                             | wx.CANCEL | wx.YES_NO, self) != wx.YES:
                 return
 
         self.parent.ffmpeg = PageTwo.GETPATH(path[0])
         self.parent.ffprobe = PageTwo.GETPATH(path[1])
         self.parent.ffplay = PageTwo.GETPATH(path[2])
         self.parent.btnNext.Enable()
         self.detectBtn.Disable()
```

### Comparing `videomass-5.0.0/videomass/vdms_io/checkup.py` & `videomass-5.0.1/videomass/vdms_io/checkup.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 File Name: checkup.py
 Porpose: input/output file check
 Compatibility: Python3, wxPython Phoenix
 Author: Gianluca Pernigotto <jeanlucperni@gmail.com>
 Copyleft - 2023 Gianluca Pernigotto <jeanlucperni@gmail.com>
 license: GPL3
-Rev: Dec.02.2022
+Rev: April.17.2023
 Code checker: flake8, pylint
 
 This file is part of Videomass.
 
    Videomass is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
@@ -22,43 +22,56 @@
    GNU General Public License for more details.
 
    You should have received a copy of the GNU General Public License
    along with Videomass.  If not, see <http://www.gnu.org/licenses/>.
 """
 import os
 import wx
+from videomass.vdms_dialogs.list_warning import ListWarning
 
 
 def check_inout(file_sources, file_dest):
     """
     check for overwriting and file/dir existence.
     return tuple([file_sources], [file_dest]).
     return None otherwise.
 
     """
     # --------------- CHECK FOR OVERWRITING:
-    files_exist = []  # already exist file LIST
+    files_ow = []  # already exist file LIST
+    files_exist = []
     for files in file_dest:
         if os.path.exists(files):
-            files_exist.append(files)
+            files_ow.append(f'"{files}"')
 
-    if files_exist:
-        if wx.MessageBox(_('Already exist: \n\n{}\n\n'
-                           'Do you want to overwrite? ').format(
-                         '\n'.join(files_exist)),
-                         _('Please Confirm'),
-                         wx.ICON_QUESTION | wx.YES_NO, None) == wx.NO:
-            return None
-    # --------------- CHECK FOR EXISTING FILES:
+    if files_ow:
+        msg = _('Files already exist, do you want to overwrite them?')
+        with ListWarning(None,
+                         dict.fromkeys(files_ow, _('Already exist')),
+                         caption=_('Please Confirm'),
+                         header=msg,
+                         buttons='CONFIRM',
+                         ) as log:
+            if log.ShowModal() != wx.ID_YES:
+                return None
+
+    # --------------- CHECK FOR MSSING FILES:
     for fln in file_sources:
         if not os.path.isfile(os.path.abspath(fln)):
-            wx.MessageBox(_('File does not exist:\n\n"{}"\n').format(fln),
-                          "Videomass", wx.ICON_ERROR
-                          )
-            return None
+            files_exist.append(f'"{fln}"')
+    if files_exist:
+        msg = _('No source files found in the specified path')
+        with ListWarning(None,
+                         dict.fromkeys(files_exist, _('Not found')),
+                         caption=_('Non-existent source files'),
+                         header=msg,
+                         buttons='OK',
+                         ) as log:
+            log.ShowModal()
+        return None
     # --------------- CHECK FOR EXISTING DIRECTORIES:
     for drn in file_dest:
         drn = os.path.abspath(os.path.dirname(drn))
         if not os.path.isdir(drn):
             wx.MessageBox(_('Output folder does not exist:\n\n"{}"\n').format(
                           drn), 'Videomass', wx.ICON_ERROR
                           )
```

### Comparing `videomass-5.0.0/videomass/vdms_io/io_tools.py` & `videomass-5.0.1/videomass/vdms_io/io_tools.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_io/make_filelog.py` & `videomass-5.0.1/videomass/vdms_io/make_filelog.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_io/presets_manager_prop.py` & `videomass-5.0.1/videomass/vdms_io/presets_manager_prop.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_main/main_frame.py` & `videomass-5.0.1/videomass/vdms_main/main_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,16 +345,16 @@
                                 'want to stop them, use the "Abort" button.'),
                               _('Videomass'), wx.ICON_WARNING, self)
                 return
 
         if self.appdata['warnexiting']:
             if wx.MessageBox(_('Are you sure you want to exit '
                                'the application?'),
-                             _('Exit'), wx.ICON_QUESTION | wx.YES_NO,
-                             self) == wx.NO:
+                             _('Exit'), wx.ICON_QUESTION | wx.CANCEL
+                             | wx.YES_NO, self) != wx.YES:
                 return
 
         if self.ytdlframe:
             if self.ytdlframe.ProcessPanel.thread_type:
                 wx.MessageBox(_("There are still active windows with running "
                                 "processes, make sure you finish your work "
                                 "before closing them."),
@@ -684,14 +684,15 @@
             if filedlg.ShowModal() == wx.ID_CANCEL:
                 return
 
             self.switch_file_import(self)
             paths = filedlg.GetPaths()
             for path in paths:
                 self.fileDnDTarget.flCtrl.dropUpdate(path)
+            self.fileDnDTarget.flCtrl.rejected_files()
     # -------------------------------------------------------------------#
 
     def openMyconversions(self, event):
         """
         Open the conversions folder with file manager
         """
         io_tools.openpath(self.appdata['outputfile'])
@@ -735,16 +736,16 @@
         Delete permanently all files inside trash folder
         """
         path = self.appdata['user_trashdir']
         if os.path.exists(path):
             files = os.listdir(path)
             if len(files) > 0:
                 if wx.MessageBox(_("Are you sure to empty trash folder?"),
-                                 "Videomass", wx.ICON_QUESTION
-                                 | wx.YES_NO, self) == wx.NO:
+                                 "Videomass", wx.ICON_QUESTION | wx.CANCEL
+                                 | wx.YES_NO, self) != wx.YES:
                     return
 
                 for fname in files:
                     os.remove(os.path.join(path, fname))
             else:
                 wx.MessageBox(_("No files to delete"),
                               "Videomass", wx.ICON_INFORMATION, self)
@@ -1073,15 +1074,15 @@
                         wx.MessageBox(_("Changes will take effect once the "
                                         "program has been restarted."),
                                       _('Videomass'), wx.ICON_WARNING, self)
                         return
                 if wx.MessageBox(_("Changes will take effect once the program "
                                    "has been restarted.\n\n"
                                    "Do you want to exit the application now?"),
-                                 _('Exit'), wx.ICON_QUESTION
+                                 _('Exit'), wx.ICON_QUESTION | wx.CANCEL
                                  | wx.YES_NO, self) == wx.YES:
                     self.on_Kill()
     # ------------------------------------------------------------------#
     # --------- Menu Help  ###
 
     def Helpme(self, event):
         """
```

### Comparing `videomass-5.0.0/videomass/vdms_miniframes/timeline.py` & `videomass-5.0.1/videomass/vdms_miniframes/timeline.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_panels/av_conversions.py` & `videomass-5.0.1/videomass/vdms_panels/av_conversions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2333,16 +2333,16 @@
         Save current setting as profile for the Presets
         Manager panel
         """
         if self.rdbx_normalize.GetSelection() in (1, 2, 3):  # EBU
             if wx.MessageBox(_('Audio normalization data cannot be saved '
                                'on the Presets Manager.\n\n'
                                'Do you want to continue?'),
-                             'Videomass',
-                             wx.ICON_QUESTION | wx.YES_NO, self) == wx.NO:
+                             'Videomass', wx.ICON_QUESTION
+                             | wx.CANCEL | wx.YES_NO, self) != wx.YES:
                 return
 
         self.update_options()
         if self.cmb_Media.GetValue() == 'Video':
             if self.opt["Vidstabdetect"]:
                 parameters = self.video_stabilizer([], [], 'save as profile')
             else:
```

### Comparing `videomass-5.0.0/videomass/vdms_panels/choose_topic.py` & `videomass-5.0.1/videomass/vdms_panels/choose_topic.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,14 +216,14 @@
     # ------------------------------------------------------------------#
 
     def on_youtube_dl(self, event):
         """
         Open a separated downloader frame for yt-dlp.
         """
         if not self.appdata['use-downloader']:
-            wx.MessageBox(_("The downloader is disabled. "
+            wx.MessageBox(_("yt-dlp is disabled. "
                             "Check your preferences."),
                           "Videomass", wx.ICON_INFORMATION, self)
             return True
 
         self.parent.youtubedl(self)
         return None
```

### Comparing `videomass-5.0.0/videomass/vdms_panels/concatenate.py` & `videomass-5.0.1/videomass/vdms_panels/concatenate.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_panels/filedrop.py` & `videomass-5.0.1/videomass/vdms_panels/filedrop.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 Name: filedrop.py
 Porpose: files drag n drop interface
 Compatibility: Python3, wxPython Phoenix
 Author: Gianluca Pernigotto <jeanlucperni@gmail.com>
 Copyleft - 2023 Gianluca Pernigotto <jeanlucperni@gmail.com>
 license: GPL3
-Rev: Feb.16.2023
+Rev: April.17.2023
 Code checker: flake8, pylint
 
 This file is part of Videomass.
 
    Videomass is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
@@ -29,14 +29,15 @@
 import wx
 from pubsub import pub
 from videomass.vdms_io.io_tools import stream_play
 from videomass.vdms_threads.ffprobe import ffprobe
 from videomass.vdms_utils.utils import get_milliseconds
 from videomass.vdms_utils.utils import to_bytes
 from videomass.vdms_dialogs.renamer import Renamer
+from videomass.vdms_dialogs.list_warning import ListWarning
 
 
 def fullpathname_sanitize(fullpathfilename):
     """
     Check for 'full path file name' sanitize.
     return message `string` if warning, `None` otherwise
     """
@@ -96,37 +97,29 @@
 
 
 class MyListCtrl(wx.ListCtrl):
     """
     This is the listControl widget.
     Note that this wideget has DnDPanel parented.
     """
-    AZURE = '#d9ffff'  # rgb form (wx.Colour(217,255,255))
-    RED = '#ea312d'
-    YELLOW = '#bd9f00'
-    GREENOLIVE = '#6aaf23'
-    ORANGE = '#f28924'
-    WHITE = '#fbf4f4'  # white for background status bar
-    BLACK = '#060505'  # black for background status bar
-    # ----------------------------------------------------------------------
-
     def __init__(self, parent):
         """
         Constructor.
         WARNING to avoid segmentation error on removing items by
         listctrl, style must be wx.LC_SINGLE_SEL .
         """
         get = wx.GetApp()
         self.ffprobe_cmd = get.appset['ffprobe_cmd']
         self.index = None
         self.parent = parent  # parent is DnDPanel class
         self.data = self.parent.data
         self.file_src = self.parent.file_src
         self.duration = self.parent.duration
         self.outputnames = self.parent.outputnames
+        self.errors = {}
         wx.ListCtrl.__init__(self,
                              parent,
                              style=wx.LC_REPORT
                              | wx.LC_SINGLE_SEL,
                              )
         self.populate()
     # ----------------------------------------------------------------------#
@@ -137,38 +130,35 @@
         """
         self.InsertColumn(0, '#', width=30)
         self.InsertColumn(1, _('File Name'), width=200)
         self.InsertColumn(2, _('Duration'), width=200)
         self.InsertColumn(3, _('Media type'), width=200)
         self.InsertColumn(4, _('Size'), width=150)
         self.InsertColumn(5, _('Output file name'), width=200)
+    # ----------------------------------------------------------------------#
 
     def dropUpdate(self, path, newname=None):
         """
         Update list-control during drag and drop.
         Note that the optional 'newname' argument is given by
         the 'on_col_click' method in the 'FileDnD' class to preserve
         the related renames in column 5 of wx.ListCtrl.
 
         """
         self.index = self.GetItemCount()
         warn = fullpathname_sanitize(path)  # check for fullname sanitize
         if warn:
-            self.parent.statusbar_msg(warn,
-                                      MyListCtrl.ORANGE,
-                                      MyListCtrl.WHITE
-                                      )
+            self.errors[f'"{path}"'] = warn
             return
 
         if not [x for x in self.data if x['format']['filename'] == path]:
             probe = ffprobe(path, self.ffprobe_cmd,
                             hide_banner=None, pretty=None)
             if probe[1]:
-                self.parent.statusbar_msg(probe[1], MyListCtrl.RED,
-                                          MyListCtrl.WHITE)
+                self.errors[f'"{path}"'] = probe[1]
                 return
 
             probe = probe[0]
             self.InsertItem(self.index, str(self.index + 1))
             self.SetItem(self.index, 1, path)
 
             if 'duration' not in probe['format'].keys():
@@ -197,22 +187,36 @@
                 fname = os.path.splitext(os.path.basename(path))[0]
                 self.SetItem(self.index, 5, fname)
                 self.outputnames.append(fname)
             self.index += 1
             self.data.append(probe)
             self.file_src.append(path)
             self.duration.append(probe['format']['duration'])
-            self.parent.statusbar_msg('', None)
+            # self.parent.statusbar_msg('', None)
             self.parent.changes_in_progress()
         else:
-            mess = _("Duplicate files are rejected: > {}").format(path)
-            self.parent.statusbar_msg(mess, MyListCtrl.YELLOW,
-                                      MyListCtrl.BLACK)
+            mess = _("Duplicate file, it has already been added to the list.")
+            self.errors[f'"{path}"'] = mess
     # ----------------------------------------------------------------------#
 
+    def rejected_files(self):
+        """
+        Handles all rejected files if any
+        """
+        if self.errors:
+            msg = _('See the error message next to each path name')
+            with ListWarning(self,
+                             self.errors,
+                             caption=_('Rejected Files'),
+                             header=msg,
+                             buttons='OK',
+                             ) as log:
+                log.ShowModal()
+            self.errors.clear()  # clear values here
+
 
 class FileDrop(wx.FileDropTarget):
     """
     This is the file drop target class
     """
     # ----------------------------------------------------------------------#
 
@@ -227,14 +231,15 @@
     def OnDropFiles(self, x, y, filenames):
         """
         When files are dropped, write where they were dropped and then
         the file paths themselves
         """
         for filepath in filenames:
             self.window.dropUpdate(filepath)  # update list control
+        self.window.rejected_files()  # call parent.rejected_files at end
 
         return True
     # ----------------------------------------------------------------------#
 
 
 class FileDnD(wx.Panel):
     """
@@ -506,22 +511,14 @@
         """
         Set a specific directory for files saving
         """
         self.text_path_save.SetValue("")
         self.text_path_save.AppendText(path)
     # -----------------------------------------------------------------------
 
-    def statusbar_msg(self, mess, bcolor, fcolor=None):
-        """
-        Set a status bar message of the parent method.
-        bcolor: background, fcolor: foreground
-        """
-        self.parent.statusbar_msg(f'{mess}', bcolor, fcolor)
-    # -----------------------------------------------------------------------
-
     def renaming_file(self):
         """
         This method is responsible for renaming the selected
         output file.
         Names consisting of only whitespaces or tabs or matching
         same name as outputnames are rejected silently.
         """
```

### Comparing `videomass-5.0.0/videomass/vdms_panels/hevc_avc.py` & `videomass-5.0.1/videomass/vdms_panels/hevc_avc.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_panels/libaom.py` & `videomass-5.0.1/videomass/vdms_panels/libaom.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_panels/long_processing_task.py` & `videomass-5.0.1/videomass/vdms_panels/long_processing_task.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_panels/presets_manager.py` & `videomass-5.0.1/videomass/vdms_panels/presets_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,16 +342,16 @@
                     'It seems that the local preset database in your '
                     'configuration folder is outdated. If you choose to '
                     'update the preset database, the outdated version '
                     'will be backed up in the same folder as the new '
                     'incoming presets:\n"{2}"\n\n'
                     'Do you want to update the preset '
                     'database now?').format(srcversion, confversion, dest)
-            if wx.MessageBox(msg, _('Please confirm'),
-                             wx.ICON_QUESTION | wx.YES_NO, self) == wx.NO:
+            if wx.MessageBox(msg, _('Please confirm'), wx.ICON_QUESTION
+                             | wx.CANCEL | wx.YES_NO, self) != wx.YES:
                 return
 
             backup = copydir_recursively(dest, dest,
                                          f'Version-{confversion}-BACKUP')
             if backup:
                 wx.MessageBox(f'{backup}', "Videomass", wx.ICON_ERROR, self)
 
@@ -520,16 +520,16 @@
         Remove or delete a preset '*.prst' on /presets path name
         and move on Removals folder
         """
         filename = self.cmbx_prst.GetValue()
         if wx.MessageBox(_('Are you sure you want to remove "{}" preset?\n\n '
                            'It will be moved to the "Removals" subfolder '
                            'of the presets folder.').format(filename),
-                         _('Please confirm'),
-                         wx.ICON_QUESTION | wx.YES_NO, self) == wx.NO:
+                         _('Please confirm'), wx.ICON_QUESTION
+                         | wx.CANCEL | wx.YES_NO, self) != wx.YES:
             return
 
         try:
             if not os.path.exists(os.path.join(self.user_prst, 'Removals')):
                 os.mkdir(os.path.join(self.user_prst, 'Removals'))
         except OSError as err:
             wx.MessageBox(_("{}\n\nSorry, removal failed, cannot "
@@ -560,16 +560,16 @@
         dlg = wx.DirDialog(self, _("Choose a folder to save the selected "
                                    "preset"), "", style=wx.DD_DEFAULT_STYLE)
         if dlg.ShowModal() == wx.ID_OK:
             path = dlg.GetPath()
             if os.path.exists(os.path.join(path, f'{combvalue}.prst')):
                 if wx.MessageBox(_('A file with this name already exists, '
                                    'do you want to overwrite it?'),
-                                 _('Please confirm'),
-                                 wx.ICON_QUESTION | wx.YES_NO, self) == wx.NO:
+                                 _('Please confirm'), wx.ICON_QUESTION
+                                 | wx.CANCEL | wx.YES_NO, self) != wx.YES:
                     return
 
             status = copy_restore(filedir,
                                   os.path.join(path, f'{combvalue}.prst'))
             dlg.Destroy()
 
             if status:
@@ -624,16 +624,16 @@
 
         if os.path.exists(os.path.join(self.user_prst, new)):
 
             if wx.MessageBox(_("This preset already exists and is about to be "
                                "updated. Don't worry, it will keep all your "
                                "saved profiles.\n\n"
                                "Do you want to continue?"),
-                             _('Please confirm'),
-                             wx.ICON_QUESTION | wx.YES_NO, self) == wx.NO:
+                             _('Please confirm'), wx.ICON_QUESTION
+                             | wx.CANCEL | wx.YES_NO, self) != wx.YES:
                 return
 
             update_oudated_profiles(newincoming,
                                     os.path.join(self.user_prst, new))
         status = copy_restore(newincoming, os.path.join(self.user_prst, new))
         if status:
             wx.MessageBox(f'{status}', "Videomass", wx.ICON_ERROR, self)
@@ -650,16 +650,16 @@
         Import all presets previously saved in a folder and replaces
         the existing ones
         """
         if not source:
             if wx.MessageBox(_("This will update the presets database. "
                                "Don't worry, it will keep all your saved "
                                "profiles.\n\nDo you want to continue?"),
-                             _("Please confirm"),
-                             wx.ICON_QUESTION | wx.YES_NO, self) == wx.NO:
+                             _("Please confirm"), wx.ICON_QUESTION
+                             | wx.CANCEL | wx.YES_NO, self) != wx.YES:
                 return
 
             dialsave = wx.DirDialog(self, _("Import a new presets folder"),
                                     "", style=wx.DD_DEFAULT_STYLE)
             if dialsave.ShowModal() == wx.ID_CANCEL:
                 return
             source = dialsave.GetPath()
@@ -833,19 +833,20 @@
                 msg = _("The selected profile command has been "
                         "changed manually.\n"
                         "Do you want to apply it "
                         "during the conversion process?")
                 dlg = wx.RichMessageDialog(self, msg,
                                            _("Please confirm"),
                                            wx.ICON_QUESTION
+                                           | wx.CANCEL
                                            | wx.YES_NO,
                                            )
                 dlg.ShowCheckBox(_("Don't show this dialog again"))
 
-                if dlg.ShowModal() == wx.ID_NO:
+                if dlg.ShowModal() != wx.ID_YES:
                     if dlg.IsCheckBoxChecked():
                         # make sure we won't show it again the next time
                         self.txtcmdedited = False
                     return
                 if dlg.IsCheckBoxChecked():
                     # make sure we won't show it again the next time
                     self.txtcmdedited = False
```

### Comparing `videomass-5.0.0/videomass/vdms_panels/sequence_to_video.py` & `videomass-5.0.1/videomass/vdms_panels/sequence_to_video.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,23 +70,23 @@
     """
     VIOLET = '#D64E93'
     LGREEN = '#52ee7d'
     BLACK = '#1f1f1f'
     MSG_1 = _("\n1. Import one or more image files such as JPG, PNG and BMP "
               "formats, then select one."
               "\n\n2. Use the Resizing function to resize images which "
-              "have different sizes such as width and height. "
+              "have different sizes such as width and\nheight. "
               "It is optional in other cases."
               "\n\n3. Use the Timeline editor (CTRL+T) to set the time "
-              "interval between images by adjusting the \"End\" duration "
-              "value and\nleaving the \"Start\" value at 00:00:00.000."
+              "interval between images by adjusting\nthe \"End\" duration "
+              "value and leaving the \"Start\" value at 00:00:00.000."
               "\n\n4. Run the conversion."
               "\n\n\nThe produced video will have the name of the selected "
-              "file in the 'Queued File' list, which will be saved in a "
-              "folder named 'Still_Images'\nwith a progressive digit, "
+              "file in the 'Queued File' list, which\nwill be saved in a "
+              "folder named 'Still_Images' with a progressive digit, "
               "in the path you specify.")
     # ---------------------------------------------------------------------
 
     def __init__(self, parent, icons):
         """
         Simple GUI panel with few controls to create slideshows
         based on ffmpeg syntax.
```

### Comparing `videomass-5.0.0/videomass/vdms_panels/video_to_sequence.py` & `videomass-5.0.1/videomass/vdms_panels/video_to_sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,21 +44,21 @@
     abilities of customization.
     """
     VIOLET = '#D64E93'
     LGREEN = '#52ee7d'
     BLACK = '#1f1f1f'
     MSG_1 = _("\n1. Import one or more video files, then select one."
               "\n\n2. To select a slice of time use the Timeline editor "
-              "(CTRL+T) by adjusting the \"End\" and the \"Start\" duration "
+              "(CTRL+T) by adjusting the\n\"End\" and the \"Start\" duration "
               "values."
               "\n\n3. Select an output format (jpg, png, bmp)."
               "\n\n4. Start the conversion."
               "\n\n\nThe images produced will be saved in a folder "
-              "named 'Movie_to_Pictures' with a progressive digit, "
-              "\nin the path you specify.")
+              "named 'Movie_to_Pictures'\nwith a progressive digit, "
+              "in the path you specify.")
     # ----------------------------------------------------------------#
 
     def __init__(self, parent, icons):
         """
         This is a panel impemented on MainFrame
         """
         get = wx.GetApp()
```

### Comparing `videomass-5.0.0/videomass/vdms_panels/webm.py` & `videomass-5.0.1/videomass/vdms_panels/webm.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_sys/app_const.py` & `videomass-5.0.1/videomass/vdms_sys/app_const.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_sys/argparser.py` & `videomass-5.0.1/videomass/vdms_sys/argparser.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_sys/configurator.py` & `videomass-5.0.1/videomass/vdms_sys/configurator.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_sys/msg_info.py` & `videomass-5.0.1/videomass/vdms_sys/msg_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     NOTE: number version > major number.minor number.micro
     number(patch number) the sub release a=alpha release, b=beta
     release, c= candidate release
     Example 19.1.1c1
     """
     release_name = 'Videomass'
     program_name = 'videomass'
-    version = '5.0.0'
+    version = '5.0.1'
     release = 'released'
     copyr = '2013-2023'
     website = 'http://jeanslack.github.io/Videomass/'
     author = ('Gianluca Pernigotto', '(aka jeanslack)')
     mail = 'jeanlucperni@gmail.com'
     comment = ("\nThanks to:\n"
                "- Python <https://www.python.org/>, programming language\n"
```

### Comparing `videomass-5.0.0/videomass/vdms_sys/settings_manager.py` & `videomass-5.0.1/videomass/vdms_sys/settings_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,17 +142,23 @@
         default value is True.
 
     ("ssl_certificate", "add_metadata", "embed_thumbnails",
     "overwr_dl_files", "include_ID_name", "restrict_fname"
     "write_subtitle") (bool)
         Checkboxes option (see YouTube Downloader)
 
+    external_downloader (str):
+        external downloader used by yt-dlp. Default is None
+
+    external_downloader_args (list):
+        args used by external downloader in yt-dlp. Default is None
+        List should be passed using aria2c ["-j", "1", "-x", "1", "-s", "1"]
 
     """
-    VERSION = 5.9
+    VERSION = 6.0
     DEFAULT_OPTIONS = {"confversion": VERSION,
                        "outputfile": f"{os.path.expanduser('~')}",
                        "outputfile_samedir": False,
                        "filesuffix": "",
                        "ffmpeg_cmd": "",
                        "ffmpeg_islocal": False,
                        "ffmpegloglev": "-loglevel warning",
@@ -182,14 +188,16 @@
                        "ssl_certificate": False,
                        "add_metadata": True,
                        "embed_thumbnails": False,
                        "overwr_dl_files": False,
                        "include_ID_name": False,
                        "restrict_fname": True,
                        "write_subtitle": False,
+                       "external_downloader": None,
+                       "external_downloader_args": None,
                        }
 
     def __init__(self, filename, makeportable=None):
         """
         Expects an existing `filename` on the file system paths
         suffixed by `.json`. If `makeportable` is `True`, some
         paths on the `DEFAULT_OPTIONS` class attribute will be
```

### Comparing `videomass-5.0.0/videomass/vdms_threads/check_bin.py` & `videomass-5.0.1/videomass/vdms_threads/check_bin.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/concat_demuxer.py` & `videomass-5.0.1/videomass/vdms_threads/concat_demuxer.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/ffplay_file.py` & `videomass-5.0.1/videomass/vdms_threads/ffplay_file.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/ffprobe.py` & `videomass-5.0.1/videomass/vdms_threads/ffprobe.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/generic_downloads.py` & `videomass-5.0.1/videomass/vdms_threads/generic_downloads.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/generic_task.py` & `videomass-5.0.1/videomass/vdms_threads/generic_task.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/one_pass.py` & `videomass-5.0.1/videomass/vdms_threads/one_pass.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/picture_exporting.py` & `videomass-5.0.1/videomass/vdms_threads/picture_exporting.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/slideshow.py` & `videomass-5.0.1/videomass/vdms_threads/slideshow.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/two_pass.py` & `videomass-5.0.1/videomass/vdms_threads/two_pass.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/two_pass_ebu.py` & `videomass-5.0.1/videomass/vdms_threads/two_pass_ebu.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/video_stabilization.py` & `videomass-5.0.1/videomass/vdms_threads/video_stabilization.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_threads/volumedetect.py` & `videomass-5.0.1/videomass/vdms_threads/volumedetect.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_utils/get_bmpfromsvg.py` & `videomass-5.0.1/videomass/vdms_utils/get_bmpfromsvg.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_utils/utils.py` & `videomass-5.0.1/videomass/vdms_utils/utils.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_ytdlp/formatcode.py` & `videomass-5.0.1/videomass/vdms_ytdlp/formatcode.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_ytdlp/long_task_ytdlp.py` & `videomass-5.0.1/videomass/vdms_ytdlp/long_task_ytdlp.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_ytdlp/main_ytdlp.py` & `videomass-5.0.1/videomass/vdms_ytdlp/main_ytdlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,16 +205,16 @@
                                 'want to stop them, use the "Abort" button.'),
                               _('Videomass'), wx.ICON_WARNING, self)
                 return
 
         if self.appdata['warnexiting'] and warn:
             if wx.MessageBox(_('Are you sure you want to exit this window?\n'
                                'All data will be lost'),
-                             _('Exit'), wx.ICON_QUESTION | wx.YES_NO,
-                             self) == wx.NO:
+                             _('Exit'), wx.ICON_QUESTION | wx.CANCEL
+                             | wx.YES_NO, self) != wx.YES:
                 return
 
         confmanager = ConfigManager(self.appdata['fileconfpath'])
         sett = confmanager.read_options()
         sett['main_ytdl_size'] = list(self.GetSize())
         sett['main_ytdl_pos'] = list(self.GetPosition())
         sett['ssl_certificate'] = self.ytDownloader.ckbx_ssl.GetValue()
```

### Comparing `videomass-5.0.0/videomass/vdms_ytdlp/playlist_indexing.py` & `videomass-5.0.1/videomass/vdms_ytdlp/playlist_indexing.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_ytdlp/textdrop.py` & `videomass-5.0.1/videomass/vdms_ytdlp/textdrop.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,35 +22,31 @@
    GNU General Public License for more details.
 
    You should have received a copy of the GNU General Public License
    along with Videomass.  If not, see <http://www.gnu.org/licenses/>.
 """
 from urllib.parse import urlparse
 import wx
+from videomass.vdms_dialogs.list_warning import ListWarning
 
 
 class MyListCtrl(wx.ListCtrl):
     """
     This is the listControl widget.
     Note that this wideget has DnDPanel parented.
     """
-    RED = '#ea312d'
-    YELLOW = '#bd9f00'
-    WHITE = '#fbf4f4'  # white for background status bar
-    BLACK = '#060505'
-    # ----------------------------------------------------------------------
-
     def __init__(self, parent):
         """
         Constructor.
         WARNING to avoid segmentation error on removing items by
         listctrl, style must be wx.LC_SINGLE_SEL .
         """
         self.index = None
         self.parent = parent  # parent is DnDPanel class
+        self.errors = {}
         wx.ListCtrl.__init__(self,
                              parent,
                              style=wx.LC_REPORT
                              | wx.LC_SINGLE_SEL,
                              )
         self.populate()
     # ----------------------------------------------------------------------#
@@ -58,67 +54,76 @@
     def populate(self):
         """
         make default colums
         """
         self.InsertColumn(0, ('#'), width=30)
         self.InsertColumn(1, (_('Url')), width=600)
 
-    def dropUpdate(self, data):
+    def dropUpdate(self, url):
         """
         Update list-control during drag and drop.
         """
         self.index = self.GetItemCount()
-        listurl = data.split()
-        for url in listurl:
-            res = urlparse(url)
-            if not res[1]:  # if empty netloc given from ParseResult
-                msg = _('Invalid URL:')
-                self.parent.statusbar_msg(f'{msg} "{url}"',
-                                          MyListCtrl.RED,
-                                          MyListCtrl.WHITE
-                                          )
-                return False
-
-            self.InsertItem(self.index, str(self.index + 1))
-            self.SetItem(self.index, 1, url)
-            self.index += 1
+        res = urlparse(url)
+        if not res[1]:  # if empty netloc given from ParseResult
+            self.errors[f'{url}'] = _('Invalid URL')
+            return False
+
+        self.InsertItem(self.index, str(self.index + 1))
+        self.SetItem(self.index, 1, url)
+        self.index += 1
 
         self.parent.changes_in_progress()
         return True
     # ----------------------------------------------------------------------#
 
+    def rejected_urls(self):
+        """
+        Handles all rejected URLs if any
+        """
+        if self.errors:
+            msg = _('List of rejected URLs')
+            with ListWarning(self,
+                             self.errors,
+                             caption=_('Rejected URLs'),
+                             header=msg,
+                             buttons='OK',
+                             ) as log:
+                log.ShowModal()
+            self.errors.clear()  # clear values here
+
 
 class UrlDropTarget(wx.TextDropTarget):
     """
-    This is a Drop target object for handle dragging text URL data
-    on a ListCtrl object.
+    This is a Drop target object for handle dragging
+    text URL data on a ListCtrl object.
     """
     def __init__(self, parent, listctrl):
         """
         Defining the ListCtrl object attribute
         """
         wx.TextDropTarget.__init__(self)
         self.parent = parent
         self.listctrl = listctrl
 
     def OnDropText(self, x, y, data):
         """
         Update ListCtrl object by dragging text inside it.
         """
-        self.listctrl.dropUpdate(data)
+        for url in data.split():
+            self.listctrl.dropUpdate(url)
+        self.listctrl.rejected_urls()
+
         return True
 
 
 class Url_DnD_Panel(wx.Panel):
     """
     Panel responsible to embed URLs controls
     """
-    ORANGE = '#f28924'
-    WHITE = '#fbf4f4'
-
     def __init__(self, parent):
         """
         parent is the MainFrame
         """
         self.parent = parent
         get = wx.GetApp()
         # colors = get.appset['icontheme'][1]
@@ -212,39 +217,34 @@
         data = []
         for x in range(self.urlctrl.GetItemCount()):
             data.append(self.urlctrl.GetItemText(x, 1))
 
         if not data == self.parent.data_url:
             self.parent.changed = True
 
-        self.statusbar_msg(_('Ready'), None)
+        self.parent.statusbar_msg(_('Ready'), None)
         self.parent.data_url = data.copy()
         self.parent.destroy_orphaned_window()
         self.parent.toolbar.EnableTool(25, True)
     # -----------------------------------------------------------------------
 
-    def statusbar_msg(self, mess, bcolor, fcolor=None):
-        """
-        Set a status bar message of the parent method.
-        bcolor: background, fcolor: foreground
-        """
-        self.parent.statusbar_msg(f'{mess}', bcolor, fcolor)
-    # -----------------------------------------------------------------------
-
     def on_paste(self, event):
         """
         Event on clicking paste button to paste
         text data on the ListCtrl
         """
         text_data = wx.TextDataObject()
         if wx.TheClipboard.Open():
             success = wx.TheClipboard.GetData(text_data)
             wx.TheClipboard.Close()
         if success:
-            self.urlctrl.dropUpdate(text_data.GetText())
+            data = text_data.GetText().split()
+            for url in data:
+                self.urlctrl.dropUpdate(url)
+            self.urlctrl.rejected_urls()
     # ----------------------------------------------------------------------
 
     def delete_all(self, event):
         """
         clear all text lines of the TxtCtrl
         """
         self.urlctrl.DeleteAllItems()
```

### Comparing `videomass-5.0.0/videomass/vdms_ytdlp/ydl_downloader.py` & `videomass-5.0.1/videomass/vdms_ytdlp/ydl_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,22 +156,21 @@
         self.count = 0
         self.args = {'urls': varargs[1],
                      'code': varargs[6],
                      'outdir': varargs[3],
                      'logname': logname,
                      'countmax': len(varargs[1]),
                      }
-
         Thread.__init__(self)
         self.start()  # run()
 
     def run(self):
         """
         Apply the options passed by the user for the
-        download process with youtube_dl
+        download process with yt_dlp
 
         """
         for url, code in itertools.zip_longest(self.args['urls'],
                                                self.args['code'],
                                                fillvalue='',
                                                ):
             if '/playlist' in url or not self.opt['noplaylist']:
@@ -193,14 +192,17 @@
                          )
 
             if self.stop_work_thread:
                 break
 
             ydl_opts = {
                 'compat_opts': 'youtube-dl',
+                'external_downloader': self.appdata["external_downloader"],
+                'external_downloader_args':
+                    self.appdata["external_downloader_args"],
                 'format': format_code,
                 'extractaudio': self.opt['format'],
                 'outtmpl': f"{self.args['outdir']}/{outtmpl}",
                 'writesubtitles': self.opt['writesubtitles'],
                 'subtitleslangs': self.opt['subtitleslangs'],
                 'skip_download': self.opt['skip_download'],
                 'addmetadata': self.opt['addmetadata'],
```

### Comparing `videomass-5.0.0/videomass/vdms_ytdlp/ydl_extractinfo.py` & `videomass-5.0.1/videomass/vdms_ytdlp/ydl_extractinfo.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_ytdlp/ydl_mediainfo.py` & `videomass-5.0.1/videomass/vdms_ytdlp/ydl_mediainfo.py`

 * *Files identical despite different names*

### Comparing `videomass-5.0.0/videomass/vdms_ytdlp/youtubedl_ui.py` & `videomass-5.0.1/videomass/vdms_ytdlp/youtubedl_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -648,22 +648,22 @@
         """
         urls = self.parent.data_url
 
         if not self.ckbx_pl.IsChecked():
             if [url for url in urls if 'playlist' in url]:
                 if wx.MessageBox(_('The URLs contain playlists. '
                                    'Are you sure you want to continue?'),
-                                 _('Please confirm'),
-                                 wx.ICON_QUESTION | wx.YES_NO, self) == wx.NO:
+                                 _('Please confirm'), wx.ICON_QUESTION
+                                 | wx.CANCEL | wx.YES_NO, self) != wx.YES:
                     return
         if [url for url in urls if 'channel' in url]:
             if wx.MessageBox(_('The URLs contain channels. '
                                'Are you sure you want to continue?'),
-                             _('Please confirm'),
-                             wx.ICON_QUESTION | wx.YES_NO, self) == wx.NO:
+                             _('Please confirm'), wx.ICON_QUESTION
+                             | wx.CANCEL | wx.YES_NO, self) != wx.YES:
                 return
 
         if self.ckbx_id.IsChecked():
             _id = '%(title).100s-%(id)s'
         else:
             _id = '%(title).100s'
```

### Comparing `videomass-5.0.0/videomass.egg-info/PKG-INFO` & `videomass-5.0.1/videomass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: videomass
-Version: 5.0.0
+Version: 5.0.1
 Summary: Videomass is a cross-platform GUI for FFmpeg and yt-dlp
 Home-page: http://jeanslack.github.io/Videomass/
 Author: Gianluca Pernigotto
 Author-email: jeanlucperni@gmail.com
 License: GPL3 (Gnu Public License)
 Platform: All
 Classifier: Environment :: X11 Applications :: GTK
```

### Comparing `videomass-5.0.0/videomass.egg-info/SOURCES.txt` & `videomass-5.0.1/videomass.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,15 @@
 videomass/vdms_dialogs/filter_colorcorrection.py
 videomass/vdms_dialogs/filter_crop.py
 videomass/vdms_dialogs/filter_deinterlace.py
 videomass/vdms_dialogs/filter_denoisers.py
 videomass/vdms_dialogs/filter_scale.py
 videomass/vdms_dialogs/filter_stab.py
 videomass/vdms_dialogs/filter_transpose.py
+videomass/vdms_dialogs/list_warning.py
 videomass/vdms_dialogs/mediainfo.py
 videomass/vdms_dialogs/preferences.py
 videomass/vdms_dialogs/presets_addnew.py
 videomass/vdms_dialogs/renamer.py
 videomass/vdms_dialogs/set_timestamp.py
 videomass/vdms_dialogs/showlogs.py
 videomass/vdms_dialogs/shownormlist.py
```

