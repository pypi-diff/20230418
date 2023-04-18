# Comparing `tmp/pinscrape-2.0.0.tar.gz` & `tmp/pinscrape-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinscrape-2.0.0.tar", last modified: Tue Nov 15 17:21:27 2022, max compression
+gzip compressed data, was "pinscrape-2.0.1.tar", last modified: Tue Apr 18 07:26:25 2023, max compression
```

## Comparing `pinscrape-2.0.0.tar` & `pinscrape-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-11-15 17:21:27.661308 pinscrape-2.0.0/
--rw-rw-rw-   0        0        0     1099 2022-11-15 17:17:03.000000 pinscrape-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     1508 2022-11-15 17:21:27.660210 pinscrape-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2022-11-15 17:17:03.000000 pinscrape-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-15 17:21:27.635117 pinscrape-2.0.0/pinscrape/
--rw-rw-rw-   0        0        0      235 2022-11-15 17:17:03.000000 pinscrape-2.0.0/pinscrape/__init__.py
--rw-rw-rw-   0        0        0       23 2022-11-15 17:18:46.000000 pinscrape-2.0.0/pinscrape/_version.py
--rw-rw-rw-   0        0        0     6288 2022-11-15 17:17:03.000000 pinscrape-2.0.0/pinscrape/pinscrape.py
-drwxrwxrwx   0        0        0        0 2022-11-15 17:21:27.658203 pinscrape-2.0.0/pinscrape.egg-info/
--rw-rw-rw-   0        0        0     1508 2022-11-15 17:21:27.000000 pinscrape-2.0.0/pinscrape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2022-11-15 17:21:27.000000 pinscrape-2.0.0/pinscrape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-15 17:21:27.000000 pinscrape-2.0.0/pinscrape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2022-11-15 17:21:27.000000 pinscrape-2.0.0/pinscrape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-11-15 17:21:27.000000 pinscrape-2.0.0/pinscrape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-15 17:21:27.661308 pinscrape-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      840 2022-11-15 17:17:03.000000 pinscrape-2.0.0/setup.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-04-18 07:26:25.574910 pinscrape-2.0.1/
+-rw-r--r--   0 atul       (501) staff       (20)     1078 2023-04-18 07:24:22.000000 pinscrape-2.0.1/LICENSE
+-rw-r--r--   0 atul       (501) staff       (20)     1469 2023-04-18 07:26:25.574798 pinscrape-2.0.1/PKG-INFO
+-rw-r--r--   0 atul       (501) staff       (20)     1042 2023-04-18 07:24:22.000000 pinscrape-2.0.1/README.md
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-04-18 07:26:25.574066 pinscrape-2.0.1/pinscrape/
+-rw-r--r--   0 atul       (501) staff       (20)      226 2023-04-18 07:24:22.000000 pinscrape-2.0.1/pinscrape/__init__.py
+-rw-r--r--   0 atul       (501) staff       (20)       22 2023-04-18 07:26:14.000000 pinscrape-2.0.1/pinscrape/_version.py
+-rw-r--r--   0 atul       (501) staff       (20)     6130 2023-04-18 07:24:22.000000 pinscrape-2.0.1/pinscrape/pinscrape.py
+drwxr-xr-x   0 atul       (501) staff       (20)        0 2023-04-18 07:26:25.574636 pinscrape-2.0.1/pinscrape.egg-info/
+-rw-r--r--   0 atul       (501) staff       (20)     1469 2023-04-18 07:26:25.000000 pinscrape-2.0.1/pinscrape.egg-info/PKG-INFO
+-rw-r--r--   0 atul       (501) staff       (20)      257 2023-04-18 07:26:25.000000 pinscrape-2.0.1/pinscrape.egg-info/SOURCES.txt
+-rw-r--r--   0 atul       (501) staff       (20)        1 2023-04-18 07:26:25.000000 pinscrape-2.0.1/pinscrape.egg-info/dependency_links.txt
+-rw-r--r--   0 atul       (501) staff       (20)       76 2023-04-18 07:26:25.000000 pinscrape-2.0.1/pinscrape.egg-info/requires.txt
+-rw-r--r--   0 atul       (501) staff       (20)       10 2023-04-18 07:26:25.000000 pinscrape-2.0.1/pinscrape.egg-info/top_level.txt
+-rw-r--r--   0 atul       (501) staff       (20)       38 2023-04-18 07:26:25.574945 pinscrape-2.0.1/setup.cfg
+-rw-r--r--   0 atul       (501) staff       (20)      813 2023-04-18 07:24:22.000000 pinscrape-2.0.1/setup.py
```

### Comparing `pinscrape-2.0.0/LICENSE` & `pinscrape-2.0.1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021-2022 Atul Kumar Singh
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021-2022 Atul Kumar Singh
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pinscrape-2.0.0/README.md` & `pinscrape-2.0.1/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# pinscrape
-[![built with Python3](https://img.shields.io/badge/built%20with-Python3.6+-red.svg)](https://www.python.org/)
-
-### This package can be use to scrape images from pinterest just by using any search keywords. Install it just by using <br><br>
-`pip install pinscrape`
-### How to use?
-```python
-from pinscrape import pinscrape
-details = pinscrape.scraper.scrape("messi", "output", {}, 10, 15)
-
-if details["isDownloaded"]:
-    print("\nDownloading completed !!")
-    print(f"\nTotal urls found: {len(details['extracted_urls'])}")
-    print(f"\nTotal images downloaded (including duplicate images): {len(details['url_list'])}")
-    print(details)
-else:
-    print("\nNothing to download !!")
-```
-
-`scrape("messi", "output", {}, 10)` <br/>
-- `"messi"` is keyword
-- `"output"` is path to a folder where you want to save images
-- `{}` is proxy list if you want to add one (optional)
-- `10` is a number of threads you want to use for downloading those images (optional)
-- `15` is the maximum number of images you want to download (optional)
+# pinscrape
+[![built with Python3](https://img.shields.io/badge/built%20with-Python3.6+-red.svg)](https://www.python.org/)
+
+### This package can be use to scrape images from pinterest just by using any search keywords. Install it just by using <br><br>
+`pip install pinscrape`
+### How to use?
+```python
+from pinscrape import pinscrape
+details = pinscrape.scraper.scrape("messi", "output", {}, 10, 15)
+
+if details["isDownloaded"]:
+    print("\nDownloading completed !!")
+    print(f"\nTotal urls found: {len(details['extracted_urls'])}")
+    print(f"\nTotal images downloaded (including duplicate images): {len(details['url_list'])}")
+    print(details)
+else:
+    print("\nNothing to download !!")
+```
+
+`scrape("messi", "output", {}, 10)` <br/>
+- `"messi"` is keyword
+- `"output"` is path to a folder where you want to save images
+- `{}` is proxy list if you want to add one (optional)
+- `10` is a number of threads you want to use for downloading those images (optional)
+- `15` is the maximum number of images you want to download (optional)
```

### Comparing `pinscrape-2.0.0/pinscrape/pinscrape.py` & `pinscrape-2.0.1/pinscrape/pinscrape.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-import re
-import json
-import os
-import cv2
-import numpy as np
-
-from requests import get
-from bs4 import BeautifulSoup as soup
-from concurrent.futures import ThreadPoolExecutor
-
-from pydotmap import DotMap
-
-
-class PinterestImageScraper:
-
-    def __init__(self):
-        self.json_data_list = []
-        self.unique_img = []
-
-    # ---------------------------------------- GET GOOGLE RESULTS ---------------------------------
-    @staticmethod
-    def get_pinterest_links(body, max_images):
-        searched_urls = []
-        html = soup(body, 'html.parser')
-        links = html.select('#main > div > div > div > a')
-        for link in links:
-            link = link.get('href')
-            link = re.sub(r'/url\?q=', '', link)
-            if link[0] != "/" and "pinterest" in link:
-                searched_urls.append(link)
-                #stops adding links if the limit has been reached
-                if max_images is not None and max_images == len(searched_urls):
-                    break
-
-        return searched_urls
-
-    # -------------------------- save json data from source code of given pinterest url -------------
-    def get_source(self, url, proxies):
-        try:
-            res = get(url, proxies=proxies)
-        except Exception as e:
-            return
-        html = soup(res.text, 'html.parser')
-        json_data = html.find_all("script", attrs={"id": "__PWS_DATA__"})
-        for a in json_data:
-            self.json_data_list.append(a.string)
-
-    # --------------------------- READ JSON OF PINTEREST WEBSITE ----------------------
-    def save_image_url(self, max_images):
-        url_list = [i for i in self.json_data_list if i.strip()]
-        if not len(url_list):
-            return url_list
-        url_list = []
-        for js in self.json_data_list:
-            try:
-                data = DotMap(json.loads(js))
-                urls = []
-                for pin in data.props.initialReduxState.pins:
-                    if isinstance(data.props.initialReduxState.pins[pin].images.get("orig"), list):
-                        for i in data.props.initialReduxState.pins[pin].images.get("orig"):
-                            urls.append(i.get("url"))
-                    else:
-                        urls.append(data.props.initialReduxState.pins[pin].images.get("orig").get("url"))
-
-                for url in urls:
-                    url_list.append(url)
-
-                    #if the maximum has been achieved, return early
-                    if max_images is not None and max_images == len(url_list):
-                        return list(set(url_list))
-                    
-
-            except Exception as e:
-                continue
-        
-        return list(set(url_list))
-
-    # ------------------------------ image hash calculation -------------------------
-    def dhash(self, image, hashSize=8):
-        resized = cv2.resize(image, (hashSize + 1, hashSize))
-        diff = resized[:, 1:] > resized[:, :-1]
-        return sum([2 ** i for (i, v) in enumerate(diff.flatten()) if v])
-
-    # ------------------------------  save all downloaded images to folder ---------------------------
-    def saving_op(self, var):
-        url_list, folder_name = var
-        if not os.path.exists(os.path.join(os.getcwd(), folder_name)):
-                os.mkdir(os.path.join(os.getcwd(), folder_name))
-        for img in url_list:
-            result = get(img, stream=True).content
-            file_name = img.split("/")[-1]
-            file_path = os.path.join(os.getcwd(), folder_name, file_name)
-            img_arr = np.asarray(bytearray(result), dtype="uint8")
-            image = cv2.imdecode(img_arr, cv2.IMREAD_COLOR)
-            if not self.dhash(image) in self.unique_img:
-                cv2.imwrite(file_path, image)
-            self.unique_img.append(self.dhash(image))
-
-    # ------------------------------  download images from image url list ----------------------------
-    def download(self, url_list, num_of_workers, output_folder):
-        idx = len(url_list) // num_of_workers if len(url_list) > 9 else len(url_list)
-        param = []
-        for i in range(num_of_workers):
-            param.append((url_list[((i*idx)):(idx*(i+1))], output_folder))
-        with ThreadPoolExecutor(max_workers=num_of_workers) as executor:
-            executor.map(self.saving_op, param)
-
-    # -------------------------- get user keyword and google search for that keywords ---------------------
-    @staticmethod
-    def start_scraping(max_images, key=None, proxies={}):
-        assert key != None, "Please provide keyword for searching images"
-        keyword = key + " pinterest"
-        keyword = keyword.replace("+", "%20")
-        url = f'http://www.google.co.in/search?hl=en&q={keyword}'
-        res = get(url, proxies=proxies)
-        searched_urls = PinterestImageScraper.get_pinterest_links(res.content,max_images)
-
-        return searched_urls, key.replace(" ", "_")
-
-
-    def scrape(self, key=None, output_folder="", proxies={}, threads=10, max_images: int = None):
-        extracted_urls, keyword = PinterestImageScraper.start_scraping(max_images,key, proxies)
-
-        for i in extracted_urls:
-            self.get_source(i, proxies)
-
-        # get all urls of images and save in a list
-        url_list = self.save_image_url(max_images)
-        return_data = {
-            "isDownloaded": False,
-            "url_list": url_list,
-            "extracted_urls": extracted_urls,
-            "keyword": key
-        }
-
-        # download images from saved images url
-        if len(url_list):
-            try:
-                out_folder = output_folder if output_folder else key
-                self.download(url_list, threads, out_folder)
-            except KeyboardInterrupt:
-                return return_data
-            
-            return_data["isDownloaded"] = True
-            return return_data
-        
-        return return_data
-
-
-scraper = PinterestImageScraper()
-
-if __name__ == "__main__":
-    details = scraper.scrape("messi", "output")
-
-    if details["isDownloaded"]:
-        print("\nDownloading completed !!")
-    else:
-        print("\nNothing to download !!")
+import re
+import json
+import os
+import cv2
+import numpy as np
+
+from requests import get
+from bs4 import BeautifulSoup as soup
+from concurrent.futures import ThreadPoolExecutor
+
+from pydotmap import DotMap
+
+
+class PinterestImageScraper:
+
+    def __init__(self):
+        self.json_data_list = []
+        self.unique_img = []
+
+    # ---------------------------------------- GET GOOGLE RESULTS ---------------------------------
+    @staticmethod
+    def get_pinterest_links(body, max_images):
+        searched_urls = []
+        html = soup(body, 'html.parser')
+        links = html.select('#main > div > div > div > a')
+        for link in links:
+            link = link.get('href')
+            link = re.sub(r'/url\?q=', '', link)
+            if link[0] != "/" and "pinterest" in link:
+                searched_urls.append(link)
+                #stops adding links if the limit has been reached
+                if max_images is not None and max_images == len(searched_urls):
+                    break
+
+        return searched_urls
+
+    # -------------------------- save json data from source code of given pinterest url -------------
+    def get_source(self, url, proxies):
+        try:
+            res = get(url, proxies=proxies)
+        except Exception as e:
+            return
+        html = soup(res.text, 'html.parser')
+        json_data = html.find_all("script", attrs={"id": "__PWS_DATA__"})
+        for a in json_data:
+            self.json_data_list.append(a.string)
+
+    # --------------------------- READ JSON OF PINTEREST WEBSITE ----------------------
+    def save_image_url(self, max_images):
+        url_list = [i for i in self.json_data_list if i.strip()]
+        if not len(url_list):
+            return url_list
+        url_list = []
+        for js in self.json_data_list:
+            try:
+                data = DotMap(json.loads(js))
+                urls = []
+                for pin in data.props.initialReduxState.pins:
+                    if isinstance(data.props.initialReduxState.pins[pin].images.get("orig"), list):
+                        for i in data.props.initialReduxState.pins[pin].images.get("orig"):
+                            urls.append(i.get("url"))
+                    else:
+                        urls.append(data.props.initialReduxState.pins[pin].images.get("orig").get("url"))
+
+                for url in urls:
+                    url_list.append(url)
+
+                    #if the maximum has been achieved, return early
+                    if max_images is not None and max_images == len(url_list):
+                        return list(set(url_list))
+                    
+
+            except Exception as e:
+                continue
+        
+        return list(set(url_list))
+
+    # ------------------------------ image hash calculation -------------------------
+    def dhash(self, image, hashSize=8):
+        resized = cv2.resize(image, (hashSize + 1, hashSize))
+        diff = resized[:, 1:] > resized[:, :-1]
+        return sum([2 ** i for (i, v) in enumerate(diff.flatten()) if v])
+
+    # ------------------------------  save all downloaded images to folder ---------------------------
+    def saving_op(self, var):
+        url_list, folder_name = var
+        if not os.path.exists(os.path.join(os.getcwd(), folder_name)):
+                os.mkdir(os.path.join(os.getcwd(), folder_name))
+        for img in url_list:
+            result = get(img, stream=True).content
+            file_name = img.split("/")[-1]
+            file_path = os.path.join(os.getcwd(), folder_name, file_name)
+            img_arr = np.asarray(bytearray(result), dtype="uint8")
+            image = cv2.imdecode(img_arr, cv2.IMREAD_COLOR)
+            if not self.dhash(image) in self.unique_img:
+                cv2.imwrite(file_path, image)
+            self.unique_img.append(self.dhash(image))
+
+    # ------------------------------  download images from image url list ----------------------------
+    def download(self, url_list, num_of_workers, output_folder):
+        idx = len(url_list) // num_of_workers if len(url_list) > 9 else len(url_list)
+        param = []
+        for i in range(num_of_workers):
+            param.append((url_list[((i*idx)):(idx*(i+1))], output_folder))
+        with ThreadPoolExecutor(max_workers=num_of_workers) as executor:
+            executor.map(self.saving_op, param)
+
+    # -------------------------- get user keyword and google search for that keywords ---------------------
+    @staticmethod
+    def start_scraping(max_images, key=None, proxies={}):
+        assert key != None, "Please provide keyword for searching images"
+        keyword = key + " pinterest"
+        keyword = keyword.replace("+", "%20")
+        url = f'http://www.google.co.in/search?hl=en&q={keyword}'
+        res = get(url, proxies=proxies)
+        searched_urls = PinterestImageScraper.get_pinterest_links(res.content,max_images)
+
+        return searched_urls, key.replace(" ", "_")
+
+
+    def scrape(self, key=None, output_folder="", proxies={}, threads=10, max_images: int = None):
+        extracted_urls, keyword = PinterestImageScraper.start_scraping(max_images,key, proxies)
+
+        for i in extracted_urls:
+            self.get_source(i, proxies)
+
+        # get all urls of images and save in a list
+        url_list = self.save_image_url(max_images)
+        return_data = {
+            "isDownloaded": False,
+            "url_list": url_list,
+            "extracted_urls": extracted_urls,
+            "keyword": key
+        }
+
+        # download images from saved images url
+        if len(url_list):
+            try:
+                out_folder = output_folder if output_folder else key
+                self.download(url_list, threads, out_folder)
+            except KeyboardInterrupt:
+                return return_data
+            
+            return_data["isDownloaded"] = True
+            return return_data
+        
+        return return_data
+
+
+scraper = PinterestImageScraper()
+
+if __name__ == "__main__":
+    details = scraper.scrape("messi", "output")
+
+    if details["isDownloaded"]:
+        print("\nDownloading completed !!")
+    else:
+        print("\nNothing to download !!")
```

### Comparing `pinscrape-2.0.0/setup.py` & `pinscrape-2.0.1/setup.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import setuptools
-from pinscrape._version import __version__
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-with open("requirements.txt", "r") as req:
-    reqs = req.read().split("\n")
-
-setuptools.setup(
-    name="pinscrape",
-    version=__version__,
-    author="Atul Singh",
-    author_email="atulsingh0401@gmail.com",
-    description="Pinterest data scraper",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/iamatulsingh/pinscrape",
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-    install_requires=reqs,
-)
+import setuptools
+from pinscrape._version import __version__
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+with open("requirements.txt", "r") as req:
+    reqs = req.read().split("\n")
+
+setuptools.setup(
+    name="pinscrape",
+    version=__version__,
+    author="Atul Singh",
+    author_email="atulsingh0401@gmail.com",
+    description="Pinterest data scraper",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/iamatulsingh/pinscrape",
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.6',
+    install_requires=reqs,
+)
```

