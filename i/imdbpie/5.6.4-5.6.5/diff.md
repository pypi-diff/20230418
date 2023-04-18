# Comparing `tmp/imdbpie-5.6.4.tar.gz` & `tmp/imdbpie-5.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imdbpie-5.6.4.tar", last modified: Fri May 10 08:23:24 2019, max compression
+gzip compressed data, was "dist/imdbpie-5.6.5.tar", last modified: Tue Apr 18 19:44:32 2023, max compression
```

## Comparing `imdbpie-5.6.4.tar` & `imdbpie-5.6.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2019-05-10 08:23:24.000000 imdbpie-5.6.4/
--rw-rw-r--   0 richard   (1001) richard   (1001)     6376 2019-05-10 08:23:24.000000 imdbpie-5.6.4/HISTORY.rst
--rw-rw-r--   0 richard   (1001) richard   (1001)      208 2019-05-10 08:23:24.000000 imdbpie-5.6.4/MANIFEST.in
--rw-rw-r--   0 richard   (1001) richard   (1001)    11325 2019-05-10 08:23:24.000000 imdbpie-5.6.4/PKG-INFO
--rw-rw-r--   0 richard   (1001) richard   (1001)     1645 2019-05-10 08:23:24.000000 imdbpie-5.6.4/README.rst
--rw-rw-r--   0 richard   (1001) richard   (1001)      182 2019-05-10 08:23:24.000000 imdbpie-5.6.4/requirements.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)      238 2019-05-10 08:23:24.000000 imdbpie-5.6.4/setup.cfg
--rw-rw-r--   0 richard   (1001) richard   (1001)     1695 2019-05-10 08:23:24.000000 imdbpie-5.6.4/setup.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie/
--rw-rw-r--   0 richard   (1001) richard   (1001)      142 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie/__init__.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     4607 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie/auth.py
--rw-rw-r--   0 richard   (1001) richard   (1001)      292 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie/constants.py
--rw-rw-r--   0 richard   (1001) richard   (1001)       64 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie/exceptions.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     7716 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie/facade.py
--rw-rw-r--   0 richard   (1001) richard   (1001)    12862 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie/imdbpie.py
--rw-rw-r--   0 richard   (1001) richard   (1001)     2292 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie/objects.py
-drwxrwxr-x   0 richard   (1001) richard   (1001)        0 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie.egg-info/
--rw-rw-r--   0 richard   (1001) richard   (1001)    11325 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1001) richard   (1001)      441 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)        1 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)        1 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie.egg-info/not-zip-safe
--rw-rw-r--   0 richard   (1001) richard   (1001)      182 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie.egg-info/requires.txt
--rw-rw-r--   0 richard   (1001) richard   (1001)        8 2019-05-10 08:23:24.000000 imdbpie-5.6.4/src/imdbpie.egg-info/top_level.txt
+drwxrwxr-x   0 amnesia   (1000) amnesia   (1000)        0 2023-04-18 19:44:32.583245 imdbpie-5.6.5/
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)     6471 2023-04-18 19:44:32.000000 imdbpie-5.6.5/HISTORY.rst
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)      583 2023-04-18 19:44:32.000000 imdbpie-5.6.5/LICENSE
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)      208 2023-04-18 19:44:32.000000 imdbpie-5.6.5/MANIFEST.in
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)     8491 2023-04-18 19:44:32.583245 imdbpie-5.6.5/PKG-INFO
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)     1441 2023-04-18 19:44:32.000000 imdbpie-5.6.5/README.rst
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)      182 2023-04-18 19:44:32.000000 imdbpie-5.6.5/requirements.txt
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)      337 2023-04-18 19:44:32.587245 imdbpie-5.6.5/setup.cfg
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)     1400 2023-04-18 19:44:32.000000 imdbpie-5.6.5/setup.py
+drwxrwxr-x   0 amnesia   (1000) amnesia   (1000)        0 2023-04-18 19:44:32.579245 imdbpie-5.6.5/src/
+drwxrwxr-x   0 amnesia   (1000) amnesia   (1000)        0 2023-04-18 19:44:32.583245 imdbpie-5.6.5/src/imdbpie/
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)      142 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie/__init__.py
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)     4732 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie/auth.py
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)      292 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie/constants.py
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)       64 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie/exceptions.py
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)     8103 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie/facade.py
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)    12785 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie/imdbpie.py
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)     2269 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie/objects.py
+drwxrwxr-x   0 amnesia   (1000) amnesia   (1000)        0 2023-04-18 19:44:32.583245 imdbpie-5.6.5/src/imdbpie.egg-info/
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)     8491 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie.egg-info/PKG-INFO
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)      449 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie.egg-info/SOURCES.txt
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)        1 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie.egg-info/dependency_links.txt
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)        1 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie.egg-info/not-zip-safe
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)      182 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie.egg-info/requires.txt
+-rw-rw-r--   0 amnesia   (1000) amnesia   (1000)        8 2023-04-18 19:44:32.000000 imdbpie-5.6.5/src/imdbpie.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `imdbpie-5.6.4/HISTORY.rst` & `imdbpie-5.6.5/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 .. :changelog:
 
 Release History
 ---------------
 
-5.6.4 (2019-05-10)
+5.6.5 (2023-04-18)
 ++++++++++++++++++
 
-- Bugfix for Unicode chars getting stripped on search.
+- Packaging fixes.
+
+
+5.6.4 (2023-04-18)
+++++++++++++++++++
+
+- Fix for JSON parsing from the API.
+- Fix for ``title_exists`` method raising 403 error.
 
 
 5.6.3 (2018-10-13)
 ++++++++++++++++++
 
 - Bugfix for handing of national characters within search methods.
```

