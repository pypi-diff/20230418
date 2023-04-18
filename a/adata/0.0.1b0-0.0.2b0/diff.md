# Comparing `tmp/adata-0.0.1b0.tar.gz` & `tmp/adata-0.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata-0.0.1b0.tar", last modified: Wed Apr  5 11:54:39 2023, max compression
+gzip compressed data, was "adata-0.0.2b0.tar", last modified: Tue Apr 18 15:37:59 2023, max compression
```

## Comparing `adata-0.0.1b0.tar` & `adata-0.0.2b0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.681016 adata-0.0.1b0/
--rw-rw-rw-   0        0        0      608 2023-04-05 02:53:34.000000 adata-0.0.1b0/HISTORY.md
--rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.1b0/LICENSE
--rw-rw-rw-   0        0        0       27 2023-04-05 11:52:29.000000 adata-0.0.1b0/MANIFEST.in
--rw-rw-rw-   0        0        0     1616 2023-04-05 11:54:39.679014 adata-0.0.1b0/PKG-INFO
--rw-rw-rw-   0        0        0      898 2023-04-05 09:53:12.000000 adata-0.0.1b0/README.en.md
--rw-rw-rw-   0        0        0      988 2023-04-05 05:03:13.000000 adata-0.0.1b0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.622401 adata-0.0.1b0/adata/
--rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.1b0/adata/__init__.py
--rw-rw-rw-   0        0        0      745 2023-04-05 11:45:42.000000 adata-0.0.1b0/adata/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.638014 adata-0.0.1b0/adata/bond/
--rw-rw-rw-   0        0        0      104 2023-04-05 09:48:29.000000 adata-0.0.1b0/adata/bond/__init__.py
--rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.1b0/adata/bond/bond_market.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.639013 adata-0.0.1b0/adata/common/
--rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.1b0/adata/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.644014 adata-0.0.1b0/adata/common/headers/
--rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.1b0/adata/common/headers/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.1b0/adata/common/headers/baidu_headers.py
--rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.1b0/adata/common/headers/ths_headers.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.651033 adata-0.0.1b0/adata/common/utils/
--rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.1b0/adata/common/utils/__init__.py
--rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.1b0/adata/common/utils/snowflake.py
--rw-rw-rw-   0        0        0      972 2023-04-05 09:48:28.000000 adata-0.0.1b0/adata/common/utils/sunrequests.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.655016 adata-0.0.1b0/adata/etf/
--rw-rw-rw-   0        0        0      103 2023-04-05 09:48:29.000000 adata-0.0.1b0/adata/etf/__init__.py
--rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.1b0/adata/etf/etf_market.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.658017 adata-0.0.1b0/adata/message/
--rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.1b0/adata/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.660015 adata-0.0.1b0/adata/stock/
--rw-rw-rw-   0        0        0      294 2023-04-05 02:53:35.000000 adata-0.0.1b0/adata/stock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.662014 adata-0.0.1b0/adata/stock/index/
--rw-rw-rw-   0        0        0       87 2023-04-05 09:48:29.000000 adata-0.0.1b0/adata/stock/index/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.669046 adata-0.0.1b0/adata/stock/info/
--rw-rw-rw-   0        0        0      289 2023-04-05 09:48:30.000000 adata-0.0.1b0/adata/stock/info/__init__.py
--rw-rw-rw-   0        0        0     2446 2023-04-05 09:48:29.000000 adata-0.0.1b0/adata/stock/info/stock_code.py
--rw-rw-rw-   0        0        0     3933 2023-04-05 05:05:45.000000 adata-0.0.1b0/adata/stock/info/stock_gn.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.676121 adata-0.0.1b0/adata/stock/market/
--rw-rw-rw-   0        0        0      378 2023-04-05 09:53:12.000000 adata-0.0.1b0/adata/stock/market/__init__.py
--rw-rw-rw-   0        0        0     2412 2023-04-05 04:59:23.000000 adata-0.0.1b0/adata/stock/market/stock_dividend.py
--rw-rw-rw-   0        0        0     3414 2023-04-05 09:48:30.000000 adata-0.0.1b0/adata/stock/market/stock_market.py
--rw-rw-rw-   0        0        0     3577 2023-04-05 04:59:22.000000 adata-0.0.1b0/adata/stock/market/stock_market_gn.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.677014 adata-0.0.1b0/adata/stock/sentiment/
--rw-rw-rw-   0        0        0       87 2023-04-05 09:48:28.000000 adata-0.0.1b0/adata/stock/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 11:54:39.631408 adata-0.0.1b0/adata.egg-info/
--rw-rw-rw-   0        0        0     1616 2023-04-05 11:54:39.000000 adata-0.0.1b0/adata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      930 2023-04-05 11:54:39.000000 adata-0.0.1b0/adata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 11:54:39.000000 adata-0.0.1b0/adata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-05 11:54:39.000000 adata-0.0.1b0/adata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-05 11:54:39.000000 adata-0.0.1b0/adata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       71 2023-04-05 05:05:21.000000 adata-0.0.1b0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 11:54:39.681016 adata-0.0.1b0/setup.cfg
--rw-rw-rw-   0        0        0     1790 2023-04-05 05:05:21.000000 adata-0.0.1b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.206817 adata-0.0.2b0/
+-rw-rw-rw-   0        0        0      186 2023-04-06 11:14:06.000000 adata-0.0.2b0/HISTORY.md
+-rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.2b0/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-04-06 11:14:06.000000 adata-0.0.2b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6780 2023-04-18 15:37:59.135762 adata-0.0.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0     6141 2023-04-18 15:14:02.000000 adata-0.0.2b0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.088171 adata-0.0.2b0/adata/
+-rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.2b0/adata/__init__.py
+-rw-rw-rw-   0        0        0      756 2023-04-18 15:34:24.000000 adata-0.0.2b0/adata/__version__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.100173 adata-0.0.2b0/adata/bond/
+-rw-rw-rw-   0        0        0      122 2023-04-06 11:14:06.000000 adata-0.0.2b0/adata/bond/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.2b0/adata/bond/bond_market.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.101174 adata-0.0.2b0/adata/common/
+-rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.2b0/adata/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.107762 adata-0.0.2b0/adata/common/headers/
+-rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.2b0/adata/common/headers/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.2b0/adata/common/headers/baidu_headers.py
+-rw-rw-rw-   0        0        0      602 2023-04-18 15:14:02.000000 adata-0.0.2b0/adata/common/headers/sina_headers.py
+-rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.2b0/adata/common/headers/ths_headers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.112762 adata-0.0.2b0/adata/common/utils/
+-rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.2b0/adata/common/utils/__init__.py
+-rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.2b0/adata/common/utils/snowflake.py
+-rw-rw-rw-   0        0        0      972 2023-04-05 09:48:28.000000 adata-0.0.2b0/adata/common/utils/sunrequests.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.116764 adata-0.0.2b0/adata/etf/
+-rw-rw-rw-   0        0        0      118 2023-04-06 11:14:06.000000 adata-0.0.2b0/adata/etf/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.2b0/adata/etf/etf_market.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.117793 adata-0.0.2b0/adata/message/
+-rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.2b0/adata/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.119763 adata-0.0.2b0/adata/stock/
+-rw-rw-rw-   0        0        0      333 2023-04-06 11:14:06.000000 adata-0.0.2b0/adata/stock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.120794 adata-0.0.2b0/adata/stock/index/
+-rw-rw-rw-   0        0        0      105 2023-04-06 11:14:06.000000 adata-0.0.2b0/adata/stock/index/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.125764 adata-0.0.2b0/adata/stock/info/
+-rw-rw-rw-   0        0        0      322 2023-04-13 14:47:15.000000 adata-0.0.2b0/adata/stock/info/__init__.py
+-rw-rw-rw-   0        0        0     2459 2023-04-13 14:47:15.000000 adata-0.0.2b0/adata/stock/info/stock_code.py
+-rw-rw-rw-   0        0        0     4145 2023-04-13 14:47:15.000000 adata-0.0.2b0/adata/stock/info/stock_concept.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.132763 adata-0.0.2b0/adata/stock/market/
+-rw-rw-rw-   0        0        0      408 2023-04-13 14:47:15.000000 adata-0.0.2b0/adata/stock/market/__init__.py
+-rw-rw-rw-   0        0        0     2644 2023-04-13 14:47:15.000000 adata-0.0.2b0/adata/stock/market/stock_dividend.py
+-rw-rw-rw-   0        0        0     9479 2023-04-18 15:14:02.000000 adata-0.0.2b0/adata/stock/market/stock_market.py
+-rw-rw-rw-   0        0        0     3631 2023-04-18 15:14:02.000000 adata-0.0.2b0/adata/stock/market/stock_market_concept.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.133763 adata-0.0.2b0/adata/stock/sentiment/
+-rw-rw-rw-   0        0        0      115 2023-04-06 11:14:06.000000 adata-0.0.2b0/adata/stock/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 15:37:59.096172 adata-0.0.2b0/adata.egg-info/
+-rw-rw-rw-   0        0        0     6780 2023-04-18 15:37:58.000000 adata-0.0.2b0/adata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2023-04-18 15:37:59.000000 adata-0.0.2b0/adata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 15:37:58.000000 adata-0.0.2b0/adata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-18 15:37:58.000000 adata-0.0.2b0/adata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-18 15:37:58.000000 adata-0.0.2b0/adata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       69 2023-04-06 11:14:06.000000 adata-0.0.2b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 15:37:59.206817 adata-0.0.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     1790 2023-04-18 15:37:51.000000 adata-0.0.2b0/setup.py
```

### Comparing `adata-0.0.1b0/LICENSE` & `adata-0.0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `adata-0.0.1b0/adata/__init__.py` & `adata-0.0.2b0/adata/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.1b0/adata/__version__.py` & `adata-0.0.2b0/adata/__version__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 
-VERSION = (0, 0, 1)
+VERSION = (0, 0, 2)
 # PRERELEASE = None  # alpha, beta or rc
 PRERELEASE = 'beta'  # alpha, beta or rc
 REVISION = None
 
 
 def generate_version(version, prerelease=None, revision=None):
     version_parts = [".".join(map(str, version))]
     if prerelease is not None:
         version_parts.append(f"-{prerelease}")
     if revision is not None:
         version_parts.append(f".{revision}")
     return "".join(version_parts)
 
 __title__ = "adata"
-__description__ = "adata,stock,A,bond"
+__description__ = "A Data,A Stock,ETF,Bond,Quant"
 __url__ = "https://gitee.com/inchaos/adata"
 __version__ = generate_version(VERSION, prerelease=PRERELEASE, revision=REVISION)
 __author__ = "1nchaos"
 __author_email__ = "9527@1nchaos.com"
 __license__ = "Apache License"
```

