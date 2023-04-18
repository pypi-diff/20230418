# Comparing `tmp/pytrakt-3.4.8.tar.gz` & `tmp/pytrakt-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrakt-3.4.8.tar", last modified: Mon Oct 24 20:06:05 2022, max compression
+gzip compressed data, was "pytrakt-3.4.9.tar", last modified: Tue Oct 25 14:20:49 2022, max compression
```

## Comparing `pytrakt-3.4.8.tar` & `pytrakt-3.4.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 20:06:05.957104 pytrakt-3.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)     9139 2022-10-24 20:05:56.000000 pytrakt-3.4.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-24 20:05:56.000000 pytrakt-3.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-24 20:05:56.000000 pytrakt-3.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13298 2022-10-24 20:06:05.957104 pytrakt-3.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3398 2022-10-24 20:05:56.000000 pytrakt-3.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 20:06:05.953104 pytrakt-3.4.8/pytrakt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13298 2022-10-24 20:06:05.000000 pytrakt-3.4.8/pytrakt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-10-24 20:06:05.000000 pytrakt-3.4.8/pytrakt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 20:06:05.000000 pytrakt-3.4.8/pytrakt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 20:06:05.000000 pytrakt-3.4.8/pytrakt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-24 20:06:05.000000 pytrakt-3.4.8/pytrakt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-24 20:06:05.000000 pytrakt-3.4.8/pytrakt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-24 20:05:56.000000 pytrakt-3.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 20:06:05.957104 pytrakt-3.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-10-24 20:05:56.000000 pytrakt-3.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 20:06:05.957104 pytrakt-3.4.8/trakt/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-10-24 20:05:56.000000 pytrakt-3.4.8/trakt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-24 20:05:57.000000 pytrakt-3.4.8/trakt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4359 2022-10-24 20:05:56.000000 pytrakt-3.4.8/trakt/calendar.py
--rw-r--r--   0 runner    (1001) docker     (121)    23635 2022-10-24 20:05:56.000000 pytrakt-3.4.8/trakt/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-10-24 20:05:56.000000 pytrakt-3.4.8/trakt/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    13566 2022-10-24 20:05:56.000000 pytrakt-3.4.8/trakt/movies.py
--rw-r--r--   0 runner    (1001) docker     (121)     6190 2022-10-24 20:05:56.000000 pytrakt-3.4.8/trakt/people.py
--rw-r--r--   0 runner    (1001) docker     (121)    18575 2022-10-24 20:05:56.000000 pytrakt-3.4.8/trakt/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)    32082 2022-10-24 20:05:56.000000 pytrakt-3.4.8/trakt/tv.py
--rw-r--r--   0 runner    (1001) docker     (121)    19168 2022-10-24 20:05:56.000000 pytrakt-3.4.8/trakt/users.py
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-10-24 20:05:56.000000 pytrakt-3.4.8/trakt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 14:20:49.860428 pytrakt-3.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     9139 2022-10-25 14:20:40.000000 pytrakt-3.4.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-10-25 14:20:40.000000 pytrakt-3.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-25 14:20:40.000000 pytrakt-3.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    13298 2022-10-25 14:20:49.860428 pytrakt-3.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3398 2022-10-25 14:20:40.000000 pytrakt-3.4.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 14:20:49.860428 pytrakt-3.4.9/pytrakt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    13298 2022-10-25 14:20:49.000000 pytrakt-3.4.9/pytrakt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2022-10-25 14:20:49.000000 pytrakt-3.4.9/pytrakt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 14:20:49.000000 pytrakt-3.4.9/pytrakt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 14:20:49.000000 pytrakt-3.4.9/pytrakt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-25 14:20:49.000000 pytrakt-3.4.9/pytrakt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-25 14:20:49.000000 pytrakt-3.4.9/pytrakt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-25 14:20:40.000000 pytrakt-3.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-25 14:20:49.860428 pytrakt-3.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-10-25 14:20:40.000000 pytrakt-3.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 14:20:49.860428 pytrakt-3.4.9/trakt/
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-10-25 14:20:40.000000 pytrakt-3.4.9/trakt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-25 14:20:41.000000 pytrakt-3.4.9/trakt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-10-25 14:20:40.000000 pytrakt-3.4.9/trakt/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23635 2022-10-25 14:20:40.000000 pytrakt-3.4.9/trakt/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-10-25 14:20:40.000000 pytrakt-3.4.9/trakt/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13566 2022-10-25 14:20:40.000000 pytrakt-3.4.9/trakt/movies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6190 2022-10-25 14:20:40.000000 pytrakt-3.4.9/trakt/people.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18681 2022-10-25 14:20:40.000000 pytrakt-3.4.9/trakt/sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32286 2022-10-25 14:20:40.000000 pytrakt-3.4.9/trakt/tv.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19289 2022-10-25 14:20:40.000000 pytrakt-3.4.9/trakt/users.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-10-25 14:20:40.000000 pytrakt-3.4.9/trakt/utils.py
```

### Comparing `pytrakt-3.4.8/HISTORY.rst` & `pytrakt-3.4.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `pytrakt-3.4.8/LICENSE` & `pytrakt-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytrakt-3.4.8/PKG-INFO` & `pytrakt-3.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrakt
-Version: 3.4.8
+Version: 3.4.9
 Summary: Pythonic abstraction layer for easier scripting of the Trakt.tv REST API.
 Home-page: https://github.com/glensc/python-pytrakt
 Author: Elan Ruusamäe
 Author-email: glen@pld-linux.org
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pytrakt-3.4.8/README.rst` & `pytrakt-3.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `pytrakt-3.4.8/pytrakt.egg-info/PKG-INFO` & `pytrakt-3.4.9/pytrakt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytrakt
-Version: 3.4.8
+Version: 3.4.9
 Summary: Pythonic abstraction layer for easier scripting of the Trakt.tv REST API.
 Home-page: https://github.com/glensc/python-pytrakt
 Author: Elan Ruusamäe
 Author-email: glen@pld-linux.org
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pytrakt-3.4.8/setup.py` & `pytrakt-3.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `pytrakt-3.4.8/trakt/calendar.py` & `pytrakt-3.4.9/trakt/calendar.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,16 @@
             e_data = {
                 'airs_at': airs_date(first_aired),
                 'ids': episode.get('ids'),
                 'title': episode.get('title'),
                 'show_data': TVShow(**show_data)
             }
             self._calendar.append(
-                TVEpisode(show_data['title'], season, ep_num, **e_data)
+                TVEpisode(show_data['title'], season, ep_num,
+                          show_id=show_data['trakt'], **e_data)
             )
         self._calendar = sorted(self._calendar, key=lambda x: x.airs_at)
 
 
 class PremiereCalendar(Calendar):
     """All shows premiering during the time period specified."""
     url = 'calendars/all/shows/new'
```