### Comparing `imdbpie-5.6.4/README.rst` & `imdbpie-5.6.5/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 ImdbPie
 =======
 
 |PyPI| |Python Versions| |Build Status|
 
 Python IMDB client using the IMDB JSON web service made available for their iOS application.
 
-NOTICE: If you're reading this on Github.com please be aware this is a mirror of the primary remote located at https://code.richard.do/explore/projects.
-Please direct any issues or pull requests Gitlab.
-
 API Terminology
 ---------------
 
 -  ``Title`` this can be a movie, tv show, video, documentary etc.
 -  ``Name`` this can be a credit, cast member, any person generally.
 
 Installation
```

### Comparing `imdbpie-5.6.4/setup.py` & `imdbpie-5.6.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,37 +18,31 @@
     readme = rm_file.read()
 
 with open('HISTORY.rst', 'r', encoding='utf-8') as hist_file:
     history = hist_file.read()
 
 setup(
     name='imdbpie',
-    version='5.6.4',
+    version='5.6.5',
     packages=find_packages('src', exclude=('tests',)),
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     description=(
         'Python IMDB client using the IMDB json web service made '
         'available for their iOS app.'
     ),
-    author='Richard O\'Dwyer',
+    author="Richard O'Dwyer",
     author_email='richard@richard.do',
     url='https://code.richard.do/richardARPANET/imdb-pie/',
     license='Apache 2.0',
     long_description=readme + '\n\n' + history,
     install_requires=install_requires,
     classifiers=[
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.2',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
         'Topic :: Internet :: WWW/HTTP',
     ],
 )
```

### Comparing `imdbpie-5.6.4/src/imdbpie/auth.py` & `imdbpie-5.6.5/src/imdbpie/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import, unicode_literals
 
 import json
 import requests
 import tempfile
 from datetime import datetime
+
 try:
     from base64 import encodebytes
 except ImportError:
     from base64 import encodestring as encodebytes
 
 import diskcache
 from dateutil.tz import tzutc
@@ -19,15 +20,14 @@
 from boto.connection import HTTPRequest
 from boto.auth import HmacAuthV3HTTPHandler
 
 from .constants import APP_KEY, HOST, USER_AGENT, BASE_URI
 
 
 class ZuluHmacAuthV3HTTPHandler(HmacAuthV3HTTPHandler):
-
     def sign_string(self, string_to_sign):
         new_hmac = self._get_hmac()
         new_hmac.update(string_to_sign)
         return encodebytes(new_hmac.digest()).decode('utf-8').strip()
 
     def headers_to_sign(self, http_request):
         headers_to_sign = {'Host': self.host}
@@ -48,22 +48,24 @@
             qs_parts.append('{0}={1}'.format(param_, value_))
         return '&'.join(qs_parts)
 
     def string_to_sign(self, http_request):
         headers_to_sign = self.headers_to_sign(http_request)
         canonical_qs = self.canonical_query_string(http_request)
         canonical_headers = self.canonical_headers(headers_to_sign)
