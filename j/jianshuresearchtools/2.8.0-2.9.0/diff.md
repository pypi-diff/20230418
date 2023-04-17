# Comparing `tmp/JianshuResearchTools-2.8.0.tar.gz` & `tmp/JianshuResearchTools-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JianshuResearchTools-2.8.0.tar", last modified: Wed Jan 12 14:59:03 2022, max compression
+gzip compressed data, was "JianshuResearchTools-2.9.0.tar", last modified: Sat Jan 22 15:50:28 2022, max compression
```

## Comparing `JianshuResearchTools-2.8.0.tar` & `JianshuResearchTools-2.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-01-12 14:59:03.306903 JianshuResearchTools-2.8.0/
-drwxrwxrwx   0        0        0        0 2022-01-12 14:59:03.041127 JianshuResearchTools-2.8.0/JianshuResearchTools/
--rw-rw-rw-   0        0        0      349 2022-01-12 14:57:08.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/__init__.py
--rw-rw-rw-   0        0        0    17639 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/article.py
--rw-rw-rw-   0        0        0     6236 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/assert_funcs.py
--rw-rw-rw-   0        0        0     9628 2022-01-12 14:57:08.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/basic_apis.py
--rw-rw-rw-   0        0        0     6066 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/beikeisland.py
--rw-rw-rw-   0        0        0    12942 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/collection.py
--rw-rw-rw-   0        0        0     8304 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/convert.py
--rw-rw-rw-   0        0        0      306 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/exceptions.py
--rw-rw-rw-   0        0        0     1050 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/headers.py
--rw-rw-rw-   0        0        0     8831 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/island.py
--rw-rw-rw-   0        0        0     6901 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/notebook.py
--rw-rw-rw-   0        0        0    30738 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/objects.py
--rw-rw-rw-   0        0        0     5466 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/rank.py
--rw-rw-rw-   0        0        0    35592 2022-01-12 14:57:08.000000 JianshuResearchTools-2.8.0/JianshuResearchTools/user.py
-drwxrwxrwx   0        0        0        0 2022-01-12 14:59:03.302896 JianshuResearchTools-2.8.0/JianshuResearchTools.egg-info/
--rw-rw-rw-   0        0        0     5199 2022-01-12 14:59:02.000000 JianshuResearchTools-2.8.0/JianshuResearchTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2022-01-12 14:59:02.000000 JianshuResearchTools-2.8.0/JianshuResearchTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-12 14:59:02.000000 JianshuResearchTools-2.8.0/JianshuResearchTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2022-01-12 14:59:02.000000 JianshuResearchTools-2.8.0/JianshuResearchTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2022-01-12 14:59:02.000000 JianshuResearchTools-2.8.0/JianshuResearchTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2021-04-11 14:48:36.000000 JianshuResearchTools-2.8.0/LICENSE
--rw-rw-rw-   0        0        0     5199 2022-01-12 14:59:03.304899 JianshuResearchTools-2.8.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-01-12 14:59:03.306903 JianshuResearchTools-2.8.0/setup.cfg
--rw-rw-rw-   0        0        0      971 2021-12-31 12:33:03.000000 JianshuResearchTools-2.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-22 15:50:28.212355 JianshuResearchTools-2.9.0/
+drwxrwxrwx   0        0        0        0 2022-01-22 15:50:27.599361 JianshuResearchTools-2.9.0/JianshuResearchTools/
+-rw-rw-rw-   0        0        0      349 2022-01-22 15:48:14.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/__init__.py
+-rw-rw-rw-   0        0        0    20666 2022-01-22 15:48:14.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/article.py
+-rw-rw-rw-   0        0        0     6236 2021-12-31 12:33:03.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/assert_funcs.py
+-rw-rw-rw-   0        0        0     9628 2022-01-12 14:57:08.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/basic_apis.py
+-rw-rw-rw-   0        0        0     6066 2021-12-31 12:33:03.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/beikeisland.py
+-rw-rw-rw-   0        0        0    15941 2022-01-22 15:48:14.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/collection.py
+-rw-rw-rw-   0        0        0     8304 2021-12-31 12:33:03.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/convert.py
+-rw-rw-rw-   0        0        0      306 2021-12-31 12:33:03.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/exceptions.py
+-rw-rw-rw-   0        0        0     1050 2021-12-31 12:33:03.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/headers.py
+-rw-rw-rw-   0        0        0    10877 2022-01-22 15:48:14.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/island.py
+-rw-rw-rw-   0        0        0     8597 2022-01-22 15:48:14.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/notebook.py
+-rw-rw-rw-   0        0        0    31958 2022-01-22 15:48:14.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/objects.py
+-rw-rw-rw-   0        0        0     5486 2022-01-22 15:48:14.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/rank.py
+-rw-rw-rw-   0        0        0    41056 2022-01-22 15:48:14.000000 JianshuResearchTools-2.9.0/JianshuResearchTools/user.py
+drwxrwxrwx   0        0        0        0 2022-01-22 15:50:28.206357 JianshuResearchTools-2.9.0/JianshuResearchTools.egg-info/
+-rw-rw-rw-   0        0        0     5199 2022-01-22 15:50:26.000000 JianshuResearchTools-2.9.0/JianshuResearchTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      696 2022-01-22 15:50:26.000000 JianshuResearchTools-2.9.0/JianshuResearchTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-22 15:50:26.000000 JianshuResearchTools-2.9.0/JianshuResearchTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2022-01-22 15:50:26.000000 JianshuResearchTools-2.9.0/JianshuResearchTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2022-01-22 15:50:26.000000 JianshuResearchTools-2.9.0/JianshuResearchTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2021-04-11 14:48:36.000000 JianshuResearchTools-2.9.0/LICENSE
+-rw-rw-rw-   0        0        0     5199 2022-01-22 15:50:28.209358 JianshuResearchTools-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2022-01-22 15:50:28.212355 JianshuResearchTools-2.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      971 2021-12-31 12:33:03.000000 JianshuResearchTools-2.9.0/setup.py
```

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/article.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/article.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,260 +10,289 @@
 
 try:
     from tomd import convert as html2md
 except ImportError:
     pass
 
 
-def GetArticleTitle(article_url: str) -> str:
+def GetArticleTitle(article_url: str, disable_check: bool = False) -> str:
     """获取文章标题
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 文章标题
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     result = json_obj["public_title"]
     return result
 
 
-def GetArticleAuthorName(article_url: str) -> str:
+def GetArticleAuthorName(article_url: str, disable_check: bool = False) -> str:
     """获取文章作者名
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 文章作者名
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleHtmlJsonDataApi(article_url)
     result = json_obj["props"]["initialState"]["note"]["data"]["user"]["nickname"]
     return result
 
 
-def GetArticleReadsCount(article_url: str) -> int:
+def GetArticleReadsCount(article_url: str, disable_check: bool = False) -> int:
     """获取文章阅读量
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 文章阅读量
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleHtmlJsonDataApi(article_url)
     result = json_obj["props"]["initialState"]["note"]["data"]["views_count"]
     return result
 
 
-def GetArticleWordage(article_url: str) -> int:
+def GetArticleWordage(article_url: str, disable_check: bool = False) -> int:
     """获取文章字数
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 文章字数
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleHtmlJsonDataApi(article_url)
     result = json_obj["props"]["initialState"]["note"]["data"]["wordage"]
     return result
 
 
-def GetArticleLikesCount(article_url: str) -> int:
+def GetArticleLikesCount(article_url: str, disable_check: bool = False) -> int:
     """获取文章点赞量
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 文章点赞量
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     result = json_obj["likes_count"]
     return result
 
 
-def GetArticleCommentsCount(article_url: str) -> int:
+def GetArticleCommentsCount(article_url: str, disable_check: bool = False) -> int:
     """获取文章评论数量
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 文章评论数量
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     result = json_obj["public_comment_count"]
     return result
 
 
-def GetArticleMostValuableCommentsCount(article_url: str) -> int:
+def GetArticleMostValuableCommentsCount(article_url: str, disable_check: bool = False) -> int:
     """获取文章精选评论数量
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 文章精选评论数量
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     result = json_obj["featured_comments_count"]
     return result
 
 
-def GetArticleTotalFPCount(article_url: str) -> float:
+def GetArticleTotalFPCount(article_url: str, disable_check: bool = False) -> float:
     """获取文章总获钻量
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 文章总获钻量
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     result = json_obj["total_fp_amount"] / 1000
     return result
 
 
-def GetArticleDescription(article_url: str) -> str:
+def GetArticleDescription(article_url: str, disable_check: bool = False) -> str:
     """获取文章摘要
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 文章摘要
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     result = json_obj["description"]
     return result
 
 
-def GetArticlePublishTime(article_url: str) -> datetime:
+def GetArticlePublishTime(article_url: str, disable_check: bool = False) -> datetime:
     """获取文章发布时间
 
     Args:
         article_url (str): 文章 Url
 
     Returns:
         datetime: 文章发布时间
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     result = datetime.fromisoformat(json_obj["first_shared_at"])
     return result
 
 
-def GetArticleUpdateTime(article_url: str) -> datetime:
+def GetArticleUpdateTime(article_url: str, disable_check: bool = False) -> datetime:
     """获取文章更新时间
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         datetime: 文章更新时间
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     result = datetime.fromtimestamp(json_obj["last_updated_at"])
     return result
 
 
-def GetArticlePaidStatus(article_url: str) -> bool:
+def GetArticlePaidStatus(article_url: str, disable_check: bool = False) -> bool:
     """获取文章付费状态
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         bool: 文章付费状态，True 为付费文章，False 为免费文章
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     paid_type = {
         "free": False,   # 免费文章
         "fbook_free": False,   # 免费连载中的免费文章
         "pbook_free": False,   # 付费连载中的免费文章
         "paid": True,   # 付费文章
         "fbook_paid": True,   # 免费连载中的付费文章
         "pbook_paid": True   # 付费连载中的付费文章
     }
     result = paid_type[json_obj["paid_type"]]
     return result
 
 
-def GetArticleReprintStatus(article_url: str) -> bool:
+def GetArticleReprintStatus(article_url: str, disable_check: bool = False) -> bool:
     """获取文章转载声明状态
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         bool: 文章转载声明状态，True 为允许转载，False 为禁止转载
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     result = json_obj["reprintable"]
     return result
 
 
-def GetArticleCommentStatus(article_url: str) -> bool:
+def GetArticleCommentStatus(article_url: str, disable_check: bool = False) -> bool:
     """获取文章评论区状态
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         bool: 文章评论区状态，True 为开启评论，False 为关闭评论
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     result = json_obj["commentable"]
     return result
 
 
-def GetArticleHtml(article_url: str) -> str:
+def GetArticleHtml(article_url: str, disable_check: bool = False) -> str:
     """获取 Html 格式的文章内容
 
     # ! 该函数可以获取设置禁止转载的文章内容，请尊重作者版权，由此带来的风险您需自行承担
     # ! 该函数不能获取文章付费部分的内容
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: Html 格式的文章内容
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     html_text = json_obj["free_content"]
     html_text = sub(r'<div class="image-[\w]*" [ \w+-="]*>', "", html_text)  # 去除 image-view 和 image-container
     html_text = sub(r'<div class="image-package">', "", html_text)  # 去除 image-package
     html_text = sub(r'<div class="image-container-fill".+>', "", html_text)  # 去除 image-container-fill
     old_img_blocks = findall(r'\<img[ \w+-="]*>', html_text)  # 匹配旧的 img 标签
     img_names = findall(r"\w+-\w+.jpg|\w+-\w+.png", html_text)  # 获取图片名称
@@ -273,52 +302,58 @@
     if not old_img_blocks:  # 文章中没有图片块
         return html_text
     for old_img_block, new_img_block in zip(old_img_blocks, new_img_blocks):
         html_text = html_text.replace(old_img_block, new_img_block)  # 替换 img 标签
     return html_text
 
 
-def GetArticleText(article_url: str) -> str:
+def GetArticleText(article_url: str, disable_check: bool = False) -> str:
     """获取纯文本格式的文章内容
 
     # ! 该函数可以获取设置禁止转载的文章内容，请尊重作者版权，由此带来的风险您需自行承担
     # ! 该函数不能获取文章付费部分的内容
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 纯文本格式的文章内容
     """
-    AssertArticleUrl(article_url)
-    AssertArticleStatusNormal(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     json_obj = GetArticleJsonDataApi(article_url)
     html_obj = etree.HTML(json_obj["free_content"])
     result = "".join(html_obj.itertext())
     result = sub(r"\s{3,}", "", result)  # 去除多余的空行
     return result
 
 
-def GetArticleMarkdown(article_url: str) -> str:
+def GetArticleMarkdown(article_url: str, disable_check: bool = False) -> str:
     """获取 Markdown 格式的文章内容
 
     # ! 该函数可以获取设置禁止转载的文章内容，请尊重作者版权，由此带来的风险您需自行承担
     # ! 该函数不能获取文章付费部分的内容
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: Markdown 格式的文章内容
     """
     try:
         html2md
     except NameError:
         raise ImportError("未安装 html2md 模块，该函数不可用")
-    html_text = GetArticleHtml(article_url)
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
+    html_text = GetArticleHtml(article_url, disable_check=True)
     image_descriptions = [description for description in findall(r'class="image-caption">.+</div>', html_text)]  # 获取图片描述块
     image_descriptions_text = [description.replace('class="image-caption">', "").replace("</div>", "")
                                for description in findall(r'class="image-caption">.+</div>', html_text)]  # 获取图片描述文本
     for index in range(len(image_descriptions)):
         html_text = html_text.replace(image_descriptions[index], "<p>&&" + image_descriptions_text[index] + "&&</p>")  # 将图片描述替换成带有标记符的文本
     images = findall(r'<img src=".+">', html_text)  # 获取图片块
     for image in images:
@@ -424,23 +459,27 @@
 
                 item_data["sub_comments"].append(sub_comment_data)
 
         result.append(item_data)
     return result
 
 
-def GetArticleAllBasicData(article_url: str) -> Dict:
+def GetArticleAllBasicData(article_url: str, disable_check: bool = False) -> Dict:
     """获取文章的全部基础信息
 
     Args:
         article_url (str): 文章 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         Dict: 文章基础信息
     """
+    if not disable_check:
+        AssertArticleUrl(article_url)
+        AssertArticleStatusNormal(article_url)
     result = {}
     json_obj = GetArticleJsonDataApi(article_url)
     html_json_obj = GetArticleHtmlJsonDataApi(article_url)
 
     result["title"] = json_obj["public_title"]
     result["author_name"] = html_json_obj["props"]["initialState"]["note"]["data"]["user"]["nickname"]
     result["reads_count"] = html_json_obj["props"]["initialState"]["note"]["data"]["views_count"]
@@ -461,29 +500,36 @@
         "pbook_paid": True
     }[json_obj["paid_type"]]
     result["reprint_status"] = json_obj["reprintable"]
     result["comment_status"] = json_obj["commentable"]
     return result
 
 
-def GetArticleAllCommentsData(article_id: int, count: int = 10,
-                              author_only: bool = False, sorting_method: str = "positive") -> Generator[List[Dict], None, None]:
+def GetArticleAllCommentsData(article_id: int, count: int = 10, author_only: bool = False,
+                              sorting_method: str = "positive", max_count: int = None) -> Generator[Dict, None, None]:
     """获取文章的全部评论信息
 
     Args:
         article_id (int): 文章 ID
         count (int, optional): 单次获取的数据数量，会影响性能. Defaults to 10.
         author_only (bool, optional): 为 True 时只获取作者发布的评论，包含作者发布的子评论及其父评论. Defaults to False.
         sorting_method (str, optional): 排序方式，为”positive“时按时间正序排列，为”reverse“时按时间倒序排列. Defaults to "positive".
+        max_count (int, optional): 获取的文章评论信息数量上限，Defaults to None.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页文章信息
+        Iterator[Dict], None, None]: 文章信息
     """
-
     page = 1
+    now_count = 0
     while True:
         result = GetArticleCommentsData(article_id, page, count, author_only, sorting_method)
         if result:
-            yield result
             page += 1
         else:
-            break
+            return
+        for item in result:
+            yield item
+            if max_count:
+                now_count += 1
+                if now_count == max_count:
+                    return
```

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/assert_funcs.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/assert_funcs.py`

 * *Files identical despite different names*

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/basic_apis.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/basic_apis.py`

 * *Files identical despite different names*

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/beikeisland.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/beikeisland.py`

 * *Files identical despite different names*

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/collection.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,153 +6,171 @@
                          GetCollectionEditorsJsonDataApi,
                          GetCollectionJsonDataApi,
                          GetCollectionRecommendedWritersJsonDataApi,
                          GetCollectionSubscribersJsonDataApi)
 from .convert import CollectionUrlToCollectionSlug
 
 
-def GetCollectionName(collection_url: str) -> str:
+def GetCollectionName(collection_url: str, disable_check: bool = False) -> str:
     """获取专题名称
 
     Args:
         collection_url (str): 专题 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 专题名称
     """
-    AssertCollectionUrl(collection_url)
-    AssertCollectionStatusNormal(collection_url)
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     json_obj = GetCollectionJsonDataApi(collection_url)
     result = json_obj["title"]
     return result
 
 
-def GetCollectionAvatarUrl(collection_url: str) -> str:
+def GetCollectionAvatarUrl(collection_url: str, disable_check: bool = False) -> str:
     """获取专题头像链接
 
     Args:
         collection_url (str): 专题 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 专题头像链接
     """
-    AssertCollectionUrl(collection_url)
-    AssertCollectionStatusNormal(collection_url)
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     json_obj = GetCollectionJsonDataApi(collection_url)
     result = json_obj["image"]
     return result
 
 
-def GetCollectionIntroductionText(collection_url: str) -> str:
+def GetCollectionIntroductionText(collection_url: str, disable_check: bool = False) -> str:
     """获取纯文本格式的专题简介
 
     Args:
         collection_url (str): 专题 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 纯文本格式的专题简介
     """
-    AssertCollectionUrl(collection_url)
-    AssertCollectionStatusNormal(collection_url)
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     json_obj = GetCollectionJsonDataApi(collection_url)
     result = json_obj["content_without_html"]
     return result
 
 
-def GetCollectionIntroductionHtml(collection_url: str) -> str:
+def GetCollectionIntroductionHtml(collection_url: str, disable_check: bool = False) -> str:
     """获取 Html 格式的专题简介
 
     Args:
         collection_url (str): 专题 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: Html 格式的专题简介
     """
-    AssertCollectionUrl(collection_url)
-    AssertCollectionStatusNormal(collection_url)
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     json_obj = GetCollectionJsonDataApi(collection_url)
     result = json_obj["content_in_full"]
     return result
 
 
-def GetCollectionArticlesCount(collection_url: str) -> int:
+def GetCollectionArticlesCount(collection_url: str, disable_check: bool = False) -> int:
     """获取专题中的文章数量
 
     Args:
         collection_url (str): 专题 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 专题中的文章数量
     """
-    AssertCollectionUrl(collection_url)
-    AssertCollectionStatusNormal(collection_url)
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     json_obj = GetCollectionJsonDataApi(collection_url)
     result = json_obj["notes_count"]
     return result
 
 
-def GetCollectionSubscribersCount(collection_url: str) -> int:
+def GetCollectionSubscribersCount(collection_url: str, disable_check: bool = False) -> int:
     """获取专题的订阅者数量
 
     Args:
         collection_url (str): 专题 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 专题的订阅者数量
     """
-    AssertCollectionUrl(collection_url)
-    AssertCollectionStatusNormal(collection_url)
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     json_obj = GetCollectionJsonDataApi(collection_url)
     result = json_obj["subscribers_count"]
     return result
 
 
-def GetCollectionArticlesUpdateTime(collection_url: str) -> datetime:
+def GetCollectionArticlesUpdateTime(collection_url: str, disable_check: bool = False) -> datetime:
     """获取专题文章更新时间
 
     Args:
         collection_url (str): 专题 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         datetime: 专题文章更新时间
     """
-    AssertCollectionUrl(collection_url)
-    AssertCollectionStatusNormal(collection_url)
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     json_obj = GetCollectionJsonDataApi(collection_url)
     result = datetime.fromtimestamp(json_obj["newly_added_at"])
     return result
 
 
-def GetCollectionInformationUpdateTime(collection_url: str) -> datetime:
+def GetCollectionInformationUpdateTime(collection_url: str, disable_check: bool = False) -> datetime:
     """获取专题信息更新时间
 
     Args:
         collection_url (str): 专题 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         datetime: 专题信息更新时间
     """
-    AssertCollectionUrl(collection_url)
-    AssertCollectionStatusNormal(collection_url)
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     json_obj = GetCollectionJsonDataApi(collection_url)
     result = datetime.fromtimestamp(json_obj["last_updated_at"])
     return result
 
 
-def GetCollectionOwnerInfo(collection_url: str) -> Dict:
+def GetCollectionOwnerInfo(collection_url: str, disable_check: bool = False) -> Dict:
     """获取专题的所有者信息
 
     Args:
         collection_url (str): 专题 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         Dict: 用户信息
     """
-    AssertCollectionUrl(collection_url)
-    AssertCollectionStatusNormal(collection_url)
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     json_obj = GetCollectionJsonDataApi(collection_url)
     result = {
         "uid": json_obj["owner"]["id"],
         "name": json_obj["owner"]["nickname"],
         "uslug": json_obj["owner"]["slug"]
     }
     return result
@@ -204,15 +222,15 @@
             "words_count": item["total_wordage"]
         }
         result.append(item_data)
     return result
 
 
 def GetCollectionSubscribersInfo(collection_id: int, start_sort_id: int = None) -> List[Dict]:
-    """该函数接收一个专题 ID，并返回该 ID 对应专题的关注者信息
+    """获取专题关注者信息
 
     Args:
         collection_id (int): 专题 ID
         start_sort_id (int): 起始序号，等于上一条数据的序号
 
     Returns:
         List[Dict]: 关注者信息
@@ -228,29 +246,32 @@
             "subscribe_time": datetime.fromisoformat(item["subscribed_at"])
         }
         result.append(item_data)
     return result
 
 
 def GetCollectionArticlesInfo(collection_url: str, page: int = 1,
-                              count: int = 10, sorting_method: str = "time") -> List[Dict]:
-    """该函数接收专题 Url ，并返回该 Url 对应专题的文章信息
+                              count: int = 10, sorting_method: str = "time",
+                              disable_check: bool = False) -> List[Dict]:
+    """获取专题文章信息
 
     Args:
         collection_url (str): 专题 Url
         page (int, optional): 页码. Defaults to 1.
         count (int, optional): 每次返回的数据数量. Defaults to 10.
         sorting_method (str, optional): 排序方法，"time" 为按照发布时间排序，
         "comment_time" 为按照最近评论时间排序，"hot" 为按照热度排序. Defaults to "time".
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         List[Dict]: 文章信息
     """
-    AssertCollectionUrl(collection_url)
-    AssertCollectionStatusNormal(collection_url)
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     order_by = {
         "time": "added_at",
         "comment_time": "commented_at",
         "hot": "top"
     }[sorting_method]
     json_obj = GetCollectionArticlesJsonDataApi(CollectionUrlToCollectionSlug(collection_url),
                                                 page=page, count=count, order_by=order_by)
@@ -277,23 +298,27 @@
             "comments_count": item["object"]["data"]["public_comments_count"],
             "rewards_count": item["object"]["data"]["total_rewards_count"]
         }
         result.append(item_data)
     return result
 
 
-def GetCollectionAllBasicData(collection_url: str) -> Dict:
+def GetCollectionAllBasicData(collection_url: str, disable_check: bool = False) -> Dict:
     """获取专题的所有基础信息
 
     Args:
         collection_url (str): 专题 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
-        dict: 专题基础信息
+        Dict: 专题基础信息
     """
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     result = {}
     json_obj = GetCollectionJsonDataApi(collection_url)
 
     result["name"] = json_obj["title"]
     result["avatar_url"] = json_obj["image"]
     result["introduction_text"] = json_obj["content_without_html"]
     result["introduction_html"] = json_obj["content_in_full"]
@@ -305,86 +330,119 @@
         "uid": json_obj["owner"]["id"],
         "name": json_obj["owner"]["nickname"],
         "uslug": json_obj["owner"]["slug"]
     }
     return result
 
 
-def GetCollectionAllEditorsInfo(collection_id: int) -> Generator[List[Dict], None, None]:
+def GetCollectionAllEditorsInfo(collection_id: int, max_count: int = None) -> Generator[Dict, None, None]:
     """获取专题的所有编辑信息
 
     Args:
         collection_id (int): 专题 ID
+        max_count (int, optional): 获取的专题编辑信息数量上限，Defaults to None.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页编辑信息
+        Iterator[Dict], None, None]: 编辑信息
     """
     page = 1
+    now_count = 0
     while True:
         result = GetCollectionEditorsInfo(collection_id, page)
         if result:
-            yield result
             page += 1
         else:
-            break
+            return
+        for item in result:
+            yield item
+            if max_count:
+                now_count += 1
+                if now_count == max_count:
+                    return
 
 
-def GetCollectionAllRecommendedWritersInfo(collection_id: int, count: int = 20) -> Generator[List[Dict], None, None]:
+def GetCollectionAllRecommendedWritersInfo(collection_id: int, count: int = 20, max_count: int = None) -> Generator[Dict, None, None]:
     """获取专题的所有推荐作者信息
 
     Args:
         collection_id (int): 专题 ID
         count (int, optional): 单次获取的数据数量，会影响性能. Defaults to 20.
+        max_count (int, optional): 获取的专题推荐作者信息数量上限，Defaults to None.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页推荐作者信息
+        Iterator[Dict], None, None]: 推荐作者信息
     """
     page = 1
+    now_count = 0
     while True:
         result = GetCollectionRecommendedWritersInfo(collection_id, page, count)
         if result:
-            yield result
             page += 1
         else:
-            break
+            return
+        for item in result:
+            yield item
+            if max_count:
+                now_count += 1
+                if now_count == max_count:
+                    return
 
 
-def GetCollectionAllSubscribersInfo(collection_id: int) -> Generator[List[Dict], None, None]:
+def GetCollectionAllSubscribersInfo(collection_id: int, max_count: int = None) -> Generator[Dict, None, None]:
     """获取专题的所有关注者信息
 
     Args:
         collection_id (int): 专题 ID
+        max_count (int, optional): 获取的专题关注者信息数量上限，Defaults to None.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页关注者信息
+        Iterator[Dict], None, None]: 关注者信息
     """
     start_sort_id = None
+    now_count = 0
     while True:
         result = GetCollectionSubscribersInfo(collection_id, start_sort_id)
         if result:
-            yield result
             start_sort_id = result[-1]["sort_id"]
         else:
-            break
+            return
+        for item in result:
+            yield item
+            if max_count:
+                now_count += 1
+                if now_count == max_count:
+                    return
 
 
 def GetCollectionAllArticlesInfo(collection_url: str, count: int = 10,
-                                 sorting_method: str = "time") -> Generator[List[Dict], None, None]:
+                                 sorting_method: str = "time", max_count: int = None,
+                                 disable_check: bool = False) -> Generator[Dict, None, None]:
     """获取专题的所有文章信息
 
     Args:
         collection_url (str): 专题 Url
         count (int, optional): 单次获取的数据数量，会影响性能. Defaults to 10.
         sorting_method (str, optional): 排序方法，"time" 为按照发布时间排序，
         "comment_time" 为按照最近评论时间排序，"hot" 为按照热度排序. Defaults to "time".
+        max_count (int, optional): 获取的专题文章信息数量上限，Defaults to None.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页文章信息
+        Iterator[Dict], None, None]: 文章信息
     """
+    if not disable_check:
+        AssertCollectionUrl(collection_url)
+        AssertCollectionStatusNormal(collection_url)
     page = 1
+    now_count = 0
     while True:
-        result = GetCollectionArticlesInfo(collection_url, page, count, sorting_method)
+        result = GetCollectionArticlesInfo(collection_url, page, count, sorting_method, disable_check=True)
         if result:
-            yield result
             page += 1
         else:
-            break
+            return
+        for item in result:
+            yield item
+            if max_count:
+                now_count += 1
+                if now_count == max_count:
+                    return
```

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/convert.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/convert.py`

 * *Files identical despite different names*

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/headers.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/headers.py`

 * *Files identical despite different names*

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/island.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/island.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,145 +5,162 @@
                            AssertIslandUrl)
 from .basic_apis import (GetIslandJsonDataApi, GetIslandPostJsonDataApi,
                          GetIslandPostsJsonDataApi)
 from .convert import (IslandPostSlugToIslandPostUrl,
                       IslandPostUrlToIslandPostSlug, IslandUrlToIslandSlug)
 
 