### Comparing `adata-0.0.1b0/adata/common/headers/baidu_headers.py` & `adata-0.0.2b0/adata/common/headers/baidu_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.1b0/adata/common/headers/ths_headers.py` & `adata-0.0.2b0/adata/common/headers/ths_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.1b0/adata/common/utils/snowflake.py` & `adata-0.0.2b0/adata/common/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.1b0/adata/common/utils/sunrequests.py` & `adata-0.0.2b0/adata/common/utils/sunrequests.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.1b0/adata/stock/info/stock_code.py` & `adata-0.0.2b0/adata/stock/info/stock_code.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,34 +21,33 @@
 
     def __init__(self) -> None:
         super().__init__()
 
     def all_code(self):
         """
         获取所有股票的代码
-        :return: 所有股票的代码信息： ['code','name','exchange','status']
+        :return: 所有股票的代码信息： ['code','name','exchange']
         """
         return self.__market_rank_baidu()
 
     def __market_rank_baidu(self):
         """
         获取百度当前涨幅排名的代码
         web： https://gushitong.baidu.com/top/ab-increase-%E6%B6%A8%E5%B9%85%E6%A6%9C
         url：https://finance.pae.baidu.com/selfselect/getmarketrank?sort_type=1&sort_key=14&from_mid=1&pn=0&rn=200&group=pclist&type=ab&finClientType=pc
         其中：pn 起始数 rn 翻页数，最大200
-        :return 代码列表：['code','name','exchange','status']
-                status: 0.停牌
+        :return 代码列表：['code','short_name','exchange']
         """
         # 1. 请求市场排名的 url
         api_url = f"https://finance.pae.baidu.com/selfselect/getmarketrank" \
                   f"?sort_type=1&sort_key=14&from_mid=1&group=pclist&type=ab&finClientType=pc"
         max_page_size = 200
         data = []
 