-        string_to_sign = '\n'.join((
-            http_request.method,
-            http_request.path,
-            canonical_qs,
-            canonical_headers,
-            '',
-            http_request.body
-        ))
+        string_to_sign = '\n'.join(
+            (
+                http_request.method,
+                http_request.path,
+                canonical_qs,
+                canonical_headers,
+                '',
+                http_request.body,
+            )
+        )
         return string_to_sign, headers_to_sign
 
 
 def _get_credentials():
     url = '{0}/authentication/credentials/temporary/ios82'.format(BASE_URI)
     response = requests.post(
         url, json={'appKey': APP_KEY}, headers={'User-Agent': USER_AGENT}
@@ -117,22 +119,28 @@
             host=HOST,
             config={},
             provider=provider.Provider(
                 name='aws',
                 access_key=creds['accessKeyId'],
                 secret_key=creds['secretAccessKey'],
                 security_token=creds['sessionToken'],
-            )
+            ),
         )
         parsed_url = urlparse(url_path)
         params = {
             key: val[0] for key, val in parse_qs(parsed_url.query).items()
         }
         request = HTTPRequest(
-            method='GET', protocol='https', host=HOST,
-            port=443, path=parsed_url.path, auth_path=None, params=params,
-            headers={}, body=''
+            method='GET',
+            protocol='https',
+            host=HOST,
+            port=443,
+            path=parsed_url.path,
+            auth_path=None,
+            params=params,
+            headers={},
+            body='',
         )
         handler.add_auth(req=request)
         headers = request.headers
         headers['User-Agent'] = USER_AGENT
         return headers
```

### Comparing `imdbpie-5.6.4/src/imdbpie/facade.py` & `imdbpie-5.6.5/src/imdbpie/facade.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 
 import re
 
 from dateutil.parser import parse
 
 from .imdbpie import Imdb
 from .objects import (
-    Title, TitleEpisodes, Name, TitleName, Image, TitleRelease,
-    TitleSearchResult, NameSearchResult,
+    Title,
+    TitleEpisodes,
+    Name,
+    TitleName,
+    Image,
+    TitleRelease,
+    TitleSearchResult,
+    NameSearchResult,
 )
 
 REGEX_IMDB_ID = re.compile(r'([a-zA-Z]{2}[0-9]{7})')
 
 
 class ImdbFacade(object):
-
     def __init__(self, client=None):
         self._client = client or Imdb()
 
     def get_title(self, imdb_id):
         title_data, title_aux_data = self._get_title_data(imdb_id=imdb_id)
         try:
             runtime = title_aux_data['runningTimes'][0]['timeMinutes']
@@ -32,16 +37,19 @@
         try:
             season = title_aux_data['season']
             episode = title_aux_data['episode']
         except KeyError:
             season = None
             episode = None
         return Title(
-            season=season, episode=episode, episodes=episodes,
-            runtime=runtime, **title_data
+            season=season,
+            episode=episode,
+            episodes=episodes,
+            runtime=runtime,
+            **title_data
         )
 
     def get_name(self, imdb_id):
         name_data = self._client.get_name(imdb_id=imdb_id)
         name = name_data['base']['name']
         imdb_id = self._parse_id(name_data['base']['id'])
 
