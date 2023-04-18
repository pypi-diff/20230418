# Comparing `tmp/seo_position_tracker-1.5.0.tar.gz` & `tmp/seo_position_tracker-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seo_position_tracker-1.5.0.tar", max compression
+gzip compressed data, was "seo_position_tracker-1.5.1.tar", max compression
```

## Comparing `seo_position_tracker-1.5.0.tar` & `seo_position_tracker-1.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1539 2023-03-17 08:59:50.159992 seo_position_tracker-1.5.0/LICENSE
--rw-r--r--   0        0        0      939 2023-03-17 09:18:49.059905 seo_position_tracker-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     8205 2023-03-17 09:29:58.968731 seo_position_tracker-1.5.0/README.md
--rw-r--r--   0        0        0       52 2023-03-17 08:59:50.161986 seo_position_tracker-1.5.0/seo_position_tracker/__init__.py
--rw-r--r--   0        0        0     4486 2023-03-17 09:14:33.993015 seo_position_tracker-1.5.0/seo_position_tracker/main.py
--rw-r--r--   0        0        0    13324 2023-03-17 08:59:50.161986 seo_position_tracker-1.5.0/seo_position_tracker/seo_position_tracker.py
--rw-r--r--   0        0        0     9087 1970-01-01 00:00:00.000000 seo_position_tracker-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1539 2023-04-18 09:57:11.290604 seo_position_tracker-1.5.1/LICENSE
+-rw-r--r--   0        0        0      985 2023-04-18 09:57:11.291599 seo_position_tracker-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9006 2023-04-18 10:07:19.784283 seo_position_tracker-1.5.1/README.md
+-rw-r--r--   0        0        0       52 2023-04-18 09:57:11.291599 seo_position_tracker-1.5.1/seo_position_tracker/__init__.py
+-rw-r--r--   0        0        0     4486 2023-04-18 09:57:11.292546 seo_position_tracker-1.5.1/seo_position_tracker/main.py
+-rw-r--r--   0        0        0    13360 2023-04-18 09:57:11.292546 seo_position_tracker-1.5.1/seo_position_tracker/seo_position_tracker.py
+-rw-r--r--   0        0        0     9813 1970-01-01 00:00:00.000000 seo_position_tracker-1.5.1/PKG-INFO
```

### Comparing `seo_position_tracker-1.5.0/LICENSE` & `seo_position_tracker-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seo_position_tracker-1.5.0/pyproject.toml` & `seo_position_tracker-1.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "seo-position-tracker"
 homepage = "https://github.com/dimitryzub/seo-position-tracker"
