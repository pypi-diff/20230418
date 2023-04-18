# Comparing `tmp/letterboxd_stats-0.1.6.tar.gz` & `tmp/letterboxd_stats-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letterboxd_stats-0.1.6.tar", last modified: Thu Apr 13 18:50:42 2023, max compression
+gzip compressed data, was "letterboxd_stats-0.1.8.tar", last modified: Tue Apr 18 12:52:03 2023, max compression
```

## Comparing `letterboxd_stats-0.1.6.tar` & `letterboxd_stats-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-13 18:50:42.603487 letterboxd_stats-0.1.6/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.6/LICENCE
--rw-rw-r--   0 marco     (1001) marco     (1001)     2963 2023-04-13 18:50:42.603487 letterboxd_stats-0.1.6/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)     2445 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.6/README.md
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-13 18:50:42.603487 letterboxd_stats-0.1.6/letterboxd_stats/
--rw-rw-r--   0 marco     (1001) marco     (1001)     1447 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.6/letterboxd_stats/__init__.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     5230 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.6/letterboxd_stats/cli.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3878 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.6/letterboxd_stats/data.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     3223 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.6/letterboxd_stats/main.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     2923 2023-04-13 18:48:10.000000 letterboxd_stats-0.1.6/letterboxd_stats/tmdb.py
--rw-rw-r--   0 marco     (1001) marco     (1001)     4697 2023-03-15 22:58:55.000000 letterboxd_stats-0.1.6/letterboxd_stats/web_scraper.py
-drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-13 18:50:42.603487 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/
--rw-rw-r--   0 marco     (1001) marco     (1001)     2963 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/entry_points.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/requires.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-04-13 18:50:42.000000 letterboxd_stats-0.1.6/letterboxd_stats.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1001) marco     (1001)      865 2023-04-13 18:48:10.000000 letterboxd_stats-0.1.6/pyproject.toml
--rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-04-13 18:50:42.603487 letterboxd_stats-0.1.6/setup.cfg
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-18 12:52:03.478683 letterboxd_stats-0.1.8/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1089 2023-03-06 16:16:14.000000 letterboxd_stats-0.1.8/LICENCE
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2963 2023-04-18 12:52:03.478683 letterboxd_stats-0.1.8/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2445 2023-04-13 13:31:47.000000 letterboxd_stats-0.1.8/README.md
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-18 12:52:03.478683 letterboxd_stats-0.1.8/letterboxd_stats/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     1460 2023-04-17 21:29:59.000000 letterboxd_stats-0.1.8/letterboxd_stats/__init__.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5222 2023-04-17 23:43:40.000000 letterboxd_stats-0.1.8/letterboxd_stats/cli.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3992 2023-04-17 23:53:40.000000 letterboxd_stats-0.1.8/letterboxd_stats/data.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     3519 2023-04-17 23:55:20.000000 letterboxd_stats-0.1.8/letterboxd_stats/main.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2949 2023-04-17 23:56:08.000000 letterboxd_stats-0.1.8/letterboxd_stats/tmdb.py
+-rw-rw-r--   0 marco     (1001) marco     (1001)     5736 2023-04-18 12:45:43.000000 letterboxd_stats-0.1.8/letterboxd_stats/web_scraper.py
+drwxrwxr-x   0 marco     (1001) marco     (1001)        0 2023-04-18 12:52:03.478683 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/
+-rw-rw-r--   0 marco     (1001) marco     (1001)     2963 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1001) marco     (1001)      434 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)        1 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       64 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/entry_points.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      126 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)       17 2023-04-18 12:52:03.000000 letterboxd_stats-0.1.8/letterboxd_stats.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1001) marco     (1001)      865 2023-04-17 23:56:33.000000 letterboxd_stats-0.1.8/pyproject.toml
+-rw-rw-r--   0 marco     (1001) marco     (1001)       38 2023-04-18 12:52:03.478683 letterboxd_stats-0.1.8/setup.cfg
```

### Comparing `letterboxd_stats-0.1.6/LICENCE` & `letterboxd_stats-0.1.8/LICENCE`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.6/PKG-INFO` & `letterboxd_stats-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxd_stats
-Version: 0.1.6
+Version: 0.1.8
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.1.6/README.md` & `letterboxd_stats-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `letterboxd_stats-0.1.6/letterboxd_stats/__init__.py` & `letterboxd_stats-0.1.8/letterboxd_stats/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,11 +27,12 @@
 
 args = parser.parse_args()
 
 folder = args.config_folder or default_folder
 path = os.path.abspath(os.path.join(folder, "config.toml"))
 if not os.path.exists(path):
     raise FileNotFoundError(
-        f"Found no configuration file in {path}. Please, add a config.toml in that folder or specify a custom one with the -c command."
+        f"Found no configuration file in {path}. "
+        + "Please, add a config.toml in that folder or specify a custom one with the -c command."
     )
 with open(path, "rb") as f:
     config = tomli.load(f)