@@ -64,94 +72,108 @@
             bios = ()
 
         filmography_data = self._client.get_name_filmography(imdb_id)
         filmography = tuple(
             self._parse_id(f['id']) for f in filmography_data['filmography']
         )
         return Name(
-            name=name, imdb_id=imdb_id, date_of_birth=date_of_birth,
-            gender=gender, birth_place=birth_place, bios=bios, image=image,
+            name=name,
+            imdb_id=imdb_id,
+            date_of_birth=date_of_birth,
+            gender=gender,
+            birth_place=birth_place,
+            bios=bios,
+            image=image,
             filmography=filmography,
         )
 
     def search_for_name(self, query):
         results = []
         for result in self._client.search_for_name(query):
             result = NameSearchResult(
-                imdb_id=result['imdb_id'], name=result['name'],
+                imdb_id=result['imdb_id'],
+                name=result['name'],
             )
             results.append(result)
         return tuple(results)
 
     def search_for_title(self, query):
         results = []
         for result in self._client.search_for_title(query):
             if result['year']:
                 year = int(result['year'])
             else:
                 year = None
             result = TitleSearchResult(
-                imdb_id=result['imdb_id'], title=result['title'],
-                type=result['type'], year=year,
+                imdb_id=result['imdb_id'],
+                title=result['title'],
+                type=result['type'],
+                year=year,
             )
             results.append(result)
         return tuple(results)
 
     def _get_writers(self, top_crew_data):
         return tuple(
             TitleName(
                 name=i['name'],
                 job=i.get('job'),
                 category=i.get('category'),
-                imdb_id=self._parse_id(i['id'])
-            ) for i in top_crew_data['writers']
+                imdb_id=self._parse_id(i['id']),
+            )
+            for i in top_crew_data['writers']
         )
 
     def _get_stars(self, principals_data):
         return tuple(
             TitleName(
                 name=i['name'],
                 job=i.get('job'),
                 characters=tuple(i.get('characters', ())),
                 category=i.get('category'),
-                imdb_id=self._parse_id(i['id'])
-            ) for i in principals_data
+                imdb_id=self._parse_id(i['id']),
+            )
+            for i in principals_data
         )
 
     def _get_creators(self, top_crew_data):
         return tuple(
             TitleName(
                 name=i['name'],
                 job=i.get('job'),
                 category=i.get('category'),
-                imdb_id=self._parse_id(i['id'])
-            ) for i in top_crew_data['writers']
+                imdb_id=self._parse_id(i['id']),
+            )
+            for i in top_crew_data['writers']
             if i.get('job') == 'creator'
         )
 
     def _get_directors(self, top_crew_data):
         return tuple(
             TitleName(
                 name=i['name'],
                 job=i.get('job'),
                 category=i.get('category'),
-                imdb_id=self._parse_id(i['id'])
-            ) for i in top_crew_data['directors']
+                imdb_id=self._parse_id(i['id']),
+            )
+            for i in top_crew_data['directors']
         )
 
     def _get_credits(self, credits_data):
         credits = []
         for category in credits_data.get('credits', ()):
             for item in credits_data['credits'][category]:
-                credits.append(TitleName(
-                    name=item['name'],
-                    category=item.get('category'),
-                    job=item.get('job'),
-                    imdb_id=self._parse_id(item['id'])
-                ))
+                credits.append(
+                    TitleName(
+                        name=item['name'],
+                        category=item.get('category'),
+                        job=item.get('job'),
+                        imdb_id=self._parse_id(item['id']),
+                    )
+                )
         return tuple(credits)
 
     def _parse_id(self, string):
         return REGEX_IMDB_ID.findall(string)[0]
 
     def _get_title_data(self, imdb_id):
         base_title_data = self._client.get_title(imdb_id=imdb_id)
@@ -208,26 +230,29 @@
             image = Image(
                 url=image_data['url'],
                 height=image_data['height'],
                 width=image_data['width'],
             )
         except KeyError:
             image = None
-        return dict(
-            imdb_id=imdb_id,
-            title=title,
-            year=year,
-            rating=rating,
-            type=type_,
-            release_date=release_date,
-            releases=releases,
-            plot_outline=plot_outline,
-            rating_count=rating_count,
-            writers=writers,
-            directors=directors,
-            creators=creators,
-            genres=genres,
-            credits=credits,
-            certification=certification,
-            image=image,
-            stars=stars,
-        ), title_aux_data
+        return (
+            dict(
+                imdb_id=imdb_id,
+                title=title,
+                year=year,
+                rating=rating,
+                type=type_,
+                release_date=release_date,
+                releases=releases,
+                plot_outline=plot_outline,
+                rating_count=rating_count,
+                writers=writers,
+                directors=directors,
+                creators=creators,
+                genres=genres,
+                credits=credits,
+                certification=certification,
+                image=image,
+                stars=stars,
+            ),
+            title_aux_data,
+        )
```

### Comparing `imdbpie-5.6.4/src/imdbpie/imdbpie.py` & `imdbpie-5.6.5/src/imdbpie/imdbpie.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import tempfile
 import logging
 
 from trans import trans
 import requests
 from six import text_type
 from six.moves import http_client as httplib
-from six.moves.urllib.parse import urlencode, urljoin, quote, unquote
+from six.moves.urllib.parse import urlencode, urljoin, quote
 
 from .constants import BASE_URI, SEARCH_BASE_URI
 from .auth import Auth
 from .exceptions import ImdbAPIError
 
 logger = logging.getLogger(__name__)
 
