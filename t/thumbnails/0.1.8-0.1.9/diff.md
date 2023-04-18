# Comparing `tmp/thumbnails-0.1.8.tar.gz` & `tmp/thumbnails-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thumbnails-0.1.8.tar", last modified: Mon Mar 20 13:03:34 2023, max compression
+gzip compressed data, was "thumbnails-0.1.9.tar", last modified: Mon Mar 27 14:32:30 2023, max compression
```

## Comparing `thumbnails-0.1.8.tar` & `thumbnails-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:03:34.612644 thumbnails-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-20 13:03:23.000000 thumbnails-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-03-20 13:03:34.612644 thumbnails-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-03-20 13:03:23.000000 thumbnails-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-20 13:03:23.000000 thumbnails-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-20 13:03:34.612644 thumbnails-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-20 13:03:23.000000 thumbnails-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:03:34.608644 thumbnails-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:03:34.608644 thumbnails-0.1.8/src/thumbnails/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/pathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-20 13:03:23.000000 thumbnails-0.1.8/src/thumbnails/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:03:34.612644 thumbnails-0.1.8/src/thumbnails.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-03-20 13:03:34.000000 thumbnails-0.1.8/src/thumbnails.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-20 13:03:34.000000 thumbnails-0.1.8/src/thumbnails.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 13:03:34.000000 thumbnails-0.1.8/src/thumbnails.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-20 13:03:34.000000 thumbnails-0.1.8/src/thumbnails.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 13:03:34.000000 thumbnails-0.1.8/src/thumbnails.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-20 13:03:34.000000 thumbnails-0.1.8/src/thumbnails.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-20 13:03:34.000000 thumbnails-0.1.8/src/thumbnails.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:32:30.874921 thumbnails-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-27 14:32:20.000000 thumbnails-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-03-27 14:32:30.874921 thumbnails-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-03-27 14:32:20.000000 thumbnails-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-27 14:32:20.000000 thumbnails-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-03-27 14:32:30.874921 thumbnails-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-27 14:32:20.000000 thumbnails-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:32:30.870921 thumbnails-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:32:30.874921 thumbnails-0.1.9/src/thumbnails/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/pathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-27 14:32:20.000000 thumbnails-0.1.9/src/thumbnails/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:32:30.874921 thumbnails-0.1.9/src/thumbnails.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-03-27 14:32:30.000000 thumbnails-0.1.9/src/thumbnails.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-27 14:32:30.000000 thumbnails-0.1.9/src/thumbnails.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:32:30.000000 thumbnails-0.1.9/src/thumbnails.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-27 14:32:30.000000 thumbnails-0.1.9/src/thumbnails.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:32:30.000000 thumbnails-0.1.9/src/thumbnails.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-27 14:32:30.000000 thumbnails-0.1.9/src/thumbnails.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 14:32:30.000000 thumbnails-0.1.9/src/thumbnails.egg-info/top_level.txt
```

### Comparing `thumbnails-0.1.8/LICENSE` & `thumbnails-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thumbnails-0.1.8/PKG-INFO` & `thumbnails-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thumbnails
-Version: 0.1.8
+Version: 0.1.9
 Summary: Video thumbnail generator for modern web video players
 Home-page: https://github.com/pysnippet/thumbnails
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: Apache 2.0
 Keywords: vtt,json,thumbnails,thumbnail-generator
 Platform: unix