-def GetIslandName(island_url: str) -> str:
+def GetIslandName(island_url: str, disable_check: bool = False) -> str:
     """获取小岛名称
 
     Args:
         island_url (str): 小岛 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 小岛名称
     """
-    AssertIslandUrl(island_url)
-    AssertIslandStatusNormal(island_url)
+    if not disable_check:
+        AssertIslandUrl(island_url)
+        AssertIslandStatusNormal(island_url)
     json_obj = GetIslandJsonDataApi(island_url)
     result = json_obj["name"]
     return result
 
 
-def GetIslandAvatarUrl(island_url: str) -> str:
+def GetIslandAvatarUrl(island_url: str, disable_check: bool = False) -> str:
     """获取小岛头像链接
 
     Args:
         island_url (str): 小岛 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 小岛头像链接
     """
-    AssertIslandUrl(island_url)
-    AssertIslandStatusNormal(island_url)
+    if not disable_check:
+        AssertIslandUrl(island_url)
+        AssertIslandStatusNormal(island_url)
     json_obj = GetIslandJsonDataApi(island_url)
     result = json_obj["image"]
     return result
 
 
-def GetIslandIntroduction(island_url: str) -> str:
+def GetIslandIntroduction(island_url: str, disable_check: bool = False) -> str:
     """获取小岛简介
 
     Args:
         island_url (str): 小岛 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 小岛简介
     """