-        # 2. 一直翻页请求数据，股票目前数据5000,100页一共2w
+        # 2. 一直翻页请求数据，股票目前数据5000,50页一共1w只,后续增加了可以再加
         for page_no in tqdm(range(49)):
             api_url = f"{api_url}&pn={page_no * max_page_size}&rn={max_page_size}"
             try:
                 res = requests.get(api_url, headers=baidu_headers.json_headers, proxies={})
                 res_json = res.json()
                 if res.status_code != 200 or res_json['ResultCode'] != '0':
                     continue
@@ -60,12 +59,12 @@
                 code_list = result[0]['DisplayData']['resultData']['tplData']['result']['rank']
                 data.extend(code_list)
             except Exception as e:
                 time.sleep(2)
                 print(e)
                 continue
         # 4. 封装数据
-        return pd.DataFrame(data=data)[['code', 'name', 'exchange', 'status']]
+        return pd.DataFrame(data=data)[['code', 'name', 'exchange']].rename(columns={'name': 'short_name'})
 
 
 if __name__ == '__main__':
     print(StockCode().all_code())
```

### Comparing `adata-0.0.1b0/adata/stock/info/stock_gn.py` & `adata-0.0.2b0/adata/stock/info/stock_concept.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 import pandas as pd
 from bs4 import BeautifulSoup
 
 from adata.common.headers import ths_headers
 from adata.common.utils import requests
 
 
