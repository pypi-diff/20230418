# Comparing `tmp/anticaptchaofficial-1.0.49-py3-none-any.whl.zip` & `tmp/anticaptchaofficial-1.0.50-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 17174 bytes, number of entries: 23
+Zip file size: 17259 bytes, number of entries: 23
 -rw-r--r--  2.0 unx      172 b- defN 20-Mar-11 07:55 anticaptchaofficial/__init__.py
 -rw-r--r--  2.0 unx     1013 b- defN 23-Jan-07 03:37 anticaptchaofficial/antibotcookietask.py
 -rw-r--r--  2.0 unx     2720 b- defN 22-Sep-27 14:01 anticaptchaofficial/antigatetask.py
 -rw-r--r--  2.0 unx     6467 b- defN 22-Jun-01 07:45 anticaptchaofficial/antinetworking.py
 -rw-r--r--  2.0 unx     1149 b- defN 22-Jun-01 07:46 anticaptchaofficial/funcaptchaproxyless.py
 -rw-r--r--  2.0 unx     1430 b- defN 22-Jun-01 07:46 anticaptchaofficial/funcaptchaproxyon.py
 -rw-r--r--  2.0 unx     1619 b- defN 22-Jun-01 07:46 anticaptchaofficial/geetestproxyless.py
@@ -12,14 +12,14 @@
 -rw-r--r--  2.0 unx     1176 b- defN 22-Jun-01 07:46 anticaptchaofficial/imagecaptcha.py
 -rw-r--r--  2.0 unx      956 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2enterpriseproxyless.py
 -rw-r--r--  2.0 unx     1278 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2enterpriseproxyon.py
 -rw-r--r--  2.0 unx     1045 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2proxyless.py
 -rw-r--r--  2.0 unx     1339 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2proxyon.py
 -rw-r--r--  2.0 unx     1318 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav3enterpriseproxyless.py
 -rw-r--r--  2.0 unx     1270 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav3proxyless.py
--rw-r--r--  2.0 unx      826 b- defN 22-Nov-02 07:37 anticaptchaofficial/turnstileproxyless.py
--rw-r--r--  2.0 unx     1135 b- defN 22-Nov-02 07:37 anticaptchaofficial/turnstileproxyon.py
--rw-r--r--  2.0 unx     9673 b- defN 23-Apr-14 03:43 anticaptchaofficial-1.0.49.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 03:43 anticaptchaofficial-1.0.49.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Apr-14 03:43 anticaptchaofficial-1.0.49.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2208 b- defN 23-Apr-14 03:43 anticaptchaofficial-1.0.49.dist-info/RECORD
-23 files, 41512 bytes uncompressed, 13488 bytes compressed:  67.5%
+-rw-r--r--  2.0 unx      943 b- defN 23-Apr-18 07:44 anticaptchaofficial/turnstileproxyless.py
+-rw-r--r--  2.0 unx     1252 b- defN 23-Apr-18 07:44 anticaptchaofficial/turnstileproxyon.py
+-rw-r--r--  2.0 unx     9734 b- defN 23-Apr-18 07:46 anticaptchaofficial-1.0.50.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 07:46 anticaptchaofficial-1.0.50.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-18 07:46 anticaptchaofficial-1.0.50.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2208 b- defN 23-Apr-18 07:46 anticaptchaofficial-1.0.50.dist-info/RECORD
+23 files, 41807 bytes uncompressed, 13573 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: anticaptchaofficial/turnstileproxyless.py
 Comment: 
 
 Filename: anticaptchaofficial/turnstileproxyon.py
 Comment: 
 
-Filename: anticaptchaofficial-1.0.49.dist-info/METADATA
+Filename: anticaptchaofficial-1.0.50.dist-info/METADATA
 Comment: 
 
-Filename: anticaptchaofficial-1.0.49.dist-info/WHEEL
+Filename: anticaptchaofficial-1.0.50.dist-info/WHEEL
 Comment: 
 
-Filename: anticaptchaofficial-1.0.49.dist-info/top_level.txt
+Filename: anticaptchaofficial-1.0.50.dist-info/top_level.txt
 Comment: 
 
-Filename: anticaptchaofficial-1.0.49.dist-info/RECORD
+Filename: anticaptchaofficial-1.0.50.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anticaptchaofficial/turnstileproxyless.py

```diff
@@ -1,18 +1,24 @@
 from anticaptchaofficial.antinetworking import *
 import time
 
 
 class turnstileProxyless(antiNetworking):
 
+    action = '';
+
+    def set_action(self, action):
+        self.action = action
+
     def solve_and_return_solution(self):
         task = {
             "type": "TurnstileTaskProxyless",
             "websiteURL": self.website_url,
-            "websiteKey": self.website_key
+            "websiteKey": self.website_key,
+            "action": self.action
         }
         if self.create_task({
             "clientKey": self.client_key,
             "task": task,
             "softId": self.soft_id
         }) == 1:
             self.log("created task with id "+str(self.task_id))
```

## anticaptchaofficial/turnstileproxyon.py