-    AssertIslandUrl(island_url)
-    AssertIslandStatusNormal(island_url)
+    if not disable_check:
+        AssertIslandUrl(island_url)
+        AssertIslandStatusNormal(island_url)
     json_obj = GetIslandJsonDataApi(island_url)
     result = json_obj["intro"]
     return result
 
 
-def GetIslandMembersCount(island_url: str) -> int:
+def GetIslandMembersCount(island_url: str, disable_check: bool = False) -> int:
     """获取小岛成员数量
 
     Args:
         island_url (str): 小岛 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 成员数量
     """
-    AssertIslandUrl(island_url)
-    AssertIslandStatusNormal(island_url)
+    if not disable_check:
+        AssertIslandUrl(island_url)
+        AssertIslandStatusNormal(island_url)
     json_obj = GetIslandJsonDataApi(island_url)
     result = json_obj["members_count"]
     return result
 
 
-def GetIslandPostsCount(island_url: str) -> int:
+def GetIslandPostsCount(island_url: str, disable_check: bool = False) -> int:
     """获取小岛帖子数量
 
     Args:
         island_url (str): 小岛 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 帖子数量
     """
-    AssertIslandUrl(island_url)
-    AssertIslandStatusNormal(island_url)
+    if not disable_check:
+        AssertIslandUrl(island_url)
+        AssertIslandStatusNormal(island_url)
     json_obj = GetIslandJsonDataApi(island_url)
     result = json_obj["posts_count"]
     return result
 
 
-def GetIslandCategory(island_url: str) -> str:
+def GetIslandCategory(island_url: str, disable_check: bool = False) -> str:
     """获取小岛分类
 
     Args:
         island_url (str): 小岛 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 分类
     """
-    AssertIslandUrl(island_url)
-    AssertIslandStatusNormal(island_url)
+    if not disable_check:
+        AssertIslandUrl(island_url)
+        AssertIslandStatusNormal(island_url)
     json_obj = GetIslandJsonDataApi(island_url)
     result = json_obj["category"]["name"]
     return result
 
 
