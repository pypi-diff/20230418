# Comparing `tmp/pyarr-5.0.0.tar.gz` & `tmp/pyarr-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyarr-5.0.0.tar", max compression
+gzip compressed data, was "pyarr-5.1.0.tar", max compression
```

## Comparing `pyarr-5.0.0.tar` & `pyarr-5.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1056 2023-04-15 19:14:27.549990 pyarr-5.0.0/LICENSE
--rw-r--r--   0        0        0     6550 2023-04-15 19:14:27.549990 pyarr-5.0.0/README.md
--rw-r--r--   0        0        0      249 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/__init__.py
--rw-r--r--   0        0        0    30979 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/base.py
--rw-r--r--   0        0        0      101 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/const.py
--rw-r--r--   0        0        0      878 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/exceptions.py
--rw-r--r--   0        0        0    26726 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/lidarr.py
--rw-r--r--   0        0        0        0 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/__init__.py
--rw-r--r--   0        0        0     2387 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/common.py
--rw-r--r--   0        0        0      974 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/lidarr.py
--rw-r--r--   0        0        0     1758 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/radarr.py
--rw-r--r--   0        0        0     1833 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/readarr.py
--rw-r--r--   0        0        0     2057 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/models/sonarr.py
--rw-r--r--   0        0        0        0 2023-04-15 19:14:27.549990 pyarr-5.0.0/pyarr/py.typed
--rw-r--r--   0        0        0    20044 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyarr/radarr.py
--rw-r--r--   0        0        0    31128 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyarr/readarr.py
--rw-r--r--   0        0        0     8163 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyarr/request_handler.py
--rw-r--r--   0        0        0    27253 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyarr/sonarr.py
--rw-r--r--   0        0        0      300 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyarr/types.py
--rw-r--r--   0        0        0     3092 2023-04-15 19:14:27.553990 pyarr-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     7854 1970-01-01 00:00:00.000000 pyarr-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-04-18 15:33:45.763792 pyarr-5.1.0/LICENSE
+-rw-r--r--   0        0        0     6550 2023-04-18 15:33:45.763792 pyarr-5.1.0/README.md
+-rw-r--r--   0        0        0      249 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/__init__.py
+-rw-r--r--   0        0        0    32046 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/base.py
+-rw-r--r--   0        0        0      101 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/const.py
+-rw-r--r--   0        0        0     1081 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/exceptions.py
+-rw-r--r--   0        0        0    28051 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/lidarr.py
+-rw-r--r--   0        0        0        0 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/models/__init__.py
+-rw-r--r--   0        0        0     2592 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/models/common.py
+-rw-r--r--   0        0        0     1059 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/models/lidarr.py
+-rw-r--r--   0        0        0     1758 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/models/radarr.py
+-rw-r--r--   0        0        0     1833 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/models/readarr.py
+-rw-r--r--   0        0        0     2057 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/models/sonarr.py
+-rw-r--r--   0        0        0        0 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/py.typed
+-rw-r--r--   0        0        0    21301 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/radarr.py
+-rw-r--r--   0        0        0    31608 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/readarr.py
+-rw-r--r--   0        0        0     8346 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/request_handler.py
+-rw-r--r--   0        0        0    26503 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/sonarr.py
+-rw-r--r--   0        0        0      300 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyarr/types.py
+-rw-r--r--   0        0        0     3092 2023-04-18 15:33:45.767792 pyarr-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7854 1970-01-01 00:00:00.000000 pyarr-5.1.0/PKG-INFO
```

### Comparing `pyarr-5.0.0/LICENSE` & `pyarr-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyarr-5.0.0/README.md` & `pyarr-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyarr-5.0.0/pyarr/base.py` & `pyarr-5.1.0/pyarr/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,22 @@
             page_size (Optional[int], optional): Number of items per page. Defaults to None.
             sort_key (Optional[PyarrSortKey], optional): Field to sort by. Defaults to None.
             sort_dir (Optional[PyarrSortDirection], optional): Direction to sort the items. Defaults to None.
 
         Returns:
            JsonObject: Dictionary with items
         """
-        params: dict[str, Union[int, PyarrHistorySortKey, PyarrSortDirection]] = {}
+        params: dict[
+            str,
+            Union[
+                int,
+                PyarrHistorySortKey,
+                PyarrSortDirection,
+            ],
+        ] = {}
 
         if page:
             params["page"] = page
 
         if page_size:
             params["pageSize"] = page_size
 
@@ -388,14 +395,22 @@
             data (JsonObject): All parameters to update
 
         Returns:
             JsonObject: Dictionary of updated record
         """
         return self._put(f"qualitydefinition/{id_}", self.ver_uri, data=data)
 