@@ -48,15 +48,14 @@
     'get_title_credits': '/title/{imdb_id}/fullcredits',
     'get_name': '/name/{imdb_id}/fulldetails',
     'get_name_filmography': '/name/{imdb_id}/filmography',
 }
 
 
 class Imdb(Auth):
-
     def __init__(self, locale=None, exclude_episodes=False, session=None):
         self.locale = locale or 'en_US'
         self.region = self.locale.split('_')[-1].upper()
         self.exclude_episodes = exclude_episodes
         self.session = session or requests.Session()
         self._cachedir = tempfile.gettempdir()
 
@@ -80,16 +79,16 @@
             resource = self._get_resource(
                 '/title/{0}/auxiliary'.format(imdb_id)
             )
         except LookupError:
             self._title_not_found()
 
         if (
-            self.exclude_episodes is True and
-            resource['base']['titleType'] == 'tvEpisode'
+            self.exclude_episodes is True
+            and resource['base']['titleType'] == 'tvEpisode'
         ):
             raise LookupError(
                 'Title not found. Title was an episode and '
                 '"exclude_episodes" is set to true'
             )
         return resource
 
@@ -104,44 +103,49 @@
                 params={
                     'inlineBannerAdWeblabOn': 'false',
                     'minwidth': '320',
                     'osVersion': '11.3.0',
                     'region': self.region,
                     'tconst': imdb_id,
                     'today': date.today().strftime('%Y-%m-%d'),
-                }
+                },
             )
         except LookupError:
             self._title_not_found()
 
         if (
-            self.exclude_episodes is True and
-            resource['titleType'].lower() == 'tvepisode'
+            self.exclude_episodes is True
+            and resource['titleType'].lower() == 'tvepisode'
         ):
             raise LookupError(
                 'Title not found. Title was an episode and '
                 '"exclude_episodes" is set to true'
             )
         return resource
 
     def _simple_get_method(self, method, path):
         """Return client method generated from ``_SIMPLE_GET_ENDPOINTS``."""
+
         def get(imdb_id):
             logger.info('called %s %s', method, imdb_id)
             self.validate_imdb_id(imdb_id)
             self._redirection_title_check(imdb_id)
             return self._get_resource(path.format(imdb_id=imdb_id))
+
         return get
 
     def title_exists(self, imdb_id):
         self.validate_imdb_id(imdb_id)
         page_url = 'https://www.imdb.com/title/{0}/'.format(imdb_id)
 
-        response = self.session.get(page_url, allow_redirects=False)
-
+        response = self.session.get(
+            page_url,
+            allow_redirects=False,
+            headers={'User-Agent': 'Mozilla/5.0'},
+        )
         if response.status_code == httplib.OK:
             return True
         elif response.status_code == httplib.NOT_FOUND:
             return False
         elif response.status_code == httplib.MOVED_PERMANENTLY:
             # redirection result
             return False
@@ -158,15 +162,15 @@
         )
         url = urljoin(SEARCH_BASE_URI, path)
         search_results = self._get(url=url, query=query_encoded)
         return search_results
 
     def search_for_name(self, name):
         logger.info('called search_for_name %s', name)
-        name = re.sub(r'\W+', '_', name, flags=re.UNICODE).strip('_')
+        name = re.sub(r'\W+', '+', name).strip('+')
         search_results = self._suggest_search(name)
         results = []
         for result in search_results.get('d', ()):
             if not result['id'].startswith('nm'):
                 # ignore non-person results
                 continue
             result_item = {
@@ -174,15 +178,15 @@
                 'imdb_id': result['id'],
             }
             results.append(result_item)
         return results
 
     def search_for_title(self, title):
         logger.info('called search_for_title %s', title)
-        title = re.sub(r'\W+', '_', title, flags=re.UNICODE).strip('_')
+        title = re.sub(r'\W+', '+', title).strip('+')
         search_results = self._suggest_search(title)
         results = []
         for result in search_results.get('d', ()):
             if not result['id'].startswith('tt'):
                 # ignore non-title results
                 continue
             result_item = {
@@ -231,46 +235,47 @@
             'start': offset,
             'season': season - 1,  # api seasons are zero indexed
             'tconst': imdb_id,
         }
         if region:
             params.update({'region': region})
 