-def GetIslandPostFullConetnt(post_url: str) -> str:
+def GetIslandPostFullConetnt(post_url: str, disable_check: bool = False) -> str:
     """获取小岛帖子完整内容
 
     Args:
         island_url (str): 小岛 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 小岛帖子完整内容
     """
-    AssertIslandPostUrl(post_url)
-    AssertIslandStatusNormal(post_url)
+    if not disable_check:
+        AssertIslandPostUrl(post_url)
+        AssertIslandStatusNormal(post_url)
     json_obj = GetIslandPostJsonDataApi(IslandPostUrlToIslandPostSlug(post_url))
     result = json_obj["content"]
     return result
 
 
 def GetIslandPosts(island_url: str, start_sort_id: int = None, count: int = 10,
-                   topic_id: int = None, sorting_method: str = "time", get_full_content: bool = False) -> List[Dict]:
+                   topic_id: int = None, sorting_method: str = "time",
+                   get_full_content: bool = False, disable_check: bool = False) -> List[Dict]:
     """获取小岛帖子信息
 
         Args:
             island_url (str): 小岛 Url
             start_sort_id (int, optional): 起始序号，等于上一条数据的序号. Defaults to None.
             count (int, optional): 每次返回的数据数量. Defaults to 10.
             topic_id (int, optional): 话题 ID. Defaults to None.
             sorting_method (str, optional): 排序方法，"time" 为按照发布时间排序，
         "comment_time" 为按照最近评论时间排序，"hot" 为按照热度排序. Defaults to "time".
             get_full_content (bool, optional): 为 True 时，当检测到获取的帖子内容不全时，
         自动调用 GetIslandPostFullConetnt 函数获取完整内容并替换. Defaults to False.
+            disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
         Returns:
             List[Dict]: 帖子信息
     """
-    AssertIslandUrl(island_url)
-    AssertIslandStatusNormal(island_url)
+    if not disable_check:
+        AssertIslandUrl(island_url)
+        AssertIslandStatusNormal(island_url)
     order_by = {
         "time": "latest",
         "hot": "hot",
         "most_valuable": "best"
     }[sorting_method],
     json_obj = GetIslandPostsJsonDataApi(group_slug=IslandUrlToIslandSlug(island_url),
                                          max_id=start_sort_id, count=count, topic_id=topic_id, order_by=order_by)
@@ -200,58 +217,76 @@
                 "tslug": item["topic"]["slug"],
                 "topic_name": item["topic"]["name"]
                 # 有个 group_role 不知道干什么用的，没解析
             }
         except KeyError:
             pass  # 没有话题则跳过
         if get_full_content and "..." in item_data["content"]:  # 获取到的帖子内容不全
-            item_data["content"] = GetIslandPostFullConetnt(IslandPostSlugToIslandPostUrl(item_data["pslug"]))
+            item_data["content"] = GetIslandPostFullConetnt(IslandPostSlugToIslandPostUrl(item_data["pslug"]),
+                                                            disable_check=True)
         result.append(item_data)
     return result
 
 
-def GetIslandAllBasicData(island_url: str) -> Dict:
+def GetIslandAllBasicData(island_url: str, disable_check: bool = False) -> Dict:
     """获取小岛的所有基础信息
 
     Args:
         island_url (str): 小岛 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         Dict: 小岛基础信息
     """
+    if not disable_check:
+        AssertIslandPostUrl(island_url)
+        AssertIslandStatusNormal(island_url)
     result = {}
     json_obj = GetIslandJsonDataApi(island_url)
 
     result["name"] = json_obj["name"]
     result["avatar_url"] = json_obj["image"]
     result["introduction"] = json_obj["intro"]
     result["members_count"] = json_obj["members_count"]
     result["posts_count"] = json_obj["posts_count"]
     result["category"] = json_obj["category"]["name"]
     return result
 
 
 def GetIslandAllPostsData(island_url: str, count: int = 10,
                           topic_id: int = None, sorting_method: str = "time",
-                          get_full_content: bool = False) -> Generator[List[Dict], None, None]:
+                          get_full_content: bool = False, max_count: int = None,
+                          disable_check: bool = False) -> Generator[Dict, None, None]:
     """获取小岛的所有帖子信息
 
     Args:
         island_url (str): 小岛 Url
         count (int, optional): 单次获取的数据数量，会影响性能. Defaults to 10.
         topic_id (int, optional): 话题 ID. Defaults to None.
         sorting_method (str, optional): 排序方法，time 为按照发布时间排序，
         comment_time 为按照最近评论时间排序，hot 为按照热度排序. Defaults to "time".
         get_full_content (bool, optional): 为 True 时，当检测到获取的帖子内容不全时，
     自动调用 GetIslandPostFullConetnt 函数获取完整内容并替换. Defaults to False.
+        max_count (int, optional): 获取的小岛帖子信息数量上限，Defaults to None.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页帖子信息
+        Iterator[Dict], None, None]: 帖子信息
     """
+    if not disable_check:
+        AssertIslandUrl(island_url)
+        AssertIslandStatusNormal(island_url)
     start_sort_id = None
+    now_count = 0
     while True:
-        result = GetIslandPosts(island_url, start_sort_id, count, topic_id, sorting_method, get_full_content)
+        result = GetIslandPosts(island_url, start_sort_id, count, topic_id,
+                                sorting_method, get_full_content, disable_check=True)
         if result:
-            yield result
             start_sort_id = result[-1]["sorted_id"]
         else:
-            break
+            return
+        for item in result:
+            yield item
+            if max_count:
+                now_count += 1
+                if now_count == max_count:
+                    return
```

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/notebook.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/notebook.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,145 @@
 from datetime import datetime
 from typing import Dict, Generator, List
 
 from .assert_funcs import AssertNotebookStatusNormal, AssertNotebookUrl
 from .basic_apis import GetNotebookArticlesJsonDataApi, GetNotebookJsonDataApi
 
 
-def GetNotebookName(notebook_url: str) -> str:
+def GetNotebookName(notebook_url: str, disable_check: bool = False) -> str:
     """获取文集名称
 
     Args:
         notebook_url (str): 文集 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 文集名称
     """
-    AssertNotebookUrl(notebook_url)
-    AssertNotebookStatusNormal(notebook_url)
+    if not disable_check:
+        AssertNotebookUrl(notebook_url)
+        AssertNotebookStatusNormal(notebook_url)
     json_obj = GetNotebookJsonDataApi(notebook_url)
     result = json_obj["name"]
     return result
 
 
-def GetNotebookArticlesCount(notebook_url: str) -> int:
+def GetNotebookArticlesCount(notebook_url: str, disable_check: bool = False) -> int:
     """获取文集中的文章数量
 
     Args:
         notebook_url (str): 文集 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 文章数量
     """
-    AssertNotebookUrl(notebook_url)
-    AssertNotebookStatusNormal(notebook_url)
+    if not disable_check:
+        AssertNotebookUrl(notebook_url)
+        AssertNotebookStatusNormal(notebook_url)
     json_obj = GetNotebookJsonDataApi(notebook_url)
     result = json_obj["notes_count"]
     return result
 
 
-def GetNotebookAuthorInfo(notebook_url: str) -> Dict:
+def GetNotebookAuthorInfo(notebook_url: str, disable_check: bool = False) -> Dict:
     """获取文集作者的信息
 
     Args:
         notebook_url (str): 文集 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         Dict: 作者信息
     """
-    AssertNotebookUrl(notebook_url)
-    AssertNotebookStatusNormal(notebook_url)
+    if not disable_check:
+        AssertNotebookUrl(notebook_url)
+        AssertNotebookStatusNormal(notebook_url)
     json_obj = GetNotebookJsonDataApi(notebook_url)
     result = {
         "name": json_obj["user"]["nickname"],
         "uslug": json_obj["user"]["slug"],
         "avatar_url": json_obj["user"]["avatar"]
     }
     return result
 
 
-def GetNotebookWordage(notebook_url: str) -> int:
+def GetNotebookWordage(notebook_url: str, disable_check: bool = False) -> int:
     """获取文集中所有文章的总字数
 
     Args:
         notebook_url (str): 文集 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 文集中的文章总字数
     """
-    AssertNotebookUrl(notebook_url)
-    AssertNotebookStatusNormal(notebook_url)
+    if not disable_check:
+        AssertNotebookUrl(notebook_url)
+        AssertNotebookStatusNormal(notebook_url)
     json_obj = GetNotebookJsonDataApi(notebook_url)
     result = json_obj["wordage"]
     return result
 
 
-def GetNotebookSubscribersCount(notebook_url: str) -> int:
+def GetNotebookSubscribersCount(notebook_url: str, disable_check: bool = False) -> int:
     """获取文集的订阅者数量
 
     Args:
         notebook_url (str): 文集 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 文集订阅者数量
     """
-    AssertNotebookUrl(notebook_url)
-    AssertNotebookStatusNormal(notebook_url)
+    if not disable_check:
+        AssertNotebookUrl(notebook_url)
+        AssertNotebookStatusNormal(notebook_url)
     json_obj = GetNotebookJsonDataApi(notebook_url)
     result = json_obj["subscribers_count"]
     return result
 
 
-def GetNotebookUpdateTime(notebook_url: str) -> datetime:
+def GetNotebookUpdateTime(notebook_url: str, disable_check: bool = False) -> datetime:
     """获取文集的更新时间
 
     Args:
         notebook_url (str): 文集 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         datetime: 更新时间
     """
-    AssertNotebookUrl(notebook_url)
-    AssertNotebookStatusNormal(notebook_url)
+    if not disable_check:
+        AssertNotebookUrl(notebook_url)
+        AssertNotebookStatusNormal(notebook_url)
     json_obj = GetNotebookJsonDataApi(notebook_url)
     result = datetime.fromtimestamp(json_obj["last_updated_at"])
     return result
 
 
 def GetNotebookArticlesInfo(notebook_url: str, page: int = 1,
-                            count: int = 10, sorting_method: str = "time") -> List[Dict]:
+                            count: int = 10, sorting_method: str = "time",
+                            disable_check: bool = False) -> List[Dict]:
     """获取文集中的文章信息
 
     Args:
         notebook_url (str): 文集 Url
         page (int, optional): 页码. Defaults to 1.
         count (int, optional): 每次返回的数据数量. Defaults to 10.
         sorting_method (str, optional): 排序方法，"time" 为按照发布时间排序，
         "comment_time" 为按照最近评论时间排序，"hot" 为按照热度排序. Defaults to "time".
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         List[Dict]: 文章信息
     """
-    AssertNotebookUrl(notebook_url)
-    AssertNotebookStatusNormal(notebook_url)
+    if not disable_check:
+        AssertNotebookUrl(notebook_url)
+        AssertNotebookStatusNormal(notebook_url)
     order_by = {
         "time": "added_at",
         "comment_time": "commented_at",
         "hot": "top"
     }[sorting_method]
     json_obj = GetNotebookArticlesJsonDataApi(notebook_url=notebook_url,
                                               page=page, count=count, order_by=order_by)
@@ -152,25 +167,27 @@
             "comments_count": item["object"]["data"]["public_comments_count"],
             "rewards_count": item["object"]["data"]["total_rewards_count"]
         }
         result.append(item_data)
     return result
 
 
-def GetNotebookAllBasicData(notebook_url: str) -> Dict:
+def GetNotebookAllBasicData(notebook_url: str, disable_check: bool = False) -> Dict:
     """获取文集的所有基础信息
 
     Args:
         notebook_url (str): 文集 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         Dict: 文集基础信息
     """
-    AssertNotebookUrl(notebook_url)
-    AssertNotebookStatusNormal(notebook_url)
+    if not disable_check:
+        AssertNotebookUrl(notebook_url)
+        AssertNotebookStatusNormal(notebook_url)
     result = {}
     json_obj = GetNotebookJsonDataApi(notebook_url)
 
     result["name"] = json_obj["name"]
     result["author_info"] = {
         "name": json_obj["user"]["nickname"],
         "uslug": json_obj["user"]["slug"],
@@ -179,28 +196,39 @@
     result["articles_count"] = json_obj["notes_count"]
     result["wordage"] = json_obj["wordage"]
     result["subscribers_count"] = json_obj["subscribers_count"]
     result["update_time"] = datetime.fromtimestamp(json_obj["last_updated_at"])
     return result
 
 
-def GetNotebookAllArticlesInfo(notebook_url: str, count: int = 10,
-                               sorting_method: str = "time") -> Generator[List[Dict], None, None]:
+def GetNotebookAllArticlesInfo(notebook_url: str, count: int = 10, sorting_method: str = "time",
+                               max_count: int = None, disable_check: bool = False) -> Generator[Dict, None, None]:
     """获取文集中的全部文章信息
 
     Args:
         notebook_url (str): 文集 Url
         count (int, optional): 单次获取的数据数量，会影响性能. Defaults to 10.
         sorting_method (str, optional): 排序方法，time 为按照发布时间排序，
         comment_time 为按照最近评论时间排序，hot 为按照热度排序. Defaults to "time".
+        max_count (int, optional): 获取的文集文章信息数量上限，Defaults to None.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页文章信息
+        Iterator[Dict], None, None]: 文章信息
     """
+    if not disable_check:
+        AssertNotebookUrl(notebook_url)
+        AssertNotebookStatusNormal(notebook_url)
     page = 1
+    now_count = 0
     while True:
-        result = GetNotebookArticlesInfo(notebook_url, page, count, sorting_method)
+        result = GetNotebookArticlesInfo(notebook_url, page, count, sorting_method, disable_check=True)
         if result:
-            yield result
             page += 1
         else:
-            break
+            return
+        for item in result:
+            yield item
+            if max_count:
+                now_count += 1
+                if max_count == now_count:
+                    return
```

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/objects.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     @cache_result
     def name(self) -> str:
         """获取用户昵称
 
         Returns:
             str: 用户昵称
         """