-class StockGn(object):
+class StockConcept(object):
     """
     股票概念
     """
 
     def __init__(self) -> None:
         super().__init__()
 
-    def all_gn_code_ths(self):
+    def all_concept_code_ths(self):
         """
         获取同花顺概念列表：代码和名称
         :return: 概念[[code,name]]
         """
-        return pd.concat([self.gn_code_ths_pc(), self.gn_code_ths_app()]).reset_index(drop=True)
+        return pd.concat([self.concept_code_ths_pc(), self.concept_code_ths_app()]).reset_index(drop=True)
 
-    def gn_code_ths_pc(self):
+    def concept_code_ths_pc(self):
         """
         获取同花顺的所有概念和概念代码
         web: http://q.10jqka.com.cn/gn/
         """
         # 1. 请求接口 url
         api_url = f"http://q.10jqka.com.cn/gn/"
         for i in range(3):
@@ -45,17 +45,19 @@
             data = []
             for a in soup.find_all('a'):
                 href = str(a['href'])
                 if href.startswith(api_url + 'detail/code/'):
                     data.append([href[-7: -1], a.string, href])
 
             # 4. 封装数据
-            return pd.DataFrame(data=data, columns=['code', 'name', 'href'])[['code', 'name']]
+            data_df = pd.DataFrame(data=data, columns=['code', 'name', 'href'])[['code', 'name']]
+            data_df['source'] = '同花顺PC'
+            return data_df
 