+    def get_quality_profile_schema(self) -> JsonArray:
+        """Get the schemas for quality profiles
+
+        Returns:
+            JsonArray: List of dictionaries with items
+        """
+        return self._get("qualityprofile/schema", self.ver_uri)
+
     # INDEXER
 
     # GET /indexer/schema
     def get_indexer_schema(
         self, implementation: Optional[PyarrIndexerSchema] = None
     ) -> Union[JsonArray, JsonObject]:
         """Get possible indexer connections
@@ -959,7 +974,28 @@
             id_ (Optional[int], optional): Database ID of the command. Defaults to None.
 
         Returns:
             Union[JsonArray, JsonObject]: List of dictionaries with items
         """
         path = f"command{f'/{id_}' if id_ else ''}"
         return self._get(path, self.ver_uri)
+
+    # GET /language/{id}
+    # TODO: update notes and tests for Sonarr once resolved
+    def get_language(
+        self, id_: Optional[int] = None
+    ) -> Union[JsonArray, dict[Any, Any]]:
+        """Gets all language profiles or specific one with id
+
+        Note:
+            This method is not working in Sonarr, use get_language_profile()
+            I have raised this with the Sonarr team.
+
+        Args:
+            id_ (Optional[int], optional): Language profile id from database. Defaults to None.
+
+        Returns:
+            Union[JsonArray, dict[Any, Any]]: List of dictionaries with items
+        """
+
+        path = f"language{f'/{id_}' if id_ else ''}"
+        return self._get(path, self.ver_uri)
```

### Comparing `pyarr-5.0.0/pyarr/exceptions.py` & `pyarr-5.1.0/pyarr/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,7 +36,15 @@
 
 class PyarrMissingArgument(PyarrError):
     """Missing one of multiple possible arguments"""
 
 
 class PyarrBadRequest(PyarrError):
     """Bad Request, possible bug."""
+
+
+class PyarrServerError(PyarrError):
+    """Server Error, missing or incorrect options."""
+
+    def __init__(self, message, response):
+        super().__init__(message)
+        self.response = response
```

### Comparing `pyarr-5.0.0/pyarr/lidarr.py` & `pyarr-5.1.0/pyarr/lidarr.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,27 +231,31 @@
     def add_album(
         self,
         album: JsonObject,
         root_dir: str,
         quality_profile_id: Optional[int] = None,
         metadata_profile_id: Optional[int] = None,
         monitored: bool = True,
+        artist_monitored: bool = True,
         artist_monitor: LidarrArtistMonitor = "all",
         artist_search_for_missing_albums: bool = False,
+        search_for_new_album: bool = False,
     ) -> JsonObject:
         """Adds an album to Lidarr
 
         Args:
             album (JsonObject): Album record from `lookup()`
             root_dir (str): Location to store music
             quality_profile_id (Optional[int], optional): Quality profile ID. Defaults to None.
             metadata_profile_id (Optional[int], optional): Metadata profile ID. Defaults to None.
             monitored (bool, optional): Should the album be monitored. Defaults to True.
+            artist_monitored (bool, optional): Should the album be monitored. Defaults to True.
             artist_monitor (LidarrArtistMonitor, optional): What level to monitor the artist. Defaults to "all".
             artist_search_for_missing_albums (bool, optional): Search for any missing albums by this artist. Defaults to False.
+            search_for_new_album (bool, optional): Search for new albums by this artist. Defaults to False.
 
         Returns:
             JsonObject: Dictionary with added record
         """
         if quality_profile_id is None:
             try:
                 quality_profile_id = self.get_quality_profile()[0]["id"]