-        return user.GetUserName(self._url)
+        return user.GetUserName(self._url, disable_check=True)
 
     @property
     @cache_result
     def gender(self) -> int:
         """获取用户性别
 
         Returns:
@@ -96,202 +96,202 @@
     @cache_result
     def followers_count(self) -> int:
         """获取用户关注数
 
         Returns:
             int: 关注数
         """
-        return user.GetUserFollowersCount(self._url)
+        return user.GetUserFollowersCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def fans_count(self) -> int:
         """获取用户粉丝数
 
         Returns:
             int: 粉丝数
         """
-        return user.GetUserFansCount(self._url)
+        return user.GetUserFansCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def articles_count(self) -> int:
         """获取用户文章数
 
         Returns:
             int: 文章数
         """
-        return user.GetUserArticlesCount(self._url)
+        return user.GetUserArticlesCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def wordage(self) -> int:
         """获取用户总字数
 
         Returns:
             int: 总字数
         """
-        return user.GetUserWordage(self._url)
+        return user.GetUserWordage(self._url, disable_check=True)
 
     @property
     @cache_result
     def likes_count(self) -> int:
         """获取用户被点赞数
 
         Returns:
             int: 被点赞数
         """
-        return user.GetUserLikesCount(self._url)
+        return user.GetUserLikesCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def assets_count(self) -> float:
         """获取用户资产量
 
         Returns:
             int: 资产量
         """
-        return user.GetUserAssetsCount(self._url)
+        return user.GetUserAssetsCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def FP_count(self) -> float:
         """获取用户简书钻数量
 
         Returns:
             int: 简书钻数量
         """
-        return user.GetUserFPCount(self._url)
+        return user.GetUserFPCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def FTN_count(self) -> float:
         """获取用户简书贝数量
 
         Returns:
             int: 简书贝数量
         """
-        return user.GetUserFTNCount(self._url)
+        return user.GetUserFTNCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def badges(self) -> List:
         """获取徽章列表
 
         Returns:
             List: 徽章列表
         """
-        return user.GetUserBadgesList(self._url)
+        return user.GetUserBadgesList(self._url, disable_check=True)
 
     @property
     @cache_result
     def last_update_time(self) -> datetime:
         """获取最近更新时间
 
         Returns:
             datetime: 最近更新时间
         """
-        return user.GetUserLastUpdateTime(self._url)
+        return user.GetUserLastUpdateTime(self._url, disable_check=True)
 
     @property
     @cache_result
     def VIP_info(self) -> Dict:
         """获取用户会员信息
 
         Returns:
             Dict: 会员信息
         """
-        return user.GetUserVIPInfo(self._url)
+        return user.GetUserVIPInfo(self._url, disable_check=True)
 
     @property
     @cache_result
     def introduction_text(self) -> str:
         """获取纯文本格式的用户简介
 
         Returns:
             str: 纯文本格式的用户简介
         """
-        return user.GetUserIntroductionText(self._url)
+        return user.GetUserIntroductionText(self._url, disable_check=True)
 
     @property
     @cache_result
     def introduction_html(self) -> str:
         """获取 Html 格式的用户简介
 
         Returns:
             str: Html 格式的用户简介
         """
-        return user.GetUserIntroductionHtml(self._url)
+        return user.GetUserIntroductionHtml(self._url, disable_check=True)
 
     @property
     @cache_result
     def notebooks(self) -> List:
         """获取用户文集信息
 
         Returns:
             List: 文集信息
         """
-        return user.GetUserNotebooksInfo(self._url)
+        return user.GetUserNotebooksInfo(self._url, disable_check=True)
 
     @property
     @cache_result
     def own_collections(self) -> List:
         """获取自己创建的专题信息
 
         Returns:
             List: 自己创建的专题信息
         """
-        return user.GetUserOwnCollectionsInfo(self._url)
+        return user.GetUserOwnCollectionsInfo(self._url, disable_check=True)
 
     @property
     @cache_result
     def manageable_collections(self) -> List:
         """获取用户有管理权的专题信息
 
         Returns:
             List: 有管理权的专题信息
         """
-        return user.GetUserManageableCollectionsInfo(self._url)
+        return user.GetUserManageableCollectionsInfo(self._url, disable_check=True)
 
     @cache_result
     def articles_info(self, page: int = 1, count: int = 10) -> List[Dict]:
         """获取文章信息
 
         Args:
             page (int, optional): 页码. Defaults to 1.
             count (int, optional): 每次获取的文章信息数量. Defaults to 1.
 
         Returns:
             List[Dict]: 文章信息
         """
-        return user.GetUserArticlesInfo(self._url, page, count)
+        return user.GetUserArticlesInfo(self._url, page, count, disable_check=True)
 
     @cache_result
     def followers_info(self, page: int = 1) -> List[Dict]:
         """获取关注者信息
 
         Args:
             page (int, optional): 页码. Defaults to 1.
 
         Returns:
             List[Dict]: 关注者信息
         """
-        return user.GetUserFollowersInfo(self._url, page)
+        return user.GetUserFollowersInfo(self._url, page, disable_check=True)
 
     @cache_result
     def fans_info(self, page: int = 1) -> List[Dict]:
         """获取粉丝信息
 
         Args:
             page (int, optional): 页码. Defaults to 1.
 
         Returns:
             List[Dict]: 粉丝信息
         """
-        return user.GetUserFansInfo(self._url, page)
+        return user.GetUserFansInfo(self._url, page, disable_check=True)
 
     def __eq__(self, other: object) -> bool:
         """判断是否是同一个用户
 
         Args:
             other (object): 另一个对象
 
@@ -376,165 +376,165 @@
     @cache_result
     def title(self) -> str:
         """获取文章标题
 
         Returns:
             str: 标题
         """
-        return article.GetArticleTitle(self._url)
+        return article.GetArticleTitle(self._url, disable_check=True)
 
     @property
     @cache_result
     def author_name(self) -> str:
         """获取文章作者名
 
         Returns:
             str: 作者名
         """
-        return article.GetArticleAuthorName(self._url)
+        return article.GetArticleAuthorName(self._url, disable_check=True)
 
     @property
     @cache_result
     def wordage(self) -> int:
         """获取文章总字数
 
         Returns:
             int: 总字数
         """
-        return article.GetArticleWordage(self._url)
+        return article.GetArticleWordage(self._url, disable_check=True)
 
     @property
     @cache_result
     def reads_count(self) -> int:
         """获取文章阅读量
 
         Returns:
             int: 阅读量
         """
-        return article.GetArticleReadsCount(self._url)
+        return article.GetArticleReadsCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def likes_count(self) -> int:
         """获取文章点赞量
 
         Returns:
             int: 文章点赞量
         """
-        return article.GetArticleLikesCount(self._url)
+        return article.GetArticleLikesCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def comments_count(self) -> int:
         """获取文章评论量
 
         Returns:
             int: 文章评论量
         """
-        return article.GetArticleCommentsCount(self._url)
+        return article.GetArticleCommentsCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def most_valuable_comments_count(self) -> int:
         """获取文章精选评论量
 
         Returns:
             int: 文章精选评论量
         """
-        return article.GetArticleMostValuableCommentsCount(self._url)
+        return article.GetArticleMostValuableCommentsCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def total_FP_count(self) -> float:
         """获取文章总获钻量
 
         Returns:
             int: 文章总获钻量
         """
-        return article.GetArticleTotalFPCount(self._url)
+        return article.GetArticleTotalFPCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def description(self) -> str:
         """获取文章摘要
 
         Returns:
             str: 文章摘要
         """
-        return article.GetArticleDescription(self._url)
+        return article.GetArticleDescription(self._url, disable_check=True)
 
     @property
     @cache_result
     def publish_time(self) -> datetime:
         """获取文章发布时间
 
         Returns:
             datetime: 文章发布时间
         """