-    def gn_code_ths_app(self):
+    def concept_code_ths_app(self):
         """
         获取app的概率列表，通过问财询问得到结果
         :return: app的概念列表： code，name
         """
         data = []
         for i in range(1, 10):
             api_url = f"http://search.10jqka.com.cn/gateway/urp/v7/landing/getDataList?perpage=100&page={i}&query=%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5&condition=%5B%7B%22indexName%22%3A%22%E6%8C%87%E6%95%B0%40%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22indexProperties%22%3A%5B%5D%2C%22source%22%3A%22new_parser%22%2C%22type%22%3A%22index%22%2C%22indexPropertiesMap%22%3A%7B%7D%2C%22reportType%22%3A%22null%22%2C%22chunkedResult%22%3A%22%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5%22%2C%22valueType%22%3A%22_%E6%8C%87%E6%95%B0%E7%B1%BB%E5%9E%8B%22%2C%22domain%22%3A%22abs_a%E6%8C%87%E9%A2%86%E5%9F%9F%22%2C%22uiText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22sonSize%22%3A0%2C%22queryText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22relatedSize%22%3A0%7D%5D&urp_sort_index=%E6%8C%87%E6%95%B0%E4%BB%A3%E7%A0%81&source=Ths_iwencai_Xuangu&urp_sort_way=desc&codelist=&page_id=&logid=35df00ee5ae706d0dfcd0dbfdb846e0c&ret=json_all&sessionid=35df00ee5ae706d0dfcd0dbfdb846e0c&iwc_token=0ac9667016801698001765831&user_id=Ths_iwencai_Xuangu_7fahywzhbkrh4lwwkwfw936njqbjzsly&uuids%5B0%5D=23119&query_type=zhishu&comp_id=6367801&business_cat=soniu&uuid=23119"
@@ -63,15 +65,17 @@
             res_json = res.json()
             if res_json['status_msg'] == 'ok':
                 data_list = res_json['answer']['components'][0]['data']['datas']
                 if len(data_list) < 1:
                     break
                 for d in data_list:
                     data.append([d['code'], d['指数简称']])
-        return pd.DataFrame(data=data, columns=['code', 'name']).drop_duplicates(keep='first', inplace=False,
-                                                                                 ignore_index=False)
+        data_df = pd.DataFrame(data=data, columns=['code', 'name']).drop_duplicates(keep='first', inplace=False,
+                                                                                    ignore_index=False)
+        data_df['source'] = '同花顺APP'
+        return data_df
 
 
 if __name__ == '__main__':
-    print(StockGn().all_gn_code_ths())
-    print(StockGn().gn_code_ths_pc())
-    print(StockGn().gn_code_ths_app())
+    print(StockConcept().all_concept_code_ths())
+    print(StockConcept().concept_code_ths_pc())
+    print(StockConcept().concept_code_ths_app())
```

### Comparing `adata-0.0.1b0/adata/stock/market/stock_dividend.py` & `adata-0.0.2b0/adata/stock/market/stock_dividend.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8 -*-
 """
-@desc: readme
+@desc: 股票分红信息
+数据来源：1. 百度
+
 @author: 1nchaos
 @time: 2023/3/29
 @log: change log
 """
 
 import pandas as pd
 
@@ -57,13 +59,15 @@
         new_company = result[-1]['DisplayData']['resultData']['tplData']['result']['tabs'][-1]['content'][
             'newCompany']
         bonus_transfer = new_company['bonusTransfer']
         header = bonus_transfer['header']
         body = bonus_transfer['body']
 
         # 4. 封装数据