```

### Comparing `letterboxd_stats-0.1.6/letterboxd_stats/cli.py` & `letterboxd_stats-0.1.8/letterboxd_stats/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,16 +100,16 @@
     try:
         datetime.strptime(s, "%Y-%m-%d")
     except ValueError:
         return False
     return True
 
 
-def add_film_questions(film: str):
-    print(f"Set all the infos for {film}:\n")
+def add_film_questions():
+    print("Set all the infos for the film:\n")
     specify_date = inquirer.confirm(message="Specify date?").execute()  # type: ignore
     today = datetime.today().strftime("%Y-%m-%d")
     get_specified_date = inquirer.text(  # type: ignore
         message="Set viewing date:",
         default=today,
         validate=lambda d: _validate_date(d),
         invalid_message="Wrong date format",
```

### Comparing `letterboxd_stats-0.1.6/letterboxd_stats/data.py` & `letterboxd_stats-0.1.8/letterboxd_stats/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 def read_watched_films(df: pd.DataFrame, path: str, name: str):
     df_profile = pd.read_csv(path)
     df.insert(0, "watched", np.where(df["Title"].isin(df_profile["Name"]), "[X]", "[ ]"))
     df["Release Date"] = pd.to_datetime(df["Release Date"])
     df.sort_values(by="Release Date", inplace=True)
     cli.render_table(df, name)
     movie_id = cli.select_movie_id(df[["Id", "Title"]])
-    return movie_id
+    movie_row = df.loc[df["Id"] == movie_id].iloc[0, :]
+    return movie_id, f"{movie_row['Title']} {movie_row['Release Date'].year}"
 
 
 def get_list_name(path: str):
     df = pd.read_csv(path, header=1)
     return df["Name"].iloc[0]
```

### Comparing `letterboxd_stats-0.1.6/letterboxd_stats/main.py` & `letterboxd_stats-0.1.8/letterboxd_stats/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,33 +25,37 @@
     downloader.download_stats()
 
 
 def get_movie_detail_from_url(letterboxd_url, is_diary=False):
     if letterboxd_url is not None:
         id = ws.get_tmdb_id(letterboxd_url, is_diary)
         if id is not None:
-            tmdb.get_movie_detail(id)
+            tmdb.get_movie_detail(id, letterboxd_url)
 
 
 def search_person(args_search: str):
     df, name = tmdb.get_person(args_search)
     path = os.path.expanduser(os.path.join(config["root_folder"], "static", "watched.csv"))
     check_path(path)
-    movie_id = data.read_watched_films(df, path, name)
+    movie_id, search_film = data.read_watched_films(df, path, name)
+    print(search_film)
+    letterboxd_url = ws.search_film(search_film)
     if movie_id is not None:
-        tmdb.get_movie_detail(movie_id)
+        tmdb.get_movie_detail(movie_id, ws.create_movie_url(letterboxd_url, "film_page"))
 
 
 def search_film(args_search_film: str):
-    search_result = tmdb.get_movie(args_search_film)
+    film_url = ws.search_film(args_search_film, True)
+    film_page_url = ws.create_movie_url(film_url, "film_page")
+    tmdb.get_movie_detail(ws.get_tmdb_id(film_page_url, False), film_page_url)  # type: ignore
     answer = ws.select_optional_operation()
     if answer != "Exit":
         downloader = ws.Downloader()
         downloader.login()
-        downloader.perform_operation(answer, search_result["title"])
+        downloader.perform_operation(answer, film_url)
 
 
 def get_wishlist(args_limit, args_ascending):
     path = os.path.expanduser(os.path.join(config["root_folder"], "static", "watchlist.csv"))
     check_path(path)
     letterboxd_url = data.open_file("Watchlist", path, args_limit, args_ascending)
     get_movie_detail_from_url(letterboxd_url)
```

### Comparing `letterboxd_stats-0.1.6/letterboxd_stats/tmdb.py` & `letterboxd_stats-0.1.8/letterboxd_stats/tmdb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from tmdbv3api import TMDb, Person, Movie, Search
 import pandas as pd
 from letterboxd_stats import cli
 from letterboxd_stats import config
-from letterboxd_stats import web_scraper
 
 tmdb = TMDb()
 tmdb.api_key = config["TMDB"]["api_key"]
 person = Person()
 movie = Movie()
 search = Search()
 
@@ -35,15 +34,16 @@
         raise ValueError("The selected person doesn't have any film.")
     df = pd.DataFrame(list_of_films)
     department = cli.select_value(
         df["Department"].unique(), f"Select a department for {p['name']}", known_for_department
     )
     df = df[df["Department"] == department]
     df = df.drop("Department", axis=1)
-    df["Duration"] = df.apply(lambda row: movie.details(row["Id"]).runtime, axis=1)  # type: ignore
+    if config["TMDB"]["get_list_runtimes"] is True:
+        df["Duration"] = df.apply(lambda row: movie.details(row["Id"]).runtime, axis=1)  # type: ignore
     return df, p["name"]
 
 
 def get_movie(movie_query: str):
     print(f"Searching for movie '{movie_query}'")
     search_results = search.movies({"query": movie_query})
     titles = [f"{result.title} ({result.release_date})" for result in search_results]  # type: ignore
@@ -51,27 +51,28 @@
         raise Exception("No results for your search")
     result_index = cli.select_search_result(titles)  # type: ignore
     movie_id = search_results[result_index]["id"]
     get_movie_detail(movie_id)
     return search_results[result_index]
 
 
-def get_movie_detail(movie_id: int):
+def get_movie_detail(movie_id: int, letterboxd_url=None):
     movie_details = movie.details(movie_id)
     poster = movie_details.get("poster_path")
     if poster is not None:
         cli.download_poster(poster)
     selected_details = {
         "Title": movie_details["title"],
         "Original Title": movie_details["original_title"],
         "Runtime": movie_details["runtime"],
         "Overview": movie_details["overview"],
         "Release Date": movie_details["release_date"],
-        "Letterboxd URL": web_scraper.create_movie_url(movie_details["title"], "film_page"),
     }
+    if letterboxd_url:
+        selected_details["Letterboxd Url"] = letterboxd_url
     cli.print_film(selected_details)
 
 
 def get_film_duration(film: str, year: int):
     search_results = search.movies({"query": film, "year": year})
     if len(search_results) > 0:
         first_result = search_results[0]
```

### Comparing `letterboxd_stats-0.1.6/letterboxd_stats/web_scraper.py` & `letterboxd_stats-0.1.8/letterboxd_stats/web_scraper.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import os
 from zipfile import ZipFile
 from letterboxd_stats import config
 from letterboxd_stats import cli
 import requests
 from lxml import html
-import re
 
 URL = "https://letterboxd.com"
 LOGIN_PAGE = URL + "/user/login.do"
 DATA_PAGE = URL + "/data/export"
 ADD_DIARY_URL = URL + "/s/save-diary-entry"
 MOVIE_OPERATIONS = {
     "Add to diary": "add_film_diary",
     "Add to watchlist": "add_watchlist",
     "Remove from watchlist": "remove_watchlist",
 }
 OPERATIONS_URLS = {
+    "search": lambda s: f"/search/films/{s}/?adult",
     "diary": lambda s: f"/csi/film/{s}/sidebar-user-actions/?esiAllowUser=true",
     "add_watchlist": lambda s: f"/film/{s}/add-to-watchlist/",
     "remove_watchlist": lambda s: f"/film/{s}/remove-from-watchlist/",
-    "film_page": lambda s: f"/film/{s}/",
+    "film_page": lambda s: f"/film/{s}",
 }
 
 
 class Downloader:
     def __init__(self):
         self.session = requests.Session()
         self.session.get(URL)
@@ -50,51 +50,49 @@
         archive = os.path.join(path, filename)
         with open(archive, "wb") as f:
             f.write(res.content)
         with ZipFile(archive, "r") as zip:
             zip.extractall(path)
         os.remove(archive)
 
-    def add_film_diary(self, title: str):
-        payload = cli.add_film_questions(title)
-        url = create_movie_url(title, "diary")
+    def add_film_diary(self, title_url: str):
+        payload = cli.add_film_questions()
+        url = create_movie_url(title_url, "diary")
         res = self.session.get(url)
         if res.status_code != 200:
             raise ConnectionError("It's been impossible to retireve the Letterboxd page")
         movie_page = html.fromstring(res.text)
         letterboxd_film_id = movie_page.get_element_by_id("frm-sidebar-rating").get("data-film-id")
-
         payload["filmId"] = letterboxd_film_id
         payload["__csrf"] = self.session.cookies.get("com.xk72.webparts.csrf")
         res = self.session.post(ADD_DIARY_URL, data=payload)
         if not (res.status_code == 200 and res.json()["result"] is True):
             raise ConnectionError("Add diary request failed.")
-        print(f"{title} was added to your diary.")
+        print("The movie was added to your diary.")
 
-    def add_watchlist(self, title: str):
-        url = create_movie_url(title, "add_watchlist")
+    def add_watchlist(self, title_url: str):
+        url = create_movie_url(title_url, "add_watchlist")
         res = self.session.post(url, data={"__csrf": self.session.cookies.get("com.xk72.webparts.csrf")})
         if not (res.status_code == 200 and res.json()["result"] is True):
             raise ConnectionError("Add diary request failed.")
-        print(f"{title} added to your watchlist.")
+        print("Added to your watchlist.")
 
-    def remove_watchlist(self, title: str):
-        url = create_movie_url(title, "remove_watchlist")
+    def remove_watchlist(self, title_url: str):
+        url = create_movie_url(title_url, "remove_watchlist")
         res = self.session.post(url, data={"__csrf": self.session.cookies.get("com.xk72.webparts.csrf")})
         if not (res.status_code == 200 and res.json()["result"] is True):
             raise ConnectionError("Add diary request failed.")
-        print(f"{title} removed to your watchlist.")
+        print("Removed to your watchlist.")
 
     def perform_operation(self, answer: str, link: str):
         getattr(self, MOVIE_OPERATIONS[answer])(link)
 
 
 def create_movie_url(title: str, operation: str):
-    lowercase_title = "-".join([re.sub("[^a-zA-Z0-9 ]", "", word.lower()) for word in title.split()])
-    url = URL + OPERATIONS_URLS[operation](lowercase_title)
+    url = URL + OPERATIONS_URLS[operation](title)
     return url
 
 
 def get_tmdb_id(link: str, is_diary: bool):
     res = requests.get(link)
     movie_page = html.fromstring(res.text)
     if is_diary:
@@ -108,7 +106,30 @@
         id = tmdb_link[0].get("href").split("/")[-2]
         return int(id)
     return None
 
 
 def select_optional_operation():
     return cli.select_value(["Exit"] + list(MOVIE_OPERATIONS.keys()), "Select operation:")
+
+
+def search_film(title: str, allow_selection=False):
+    search_url = URL + OPERATIONS_URLS["search"](title)
+    res = requests.get(search_url)
+    if res.status_code != 200:
+        raise ConnectionError("It's been impossible to retireve the Letterboxd page")
+    search_page = html.fromstring(res.text)
+    if allow_selection:
+        titles = search_page.xpath("//div[@class='film-detail-content']")
+        if len(titles) == 0:
+            raise ValueError(f"No film found with search query {title}")
+        title_years_directors_links = {
+            f"{t.xpath('./h2/span/a')[0].text.rstrip()} "
+            + f"({t.xpath('./h2/span//small/a')[0].text}) - "
+            + f"{t.xpath('./p/a')[0].text}": t.xpath("./h2/span/a")[0].get("href")
+            for t in titles
+        }
+        selected_film = cli.select_value(list(title_years_directors_links.keys()), "Select your film")
+        title_url = title_years_directors_links[selected_film].split("/")[-2]
+    else:
+        title_url = search_page.xpath("//span[@class='film-title-wrapper']/a")[0].get("href").split("/")[-2]
+    return title_url
```

### Comparing `letterboxd_stats-0.1.6/letterboxd_stats.egg-info/PKG-INFO` & `letterboxd_stats-0.1.8/letterboxd_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letterboxd-stats
-Version: 0.1.6
+Version: 0.1.8
 Summary: Get information about your Letterboxd activity.
 Author: mBaratta96
 Project-URL: Homepage, https://github.com/mBaratta96/letterboxd_stats
 Project-URL: Bug Tracker, https://github.com/mBaratta96/letterboxd_stats/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `letterboxd_stats-0.1.6/pyproject.toml` & `letterboxd_stats-0.1.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "letterboxd_stats"
-version = "0.1.6"
+version = "0.1.8"
 authors = [{ name = "mBaratta96" }]
 description = "Get information about your Letterboxd activity."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
```