-        return self._get(urljoin(
-            BASE_URI, '/template/imdb-ios-writable/tv-episodes-v2.jstl/render'
-        ), params=params)
+        return self._get(
+            urljoin(
+                BASE_URI,
+                '/template/imdb-ios-writable/tv-episodes-v2.jstl/render',
+            ),
+            params=params,
+        )
 
     def get_title_top_crew(self, imdb_id):
         """
         Request detailed information about title's top crew
         (ie: directors, writters, etc.).
 
         :param imdb_id: The imdb id including the TT prefix.
         """
         logger.info('called get_title_top_crew %s', imdb_id)
         self.validate_imdb_id(imdb_id)
         params = {'tconst': imdb_id}
-        return self._get(urljoin(
-            BASE_URI,
-            '/template/imdb-android-writable/7.3.top-crew.jstl/render'
-        ), params=params)
+        return self._get(
+            urljoin(
+                BASE_URI,
+                '/template/imdb-android-writable/7.3.top-crew.jstl/render',
+            ),
+            params=params,
+        )
 
     @staticmethod
     def _parse_dirty_json(data, query=None):
         if query is None:
             match_json_within_dirty_json = r'imdb\$.+\({1}(.+)\){1}'
         else:
-            query_match = ''.join(
-                char if char.isalnum() else '[{0}]'.format(char)
-                for char in unquote(query)
-            )
-            query_match = query_match.replace('[ ]', '.+')
-            match_json_within_dirty_json = (
-                r'imdb\${}\((.+)\)'.format(query_match)
-            )
+            # No need to unquote as the json is containing quoted query
+            match_json_within_dirty_json = r'imdb\${}\((.+)\)'.format(query)
         data_clean = re.match(
             match_json_within_dirty_json, data, re.IGNORECASE
         ).groups()[0]
         return json.loads(data_clean)
 
     @staticmethod
     def validate_imdb_id(imdb_id):
@@ -283,17 +288,16 @@
     @staticmethod
     def _is_redirection_result(response):
         """
         Return True if response is that of a redirection else False
         Redirection results have no information of use.
         """
         imdb_id = response['data'].get('tconst')
-        if (
-            imdb_id and
-            imdb_id != response['data'].get('news', {}).get('channel')
+        if imdb_id and imdb_id != response['data'].get('news', {}).get(
+            'channel'
         ):
             return True
         return False
 
     def _get_resource(self, path):
         url = urljoin(BASE_URI, path)
         return self._get(url=url)['resource']
@@ -302,28 +306,25 @@
         headers = {'Accept-Language': self.locale}
         if params:
             full_url = '{0}?{1}'.format(url, urlencode(params))
         else:
             full_url = url
         headers.update(self.get_auth_headers(full_url))
         resp = self.session.get(url, headers=headers, params=params)
-
         if not resp.ok:
             if resp.status_code == httplib.NOT_FOUND:
                 raise LookupError('Resource {0} not found'.format(url))
             else:
                 msg = '{0} {1}'.format(resp.status_code, resp.text)
                 raise ImdbAPIError(msg)
         resp_data = resp.content.decode('utf-8')
         try:
             resp_dict = json.loads(resp_data)
         except ValueError:
-            resp_dict = self._parse_dirty_json(
-                data=resp_data, query=query
-            )
+            resp_dict = self._parse_dirty_json(data=resp_data, query=query)
 
         if resp_dict.get('error'):
             return None
         return resp_dict
 
     def _redirection_title_check(self, imdb_id):
         if self.is_redirection_title(imdb_id):
```

### Comparing `imdbpie-5.6.4/src/imdbpie/objects.py` & `imdbpie-5.6.5/src/imdbpie/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,17 @@
 class Image(object):
     url = attr.ib()
     width = attr.ib()
     height = attr.ib()
 
 
 class TitleEpisodes(object):
-
     def __init__(self, facade, imdb_id):
         self._facade = facade
-        episodes = self._facade._client.get_title_episodes(
-            imdb_id=imdb_id
-        )
+        episodes = self._facade._client.get_title_episodes(imdb_id=imdb_id)
         self._episode_imdb_ids = []
         for season in episodes['seasons']:
             for episode in season['episodes']:
                 imdb_id = self._facade._parse_id(episode['id'])
                 self._episode_imdb_ids.append(imdb_id)
         self._count = len(self._episode_imdb_ids)
```