### Comparing `pytrakt-3.4.8/trakt/core.py` & `pytrakt-3.4.9/trakt/core.py`

 * *Files identical despite different names*

### Comparing `pytrakt-3.4.8/trakt/errors.py` & `pytrakt-3.4.9/trakt/errors.py`

 * *Files identical despite different names*

### Comparing `pytrakt-3.4.8/trakt/movies.py` & `pytrakt-3.4.9/trakt/movies.py`

 * *Files identical despite different names*

### Comparing `pytrakt-3.4.8/trakt/people.py` & `pytrakt-3.4.9/trakt/people.py`

 * *Files identical despite different names*

### Comparing `pytrakt-3.4.8/trakt/sync.py` & `pytrakt-3.4.9/trakt/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,15 +332,17 @@
     data = yield uri
     results = []
     for d in data:
         if 'episode' in d:
             from trakt.tv import TVEpisode
             show = d.pop('show')
             extract_ids(d['episode'])
-            results.append(TVEpisode(show.get('title', None), **d['episode']))
+            results.append(TVEpisode(show.get('title', None),
+                                     show_id=show.get('trakt', None),
+                                     **d['episode']))
         elif 'movie' in d:
             from trakt.movies import Movie
             results.append(Movie(**d.pop('movie')))
         elif 'show' in d:
             from trakt.tv import TVShow
             results.append(TVShow(**d.pop('show')))
 