-version = "1.5.0"
+version = "1.5.1"
 description = "A simple Python package for SEO position tracking from Google and other search engines."
 authors = ["Dimitry Zub <dimitryzub@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "Operating System :: Microsoft :: Windows",
@@ -15,15 +15,17 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
-google-search-results = "^2.4.1"
-pandas = "^1.4.3"
+google-search-results = "^2.4.2"
 
 [tool.poetry.dev-dependencies]
 
+[tool.poetry.scripts]
+seo = "seo_position_tracker.main:main"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `seo_position_tracker-1.5.0/README.md` & `seo_position_tracker-1.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,28 @@
+<div align="center">
+<p>Sponsor of the project:</p>
+<div>
+   <img src="https://user-images.githubusercontent.com/81998012/231172985-81515e8b-bc41-46b4-83fa-d129d5f3e718.svg" width="100" alt="SerpApi">
+</div>
+<a href="https://serpapi.com">
+  <b>API to get search engine results with ease.</b>
+</a>
+</div>
+
+______
+
 <h1 align="center">SEO Position Tracker 📡</h1>
 
 <p align="center">A simple Python CLI and in-code SEO position tracking tool for Google and 6 other search engines.</p>
 <p align="center">This project uses <a href="http://serpapi.com/">SerpApi</a></p>
 
+<div align="center">
+   <img src="https://user-images.githubusercontent.com/78694043/231775565-1b007b07-e168-4b88-9518-865148e1d2a4.svg" width="700" alt="SerpApi">
+</div>
+
 
 <div align="center">
 
   <a href="https://pepy.tech/project/seo-position-tracker">![Downloads](https://static.pepy.tech/personalized-badge/seo-position-tracker?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)</a>
   <a href="">![licence](https://img.shields.io/github/license/dimitryzub/seo-position-tracker?color=blue)</a>
 
 </div>
@@ -27,36 +43,53 @@
 
 ```bash
 $ pip install seo-position-tracker
 ```
 
 Install from source:
 
+Windows:
+
 ```bash
 $ git clone https://github.com/dimitryzub/seo-position-tracking.git
-$ cd seo_position_tracker/
-$ python -m venv env && source env/bin/activate # or env/Scripts/activate for Windows
+$ cd seo-position-tracker/
+$ python -m venv env
+$ env/Scripts/activate
+$ pip install poetry
 $ poetry install
 ```
 
 If you get an error, try: 
+
 ```bash
 $ pip install chardet 
 $ poetry install
 ```
 
 
 ## 🤹‍♂️Usage
 
-#### Available CLI arugments:
+You can envoke script by this two commands. 
+
+Examples below will show usage with `poetry run seo <command>`, but you can use `python main.py <command>` instead.  
 
 ```bash
+$ cd seo_position_tracker # dive inside the module folder
 $ python main.py -h
 ```
 
+```bash
+$ poetry run seo -h
+```
+
+<details>
+<summary>
+Available arugments
+</summary>
+
 ```lang-none
 SerpApi SEO position tracker [-h] [-q] [-tk  [...]] [-tw  [...]] [-se  [...]] [-ak] [-hl] [-gl] [-loc] [-d] [-st]
 
 A simple Python CLI for SEO position tracking from Google, Baidu, Bing, DuckDuckGo, Yahoo, Yandex and Naver.
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -75,23 +108,26 @@
                         countries"
   -loc , --location     Location of the search. Supported only for "google", "bing", "duckduckgo" and "yandex" engines. Default "None". Find more by Googling: "SerpApi supported    
                         <engine> locations"
   -d , --domain         Search engine domain to use. Supported only for "google", "yahoo" and "yandex" engines. Default "None". Find more by Googling: "SerpApi supported <engine>   
                         domains"
   -st , --save-to       Saves the results in the current directory in the selected format (CSV, JSON, TXT). Default CSV.
 
+
 Found a bug? Open issue: https://github.com/dimitryzub/seo-position-tracker/issues
 ```
 
+</details>
+
 ## 🤹‍♂️Examples
 
 #### Extracting positions from all search engines for a given query with a target website and a target keyword:
 
 ```bash
-$ python main.py --api-key=<your_serpapi_api_key> \
+$ poetry run seo --api-key=<your_serpapi_api_key> \
 -q "minecraft" \
 -tk official \
 -tw minecraft.net
 ```
 
 ```json
 [
@@ -151,15 +187,15 @@
   }
 ]
 ```
 
 #### Extracting positions from 3 search engines with default arguments and saving to JSON:
 
 ```bash
-$ python main.py --api-key=<your_serpapi_api_key> \
+$ poetry run seo --api-key=<your_serpapi_api_key> \
 -se google bing duckduckgo \
 -st JSON
 ```
 
 ```json
 [
   {
@@ -182,15 +218,15 @@
   }
 ]
 ```
 
 #### Extracting positions from one engine with all arguments for it:
 
 ```bash       
-$ python main.py --api-key=<your_serpapi_api_key> \
+$ poetry run seo --api-key=<your_serpapi_api_key> \
 -q serpapi \
 -tk serpapi \
 -tw https://serpapi.com/ https://github.com/ \
 -se google \
 -hl de \
 -gl de \
 -loc Germany \
```

#### html2text {}

```diff
@@ -1,78 +1,86 @@
+                            Sponsor of the project:
+                                   [SerpApi]
+                  API_to_get_search_engine_results_with_ease.
+______
                     ****** SEO Position Tracker ð¡ ******
   A simple Python CLI and in-code SEO position tracking tool for Google and 6
                              other search engines.
                            This project uses SerpApi
+                                   [SerpApi]
     ![Downloads](https://static.pepy.tech/personalized-badge/seo-position-
 tracker?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)
    ![licence](https://img.shields.io/github/license/dimitryzub/seo-position-
                               tracker?color=blue)
 ## ð Current search engines support - Google Search - first 100 organic
 results. - Baidu Search - first 50 organic results. - Bing Search - first 50
 organic results. - DuckDuckGo Search - up to 30 organic results. - Yahoo!
 Search - first 10 organic results. - Yandex Search - up to 15 organic results.
 - Naver Search - first 15 organic results. ## âï¸Installation ```bash $ pip