```diff
@@ -1,18 +1,24 @@
 from anticaptchaofficial.antinetworking import *
 import time
 
 
 class turnstileProxyon(antiNetworking):
 
+    action = '';
+
+    def set_action(self, action):
+        self.action = action
+
     def solve_and_return_solution(self):
         task = {
             "type": "TurnstileTask",
             "websiteURL": self.website_url,
             "websiteKey": self.website_key,
+            "action": self.action,
             "proxyType": self.proxy_type,
             "proxyAddress": self.proxy_address,
             "proxyPort": self.proxy_port,
             "proxyLogin": self.proxy_login,
             "proxyPassword": self.proxy_password
         }
         if self.is_invisible:
```

## Comparing `anticaptchaofficial-1.0.49.dist-info/METADATA` & `anticaptchaofficial-1.0.50.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anticaptchaofficial
-Version: 1.0.49
+Version: 1.0.50
 Summary: Official anti-captcha.com library
 Home-page: https://github.com/AdminAnticaptcha/anticaptcha-python
 Author: Anti Admin
 Author-email: admin@anti-captcha.com
 License: MIT
 Keywords: anticaptcha anti captcha recognition solve bypass recaptcha enterprise funcaptcha arkoselabs geetest hcaptcha antigate turnstile
 Platform: UNKNOWN
@@ -231,14 +231,17 @@
 
 solver = turnstileProxyless()
 solver.set_verbose(1)
 solver.set_key("YOUR_API_KEY")
 solver.set_website_url("https://website.com")
 solver.set_website_key("SITE_KEY")
 
+# Optionally specify page action
+solver.set_action("login")
+
 # Specify softId to earn 10% commission with your app.
 # Get your softId here: https://anti-captcha.com/clients/tools/devcenter
 solver.set_soft_id(0)
 
 token = solver.solve_and_return_solution()
 if token != 0:
     print "token: "+token
```

## Comparing `anticaptchaofficial-1.0.49.dist-info/RECORD` & `anticaptchaofficial-1.0.50.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 anticaptchaofficial/imagecaptcha.py,sha256=aKupUYdeNjuQanbY4aI8TuK6uty32e8XzP0Uzg3RL7I,1176
 anticaptchaofficial/recaptchav2enterpriseproxyless.py,sha256=XnDx-6-KsETqXySaT0RDWtuh-9Sk3gSWy2rF8Jy1gLk,956
 anticaptchaofficial/recaptchav2enterpriseproxyon.py,sha256=p7sdV0qHScbrIrhw00624pH_2hQeG95RTGjRQDutxs4,1278
 anticaptchaofficial/recaptchav2proxyless.py,sha256=12fviOgw1waeeRbyzwvSctIoc1w3qCBYJY7GYi0FSJc,1045
 anticaptchaofficial/recaptchav2proxyon.py,sha256=KKjm72dfxdCChyj3Qn5y5Twm8qT3sZsvSGSfjbdrIM8,1339
 anticaptchaofficial/recaptchav3enterpriseproxyless.py,sha256=exQ-sgvOdcSpsh0mWsUDKEGudM4k23SrROVZ9p0pU5M,1318
 anticaptchaofficial/recaptchav3proxyless.py,sha256=Fv0nfDG-Jp8Vzz8C4-vccz3BJ0hm89MTAs3y9Okzctw,1270
-anticaptchaofficial/turnstileproxyless.py,sha256=k12CETrs6iRhZj3shXrOZrCf8EBvFodXcRa3N6rXKJU,826
-anticaptchaofficial/turnstileproxyon.py,sha256=6yx5EBxQgi2m4yfvkichbZNB87xMg9LveApeKYVLkII,1135
-anticaptchaofficial-1.0.49.dist-info/METADATA,sha256=P9V50kSHTVatlsw54bFXUcoTBmm3sfsTSblBbpHNsJk,9673
-anticaptchaofficial-1.0.49.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-anticaptchaofficial-1.0.49.dist-info/top_level.txt,sha256=lLc0em6A2B5BH-M8v9OP54jTh3u65A4xb2trGoI2_5A,20
-anticaptchaofficial-1.0.49.dist-info/RECORD,,
+anticaptchaofficial/turnstileproxyless.py,sha256=nK737Ccr8mZy0_CL6_gB1P5UiCWLaJ0gM9SoCVshMpg,943
+anticaptchaofficial/turnstileproxyon.py,sha256=0HpomUlH1PuLglzrtMBEu5R4287oE3cpp3QnsDhfF2k,1252
+anticaptchaofficial-1.0.50.dist-info/METADATA,sha256=sbParzvrDYFwruti_fIlN2Yr1IYmnSEP0b8tF6n7dhY,9734
+anticaptchaofficial-1.0.50.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+anticaptchaofficial-1.0.50.dist-info/top_level.txt,sha256=lLc0em6A2B5BH-M8v9OP54jTh3u65A4xb2trGoI2_5A,20
+anticaptchaofficial-1.0.50.dist-info/RECORD,,
```