-        result_df = pd.DataFrame(data=body, columns=header)
-        return result_df[['公告日', '分红方案', '除权除息日']]
+        result_df = pd.DataFrame(data=body, columns=header)[['公告日', '分红方案', '除权除息日']]
+        result_df['code'] = code
+        rename_columns = {'公告日': 'report_date', '分红方案': 'dividend_plan', '除权除息日': 'ex_dividend_date'}
+        return result_df.rename(columns=rename_columns)
 
 
 if __name__ == '__main__':
     print(StockDividend().get_dividend(code='000001'))
```

### Comparing `adata-0.0.1b0/adata/stock/market/stock_market_gn.py` & `adata-0.0.2b0/adata/stock/market/stock_market_concept.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
 import pandas as pd
 
 from adata.common.headers import ths_headers
 from adata.common.utils import requests
 
 
-class StockMarketGn(object):
+class StockMarketConcept(object):
     """
     股票概念 行情
     """
 
     def __init__(self) -> None:
         super().__init__()
 
-    def get_market_gn_ths(self, code: str = '886013', k_type: int = 1, adjust_type: int = 1):
+    def get_market_concept_ths(self, code: str = '886013', k_type: int = 1, adjust_type: int = 1):
         """
         获取同花顺的概率的行情
         web: http://q.10jqka.com.cn/gn/
         url: http://d.10jqka.com.cn/v6/line/48_886013/01/last1800.js
         00 日k不复权；01日k前复权；02日k后复权；11周k前复权；21月k前复权
         :param code: 同花顺概念代码
         :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
@@ -47,17 +47,18 @@
         result_text = text[text.index('{'):-1]
         data_list = json.loads(result_text)['data'].split(';')
         data = []
         for d in data_list:
             data.append(str(d).split(',')[0:7])
         return pd.DataFrame(data=data, columns=['trade_date', 'open', 'high', 'low', 'close', 'vol', 'amount'])
 
-    def get_market_gn_today_ths(self, code):
+    def get_market_concept_min_ths(self, code):
         """
         获取概念行情当日分时 TODO
         web： http://d.10jqka.com.cn/v6/time/48_886013/last.js
         :param code: 概念代码
         """
+        return pd.DataFrame()
 
 
 if __name__ == '__main__':
-    print(StockMarketGn().get_market_gn_ths(code='886013'))
+    print(StockMarketConcept().get_market_concept_ths(code='886013'))
```

### Comparing `adata-0.0.1b0/adata.egg-info/SOURCES.txt` & `adata-0.0.2b0/adata.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 HISTORY.md
 LICENSE
 MANIFEST.in
-README.en.md
 README.md
 requirements.txt
 setup.py
 adata/__init__.py
 adata/__version__.py
 adata.egg-info/PKG-INFO
 adata.egg-info/SOURCES.txt
@@ -13,24 +12,25 @@
 adata.egg-info/requires.txt
 adata.egg-info/top_level.txt
 adata/bond/__init__.py
 adata/bond/bond_market.py
 adata/common/__init__.py
 adata/common/headers/__init__.py
 adata/common/headers/baidu_headers.py
+adata/common/headers/sina_headers.py
 adata/common/headers/ths_headers.py
 adata/common/utils/__init__.py
 adata/common/utils/snowflake.py
 adata/common/utils/sunrequests.py
 adata/etf/__init__.py
 adata/etf/etf_market.py
 adata/message/__init__.py
 adata/stock/__init__.py
 adata/stock/index/__init__.py
 adata/stock/info/__init__.py
 adata/stock/info/stock_code.py
-adata/stock/info/stock_gn.py
+adata/stock/info/stock_concept.py
 adata/stock/market/__init__.py
 adata/stock/market/stock_dividend.py
 adata/stock/market/stock_market.py
-adata/stock/market/stock_market_gn.py
+adata/stock/market/stock_market_concept.py
 adata/stock/sentiment/__init__.py
```

### Comparing `adata-0.0.1b0/setup.py` & `adata-0.0.2b0/setup.py`

 * *Files identical despite different names*