-install seo-position-tracker ``` Install from source: ```bash $ git clone
-https://github.com/dimitryzub/seo-position-tracking.git $ cd
-seo_position_tracker/ $ python -m venv env && source env/bin/activate # or env/
-Scripts/activate for Windows $ poetry install ``` If you get an error, try:
-```bash $ pip install chardet $ poetry install ``` ## ð¤¹ââï¸Usage ####
-Available CLI arugments: ```bash $ python main.py -h ``` ```lang-none SerpApi
-SEO position tracker [-h] [-q] [-tk [...]] [-tw [...]] [-se [...]] [-ak] [-hl]
-[-gl] [-loc] [-d] [-st] A simple Python CLI for SEO position tracking from
-Google, Baidu, Bing, DuckDuckGo, Yahoo, Yandex and Naver. optional arguments: -
-h, --help show this help message and exit -q , --query Search query. Default
-"coffee". -tk [ ...], --target-keywords [ ...] Target keywords to track.
-Default "['coffee']". -tw [ ...], --target-websites [ ...] Target websites to
-track. Default "['starbucks.com']". -se [ ...], --search-engine [ ...] Choosing
-a search engine to track: "google", "baidu", "bing", "duckduckgo", "yahoo",
-"yandex", "naver". You can select multiple search engines. All search engines
-are selected by default. -ak , --api-key Your SerpApi API key: https://
-serpapi.com/manage-api-key. Default is a test API key to test CLI. -hl , --lang
-Language of the search. Supported only for "google", "baidu", "yahoo" and
-"yandex" engines. Default "None". Find more by Googling: "SerpApi supported
-languages" -gl , --country Country of the search. Supported only for "google",
-"bing" and "yahoo" engines. Default "None". Find more by Googling: "SerpApi
-supported  countries" -loc , --location Location of the search. Supported only
-for "google", "bing", "duckduckgo" and "yandex" engines. Default "None". Find
-more by Googling: "SerpApi supported  locations" -d , --domain Search engine
-domain to use. Supported only for "google", "yahoo" and "yandex" engines.
-Default "None". Find more by Googling: "SerpApi supported  domains" -st , --
-save-to Saves the results in the current directory in the selected format (CSV,
-JSON, TXT). Default CSV. Found a bug? Open issue: https://github.com/
-dimitryzub/seo-position-tracker/issues ``` ## ð¤¹ââï¸Examples ####
-Extracting positions from all search engines for a given query with a target
-website and a target keyword: ```bash $ python main.py --api-key= \ -
-q "minecraft" \ -tk official \ -tw minecraft.net ``` ```json [ { "engine":
-"google", "position": 1, "title": "Welcome to the Minecraft Official Site |
+install seo-position-tracker ``` Install from source: Windows: ```bash $ git
+clone https://github.com/dimitryzub/seo-position-tracking.git $ cd seo-
+position-tracker/ $ python -m venv env $ env/Scripts/activate $ pip install
+poetry $ poetry install ``` If you get an error, try: ```bash $ pip install
+chardet $ poetry install ``` ## ð¤¹ââï¸Usage You can envoke script by
+this two commands. Examples below will show usage with `poetry run seo `, but
+you can use `python main.py ` instead. ```bash $ cd seo_position_tracker # dive
+inside the module folder $ python main.py -h ``` ```bash $ poetry run seo -
+h ```   Available arugments  ```lang-none SerpApi SEO position tracker [-h] [-
+q] [-tk [...]] [-tw [...]] [-se [...]] [-ak] [-hl] [-gl] [-loc] [-d] [-st] A
+simple Python CLI for SEO position tracking from Google, Baidu, Bing,
+DuckDuckGo, Yahoo, Yandex and Naver. optional arguments: -h, --help show this
+help message and exit -q , --query Search query. Default "coffee". -tk [ ...],
+--target-keywords [ ...] Target keywords to track. Default "['coffee']". -tw
+[ ...], --target-websites [ ...] Target websites to track. Default "
+['starbucks.com']". -se [ ...], --search-engine [ ...] Choosing a search engine
+to track: "google", "baidu", "bing", "duckduckgo", "yahoo", "yandex", "naver".
+You can select multiple search engines. All search engines are selected by
+default. -ak , --api-key Your SerpApi API key: https://serpapi.com/manage-api-
+key. Default is a test API key to test CLI. -hl , --lang Language of the
+search. Supported only for "google", "baidu", "yahoo" and "yandex" engines.
+Default "None". Find more by Googling: "SerpApi supported  languages" -gl , --
+country Country of the search. Supported only for "google", "bing" and "yahoo"
+engines. Default "None". Find more by Googling: "SerpApi supported  countries"
+-loc , --location Location of the search. Supported only for "google", "bing",
+"duckduckgo" and "yandex" engines. Default "None". Find more by Googling:
+"SerpApi supported  locations" -d , --domain Search engine domain to use.
+Supported only for "google", "yahoo" and "yandex" engines. Default "None". Find
+more by Googling: "SerpApi supported  domains" -st , --save-to Saves the
+results in the current directory in the selected format (CSV, JSON, TXT).
+Default CSV. Found a bug? Open issue: https://github.com/dimitryzub/seo-
+position-tracker/issues ```  ## ð¤¹ââï¸Examples #### Extracting positions
+from all search engines for a given query with a target website and a target
+keyword: ```bash $ poetry run seo --api-key= \ -q "minecraft" \ -tk official \
+-tw minecraft.net ``` ```json [ { "engine": "google", "position": 1, "title":
+"Welcome to the Minecraft Official Site | Minecraft", "link": "https://
+www.minecraft.net/en-us" }, { "engine": "bing", "position": 1, "title":
+"Minecraft - Official Site", "link": "https://minecraft.net/" }, { "engine":
+"bing", "position": 2, "title": "Welcome to the Minecraft Official Site |
 Minecraft", "link": "https://www.minecraft.net/en-us" }, { "engine": "bing",
+"position": 10, "title": "Minecraft Official Site | Minecraft Education",
+"link": "https://education.minecraft.net/en-us" }, { "engine": "duckduckgo",
 "position": 1, "title": "Minecraft - Official Site", "link": "https://
-minecraft.net/" }, { "engine": "bing", "position": 2, "title": "Welcome to the
-Minecraft Official Site | Minecraft", "link": "https://www.minecraft.net/en-us"
-}, { "engine": "bing", "position": 10, "title": "Minecraft Official Site |
-Minecraft Education", "link": "https://education.minecraft.net/en-us" },
-{ "engine": "duckduckgo", "position": 1, "title": "Minecraft - Official Site",
-"link": "https://minecraft.net/" }, { "engine": "duckduckgo", "position": 2,
-"title": "Welcome to the Minecraft Official Site | Minecraft", "link": "https:/
-/www.minecraft.net/en-us" }, { "engine": "yahoo", "position": 1, "title":
+minecraft.net/" }, { "engine": "duckduckgo", "position": 2, "title": "Welcome
+to the Minecraft Official Site | Minecraft", "link": "https://
+www.minecraft.net/en-us" }, { "engine": "yahoo", "position": 1, "title":
 "Minecraft - Official Site", "link": "https://minecraft.net/" }, { "engine":
 "yahoo", "position": 2, "title": "Welcome to the Minecraft Official Site |
 Minecraft", "link": "https://www.minecraft.net/en-us" }, { "engine": "yandex",
 "position": 2, "title": "Welcome to the Minecraft Official Site | Minecraft",
 "link": "https://www.minecraft.net/" } ] ``` #### Extracting positions from 3
-search engines with default arguments and saving to JSON: ```bash $ python
-main.py --api-key= \ -se google bing duckduckgo \ -st JSON ``` ```json [
+search engines with default arguments and saving to JSON: ```bash $ poetry run
+seo --api-key= \ -se google bing duckduckgo \ -st JSON ``` ```json [
 { "engine": "google", "position": 6, "title": "Starbucks Coffee Company",
 "link": "https://www.starbucks.com/" }, { "engine": "bing", "position": 12,
 "title": "The Best Coffee from Starbucks Coffee: Starbucks Coffee Company",
 "link": "https://www.starbucks.com/coffee/" }, { "engine": "duckduckgo",
 "position": 11, "title": "The Best Coffee from Starbucks Coffee: Starbucks
 Coffee Company", "link": "https://www.starbucks.com/coffee/" } ] ``` ####
 Extracting positions from one engine with all arguments for it: ```bash $
-python main.py --api-key= \ -q serpapi \ -tk serpapi \ -tw https://serpapi.com/
+poetry run seo --api-key= \ -q serpapi \ -tk serpapi \ -tw https://serpapi.com/
 https://github.com/ \ -se google \ -hl de \ -gl de \ -loc Germany \ -
 d google.de \ -st TXT ``` ```json [ { "engine": "google", "position": 1,
 "title": "SerpApi: Google Search API", "link": "https://serpapi.com/" },
 { "engine": "google", "position": 3, "title": "SerpApi - GitHub", "link":
 "https://github.com/serpapi" } ] ``` #### Extracting positions from all search
 engines manually (without CLI): ```python from
 seo_position_tracker.seo_position_tracker import SeoPositionTracker import json
```

### Comparing `seo_position_tracker-1.5.0/seo_position_tracker/main.py` & `seo_position_tracker-1.5.1/seo_position_tracker/main.py`

 * *Files identical despite different names*

### Comparing `seo_position_tracker-1.5.0/seo_position_tracker/seo_position_tracker.py` & `seo_position_tracker-1.5.1/seo_position_tracker/seo_position_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,22 +261,22 @@
         
         return self.__find_positions(results, 'naver')
 
 
     def save_to_csv(self, data: list) -> None:
         keys = data[0].keys()
 
-        with open(f"{self.query.replace(' ', '_')}.csv", 'w') as csv_file:
+        with open(f"{self.query.replace(' ', '_')}.csv", 'w', encoding='utf-8') as csv_file:
             writer = csv.DictWriter(csv_file, keys)
             writer.writeheader()
             writer.writerows(data)
         
 
     def save_to_json(self, data: list) -> None:
         with open(f"{self.query.replace(' ', '_')}.json", 'w', encoding='utf-8') as json_file:
             json.dump(data, json_file, indent=2, ensure_ascii=False)
 
 
     def save_to_txt(self, data: list) -> None:
-        with open(f'{self.query.replace(" ", "_")}.txt', 'w') as txt_file:
+        with open(f'{self.query.replace(" ", "_")}.txt', 'w', encoding='utf-8') as txt_file:
             for element in data:
                 txt_file.write(f"{element.get('engine')} {element.get('position')} {element.get('title')} {element.get('link')}\n")
```

### Comparing `seo_position_tracker-1.5.0/PKG-INFO` & `seo_position_tracker-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seo-position-tracker
-Version: 1.5.0
+Version: 1.5.1
 Summary: A simple Python package for SEO position tracking from Google and other search engines.
 Home-page: https://github.com/dimitryzub/seo-position-tracker
 License: BSD-3-Clause
 Author: Dimitry Zub
 Author-email: dimitryzub@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -17,23 +17,38 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
+Requires-Dist: google-search-results (>=2.4.2,<3.0.0)
 Description-Content-Type: text/markdown
 
+<div align="center">
+<p>Sponsor of the project:</p>
+<div>
+   <img src="https://user-images.githubusercontent.com/81998012/231172985-81515e8b-bc41-46b4-83fa-d129d5f3e718.svg" width="100" alt="SerpApi">
+</div>
+<a href="https://serpapi.com">
+  <b>API to get search engine results with ease.</b>
+</a>
+</div>
+
+______
+
 <h1 align="center">SEO Position Tracker 📡</h1>
 
 <p align="center">A simple Python CLI and in-code SEO position tracking tool for Google and 6 other search engines.</p>
 <p align="center">This project uses <a href="http://serpapi.com/">SerpApi</a></p>
 
+<div align="center">
+   <img src="https://user-images.githubusercontent.com/78694043/231775565-1b007b07-e168-4b88-9518-865148e1d2a4.svg" width="700" alt="SerpApi">
+</div>
+
 
 <div align="center">
 
   <a href="https://pepy.tech/project/seo-position-tracker">![Downloads](https://static.pepy.tech/personalized-badge/seo-position-tracker?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)</a>
   <a href="">![licence](https://img.shields.io/github/license/dimitryzub/seo-position-tracker?color=blue)</a>
 
 </div>
@@ -54,36 +69,53 @@
 
 ```bash
 $ pip install seo-position-tracker
 ```
 
 Install from source:
 
+Windows:
+
 ```bash
 $ git clone https://github.com/dimitryzub/seo-position-tracking.git
-$ cd seo_position_tracker/
-$ python -m venv env && source env/bin/activate # or env/Scripts/activate for Windows
+$ cd seo-position-tracker/
+$ python -m venv env
+$ env/Scripts/activate
+$ pip install poetry
 $ poetry install
 ```
 
 If you get an error, try: 
+
 ```bash
 $ pip install chardet 
 $ poetry install
 ```
 
 
 ## 🤹‍♂️Usage
 
-#### Available CLI arugments:
+You can envoke script by this two commands. 
+
+Examples below will show usage with `poetry run seo <command>`, but you can use `python main.py <command>` instead.  
 
 ```bash
+$ cd seo_position_tracker # dive inside the module folder
 $ python main.py -h
 ```
 
+```bash
+$ poetry run seo -h
+```
+
+<details>
+<summary>
+Available arugments
+</summary>
+
 ```lang-none
 SerpApi SEO position tracker [-h] [-q] [-tk  [...]] [-tw  [...]] [-se  [...]] [-ak] [-hl] [-gl] [-loc] [-d] [-st]
 
 A simple Python CLI for SEO position tracking from Google, Baidu, Bing, DuckDuckGo, Yahoo, Yandex and Naver.
 
 optional arguments:
   -h, --help            show this help message and exit
@@ -102,23 +134,26 @@
                         countries"
   -loc , --location     Location of the search. Supported only for "google", "bing", "duckduckgo" and "yandex" engines. Default "None". Find more by Googling: "SerpApi supported    
                         <engine> locations"
   -d , --domain         Search engine domain to use. Supported only for "google", "yahoo" and "yandex" engines. Default "None". Find more by Googling: "SerpApi supported <engine>   
                         domains"
   -st , --save-to       Saves the results in the current directory in the selected format (CSV, JSON, TXT). Default CSV.
 
+
 Found a bug? Open issue: https://github.com/dimitryzub/seo-position-tracker/issues
 ```
 
+</details>
+
 ## 🤹‍♂️Examples
 
 #### Extracting positions from all search engines for a given query with a target website and a target keyword:
 
 ```bash
-$ python main.py --api-key=<your_serpapi_api_key> \
+$ poetry run seo --api-key=<your_serpapi_api_key> \
 -q "minecraft" \
 -tk official \
 -tw minecraft.net
 ```
 
 ```json
 [
@@ -178,15 +213,15 @@
   }
 ]
 ```
 
 #### Extracting positions from 3 search engines with default arguments and saving to JSON:
 
 ```bash
-$ python main.py --api-key=<your_serpapi_api_key> \
+$ poetry run seo --api-key=<your_serpapi_api_key> \
 -se google bing duckduckgo \
 -st JSON
 ```
 
 ```json
 [
   {
@@ -209,15 +244,15 @@
   }
 ]
 ```
 
 #### Extracting positions from one engine with all arguments for it:
 
 ```bash       
-$ python main.py --api-key=<your_serpapi_api_key> \
+$ poetry run seo --api-key=<your_serpapi_api_key> \
 -q serpapi \
 -tk serpapi \
 -tw https://serpapi.com/ https://github.com/ \
 -se google \
 -hl de \
 -gl de \
 -loc Germany \
```

#### html2text {}

```diff
@@ -1,93 +1,101 @@
-Metadata-Version: 2.1 Name: seo-position-tracker Version: 1.5.0 Summary: A
+Metadata-Version: 2.1 Name: seo-position-tracker Version: 1.5.1 Summary: A
 simple Python package for SEO position tracking from Google and other search
 engines. Home-page: https://github.com/dimitryzub/seo-position-tracker License:
 BSD-3-Clause Author: Dimitry Zub Author-email: dimitryzub@gmail.com Requires-
 Python: >=3.8,<4.0 Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows Classifier: Operating
 System :: POSIX :: Linux Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0) Description-Content-Type: text/markdown
+Language :: Python :: 3.9 Requires-Dist: google-search-results (>=2.4.2,<3.0.0)
+Description-Content-Type: text/markdown
+                            Sponsor of the project:
+                                   [SerpApi]
+                  API_to_get_search_engine_results_with_ease.
+______
                     ****** SEO Position Tracker ð¡ ******
   A simple Python CLI and in-code SEO position tracking tool for Google and 6
                              other search engines.
                            This project uses SerpApi
+                                   [SerpApi]
     ![Downloads](https://static.pepy.tech/personalized-badge/seo-position-
 tracker?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)
    ![licence](https://img.shields.io/github/license/dimitryzub/seo-position-
                               tracker?color=blue)
 ## ð Current search engines support - Google Search - first 100 organic
 results. - Baidu Search - first 50 organic results. - Bing Search - first 50
 organic results. - DuckDuckGo Search - up to 30 organic results. - Yahoo!
 Search - first 10 organic results. - Yandex Search - up to 15 organic results.
 - Naver Search - first 15 organic results. ## âï¸Installation ```bash $ pip
-install seo-position-tracker ``` Install from source: ```bash $ git clone
-https://github.com/dimitryzub/seo-position-tracking.git $ cd
-seo_position_tracker/ $ python -m venv env && source env/bin/activate # or env/
-Scripts/activate for Windows $ poetry install ``` If you get an error, try:
-```bash $ pip install chardet $ poetry install ``` ## ð¤¹ââï¸Usage ####
-Available CLI arugments: ```bash $ python main.py -h ``` ```lang-none SerpApi
-SEO position tracker [-h] [-q] [-tk [...]] [-tw [...]] [-se [...]] [-ak] [-hl]
-[-gl] [-loc] [-d] [-st] A simple Python CLI for SEO position tracking from
-Google, Baidu, Bing, DuckDuckGo, Yahoo, Yandex and Naver. optional arguments: -
-h, --help show this help message and exit -q , --query Search query. Default
-"coffee". -tk [ ...], --target-keywords [ ...] Target keywords to track.
-Default "['coffee']". -tw [ ...], --target-websites [ ...] Target websites to
-track. Default "['starbucks.com']". -se [ ...], --search-engine [ ...] Choosing
-a search engine to track: "google", "baidu", "bing", "duckduckgo", "yahoo",
-"yandex", "naver". You can select multiple search engines. All search engines
-are selected by default. -ak , --api-key Your SerpApi API key: https://
-serpapi.com/manage-api-key. Default is a test API key to test CLI. -hl , --lang
-Language of the search. Supported only for "google", "baidu", "yahoo" and
-"yandex" engines. Default "None". Find more by Googling: "SerpApi supported
-languages" -gl , --country Country of the search. Supported only for "google",
-"bing" and "yahoo" engines. Default "None". Find more by Googling: "SerpApi
-supported  countries" -loc , --location Location of the search. Supported only
-for "google", "bing", "duckduckgo" and "yandex" engines. Default "None". Find
-more by Googling: "SerpApi supported  locations" -d , --domain Search engine
-domain to use. Supported only for "google", "yahoo" and "yandex" engines.
-Default "None". Find more by Googling: "SerpApi supported  domains" -st , --
-save-to Saves the results in the current directory in the selected format (CSV,
-JSON, TXT). Default CSV. Found a bug? Open issue: https://github.com/
-dimitryzub/seo-position-tracker/issues ``` ## ð¤¹ââï¸Examples ####
-Extracting positions from all search engines for a given query with a target
-website and a target keyword: ```bash $ python main.py --api-key= \ -
-q "minecraft" \ -tk official \ -tw minecraft.net ``` ```json [ { "engine":
-"google", "position": 1, "title": "Welcome to the Minecraft Official Site |
+install seo-position-tracker ``` Install from source: Windows: ```bash $ git
+clone https://github.com/dimitryzub/seo-position-tracking.git $ cd seo-
+position-tracker/ $ python -m venv env $ env/Scripts/activate $ pip install
+poetry $ poetry install ``` If you get an error, try: ```bash $ pip install
+chardet $ poetry install ``` ## ð¤¹ââï¸Usage You can envoke script by
+this two commands. Examples below will show usage with `poetry run seo `, but
+you can use `python main.py ` instead. ```bash $ cd seo_position_tracker # dive
+inside the module folder $ python main.py -h ``` ```bash $ poetry run seo -
+h ```   Available arugments  ```lang-none SerpApi SEO position tracker [-h] [-
+q] [-tk [...]] [-tw [...]] [-se [...]] [-ak] [-hl] [-gl] [-loc] [-d] [-st] A
+simple Python CLI for SEO position tracking from Google, Baidu, Bing,
+DuckDuckGo, Yahoo, Yandex and Naver. optional arguments: -h, --help show this
+help message and exit -q , --query Search query. Default "coffee". -tk [ ...],
+--target-keywords [ ...] Target keywords to track. Default "['coffee']". -tw
+[ ...], --target-websites [ ...] Target websites to track. Default "
+['starbucks.com']". -se [ ...], --search-engine [ ...] Choosing a search engine
+to track: "google", "baidu", "bing", "duckduckgo", "yahoo", "yandex", "naver".
+You can select multiple search engines. All search engines are selected by
+default. -ak , --api-key Your SerpApi API key: https://serpapi.com/manage-api-
+key. Default is a test API key to test CLI. -hl , --lang Language of the
+search. Supported only for "google", "baidu", "yahoo" and "yandex" engines.
+Default "None". Find more by Googling: "SerpApi supported  languages" -gl , --
+country Country of the search. Supported only for "google", "bing" and "yahoo"
+engines. Default "None". Find more by Googling: "SerpApi supported  countries"
+-loc , --location Location of the search. Supported only for "google", "bing",
+"duckduckgo" and "yandex" engines. Default "None". Find more by Googling:
+"SerpApi supported  locations" -d , --domain Search engine domain to use.
+Supported only for "google", "yahoo" and "yandex" engines. Default "None". Find
+more by Googling: "SerpApi supported  domains" -st , --save-to Saves the
+results in the current directory in the selected format (CSV, JSON, TXT).
+Default CSV. Found a bug? Open issue: https://github.com/dimitryzub/seo-
+position-tracker/issues ```  ## ð¤¹ââï¸Examples #### Extracting positions
+from all search engines for a given query with a target website and a target
+keyword: ```bash $ poetry run seo --api-key= \ -q "minecraft" \ -tk official \
+-tw minecraft.net ``` ```json [ { "engine": "google", "position": 1, "title":
+"Welcome to the Minecraft Official Site | Minecraft", "link": "https://
+www.minecraft.net/en-us" }, { "engine": "bing", "position": 1, "title":
+"Minecraft - Official Site", "link": "https://minecraft.net/" }, { "engine":
+"bing", "position": 2, "title": "Welcome to the Minecraft Official Site |
 Minecraft", "link": "https://www.minecraft.net/en-us" }, { "engine": "bing",
+"position": 10, "title": "Minecraft Official Site | Minecraft Education",
+"link": "https://education.minecraft.net/en-us" }, { "engine": "duckduckgo",
 "position": 1, "title": "Minecraft - Official Site", "link": "https://
-minecraft.net/" }, { "engine": "bing", "position": 2, "title": "Welcome to the
-Minecraft Official Site | Minecraft", "link": "https://www.minecraft.net/en-us"
-}, { "engine": "bing", "position": 10, "title": "Minecraft Official Site |
-Minecraft Education", "link": "https://education.minecraft.net/en-us" },
-{ "engine": "duckduckgo", "position": 1, "title": "Minecraft - Official Site",
-"link": "https://minecraft.net/" }, { "engine": "duckduckgo", "position": 2,
-"title": "Welcome to the Minecraft Official Site | Minecraft", "link": "https:/
-/www.minecraft.net/en-us" }, { "engine": "yahoo", "position": 1, "title":
+minecraft.net/" }, { "engine": "duckduckgo", "position": 2, "title": "Welcome
+to the Minecraft Official Site | Minecraft", "link": "https://
+www.minecraft.net/en-us" }, { "engine": "yahoo", "position": 1, "title":
 "Minecraft - Official Site", "link": "https://minecraft.net/" }, { "engine":
 "yahoo", "position": 2, "title": "Welcome to the Minecraft Official Site |
 Minecraft", "link": "https://www.minecraft.net/en-us" }, { "engine": "yandex",
 "position": 2, "title": "Welcome to the Minecraft Official Site | Minecraft",
 "link": "https://www.minecraft.net/" } ] ``` #### Extracting positions from 3
-search engines with default arguments and saving to JSON: ```bash $ python
-main.py --api-key= \ -se google bing duckduckgo \ -st JSON ``` ```json [
+search engines with default arguments and saving to JSON: ```bash $ poetry run
+seo --api-key= \ -se google bing duckduckgo \ -st JSON ``` ```json [
 { "engine": "google", "position": 6, "title": "Starbucks Coffee Company",
 "link": "https://www.starbucks.com/" }, { "engine": "bing", "position": 12,
 "title": "The Best Coffee from Starbucks Coffee: Starbucks Coffee Company",
 "link": "https://www.starbucks.com/coffee/" }, { "engine": "duckduckgo",
 "position": 11, "title": "The Best Coffee from Starbucks Coffee: Starbucks
 Coffee Company", "link": "https://www.starbucks.com/coffee/" } ] ``` ####
 Extracting positions from one engine with all arguments for it: ```bash $
-python main.py --api-key= \ -q serpapi \ -tk serpapi \ -tw https://serpapi.com/
+poetry run seo --api-key= \ -q serpapi \ -tk serpapi \ -tw https://serpapi.com/
 https://github.com/ \ -se google \ -hl de \ -gl de \ -loc Germany \ -
 d google.de \ -st TXT ``` ```json [ { "engine": "google", "position": 1,
 "title": "SerpApi: Google Search API", "link": "https://serpapi.com/" },
 { "engine": "google", "position": 3, "title": "SerpApi - GitHub", "link":
 "https://github.com/serpapi" } ] ``` #### Extracting positions from all search
 engines manually (without CLI): ```python from
 seo_position_tracker.seo_position_tracker import SeoPositionTracker import json
```