@@ -263,23 +267,26 @@
             try:
                 metadata_profile_id = self.get_metadata_profile()[0]["id"]
             except IndexError as exception:
                 raise PyarrMissingProfile(
                     "There is no Metadata Profile setup"
                 ) from exception
 
-        album["id"] = 0
         album["artist"]["metadataProfileId"] = metadata_profile_id
         album["artist"]["qualityProfileId"] = quality_profile_id
         album["artist"]["rootFolderPath"] = root_dir
+        album["artist"]["monitored"] = artist_monitored
         album["artist"]["addOptions"] = {
             "monitor": artist_monitor,
             "searchForMissingAlbums": artist_search_for_missing_albums,
         }
         album["monitored"] = monitored
+        album["addOptions"] = {
+            "searchForNewAlbum": search_for_new_album,
+        }
         return self._post("album", self.ver_uri, data=album)
 
     def upd_album(self, data: JsonObject) -> JsonObject:
         """Update an album
 
         Args:
             data (JsonObject): data to update albums
@@ -733,27 +740,47 @@
             "retag",
             self.ver_uri,
             params=params,
         )
 
     # POST /qualityprofile
     def add_quality_profile(
-        self, name: str, upgrades_allowed: bool, cutoff: int, items: list
+        self,
+        name: str,
+        upgrade_allowed: bool,
+        cutoff: int,
+        schema: dict[str, Any],
+        language: dict,
+        min_format_score: int = 0,
+        cutoff_format_score: int = 0,
+        format_items: list = None,
     ) -> JsonObject:
-        """Add new quality profile
+        """Add new quality profile.
 
         Args:
             name (str): Name of the profile
-            upgrades_allowed (bool): Are upgrades in quality allowed?
+            upgrade_allowed (bool): Are upgrades in quality allowed?
             cutoff (int): ID of quality definition to cutoff at. Must be an allowed definition ID.
-            items (list): Add a list of items (from `get_quality_definition()`)
+            schema (dict[str, Any]): Add the profile schema (from `get_quality_profile_schema()`)
+            language (dict): Language profile (from `get_language()`)
+            min_format_score (int, optional): Minimum format score. Defaults to 0.
+            cutoff_format_score (int, optional): Cutoff format score. Defaults to 0.
+            format_items (list, optional): Format items. Defaults to [].
+
+        Note:
+            Update the result from `get_quality_profile_schema()` set the items you need
+            from `"allowed": false` to `"allowed": true`. See tests for more details.
 
         Returns:
             JsonObject: An object containing the profile
         """
-        data = {
-            "name": name,
-            "upgradeAllowed": upgrades_allowed,
-            "cutoff": cutoff,
-            "items": items,
-        }
-        return self._post("qualityprofile", self.ver_uri, data=data)
+        if format_items is None:
+            format_items = []
+        schema["name"] = name
+        schema["upgradeAllowed"] = upgrade_allowed
+        schema["cutoff"] = cutoff
+        schema["formatItems"] = format_items
+        schema["language"] = language
+        schema["minFormatScore"] = min_format_score
+        schema["cutoffFormatScore"] = cutoff_format_score
+
+        return self._post("qualityprofile", self.ver_uri, data=schema)
```

### Comparing `pyarr-5.0.0/pyarr/models/common.py` & `pyarr-5.1.0/pyarr/models/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,17 +19,30 @@
 """Block list sort keys
 
 Note:
     There may be more, but these are not well documented
     within Arr api docs.
 """
 