-        return article.GetArticlePublishTime(self._url)
+        return article.GetArticlePublishTime(self._url, disable_check=True)
 
     @property
     @cache_result
     def update_time(self) -> datetime:
         """获取文章更新时间
 
         Returns:
             datetime: 文章更新时间
         """
-        return article.GetArticleUpdateTime(self._url)
+        return article.GetArticleUpdateTime(self._url, disable_check=True)
 
     @property
     @cache_result
     def paid_status(self) -> bool:
         """获取文章付费状态
 
         Returns:
             bool: 文章付费状态
         """
-        return article.GetArticlePaidStatus(self._url)
+        return article.GetArticlePaidStatus(self._url, disable_check=True)
 
     @property
     @cache_result
     def reprint_status(self) -> bool:
         """获取文章转载状态
 
         Returns:
             bool: 文章转载状态
         """
-        return article.GetArticleReprintStatus(self._url)
+        return article.GetArticleReprintStatus(self._url, disable_check=True)
 
     @property
     @cache_result
     def comment_status(self) -> bool:
         """获取文章评论状态
 
         Returns:
             bool: 文章评论状态
         """
-        return article.GetArticleCommentStatus(self._url)
+        return article.GetArticleCommentStatus(self._url, disable_check=True)
 
     @property
     @cache_result
     def html(self) -> str:
         """获取 Html 格式的文章内容
 
         Returns:
             str: Html 格式的文章内容
         """
-        return article.GetArticleHtml(self._url)
+        return article.GetArticleHtml(self._url, disable_check=True)
 
     @property
     @cache_result
     def text(self) -> str:
         """获取纯文本格式的文章内容
 
         Returns:
             str: 纯文本格式的文章内容
         """
-        return article.GetArticleText(self._url)
+        return article.GetArticleText(self._url, disable_check=True)
 
     def __eq__(self, other: object) -> bool:
         """判断是否是同一篇文章
 
         Args:
             other (object): 另一个对象
 
@@ -624,90 +624,90 @@
     @cache_result
     def name(self) -> str:
         """获取文集名称
 
         Returns:
             str: 文集名称
         """
-        return notebook.GetNotebookName(self._url)
+        return notebook.GetNotebookName(self._url, disable_check=True)
 
     @property
     @cache_result
     def articles_count(self) -> int:
         """获取文集中的文章总数
 
         Returns:
             int: 文章总数
         """
-        return notebook.GetNotebookArticlesCount(self._url)
+        return notebook.GetNotebookArticlesCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def author_name(self) -> str:
         """获取文集的作者名
 
         Returns:
             str: 作者名
         """
-        return notebook.GetNotebookAuthorInfo(self._url)["name"]
+        return notebook.GetNotebookAuthorInfo(self._url, disable_check=True)["name"]
 
     @property
     @cache_result
     def author_info(self) -> Dict:
         """获取文集的作者信息
 
         Returns:
             Dict: 作者信息
         """
-        return notebook.GetNotebookAuthorInfo(self._url)
+        return notebook.GetNotebookAuthorInfo(self._url, disable_check=True)
 
     @property
     @cache_result
     def wordage(self) -> int:
         """获取文集中所有文章的总字数
 
         Returns:
             int: 文集总字数
         """
-        return notebook.GetNotebookWordage(self._url)
+        return notebook.GetNotebookWordage(self._url, disable_check=True)
 
     @property
     @cache_result
     def subscribers_count(self) -> int:
         """获取文集的关注者数量
 
         Returns:
             int: 关注者数量
         """
-        return notebook.GetNotebookSubscribersCount(self._url)
+        return notebook.GetNotebookSubscribersCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def update_time(self) -> datetime:
         """获取文集的更新时间
 
         Returns:
             datetime: 更新时间
         """
-        return notebook.GetNotebookUpdateTime(self._url)
+        return notebook.GetNotebookUpdateTime(self._url, disable_check=True)
 
     @cache_result
     def articles_info(self, page: int = 1, count: int = 10, sorting_method: str = "time") -> List[Dict]:
         """获取文集中的文章信息
 
         Args:
             page (int, optional): 页码. Defaults to 1.
             count (int, optional): 每次返回的数据数量. Defaults to 10.
             sorting_method (str, optional): 排序方法，time 为按照发布时间排序，
             comment_time 为按照最近评论时间排序，hot 为按照热度排序. Defaults to "time".
 
         Returns:
             List[Dict]: 文章信息
         """
-        return notebook.GetNotebookArticlesInfo(self._url, page, count, sorting_method)
+        return notebook.GetNotebookArticlesInfo(self._url, page, count, sorting_method, disable_check=True)
 
     def __eq__(self, other: object) -> bool:
         """判断是否是同一个文集
 
         Args:
             other (object): 另一个对象
 
@@ -792,95 +792,95 @@
     @cache_result
     def name(self) -> str:
         """获取专题名称
 
         Returns:
             str: 专题名称
         """
-        return collection.GetCollectionName(self._url)
+        return collection.GetCollectionName(self._url, disable_check=True)
 
     @property
     @cache_result
     def avatar_url(self) -> str:
         """获取专题头像链接
 
         Returns:
             str: 专题头像链接
         """
-        return collection.GetCollectionAvatarUrl(self._url)
+        return collection.GetCollectionAvatarUrl(self._url, disable_check=True)
 
     @property
     @cache_result
     def introduction_text(self) -> str:
         """获取纯文本格式的专题简介
 
         Returns:
             str: 纯文本格式的专题简介
         """
-        return collection.GetCollectionIntroductionText(self._url)
+        return collection.GetCollectionIntroductionText(self._url, disable_check=True)
 
     @property
     @cache_result
     def introduction_html(self) -> str:
         """获取 Html 格式的专题简介
 
         Returns:
             str:  Html 格式的专题简介
         """
-        return collection.GetCollectionIntroductionHtml(self._url)
+        return collection.GetCollectionIntroductionHtml(self._url, disable_check=True)
 
     @property
     @cache_result
     def articles_update_time(self) -> datetime:
         """获取专题文章更新时间
 
         Returns:
             datetime: 专题文章更新时间
         """
-        return collection.GetCollectionArticlesUpdateTime(self._url)
+        return collection.GetCollectionArticlesUpdateTime(self._url, disable_check=True)
 
     @property
     @cache_result
     def info_update_time(self) -> datetime:
         """获取专题信息更新时间
 
         Returns:
             datetime: 专题信息更新时间
         """
-        return collection.GetCollectionInfoUpdateTime(self._url)
+        return collection.GetCollectionInfoUpdateTime(self._url, disable_check=True)
 
     @property
     @cache_result
     def owner_info(self) -> Dict:
         """获取专题的所有者信息
 
         Returns:
             Dict: 用户信息
         """
-        return collection.GetCollectionOwnerInfo(self._url)
+        return collection.GetCollectionOwnerInfo(self._url, disable_check=True)
 
     @property
     @cache_result
     def articles_count(self) -> int:
         """获取专题文章数
 
         Returns:
             int: 专题文章数
         """
-        return collection.GetCollectionArticlesCount(self._url)
+        return collection.GetCollectionArticlesCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def subscribers_count(self) -> int:
         """获取专题关注者数
 
         Returns:
             int: 专题关注者数
         """
-        return collection.GetCollectionSubscribersCount(self._url)
+        return collection.GetCollectionSubscribersCount(self._url, disable_check=True)
 
     @cache_result
     def editors_info(self, page: int = 1) -> List[Dict]:
         """获取专题编辑信息
 
         Args:
             page (int, optional): 页码. Defause to 1.
@@ -939,15 +939,15 @@
             count (int, optional): 每次返回的数据数量. Defaults to 10.
             sorting_method (str, optional): 排序方法，time 为按照发布时间排序，
             comment_time 为按照最近评论时间排序，hot 为按照热度排序. Defaults to "time".
 
         Returns:
             List[Dict]: 专题中的文章信息
         """
-        return collection.GetCollectionArticlesInfo(self._url, page, count, sorting_method)
+        return collection.GetCollectionArticlesInfo(self._url, page, count, sorting_method, disable_check=True)
 
     def __eq__(self, other: object) -> bool:
         """判断是否是同一个专题
 
         Args:
             other (object): 另一个对象
 
@@ -1021,65 +1021,65 @@
     @cache_result
     def name(self) -> str:
         """获取小岛名称
 
         Returns:
             str: 小岛名称
         """
-        return island.GetIslandName(self._url)
+        return island.GetIslandName(self._url, disable_check=True)
 
     @property
     @cache_result
     def avatar_url(self) -> str:
         """获取小岛头像链接
 
         Returns:
             str: 小岛头像链接
         """
-        return island.GetIslandAvatarUrl(self._url)
+        return island.GetIslandAvatarUrl(self._url, disable_check=True)
 
     @property
     @cache_result
     def introduction(self) -> str:
         """获取小岛简介
 
         Returns:
             str: 小岛简介
         """
-        return island.GetIslandIntroduction(self._url)
+        return island.GetIslandIntroduction(self._url, disable_check=True)
 
     @property
     @cache_result
     def members_count(self) -> int:
         """获取小岛成员数量
 
         Returns:
             int: 成员数量
         """
-        return island.GetIslandMembersCount(self._url)
+        return island.GetIslandMembersCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def posts_count(self) -> int:
         """获取小岛帖子数量
 
         Returns:
             int: 帖子数量
         """
-        return island.GetIslandPostsCount(self._url)
+        return island.GetIslandPostsCount(self._url, disable_check=True)
 
     @property
     @cache_result
     def category(self) -> str:
         """获取小岛分类
 
         Returns:
             str: 分类
         """
-        return island.GetIslandCategory(self._url)
+        return island.GetIslandCategory(self._url, disable_check=True)
 
     @cache_result
     def posts(self, start_sort_id: int = None, count: int = 10,
               topic_id: int = None, sorting_method: str = "time") -> List[Dict]:
         """获取小岛帖子信息
 
         Args:
@@ -1088,15 +1088,15 @@
             topic_id (int, optional): 话题 ID. Defaults to None.
             sorting_method (str, optional): 排序方法，time 为按照发布时间排序，
             comment_time 为按照最近评论时间排序，hot 为按照热度排序. Defaults to "time".
 
         Returns:
             List[Dict]: 帖子信息
         """
-        return island.GetIslandPosts(self._url, start_sort_id, count, topic_id, sorting_method)
+        return island.GetIslandPosts(self._url, start_sort_id, count, topic_id, sorting_method, disable_check=True)
 
     def __eq__(self, other: object) -> bool:
         """判断是否是同一个小岛
 
         Args:
             other (object): 另一个对象