@@ -356,15 +358,15 @@
     :param extended: Optional value for requesting extended information.
     """
     valid_type = ('movies', 'shows', 'seasons', 'episodes')
 
     if list_type and list_type not in valid_type:
         raise ValueError('list_type must be one of {}'.format(valid_type))
 
-    uri = 'sync/watchlist'
+    uri = 'sync/watched'
     if list_type:
         uri += '/{}'.format(list_type)
 
     if list_type == 'shows' and extended:
         uri += '?extended={extended}'.format(extended=extended)
 
     data = yield uri
@@ -393,15 +395,15 @@
     :param extended: Optional value for requesting extended information.
     """
     valid_type = ('movies', 'shows')
 
     if list_type and list_type not in valid_type:
         raise ValueError('list_type must be one of {}'.format(valid_type))
 
-    uri = 'sync/watchlist'
+    uri = 'sync/collection'
     if list_type:
         uri += '/{}'.format(list_type)
 
     if extended:
         uri += '?extended={extended}'.format(extended=extended)
 
     data = yield uri
```

### Comparing `pytrakt-3.4.8/trakt/tv.py` & `pytrakt-3.4.9/trakt/tv.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,15 +435,16 @@
             self._seasons = []
             for season in data:
                 extract_ids(season)
 
                 # Prepare episodes
                 episodes = []
                 for ep in season.pop('episodes', []):
-                    episode = TVEpisode(show=self.title, **ep)
+                    episode = TVEpisode(show=self.title,
+                                        show_id=self.trakt, **ep)
                     episodes.append(episode)
                 season['episodes'] = episodes
 
                 number = season.pop('number')
                 season = TVSeason(self.title, number, **season)
                 self._seasons.append(season)
         yield self._seasons
@@ -452,26 +453,28 @@
     @get
     def last_episode(self):
         """Returns the most recently aired :class:`TVEpisode`. If no episode
         is found, `None` will be returned.
         """
         if self._last_episode is None:
             data = yield self.ext + '/last_episode?extended=full'
-            self._last_episode = data and TVEpisode(show=self.title, **data)
+            self._last_episode = data and TVEpisode(show=self.title,
+                                                    show_id=self.trakt, **data)
         yield self._last_episode
 
     @property
     @get
     def next_episode(self):
         """Returns the next scheduled to air :class:`TVEpisode`. If no episode
         is found, `None` will be returned.
         """
         if self._next_episode is None:
             data = yield self.ext + '/next_episode?extended=full'
-            self._next_episode = data and TVEpisode(show=self.title, **data)
+            self._next_episode = data and TVEpisode(show=self.title,
+                                                    show_id=self.trakt, **data)
         yield self._next_episode
 
     @property
     @get
     def watching_now(self):
         """A list of all :class:`User`'s watching a movie."""
         from .users import User
```

### Comparing `pytrakt-3.4.8/trakt/users.py` & `pytrakt-3.4.9/trakt/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,16 @@
                 season = TVSeason(show_data['title'], item_data['number'],
                                   show_data['slug'])
                 self._items.append(season)
             elif item_type == 'episode':
                 show_data = item.pop('show')
                 extract_ids(show_data)
                 episode = TVEpisode(show_data['title'], item_data['season'],
-                                    item_data['number'])
+                                    item_data['number'],
+                                    show_id=show_data['trakt'])
                 self._items.append(episode)
             elif item_type == 'person':
                 self._items.append(Person(item_data['name'],
                                           item_data['slug']))
 
         yield self._items
 
@@ -435,15 +436,16 @@
             extract_ids(movie_data)
             movie_data.update(data)
             yield Movie(**movie_data)
         else:  # media_type == 'episode'
             ep_data = data.pop('episode')
             extract_ids(ep_data)
             sh_data = data.pop('show')
-            ep_data.update(data, show=sh_data.get('title'))
+            ep_data.update(data, show=sh_data.get('title'),
+                           show_id=sh_data.get('trakt'))
             yield TVEpisode(**ep_data)
 
     @staticmethod
     def get_follower_requests():
         """Return a list of all pending follower requests for the authenticated
         user
         """
```

### Comparing `pytrakt-3.4.8/trakt/utils.py` & `pytrakt-3.4.9/trakt/utils.py`

 * *Files identical despite different names*