```

### Comparing `thumbnails-0.1.8/README.md` & `thumbnails-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `thumbnails-0.1.8/setup.cfg` & `thumbnails-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `thumbnails-0.1.8/src/thumbnails/__init__.py` & `thumbnails-0.1.9/src/thumbnails/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .thumbnail import Thumbnail
 from .thumbnail import ThumbnailExistsError
 from .thumbnail import ThumbnailFactory
 from .thumbnail import ThumbnailJSON
 from .thumbnail import ThumbnailVTT
 from .thumbnail import register_thumbnail
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 __all__ = (
     "Generator",
     "Thumbnail",
     "ThumbnailExistsError",
     "ThumbnailFactory",
     "ThumbnailJSON",
     "ThumbnailVTT",
```

### Comparing `thumbnails-0.1.8/src/thumbnails/cli.py` & `thumbnails-0.1.9/src/thumbnails/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,31 +6,34 @@
 from . import __version__
 from .constants import DEFAULT_BASE
 from .constants import DEFAULT_COMPRESS
 from .constants import DEFAULT_FORMAT
 from .constants import DEFAULT_INTERVAL
 from .constants import DEFAULT_OUTPUT
 from .constants import DEFAULT_SKIP
+from .constants import DEFAULT_WORKERS
 
 # Help messages of the particular option of the CLI.
 HELP_BASE = "The prefix of the thumbnails path can be customized."
 HELP_SKIP = "Skip the existing thumbnails. Default is not set."
 HELP_OUTPUT = "The output directory. Default is the current directory."
 HELP_FORMAT = "Output format. Default is %s." % DEFAULT_FORMAT
 HELP_COMPRESS = "The image scale coefficient. A number from 0 to 1."
 HELP_INTERVAL = "The interval between neighbor thumbnails in seconds."
+HELP_WORKERS = "Workers number for concurrent processing. Default is calculated automatically."
 
 # This defines a choice of supported values for the '--format' option of the CLI.
 format_choice = click.Choice(ThumbnailFactory.thumbnails.keys(), case_sensitive=False)
 
 
 def cli(func):
     @click.command()
     @click.option("--compress", "-C", default=DEFAULT_COMPRESS, help=HELP_COMPRESS)
     @click.option("--interval", "-I", default=DEFAULT_INTERVAL, help=HELP_INTERVAL)
+    @click.option("--workers", "-W", default=DEFAULT_WORKERS, help=HELP_WORKERS)
     @click.option("--base", "-B", default=DEFAULT_BASE, help=HELP_BASE)
     @click.option("--skip", "-S", default=DEFAULT_SKIP, help=HELP_SKIP, is_flag=True)
     @click.option("--output", "-O", default=DEFAULT_OUTPUT, type=click.Path(), help=HELP_OUTPUT)
     @click.option("--format", "-F", default=DEFAULT_FORMAT, type=format_choice, help=HELP_FORMAT)
     @click.argument("inputs", required=True, type=click.Path(), nargs=-1)
     @click.version_option(__version__, "-V", "--version")
     @click.help_option("-h", "--help")
```

### Comparing `thumbnails-0.1.8/src/thumbnails/ffmpeg.py` & `thumbnails-0.1.9/src/thumbnails/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `thumbnails-0.1.8/src/thumbnails/frame.py` & `thumbnails-0.1.9/src/thumbnails/frame.py`

 * *Files identical despite different names*

### Comparing `thumbnails-0.1.8/src/thumbnails/generator.py` & `thumbnails-0.1.9/src/thumbnails/generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .constants import DEFAULT_BASE
 from .constants import DEFAULT_COMPRESS
 from .constants import DEFAULT_FORMAT
 from .constants import DEFAULT_INTERVAL
 from .constants import DEFAULT_OUTPUT
 from .constants import DEFAULT_SKIP
+from .constants import DEFAULT_WORKERS
 from .pathtools import listdir
 from .progress import use_progress
 from .thumbnail import ThumbnailExistsError
 from .thumbnail import ThumbnailFactory
 from .video import Video
 
 
@@ -30,18 +31,32 @@
 
         self.base = DEFAULT_BASE
         self.skip = DEFAULT_SKIP
         self.output = DEFAULT_OUTPUT
         self.format = DEFAULT_FORMAT
         self.compress = DEFAULT_COMPRESS
         self.interval = DEFAULT_INTERVAL
+        self._workers = DEFAULT_WORKERS
 
         # Remove non-video files in case of input directory already contains other generated files.
         self.inputs = [file for file in self.inputs if re.match(r"^.*\.(?:(?!png|vtt|json).)+$", file)]
 
+    @property
+    def workers(self):
+        """Returns the number of workers for concurrent processing."""
+        if self._workers > 0:
+            return self._workers
+        # Limit the auto-calculated workers for super-multicore machines.
+        return min(32, len(self.inputs), (os.cpu_count() or 1) + 4)
+
+    @workers.setter
+    def workers(self, value):
+        """Sets the number of workers for concurrent processing."""
+        self._workers = value
+
     @staticmethod
     def worker(video, fmt, base, skip, output):
         """Executes the required workflows for generating a thumbnail."""
         try:
             thumbnail = ThumbnailFactory.create_thumbnail(fmt, video, base, skip, output)
         except ThumbnailExistsError:
             return print("Skipping '%s'" % os.path.relpath(video.filepath))
@@ -56,15 +71,15 @@
         try:
             return Video(self.inputs.pop(), self.compress, self.interval)
         except IndexError:
             raise StopIteration
 
     @use_progress
     def generate(self):
-        with concurrent.futures.ThreadPoolExecutor() as executor:
+        with concurrent.futures.ThreadPoolExecutor(max_workers=self.workers) as executor:
             executor.map(
                 functools.partial(
                     self.worker,
                     fmt=self.format,
                     base=self.base,
                     skip=self.skip,
                     output=self.output,
```

### Comparing `thumbnails-0.1.8/src/thumbnails/pathtools.py` & `thumbnails-0.1.9/src/thumbnails/pathtools.py`

 * *Files identical despite different names*

### Comparing `thumbnails-0.1.8/src/thumbnails/progress.py` & `thumbnails-0.1.9/src/thumbnails/progress.py`

 * *Files identical despite different names*

### Comparing `thumbnails-0.1.8/src/thumbnails/thumbnail.py` & `thumbnails-0.1.9/src/thumbnails/thumbnail.py`

 * *Files identical despite different names*

### Comparing `thumbnails-0.1.8/src/thumbnails/video.py` & `thumbnails-0.1.9/src/thumbnails/video.py`

 * *Files identical despite different names*

### Comparing `thumbnails-0.1.8/src/thumbnails.egg-info/PKG-INFO` & `thumbnails-0.1.9/src/thumbnails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thumbnails
-Version: 0.1.8
+Version: 0.1.9
 Summary: Video thumbnail generator for modern web video players
 Home-page: https://github.com/pysnippet/thumbnails
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: Apache 2.0
 Keywords: vtt,json,thumbnails,thumbnail-generator
 Platform: unix
```

### Comparing `thumbnails-0.1.8/src/thumbnails.egg-info/SOURCES.txt` & `thumbnails-0.1.9/src/thumbnails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