```

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/rank.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/rank.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             "name": item["user"]["nickname"],
             "avatar_url": item["user"]["avatar"],
             "FP": item["amount"] / 1000
         }
         if get_full:
             user_url = UserSlugToUserUrl(item_data["uslug"])
             try:
-                item_data["Assets"] = GetUserAssetsCount(user_url)
+                item_data["Assets"] = GetUserAssetsCount(user_url, disable_check=True)
                 item_data["FTN"] = round(item_data["Assets"] - item_data["FP"], 3)  # 处理浮点数精度问题
             except APIError:
                 pass
         result.append(item_data)
     return result
```

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools/user.py` & `JianshuResearchTools-2.9.0/JianshuResearchTools/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,242 +13,267 @@
                          GetUserPCHtmlDataApi, GetUserTimelineHtmlDataApi)
 from .convert import (ArticleSlugToArticleUrl, CollectionSlugToCollectionUrl,
                       NotebookSlugToNotebookUrl, UserSlugToUserUrl,
                       UserUrlToUserSlug)
 from .exceptions import APIError
 
 
-def GetUserName(user_url: str) -> str:
+def GetUserName(user_url: str, disable_check: bool = False) -> str:
     """获取用户昵称
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 用户昵称
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     result = json_obj["nickname"]
     return result
 
 
-def GetUserGender(user_url: str) -> int:
+def GetUserGender(user_url: str, disable_check: bool = False) -> int:
     """获取用户性别
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 用户性别，0 为未知，1 为男，2 为女
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     result = json_obj["gender"]
     if result == 3:  # 某些未设置性别的账号性别值为 3，怀疑为简书系统遗留问题
         result = 0  # 3 也代表性别未知
     return result
 
 
-def GetUserFollowersCount(user_url: str) -> int:
+def GetUserFollowersCount(user_url: str, disable_check: bool = False) -> int:
     """获取用户关注人数
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 用户关注人数
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     result = json_obj["following_users_count"]
     return result
 
 
-def GetUserFansCount(user_url: str) -> int:
+def GetUserFansCount(user_url: str, disable_check: bool = False) -> int:
     """获取用户粉丝数
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 用户粉丝数
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     result = json_obj["followers_count"]
     return result
 
 
-def GetUserArticlesCount(user_url: str) -> int:
+def GetUserArticlesCount(user_url: str, disable_check: bool = False) -> int:
     """获取用户文章数
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 用户文章数
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     html_obj = GetUserPCHtmlDataApi(user_url)
     result = html_obj.xpath("//div[@class='info']/ul/li[3]/div[@class='meta-block']/a/p")[0].text
     result = int(result)
     return result
 
 
-def GetUserWordage(user_url: str) -> int:
+def GetUserWordage(user_url: str, disable_check: bool = False) -> int:
     """获取用户文章总字数
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 用户文章总字数
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     result = json_obj["total_wordage"]
     return result
 
 
-def GetUserLikesCount(user_url: str) -> int:
+def GetUserLikesCount(user_url: str, disable_check: bool = False) -> int:
     """获取用户被喜欢数
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         int: 用户被喜欢数
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     result = json_obj["total_likes_count"]
     return result
 
 
-def GetUserAssetsCount(user_url: str) -> float:
+def GetUserAssetsCount(user_url: str, disable_check: bool = False) -> float:
     """获取用户总资产
 
     # ! 当用户资产大于 10000 时，结果的精确度将下降到 1000
     # ! 当用户没有文章时，该函数将抛出 APIError 异常
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Raises:
         APIError: 由于用户没有文章导致无法获取总资产信息时抛出此异常
 
     Returns:
         float: 用户总资产
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     html_obj = GetUserPCHtmlDataApi(user_url)
     try:
         result = html_obj.xpath("//div[@class='info']/ul/li[6]/div[@class='meta-block']/p")[0].text
     except IndexError:
         raise APIError("受 API 限制（用户无文章时无法获取总资产信息），无法获取该用户的总资产")
     result = float(result.replace(".", "").replace("w", "000"))
     return result
 
 
-def GetUserFPCount(user_url: str) -> float:
+def GetUserFPCount(user_url: str, disable_check: bool = False) -> float:
     """获取用户简书钻数量
 
     # ! 当用户没有文章时，该函数将抛出 APIError 异常
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Raises:
         APIError: 由于用户没有文章导致无法获取总资产信息时抛出此异常
 
     Returns:
         float: 用户简书钻数量
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     result = json_obj["jsd_balance"] / 1000
     if json_obj["total_wordage"] == 0 and result == 0:
         raise APIError("受 API 限制（用户无文章时无法获取总资产信息），无法获取该用户的简书钻数量")
     return result
 
 
-def GetUserFTNCount(user_url: str) -> float:
+def GetUserFTNCount(user_url: str, disable_check: bool = False) -> float:
     """获取用户简书贝数量
 
     # ! 视用户资产配置情况不同，该函数获取到的数值会有不大于 1000 的偏差
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         float: 用户简书贝数量
     """
     assets = GetUserAssetsCount(user_url)
     FTN = GetUserFPCount(user_url)
     result = assets - FTN
     result = abs(result)  # 处理用户简书贝数量较少导致结果为负的情况
     result = round(result, 3)  # 处理浮点数精度问题
     return result
 
 
-def GetUserBadgesList(user_url: str) -> List[str]:
+def GetUserBadgesList(user_url: str, disable_check: bool = False) -> List[str]:
     """获取用户徽章列表
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         List[str]: 用户徽章列表
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     html_obj = GetUserPCHtmlDataApi(user_url)
     result = html_obj.xpath("//li[@class='badge-icon']/a/text()")
     result = [item.replace(" ", "").replace("\n", "") for item in result]  # 移除空格和换行符
     result = [item for item in result if item != ""]  # 去除空值
     return result
 
 
-def GetUserLastUpdateTime(user_url: str) -> datetime:
+def GetUserLastUpdateTime(user_url: str, disable_check: bool = False) -> datetime:
     """获取用户文章最后更新时间
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         datetime: 用户文章最后更新时间
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     result = datetime.fromtimestamp(json_obj["last_updated_at"])
     return result
 
 
-def GetUserVIPInfo(user_url: str) -> Dict:
+def GetUserVIPInfo(user_url: str, disable_check: bool = False) -> Dict:
     """获取用户会员信息
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         Dict: 用户会员信息
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     try:
         result = {
             "vip_type": {
                 "bronze": "铜牌",
                 "silver": "银牌",
                 "gold": "黄金",
@@ -260,158 +285,172 @@
         result = {
             "vip_type": None,
             "expire_date": None
         }
     return result
 
 
-def GetUserIntroductionHtml(user_url: str) -> str:
+def GetUserIntroductionHtml(user_url: str, disable_check: bool = False) -> str:
     """获取 Html 格式的用户简介
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: Html 格式的用户个人简介
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     result = json_obj["intro"]
     return result
 
 
-def GetUserIntroductionText(user_url: str) -> str:
+def GetUserIntroductionText(user_url: str, disable_check: bool = False) -> str:
     """获取纯文本格式的用户简介
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         str: 纯文本格式的用户个人简介
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserJsonDataApi(user_url)
     if json_obj["intro"] == "":   # 简介为空
         return ""
     html_obj = etree.HTML(json_obj["intro"])
     result = html_obj.xpath("//*/text()")
     result = "\n".join(result)
     return result
 
 
-def GetUserNextAnniversaryDay(user_url: str) -> datetime:
+def GetUserNextAnniversaryDay(user_url: str, disable_check: bool = False) -> datetime:
     """获取用户的下一次简书周年纪念日
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         datetime: 用户的下一次简书周年纪念日
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     user_slug = UserUrlToUserSlug(user_url)
     html_obj = GetUserNextAnniversaryDayHtmlDataApi(user_slug)
     result = html_obj.xpath('//*[@id="app"]/div[1]/div/text()')[0]
     result = findall(r"\d+", result)
     result = datetime.fromisoformat("-".join(result))
     return result
 
 
-def GetUserNotebooksInfo(user_url: str) -> List[Dict]:
+def GetUserNotebooksInfo(user_url: str, disable_check: bool = False) -> List[Dict]:
     """获取用户文集与连载信息
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         List[Dict]: 用户文集与连载信息
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserCollectionsAndNotebooksJsonDataApi(user_url=user_url, user_slug=UserUrlToUserSlug(user_url))
     result = []
     for item in json_obj["notebooks"]:
         item_data = {
             "nid": item["id"],
             "name": item["name"],
             "is_book": item["book"]
         }
         if item["book"]:
             item_data["is_paid_book"] = item["paid_book"]  # 如果是连载，则判断是否是付费连载
         result.append(item_data)
     return result
 
 
-def GetUserOwnCollectionsInfo(user_url: str) -> List[Dict]:
+def GetUserOwnCollectionsInfo(user_url: str, disable_check: bool = False) -> List[Dict]:
     """获取用户自己创建的专题信息
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         List[Dict]: 用户自己创建的专题信息
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserCollectionsAndNotebooksJsonDataApi(user_url=user_url, user_slug=UserUrlToUserSlug(user_url))
     result = []
     for item in json_obj["own_collections"]:
         item_data = {
             "cid": item["id"],
             "cslug": item["slug"],
             "name": item["title"],
             "avatar_url": item["avatar"]
         }
         result.append(item_data)
     return result
 
 
-def GetUserManageableCollectionsInfo(user_url: str) -> List[Dict]:
+def GetUserManageableCollectionsInfo(user_url: str, disable_check: bool = False) -> List[Dict]:
     """获取用户管理的专题信息
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         List[Dict]: 用户管理的专题信息
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     json_obj = GetUserCollectionsAndNotebooksJsonDataApi(user_url=user_url, user_slug=UserUrlToUserSlug(user_url))
     result = []
     for item in json_obj["manageable_collections"]:
         item_data = {
             "cid": item["id"],
             "cslug": item["slug"],
             "name": item["title"],
             "avatar_url": item["avatar"]
         }
         result.append(item_data)
     return result
 
 
 def GetUserArticlesInfo(user_url: str, page: int = 1, count: int = 10,
-                        sorting_method: str = "time") -> List[Dict]:
+                        sorting_method: str = "time", disable_check: bool = False) -> List[Dict]:
     """获取用户文章信息
 
     Args:
         user_url (str): 用户个人主页 Url
         page (int, optional): 页码，与网页端文章顺序相同. Defaults to 1.
         count (int, optional): 获取的文章数量. Defaults to 10.
         sorting_method (str, optional): 排序方法，time 为按照发布时间排序，
         comment_time 为按照最近评论时间排序，hot 为按照热度排序. Defaults to "time".
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         List[Dict]: 用户文章信息
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     order_by = {
         "time": "added_at",
         "comment_time": "commented_at",
         "hot": "top"
     }[sorting_method]
     json_obj = GetUserArticlesListJsonDataApi(user_url=user_url, page=page,
                                               count=count, order_by=order_by)
@@ -439,26 +478,28 @@
             "comments_count": item["object"]["data"]["public_comments_count"],
             "rewards_count": item["object"]["data"]["total_rewards_count"]
         }
         result.append(item_data)
     return result
 
 
-def GetUserFollowingInfo(user_url: str, page: int = 1) -> List[Dict]:
+def GetUserFollowingInfo(user_url: str, disable_check: bool = False, page: int = 1) -> List[Dict]:
     """获取用户关注者信息
 
     Args:
         user_url (str): 用户个人主页 Url
         page (int, optional): 关注列表页码. Defaults to 1.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         List[Dict]: 用户关注者信息
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     html_obj = GetUserFollowingListHtmlDataApi(user_url=user_url, page=page)
     name_raw_data = html_obj.xpath("//a[@class='name']")[1:]
     if not name_raw_data:  # 判断该页数据是否为空
         return []
     followers_raw_data = html_obj.xpath("//div[@class='meta'][1]/span[1]")
     fans_raw_data = html_obj.xpath("//div[@class='meta'][1]/span[2]")
     articles_raw_data = html_obj.xpath("//div[@class='meta'][1]/span[3]")
@@ -473,26 +514,28 @@
             "words_count": int(findall(r"\d+", words_and_likes_raw_data[index].text)[0]),   # TODO: 重复运行正则匹配，影响效率，需要优化
             "likes_count": int(findall(r"\d+", words_and_likes_raw_data[index].text)[1])
         }
         result.append(item_data)
     return result
 
 
