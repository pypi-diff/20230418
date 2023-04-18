# Comparing `tmp/yourtools-0.5.5.tar.gz` & `tmp/yourtools-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yourtools-0.5.5.tar", last modified: Tue Apr 18 01:52:47 2023, max compression
+gzip compressed data, was "dist/yourtools-0.5.6.tar", last modified: Tue Apr 18 06:07:54 2023, max compression
```

## Comparing `yourtools-0.5.5.tar` & `yourtools-0.5.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 01:52:47.000000 yourtools-0.5.5/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools/db/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.5.5/yourtools/db/__init__.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.5.5/yourtools/db/dbutils.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.5.5/yourtools/db/hive.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.5.5/yourtools/db/mysql.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.5.5/yourtools/Azkaban.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     1025 2023-04-18 01:51:31.000000 yourtools-0.5.5/yourtools/Time.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     6292 2023-04-14 11:05:56.000000 yourtools-0.5.5/yourtools/WeChat.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      474 2023-04-14 10:42:59.000000 yourtools-0.5.5/yourtools/__init__.py
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/SOURCES.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/dependency_links.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/requires.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/top_level.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.5.5/README.md
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.5.5/requirements.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-14 10:46:10.000000 yourtools-0.5.5/setup.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-18 01:52:47.000000 yourtools-0.5.5/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-18 01:52:47.000000 yourtools-0.5.5/setup.cfg
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 06:07:54.000000 yourtools-0.5.6/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 06:07:54.000000 yourtools-0.5.6/yourtools/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 06:07:54.000000 yourtools-0.5.6/yourtools/db/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.5.6/yourtools/db/__init__.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.5.6/yourtools/db/dbutils.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.5.6/yourtools/db/hive.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.5.6/yourtools/db/mysql.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.5.6/yourtools/Azkaban.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     1025 2023-04-18 01:51:31.000000 yourtools-0.5.6/yourtools/Time.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     6292 2023-04-14 11:05:56.000000 yourtools-0.5.6/yourtools/WeChat.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      474 2023-04-14 10:42:59.000000 yourtools-0.5.6/yourtools/__init__.py
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 06:07:54.000000 yourtools-0.5.6/yourtools.egg-info/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-18 06:07:54.000000 yourtools-0.5.6/yourtools.egg-info/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-18 06:07:54.000000 yourtools-0.5.6/yourtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-18 06:07:54.000000 yourtools-0.5.6/yourtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-18 06:07:54.000000 yourtools-0.5.6/yourtools.egg-info/requires.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-18 06:07:54.000000 yourtools-0.5.6/yourtools.egg-info/top_level.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.5.6/README.md
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.5.6/requirements.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2364 2023-04-18 06:07:38.000000 yourtools-0.5.6/setup.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-18 06:07:54.000000 yourtools-0.5.6/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-18 06:07:54.000000 yourtools-0.5.6/setup.cfg
```

### Comparing `yourtools-0.5.5/yourtools/db/dbutils.py` & `yourtools-0.5.6/yourtools/db/dbutils.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.5/yourtools/db/hive.py` & `yourtools-0.5.6/yourtools/db/hive.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.5/yourtools/db/mysql.py` & `yourtools-0.5.6/yourtools/db/mysql.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.5/yourtools/Azkaban.py` & `yourtools-0.5.6/yourtools/Azkaban.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.5/yourtools/Time.py` & `yourtools-0.5.6/yourtools/Time.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.5/yourtools/WeChat.py` & `yourtools-0.5.6/yourtools/WeChat.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.5/yourtools.egg-info/PKG-INFO` & `yourtools-0.5.6/yourtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.5.5
+Version: 0.5.6
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yourtools-0.5.5/README.md` & `yourtools-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.5/setup.py` & `yourtools-0.5.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,31 @@
 import setuptools
 import re
+import requests
+from bs4 import BeautifulSoup
 
-with open('VERSION') as f:
-    version_str = f.read()
+package_name = "yourtools"
+
+
+def curr_version():
+    # 方法1：通过文件临时存储版本号
+    # with open('VERSION') as f:
+    #     version_str = f.read()
+
+    # 方法2：从官网获取版本号
+    url = f"https://pypi.org/project/{package_name}/"
+    response = requests.get(url)
+    soup = BeautifulSoup(response.content, "html.parser")
+    latest_version = soup.select_one(".release__version").text.strip()
+    return str(latest_version)
 
 
 def get_version():
     # 从版本号字符串中提取三个数字并将它们转换为整数类型
-    match = re.search(r"(\d+)\.(\d+)\.(\d+)", version_str)
+    match = re.search(r"(\d+)\.(\d+)\.(\d+)", curr_version())
     major = int(match.group(1))
     minor = int(match.group(2))
     patch = int(match.group(3))
 
     # 对三个数字进行加一操作
     patch += 1
     if patch > 9:
@@ -20,41 +34,54 @@
         if minor > 9:
             minor = 0
             major += 1
     new_version_str = f"{major}.{minor}.{patch}"
     return new_version_str
 
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-with open('requirements.txt') as f:
-    required = f.read().splitlines()
-
-setuptools.setup(
-    name="yourtools",
-    version=get_version(),
-    author="zfang",
-    author_email="founder517518@163.com",
-    description="Python helper tools",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://pypi.org/project/yourtools/",
-    packages=setuptools.find_packages(),
-    data_files=["requirements.txt"],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.6',
-    install_requires=required,
-)
+def upload():
+    with open("README.md", "r") as fh:
+        long_description = fh.read()
+    with open('requirements.txt') as f:
+        required = f.read().splitlines()
+
+    setuptools.setup(
+        name=package_name,
+        version=get_version(),
+        author="zfang",
+        author_email="founder517518@163.com",
+        description="Python helper tools",
+        long_description=long_description,
+        long_description_content_type="text/markdown",
+        url="https://pypi.org/project/yourtools/",
+        packages=setuptools.find_packages(),
+        data_files=["requirements.txt"],
+        classifiers=[
+            "Programming Language :: Python :: 3",
+            "License :: OSI Approved :: MIT License",
+            "Operating System :: OS Independent",
+        ],
+        python_requires='>=3.6',
+        install_requires=required,
+    )
 
 
 def write_now_version():
     print("Current VERSION:", get_version())
     with open("VERSION", "w") as version_f:
         version_f.write(get_version())
 
 
-# 将新的版本号字符串回写入文件中
-write_now_version()
+def main():
+    try:
+        upload()
+    except Exception as e:
+        raise Exception("Upload package error", e)
+
+    # 将新的版本号字符串回写入文件中
+    # write_now_version()
+
+    print("Upload success , Current VERSION:", curr_version())
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `yourtools-0.5.5/PKG-INFO` & `yourtools-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.5.5
+Version: 0.5.6
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