-PyarrHistorySortKey = Literal["time"]
+PyarrHistorySortKey = Literal[
+    "id",
+    "date",
+    "eventType",
+    "series.title",
+    "episode.title",
+    "movieFile.relativePath",
+    "sourceTitle",
+    "status",
+]
 """History sort keys
 
+series.title (Sonarr)
+episode.title (Sonarr)
+status (Lidarr only)
+
 Note:
     There may be more, but these are not well documented
     within Arr api docs.
 """
 
 PyarrTaskSortKey = Literal["timeleft"]
 """Task sort keys
```

### Comparing `pyarr-5.0.0/pyarr/models/lidarr.py` & `pyarr-5.1.0/pyarr/models/lidarr.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,7 +46,10 @@
     "LastFmUser",
     "LidarrLists",
     "MusicBrainzSeries",
     "SpotifyFollowedArtists",
     "SpotifyPlaylist",
     "SpotifySavedAlbums",
 ]
+
+#: Lidarr History Sort Keys
+LidarrHistorySortKey = Literal["sourceTitle", "status"]
```

### Comparing `pyarr-5.0.0/pyarr/models/radarr.py` & `pyarr-5.1.0/pyarr/models/radarr.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.0.0/pyarr/models/readarr.py` & `pyarr-5.1.0/pyarr/models/readarr.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.0.0/pyarr/models/sonarr.py` & `pyarr-5.1.0/pyarr/models/sonarr.py`

 * *Files identical despite different names*

### Comparing `pyarr-5.0.0/pyarr/radarr.py` & `pyarr-5.1.0/pyarr/radarr.py`

 * *Files 7% similar despite different names*

```diff
@@ -537,34 +537,58 @@
         Returns:
             JsonArray: List of dictionaries with items
         """
         return self._get("customfilter", self.ver_uri)
 
     # POST /qualityprofile
     def add_quality_profile(
-        self, name: str, upgrades_allowed: bool, cutoff: int, items: list
+        self,
+        name: str,
+        schema: dict[str, Any],
+        cutoff: int,
+        upgrade_allowed: Optional[bool] = None,
+        language: Optional[dict[str, Any]] = None,
+        min_format_score: Optional[int] = None,
+        cutoff_format_score: Optional[int] = None,
+        format_items: Optional[list] = None,
     ) -> JsonObject:
         """Add new quality profile
 
         Args:
             name (str): Name of the profile
-            upgrades_allowed (bool): Are upgrades in quality allowed?
+            schema (dict[str, Any]): Add the profile schema (from `get_quality_profile_schema()`)
             cutoff (int): ID of quality definition to cutoff at. Must be an allowed definition ID.
-            items (list): Add a list of items (from `get_quality_definition()`)
+            upgrade_allowed (bool, optional): Are upgrades in quality allowed?. Default provided by schema.
+            language (dict, optional): Language profile (from `get_language()`). Default provided by schema.
+            min_format_score (int, optional): Minimum format score. Default provided by schema.
+            cutoff_format_score (int, optional): Cutoff format score. Default provided by schema.
+            format_items (list, optional): Format items. Default provided by schema.
+
+        Note:
+            Update the result from `get_quality_profile_schema()` set the items you need
+            from `"allowed": false` to `"allowed": true`. See tests for more details.
 
         Returns:
             JsonObject: An object containing the profile
         """