-def GetUserFansInfo(user_url: str, page: int = 1) -> List[Dict]:
+def GetUserFansInfo(user_url: str, page: int = 1, disable_check: bool = False) -> List[Dict]:
     """获取用户粉丝信息
 
     Args:
         user_url (str): 用户个人主页 Url
         page (int, optional): 粉丝列表页码. Defaults to 1.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         List[Dict]: 用户粉丝信息
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     html_obj = GetUserFollowersListHtmlDataApi(user_url=user_url, page=page)
     name_raw_data = html_obj.xpath("//a[@class='name']")[1:]
     if not name_raw_data:  # 判断该页数据是否为空
         return []
     followers_raw_data = html_obj.xpath("//div[@class='meta'][1]/span[1]")
     fans_raw_data = html_obj.xpath("//div[@class='meta'][1]/span[2]")
     articles_raw_data = html_obj.xpath("//div[@class='meta'][1]/span[3]")
@@ -507,24 +550,27 @@
             "words_count": int(findall(r"\d+", words_and_likes_raw_data[index].text)[0]),   # TODO: 重复运行正则匹配，影响效率，需要优化
             "likes_count": int(findall(r"\d+", words_and_likes_raw_data[index].text)[1])
         }
         result.append(item_data)
     return result
 
 
-def GetUserAllBasicData(user_url: str) -> Dict:
+def GetUserAllBasicData(user_url: str, disable_check: bool = False) -> Dict:
     """获取用户的所有基础信息
 
     Args:
         user_url (str): 用户个人主页 Url
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
         Dict: 用户基础信息
     """
-
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     result = {}
     json_obj = GetUserJsonDataApi(user_url)
     html_obj = GetUserPCHtmlDataApi(user_url)
     anniversary_day_html_obj = GetUserNextAnniversaryDayHtmlDataApi(UserUrlToUserSlug(user_url))
 
     result["name"] = json_obj["nickname"]
     result["url"] = user_url
@@ -574,28 +620,30 @@
     else:
         result["introduction_text"] = "\n".join(etree.HTML(result["introduction_html"]).xpath("//*/text()"))
     result["next_anniversary_day"] = anniversary_day_html_obj.xpath('//*[@id="app"]/div[1]/div/text()')[0]
     result["next_anniversary_day"] = datetime.fromisoformat("-".join(findall(r"\d+", result["next_anniversary_day"])))
     return result
 
 
-def GetUserTimelineInfo(user_url: str, max_id: int = 1000000000) -> List[Dict]:
+def GetUserTimelineInfo(user_url: str, disable_check: bool = False, max_id: int = 1000000000) -> List[Dict]:
     """获取用户动态信息
 
     ！在极少数情况下可能会遇到不在可解析列表中的动态类型，此时程序会跳过这条动态，不会抛出异常
 
     Args:
         user_url (str): 用户个人主页 Url
         max_id (int, optional): 最大 id，值等于上一次获取到的数据中最后一项的 operation_id. Defaults to 1000000000.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Returns:
-        List[Dict]: [description]
+        List[Dict]: 用户动态信息
     """
-    AssertUserUrl(user_url)
-    AssertUserStatusNormal(user_url)
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     user_slug = UserUrlToUserSlug(user_url)
     html_obj = GetUserTimelineHtmlDataApi(user_slug, max_id)
     blocks = [x.__copy__() for x in html_obj.xpath("//li[starts-with(@id, 'feed-')]")]
     result = []
 
     for block in blocks:
         item_data = {}
@@ -739,87 +787,129 @@
             item_data["operator_url"] = UserSlugToUserUrl(block.xpath("//a[@class='nickname']/@href")[0][4:])
             item_data["operator_avatar_url"] = block.xpath("//a[@class='avatar']/img/@src")[0]
 
         result.append(item_data)
     return result
 
 
-def GetUserAllArticlesInfo(user_url: str, count: int = 10, sorting_method: str = "time") -> Generator[List[Dict], None, None]:
+def GetUserAllArticlesInfo(user_url: str, count: int = 10, sorting_method: str = "time",
+                           max_count: int = None, disable_check: bool = False) -> Generator[Dict, None, None]:
     """获取用户的所有文章信息
 
     Args:
         user_url (str): 用户个人主页 Url
         count (int, optional): 单次获取的数据数量，会影响性能. Defaults to 10.
         sorting_method (str, optional): 排序方法，time 为按照发布时间排序，
         comment_time 为按照最近评论时间排序，hot 为按照热度排序. Defaults to "time".
+        max_count (int, optional): 获取的文章信息数量上限，Defaults to None.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页文章信息
+        Iterator[Dict], None, None]: 文章信息
     """
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     page = 1
+    now_count = 0
     while True:
-        result = GetUserArticlesInfo(user_url, page, count, sorting_method)
+        result = GetUserArticlesInfo(user_url, page, count, sorting_method, disable_check=True)
         if result:
-            yield result
             page += 1
-        else:
-            break
+        else:  # 没有新的数据
+            return
+        for item in result:
+            yield item
+            if max_count:  # 如果有上限
+                now_count += 1
+                if now_count == max_count:  # 达到上限
+                    return
 
 
-def GetUserAllFollowingInfo(user_url: str) -> Generator[List[Dict], None, None]:
+def GetUserAllFollowingInfo(user_url: str, max_count: int = None, disable_check: bool = False) -> Generator[Dict, None, None]:
     """获取用户的所有关注者信息
 
     Args:
         user_url (str): 用户个人主页 Url
+        max_count (int, optional): 获取的关注者信息数量上限，Defaults to None.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页关注者信息
+        Iterator[Dict], None, None]: 关注者信息
     """
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     page = 1
+    now_count = 0
     while True:
-        result = GetUserFollowingInfo(user_url, page)
+        result = GetUserFollowingInfo(user_url, page, disable_check=True)
         if result:
-            yield result
             page += 1
         else:
-            break
+            return
+        for item in result:
+            yield item
+            if max_count:
+                now_count += 1
+                if now_count == max_count:
+                    return
 
 
-def GetUserAllFansInfo(user_url: str) -> Generator[List[Dict], None, None]:
+def GetUserAllFansInfo(user_url: str, max_count: int = None, disable_check: bool = False) -> Generator[Dict, None, None]:
     """获取用户的所有粉丝信息
 
     Args:
         user_url (str): 用户个人主页 Url
+        max_count (int, optional): 获取的粉丝信息数量上限，Defaults to None.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页粉丝信息
+        Iterator[Dict], None, None]: 粉丝信息
     """
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     page = 1
+    now_count = 0
     while True:
-        result = GetUserFansInfo(user_url, page)
+        result = GetUserFansInfo(user_url, page, disable_check=True)
         if result:
-            yield result
             page += 1
         else:
-            break
+            return
+        for item in result:
+            yield item
+            if max_count:
+                now_count += 1
+                if now_count == max_count:
+                    return
 
 
-def GetUserAllTimelineInfo(user_url: str) -> Generator[List[Dict], None, None]:
+def GetUserAllTimelineInfo(user_url: str, max_count: int = None, disable_check: bool = False) -> Generator[Dict, None, None]:
     """获取用户的所有动态信息
 
     Args:
         user_url (str): 用户个人主页 Url
+        max_count (int, optional): 获取的动态信息数量上限，Defaults to None.
+        disable_check (bool): 禁用参数有效性检查. Defaults to False.
 
     Yields:
-        Iterator[List[Dict], None, None]: 当前页动态信息
+        Iterator[Dict], None, None]: 动态信息
     """
+    if not disable_check:
+        AssertUserUrl(user_url)
+        AssertUserStatusNormal(user_url)
     max_id = None
+    now_count = 0
     while True:
-        if max_id:
-            result = GetUserTimelineInfo(user_url, max_id)
-        else:
-            result = GetUserTimelineInfo(user_url)
-        if not result:
-            break
-        else:
-            yield result
+        result = GetUserTimelineInfo(user_url, max_id, disable_check=True)
+        if result:
             max_id = result[-1]["operation_id"]
+        else:
+            return
+        for item in result:
+            yield item
+            if max_count:
+                now_count += 1
+                if now_count == max_count:
+                    return
```

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools.egg-info/PKG-INFO` & `JianshuResearchTools-2.9.0/JianshuResearchTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JianshuResearchTools
-Version: 2.8.0
+Version: 2.9.0
 Summary: 科技赋能创作星辰
 Home-page: https://github.com/FHU-yezi/JianshuResearchTools
 Author: FHU-yezi
 Author-email: yehaowei20060411@qq.com
 License: UNKNOWN
 Description: # 项目简介
```

### Comparing `JianshuResearchTools-2.8.0/JianshuResearchTools.egg-info/SOURCES.txt` & `JianshuResearchTools-2.9.0/JianshuResearchTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JianshuResearchTools-2.8.0/LICENSE` & `JianshuResearchTools-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JianshuResearchTools-2.8.0/PKG-INFO` & `JianshuResearchTools-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JianshuResearchTools
-Version: 2.8.0
+Version: 2.9.0
 Summary: 科技赋能创作星辰
 Home-page: https://github.com/FHU-yezi/JianshuResearchTools
 Author: FHU-yezi
 Author-email: yehaowei20060411@qq.com
 License: UNKNOWN
 Description: # 项目简介
```

### Comparing `JianshuResearchTools-2.8.0/setup.py` & `JianshuResearchTools-2.9.0/setup.py`

 * *Files identical despite different names*

