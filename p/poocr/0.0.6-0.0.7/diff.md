# Comparing `tmp/poocr-0.0.6.tar.gz` & `tmp/poocr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poocr-0.0.6.tar", last modified: Tue Apr 18 14:51:13 2023, max compression
+gzip compressed data, was "poocr-0.0.7.tar", last modified: Tue Apr 18 16:21:14 2023, max compression
```

## Comparing `poocr-0.0.6.tar` & `poocr-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 14:51:13.875676 poocr-0.0.6/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4588 2023-04-18 14:51:13.875676 poocr-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4067 2023-04-02 05:09:27.000000 poocr-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 14:51:13.829455 poocr-0.0.6/poocr/
--rw-rw-rw-   0        0        0      523 2023-03-25 11:20:01.000000 poocr-0.0.6/poocr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:51:13.858444 poocr-0.0.6/poocr/api/
--rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.6/poocr/api/__init__.py
--rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.6/poocr/api/ocr.py
--rw-rw-rw-   0        0        0     3259 2023-04-18 14:46:51.000000 poocr-0.0.6/poocr/api/ocr2excel.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:51:13.863423 poocr-0.0.6/poocr/core/
--rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.6/poocr/core/OCR.py
--rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.6/poocr/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:51:13.869656 poocr-0.0.6/poocr/lib/
--rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.6/poocr/lib/CommonUtils.py
--rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.6/poocr/lib/Config.py
--rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.6/poocr/lib/Const.py
--rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.6/poocr/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:51:13.851421 poocr-0.0.6/poocr.egg-info/
--rw-rw-rw-   0        0        0     4588 2023-04-18 14:51:13.000000 poocr-0.0.6/poocr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-04-18 14:51:13.000000 poocr-0.0.6/poocr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 14:51:13.000000 poocr-0.0.6/poocr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-18 14:43:22.000000 poocr-0.0.6/poocr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       40 2023-04-18 14:51:13.000000 poocr-0.0.6/poocr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-18 14:51:13.000000 poocr-0.0.6/poocr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      732 2023-04-18 14:51:13.877962 poocr-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 14:51:13.873673 poocr-0.0.6/tests/
--rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0      823 2023-04-16 09:36:45.000000 poocr-0.0.6/tests/test_tencent.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.121553 poocr-0.0.7/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 poocr-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4115 2023-04-18 16:21:14.121553 poocr-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3594 2023-04-18 15:02:36.000000 poocr-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.078671 poocr-0.0.7/poocr/
+-rw-rw-rw-   0        0        0      522 2023-04-18 16:20:50.000000 poocr-0.0.7/poocr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.103478 poocr-0.0.7/poocr/api/
+-rw-rw-rw-   0        0        0      265 2023-03-25 11:08:27.000000 poocr-0.0.7/poocr/api/__init__.py
+-rw-rw-rw-   0        0        0    20975 2023-01-30 12:39:04.000000 poocr-0.0.7/poocr/api/ocr.py
+-rw-rw-rw-   0        0        0     3259 2023-04-18 14:46:51.000000 poocr-0.0.7/poocr/api/ocr2excel.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.107488 poocr-0.0.7/poocr/core/
+-rw-rw-rw-   0        0        0     4071 2023-01-30 12:39:04.000000 poocr-0.0.7/poocr/core/OCR.py
+-rw-rw-rw-   0        0        0      223 2023-01-22 06:56:13.000000 poocr-0.0.7/poocr/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.116026 poocr-0.0.7/poocr/lib/
+-rw-rw-rw-   0        0        0     1017 2023-01-28 13:49:56.000000 poocr-0.0.7/poocr/lib/CommonUtils.py
+-rw-rw-rw-   0        0        0     1132 2023-01-30 12:39:04.000000 poocr-0.0.7/poocr/lib/Config.py
+-rw-rw-rw-   0        0        0      852 2023-01-30 12:39:04.000000 poocr-0.0.7/poocr/lib/Const.py
+-rw-rw-rw-   0        0        0        0 2023-01-22 10:20:33.000000 poocr-0.0.7/poocr/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.097426 poocr-0.0.7/poocr.egg-info/
+-rw-rw-rw-   0        0        0     4115 2023-04-18 16:21:13.000000 poocr-0.0.7/poocr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-04-18 16:21:13.000000 poocr-0.0.7/poocr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 16:21:13.000000 poocr-0.0.7/poocr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 16:20:22.000000 poocr-0.0.7/poocr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-04-18 16:21:13.000000 poocr-0.0.7/poocr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-18 16:21:13.000000 poocr-0.0.7/poocr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      741 2023-04-18 16:21:14.124546 poocr-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 poocr-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 16:21:14.119027 poocr-0.0.7/tests/
+-rw-rw-rw-   0        0        0      181 2023-01-30 12:39:04.000000 poocr-0.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      823 2023-04-16 09:36:45.000000 poocr-0.0.7/tests/test_tencent.py
```

### Comparing `poocr-0.0.6/LICENSE` & `poocr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `poocr-0.0.6/PKG-INFO` & `poocr-0.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poocr
-Version: 0.0.6
+Version: 0.0.7
 Summary: pip install poocr
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
@@ -47,15 +47,15 @@
 ## 📚简介
 
 
 poocr 是快速调用腾讯云AI平台功能的接口合集。
 
 ``poocr``所有功能的实现，都依托于腾讯云的文字识别，如果是小白用户，可以**扫码下图，免费开通**~
 
-![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/poocr%2Fapi-doc%2Fshare.jpg)
+![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/potencent%2Fapi-doc%2Fshare.jpg)
 
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
@@ -64,40 +64,34 @@
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
 
-[📘官网：https://www.python-office.com/](https://www.python-office.com/)
+- [📘官网：https://www.python-office.com/](https://www.python-office.com/)
 
-## 💻所有功能的列表👉[点我直达](https://mp.weixin.qq.com/s/WxICBZZSgkm-OrvXB82hbg)
+-  💻所有功能的列表👉[点我直达](https://www.python-office.com/video/poocr.html)
 
-## 🏗️添砖加瓦
 
+## 常见问题
 
-### 📐PR的建议
+1. 如何配置poocr-config.toml？
 
-python-office欢迎任何人来添砖加瓦，贡献代码，建议提交的pr（pull request）符合一些规范，规范如下：
+第一步，你需要开通腾讯云的发票识别功能（收费功能，很便宜）：[点我直达](https://cloud.tencent.com/act/cps/redirect?redirect=10098&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
 
-参与项目建设的步骤：
-- 例如：你需要给python-office添加一个add方法。
-   1. 你的Github账户名为：demo
-   2. 于是你在./contributors新建了文件夹./demo
-   3. 新建了add.py文件，编辑你的代码
-   4. 编辑完成，提交pr到master分支（gitee或者GitHub，都可以）。可以注明你对自己功能的取名建议
-   5. 晚枫收到后，会对各位的代码进行测试后，合并后打包上传到python官方库
-
-### 📐代码规范
-
-1. 注释完备，尤其每个新增的方法应按照Google Python文档规范标明方法说明、参数说明、返回值说明等信息，必要时请添加单元测试，如果愿意，也可以加上你的大名。
-2. python-office的文档，需要进行格式化。注意：只能格式化你自己的代码
-3. 请直接pull request到`master`分支。`master`是主分支，表示已经发布pypi库的版本。**未来参与人数增多，会开辟新的分支，请留意本文档的更新。**
-4. 我们如果关闭了你的issue或pr，请不要诧异，这是我们保持问题处理整洁的一种方式，你依旧可以继续讨论，当有讨论结果时我们会重新打开。
+第二步，你需要设置一个子账户（不花钱）：[点我直达](https://cloud.tencent.com/act/cps/redirect?redirect=36394&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
+
+如果以上配置，自己不懂技术，难以实现的话，可以付费找我帮你配置。我的微信，点击直达👉[CoderWanFeng](http://python4office.cn/wechat-qrcode/)，99元/次，一次就够了。我有自己的工作，都是打工人，拒绝白嫖哈，多谢理解。
+## 🏗️添砖加瓦
+
+
+### 📐PR的建议
 
+poocr欢迎任何人来添砖加瓦，贡献代码，建议提交的pr（pull request）符合一些规范，规范如下：
 
 ### 🧬贡献代码的步骤
 
 1. 在Gitee或者Github上fork项目到自己的repo
 2. 把fork过去的项目也就是你的项目clone到你的本地
 3. 修改代码
 4. commit后push到自己的库
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poocr Version: 0.0.6 Summary: pip install poocr
+Metadata-Version: 2.1 Name: poocr Version: 0.0.7 Summary: pip install poocr
 Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
 1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
 CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
 CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
 github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
@@ -10,41 +10,34 @@
             ð é¡¹ç®å®ç½ï¼https://www.python-office.com/ ð
                      ð æ¬å¼æºé¡¹ç®çäº¤æµç¾¤ ð
   [https://img.shields.io/badge/QQ-163434413-orange] [https://img.shields.io/
        badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-brightgreen]
 ------------------------------------------------------------------------------
 - ## ðç®ä» poocr æ¯å¿«éè°ç¨è¾è®¯äºAIå¹³å°åè½çæ¥å£åéã
 ``poocr``ææåè½çå®ç°ï¼é½ä¾æäºè¾è®¯äºçæå­è¯å«ï¼å¦ææ¯å°ç½ç¨æ·ï¼å¯ä»¥**æ«ç ä¸å¾ï¼åè´¹å¼é**~
-![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/poocr%2Fapi-
+![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/potencent%2Fapi-
 doc%2Fshare.jpg) --------------------------------------------------------------
 ----------------- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install
 -i https://mirrors.aliyun.com/pypi/simple/ poocr -U ``` -----------------------