-        data = {
-            "name": name,
-            "upgradeAllowed": upgrades_allowed,
-            "cutoff": cutoff,
-            "items": items,
-        }
-        return self._post("qualityprofile", self.ver_uri, data=data)
+        schema["name"] = name
+        schema["cutoff"] = cutoff
+
+        if format_items is not None:
+            schema["formatItems"] = format_items
+        if language is not None:
+            schema["language"] = language
+        if upgrade_allowed is not None:
+            schema["upgradeAllowed"] = upgrade_allowed
+        if min_format_score is not None:
+            schema["minFormatScore"] = min_format_score
+        if cutoff_format_score is not None:
+            schema["cutoffFormatScore"] = cutoff_format_score
+
+        return self._post("qualityprofile", self.ver_uri, data=schema)
 
     # GET /manualimport
     def get_manual_import(
         self,
         folder: str,
         download_id: Optional[str] = None,
         movie_id: Optional[int] = None,
```

### Comparing `pyarr-5.0.0/pyarr/readarr.py` & `pyarr-5.1.0/pyarr/readarr.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,28 +428,33 @@
         book["monitored"] = monitored
         book["author"]["manualAdd"] = True
         book["addOptions"] = {"searchForNewBook": search_for_new_book}
 
         return self._post("book", self.ver_uri, data=book)
 
     # PUT /book/{id}
-    def upd_book(self, id_: int, data: JsonObject) -> JsonObject:
-        """Update the given book, currently only monitored is changed, all other modifications are ignored.
+    def upd_book(self, book: JsonObject, editions: JsonArray) -> JsonObject:
+        """Update the given book.
 
         Note:
-            To be used in conjunction with get_book()
+            To be used in conjunction with get_book() and get_edition()
+
+            Currently only monitored states are updated (for the book and edition).
 
         Args:
             id_ (int): Book database ID to update
-            data (JsonObject): All parameters to update book
+            book (JsonObject): All parameters to update book
+            editions (JsonArray): List of editions to update book from `get_edition()`
 
         Returns:
             JsonObject: Dictionary with updated record
         """
-        return self._put(f"book/{id_}", self.ver_uri, data=data)
+        book["editions"] = editions
+
+        return self._put("book", self.ver_uri, data=book)
 
     # PUT /book/monitor
     def upd_book_monitor(
         self, book_ids: list[int], monitored: bool = True
     ) -> JsonArray:
         """Update book monitored status
 
@@ -837,7 +842,20 @@
         Args:
             data (JsonObject): Data containing changes
 
         Returns:
             JsonObject: Dictionary of updated record
         """
         return self._put("manualimport", self.ver_uri, data=data)
+
+    # GET /edition
+    def get_edition(self, id_: int) -> JsonArray:
+        """Get edition's for specific book
+
+        Args:
+            id_ (int): Database ID of book
+
+        Returns:
+            JsonObject: Dictionary of editions
+        """
+
+        return self._get("edition", self.ver_uri, params={"bookId": id_})
```

### Comparing `pyarr-5.0.0/pyarr/request_handler.py` & `pyarr-5.1.0/pyarr/request_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .exceptions import (
     PyarrAccessRestricted,
     PyarrBadGateway,
     PyarrBadRequest,
     PyarrConnectionError,
     PyarrMethodNotAllowed,
     PyarrResourceNotFound,
+    PyarrServerError,
     PyarrUnauthorizedError,
 )
 from .types import _ReturnType
 
 
 class RequestHandler:
     """Base class for API Wrappers"""
@@ -237,18 +238,23 @@
         )
     if res.status_code == 403:
         raise PyarrAccessRestricted(
             "Access restricted. Please ensure API Key has correct permissions", {}
         )
     if res.status_code == 404:
         raise PyarrResourceNotFound("Resource not found")
-    if res.status_code == 502:
-        raise PyarrBadGateway("Bad Gateway. Check your server is accessible")
     if res.status_code == 405:
         raise PyarrMethodNotAllowed(f"The endpoint {res.url} is not allowed")
+    if res.status_code == 500:
+        raise PyarrServerError(
+            f"Internal Server Error: {res.json()['message']}",
+            res.json(),
+        )
+    if res.status_code == 502:
+        raise PyarrBadGateway("Bad Gateway. Check your server is accessible.")
 
     content_type = res.headers.get("Content-Type", "")
     if "application/json" in content_type:
         return res.json()
     else:
         assert isinstance(res, Response)
     return res
```

### Comparing `pyarr-5.0.0/pyarr/sonarr.py` & `pyarr-5.1.0/pyarr/sonarr.py`

 * *Files 6% similar despite different names*

```diff
@@ -514,22 +514,15 @@
         series["monitored"] = monitored
         series["addOptions"] = {
             "ignoreEpisodesWithFiles": ignore_episodes_with_files,
             "ignoreEpisodesWithoutFiles": ignore_episodes_without_files,
             "searchForMissingEpisodes": search_for_missing_episodes,
         }
 
-        response: dict[str, Any] = self._post("series", self.ver_uri, data=series)
-        for item in response:
-            if "errorMessage" in item:
-                raise Exception(item)
-            else:
-                continue
-
-        return response
+        return self._post("series", self.ver_uri, data=series)
 
     # PUT /series
     def upd_series(self, data: JsonObject) -> JsonObject:
         """Update an existing series
 
         Args:
             data (JsonObject): contains data obtained by get_series()
@@ -613,15 +606,18 @@
             sort_key (Optional[PyarrHistorySortKey], optional): Field to sort by. Defaults to None.
             sort_dir (Optional[PyarrSortDirection], optional): Direction to sort the items. Defaults to None.
             id_ (Optional[int], optional): Filter to a specific episode ID. Defaults to None.
 
         Returns:
            JsonObject: Dictionary with items
         """
-        params: dict[str, Union[int, PyarrHistorySortKey, PyarrSortDirection]] = {}
+        params: dict[
+            str,
+            Union[int, PyarrHistorySortKey, PyarrSortDirection],
+        ] = {}
 
         if page:
             params["page"] = page
 
         if page_size:
             params["pageSize"] = page_size
 
@@ -641,52 +637,30 @@
         self, id_: Optional[int] = None
     ) -> Union[JsonArray, dict[Any, Any]]:
         """Gets all language profiles or specific one with id
 
         Args:
             id_ (Optional[int], optional): Language profile id from database. Defaults to None.
 
+        Note:
+            This method is deprecated and will be removed in a
+            future release. Please use get_language()
+
         Returns:
             Union[JsonArray, dict[Any, Any]]: List of dictionaries with items
         """
+        warn(
+            "This method is deprecated and will be removed in a future release. Please use get_language()",
+            DeprecationWarning,
+            stacklevel=2,
+        )
 
         path = f"languageprofile{f'/{id_}' if id_ else ''}"
         return self._get(path, self.ver_uri)
 
-    # PUT /languageprofile/{id}
-    def upd_language_profile(self, id_: int, data: JsonObject) -> JsonObject:
-        """Update the language profile data
-
-        Note:
-            To be used in conjunction with get_language_profile()
-
-        Args:
-            id_ (int): Profile ID to Update
-            data (JsonObject): All parameters to update
-
-        Returns:
-            JsonObject: Dictionary of updated record
-        """
-
-        return self._put(f"languageprofile/{id_}", self.ver_uri, data=data)
-
-    # DELETE /languageprofile
-    def del_language_profile(
-        self, id_: int
-    ) -> Union[Response, JsonObject, dict[Any, Any]]:
-        """Removes a specific language profile from the blocklist
-
-        Args:
-            id_ (int): Profile ID from database
-
-        Returns:
-            Response: HTTP Response
-        """
-        return self._delete(f"languageprofile/{id_}", self.ver_uri)
-
     # GET /languageprofile/schema/{id}
     def get_language_profile_schema(
         self, id_: Optional[int] = None
     ) -> Union[JsonArray, dict[Any, Any]]:
         """Gets all language profile schemas or specific one with id
 
         Args:
```

### Comparing `pyarr-5.0.0/pyproject.toml` & `pyarr-5.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyarr"
-version = "5.0.0"
+version = "5.1.0"
 description = "Synchronous Sonarr, Radarr, Lidarr and Readarr API's for Python"
 authors = ["Steven Marks <marksie1988@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["sonarr", "radarr", "readarr", "lidarr", "api", "wrapper", "plex"]
 homepage = "https://github.com/totaldebug/pyarr"
 repository = "https://github.com/totaldebug/pyarr"
```

### Comparing `pyarr-5.0.0/PKG-INFO` & `pyarr-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarr
-Version: 5.0.0
+Version: 5.1.0
 Summary: Synchronous Sonarr, Radarr, Lidarr and Readarr API's for Python
 Home-page: https://github.com/totaldebug/pyarr
 License: MIT
 Keywords: sonarr,radarr,readarr,lidarr,api,wrapper,plex
 Author: Steven Marks
 Author-email: marksie1988@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyarr Version: 5.0.0 Summary: Synchronous Sonarr,
+Metadata-Version: 2.1 Name: pyarr Version: 5.1.0 Summary: Synchronous Sonarr,
 Radarr, Lidarr and Readarr API's for Python Home-page: https://github.com/
 totaldebug/pyarr License: MIT Keywords:
 sonarr,radarr,readarr,lidarr,api,wrapper,plex Author: Steven Marks Author-
 email: marksie1988@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