--------------------------------------------------------- ## ðåè½
-[ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/
-) ## ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
-WxICBZZSgkm-OrvXB82hbg) ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®® python-
-officeæ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ï¼å»ºè®®æäº¤çprï¼pull
-requestï¼ç¬¦åä¸äºè§èï¼è§èå¦ä¸ï¼ åä¸é¡¹ç®å»ºè®¾çæ­¥éª¤ï¼ -
-ä¾å¦ï¼ä½ éè¦ç»python-officeæ·»å ä¸ä¸ªaddæ¹æ³ã 1.
-ä½ çGithubè´¦æ·åä¸ºï¼demo 2. äºæ¯ä½ å¨./
-contributorsæ°å»ºäºæä»¶å¤¹./demo 3.
-æ°å»ºäºadd.pyæä»¶ï¼ç¼è¾ä½ çä»£ç  4.
-ç¼è¾å®æï¼æäº¤prå°masteråæ¯ï¼giteeæèGitHubï¼é½å¯ä»¥ï¼ãå¯ä»¥æ³¨æä½ å¯¹èªå·±åè½çååå»ºè®®
-5.
-ææ«æ¶å°åï¼ä¼å¯¹åä½çä»£ç è¿è¡æµè¯åï¼åå¹¶åæåä¸ä¼ å°pythonå®æ¹åº
-### ðä»£ç è§è 1.
-æ³¨éå®å¤ï¼å°¤å¶æ¯ä¸ªæ°å¢çæ¹æ³åºæç§Google
-Pythonææ¡£è§èæ ææ¹æ³è¯´æãåæ°è¯´æãè¿åå¼è¯´æç­ä¿¡æ¯ï¼å¿è¦æ¶è¯·æ·»å ååæµè¯ï¼å¦ææ¿æï¼ä¹å¯ä»¥å ä¸ä½ çå¤§åã
-2. python-
-officeçææ¡£ï¼éè¦è¿è¡æ ¼å¼åãæ³¨æï¼åªè½æ ¼å¼åä½ èªå·±çä»£ç 
-3. è¯·ç´æ¥pull
-requestå°`master`åæ¯ã`master`æ¯ä¸»åæ¯ï¼è¡¨ç¤ºå·²ç»åå¸pypiåºççæ¬ã**æªæ¥åä¸äººæ°å¢å¤ï¼ä¼å¼è¾æ°çåæ¯ï¼è¯·çææ¬ææ¡£çæ´æ°ã**
-4.
-æä»¬å¦æå³é­äºä½ çissueæprï¼è¯·ä¸è¦è¯§å¼ï¼è¿æ¯æä»¬ä¿æé®é¢å¤çæ´æ´çä¸ç§æ¹å¼ï¼ä½ ä¾æ§å¯ä»¥ç»§ç»­è®¨è®ºï¼å½æè®¨è®ºç»ææ¶æä»¬ä¼éæ°æå¼ã
-### ð§¬è´¡ç®ä»£ç çæ­¥éª¤ 1.
+-------------------------------------------------------- ## ðåè½ -
+[ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/) -
+ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://www.python-office.com/
+video/poocr.html) ## å¸¸è§é®é¢ 1. å¦ä½éç½®poocr-config.tomlï¼
+ç¬¬ä¸æ­¥ï¼ä½ éè¦å¼éè¾è®¯äºçåç¥¨è¯å«åè½ï¼æ¶è´¹åè½ï¼å¾ä¾¿å®ï¼ï¼
+[ç¹æç´è¾¾](https://cloud.tencent.com/act/cps/
+redirect?redirect=10098&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
+ç¬¬äºæ­¥ï¼ä½ éè¦è®¾ç½®ä¸ä¸ªå­è´¦æ·ï¼ä¸è±é±ï¼ï¼[ç¹æç´è¾¾]
+(https://cloud.tencent.com/act/cps/
+redirect?redirect=36394&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
+å¦æä»¥ä¸éç½®ï¼èªå·±ä¸æææ¯ï¼é¾ä»¥å®ç°çè¯ï¼å¯ä»¥ä»è´¹æ¾æå¸®ä½ éç½®ãæçå¾®ä¿¡ï¼ç¹å»ç´è¾¾ð
+[CoderWanFeng](http://python4office.cn/wechat-qrcode/)ï¼99å/
+æ¬¡ï¼ä¸æ¬¡å°±å¤äºãææèªå·±çå·¥ä½ï¼é½æ¯æå·¥äººï¼æç»ç½å«åï¼å¤è°¢çè§£ã
+## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®®
+poocræ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ï¼å»ºè®®æäº¤çprï¼pull
+requestï¼ç¬¦åä¸äºè§èï¼è§èå¦ä¸ï¼ ### ð§¬è´¡ç®ä»£ç çæ­¥éª¤ 1.
 å¨GiteeæèGithubä¸forké¡¹ç®å°èªå·±çrepo 2.
 æforkè¿å»çé¡¹ç®ä¹å°±æ¯ä½ çé¡¹ç®cloneå°ä½ çæ¬å° 3. ä¿®æ¹ä»£ç 
 4. commitåpushå°èªå·±çåº 5.
 ç»å½GiteeæGithubå¨ä½ é¦é¡µå¯ä»¥çå°ä¸ä¸ª pull request
 æé®ï¼ç¹å»å®ï¼å¡«åä¸äºè¯´æä¿¡æ¯ï¼ç¶åæäº¤å°masteråæ¯å³å¯ã
 6. ç­å¾ç»´æ¤èåå¹¶ ### ðæä¾bugåé¦æå»ºè®®
 æäº¤é®é¢åé¦æ¶ï¼è¯·å¡å¿å¡«ååpython-
```

### Comparing `poocr-0.0.6/README.md` & `poocr-0.0.7/poocr.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: poocr
+Version: 0.0.7
+Summary: pip install poocr
+Home-page: https://www.python-office.com/
+Author: CoderWanFeng
+Author-email: 1957875073@qq.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/CoderWanFeng/poocr/issues
+Project-URL: Documentation, https://github.com/CoderWanFeng/poocr/blob/main/README.md
+Project-URL: Source Code, https://github.com/CoderWanFeng/poocr
+Platform: any
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 <p align="center">
     <a target="_blank" href='https://url.cn/Z4lzPLaF'>
     <img src="https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-tencent.jpg" width="100%"/>
     </a>   
 </p>
 
@@ -31,15 +47,15 @@
 ## 📚简介
 
 
 poocr 是快速调用腾讯云AI平台功能的接口合集。
 
 ``poocr``所有功能的实现，都依托于腾讯云的文字识别，如果是小白用户，可以**扫码下图，免费开通**~
 
-![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/poocr%2Fapi-doc%2Fshare.jpg)
+![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/potencent%2Fapi-doc%2Fshare.jpg)
 
 -------------------------------------------------------------------------------
 
 ## 📦安装
 
 ### 🍊pip 自动下载&更新
 
@@ -48,40 +64,34 @@
 ```
 
 
 -------------------------------------------------------------------------------
 
 ## 📝功能
 
-[📘官网：https://www.python-office.com/](https://www.python-office.com/)
+- [📘官网：https://www.python-office.com/](https://www.python-office.com/)
 
-## 💻所有功能的列表👉[点我直达](https://mp.weixin.qq.com/s/WxICBZZSgkm-OrvXB82hbg)
+-  💻所有功能的列表👉[点我直达](https://www.python-office.com/video/poocr.html)
 
-## 🏗️添砖加瓦
 
+## 常见问题
 
-### 📐PR的建议
+1. 如何配置poocr-config.toml？
+
+第一步，你需要开通腾讯云的发票识别功能（收费功能，很便宜）：[点我直达](https://cloud.tencent.com/act/cps/redirect?redirect=10098&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
 
-python-office欢迎任何人来添砖加瓦，贡献代码，建议提交的pr（pull request）符合一些规范，规范如下：
+第二步，你需要设置一个子账户（不花钱）：[点我直达](https://cloud.tencent.com/act/cps/redirect?redirect=36394&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
 
-参与项目建设的步骤：
-- 例如：你需要给python-office添加一个add方法。
-   1. 你的Github账户名为：demo
-   2. 于是你在./contributors新建了文件夹./demo
-   3. 新建了add.py文件，编辑你的代码
-   4. 编辑完成，提交pr到master分支（gitee或者GitHub，都可以）。可以注明你对自己功能的取名建议
-   5. 晚枫收到后，会对各位的代码进行测试后，合并后打包上传到python官方库
-
-### 📐代码规范
-
-1. 注释完备，尤其每个新增的方法应按照Google Python文档规范标明方法说明、参数说明、返回值说明等信息，必要时请添加单元测试，如果愿意，也可以加上你的大名。
-2. python-office的文档，需要进行格式化。注意：只能格式化你自己的代码
-3. 请直接pull request到`master`分支。`master`是主分支，表示已经发布pypi库的版本。**未来参与人数增多，会开辟新的分支，请留意本文档的更新。**
-4. 我们如果关闭了你的issue或pr，请不要诧异，这是我们保持问题处理整洁的一种方式，你依旧可以继续讨论，当有讨论结果时我们会重新打开。
+如果以上配置，自己不懂技术，难以实现的话，可以付费找我帮你配置。我的微信，点击直达👉[CoderWanFeng](http://python4office.cn/wechat-qrcode/)，99元/次，一次就够了。我有自己的工作，都是打工人，拒绝白嫖哈，多谢理解。
+## 🏗️添砖加瓦
+
+
+### 📐PR的建议
 
+poocr欢迎任何人来添砖加瓦，贡献代码，建议提交的pr（pull request）符合一些规范，规范如下：
 
 ### 🧬贡献代码的步骤
 
 1. 在Gitee或者Github上fork项目到自己的repo
 2. 把fork过去的项目也就是你的项目clone到你的本地
 3. 修改代码
 4. commit后push到自己的库
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
+Metadata-Version: 2.1 Name: poocr Version: 0.0.7 Summary: pip install poocr
+Home-page: https://www.python-office.com/ Author: CoderWanFeng Author-email:
+1957875073@qq.com License: MIT Project-URL: Bug Tracker, https://github.com/
+CoderWanFeng/poocr/issues Project-URL: Documentation, https://github.com/
+CoderWanFeng/poocr/blob/main/README.md Project-URL: Source Code, https://
+github.com/CoderWanFeng/poocr Platform: any Requires-Python: >=3.7 Description-
+Content-Type: text/markdown License-File: LICENSE
 [https://website-python-1300615378.cos.ap-nanjing.myqcloud.com/ads%2F1040x100-
                                  tencent.jpg]
             ð é¡¹ç®å®ç½ï¼https://www.python-office.com/ ð
                      ð æ¬å¼æºé¡¹ç®çäº¤æµç¾¤ ð
   [https://img.shields.io/badge/QQ-163434413-orange] [https://img.shields.io/
        badge/%E5%BE%AE%E4%BF%A1-%E4%BA%A4%E6%B5%81%E7%BE%A4-brightgreen]
 ------------------------------------------------------------------------------
 - ## ðç®ä» poocr æ¯å¿«éè°ç¨è¾è®¯äºAIå¹³å°åè½çæ¥å£åéã
 ``poocr``ææåè½çå®ç°ï¼é½ä¾æäºè¾è®¯äºçæå­è¯å«ï¼å¦ææ¯å°ç½ç¨æ·ï¼å¯ä»¥**æ«ç ä¸å¾ï¼åè´¹å¼é**~
-![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/poocr%2Fapi-
+![](https://article-1300615378.cos.ap-nanjing.myqcloud.com/potencent%2Fapi-
 doc%2Fshare.jpg) --------------------------------------------------------------
 ----------------- ## ð¦å®è£ ### ðpip èªå¨ä¸è½½&æ´æ° ``` pip install
 -i https://mirrors.aliyun.com/pypi/simple/ poocr -U ``` -----------------------
--------------------------------------------------------- ## ðåè½
-[ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/
-) ## ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://mp.weixin.qq.com/s/
-WxICBZZSgkm-OrvXB82hbg) ## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®® python-
-officeæ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ï¼å»ºè®®æäº¤çprï¼pull
-requestï¼ç¬¦åä¸äºè§èï¼è§èå¦ä¸ï¼ åä¸é¡¹ç®å»ºè®¾çæ­¥éª¤ï¼ -
-ä¾å¦ï¼ä½ éè¦ç»python-officeæ·»å ä¸ä¸ªaddæ¹æ³ã 1.
-ä½ çGithubè´¦æ·åä¸ºï¼demo 2. äºæ¯ä½ å¨./
-contributorsæ°å»ºäºæä»¶å¤¹./demo 3.
-æ°å»ºäºadd.pyæä»¶ï¼ç¼è¾ä½ çä»£ç  4.
-ç¼è¾å®æï¼æäº¤prå°masteråæ¯ï¼giteeæèGitHubï¼é½å¯ä»¥ï¼ãå¯ä»¥æ³¨æä½ å¯¹èªå·±åè½çååå»ºè®®
-5.
-ææ«æ¶å°åï¼ä¼å¯¹åä½çä»£ç è¿è¡æµè¯åï¼åå¹¶åæåä¸ä¼ å°pythonå®æ¹åº
-### ðä»£ç è§è 1.
-æ³¨éå®å¤ï¼å°¤å¶æ¯ä¸ªæ°å¢çæ¹æ³åºæç§Google
-Pythonææ¡£è§èæ ææ¹æ³è¯´æãåæ°è¯´æãè¿åå¼è¯´æç­ä¿¡æ¯ï¼å¿è¦æ¶è¯·æ·»å ååæµè¯ï¼å¦ææ¿æï¼ä¹å¯ä»¥å ä¸ä½ çå¤§åã
-2. python-
-officeçææ¡£ï¼éè¦è¿è¡æ ¼å¼åãæ³¨æï¼åªè½æ ¼å¼åä½ èªå·±çä»£ç 
-3. è¯·ç´æ¥pull
-requestå°`master`åæ¯ã`master`æ¯ä¸»åæ¯ï¼è¡¨ç¤ºå·²ç»åå¸pypiåºççæ¬ã**æªæ¥åä¸äººæ°å¢å¤ï¼ä¼å¼è¾æ°çåæ¯ï¼è¯·çææ¬ææ¡£çæ´æ°ã**
-4.
-æä»¬å¦æå³é­äºä½ çissueæprï¼è¯·ä¸è¦è¯§å¼ï¼è¿æ¯æä»¬ä¿æé®é¢å¤çæ´æ´çä¸ç§æ¹å¼ï¼ä½ ä¾æ§å¯ä»¥ç»§ç»­è®¨è®ºï¼å½æè®¨è®ºç»ææ¶æä»¬ä¼éæ°æå¼ã
-### ð§¬è´¡ç®ä»£ç çæ­¥éª¤ 1.
+-------------------------------------------------------- ## ðåè½ -
+[ðå®ç½ï¼https://www.python-office.com/](https://www.python-office.com/) -
+ð»ææåè½çåè¡¨ð[ç¹æç´è¾¾](https://www.python-office.com/
+video/poocr.html) ## å¸¸è§é®é¢ 1. å¦ä½éç½®poocr-config.tomlï¼
+ç¬¬ä¸æ­¥ï¼ä½ éè¦å¼éè¾è®¯äºçåç¥¨è¯å«åè½ï¼æ¶è´¹åè½ï¼å¾ä¾¿å®ï¼ï¼
+[ç¹æç´è¾¾](https://cloud.tencent.com/act/cps/
+redirect?redirect=10098&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
+ç¬¬äºæ­¥ï¼ä½ éè¦è®¾ç½®ä¸ä¸ªå­è´¦æ·ï¼ä¸è±é±ï¼ï¼[ç¹æç´è¾¾]
+(https://cloud.tencent.com/act/cps/
+redirect?redirect=36394&cps_key=ca76be5a2293ba3906d6d5407aea15ee)
+å¦æä»¥ä¸éç½®ï¼èªå·±ä¸æææ¯ï¼é¾ä»¥å®ç°çè¯ï¼å¯ä»¥ä»è´¹æ¾æå¸®ä½ éç½®ãæçå¾®ä¿¡ï¼ç¹å»ç´è¾¾ð
+[CoderWanFeng](http://python4office.cn/wechat-qrcode/)ï¼99å/
+æ¬¡ï¼ä¸æ¬¡å°±å¤äºãææèªå·±çå·¥ä½ï¼é½æ¯æå·¥äººï¼æç»ç½å«åï¼å¤è°¢çè§£ã
+## ðï¸æ·»ç å ç¦ ### ðPRçå»ºè®®
+poocræ¬¢è¿ä»»ä½äººæ¥æ·»ç å ç¦ï¼è´¡ç®ä»£ç ï¼å»ºè®®æäº¤çprï¼pull
+requestï¼ç¬¦åä¸äºè§èï¼è§èå¦ä¸ï¼ ### ð§¬è´¡ç®ä»£ç çæ­¥éª¤ 1.
 å¨GiteeæèGithubä¸forké¡¹ç®å°èªå·±çrepo 2.
 æforkè¿å»çé¡¹ç®ä¹å°±æ¯ä½ çé¡¹ç®cloneå°ä½ çæ¬å° 3. ä¿®æ¹ä»£ç 
 4. commitåpushå°èªå·±çåº 5.
 ç»å½GiteeæGithubå¨ä½ é¦é¡µå¯ä»¥çå°ä¸ä¸ª pull request
 æé®ï¼ç¹å»å®ï¼å¡«åä¸äºè¯´æä¿¡æ¯ï¼ç¶åæäº¤å°masteråæ¯å³å¯ã
 6. ç­å¾ç»´æ¤èåå¹¶ ### ðæä¾bugåé¦æå»ºè®®
 æäº¤é®é¢åé¦æ¶ï¼è¯·å¡å¿å¡«ååpython-
```

### Comparing `poocr-0.0.6/poocr/__init__.py` & `poocr-0.0.7/poocr/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,9 +3,9 @@
 from poocr.lib.Const import SPLIT_LINE
 
 print(SPLIT_LINE)
 print('【poocr库】，功能持续更新中')
 print('使用有问题 or 提交你的功能需求 or 参与项目开发')
 print('1、全部功能【视频 & 文字】教程：https://mp.weixin.qq.com/s/WxICBZZSgkm-OrvXB82hbg')
 print('2、请+【项目交流群】：http://t.cn/A65MiFvH')
-print('3、本开源项目的【代码仓库】：https://github.com/CoderWanFeng/poocr')
+print('3、本开源项目的【代码仓库】：https://gitee.com/CoderWanFeng/poocr')
 print(SPLIT_LINE)
```

### Comparing `poocr-0.0.6/poocr/api/ocr.py` & `poocr-0.0.7/poocr/api/ocr.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.6/poocr/api/ocr2excel.py` & `poocr-0.0.7/poocr/api/ocr2excel.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.6/poocr/core/OCR.py` & `poocr-0.0.7/poocr/core/OCR.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.6/poocr/lib/CommonUtils.py` & `poocr-0.0.7/poocr/lib/CommonUtils.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.6/poocr/lib/Config.py` & `poocr-0.0.7/poocr/lib/Config.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.6/poocr/lib/Const.py` & `poocr-0.0.7/poocr/lib/Const.py`

 * *Files identical despite different names*

### Comparing `poocr-0.0.6/setup.cfg` & `poocr-0.0.7/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f6f 6372 0d0a 7665 7273 696f   = poocr..versio
-00000020: 6e20 3d20 302e 302e 360d 0a64 6573 6372  n = 0.0.6..descr
+00000020: 6e20 3d20 302e 302e 370d 0a64 6573 6372  n = 0.0.7..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f6f 6372 0d0a 6c6f 6e67  tall poocr..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
@@ -32,15 +32,16 @@
 000001f0: 6d2f 436f 6465 7257 616e 4665 6e67 2f70  m/CoderWanFeng/p
 00000200: 6f6f 6372 0d0a 0d0a 5b6f 7074 696f 6e73  oocr....[options
 00000210: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
 00000220: 6e64 3a0d 0a69 6e73 7461 6c6c 5f72 6571  nd:..install_req
 00000230: 7569 7265 7320 3d20 0d0a 0974 6f6d 6c0d  uires = ...toml.
 00000240: 0a09 7465 6e63 656e 7463 6c6f 7564 2d73  ..tencentcloud-s
 00000250: 646b 2d70 7974 686f 6e0d 0a09 706f 7072  dk-python...popr
-00000260: 6f67 7265 7373 0d0a 7079 7468 6f6e 5f72  ogress..python_r
-00000270: 6571 7569 7265 7320 3d20 3e3d 332e 370d  equires = >=3.7.
-00000280: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
-00000290: 5f64 6174 6120 3d20 5472 7565 0d0a 7a69  _data = True..zi
-000002a0: 705f 7361 6665 203d 2046 616c 7365 0d0a  p_safe = False..
-000002b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000002c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-000002d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000260: 6f67 7265 7373 0d0a 0970 6f66 696c 650d  ogress...pofile.
+00000270: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000280: 203d 203e 3d33 2e37 0d0a 696e 636c 7564   = >=3.7..includ
+00000290: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
+000002a0: 2054 7275 650d 0a7a 6970 5f73 6166 6520   True..zip_safe 
+000002b0: 3d20 4661 6c73 650d 0a0d 0a5b 6567 675f  = False....[egg_
+000002c0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+000002d0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+000002e0: 300d 0a0d 0a                             0....
```

### Comparing `poocr-0.0.6/tests/test_tencent.py` & `poocr-0.0.7/tests/test_tencent.py`

 * *Files identical despite different names*

